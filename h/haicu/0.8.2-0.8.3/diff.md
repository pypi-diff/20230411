# Comparing `tmp/haicu-0.8.2.tar.gz` & `tmp/haicu-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haicu-0.8.2.tar", last modified: Tue Apr 11 20:08:06 2023, max compression
+gzip compressed data, was "haicu-0.8.3.tar", last modified: Tue Apr 11 20:11:16 2023, max compression
```

## Comparing `haicu-0.8.2.tar` & `haicu-0.8.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:08:06.498181 haicu-0.8.2/
--rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-0.8.2/LICENSE
--rw-rw-r--   0 bry       (1000) bry       (1000)     3555 2023-04-11 20:08:06.498181 haicu-0.8.2/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)     2042 2023-04-11 19:58:00.000000 haicu-0.8.2/README.md
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:08:06.498181 haicu-0.8.2/haicu/
--rw-rw-r--   0 bry       (1000) bry       (1000)        0 2023-03-10 00:08:52.000000 haicu-0.8.2/haicu/__init__.py
--rwxrwxr-x   0 bry       (1000) bry       (1000)    28485 2023-04-11 20:07:56.000000 haicu-0.8.2/haicu/__main__.py
--rwxrwxr-x   0 bry       (1000) bry       (1000)    12563 2023-04-11 18:21:24.000000 haicu-0.8.2/haicu/format.py
--rw-rw-r--   0 bry       (1000) bry       (1000)    11443 2023-04-11 18:13:59.000000 haicu-0.8.2/haicu/ftdi.py
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:08:06.498181 haicu-0.8.2/haicu.egg-info/
--rw-rw-r--   0 bry       (1000) bry       (1000)     3555 2023-04-11 20:08:06.000000 haicu-0.8.2/haicu.egg-info/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)      274 2023-04-11 20:08:06.000000 haicu-0.8.2/haicu.egg-info/SOURCES.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-04-11 20:08:06.000000 haicu-0.8.2/haicu.egg-info/dependency_links.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       50 2023-04-11 20:08:06.000000 haicu-0.8.2/haicu.egg-info/entry_points.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-04-11 20:08:06.000000 haicu-0.8.2/haicu.egg-info/requires.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-04-11 20:08:06.000000 haicu-0.8.2/haicu.egg-info/top_level.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)      742 2023-04-11 20:08:01.000000 haicu-0.8.2/pyproject.toml
--rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-04-11 20:08:06.498181 haicu-0.8.2/setup.cfg
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:11:16.250266 haicu-0.8.3/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-0.8.3/LICENSE
+-rw-rw-r--   0 bry       (1000) bry       (1000)     3555 2023-04-11 20:11:16.250266 haicu-0.8.3/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)     2042 2023-04-11 19:58:00.000000 haicu-0.8.3/README.md
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:11:16.250266 haicu-0.8.3/haicu/
+-rw-rw-r--   0 bry       (1000) bry       (1000)        0 2023-03-10 00:08:52.000000 haicu-0.8.3/haicu/__init__.py
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    28509 2023-04-11 20:10:54.000000 haicu-0.8.3/haicu/__main__.py
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    12563 2023-04-11 18:21:24.000000 haicu-0.8.3/haicu/format.py
+-rw-rw-r--   0 bry       (1000) bry       (1000)    11443 2023-04-11 18:13:59.000000 haicu-0.8.3/haicu/ftdi.py
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:11:16.250266 haicu-0.8.3/haicu.egg-info/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     3555 2023-04-11 20:11:16.000000 haicu-0.8.3/haicu.egg-info/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)      274 2023-04-11 20:11:16.000000 haicu-0.8.3/haicu.egg-info/SOURCES.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-04-11 20:11:16.000000 haicu-0.8.3/haicu.egg-info/dependency_links.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       50 2023-04-11 20:11:16.000000 haicu-0.8.3/haicu.egg-info/entry_points.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-04-11 20:11:16.000000 haicu-0.8.3/haicu.egg-info/requires.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-04-11 20:11:16.000000 haicu-0.8.3/haicu.egg-info/top_level.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)      742 2023-04-11 20:11:10.000000 haicu-0.8.3/pyproject.toml
+-rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-04-11 20:11:16.250266 haicu-0.8.3/setup.cfg
```

### Comparing `haicu-0.8.2/LICENSE` & `haicu-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `haicu-0.8.2/PKG-INFO` & `haicu-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.8.2
+Version: 0.8.3
 Summary: package for HAICU
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

### Comparing `haicu-0.8.2/README.md` & `haicu-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `haicu-0.8.2/haicu/__main__.py` & `haicu-0.8.3/haicu/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,37 +13,38 @@
 from . import ftdi as haicu_ftdi
 from . import format as haicu_format
 
 VERSION = pkg_resources.get_distribution('haicu').version
 
 # Table to convert 'get' request name to status register address
 GET_REG_TABLE = {
-    'invert_frontpanel': 22,
-    'invert_right_address': 21,
-    'invert_left_address': 20,
-    'invert_tunebox8': 19,
-    'invert_tunebox7': 18,
-    'invert_tunebox6': 17,
-    'invert_tunebox5': 16,
-    'invert_tunebox4': 15,
-    'invert_tunebox3': 14,
-    'invert_tunebox2': 13,
-    'invert_tunebox1': 12,
-    'enable_frontpanel': 11,
-    'enable_right_address': 10,
-    'enable_left_address': 9,
-    'enable_tunebox8': 8,
-    'enable_tunebox7': 7,
-    'enable_tunebox6': 6,
-    'enable_tunebox5': 5,
-    'enable_tunebox4': 4,
-    'enable_tunebox3': 3,
-    'enable_tunebox2': 2,
-    'enable_tunebox1': 1,
-    'trigger_invert': 0,
+    'invert_frontpanel': 23,
+    'invert_right_address': 22,
+    'invert_left_address': 21,
+    'invert_tunebox8': 20,
+    'invert_tunebox7': 19,
+    'invert_tunebox6': 18,
+    'invert_tunebox5': 17,
+    'invert_tunebox4': 16,
+    'invert_tunebox3': 15,
+    'invert_tunebox2': 14,
+    'invert_tunebox1': 13,
+    'enable_frontpanel': 12,
+    'enable_right_address': 11,
+    'enable_left_address': 10,
+    'enable_tunebox8': 9,
+    'enable_tunebox7': 8,
+    'enable_tunebox6': 7,
+    'enable_tunebox5': 6,
+    'enable_tunebox4': 5,
+    'enable_tunebox3': 4,
+    'enable_tunebox2': 3,
+    'enable_tunebox1': 2,
+    'trigger_invert': 1,
+    'trigger_delay': 0
 }
 
 GET_PROGRAM_TABLE = {
     'left': 0,
     'right': 1,
     'extension': 2
 }
```

### Comparing `haicu-0.8.2/haicu/format.py` & `haicu-0.8.3/haicu/format.py`

 * *Files identical despite different names*

### Comparing `haicu-0.8.2/haicu/ftdi.py` & `haicu-0.8.3/haicu/ftdi.py`

 * *Files identical despite different names*

### Comparing `haicu-0.8.2/haicu.egg-info/PKG-INFO` & `haicu-0.8.3/haicu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.8.2
+Version: 0.8.3
 Summary: package for HAICU
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

