# Comparing `tmp/nlp2cron-0.1.1.tar.gz` & `tmp/nlp2cron-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp2cron-0.1.1.tar", max compression
+gzip compressed data, was "nlp2cron-0.1.3.tar", max compression
```

## Comparing `nlp2cron-0.1.1.tar` & `nlp2cron-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      373 2023-04-11 03:35:14.927410 nlp2cron-0.1.1/README.md
--rw-r--r--   0        0        0    10385 2023-04-11 03:33:50.638817 nlp2cron-0.1.1/nlp2cron.py
--rw-r--r--   0        0        0      306 2023-04-11 03:35:35.081311 nlp2cron-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nlp2cron-0.1.1/setup.py
--rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 nlp2cron-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      373 2023-04-11 03:35:14.927410 nlp2cron-0.1.3/README.md
+-rw-r--r--   0        0        0    10579 2023-04-11 07:08:44.515197 nlp2cron-0.1.3/nlp2cron.py
+-rw-r--r--   0        0        0      306 2023-04-11 07:10:56.505538 nlp2cron-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nlp2cron-0.1.3/setup.py
+-rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 nlp2cron-0.1.3/PKG-INFO
```

### Comparing `nlp2cron-0.1.1/nlp2cron.py` & `nlp2cron-0.1.3/nlp2cron.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,32 +100,34 @@
         else:
             return False
 
     def extract_freq(self):
         if '每个月' in self.message: self.message = self.message.replace('个', '')
         if '每月' in self.message:
             self.dict['month'] = '*'
-            mindex = self.message.index("每月")
-            tmp = self.message[mindex:]
-            day = re.findall(r'(\d+)', tmp)
-            if day: self.dict['day'] = str(day[0])
-            else: self.dict['day'] = str(1)
+            day = re.findall(r'每月(\d{1,2})', self.message)
+            if day: 
+                self.dict['day'] = str(day[0])
+            elif '最后1天' in self.message:
+                self.dict['day'] = 'L'
+            else:
+                self.dict['day'] = '1'
 
         wk = re.findall(r'每月周(\d{1})', self.message)
         if wk:
             ## 就是没有周几去干嘛
             self.dict['week'] = wk[0]
             self.dict['day'] = '*'
 
         elif '每周' in self.message:
-            mindex = self.message.index("每周")
-            tmp = self.message[mindex:]
-            day = re.findall(r'(\d{1})', tmp)
-            if day: self.dict['week'] = str(day[0])
-            else: self.dict['week'] = '1'
+            if '每周日' in self.message: self.dict['week'] = '0'
+            wd = re.findall(r'每周(\d{1})', self.message)
+            if wd:
+                week = wd[0]
+                self.dict['week'] = week
 
         elif '每天' in self.message:
             self.dict['day'] = '*'
 
         if '点' in self.message:
                 hour = re.findall(r'(\d{1}|\d{2})点', self.message)
                 if hour: 
@@ -162,15 +164,15 @@
 
         if self.dict['day'] == '29':
             ## 判断是不是有闰年，如果是闰年，则改29为28
             year = self.now.year
             if self.is_leap_year(year):
                 self.dict['day'] = '28'
 
-        if '月末' in self.message or '月底' in self.message or '最后一天' in self.message:
+        if ('月末' in self.message) or ('月底' in self.message) or ('最后一天' in self.message):
             self.dict['day'] = 'L'
 
         if '点半' in self.message:
             self.dict['min'] = '30'
 
         if '点' in self.message and '分' not in self.message and '点半' not in self.message:
             min = re.findall(r'点(\d+)', self.message)
@@ -265,14 +267,17 @@
                 '每月周五10点30去爬山',
                 '每周五早上10点25分写周报',
                 '每周五下午3点发送邮件',
                 '每天早上6点定时备份数据库',
                 '每月1号凌晨2点清理日志',
                 '每个月3号10点35去南京',
                 '每小时执行一次备份',
-                '每个月1号凌晨2点清理日志'
+                '每个月1号凌晨2点清理日志',
+                '每个月最后一天12点20分去散步',
+                '每周日10点去散步',
+                '每周五下午6点10分去散步'
 
     ]
 
     for task in tasks:
         crontab = nlp2cron(task)
         print(task + ': ' + str(crontab))
```

### Comparing `nlp2cron-0.1.1/setup.py` & `nlp2cron-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 modules = \
 ['nlp2cron']
 install_requires = \
 ['cn2an>=0.5.19,<0.6.0']
 
 setup_kwargs = {
     'name': 'nlp2cron',
-    'version': '0.1.1',
+    'version': '0.1.3',
     'description': 'Nature language to cron',
     'long_description': '## 中文自然语言转CRON\n\npip install nlp2cron\n\n```python\nfrom nlp2cron import nlp2cron\ncron = nlp2cron("每天10点25分叫我去买菜")\n\n```\n\n你会得到一个`cron`表达式. 目前代码写的有点乱, 但只要不太随意的自然语言都可以解决\n代码里面有一些例子, 详细看代码啦. 代码写的比较随意, 如果要求高请不要用啦.\n\n',
     'author': 'quqinglei',
     'author_email': 'quqinglei@icloud.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `nlp2cron-0.1.1/PKG-INFO` & `nlp2cron-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp2cron
-Version: 0.1.1
+Version: 0.1.3
 Summary: Nature language to cron
 Author: quqinglei
 Author-email: quqinglei@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

