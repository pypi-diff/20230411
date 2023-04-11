# Comparing `tmp/huhangkai-1.0.6.tar.gz` & `tmp/huhangkai-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.0.6.tar", last modified: Thu Mar  9 05:18:09 2023, max compression
+gzip compressed data, was "huhangkai-1.0.7.tar", last modified: Tue Apr 11 07:16:16 2023, max compression
```

## Comparing `huhangkai-1.0.6.tar` & `huhangkai-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 05:18:09.571385 huhangkai-1.0.6/
--rw-rw-rw-   0        0        0      228 2023-03-09 05:18:09.571385 huhangkai-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-09 05:18:09.559419 huhangkai-1.0.6/commen/
--rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.0.6/commen/__init__.py
--rw-rw-rw-   0        0        0    32340 2023-02-22 03:30:12.000000 huhangkai-1.0.6/commen/init_project.py
--rw-rw-rw-   0        0        0     4508 2022-11-09 07:51:47.000000 huhangkai-1.0.6/commen/unit_dict.py
--rw-rw-rw-   0        0        0    17811 2023-02-22 05:53:41.000000 huhangkai-1.0.6/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2022-11-09 07:51:47.000000 huhangkai-1.0.6/commen/unit_logger.py
--rw-rw-rw-   0        0        0     6122 2023-02-15 10:10:32.000000 huhangkai-1.0.6/commen/unit_request.py
-drwxrwxrwx   0        0        0        0 2023-03-09 05:18:09.569390 huhangkai-1.0.6/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-03-09 05:18:09.000000 huhangkai-1.0.6/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-03-09 05:18:09.000000 huhangkai-1.0.6/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 05:18:09.000000 huhangkai-1.0.6/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-03-09 05:18:09.000000 huhangkai-1.0.6/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-09 05:18:09.000000 huhangkai-1.0.6/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-09 05:18:09.572382 huhangkai-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      495 2023-03-09 05:18:04.000000 huhangkai-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:16:16.486534 huhangkai-1.0.7/
+-rw-rw-rw-   0        0        0      228 2023-04-11 07:16:16.485537 huhangkai-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 07:16:16.468580 huhangkai-1.0.7/commen/
+-rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.0.7/commen/__init__.py
+-rw-rw-rw-   0        0        0    32340 2023-02-22 03:30:12.000000 huhangkai-1.0.7/commen/init_project.py
+-rw-rw-rw-   0        0        0     4508 2022-11-09 07:51:47.000000 huhangkai-1.0.7/commen/unit_dict.py
+-rw-rw-rw-   0        0        0    18531 2023-04-07 08:26:33.000000 huhangkai-1.0.7/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2022-11-09 07:51:47.000000 huhangkai-1.0.7/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     6122 2023-02-15 10:10:32.000000 huhangkai-1.0.7/commen/unit_request.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:16:16.482543 huhangkai-1.0.7/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-04-11 07:16:16.000000 huhangkai-1.0.7/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-04-11 07:16:16.000000 huhangkai-1.0.7/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 07:16:16.000000 huhangkai-1.0.7/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-11 07:16:16.000000 huhangkai-1.0.7/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 07:16:16.000000 huhangkai-1.0.7/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 07:16:16.486534 huhangkai-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      495 2023-04-11 07:15:57.000000 huhangkai-1.0.7/setup.py
```

### Comparing `huhangkai-1.0.6/commen/__init__.py` & `huhangkai-1.0.7/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.6/commen/init_project.py` & `huhangkai-1.0.7/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.6/commen/unit_dict.py` & `huhangkai-1.0.7/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.6/commen/unit_fun.py` & `huhangkai-1.0.7/commen/unit_fun.py`

 * *Files 6% similar despite different names*

```diff
@@ -404,14 +404,31 @@
                         return [i.get(name) for i in value]
                     elif isinstance(value, dict):
                         for key2, value2 in value.items():
                             if isinstance(value2, list):
                                 return [i.get(name) for i in value2 if i.get(name)]
             return []
 
+    def excelWriter(self, filename, data):
+        from pandas import DataFrame, ExcelWriter
+        filename = filename[:4] + filename[4:].replace(":", "").replace(' ', '_')
+        with ExcelWriter(filename) as writer:
+            # 写入到第一个sheet
+            if data and isinstance(data[0], list):
+                h = data[0]
+                data1 = []
+                for i in data[1:]:
+                    data1.append({x[0]: str(x[1]) for x in zip(h, i)})
+                data = data1
+            DataFrame(data).to_excel(writer,
+                              sheet_name="sheet1",
+                              index=False,
+                              engine="openpyxl"
+                              )
+
 
 if __name__ == '__main__':
     f = FunBase().faker()
     # print(f.run_mysql("", ))
     # print(f.name())  # 随机姓名
     # print(f.ipv4())  # 随机IP4地址
     # print(f.uri())  # 随机URI地址
```

### Comparing `huhangkai-1.0.6/commen/unit_logger.py` & `huhangkai-1.0.7/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.0.6/commen/unit_request.py` & `huhangkai-1.0.7/commen/unit_request.py`

 * *Files identical despite different names*

