# Comparing `tmp/besapi-3.1.4.tar.gz` & `tmp/besapi-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besapi-3.1.4.tar", last modified: Thu Feb 16 21:38:18 2023, max compression
+gzip compressed data, was "besapi-3.1.5.tar", last modified: Tue Apr 11 13:25:13 2023, max compression
```

## Comparing `besapi-3.1.4.tar` & `besapi-3.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:38:18.470311 besapi-3.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-16 21:34:27.000000 besapi-3.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-16 21:34:27.000000 besapi-3.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-02-16 21:38:18.470311 besapi-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-02-16 21:34:27.000000 besapi-3.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-16 21:34:27.000000 besapi-3.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-16 21:38:18.470311 besapi-3.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-16 21:34:27.000000 besapi-3.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:38:18.466311 besapi-3.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:38:18.470311 besapi-3.1.4/src/besapi/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-16 21:34:27.000000 besapi-3.1.4/src/besapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-16 21:34:27.000000 besapi-3.1.4/src/besapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34032 2023-02-16 21:34:27.000000 besapi-3.1.4/src/besapi/besapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:38:18.470311 besapi-3.1.4/src/besapi/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    42635 2023-02-16 21:34:27.000000 besapi-3.1.4/src/besapi/schemas/BES.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    25664 2023-02-16 21:34:27.000000 besapi-3.1.4/src/besapi/schemas/BESAPI.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    20054 2023-02-16 21:34:27.000000 besapi-3.1.4/src/besapi/schemas/BESActionSettings.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:38:18.470311 besapi-3.1.4/src/besapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-02-16 21:38:18.000000 besapi-3.1.4/src/besapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-16 21:38:18.000000 besapi-3.1.4/src/besapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 21:38:18.000000 besapi-3.1.4/src/besapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-16 21:38:18.000000 besapi-3.1.4/src/besapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-16 21:38:18.000000 besapi-3.1.4/src/besapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:38:18.470311 besapi-3.1.4/src/bescli/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-16 21:34:27.000000 besapi-3.1.4/src/bescli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-16 21:34:27.000000 besapi-3.1.4/src/bescli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-02-16 21:34:27.000000 besapi-3.1.4/src/bescli/bescli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 21:38:18.470311 besapi-3.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-02-16 21:34:27.000000 besapi-3.1.4/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:25:13.386768 besapi-3.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 13:18:54.000000 besapi-3.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 13:18:54.000000 besapi-3.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-11 13:25:13.386768 besapi-3.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-11 13:18:54.000000 besapi-3.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-11 13:18:54.000000 besapi-3.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-11 13:25:13.386768 besapi-3.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-11 13:18:54.000000 besapi-3.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:25:13.378768 besapi-3.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:25:13.382768 besapi-3.1.5/src/besapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-11 13:18:54.000000 besapi-3.1.5/src/besapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 13:18:54.000000 besapi-3.1.5/src/besapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34032 2023-04-11 13:18:54.000000 besapi-3.1.5/src/besapi/besapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:25:13.382768 besapi-3.1.5/src/besapi/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    42635 2023-04-11 13:18:54.000000 besapi-3.1.5/src/besapi/schemas/BES.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    25664 2023-04-11 13:18:54.000000 besapi-3.1.5/src/besapi/schemas/BESAPI.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    20054 2023-04-11 13:18:54.000000 besapi-3.1.5/src/besapi/schemas/BESActionSettings.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:25:13.382768 besapi-3.1.5/src/besapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-11 13:25:13.000000 besapi-3.1.5/src/besapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-11 13:25:13.000000 besapi-3.1.5/src/besapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:25:13.000000 besapi-3.1.5/src/besapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 13:25:13.000000 besapi-3.1.5/src/besapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 13:25:13.000000 besapi-3.1.5/src/besapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:25:13.386768 besapi-3.1.5/src/bescli/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-11 13:18:54.000000 besapi-3.1.5/src/bescli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 13:18:54.000000 besapi-3.1.5/src/bescli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-04-11 13:18:54.000000 besapi-3.1.5/src/bescli/bescli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:25:13.386768 besapi-3.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-11 13:18:54.000000 besapi-3.1.5/tests/tests.py
```

### Comparing `besapi-3.1.4/LICENSE.txt` & `besapi-3.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `besapi-3.1.4/PKG-INFO` & `besapi-3.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besapi
-Version: 3.1.4
+Version: 3.1.5
 Summary: Library for working with the BigFix REST API
 Home-page: https://github.com/CLCMacTeam/besapi
 Author: Matt Hansen, James Stewart
 Author-email: hansen.m@psu.edu, james@jgstew.com
 License: MIT
 Keywords: bigfix iem tem rest api
 Classifier: Programming Language :: Python :: 3
```

### Comparing `besapi-3.1.4/README.md` & `besapi-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `besapi-3.1.4/setup.py` & `besapi-3.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `besapi-3.1.4/src/besapi/besapi.py` & `besapi-3.1.5/src/besapi/besapi.py`

 * *Files identical despite different names*

### Comparing `besapi-3.1.4/src/besapi/schemas/BES.xsd` & `besapi-3.1.5/src/besapi/schemas/BES.xsd`

 * *Files identical despite different names*

### Comparing `besapi-3.1.4/src/besapi/schemas/BESAPI.xsd` & `besapi-3.1.5/src/besapi/schemas/BESAPI.xsd`

 * *Files identical despite different names*

### Comparing `besapi-3.1.4/src/besapi/schemas/BESActionSettings.xsd` & `besapi-3.1.5/src/besapi/schemas/BESActionSettings.xsd`

 * *Files identical despite different names*

### Comparing `besapi-3.1.4/src/besapi.egg-info/PKG-INFO` & `besapi-3.1.5/src/besapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besapi
-Version: 3.1.4
+Version: 3.1.5
 Summary: Library for working with the BigFix REST API
 Home-page: https://github.com/CLCMacTeam/besapi
 Author: Matt Hansen, James Stewart
 Author-email: hansen.m@psu.edu, james@jgstew.com
 License: MIT
 Keywords: bigfix iem tem rest api
 Classifier: Programming Language :: Python :: 3
```

### Comparing `besapi-3.1.4/src/bescli/bescli.py` & `besapi-3.1.5/src/bescli/bescli.py`

 * *Files identical despite different names*

### Comparing `besapi-3.1.4/tests/tests.py` & `besapi-3.1.5/tests/tests.py`

 * *Files identical despite different names*

