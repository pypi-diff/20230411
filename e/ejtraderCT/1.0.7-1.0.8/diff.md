# Comparing `tmp/ejtraderCT-1.0.7.tar.gz` & `tmp/ejtraderCT-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ejtraderCT-1.0.7.tar", last modified: Wed Mar 29 15:00:39 2023, max compression
+gzip compressed data, was "ejtraderCT-1.0.8.tar", last modified: Tue Apr 11 10:56:44 2023, max compression
```

## Comparing `ejtraderCT-1.0.7.tar` & `ejtraderCT-1.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-03-29 15:00:39.118685 ejtraderCT-1.0.7/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)    35128 2023-03-28 17:20:01.000000 ejtraderCT-1.0.7/LICENSE
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       68 2023-03-28 17:20:01.000000 ejtraderCT-1.0.7/MANIFEST.in
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     4750 2023-03-29 15:00:39.119513 ejtraderCT-1.0.7/PKG-INFO
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     3459 2023-03-28 17:20:01.000000 ejtraderCT-1.0.7/README.md
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-03-29 15:00:39.108604 ejtraderCT-1.0.7/ejtraderCT/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       38 2023-03-28 17:20:01.000000 ejtraderCT-1.0.7/ejtraderCT/__init__.py
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-03-29 15:00:39.116983 ejtraderCT-1.0.7/ejtraderCT/api/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     9963 2023-03-28 17:20:01.000000 ejtraderCT-1.0.7/ejtraderCT/api/Symbol.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)        0 2023-03-28 17:20:01.000000 ejtraderCT-1.0.7/ejtraderCT/api/__init__.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      442 2023-03-28 17:20:01.000000 ejtraderCT-1.0.7/ejtraderCT/api/buffer.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)    17020 2023-03-29 14:59:32.000000 ejtraderCT-1.0.7/ejtraderCT/api/ctrader.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)    25262 2023-03-28 18:26:39.000000 ejtraderCT-1.0.7/ejtraderCT/api/fix.py
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      620 2023-03-28 17:20:01.000000 ejtraderCT-1.0.7/ejtraderCT/api/math.py
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-03-29 15:00:39.114539 ejtraderCT-1.0.7/ejtraderCT.egg-info/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     4750 2023-03-29 15:00:39.000000 ejtraderCT-1.0.7/ejtraderCT.egg-info/PKG-INFO
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      423 2023-03-29 15:00:39.000000 ejtraderCT-1.0.7/ejtraderCT.egg-info/SOURCES.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)        1 2023-03-29 15:00:39.000000 ejtraderCT-1.0.7/ejtraderCT.egg-info/dependency_links.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       15 2023-03-29 15:00:39.000000 ejtraderCT-1.0.7/ejtraderCT.egg-info/requires.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       11 2023-03-29 15:00:39.000000 ejtraderCT-1.0.7/ejtraderCT.egg-info/top_level.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)        0 2023-03-28 17:20:01.000000 ejtraderCT-1.0.7/requirements.txt
--rw-r--r--   0 emersonpedroso   (501) staff       (20)       79 2023-03-29 15:00:39.120343 ejtraderCT-1.0.7/setup.cfg
--rw-r--r--   0 emersonpedroso   (501) staff       (20)     2010 2023-03-29 14:59:41.000000 ejtraderCT-1.0.7/setup.py
-drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-03-29 15:00:39.118328 ejtraderCT-1.0.7/test/
--rw-r--r--   0 emersonpedroso   (501) staff       (20)      631 2023-03-28 17:20:01.000000 ejtraderCT-1.0.7/test/test_math.py
+drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-04-11 10:56:44.038385 ejtraderCT-1.0.8/
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)    35128 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/LICENSE
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)       68 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/MANIFEST.in
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)     4750 2023-04-11 10:56:44.038521 ejtraderCT-1.0.8/PKG-INFO
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)     3459 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/README.md
+drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-04-11 10:56:44.033737 ejtraderCT-1.0.8/ejtraderCT/
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)       38 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/ejtraderCT/__init__.py
+drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-04-11 10:56:44.037550 ejtraderCT-1.0.8/ejtraderCT/api/
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)     9963 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/ejtraderCT/api/Symbol.py
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)        0 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/ejtraderCT/api/__init__.py
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)      442 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/ejtraderCT/api/buffer.py
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)    17077 2023-04-11 10:54:43.000000 ejtraderCT-1.0.8/ejtraderCT/api/ctrader.py
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)    25262 2023-03-28 18:26:39.000000 ejtraderCT-1.0.8/ejtraderCT/api/fix.py
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)      620 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/ejtraderCT/api/math.py
+drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-04-11 10:56:44.035233 ejtraderCT-1.0.8/ejtraderCT.egg-info/
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)     4750 2023-04-11 10:56:43.000000 ejtraderCT-1.0.8/ejtraderCT.egg-info/PKG-INFO
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)      423 2023-04-11 10:56:43.000000 ejtraderCT-1.0.8/ejtraderCT.egg-info/SOURCES.txt
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)        1 2023-04-11 10:56:43.000000 ejtraderCT-1.0.8/ejtraderCT.egg-info/dependency_links.txt
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)       15 2023-04-11 10:56:43.000000 ejtraderCT-1.0.8/ejtraderCT.egg-info/requires.txt
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)       11 2023-04-11 10:56:43.000000 ejtraderCT-1.0.8/ejtraderCT.egg-info/top_level.txt
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)        0 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/requirements.txt
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)       79 2023-04-11 10:56:44.039148 ejtraderCT-1.0.8/setup.cfg
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)     2010 2023-04-11 10:56:12.000000 ejtraderCT-1.0.8/setup.py
+drwxr-xr-x   0 emersonpedroso   (501) staff       (20)        0 2023-04-11 10:56:44.037950 ejtraderCT-1.0.8/test/
+-rw-r--r--   0 emersonpedroso   (501) staff       (20)      631 2023-03-28 17:20:01.000000 ejtraderCT-1.0.8/test/test_math.py
```

### Comparing `ejtraderCT-1.0.7/LICENSE` & `ejtraderCT-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.0.7/PKG-INFO` & `ejtraderCT-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderCT
-Version: 1.0.7
+Version: 1.0.8
 Summary: Ctrader Fix API
 Home-page: https://ejtraderCT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso & Douglas Barros
 Author-email: support@ejtrader.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderCT/issues
```

### Comparing `ejtraderCT-1.0.7/README.md` & `ejtraderCT-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.0.7/ejtraderCT/api/Symbol.py` & `ejtraderCT-1.0.8/ejtraderCT/api/Symbol.py`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.0.7/ejtraderCT/api/ctrader.py` & `ejtraderCT-1.0.8/ejtraderCT/api/ctrader.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,7 +413,10 @@
         self.market_data_list[name] = { "bid": bid_str, "ask": offer_str, "spread": spread_str, "time": time.time()}
     
     def close_all(self):
         self.fix.close_all()
     
     def cancel_all(self):
         self.fix.cancel_all()
+        
+    def logout(self):
+        self.fix.logout()
```

### Comparing `ejtraderCT-1.0.7/ejtraderCT/api/fix.py` & `ejtraderCT-1.0.8/ejtraderCT/api/fix.py`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.0.7/ejtraderCT/api/math.py` & `ejtraderCT-1.0.8/ejtraderCT/api/math.py`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.0.7/ejtraderCT.egg-info/PKG-INFO` & `ejtraderCT-1.0.8/ejtraderCT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderCT
-Version: 1.0.7
+Version: 1.0.8
 Summary: Ctrader Fix API
 Home-page: https://ejtraderCT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso & Douglas Barros
 Author-email: support@ejtrader.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderCT/issues
```

### Comparing `ejtraderCT-1.0.7/setup.py` & `ejtraderCT-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         for line in f.readlines():
             reqs.append(line.strip())
     return reqs
 
 
 setup(
     name='ejtraderCT',
-    version='1.0.7',
+    version='1.0.8',
     packages=find_packages(),
     url='https://ejtraderCT.readthedocs.io/',
     download_url='https://ejtrader.com',
     license='MIT License',
     author='Emerson Pedroso & Douglas Barros',
     author_email='support@ejtrader.com',
     description='Ctrader Fix API',
```

### Comparing `ejtraderCT-1.0.7/test/test_math.py` & `ejtraderCT-1.0.8/test/test_math.py`

 * *Files identical despite different names*

