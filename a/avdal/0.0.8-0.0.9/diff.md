# Comparing `tmp/avdal-0.0.8.tar.gz` & `tmp/avdal-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/hazim/Desktop/tmp/config/dist/tmpbnyln41o/avdal-0.0.8.tar", last modified: Sat Oct  2 06:49:48 2021, max compression
+gzip compressed data, was "/home/hazim/Desktop/tmp/config/dist/tmp08_euvdw/avdal-0.0.9.tar", last modified: Sat Oct  2 06:51:41 2021, max compression
```

## Comparing `avdal-0.0.8.tar` & `avdal-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hazim     (1000) hazim     (1000)        0 2021-10-02 06:49:48.000000 avdal-0.0.8/
--rw-r--r--   0 hazim     (1000) hazim     (1000)     1068 2021-10-02 03:02:49.000000 avdal-0.0.8/LICENSE
--rw-r--r--   0 hazim     (1000) hazim     (1000)      544 2021-10-02 06:49:48.000000 avdal-0.0.8/PKG-INFO
--rw-r--r--   0 hazim     (1000) hazim     (1000)        0 2021-10-02 02:55:33.000000 avdal-0.0.8/README
--rw-r--r--   0 hazim     (1000) hazim     (1000)      103 2021-10-02 02:53:06.000000 avdal-0.0.8/pyproject.toml
--rw-r--r--   0 hazim     (1000) hazim     (1000)      622 2021-10-02 06:49:48.000000 avdal-0.0.8/setup.cfg
-drwxr-xr-x   0 hazim     (1000) hazim     (1000)        0 2021-10-02 06:49:48.000000 avdal-0.0.8/src/
-drwxr-xr-x   0 hazim     (1000) hazim     (1000)        0 2021-10-02 06:49:48.000000 avdal-0.0.8/src/avdal/
--rw-r--r--   0 hazim     (1000) hazim     (1000)        0 2021-10-02 02:50:13.000000 avdal-0.0.8/src/avdal/__init__.py
--rw-r--r--   0 hazim     (1000) hazim     (1000)      962 2021-10-02 05:36:52.000000 avdal-0.0.8/src/avdal/annotations.py
--rw-r--r--   0 hazim     (1000) hazim     (1000)     1689 2021-10-02 06:48:21.000000 avdal-0.0.8/src/avdal/config.py
-drwxr-xr-x   0 hazim     (1000) hazim     (1000)        0 2021-10-02 06:49:48.000000 avdal-0.0.8/src/avdal.egg-info/
--rw-r--r--   0 hazim     (1000) hazim     (1000)      544 2021-10-02 06:49:48.000000 avdal-0.0.8/src/avdal.egg-info/PKG-INFO
--rw-r--r--   0 hazim     (1000) hazim     (1000)      238 2021-10-02 06:49:48.000000 avdal-0.0.8/src/avdal.egg-info/SOURCES.txt
--rw-r--r--   0 hazim     (1000) hazim     (1000)        1 2021-10-02 06:49:48.000000 avdal-0.0.8/src/avdal.egg-info/dependency_links.txt
--rw-r--r--   0 hazim     (1000) hazim     (1000)        6 2021-10-02 06:49:48.000000 avdal-0.0.8/src/avdal.egg-info/top_level.txt
+drwxr-xr-x   0 hazim     (1000) hazim     (1000)        0 2021-10-02 06:51:41.000000 avdal-0.0.9/
+-rw-r--r--   0 hazim     (1000) hazim     (1000)     1068 2021-10-02 03:02:49.000000 avdal-0.0.9/LICENSE
+-rw-r--r--   0 hazim     (1000) hazim     (1000)      544 2021-10-02 06:51:41.000000 avdal-0.0.9/PKG-INFO
+-rw-r--r--   0 hazim     (1000) hazim     (1000)        0 2021-10-02 02:55:33.000000 avdal-0.0.9/README
+-rw-r--r--   0 hazim     (1000) hazim     (1000)      103 2021-10-02 02:53:06.000000 avdal-0.0.9/pyproject.toml
+-rw-r--r--   0 hazim     (1000) hazim     (1000)      622 2021-10-02 06:51:41.000000 avdal-0.0.9/setup.cfg
+drwxr-xr-x   0 hazim     (1000) hazim     (1000)        0 2021-10-02 06:51:41.000000 avdal-0.0.9/src/
+drwxr-xr-x   0 hazim     (1000) hazim     (1000)        0 2021-10-02 06:51:41.000000 avdal-0.0.9/src/avdal/
+-rw-r--r--   0 hazim     (1000) hazim     (1000)        0 2021-10-02 02:50:13.000000 avdal-0.0.9/src/avdal/__init__.py
+-rw-r--r--   0 hazim     (1000) hazim     (1000)      962 2021-10-02 05:36:52.000000 avdal-0.0.9/src/avdal/annotations.py
+-rw-r--r--   0 hazim     (1000) hazim     (1000)     1696 2021-10-02 06:51:18.000000 avdal-0.0.9/src/avdal/config.py
+drwxr-xr-x   0 hazim     (1000) hazim     (1000)        0 2021-10-02 06:51:41.000000 avdal-0.0.9/src/avdal.egg-info/
+-rw-r--r--   0 hazim     (1000) hazim     (1000)      544 2021-10-02 06:51:41.000000 avdal-0.0.9/src/avdal.egg-info/PKG-INFO
+-rw-r--r--   0 hazim     (1000) hazim     (1000)      238 2021-10-02 06:51:41.000000 avdal-0.0.9/src/avdal.egg-info/SOURCES.txt
+-rw-r--r--   0 hazim     (1000) hazim     (1000)        1 2021-10-02 06:51:41.000000 avdal-0.0.9/src/avdal.egg-info/dependency_links.txt
+-rw-r--r--   0 hazim     (1000) hazim     (1000)        6 2021-10-02 06:51:41.000000 avdal-0.0.9/src/avdal.egg-info/top_level.txt
```

### Comparing `avdal-0.0.8/LICENSE` & `avdal-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `avdal-0.0.8/PKG-INFO` & `avdal-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avdal
-Version: 0.0.8
+Version: 0.0.9
 Summary: Boilerplate python code used in my personal projects
 Home-page: https://github.com/hazimavdal/pip
 Author: Hazim Avdal
 Author-email: dev@avd.al
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hazimavdal/pip/issues
 Platform: UNKNOWN
```

### Comparing `avdal-0.0.8/setup.cfg` & `avdal-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = avdal
-version = 0.0.8
+version = 0.0.9
 author = Hazim Avdal
 author_email = dev@avd.al
 description = Boilerplate python code used in my personal projects
 long_description = file: README
 long_description_content_type = text/markdown
 url = https://github.com/hazimavdal/pip
 project_urls =
```

### Comparing `avdal-0.0.8/src/avdal/annotations.py` & `avdal-0.0.9/src/avdal/annotations.py`

 * *Files identical despite different names*

### Comparing `avdal-0.0.8/src/avdal/config.py` & `avdal-0.0.9/src/avdal/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import re
-import annotations
+from . import annotations
 
 _envre = re.compile(r'''^(?:export\s*)?([_a-zA-Z][\w_]*)\s*=\s*(.*)$''')
 _varre = re.compile(r'''\$([\w_]+)''')
 _include_re = re.compile(r'''^#include\s+(.*)\s*$''')
 
 
 @annotations.enforce_types
```

### Comparing `avdal-0.0.8/src/avdal.egg-info/PKG-INFO` & `avdal-0.0.9/src/avdal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avdal
-Version: 0.0.8
+Version: 0.0.9
 Summary: Boilerplate python code used in my personal projects
 Home-page: https://github.com/hazimavdal/pip
 Author: Hazim Avdal
 Author-email: dev@avd.al
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hazimavdal/pip/issues
 Platform: UNKNOWN
```

