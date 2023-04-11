# Comparing `tmp/fsst-0.6.6.tar.gz` & `tmp/fsst-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsst-0.6.6.tar", last modified: Wed Apr  5 14:52:42 2023, max compression
+gzip compressed data, was "fsst-0.6.7.tar", last modified: Tue Apr 11 11:54:28 2023, max compression
```

## Comparing `fsst-0.6.6.tar` & `fsst-0.6.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-05 14:52:42.599524 fsst-0.6.6/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-04-05 14:52:42.599524 fsst-0.6.6/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.6.6/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-05 14:52:42.599524 fsst-0.6.6/fsst.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-04-05 14:52:42.000000 fsst-0.6.6/fsst.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-04-05 14:52:42.000000 fsst-0.6.6/fsst.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-04-05 14:52:42.000000 fsst-0.6.6/fsst.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-04-05 14:52:42.000000 fsst-0.6.6/fsst.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.6.6/fsst.egg-info/not-zip-safe
--rw-rw-r--   0 rob       (1000) rob       (1000)       80 2023-04-05 14:52:42.000000 fsst-0.6.6/fsst.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-04-05 14:52:42.000000 fsst-0.6.6/fsst.egg-info/top_level.txt
--rwxr-xr-x   0 rob       (1000) rob       (1000)   109707 2023-04-05 14:52:18.000000 fsst-0.6.6/fsst.py
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-04-05 14:52:42.599524 fsst-0.6.6/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)     1162 2023-04-05 14:52:30.000000 fsst-0.6.6/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-11 11:54:28.540213 fsst-0.6.7/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-04-11 11:54:28.540213 fsst-0.6.7/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.6.7/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-11 11:54:28.540213 fsst-0.6.7/fsst.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-04-11 11:54:28.000000 fsst-0.6.7/fsst.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-04-11 11:54:28.000000 fsst-0.6.7/fsst.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-04-11 11:54:28.000000 fsst-0.6.7/fsst.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-04-11 11:54:28.000000 fsst-0.6.7/fsst.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.6.7/fsst.egg-info/not-zip-safe
+-rw-rw-r--   0 rob       (1000) rob       (1000)       80 2023-04-11 11:54:28.000000 fsst-0.6.7/fsst.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-04-11 11:54:28.000000 fsst-0.6.7/fsst.egg-info/top_level.txt
+-rwxrwxr-x   0 rob       (1000) rob       (1000)   109707 2023-04-11 11:53:18.000000 fsst-0.6.7/fsst.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-04-11 11:54:28.540213 fsst-0.6.7/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1162 2023-04-11 11:53:38.000000 fsst-0.6.7/setup.py
```

### Comparing `fsst-0.6.6/PKG-INFO` & `fsst-0.6.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.6.6
+Version: 0.6.7
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.6.6/README.md` & `fsst-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `fsst-0.6.6/fsst.egg-info/PKG-INFO` & `fsst-0.6.7/fsst.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.6.6
+Version: 0.6.7
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.6.6/fsst.py` & `fsst-0.6.7/fsst.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import argparse
 import json
 import time
 import asyncio
 import itertools
 import importlib.util
 import requests
-VERSION = "0.5.5"
+VERSION = "0.6.7"
 CRYPTO_OK = True
 DOCKER_OK = True
 try:
     import aioflureedb
 except ModuleNotFoundError:
     print("WARNING: - aioflureedb python lib not found.")
     CRYPTO_OK = False
```

### Comparing `fsst-0.6.6/setup.py` & `fsst-0.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='fsst',
-    version="0.6.6",
+    version="0.6.7",
     description="Fluree Schema Scenario Tool",
     long_description="Testing tool for schema and smart function unit tests for FlureeDB",
     author='Rob Meijer',
     author_email='pibara@gmail.com',
     url='https://github.com/pibara/fluree-schema-scenario-tool',
     license='BSD',
     py_modules=['fsst'],
```

