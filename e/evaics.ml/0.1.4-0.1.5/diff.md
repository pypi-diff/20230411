# Comparing `tmp/evaics.ml-0.1.4.tar.gz` & `tmp/evaics.ml-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evaics.ml-0.1.4.tar", last modified: Mon Apr 10 20:34:37 2023, max compression
+gzip compressed data, was "evaics.ml-0.1.5.tar", last modified: Tue Apr 11 00:25:58 2023, max compression
```

## Comparing `evaics.ml-0.1.4.tar` & `evaics.ml-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-10 20:34:37.887184 evaics.ml-0.1.4/
--rw-r--r--   0 divisor   (1000) root         (0)    11357 2023-03-29 17:24:22.000000 evaics.ml-0.1.4/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)      711 2023-04-10 20:34:37.887184 evaics.ml-0.1.4/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      136 2023-04-08 21:45:24.000000 evaics.ml-0.1.4/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-10 20:34:37.887184 evaics.ml-0.1.4/evaics/
--rw-r--r--   0 divisor   (1000) root         (0)        0 2023-04-10 20:34:34.000000 evaics.ml-0.1.4/evaics/__init__.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-10 20:34:37.887184 evaics.ml-0.1.4/evaics/ml/
--rw-r--r--   0 divisor   (1000) root         (0)    15851 2023-04-10 20:34:34.000000 evaics.ml-0.1.4/evaics/ml/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)    12572 2023-04-10 20:34:34.000000 evaics.ml-0.1.4/evaics/ml/learning.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-10 20:34:37.887184 evaics.ml-0.1.4/evaics.ml.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)      711 2023-04-10 20:34:37.000000 evaics.ml-0.1.4/evaics.ml.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      253 2023-04-10 20:34:37.000000 evaics.ml-0.1.4/evaics.ml.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2023-04-10 20:34:37.000000 evaics.ml-0.1.4/evaics.ml.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)       60 2023-04-10 20:34:37.000000 evaics.ml-0.1.4/evaics.ml.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)        7 2023-04-10 20:34:37.000000 evaics.ml-0.1.4/evaics.ml.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2023-04-10 20:34:37.887184 evaics.ml-0.1.4/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)      918 2023-04-10 20:34:34.000000 evaics.ml-0.1.4/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-11 00:25:58.459288 evaics.ml-0.1.5/
+-rw-r--r--   0 divisor   (1000) root         (0)    11357 2023-03-29 17:24:22.000000 evaics.ml-0.1.5/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)      711 2023-04-11 00:25:58.459288 evaics.ml-0.1.5/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      136 2023-04-08 21:45:24.000000 evaics.ml-0.1.5/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-11 00:25:58.459288 evaics.ml-0.1.5/evaics/
+-rw-r--r--   0 divisor   (1000) root         (0)        0 2023-04-11 00:25:53.000000 evaics.ml-0.1.5/evaics/__init__.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-11 00:25:58.459288 evaics.ml-0.1.5/evaics/ml/
+-rw-r--r--   0 divisor   (1000) root         (0)    15866 2023-04-11 00:25:53.000000 evaics.ml-0.1.5/evaics/ml/__init__.py
+-rw-r--r--   0 divisor   (1000) root         (0)    12572 2023-04-11 00:25:53.000000 evaics.ml-0.1.5/evaics/ml/learning.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-11 00:25:58.459288 evaics.ml-0.1.5/evaics.ml.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)      711 2023-04-11 00:25:58.000000 evaics.ml-0.1.5/evaics.ml.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      253 2023-04-11 00:25:58.000000 evaics.ml-0.1.5/evaics.ml.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2023-04-11 00:25:58.000000 evaics.ml-0.1.5/evaics.ml.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       60 2023-04-11 00:25:58.000000 evaics.ml-0.1.5/evaics.ml.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        7 2023-04-11 00:25:58.000000 evaics.ml-0.1.5/evaics.ml.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2023-04-11 00:25:58.459288 evaics.ml-0.1.5/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)      918 2023-04-11 00:25:53.000000 evaics.ml-0.1.5/setup.py
```

### Comparing `evaics.ml-0.1.4/LICENSE` & `evaics.ml-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `evaics.ml-0.1.4/PKG-INFO` & `evaics.ml-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evaics.ml
-Version: 0.1.4
+Version: 0.1.5
 Summary: EVA ICS v4 Machine Learning Kit
 Home-page: https://github.com/eva-ics/eva-mlkit-client-python
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `evaics.ml-0.1.4/evaics/ml/__init__.py` & `evaics.ml-0.1.5/evaics/ml/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 import sys
 import requests
 import gzip
 import logging
 import time
 import json
@@ -376,25 +376,25 @@
                 data[col] = stats.pop(f'{oid}/value')
         return pa.Table.from_pydict(data)
 
     def fetch(self,
               t_col: str = 'keep',
               tz: str = 'local',
               output='arrow',
-              strict_col_order=False):
+              strict_col_order=True):
         """
         Fetch data
 
         Optional:
             output: output format (arrow, pandas or polars)
             t_col: time column processing, "keep" - keep the column, "drop" -
             drop the time column
             tz: time zone (local, custom or None to keep time column as UNIX
             timestamp), the default is "local"
-            strict_col_order: force strict column ordering
+            strict_col_order: force strict column ordering (default: True)
 
 
         Returns:
             a prepared Pandas DataFrame object
         """
         if t_col not in ['keep', 'drop']:
             raise RuntimeError('unsupported t_col op')
```

### Comparing `evaics.ml-0.1.4/evaics/ml/learning.py` & `evaics.ml-0.1.5/evaics/ml/learning.py`

 * *Files identical despite different names*

### Comparing `evaics.ml-0.1.4/evaics.ml.egg-info/PKG-INFO` & `evaics.ml-0.1.5/evaics.ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evaics.ml
-Version: 0.1.4
+Version: 0.1.5
 Summary: EVA ICS v4 Machine Learning Kit
 Home-page: https://github.com/eva-ics/eva-mlkit-client-python
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `evaics.ml-0.1.4/setup.py` & `evaics.ml-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
```

