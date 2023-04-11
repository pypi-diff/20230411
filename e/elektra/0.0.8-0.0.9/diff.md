# Comparing `tmp/elektra-0.0.8.tar.gz` & `tmp/elektra-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/elektra-0.0.8.tar", last modified: Fri Mar  5 21:43:49 2021, max compression
+gzip compressed data, was "dist/elektra-0.0.9.tar", last modified: Fri Mar  5 21:52:34 2021, max compression
```

## Comparing `elektra-0.0.8.tar` & `elektra-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 paulkaisharis  (1000) paulkaisharis  (1000)        0 2021-03-05 21:43:49.574634 elektra-0.0.8/
--rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)     5729 2021-03-05 21:43:49.570634 elektra-0.0.8/PKG-INFO
--rw-r--r--   0 paulkaisharis  (1000) paulkaisharis  (1000)     4835 2020-12-10 17:09:25.000000 elektra-0.0.8/README.md
-drwxrwxr-x   0 paulkaisharis  (1000) paulkaisharis  (1000)        0 2021-03-05 21:43:49.570634 elektra-0.0.8/elektra.egg-info/
--rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)     5729 2021-03-05 21:43:49.000000 elektra-0.0.8/elektra.egg-info/PKG-INFO
--rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)      204 2021-03-05 21:43:49.000000 elektra-0.0.8/elektra.egg-info/SOURCES.txt
--rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)        1 2021-03-05 21:43:49.000000 elektra-0.0.8/elektra.egg-info/dependency_links.txt
--rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)       28 2021-03-05 21:43:49.000000 elektra-0.0.8/elektra.egg-info/requires.txt
--rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)        6 2021-03-05 21:43:49.000000 elektra-0.0.8/elektra.egg-info/top_level.txt
--rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)       38 2021-03-05 21:43:49.574634 elektra-0.0.8/setup.cfg
--rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)      558 2021-03-05 21:43:43.000000 elektra-0.0.8/setup.py
-drwxrwxr-x   0 paulkaisharis  (1000) paulkaisharis  (1000)        0 2021-03-05 21:43:49.570634 elektra-0.0.8/tests/
--rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)        0 2020-10-21 17:38:58.000000 elektra-0.0.8/tests/__init__.py
--rw-r--r--   0 paulkaisharis  (1000) paulkaisharis  (1000)     1264 2020-10-21 19:06:30.000000 elektra-0.0.8/tests/test.py
+drwxrwxr-x   0 paulkaisharis  (1000) paulkaisharis  (1000)        0 2021-03-05 21:52:34.559405 elektra-0.0.9/
+-rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)     5729 2021-03-05 21:52:34.559405 elektra-0.0.9/PKG-INFO
+-rw-r--r--   0 paulkaisharis  (1000) paulkaisharis  (1000)     4835 2020-12-10 17:09:25.000000 elektra-0.0.9/README.md
+drwxrwxr-x   0 paulkaisharis  (1000) paulkaisharis  (1000)        0 2021-03-05 21:52:34.559405 elektra-0.0.9/elektra.egg-info/
+-rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)     5729 2021-03-05 21:52:34.000000 elektra-0.0.9/elektra.egg-info/PKG-INFO
+-rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)      204 2021-03-05 21:52:34.000000 elektra-0.0.9/elektra.egg-info/SOURCES.txt
+-rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)        1 2021-03-05 21:52:34.000000 elektra-0.0.9/elektra.egg-info/dependency_links.txt
+-rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)       28 2021-03-05 21:52:34.000000 elektra-0.0.9/elektra.egg-info/requires.txt
+-rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)        6 2021-03-05 21:52:34.000000 elektra-0.0.9/elektra.egg-info/top_level.txt
+-rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)       38 2021-03-05 21:52:34.559405 elektra-0.0.9/setup.cfg
+-rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)      558 2021-03-05 21:47:15.000000 elektra-0.0.9/setup.py
+drwxrwxr-x   0 paulkaisharis  (1000) paulkaisharis  (1000)        0 2021-03-05 21:52:34.559405 elektra-0.0.9/tests/
+-rw-rw-r--   0 paulkaisharis  (1000) paulkaisharis  (1000)        0 2020-10-21 17:38:58.000000 elektra-0.0.9/tests/__init__.py
+-rw-r--r--   0 paulkaisharis  (1000) paulkaisharis  (1000)     1264 2020-10-21 19:06:30.000000 elektra-0.0.9/tests/test.py
```

### Comparing `elektra-0.0.8/PKG-INFO` & `elektra-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elektra
-Version: 0.0.8
+Version: 0.0.9
 Summary: Power block price creation and conversion
 Home-page: https://github.com/wearemolecule/elektra
 Author: Molecule
 Author-email: devs@molecule.io
 License: MIT
 Description: # elektra
```

### Comparing `elektra-0.0.8/README.md` & `elektra-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `elektra-0.0.8/elektra.egg-info/PKG-INFO` & `elektra-0.0.9/elektra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elektra
-Version: 0.0.8
+Version: 0.0.9
 Summary: Power block price creation and conversion
 Home-page: https://github.com/wearemolecule/elektra
 Author: Molecule
 Author-email: devs@molecule.io
 License: MIT
 Description: # elektra
```

### Comparing `elektra-0.0.8/setup.py` & `elektra-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     README = fh.read()
 
 setuptools.setup(
     name="elektra",
-    version="0.0.8",
+    version="0.0.9",
     author="Molecule",
     author_email="devs@molecule.io",
     description="Power block price creation and conversion",
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/wearemolecule/elektra',
     packages=setuptools.find_packages(),
```

### Comparing `elektra-0.0.8/tests/test.py` & `elektra-0.0.9/tests/test.py`

 * *Files identical despite different names*

