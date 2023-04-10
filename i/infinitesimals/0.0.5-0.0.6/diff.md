# Comparing `tmp/infinitesimals-0.0.5.tar.gz` & `tmp/infinitesimals-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infinitesimals-0.0.5.tar", last modified: Mon Apr 10 22:14:17 2023, max compression
+gzip compressed data, was "infinitesimals-0.0.6.tar", last modified: Mon Apr 10 22:23:20 2023, max compression
```

## Comparing `infinitesimals-0.0.5.tar` & `infinitesimals-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 22:14:17.582971 infinitesimals-0.0.5/
--rw-rw-rw-   0        0        0      363 2023-04-10 22:13:50.000000 infinitesimals-0.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 infinitesimals-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-10 19:18:21.000000 infinitesimals-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1108 2023-04-10 22:14:17.581973 infinitesimals-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      100 2023-04-10 19:05:04.000000 infinitesimals-0.0.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 22:14:17.561030 infinitesimals-0.0.5/infinitesimals/
--rw-rw-rw-   0        0        0        0 2023-04-10 21:59:32.000000 infinitesimals-0.0.5/infinitesimals/__init__.py
--rw-rw-rw-   0        0        0     3279 2023-04-10 22:01:57.000000 infinitesimals-0.0.5/infinitesimals/example.py
--rw-rw-rw-   0        0        0    10188 2023-04-10 20:45:12.000000 infinitesimals-0.0.5/infinitesimals/infinitesimals.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:14:17.580976 infinitesimals-0.0.5/infinitesimals.egg-info/
--rw-rw-rw-   0        0        0     1108 2023-04-10 22:14:17.000000 infinitesimals-0.0.5/infinitesimals.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-04-10 22:14:17.000000 infinitesimals-0.0.5/infinitesimals.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 22:14:17.000000 infinitesimals-0.0.5/infinitesimals.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-10 22:14:17.000000 infinitesimals-0.0.5/infinitesimals.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-10 22:14:17.000000 infinitesimals-0.0.5/infinitesimals.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 22:14:17.582971 infinitesimals-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      893 2023-04-10 22:13:50.000000 infinitesimals-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:23:20.605577 infinitesimals-0.0.6/
+-rw-rw-rw-   0        0        0      152 2023-04-10 22:22:53.000000 infinitesimals-0.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 infinitesimals-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-10 19:18:21.000000 infinitesimals-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      897 2023-04-10 22:23:20.604579 infinitesimals-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      100 2023-04-10 19:05:04.000000 infinitesimals-0.0.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 22:23:20.584632 infinitesimals-0.0.6/infinitesimals/
+-rw-rw-rw-   0        0        0    10188 2023-04-10 22:21:37.000000 infinitesimals-0.0.6/infinitesimals/__init__.py
+-rw-rw-rw-   0        0        0     3285 2023-04-10 22:22:37.000000 infinitesimals-0.0.6/infinitesimals/example.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:23:20.603582 infinitesimals-0.0.6/infinitesimals.egg-info/
+-rw-rw-rw-   0        0        0      897 2023-04-10 22:23:20.000000 infinitesimals-0.0.6/infinitesimals.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-10 22:23:20.000000 infinitesimals-0.0.6/infinitesimals.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 22:23:20.000000 infinitesimals-0.0.6/infinitesimals.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-10 22:23:20.000000 infinitesimals-0.0.6/infinitesimals.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 22:23:20.000000 infinitesimals-0.0.6/infinitesimals.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 22:23:20.605577 infinitesimals-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      893 2023-04-10 22:23:16.000000 infinitesimals-0.0.6/setup.py
```

### Comparing `infinitesimals-0.0.5/LICENSE.txt` & `infinitesimals-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `infinitesimals-0.0.5/PKG-INFO` & `infinitesimals-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infinitesimals
-Version: 0.0.5
+Version: 0.0.6
 Summary: A capable HyperReal class and related methods for work with infinitesimals and nonstandard analysis.
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,infinitesimal,infinitesimals,hyperreal,analysis,nonstandard analysis
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,22 +19,10 @@
 Change Log
 ==========
 
 0.0.1 (10/04/2023)
 ------------------
 - First Release
 
-0.0.2 (10/04/2023)
--------------------
-- Fixed install_requires
-
-0.0.3 (10/04/2023)
--------------------
-- Fixed __init__ directory
-
-0.0.4 (10/04/2023)
--------------------
-- Fixed __init__ directory
-
-0.0.4 (10/04/2023)
+0.0.6 (10/04/2023)
 -------------------
 - Fixed __init__ directory
```

### Comparing `infinitesimals-0.0.5/infinitesimals/example.py` & `infinitesimals-0.0.6/infinitesimals/example.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import infinitesimals
-from infinitesimals import *
+import __init__ as infinitesimals
+from __init__ import *
 from math import floor, ceil
 from sys import float_info
 
 """Example program for demonstrating the capabilities of the infinitesimal library"""
 
 
 def main():
```

### Comparing `infinitesimals-0.0.5/infinitesimals/infinitesimals.py` & `infinitesimals-0.0.6/infinitesimals/__init__.py`

 * *Files identical despite different names*

### Comparing `infinitesimals-0.0.5/infinitesimals.egg-info/PKG-INFO` & `infinitesimals-0.0.6/infinitesimals.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infinitesimals
-Version: 0.0.5
+Version: 0.0.6
 Summary: A capable HyperReal class and related methods for work with infinitesimals and nonstandard analysis.
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,infinitesimal,infinitesimals,hyperreal,analysis,nonstandard analysis
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,22 +19,10 @@
 Change Log
 ==========
 
 0.0.1 (10/04/2023)
 ------------------
 - First Release
 
-0.0.2 (10/04/2023)
--------------------
-- Fixed install_requires
-
-0.0.3 (10/04/2023)
--------------------
-- Fixed __init__ directory
-
-0.0.4 (10/04/2023)
--------------------
-- Fixed __init__ directory
-
-0.0.4 (10/04/2023)
+0.0.6 (10/04/2023)
 -------------------
 - Fixed __init__ directory
```

### Comparing `infinitesimals-0.0.5/setup.py` & `infinitesimals-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='infinitesimals',
-    version='0.0.5',
+    version='0.0.6',
     description='A capable HyperReal class and related methods for work with infinitesimals and nonstandard analysis.',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Lyam Boylan',
     author_email='lyamboylan@gmail.com',
     license='MIT',
     keywords=['math', 'infinitesimal', 'infinitesimals', 'hyperreal', 'analysis', 'nonstandard analysis'],
```

