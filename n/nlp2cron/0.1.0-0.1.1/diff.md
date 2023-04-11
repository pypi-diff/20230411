# Comparing `tmp/nlp2cron-0.1.0.tar.gz` & `tmp/nlp2cron-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp2cron-0.1.0.tar", max compression
+gzip compressed data, was "nlp2cron-0.1.1.tar", max compression
```

## Comparing `nlp2cron-0.1.0.tar` & `nlp2cron-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      217 2023-04-11 03:15:22.870066 nlp2cron-0.1.0/README.md
--rw-r--r--   0        0        0     9788 2023-04-11 03:14:09.178459 nlp2cron-0.1.0/nlp2cron.py
--rw-r--r--   0        0        0      306 2023-04-11 03:11:30.731177 nlp2cron-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 nlp2cron-0.1.0/setup.py
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 nlp2cron-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      373 2023-04-11 03:35:14.927410 nlp2cron-0.1.1/README.md
+-rw-r--r--   0        0        0    10385 2023-04-11 03:33:50.638817 nlp2cron-0.1.1/nlp2cron.py
+-rw-r--r--   0        0        0      306 2023-04-11 03:35:35.081311 nlp2cron-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nlp2cron-0.1.1/setup.py
+-rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 nlp2cron-0.1.1/PKG-INFO
```

### Comparing `nlp2cron-0.1.0/nlp2cron.py` & `nlp2cron-0.1.1/nlp2cron.py`

 * *Files 3% similar despite different names*

```diff
@@ -203,26 +203,42 @@
         if (month == '*' or month in ('2', '4', '6', '9', '11')) and day not in ('*', 'L'):
             if int(day) > 30: return None
 
         return True
 
     def crontab(self):
         if self.a1 or self.a2:
-
             ## 从分开始判断
             ### 判断数字是否合法
             ck = self.check(self.dict['min'], self.dict['hour'], self.dict['day'], self.dict['month'], self.dict['week'])
             if ck is None: return None
             cron = str(self.dict['min']) + ' ' + str(self.dict['hour']) + ' ' + str(self.dict['day']) + \
                 ' ' + str(self.dict['month']) + ' ' + str(self.dict['week']) + ' ' + str(self.freq)
             return cron
         return None
 
+    def cron(self):
+        if self.a1 or self.a2:
+            ## 从分开始判断
+            ### 判断数字是否合法
+            ck = self.check(self.dict['min'], self.dict['hour'], self.dict['day'], self.dict['month'], self.dict['week'])
+            if ck is None: return None
+            cron = str(self.dict['min']) + ' ' + str(self.dict['hour']) + ' ' + str(self.dict['day']) + \
+                ' ' + str(self.dict['month']) + ' ' + str(self.dict['week'])
+            return cron
+        return None
+
+
+
 def nlp2cron(message):
     nlpcron= NLPCron(message)
+    return nlpcron.cron()
+
+def nlp2crons(message):
+    nlpcron= NLPCron(message)
     return nlpcron.crontab()
 
 
 if __name__ == '__main__':
     tasks = [
                 '明天要去医院看病，要带上病历和身份证。',
                 '下周二是最后一天交作业，要抓紧时间写作。',
```

