# Comparing `tmp/infinitesimals-0.0.4.tar.gz` & `tmp/infinitesimals-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infinitesimals-0.0.4.tar", last modified: Mon Apr 10 22:04:28 2023, max compression
+gzip compressed data, was "infinitesimals-0.0.5.tar", last modified: Mon Apr 10 22:14:17 2023, max compression
```

## Comparing `infinitesimals-0.0.4.tar` & `infinitesimals-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 22:04:28.211332 infinitesimals-0.0.4/
--rw-rw-rw-   0        0        0      292 2023-04-10 22:04:22.000000 infinitesimals-0.0.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 infinitesimals-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-10 19:18:21.000000 infinitesimals-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1037 2023-04-10 22:04:28.209338 infinitesimals-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      100 2023-04-10 19:05:04.000000 infinitesimals-0.0.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 22:04:28.202356 infinitesimals-0.0.4/infinitesimals.egg-info/
--rw-rw-rw-   0        0        0     1037 2023-04-10 22:04:28.000000 infinitesimals-0.0.4/infinitesimals.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-10 22:04:28.000000 infinitesimals-0.0.4/infinitesimals.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 22:04:28.000000 infinitesimals-0.0.4/infinitesimals.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-10 22:04:28.000000 infinitesimals-0.0.4/infinitesimals.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-10 22:04:28.000000 infinitesimals-0.0.4/infinitesimals.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 22:04:28.211332 infinitesimals-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      893 2023-04-10 22:01:49.000000 infinitesimals-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:04:28.208340 infinitesimals-0.0.4/src/
--rw-rw-rw-   0        0        0        0 2023-04-10 21:59:32.000000 infinitesimals-0.0.4/src/__init__.py
--rw-rw-rw-   0        0        0     3279 2023-04-10 22:01:57.000000 infinitesimals-0.0.4/src/example.py
--rw-rw-rw-   0        0        0    10188 2023-04-10 20:45:12.000000 infinitesimals-0.0.4/src/infinitesimals.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:14:17.582971 infinitesimals-0.0.5/
+-rw-rw-rw-   0        0        0      363 2023-04-10 22:13:50.000000 infinitesimals-0.0.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 infinitesimals-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-10 19:18:21.000000 infinitesimals-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1108 2023-04-10 22:14:17.581973 infinitesimals-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      100 2023-04-10 19:05:04.000000 infinitesimals-0.0.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 22:14:17.561030 infinitesimals-0.0.5/infinitesimals/
+-rw-rw-rw-   0        0        0        0 2023-04-10 21:59:32.000000 infinitesimals-0.0.5/infinitesimals/__init__.py
+-rw-rw-rw-   0        0        0     3279 2023-04-10 22:01:57.000000 infinitesimals-0.0.5/infinitesimals/example.py
+-rw-rw-rw-   0        0        0    10188 2023-04-10 20:45:12.000000 infinitesimals-0.0.5/infinitesimals/infinitesimals.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:14:17.580976 infinitesimals-0.0.5/infinitesimals.egg-info/
+-rw-rw-rw-   0        0        0     1108 2023-04-10 22:14:17.000000 infinitesimals-0.0.5/infinitesimals.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-04-10 22:14:17.000000 infinitesimals-0.0.5/infinitesimals.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 22:14:17.000000 infinitesimals-0.0.5/infinitesimals.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-10 22:14:17.000000 infinitesimals-0.0.5/infinitesimals.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 22:14:17.000000 infinitesimals-0.0.5/infinitesimals.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 22:14:17.582971 infinitesimals-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      893 2023-04-10 22:13:50.000000 infinitesimals-0.0.5/setup.py
```

### Comparing `infinitesimals-0.0.4/LICENSE.txt` & `infinitesimals-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `infinitesimals-0.0.4/PKG-INFO` & `infinitesimals-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infinitesimals
-Version: 0.0.4
+Version: 0.0.5
 Summary: A capable HyperReal class and related methods for work with infinitesimals and nonstandard analysis.
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,infinitesimal,infinitesimals,hyperreal,analysis,nonstandard analysis
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -30,7 +30,11 @@
 0.0.3 (10/04/2023)
 -------------------
 - Fixed __init__ directory
 
 0.0.4 (10/04/2023)
 -------------------
 - Fixed __init__ directory
+
+0.0.4 (10/04/2023)
+-------------------
+- Fixed __init__ directory
```

### Comparing `infinitesimals-0.0.4/infinitesimals.egg-info/PKG-INFO` & `infinitesimals-0.0.5/infinitesimals.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infinitesimals
-Version: 0.0.4
+Version: 0.0.5
 Summary: A capable HyperReal class and related methods for work with infinitesimals and nonstandard analysis.
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,infinitesimal,infinitesimals,hyperreal,analysis,nonstandard analysis
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -30,7 +30,11 @@
 0.0.3 (10/04/2023)
 -------------------
 - Fixed __init__ directory
 
 0.0.4 (10/04/2023)
 -------------------
 - Fixed __init__ directory
+
+0.0.4 (10/04/2023)
+-------------------
+- Fixed __init__ directory
```

### Comparing `infinitesimals-0.0.4/setup.py` & `infinitesimals-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='infinitesimals',
-    version='0.0.4',
+    version='0.0.5',
     description='A capable HyperReal class and related methods for work with infinitesimals and nonstandard analysis.',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Lyam Boylan',
     author_email='lyamboylan@gmail.com',
     license='MIT',
     keywords=['math', 'infinitesimal', 'infinitesimals', 'hyperreal', 'analysis', 'nonstandard analysis'],
```

### Comparing `infinitesimals-0.0.4/src/example.py` & `infinitesimals-0.0.5/infinitesimals/example.py`

 * *Files identical despite different names*

### Comparing `infinitesimals-0.0.4/src/infinitesimals.py` & `infinitesimals-0.0.5/infinitesimals/infinitesimals.py`

 * *Files identical despite different names*

