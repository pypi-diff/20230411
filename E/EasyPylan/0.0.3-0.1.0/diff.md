# Comparing `tmp/EasyPylan-0.0.3.tar.gz` & `tmp/EasyPylan-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyPylan-0.0.3.tar", last modified: Tue Apr 11 11:05:39 2023, max compression
+gzip compressed data, was "EasyPylan-0.1.0.tar", last modified: Tue Apr 11 11:08:08 2023, max compression
```

## Comparing `EasyPylan-0.0.3.tar` & `EasyPylan-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 11:05:39.194750 EasyPylan-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-04-11 11:05:39.189367 EasyPylan-0.0.3/EasyPylan.egg-info/
--rw-rw-rw-   0        0        0     1193 2023-04-11 11:05:39.000000 EasyPylan-0.0.3/EasyPylan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-04-11 11:05:39.000000 EasyPylan-0.0.3/EasyPylan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 11:05:39.000000 EasyPylan-0.0.3/EasyPylan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-04-11 11:05:39.000000 EasyPylan-0.0.3/EasyPylan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 11:05:39.000000 EasyPylan-0.0.3/EasyPylan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1075 2023-04-11 10:11:22.000000 EasyPylan-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1193 2023-04-11 11:05:39.193744 EasyPylan-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2021-06-06 11:11:49.000000 EasyPylan-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 11:05:39.194750 EasyPylan-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1539 2023-04-11 11:05:30.000000 EasyPylan-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:08:08.362477 EasyPylan-0.1.0/
+drwxrwxrwx   0        0        0        0 2023-04-11 11:08:08.358498 EasyPylan-0.1.0/EasyPylan.egg-info/
+-rw-rw-rw-   0        0        0     1197 2023-04-11 11:08:08.000000 EasyPylan-0.1.0/EasyPylan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-04-11 11:08:08.000000 EasyPylan-0.1.0/EasyPylan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 11:08:08.000000 EasyPylan-0.1.0/EasyPylan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-04-11 11:08:08.000000 EasyPylan-0.1.0/EasyPylan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 11:08:08.000000 EasyPylan-0.1.0/EasyPylan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1075 2023-04-11 10:11:22.000000 EasyPylan-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1197 2023-04-11 11:08:08.359751 EasyPylan-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2021-06-06 11:11:49.000000 EasyPylan-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 11:08:08.362477 EasyPylan-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1543 2023-04-11 11:07:54.000000 EasyPylan-0.1.0/setup.py
```

### Comparing `EasyPylan-0.0.3/EasyPylan.egg-info/PKG-INFO` & `EasyPylan-0.1.0/EasyPylan.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: EasyPylan
-Version: 0.0.3
-Summary: PyLan
+Version: 0.1.0
+Summary: EasyPyLan
 Author: Developer HelloUsers
 Author-email: duartesaopedrocat1@gmail.com
 Keywords: python,Pylan,pylan,EasyPython,EasyPyLan,easypylan
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `EasyPylan-0.0.3/LICENSE` & `EasyPylan-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EasyPylan-0.0.3/PKG-INFO` & `EasyPylan-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: EasyPylan
-Version: 0.0.3
-Summary: PyLan
+Version: 0.1.0
+Summary: EasyPyLan
 Author: Developer HelloUsers
 Author-email: duartesaopedrocat1@gmail.com
 Keywords: python,Pylan,pylan,EasyPython,EasyPyLan,easypylan
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `EasyPylan-0.0.3/README.md` & `EasyPylan-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `EasyPylan-0.0.3/setup.py` & `EasyPylan-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.3'
-DESCRIPTION = 'PyLan'
+VERSION = '0.1.0'
+DESCRIPTION = 'EasyPyLan'
 LONG_DESCRIPTION = """
 Easy Python Language
 
 Helps you to make python easier and more understandable
 
 some example:
 you can change color of text, print on same line, delete and re-output again and many others, image process.
```

