# Comparing `tmp/HiPart-0.3.0.tar.gz` & `tmp/HiPart-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HiPart-0.3.0.tar", last modified: Wed Feb  1 15:10:14 2023, max compression
+gzip compressed data, was "HiPart-0.3.1.tar", last modified: Tue Apr 11 01:05:50 2023, max compression
```

## Comparing `HiPart-0.3.0.tar` & `HiPart-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:10:14.591225 HiPart-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-02-01 15:10:03.000000 HiPart-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-01 15:10:03.000000 HiPart-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-02-01 15:10:14.591225 HiPart-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-02-01 15:10:03.000000 HiPart-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-01 15:10:03.000000 HiPart-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 15:10:14.591225 HiPart-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-02-01 15:10:03.000000 HiPart-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:10:14.591225 HiPart-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:10:14.591225 HiPart-0.3.0/src/HiPart/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-02-01 15:10:03.000000 HiPart-0.3.0/src/HiPart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-02-01 15:10:03.000000 HiPart-0.3.0/src/HiPart/__utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:10:14.591225 HiPart-0.3.0/src/HiPart/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-02-01 15:10:03.000000 HiPart-0.3.0/src/HiPart/assets/int_viz.css
--rw-r--r--   0 runner    (1001) docker     (123)    71744 2023-02-01 15:10:03.000000 HiPart-0.3.0/src/HiPart/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    42704 2023-02-01 15:10:03.000000 HiPart-0.3.0/src/HiPart/interactive_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-02-01 15:10:03.000000 HiPart-0.3.0/src/HiPart/visualizations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:10:14.591225 HiPart-0.3.0/src/HiPart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-02-01 15:10:14.000000 HiPart-0.3.0/src/HiPart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-02-01 15:10:14.000000 HiPart-0.3.0/src/HiPart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 15:10:14.000000 HiPart-0.3.0/src/HiPart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-01 15:10:14.000000 HiPart-0.3.0/src/HiPart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-01 15:10:14.000000 HiPart-0.3.0/src/HiPart.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:05:50.461252 HiPart-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-11 01:05:40.000000 HiPart-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 01:05:40.000000 HiPart-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-11 01:05:50.461252 HiPart-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-04-11 01:05:40.000000 HiPart-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 01:05:40.000000 HiPart-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:05:50.461252 HiPart-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-11 01:05:40.000000 HiPart-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:05:50.457252 HiPart-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:05:50.461252 HiPart-0.3.1/src/HiPart/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-11 01:05:40.000000 HiPart-0.3.1/src/HiPart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-04-11 01:05:40.000000 HiPart-0.3.1/src/HiPart/__utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:05:50.461252 HiPart-0.3.1/src/HiPart/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-04-11 01:05:40.000000 HiPart-0.3.1/src/HiPart/assets/int_viz.css
+-rw-r--r--   0 runner    (1001) docker     (123)    71744 2023-04-11 01:05:40.000000 HiPart-0.3.1/src/HiPart/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42704 2023-04-11 01:05:40.000000 HiPart-0.3.1/src/HiPart/interactive_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-04-11 01:05:40.000000 HiPart-0.3.1/src/HiPart/visualizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:05:50.461252 HiPart-0.3.1/src/HiPart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-11 01:05:50.000000 HiPart-0.3.1/src/HiPart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-11 01:05:50.000000 HiPart-0.3.1/src/HiPart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:05:50.000000 HiPart-0.3.1/src/HiPart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-11 01:05:50.000000 HiPart-0.3.1/src/HiPart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 01:05:50.000000 HiPart-0.3.1/src/HiPart.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:05:50.461252 HiPart-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17298 2023-04-11 01:05:40.000000 HiPart-0.3.1/tests/test_package.py
```

### Comparing `HiPart-0.3.0/LICENSE` & `HiPart-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `HiPart-0.3.0/PKG-INFO` & `HiPart-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiPart
-Version: 0.3.0
+Version: 0.3.1
 Summary: A hierarchical divisive clustering toolbox
 Home-page: https://github.com/panagiotisanagnostou/HiPart
 Author: Panagiotis Anagnostou
 Author-email: panagno@uth.gr
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/panagiotisanagnostou/HiPart
 Keywords: data structure,tree,tools
```

### Comparing `HiPart-0.3.0/README.md` & `HiPart-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `HiPart-0.3.0/setup.py` & `HiPart-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 setuptools.setup(
     name="HiPart",
     version=__version__,
     url="https://github.com/panagiotisanagnostou/HiPart",
     author="Panagiotis Anagnostou",
     author_email="panagno@uth.gr",
```

### Comparing `HiPart-0.3.0/src/HiPart/__init__.py` & `HiPart-0.3.1/src/HiPart/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,13 +33,13 @@
 
 """
 
 from KDEpy.NaiveKDE import NaiveKDE
 from KDEpy.TreeKDE import TreeKDE
 from KDEpy.FFTKDE import FFTKDE
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __author__ = "Panagiotis Anagnostou"
 
 TreeKDE = TreeKDE
 NaiveKDE = NaiveKDE
 FFTKDE = FFTKDE
```

### Comparing `HiPart-0.3.0/src/HiPart/__utility_functions.py` & `HiPart-0.3.1/src/HiPart/__utility_functions.py`

 * *Files identical despite different names*

### Comparing `HiPart-0.3.0/src/HiPart/assets/int_viz.css` & `HiPart-0.3.1/src/HiPart/assets/int_viz.css`

 * *Files identical despite different names*

### Comparing `HiPart-0.3.0/src/HiPart/clustering.py` & `HiPart-0.3.1/src/HiPart/clustering.py`

 * *Files identical despite different names*

### Comparing `HiPart-0.3.0/src/HiPart/interactive_visualization.py` & `HiPart-0.3.1/src/HiPart/interactive_visualization.py`

 * *Files identical despite different names*

### Comparing `HiPart-0.3.0/src/HiPart/visualizations.py` & `HiPart-0.3.1/src/HiPart/visualizations.py`

 * *Files identical despite different names*

### Comparing `HiPart-0.3.0/src/HiPart.egg-info/PKG-INFO` & `HiPart-0.3.1/src/HiPart.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiPart
-Version: 0.3.0
+Version: 0.3.1
 Summary: A hierarchical divisive clustering toolbox
 Home-page: https://github.com/panagiotisanagnostou/HiPart
 Author: Panagiotis Anagnostou
 Author-email: panagno@uth.gr
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/panagiotisanagnostou/HiPart
 Keywords: data structure,tree,tools
```

