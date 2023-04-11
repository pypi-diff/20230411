# Comparing `tmp/haicu-0.0.95.tar.gz` & `tmp/haicu-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haicu-0.0.95.tar", last modified: Tue Apr 11 18:16:31 2023, max compression
+gzip compressed data, was "haicu-0.0.96.tar", last modified: Tue Apr 11 18:24:00 2023, max compression
```

## Comparing `haicu-0.0.95.tar` & `haicu-0.0.96.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:16:31.493294 haicu-0.0.95/
--rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-0.0.95/LICENSE
--rw-rw-r--   0 bry       (1000) bry       (1000)     2593 2023-04-11 18:16:31.493294 haicu-0.0.95/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)     1073 2023-04-11 17:00:57.000000 haicu-0.0.95/README.md
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:16:31.493294 haicu-0.0.95/haicu/
--rw-rw-r--   0 bry       (1000) bry       (1000)        0 2023-03-10 00:08:52.000000 haicu-0.0.95/haicu/__init__.py
--rwxrwxr-x   0 bry       (1000) bry       (1000)    28623 2023-04-11 18:14:35.000000 haicu-0.0.95/haicu/__main__.py
--rwxrwxr-x   0 bry       (1000) bry       (1000)    12563 2023-04-11 18:13:59.000000 haicu-0.0.95/haicu/format.py
--rw-rw-r--   0 bry       (1000) bry       (1000)    11443 2023-04-11 18:13:59.000000 haicu-0.0.95/haicu/ftdi.py
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:16:31.493294 haicu-0.0.95/haicu.egg-info/
--rw-rw-r--   0 bry       (1000) bry       (1000)     2593 2023-04-11 18:16:31.000000 haicu-0.0.95/haicu.egg-info/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)      274 2023-04-11 18:16:31.000000 haicu-0.0.95/haicu.egg-info/SOURCES.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-04-11 18:16:31.000000 haicu-0.0.95/haicu.egg-info/dependency_links.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       50 2023-04-11 18:16:31.000000 haicu-0.0.95/haicu.egg-info/entry_points.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-04-11 18:16:31.000000 haicu-0.0.95/haicu.egg-info/requires.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-04-11 18:16:31.000000 haicu-0.0.95/haicu.egg-info/top_level.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)      709 2023-04-11 18:16:25.000000 haicu-0.0.95/pyproject.toml
--rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-04-11 18:16:31.493294 haicu-0.0.95/setup.cfg
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:24:00.606074 haicu-0.0.96/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-0.0.96/LICENSE
+-rw-rw-r--   0 bry       (1000) bry       (1000)     2587 2023-04-11 18:24:00.606074 haicu-0.0.96/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)     1073 2023-04-11 17:00:57.000000 haicu-0.0.96/README.md
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:24:00.606074 haicu-0.0.96/haicu/
+-rw-rw-r--   0 bry       (1000) bry       (1000)        0 2023-03-10 00:08:52.000000 haicu-0.0.96/haicu/__init__.py
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    28700 2023-04-11 18:22:57.000000 haicu-0.0.96/haicu/__main__.py
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    12563 2023-04-11 18:21:24.000000 haicu-0.0.96/haicu/format.py
+-rw-rw-r--   0 bry       (1000) bry       (1000)    11443 2023-04-11 18:13:59.000000 haicu-0.0.96/haicu/ftdi.py
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:24:00.606074 haicu-0.0.96/haicu.egg-info/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     2587 2023-04-11 18:24:00.000000 haicu-0.0.96/haicu.egg-info/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)      274 2023-04-11 18:24:00.000000 haicu-0.0.96/haicu.egg-info/SOURCES.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-04-11 18:24:00.000000 haicu-0.0.96/haicu.egg-info/dependency_links.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       50 2023-04-11 18:24:00.000000 haicu-0.0.96/haicu.egg-info/entry_points.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-04-11 18:24:00.000000 haicu-0.0.96/haicu.egg-info/requires.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-04-11 18:24:00.000000 haicu-0.0.96/haicu.egg-info/top_level.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)      703 2023-04-11 18:23:27.000000 haicu-0.0.96/pyproject.toml
+-rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-04-11 18:24:00.606074 haicu-0.0.96/setup.cfg
```

### Comparing `haicu-0.0.95/LICENSE` & `haicu-0.0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `haicu-0.0.95/PKG-INFO` & `haicu-0.0.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.0.95
-Summary: haicu package for HAICU
+Version: 0.0.96
+Summary: package for HAICU
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `haicu-0.0.95/README.md` & `haicu-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `haicu-0.0.95/haicu/__main__.py` & `haicu-0.0.96/haicu/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 import argparse
 import sys
 import random
 import time
 import configparser
 import os
 import pprint
+import pkg_resources
 from simplejson import dumps
-import ftdi as haicu_ftdi
-import format as haicu_format
+from . import ftdi as haicu_ftdi
+from . import format as haicu_format
 
-VERSION = "1.0"
+VERSION = pkg_resources.get_distribution('haicu').version
 
 # Table to convert 'get' request name to status register address
 GET_REG_TABLE = {
     'invert_frontpanel': 22,
     'invert_right_address': 21,
     'invert_left_address': 20,
     'invert_tunebox8': 19,
```

### Comparing `haicu-0.0.95/haicu/format.py` & `haicu-0.0.96/haicu/format.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import struct
 import csv
-from simplejson import dumps
 import pprint
+from simplejson import dumps
 
 MAX_RUN_ALLOWED_RLE = 8192  # 13-bit maximum in run-length encoding 'run' field
 
 def convert_derived2rle(derived_file_name):
     initial = []
     final = []
```

### Comparing `haicu-0.0.95/haicu/ftdi.py` & `haicu-0.0.96/haicu/ftdi.py`

 * *Files identical despite different names*

### Comparing `haicu-0.0.95/haicu.egg-info/PKG-INFO` & `haicu-0.0.96/haicu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.0.95
-Summary: haicu package for HAICU
+Version: 0.0.96
+Summary: package for HAICU
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `haicu-0.0.95/pyproject.toml` & `haicu-0.0.96/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "haicu"
-description = "haicu package for HAICU"
-version = "0.0.95"
+description = "package for HAICU"
+version = "0.0.96"
 authors = [
     { name = "Bryerton Shaw", email = "bryerton@triumf.ca" }
 ]
 maintainers = [
     { name = "Bryerton Shaw", email = "bryerton@triumf.ca" }
 ]
 readme.file = "README.md"
```

