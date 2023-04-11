# Comparing `tmp/query_toolkits-1.1.8.tar.gz` & `tmp/query_toolkits-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/query_toolkits-1.1.8.tar", last modified: Fri Mar 24 02:48:33 2023, max compression
+gzip compressed data, was "dist/query_toolkits-1.1.9.tar", last modified: Wed Mar 29 03:10:16 2023, max compression
```

## Comparing `query_toolkits-1.1.8.tar` & `query_toolkits-1.1.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 datagrand   (501) staff       (20)        0 2023-03-24 02:48:33.000000 query_toolkits-1.1.8/
--rw-r--r--   0 datagrand   (501) staff       (20)     6148 2023-03-24 02:47:23.000000 query_toolkits-1.1.8/.DS_Store
--rw-r--r--   0 datagrand   (501) staff       (20)       35 2022-08-12 09:08:51.000000 query_toolkits-1.1.8/MANIFEST.in
--rw-r--r--   0 datagrand   (501) staff       (20)      197 2023-03-24 02:48:33.000000 query_toolkits-1.1.8/PKG-INFO
-drwxr-xr-x   0 datagrand   (501) staff       (20)        0 2023-03-24 02:48:33.000000 query_toolkits-1.1.8/query_toolkits/
--rw-r--r--   0 datagrand   (501) staff       (20)      486 2023-03-24 02:46:16.000000 query_toolkits-1.1.8/query_toolkits/__init__.py
--rw-r--r--   0 datagrand   (501) staff       (20)    40837 2022-11-12 10:20:35.000000 query_toolkits-1.1.8/query_toolkits/error_correction.py
--rw-r--r--   0 datagrand   (501) staff       (20)    23157 2023-03-24 02:43:02.000000 query_toolkits-1.1.8/query_toolkits/extractor.py
--rw-r--r--   0 datagrand   (501) staff       (20)      658 2023-03-20 09:28:22.000000 query_toolkits-1.1.8/query_toolkits/financial_index.txt
--rw-r--r--   0 datagrand   (501) staff       (20)  1056198 2023-02-27 08:08:44.000000 query_toolkits-1.1.8/query_toolkits/fund_product.txt
--rw-r--r--   0 datagrand   (501) staff       (20)      153 2022-10-10 04:02:17.000000 query_toolkits-1.1.8/query_toolkits/keyword.txt
--rw-r--r--   0 datagrand   (501) staff       (20)   634483 2022-10-12 02:15:14.000000 query_toolkits-1.1.8/query_toolkits/organization.txt
--rw-r--r--   0 datagrand   (501) staff       (20)     2237 2022-08-15 03:50:09.000000 query_toolkits-1.1.8/query_toolkits/unit_transform
--rw-r--r--   0 datagrand   (501) staff       (20)     5166 2023-03-24 02:37:00.000000 query_toolkits-1.1.8/query_toolkits/utils.py
--rw-------   0 datagrand   (501) staff       (20)   420676 2022-10-20 07:33:48.000000 query_toolkits-1.1.8/query_toolkits/weapon.txt
-drwxr-xr-x   0 datagrand   (501) staff       (20)        0 2023-03-24 02:48:33.000000 query_toolkits-1.1.8/query_toolkits.egg-info/
--rw-r--r--   0 datagrand   (501) staff       (20)      197 2023-03-24 02:48:33.000000 query_toolkits-1.1.8/query_toolkits.egg-info/PKG-INFO
--rw-r--r--   0 datagrand   (501) staff       (20)      495 2023-03-24 02:48:33.000000 query_toolkits-1.1.8/query_toolkits.egg-info/SOURCES.txt
--rw-r--r--   0 datagrand   (501) staff       (20)        1 2023-03-24 02:48:33.000000 query_toolkits-1.1.8/query_toolkits.egg-info/dependency_links.txt
--rw-r--r--   0 datagrand   (501) staff       (20)       15 2023-03-24 02:48:33.000000 query_toolkits-1.1.8/query_toolkits.egg-info/top_level.txt
--rw-r--r--   0 datagrand   (501) staff       (20)        0 2022-08-12 09:05:37.000000 query_toolkits-1.1.8/requirements.txt
--rw-r--r--   0 datagrand   (501) staff       (20)       38 2023-03-24 02:48:33.000000 query_toolkits-1.1.8/setup.cfg
--rw-r--r--   0 datagrand   (501) staff       (20)      588 2023-03-24 02:48:29.000000 query_toolkits-1.1.8/setup.py
+drwxr-xr-x   0 datagrand   (501) staff       (20)        0 2023-03-29 03:10:16.000000 query_toolkits-1.1.9/
+-rw-r--r--   0 datagrand   (501) staff       (20)     6148 2023-03-29 02:13:08.000000 query_toolkits-1.1.9/.DS_Store
+-rw-r--r--   0 datagrand   (501) staff       (20)       35 2022-08-12 09:08:51.000000 query_toolkits-1.1.9/MANIFEST.in
+-rw-r--r--   0 datagrand   (501) staff       (20)      197 2023-03-29 03:10:16.000000 query_toolkits-1.1.9/PKG-INFO
+drwxr-xr-x   0 datagrand   (501) staff       (20)        0 2023-03-29 03:10:16.000000 query_toolkits-1.1.9/query_toolkits/
+-rw-r--r--   0 datagrand   (501) staff       (20)      529 2023-03-29 02:54:25.000000 query_toolkits-1.1.9/query_toolkits/__init__.py
+-rw-r--r--   0 datagrand   (501) staff       (20)    40836 2023-03-29 03:08:22.000000 query_toolkits-1.1.9/query_toolkits/error_correction.py
+-rw-r--r--   0 datagrand   (501) staff       (20)    23660 2023-03-29 02:57:23.000000 query_toolkits-1.1.9/query_toolkits/extractor.py
+-rw-r--r--   0 datagrand   (501) staff       (20)      658 2023-03-20 09:28:22.000000 query_toolkits-1.1.9/query_toolkits/financial_index.txt
+-rw-r--r--   0 datagrand   (501) staff       (20)  1056198 2023-02-27 08:08:44.000000 query_toolkits-1.1.9/query_toolkits/fund_product.txt
+-rw-------   0 datagrand   (501) staff       (20) 44320114 2023-03-29 02:13:06.000000 query_toolkits-1.1.9/query_toolkits/info.json
+-rw-r--r--   0 datagrand   (501) staff       (20)      153 2022-10-10 04:02:17.000000 query_toolkits-1.1.9/query_toolkits/keyword.txt
+-rw-r--r--   0 datagrand   (501) staff       (20)   634483 2022-10-12 02:15:14.000000 query_toolkits-1.1.9/query_toolkits/organization.txt
+-rw-r--r--   0 datagrand   (501) staff       (20)     2237 2022-08-15 03:50:09.000000 query_toolkits-1.1.9/query_toolkits/unit_transform
+-rw-r--r--   0 datagrand   (501) staff       (20)     5453 2023-03-29 02:52:09.000000 query_toolkits-1.1.9/query_toolkits/utils.py
+-rw-------   0 datagrand   (501) staff       (20)   420676 2022-10-20 07:33:48.000000 query_toolkits-1.1.9/query_toolkits/weapon.txt
+drwxr-xr-x   0 datagrand   (501) staff       (20)        0 2023-03-29 03:10:16.000000 query_toolkits-1.1.9/query_toolkits.egg-info/
+-rw-r--r--   0 datagrand   (501) staff       (20)      197 2023-03-29 03:10:15.000000 query_toolkits-1.1.9/query_toolkits.egg-info/PKG-INFO
+-rw-r--r--   0 datagrand   (501) staff       (20)      520 2023-03-29 03:10:15.000000 query_toolkits-1.1.9/query_toolkits.egg-info/SOURCES.txt
+-rw-r--r--   0 datagrand   (501) staff       (20)        1 2023-03-29 03:10:15.000000 query_toolkits-1.1.9/query_toolkits.egg-info/dependency_links.txt
+-rw-r--r--   0 datagrand   (501) staff       (20)       15 2023-03-29 03:10:15.000000 query_toolkits-1.1.9/query_toolkits.egg-info/top_level.txt
+-rw-r--r--   0 datagrand   (501) staff       (20)        0 2022-08-12 09:05:37.000000 query_toolkits-1.1.9/requirements.txt
+-rw-r--r--   0 datagrand   (501) staff       (20)       38 2023-03-29 03:10:16.000000 query_toolkits-1.1.9/setup.cfg
+-rw-r--r--   0 datagrand   (501) staff       (20)      588 2023-03-29 03:08:22.000000 query_toolkits-1.1.9/setup.py
```

### Comparing `query_toolkits-1.1.8/.DS_Store` & `query_toolkits-1.1.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `query_toolkits-1.1.8/query_toolkits/error_correction.py` & `query_toolkits-1.1.9/query_toolkits/error_correction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import re
 
 class Corrector:
 
     def _get_dict(self):
         di = {
-
             ('den', 'lu', 'mi', 'ma', 'chong', 'zhi'): '登录密码重置',
             ('deng', 'lu', 'mi', 'ma', 'cong', 'zhi'): '登录密码重置',
             ('deng', 'lu', 'mi', 'ma', 'chong', 'zi'): '登录密码重置',
             ('qing', 'qing', 'qian', 'bao'): '亲情钱包',
             ('qin', 'qin', 'qian', 'bao'): '亲情钱包',
             ('qin', 'qing', 'qiang', 'bao'): '亲情钱包',
             ('ji', 'jing'): '基金',
```

### Comparing `query_toolkits-1.1.8/query_toolkits/extractor.py` & `query_toolkits-1.1.9/query_toolkits/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     def __init__(self):
         self.unit_transform = utils._read_table(_get_module_path("unit_transform"))
         self.organization = utils._read_list(_get_module_path("organization.txt"))
         self.keyword = utils._read_list(_get_module_path("keyword.txt"))
         self.financial_dict = utils.list2dict(utils._read_list(_get_module_path("financial_index.txt")))
         self.financial_dict_keys = set(self.financial_dict.keys())
         self.fund_name = utils._read_list(_get_module_path("fund_product.txt"))
+        self.stock_dict = utils._stock_dict(_get_module_path("info.json"))
 
 
     def _check_time_valid(self, word):
         m = re.match("\d+$", word)
         if m:
             if len(word) <= 6:
                 return None
@@ -436,14 +437,20 @@
 
     def extract_fund_name(self, text, word_set=None):
         res = utils.max_backward_match(text, self.fund_name if word_set is None else word_set, 40)
         res = [elem[0] for elem in res]
         return res
 
 
+    def extract_stock_name(self, text, word_dict=None):
+        di = self.stock_dict if word_dict is None else word_dict
+        keys = di.keys()
+        res = utils.max_backward_match(text, keys, 40)
+        res = [(elem[0], di[elem[0]]) for elem in res]
+        return res
 
 
 
 
 
 
 
@@ -509,85 +516,85 @@
 
 
 
 
 
 
 
-if __name__ == '__main__':
-    et = Extractor()
-    cut_res = psg.cut("pe和市净率市盈率吃在2432")
-    res = et.extract_financial_index(cut_res)
-    print(res)
-    exit(0)
-    # res = et.extract_letters("wrw234ef4 4er53 3rr shen")
-    # print(res)
-    # exit(0)
-    count_all = 0
-    count = 0
-    with open("weapon.txt", "r") as f:
-        for line in f:
-            count_all += 1
-            res = et.extract_weapon(line)
-            print(line, res)
-            if not res:
-                count += 1
-
-    print(count/count_all)
-    exit(0)
-    res = et.extract_reference_no("银发〔2015〕324号/JR/T 0125-2015")
-    print(res)
-    print(datetime.today())
-    start = time.time()
-    # text = "2021-03-0914:00开庭审理杨峰？"
-    # get_range_time_from_query(text)
-    # exit(0)
-    li = [
-        '上周六的股票',
-        '我前天来的',
-        '我今天到的',
-        '12月26号的天气怎么样',
-        '2020.10.03的2022.1.5利率是多少？',
-        "周二的api是多少",
-        "2018/1/1,利率",
-        "现在，利率",
-        "8月1日，利率",
-        "9.8，利率",
-        "第3026期，利率",
-        "2019年7月1日的利率是多少",
-        "2020年8月1日 利率",
-        "8月1日 利率",
-        "1月5日 利率",
-        "2022年11月1日中国历史",
-        "中国2021年9月18日历史",
-        "利现在，率",
-        "利2018/1/1,率",
-        "利8月1日 率",
-        "20年8月1日 利率",
-        '的2022.1.5利率是多少？',
-        '去年9月10日利率是多少？',
-        '2020年12月利率是多少？',
-        '2020.1/26利率是多少？',
-        '利率2020.1/26是多少？',
-        '利率是多少？2020.1/26',
-        '利率2020.1月26是多少？',
-        '利率2020年1月2日是多少？',
-        '我可以9月10日利率是多少？',
-        '2021-03-09 14:00开庭审理杨峰',
-        '2021-03-0914:00开庭审理杨峰',
-        '01-09 14:00开庭审理杨峰',
-        '03 09 yuhuagangtie',
-        '2022年11月12日 14:00开庭审理杨峰',
-        '我上上周五的时候利率',
-        '2015年3月5日 14：32到5月22日 13：00',
-        '1993年5月28',
-        '大前年',
-        '达观数据']
-    li = ["2004年2008年3月", "2050年6月21习主席", "2012.3.4", "2008年"]
-    for text in li:
-        cut_res = list(psg.cut(text))
-        #print(text, get_range_time_from_query(text), sep=':')
-        print(text)
-        res = et.extract_time(text, cut_res)
-        print(res)
-    print((time.time() - start)/len(li))
+# if __name__ == '__main__':
+#     et = Extractor()
+#     cut_res = psg.cut("pe和市净率市盈率吃在2432")
+#     res = et.extract_financial_index(cut_res)
+#     print(res)
+#     exit(0)
+#     # res = et.extract_letters("wrw234ef4 4er53 3rr shen")
+#     # print(res)
+#     # exit(0)
+#     count_all = 0
+#     count = 0
+#     with open("weapon.txt", "r") as f:
+#         for line in f:
+#             count_all += 1
+#             res = et.extract_weapon(line)
+#             print(line, res)
+#             if not res:
+#                 count += 1
+#
+#     print(count/count_all)
+#     exit(0)
+#     res = et.extract_reference_no("银发〔2015〕324号/JR/T 0125-2015")
+#     print(res)
+#     print(datetime.today())
+#     start = time.time()
+#     # text = "2021-03-0914:00开庭审理杨峰？"
+#     # get_range_time_from_query(text)
+#     # exit(0)
+#     li = [
+#         '上周六的股票',
+#         '我前天来的',
+#         '我今天到的',
+#         '12月26号的天气怎么样',
+#         '2020.10.03的2022.1.5利率是多少？',
+#         "周二的api是多少",
+#         "2018/1/1,利率",
+#         "现在，利率",
+#         "8月1日，利率",
+#         "9.8，利率",
+#         "第3026期，利率",
+#         "2019年7月1日的利率是多少",
+#         "2020年8月1日 利率",
+#         "8月1日 利率",
+#         "1月5日 利率",
+#         "2022年11月1日中国历史",
+#         "中国2021年9月18日历史",
+#         "利现在，率",
+#         "利2018/1/1,率",
+#         "利8月1日 率",
+#         "20年8月1日 利率",
+#         '的2022.1.5利率是多少？',
+#         '去年9月10日利率是多少？',
+#         '2020年12月利率是多少？',
+#         '2020.1/26利率是多少？',
+#         '利率2020.1/26是多少？',
+#         '利率是多少？2020.1/26',
+#         '利率2020.1月26是多少？',
+#         '利率2020年1月2日是多少？',
+#         '我可以9月10日利率是多少？',
+#         '2021-03-09 14:00开庭审理杨峰',
+#         '2021-03-0914:00开庭审理杨峰',
+#         '01-09 14:00开庭审理杨峰',
+#         '03 09 yuhuagangtie',
+#         '2022年11月12日 14:00开庭审理杨峰',
+#         '我上上周五的时候利率',
+#         '2015年3月5日 14：32到5月22日 13：00',
+#         '1993年5月28',
+#         '大前年',
+#         '达观数据']
+#     li = ["2004年2008年3月", "2050年6月21习主席", "2012.3.4", "2008年"]
+#     for text in li:
+#         cut_res = list(psg.cut(text))
+#         #print(text, get_range_time_from_query(text), sep=':')
+#         print(text)
+#         res = et.extract_time(text, cut_res)
+#         print(res)
+#     print((time.time() - start)/len(li))
```

### Comparing `query_toolkits-1.1.8/query_toolkits/financial_index.txt` & `query_toolkits-1.1.9/query_toolkits/financial_index.txt`

 * *Files identical despite different names*

### Comparing `query_toolkits-1.1.8/query_toolkits/fund_product.txt` & `query_toolkits-1.1.9/query_toolkits/fund_product.txt`

 * *Files identical despite different names*

### Comparing `query_toolkits-1.1.8/query_toolkits/organization.txt` & `query_toolkits-1.1.9/query_toolkits/organization.txt`

 * *Files identical despite different names*

### Comparing `query_toolkits-1.1.8/query_toolkits/unit_transform` & `query_toolkits-1.1.9/query_toolkits/unit_transform`

 * *Files identical despite different names*

### Comparing `query_toolkits-1.1.8/query_toolkits/utils.py` & `query_toolkits-1.1.9/query_toolkits/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import re
+import json
 
 
 
 """
 direct_transform = {
     "个百分点": ["%", 1],
 
@@ -187,8 +188,20 @@
         for e in one_line:
             e = e.strip()
             if e != "":
                 di[e] = first
     return di
 
 
+def _stock_dict(filename="info.json"):
+    di = dict()
+    json_dict = json.load(open(filename))
+    for key in json_dict:
+        elems = json_dict[key]
+        for code in elems:
+            di[code] = code
+            di[elems[code]["stock_name"]] = code
+    return di
+
+
+
```

### Comparing `query_toolkits-1.1.8/query_toolkits/weapon.txt` & `query_toolkits-1.1.9/query_toolkits/weapon.txt`

 * *Files identical despite different names*

### Comparing `query_toolkits-1.1.8/setup.py` & `query_toolkits-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '1.1.8' # 版本号
+__version__ = '1.1.9' # 版本号
 requirements = open('requirements.txt').readlines() # 依赖文件
 setup(
     name='query_toolkits', # 在pip中显示的项目名称
     version=__version__,
     author='huyi',
     author_email='huyi@datagrand.com',
     url='https://pypi.org/project/query_toolkits',
```

