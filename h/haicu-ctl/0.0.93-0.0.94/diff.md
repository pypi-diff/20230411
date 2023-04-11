# Comparing `tmp/haicu-ctl-0.0.93.tar.gz` & `tmp/haicu-ctl-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haicu-ctl-0.0.93.tar", last modified: Tue Apr 11 18:08:44 2023, max compression
+gzip compressed data, was "haicu-ctl-0.0.94.tar", last modified: Tue Apr 11 18:10:17 2023, max compression
```

## Comparing `haicu-ctl-0.0.93.tar` & `haicu-ctl-0.0.94.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:08:44.036716 haicu-ctl-0.0.93/
--rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-ctl-0.0.93/LICENSE
--rw-rw-r--   0 bry       (1000) bry       (1000)     2601 2023-04-11 18:08:44.036716 haicu-ctl-0.0.93/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)     1073 2023-04-11 17:00:57.000000 haicu-ctl-0.0.93/README.md
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:08:44.032716 haicu-ctl-0.0.93/haicu_ctl/
--rw-rw-r--   0 bry       (1000) bry       (1000)        0 2023-03-10 00:08:52.000000 haicu-ctl-0.0.93/haicu_ctl/__init__.py
--rwxrwxr-x   0 bry       (1000) bry       (1000)    28653 2023-04-11 16:56:01.000000 haicu-ctl-0.0.93/haicu_ctl/__main__.py
--rw-rw-r--   0 bry       (1000) bry       (1000)    28669 2023-04-11 17:00:50.000000 haicu-ctl-0.0.93/haicu_ctl/haicu_ctl.py
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:08:44.032716 haicu-ctl-0.0.93/haicu_ctl.egg-info/
--rw-rw-r--   0 bry       (1000) bry       (1000)     2601 2023-04-11 18:08:44.000000 haicu-ctl-0.0.93/haicu_ctl.egg-info/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)      299 2023-04-11 18:08:44.000000 haicu-ctl-0.0.93/haicu_ctl.egg-info/SOURCES.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-04-11 18:08:44.000000 haicu-ctl-0.0.93/haicu_ctl.egg-info/dependency_links.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       54 2023-04-11 18:08:44.000000 haicu-ctl-0.0.93/haicu_ctl.egg-info/entry_points.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       35 2023-04-11 18:08:44.000000 haicu-ctl-0.0.93/haicu_ctl.egg-info/requires.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       10 2023-04-11 18:08:44.000000 haicu-ctl-0.0.93/haicu_ctl.egg-info/top_level.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)      734 2023-04-11 18:08:33.000000 haicu-ctl-0.0.93/pyproject.toml
--rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-04-11 18:08:44.036716 haicu-ctl-0.0.93/setup.cfg
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:10:17.748837 haicu-ctl-0.0.94/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-ctl-0.0.94/LICENSE
+-rw-rw-r--   0 bry       (1000) bry       (1000)     2601 2023-04-11 18:10:17.748837 haicu-ctl-0.0.94/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)     1073 2023-04-11 17:00:57.000000 haicu-ctl-0.0.94/README.md
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:10:17.748837 haicu-ctl-0.0.94/haicu_ctl/
+-rw-rw-r--   0 bry       (1000) bry       (1000)        0 2023-03-10 00:08:52.000000 haicu-ctl-0.0.94/haicu_ctl/__init__.py
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    28645 2023-04-11 18:09:46.000000 haicu-ctl-0.0.94/haicu_ctl/__main__.py
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:10:17.748837 haicu-ctl-0.0.94/haicu_ctl.egg-info/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     2601 2023-04-11 18:10:17.000000 haicu-ctl-0.0.94/haicu_ctl.egg-info/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)      276 2023-04-11 18:10:17.000000 haicu-ctl-0.0.94/haicu_ctl.egg-info/SOURCES.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-04-11 18:10:17.000000 haicu-ctl-0.0.94/haicu_ctl.egg-info/dependency_links.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       54 2023-04-11 18:10:17.000000 haicu-ctl-0.0.94/haicu_ctl.egg-info/entry_points.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       35 2023-04-11 18:10:17.000000 haicu-ctl-0.0.94/haicu_ctl.egg-info/requires.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       10 2023-04-11 18:10:17.000000 haicu-ctl-0.0.94/haicu_ctl.egg-info/top_level.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)      734 2023-04-11 18:10:07.000000 haicu-ctl-0.0.94/pyproject.toml
+-rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-04-11 18:10:17.748837 haicu-ctl-0.0.94/setup.cfg
```

### Comparing `haicu-ctl-0.0.93/LICENSE` & `haicu-ctl-0.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `haicu-ctl-0.0.93/PKG-INFO` & `haicu-ctl-0.0.94/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu-ctl
-Version: 0.0.93
+Version: 0.0.94
 Summary: haicu-ctl package for HAICU
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

### Comparing `haicu-ctl-0.0.93/README.md` & `haicu-ctl-0.0.94/README.md`

 * *Files identical despite different names*

### Comparing `haicu-ctl-0.0.93/haicu_ctl/__main__.py` & `haicu-ctl-0.0.94/haicu_ctl/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import sys
 import random
 import time
 import configparser
 import os
 import pprint
 from simplejson import dumps
-from haicu_ctl import ftdi as haicu_ftdi
-from haicu_ctl import format as haicu_format
+from haicu import ftdi as haicu_ftdi
+from haicu import format as haicu_format
 
 VERSION = "1.0"
 
 # Table to convert 'get' request name to status register address
 GET_REG_TABLE = {
     'invert_frontpanel': 22,
     'invert_right_address': 21,
```

### Comparing `haicu-ctl-0.0.93/haicu_ctl.egg-info/PKG-INFO` & `haicu-ctl-0.0.94/haicu_ctl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu-ctl
-Version: 0.0.93
+Version: 0.0.94
 Summary: haicu-ctl package for HAICU
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

### Comparing `haicu-ctl-0.0.93/pyproject.toml` & `haicu-ctl-0.0.94/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "haicu-ctl"
 description = "haicu-ctl package for HAICU"
-version = "0.0.93"
+version = "0.0.94"
 authors = [
     { name = "Bryerton Shaw", email = "bryerton@triumf.ca" }
 ]
 maintainers = [
     { name = "Bryerton Shaw", email = "bryerton@triumf.ca" }
 ]
 readme.file = "README.md"
```

