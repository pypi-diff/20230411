# Comparing `tmp/promptoria-0.1.0.tar.gz` & `tmp/promptoria-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptoria-0.1.0.tar", last modified: Tue Apr 11 18:21:28 2023, max compression
+gzip compressed data, was "promptoria-0.1.1.tar", last modified: Tue Apr 11 18:27:14 2023, max compression
```

## Comparing `promptoria-0.1.0.tar` & `promptoria-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-11 18:21:28.470739 promptoria-0.1.0/
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)     1084 2023-04-05 13:35:13.000000 promptoria-0.1.0/LICENSE
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)      648 2023-04-11 18:21:28.470739 promptoria-0.1.0/PKG-INFO
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)     1472 2023-04-11 18:20:27.000000 promptoria-0.1.0/README.md
-drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-11 18:21:28.470739 promptoria-0.1.0/promptoria.egg-info/
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)      648 2023-04-11 18:21:28.000000 promptoria-0.1.0/promptoria.egg-info/PKG-INFO
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)      272 2023-04-11 18:21:28.000000 promptoria-0.1.0/promptoria.egg-info/SOURCES.txt
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)        1 2023-04-11 18:21:28.000000 promptoria-0.1.0/promptoria.egg-info/dependency_links.txt
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)        1 2023-04-11 18:21:28.000000 promptoria-0.1.0/promptoria.egg-info/not-zip-safe
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)       11 2023-04-11 18:21:28.000000 promptoria-0.1.0/promptoria.egg-info/top_level.txt
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)       38 2023-04-11 18:21:28.470739 promptoria-0.1.0/setup.cfg
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)     1422 2023-04-11 18:19:59.000000 promptoria-0.1.0/setup.py
-drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-11 18:21:28.460739 promptoria-0.1.0/src/
-drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-11 18:21:28.470739 promptoria-0.1.0/src/promptoria/
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)       59 2023-04-05 15:28:04.000000 promptoria-0.1.0/src/promptoria/__init__.py
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)     3448 2023-04-11 18:17:21.000000 promptoria-0.1.0/src/promptoria/pyprompt.py
-drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-11 18:21:28.470739 promptoria-0.1.0/tests/
--rw-r--r--   0 buanzo    (1000) buanzo    (1000)     2030 2023-04-11 18:20:49.000000 promptoria-0.1.0/tests/test_pyprompt.py
+drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-11 18:27:14.930739 promptoria-0.1.1/
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)     1084 2023-04-05 13:35:13.000000 promptoria-0.1.1/LICENSE
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)      648 2023-04-11 18:27:14.930739 promptoria-0.1.1/PKG-INFO
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)     1472 2023-04-11 18:20:27.000000 promptoria-0.1.1/README.md
+drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-11 18:27:14.930739 promptoria-0.1.1/promptoria.egg-info/
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)      648 2023-04-11 18:27:14.000000 promptoria-0.1.1/promptoria.egg-info/PKG-INFO
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)      272 2023-04-11 18:27:14.000000 promptoria-0.1.1/promptoria.egg-info/SOURCES.txt
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)        1 2023-04-11 18:27:14.000000 promptoria-0.1.1/promptoria.egg-info/dependency_links.txt
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)        1 2023-04-11 18:21:28.000000 promptoria-0.1.1/promptoria.egg-info/not-zip-safe
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)       11 2023-04-11 18:27:14.000000 promptoria-0.1.1/promptoria.egg-info/top_level.txt
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)       38 2023-04-11 18:27:14.930739 promptoria-0.1.1/setup.cfg
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)     1422 2023-04-11 18:19:59.000000 promptoria-0.1.1/setup.py
+drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-11 18:27:14.930739 promptoria-0.1.1/src/
+drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-11 18:27:14.930739 promptoria-0.1.1/src/promptoria/
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)       59 2023-04-05 15:28:04.000000 promptoria-0.1.1/src/promptoria/__init__.py
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)     3448 2023-04-11 18:26:46.000000 promptoria-0.1.1/src/promptoria/pyprompt.py
+drwxr-xr-x   0 buanzo    (1000) buanzo    (1000)        0 2023-04-11 18:27:14.930739 promptoria-0.1.1/tests/
+-rw-r--r--   0 buanzo    (1000) buanzo    (1000)     2030 2023-04-11 18:20:49.000000 promptoria-0.1.1/tests/test_pyprompt.py
```

### Comparing `promptoria-0.1.0/LICENSE` & `promptoria-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `promptoria-0.1.0/PKG-INFO` & `promptoria-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptoria
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to help you focus on your app and not 100% in the prompt. Works great with Jinja2.
 Home-page: https://github.com/buanzo/promptoria
 Author: Arturo "Buanzo" Busleiman
 Author-email: buanzo@buanzo.com.ar
 License: MIT
 Keywords: python3,utility
 Classifier: Intended Audience :: Developers
```

### Comparing `promptoria-0.1.0/README.md` & `promptoria-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `promptoria-0.1.0/promptoria.egg-info/PKG-INFO` & `promptoria-0.1.1/promptoria.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptoria
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to help you focus on your app and not 100% in the prompt. Works great with Jinja2.
 Home-page: https://github.com/buanzo/promptoria
 Author: Arturo "Buanzo" Busleiman
 Author-email: buanzo@buanzo.com.ar
 License: MIT
 Keywords: python3,utility
 Classifier: Intended Audience :: Developers
```

### Comparing `promptoria-0.1.0/setup.py` & `promptoria-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `promptoria-0.1.0/src/promptoria/pyprompt.py` & `promptoria-0.1.1/src/promptoria/pyprompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 import os
 import json
 import sys
 import openai
 from pprint import pprint,pformat
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 # This script is meant to be imported and used as a module.
 # It is not supposed to be called directly.
 # If you want to use it, import it in your code and call the functions you need.
 
 # First, we need a __init__ function that will set the API key, among other defaults.
```

### Comparing `promptoria-0.1.0/tests/test_pyprompt.py` & `promptoria-0.1.1/tests/test_pyprompt.py`

 * *Files identical despite different names*

