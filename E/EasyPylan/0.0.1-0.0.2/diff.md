# Comparing `tmp/EasyPylan-0.0.1.tar.gz` & `tmp/EasyPylan-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyPylan-0.0.1.tar", last modified: Tue Apr 11 10:44:34 2023, max compression
+gzip compressed data, was "EasyPylan-0.0.2.tar", last modified: Tue Apr 11 10:56:42 2023, max compression
```

## Comparing `EasyPylan-0.0.1.tar` & `EasyPylan-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 10:44:34.753232 EasyPylan-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-11 10:44:34.753232 EasyPylan-0.0.1/EasyPylan.egg-info/
--rw-rw-rw-   0        0        0     1129 2023-04-11 10:44:34.000000 EasyPylan-0.0.1/EasyPylan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-04-11 10:44:34.000000 EasyPylan-0.0.1/EasyPylan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 10:44:34.000000 EasyPylan-0.0.1/EasyPylan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-04-11 10:44:34.000000 EasyPylan-0.0.1/EasyPylan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 10:44:34.000000 EasyPylan-0.0.1/EasyPylan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1075 2023-04-11 10:11:22.000000 EasyPylan-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1129 2023-04-11 10:44:34.753232 EasyPylan-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2021-06-06 11:11:49.000000 EasyPylan-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 10:44:34.759415 EasyPylan-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1482 2023-04-11 10:44:14.000000 EasyPylan-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 10:56:42.960460 EasyPylan-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-04-11 10:56:42.954097 EasyPylan-0.0.2/EasyPylan.egg-info/
+-rw-rw-rw-   0        0        0     1197 2023-04-11 10:56:42.000000 EasyPylan-0.0.2/EasyPylan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-04-11 10:56:42.000000 EasyPylan-0.0.2/EasyPylan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 10:56:42.000000 EasyPylan-0.0.2/EasyPylan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-04-11 10:56:42.000000 EasyPylan-0.0.2/EasyPylan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 10:56:42.000000 EasyPylan-0.0.2/EasyPylan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1075 2023-04-11 10:11:22.000000 EasyPylan-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1197 2023-04-11 10:56:42.957902 EasyPylan-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2021-06-06 11:11:49.000000 EasyPylan-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 10:56:42.960460 EasyPylan-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1543 2023-04-11 10:56:40.000000 EasyPylan-0.0.2/setup.py
```

### Comparing `EasyPylan-0.0.1/EasyPylan.egg-info/PKG-INFO` & `EasyPylan-0.0.2/EasyPylan.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyPylan
-Version: 0.0.1
+Version: 0.0.2
 Summary: EasyPyLan
 Author: Developer HelloUsers
 Author-email: duartesaopedrocat1@gmail.com
 Keywords: python,Pylan,pylan,EasyPython,EasyPyLan,easypylan
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -23,10 +23,17 @@
 you can change color of text, print on same line, delete and re-output again and many others, image process.
 It makes making 2d game easier you can scroll background with just one line of code, check user input, collide and many others.
 put image, and many others
 calculate any number like using calculate("2+2*4/5") and builtin bot
 
 turn text to speech and speech to text just on one of code
 
+some function
+
+Bot()
+calculate()
+re_output()
+resizeImage() 
+
 join on discord (Shiva321#1848) for update and help.
```

### Comparing `EasyPylan-0.0.1/LICENSE` & `EasyPylan-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `EasyPylan-0.0.1/PKG-INFO` & `EasyPylan-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyPylan
-Version: 0.0.1
+Version: 0.0.2
 Summary: EasyPyLan
 Author: Developer HelloUsers
 Author-email: duartesaopedrocat1@gmail.com
 Keywords: python,Pylan,pylan,EasyPython,EasyPyLan,easypylan
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -23,10 +23,17 @@
 you can change color of text, print on same line, delete and re-output again and many others, image process.
 It makes making 2d game easier you can scroll background with just one line of code, check user input, collide and many others.
 put image, and many others
 calculate any number like using calculate("2+2*4/5") and builtin bot
 
 turn text to speech and speech to text just on one of code
 
+some function
+
+Bot()
+calculate()
+re_output()
+resizeImage() 
+
 join on discord (Shiva321#1848) for update and help.
```

### Comparing `EasyPylan-0.0.1/README.md` & `EasyPylan-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `EasyPylan-0.0.1/setup.py` & `EasyPylan-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'EasyPyLan'
 LONG_DESCRIPTION = """
 Easy Python Language
 
 Helps you to make python easier and more understandable
 
 some example:
 you can change color of text, print on same line, delete and re-output again and many others, image process.
 It makes making 2d game easier you can scroll background with just one line of code, check user input, collide and many others.
 put image, and many others
 calculate any number like using calculate(\"2+2*4/5\") and builtin bot
 
 turn text to speech and speech to text just on one of code
 
+some function
+
+Bot()
+calculate()
+re_output()
+resizeImage() 
+
 join on discord (Shiva321#1848) for update and help.
 
 
 """
 
 # Setting up
 setup(
```

