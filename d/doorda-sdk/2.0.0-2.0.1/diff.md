# Comparing `tmp/doorda_sdk-2.0.0.tar.gz` & `tmp/doorda_sdk-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doorda_sdk-2.0.0.tar", last modified: Tue Jan 24 13:10:08 2023, max compression
+gzip compressed data, was "doorda_sdk-2.0.1.tar", last modified: Tue Apr 11 17:28:59 2023, max compression
```

## Comparing `doorda_sdk-2.0.0.tar` & `doorda_sdk-2.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:10:08.408228 doorda_sdk-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-24 13:09:58.000000 doorda_sdk-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-01-24 13:10:08.408228 doorda_sdk-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-01-24 13:09:58.000000 doorda_sdk-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:10:08.404228 doorda_sdk-2.0.0/doorda_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-24 13:09:58.000000 doorda_sdk-2.0.0/doorda_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:10:08.404228 doorda_sdk-2.0.0/doorda_sdk/host/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:09:58.000000 doorda_sdk-2.0.0/doorda_sdk/host/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-01-24 13:09:58.000000 doorda_sdk-2.0.0/doorda_sdk/host/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:10:08.408228 doorda_sdk-2.0.0/doorda_sdk/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:09:58.000000 doorda_sdk-2.0.0/doorda_sdk/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-01-24 13:09:58.000000 doorda_sdk-2.0.0/doorda_sdk/util/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-01-24 13:09:58.000000 doorda_sdk-2.0.0/doorda_sdk/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-01-24 13:09:58.000000 doorda_sdk-2.0.0/doorda_sdk/util/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-01-24 13:09:58.000000 doorda_sdk-2.0.0/doorda_sdk/util/permissions_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:10:08.404228 doorda_sdk-2.0.0/doorda_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-01-24 13:10:08.000000 doorda_sdk-2.0.0/doorda_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-01-24 13:10:08.000000 doorda_sdk-2.0.0/doorda_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 13:10:08.000000 doorda_sdk-2.0.0/doorda_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-24 13:10:08.000000 doorda_sdk-2.0.0/doorda_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-24 13:10:08.000000 doorda_sdk-2.0.0/doorda_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-01-24 13:09:58.000000 doorda_sdk-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-01-24 13:10:08.408228 doorda_sdk-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-01-24 13:09:58.000000 doorda_sdk-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:28:59.585124 doorda_sdk-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 17:28:48.000000 doorda_sdk-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-11 17:28:59.585124 doorda_sdk-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-11 17:28:48.000000 doorda_sdk-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:28:59.581124 doorda_sdk-2.0.1/doorda_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 17:28:48.000000 doorda_sdk-2.0.1/doorda_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:28:59.581124 doorda_sdk-2.0.1/doorda_sdk/host/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:28:48.000000 doorda_sdk-2.0.1/doorda_sdk/host/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-04-11 17:28:48.000000 doorda_sdk-2.0.1/doorda_sdk/host/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:28:59.585124 doorda_sdk-2.0.1/doorda_sdk/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:28:48.000000 doorda_sdk-2.0.1/doorda_sdk/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-04-11 17:28:48.000000 doorda_sdk-2.0.1/doorda_sdk/util/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-11 17:28:48.000000 doorda_sdk-2.0.1/doorda_sdk/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-11 17:28:48.000000 doorda_sdk-2.0.1/doorda_sdk/util/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-11 17:28:48.000000 doorda_sdk-2.0.1/doorda_sdk/util/permissions_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:28:59.581124 doorda_sdk-2.0.1/doorda_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-11 17:28:59.000000 doorda_sdk-2.0.1/doorda_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-11 17:28:59.000000 doorda_sdk-2.0.1/doorda_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:28:59.000000 doorda_sdk-2.0.1/doorda_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 17:28:59.000000 doorda_sdk-2.0.1/doorda_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 17:28:59.000000 doorda_sdk-2.0.1/doorda_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-11 17:28:48.000000 doorda_sdk-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-11 17:28:59.585124 doorda_sdk-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-11 17:28:48.000000 doorda_sdk-2.0.1/setup.py
```

### Comparing `doorda_sdk-2.0.0/LICENSE` & `doorda_sdk-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `doorda_sdk-2.0.0/PKG-INFO` & `doorda_sdk-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doorda_sdk
-Version: 2.0.0
+Version: 2.0.1
 Summary: Doorda SDK for access to Hosted Platform
 Home-page: https://github.com/doorda/doorda-python-sdk
 Download-URL: https://github.com/Doorda/doorda-python-sdk/releases/latest
 Author: Samuel Tan
 Author-email: samuel@doorda.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doorda_sdk-2.0.0/README.md` & `doorda_sdk-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `doorda_sdk-2.0.0/doorda_sdk/host/client.py` & `doorda_sdk-2.0.1/doorda_sdk/host/client.py`

 * *Files identical despite different names*

### Comparing `doorda_sdk-2.0.0/doorda_sdk/util/common.py` & `doorda_sdk-2.0.1/doorda_sdk/util/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,21 +54,21 @@
         raw_type = type_signature["rawType"]
         arguments = type_signature["arguments"]
         return (
             column["name"],  # name
             column["type"],  # type_code
             None,  # display_size
             arguments[0]["value"]
-            if raw_type in LENGTH_TYPES
+            if raw_type in LENGTH_TYPES and arguments
             else None,  # internal_size
             arguments[0]["value"]
-            if raw_type in PRECISION_TYPES
+            if raw_type in PRECISION_TYPES and arguments
             else None,  # precision
             arguments[1]["value"]
-            if raw_type in SCALE_TYPES
+            if raw_type in SCALE_TYPES and arguments
             else None,  # scale
             None,  # null_ok
         )
 
     def _fetch_while(self, fn):
         while fn():
             self._fetch_more()
```

### Comparing `doorda_sdk-2.0.0/doorda_sdk/util/decorators.py` & `doorda_sdk-2.0.1/doorda_sdk/util/decorators.py`

 * *Files identical despite different names*

### Comparing `doorda_sdk-2.0.0/doorda_sdk/util/exc.py` & `doorda_sdk-2.0.1/doorda_sdk/util/exc.py`

 * *Files identical despite different names*

### Comparing `doorda_sdk-2.0.0/doorda_sdk/util/permissions_tree.py` & `doorda_sdk-2.0.1/doorda_sdk/util/permissions_tree.py`

 * *Files identical despite different names*

### Comparing `doorda_sdk-2.0.0/doorda_sdk.egg-info/PKG-INFO` & `doorda_sdk-2.0.1/doorda_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doorda-sdk
-Version: 2.0.0
+Version: 2.0.1
 Summary: Doorda SDK for access to Hosted Platform
 Home-page: https://github.com/doorda/doorda-python-sdk
 Download-URL: https://github.com/Doorda/doorda-python-sdk/releases/latest
 Author: Samuel Tan
 Author-email: samuel@doorda.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doorda_sdk-2.0.0/setup.py` & `doorda_sdk-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 INSTALL_REQUIRES = ["future>=0.16.0", "requests>=2.21.0"]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="doorda_sdk",
-    version="2.0.0",
+    version="2.0.1",
     author="Samuel Tan",
     author_email="samuel@doorda.com",
     description="Doorda SDK for access to Hosted Platform",
     license="Apache License 2.0",
     long_description=long_description,
     url="https://github.com/doorda/doorda-python-sdk",
     packages=["doorda_sdk"]
```

