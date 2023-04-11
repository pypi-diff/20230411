# Comparing `tmp/bigbucks_port-0.0.5.tar.gz` & `tmp/bigbucks_port-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigbucks_port-0.0.5.tar", last modified: Tue Apr 11 03:48:33 2023, max compression
+gzip compressed data, was "bigbucks_port-0.0.7.tar", last modified: Tue Apr 11 04:14:33 2023, max compression
```

## Comparing `bigbucks_port-0.0.5.tar` & `bigbucks_port-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 03:48:33.985796 bigbucks_port-0.0.5/
--rw-r--r--   0 cuiwenjie   (501) staff       (20)     1065 2023-04-03 00:48:13.000000 bigbucks_port-0.0.5/LICENSE
--rw-r--r--   0 cuiwenjie   (501) staff       (20)     3464 2023-04-11 03:48:33.985619 bigbucks_port-0.0.5/PKG-INFO
--rw-r--r--   0 cuiwenjie   (501) staff       (20)     3264 2023-04-06 03:40:05.000000 bigbucks_port-0.0.5/README.md
--rw-r--r--   0 cuiwenjie   (501) staff       (20)       38 2023-04-11 03:48:33.985848 bigbucks_port-0.0.5/setup.cfg
--rw-r--r--   0 cuiwenjie   (501) staff       (20)      346 2023-04-11 03:41:43.000000 bigbucks_port-0.0.5/setup.py
-drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 03:48:33.983076 bigbucks_port-0.0.5/src/
-drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 03:48:33.984236 bigbucks_port-0.0.5/src/bigbucks_port/
--rw-r--r--   0 cuiwenjie   (501) staff       (20)        0 2023-04-02 23:17:45.000000 bigbucks_port-0.0.5/src/bigbucks_port/__init__.py
--rw-r--r--   0 cuiwenjie   (501) staff       (20)     8947 2023-04-11 03:34:35.000000 bigbucks_port-0.0.5/src/bigbucks_port/portfolio.py
-drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 03:48:33.984969 bigbucks_port-0.0.5/src/bigbucks_port.egg-info/
--rw-r--r--   0 cuiwenjie   (501) staff       (20)     3464 2023-04-11 03:48:33.000000 bigbucks_port-0.0.5/src/bigbucks_port.egg-info/PKG-INFO
--rw-r--r--   0 cuiwenjie   (501) staff       (20)      275 2023-04-11 03:48:33.000000 bigbucks_port-0.0.5/src/bigbucks_port.egg-info/SOURCES.txt
--rw-r--r--   0 cuiwenjie   (501) staff       (20)        1 2023-04-11 03:48:33.000000 bigbucks_port-0.0.5/src/bigbucks_port.egg-info/dependency_links.txt
--rw-r--r--   0 cuiwenjie   (501) staff       (20)       14 2023-04-11 03:48:33.000000 bigbucks_port-0.0.5/src/bigbucks_port.egg-info/top_level.txt
-drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 03:48:33.985159 bigbucks_port-0.0.5/tests/
--rw-r--r--   0 cuiwenjie   (501) staff       (20)      531 2023-04-11 03:43:40.000000 bigbucks_port-0.0.5/tests/test_portfolio.py
+drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 04:14:33.939888 bigbucks_port-0.0.7/
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)     1065 2023-04-03 00:48:13.000000 bigbucks_port-0.0.7/LICENSE
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)     3464 2023-04-11 04:14:33.939726 bigbucks_port-0.0.7/PKG-INFO
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)     3264 2023-04-06 03:40:05.000000 bigbucks_port-0.0.7/README.md
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)       38 2023-04-11 04:14:33.939934 bigbucks_port-0.0.7/setup.cfg
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)      346 2023-04-11 04:13:46.000000 bigbucks_port-0.0.7/setup.py
+drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 04:14:33.937357 bigbucks_port-0.0.7/src/
+drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 04:14:33.938427 bigbucks_port-0.0.7/src/bigbucks_port/
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)        0 2023-04-02 23:17:45.000000 bigbucks_port-0.0.7/src/bigbucks_port/__init__.py
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)     8912 2023-04-11 04:10:05.000000 bigbucks_port-0.0.7/src/bigbucks_port/portfolio.py
+drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 04:14:33.939385 bigbucks_port-0.0.7/src/bigbucks_port.egg-info/
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)     3464 2023-04-11 04:14:33.000000 bigbucks_port-0.0.7/src/bigbucks_port.egg-info/PKG-INFO
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)      275 2023-04-11 04:14:33.000000 bigbucks_port-0.0.7/src/bigbucks_port.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)        1 2023-04-11 04:14:33.000000 bigbucks_port-0.0.7/src/bigbucks_port.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)       14 2023-04-11 04:14:33.000000 bigbucks_port-0.0.7/src/bigbucks_port.egg-info/top_level.txt
+drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 04:14:33.939539 bigbucks_port-0.0.7/tests/
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)      481 2023-04-11 04:12:52.000000 bigbucks_port-0.0.7/tests/test_portfolio.py
```

### Comparing `bigbucks_port-0.0.5/LICENSE` & `bigbucks_port-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bigbucks_port-0.0.5/PKG-INFO` & `bigbucks_port-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigbucks_port
-Version: 0.0.5
+Version: 0.0.7
 Summary: A package used for portfolio analysis in Fintech512
 Author: Wenjie Cui
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Introduction
```

### Comparing `bigbucks_port-0.0.5/README.md` & `bigbucks_port-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bigbucks_port-0.0.5/src/bigbucks_port/portfolio.py` & `bigbucks_port-0.0.7/src/bigbucks_port/portfolio.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,16 +185,15 @@
 def frontier_json(objs,id,num):
     returns,risk = frontier(objs,id,num)
     # A list of json objects 
     js_list =[]
     for i in range(len(returns)):
         dict_obj = {'std': risk[i], 'mean': returns[i]}
         js_list.append(dict_obj)
-    js_result = {"data":js_list}
-    return json.dumps(js_result)
+    return json.dumps(js_list)
 
 # optimal portfolio with max sharpe
 def optimize_port(rf,objs,id):
     er = er_covar(objs,id)[0].to_numpy()
     covar = er_covar(objs,id)[2].to_numpy()
     n = len(er)
     def sharpe_cal(w):
```

### Comparing `bigbucks_port-0.0.5/src/bigbucks_port.egg-info/PKG-INFO` & `bigbucks_port-0.0.7/src/bigbucks_port.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigbucks-port
-Version: 0.0.5
+Version: 0.0.7
 Summary: A package used for portfolio analysis in Fintech512
 Author: Wenjie Cui
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Introduction
```

