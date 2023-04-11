# Comparing `tmp/EasyPythonLanguage-1.0.0.tar.gz` & `tmp/EasyPythonLanguage-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyPythonLanguage-1.0.0.tar", last modified: Tue Apr 11 11:35:34 2023, max compression
+gzip compressed data, was "EasyPythonLanguage-1.0.1.tar", last modified: Tue Apr 11 11:57:54 2023, max compression
```

## Comparing `EasyPythonLanguage-1.0.0.tar` & `EasyPythonLanguage-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 11:35:34.276385 EasyPythonLanguage-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-04-11 11:35:34.271489 EasyPythonLanguage-1.0.0/EasyPythonLanguage.egg-info/
--rw-rw-rw-   0        0        0     1250 2023-04-11 11:35:34.000000 EasyPythonLanguage-1.0.0/EasyPythonLanguage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-11 11:35:34.000000 EasyPythonLanguage-1.0.0/EasyPythonLanguage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 11:35:34.000000 EasyPythonLanguage-1.0.0/EasyPythonLanguage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-04-11 11:35:34.000000 EasyPythonLanguage-1.0.0/EasyPythonLanguage.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-11 11:35:34.000000 EasyPythonLanguage-1.0.0/EasyPythonLanguage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1075 2023-04-11 10:11:22.000000 EasyPythonLanguage-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1250 2023-04-11 11:35:34.276385 EasyPythonLanguage-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 11:35:34.274797 EasyPythonLanguage-1.0.0/PyLan/
--rw-rw-rw-   0        0        0      163 2023-04-11 11:33:22.000000 EasyPythonLanguage-1.0.0/PyLan/__init__.py
--rw-rw-rw-   0        0        0     1456 2021-06-06 11:11:49.000000 EasyPythonLanguage-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 11:35:34.276385 EasyPythonLanguage-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1604 2023-04-11 11:35:22.000000 EasyPythonLanguage-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:57:54.305532 EasyPythonLanguage-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-04-11 11:57:54.298737 EasyPythonLanguage-1.0.1/EasyPythonLanguage.egg-info/
+-rw-rw-rw-   0        0        0     1250 2023-04-11 11:57:54.000000 EasyPythonLanguage-1.0.1/EasyPythonLanguage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-11 11:57:54.000000 EasyPythonLanguage-1.0.1/EasyPythonLanguage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 11:57:54.000000 EasyPythonLanguage-1.0.1/EasyPythonLanguage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-04-11 11:57:54.000000 EasyPythonLanguage-1.0.1/EasyPythonLanguage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-11 11:57:54.000000 EasyPythonLanguage-1.0.1/EasyPythonLanguage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1075 2023-04-11 10:11:22.000000 EasyPythonLanguage-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1250 2023-04-11 11:57:54.304037 EasyPythonLanguage-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 11:57:54.301912 EasyPythonLanguage-1.0.1/PyLan/
+-rw-rw-rw-   0        0        0    21065 2023-04-11 11:53:52.000000 EasyPythonLanguage-1.0.1/PyLan/__init__.py
+-rw-rw-rw-   0        0        0     1456 2021-06-06 11:11:49.000000 EasyPythonLanguage-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 11:57:54.306883 EasyPythonLanguage-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1604 2023-04-11 11:57:40.000000 EasyPythonLanguage-1.0.1/setup.py
```

### Comparing `EasyPythonLanguage-1.0.0/EasyPythonLanguage.egg-info/PKG-INFO` & `EasyPythonLanguage-1.0.1/EasyPythonLanguage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyPythonLanguage
-Version: 1.0.0
+Version: 1.0.1
 Summary: EasyPythonLanguage
 Author: Developer HelloUsers
 Author-email: duartesaopedrocat1@gmail.com
 Keywords: python,Pylan,pylan,EasyPython,EasyPyLan,easypylan,pygame,game,image
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EasyPythonLanguage-1.0.0/LICENSE` & `EasyPythonLanguage-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `EasyPythonLanguage-1.0.0/PKG-INFO` & `EasyPythonLanguage-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyPythonLanguage
-Version: 1.0.0
+Version: 1.0.1
 Summary: EasyPythonLanguage
 Author: Developer HelloUsers
 Author-email: duartesaopedrocat1@gmail.com
 Keywords: python,Pylan,pylan,EasyPython,EasyPyLan,easypylan,pygame,game,image
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EasyPythonLanguage-1.0.0/README.md` & `EasyPythonLanguage-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `EasyPythonLanguage-1.0.0/setup.py` & `EasyPythonLanguage-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'EasyPythonLanguage'
 LONG_DESCRIPTION = """
 Easy Python Language
 
 Helps you to make python easier and more understandable
 
 some example:
```

