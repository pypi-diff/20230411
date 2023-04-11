# Comparing `tmp/cgal-5.5.post202210041706.tar.gz` & `tmp/cgal-5.5.post202210051748.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgal-5.5.post202210041706.tar", last modified: Tue Oct  4 15:56:03 2022, max compression
+gzip compressed data, was "cgal-5.5.post202210051748.tar", last modified: Wed Oct  5 16:13:44 2022, max compression
```

## Comparing `cgal-5.5.post202210041706.tar` & `cgal-5.5.post202210051748.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 15:56:03.702389 cgal-5.5.post202210041706/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-04 15:55:54.000000 cgal-5.5.post202210041706/LICENSE.COMMERCIAL
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-10-04 15:55:54.000000 cgal-5.5.post202210041706/LICENSE.GPL
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-10-04 15:56:03.702389 cgal-5.5.post202210041706/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-10-04 15:55:54.000000 cgal-5.5.post202210041706/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 15:56:03.702389 cgal-5.5.post202210041706/cgal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-10-04 15:56:03.000000 cgal-5.5.post202210041706/cgal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-10-04 15:56:03.000000 cgal-5.5.post202210041706/cgal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-04 15:56:03.000000 cgal-5.5.post202210041706/cgal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-04 15:56:03.000000 cgal-5.5.post202210041706/cgal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-10-04 15:56:03.000000 cgal-5.5.post202210041706/cgal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-04 15:56:03.702389 cgal-5.5.post202210041706/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    17025 2022-10-04 15:55:54.000000 cgal-5.5.post202210041706/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 16:13:44.071141 cgal-5.5.post202210051748/
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-05 16:13:29.000000 cgal-5.5.post202210051748/LICENSE.COMMERCIAL
+-rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-10-05 16:13:29.000000 cgal-5.5.post202210051748/LICENSE.GPL
+-rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-10-05 16:13:44.071141 cgal-5.5.post202210051748/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2022-10-05 16:13:29.000000 cgal-5.5.post202210051748/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 16:13:44.071141 cgal-5.5.post202210051748/cgal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-10-05 16:13:43.000000 cgal-5.5.post202210051748/cgal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-10-05 16:13:43.000000 cgal-5.5.post202210051748/cgal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 16:13:43.000000 cgal-5.5.post202210051748/cgal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-05 16:13:43.000000 cgal-5.5.post202210051748/cgal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-10-05 16:13:43.000000 cgal-5.5.post202210051748/cgal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-05 16:13:44.071141 cgal-5.5.post202210051748/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)    17025 2022-10-05 16:13:29.000000 cgal-5.5.post202210051748/setup.py
```

### Comparing `cgal-5.5.post202210041706/LICENSE.GPL` & `cgal-5.5.post202210051748/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `cgal-5.5.post202210041706/PKG-INFO` & `cgal-5.5.post202210051748/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgal
-Version: 5.5.post202210041706
+Version: 5.5.post202210051748
 Summary: CGAL bindings, allowing to use some of the CGAL library in python.
 Home-page: https://github.com/CGAL/cgal-swig-bindings
 Author: CGAL Project
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `cgal-5.5.post202210041706/cgal.egg-info/PKG-INFO` & `cgal-5.5.post202210051748/cgal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgal
-Version: 5.5.post202210041706
+Version: 5.5.post202210051748
 Summary: CGAL bindings, allowing to use some of the CGAL library in python.
 Home-page: https://github.com/CGAL/cgal-swig-bindings
 Author: CGAL Project
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `cgal-5.5.post202210041706/cgal.egg-info/top_level.txt` & `cgal-5.5.post202210051748/cgal.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `cgal-5.5.post202210041706/setup.py` & `cgal-5.5.post202210051748/setup.py`

 * *Files identical despite different names*

