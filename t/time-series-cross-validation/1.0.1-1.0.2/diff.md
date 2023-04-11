# Comparing `tmp/time_series_cross_validation-1.0.1.tar.gz` & `tmp/time_series_cross_validation-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series_cross_validation-1.0.1.tar", last modified: Tue Apr 11 21:10:05 2023, max compression
+gzip compressed data, was "time_series_cross_validation-1.0.2.tar", last modified: Tue Apr 11 21:14:35 2023, max compression
```

## Comparing `time_series_cross_validation-1.0.1.tar` & `time_series_cross_validation-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 21:10:05.376615 time_series_cross_validation-1.0.1/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     1085 2023-04-11 20:55:29.000000 time_series_cross_validation-1.0.1/LICENCE.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      561 2023-04-11 21:10:05.376615 time_series_cross_validation-1.0.1/PKG-INFO
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       35 2023-04-11 20:55:44.000000 time_series_cross_validation-1.0.1/README.md
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       38 2023-04-11 21:10:05.376615 time_series_cross_validation-1.0.1/setup.cfg
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      784 2023-04-11 21:09:54.000000 time_series_cross_validation-1.0.1/setup.py
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 21:10:05.372615 time_series_cross_validation-1.0.1/time_series_cross_validation/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       59 2023-04-11 20:57:49.000000 time_series_cross_validation-1.0.1/time_series_cross_validation/__init__.py
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     6152 2023-04-11 21:07:08.000000 time_series_cross_validation-1.0.1/time_series_cross_validation/mult_period_validation.py
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 21:10:05.376615 time_series_cross_validation-1.0.1/time_series_cross_validation.egg-info/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      561 2023-04-11 21:10:05.000000 time_series_cross_validation-1.0.1/time_series_cross_validation.egg-info/PKG-INFO
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      385 2023-04-11 21:10:05.000000 time_series_cross_validation-1.0.1/time_series_cross_validation.egg-info/SOURCES.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)        1 2023-04-11 21:10:05.000000 time_series_cross_validation-1.0.1/time_series_cross_validation.egg-info/dependency_links.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       32 2023-04-11 21:10:05.000000 time_series_cross_validation-1.0.1/time_series_cross_validation.egg-info/requires.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       29 2023-04-11 21:10:05.000000 time_series_cross_validation-1.0.1/time_series_cross_validation.egg-info/top_level.txt
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 21:14:35.466142 time_series_cross_validation-1.0.2/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     1085 2023-04-11 20:55:29.000000 time_series_cross_validation-1.0.2/LICENCE.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      561 2023-04-11 21:14:35.462142 time_series_cross_validation-1.0.2/PKG-INFO
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       35 2023-04-11 20:55:44.000000 time_series_cross_validation-1.0.2/README.md
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       38 2023-04-11 21:14:35.466142 time_series_cross_validation-1.0.2/setup.cfg
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      784 2023-04-11 21:14:16.000000 time_series_cross_validation-1.0.2/setup.py
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 21:14:35.462142 time_series_cross_validation-1.0.2/time_series_cross_validation/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       56 2023-04-11 21:13:00.000000 time_series_cross_validation-1.0.2/time_series_cross_validation/__init__.py
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     6143 2023-04-11 21:14:00.000000 time_series_cross_validation-1.0.2/time_series_cross_validation/time_series_cross_validation.py
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 21:14:35.462142 time_series_cross_validation-1.0.2/time_series_cross_validation.egg-info/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      561 2023-04-11 21:14:35.000000 time_series_cross_validation-1.0.2/time_series_cross_validation.egg-info/PKG-INFO
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      391 2023-04-11 21:14:35.000000 time_series_cross_validation-1.0.2/time_series_cross_validation.egg-info/SOURCES.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)        1 2023-04-11 21:14:35.000000 time_series_cross_validation-1.0.2/time_series_cross_validation.egg-info/dependency_links.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       32 2023-04-11 21:14:35.000000 time_series_cross_validation-1.0.2/time_series_cross_validation.egg-info/requires.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       29 2023-04-11 21:14:35.000000 time_series_cross_validation-1.0.2/time_series_cross_validation.egg-info/top_level.txt
```

### Comparing `time_series_cross_validation-1.0.1/LICENCE.txt` & `time_series_cross_validation-1.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `time_series_cross_validation-1.0.1/PKG-INFO` & `time_series_cross_validation-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time_series_cross_validation
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for cross-validating time series
 Home-page: https://github.com/biazotogabriel/deep_tracking
 Author: Gabriel Nuernberg Biazoto
 Author-email: biazotogabriel@gmail.com
 License: MIT
 Keywords: deep time series cross validation data science
 Classifier: Programming Language :: Python :: 3
```

### Comparing `time_series_cross_validation-1.0.1/setup.py` & `time_series_cross_validation-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='time_series_cross_validation',
-    version='1.0.1',
+    version='1.0.2',
     description='Library for cross-validating time series',
     long_description = 'Library for cross-validating time series',
     author='Gabriel Nuernberg Biazoto',
     author_email='biazotogabriel@gmail.com',
     url='https://github.com/biazotogabriel/deep_tracking',
     packages=['time_series_cross_validation'],
     license = 'MIT',
```

### Comparing `time_series_cross_validation-1.0.1/time_series_cross_validation/mult_period_validation.py` & `time_series_cross_validation-1.0.2/time_series_cross_validation/time_series_cross_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import matplotlib.pyplot as plt
 from datetime import timedelta, datetime
 import time
 from IPython.display import clear_output
 import threading
 import signal
 
-class Multi_period_validation:
+class Time_series_CV:
     def __init__(self, time_range, offset, k_folds=6,
                  test_size=None, min_test_size=None, max_test_size=None,
                  train_size=None, min_train_size=None):
         
         for parameter in [offset, test_size, min_test_size, max_test_size, train_size, min_train_size]:
             if not(isinstance(parameter, timedelta)) and parameter is not None: 
                 raise AttributeError('Please, argument must be a timedelta or None.')
```

### Comparing `time_series_cross_validation-1.0.1/time_series_cross_validation.egg-info/PKG-INFO` & `time_series_cross_validation-1.0.2/time_series_cross_validation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time-series-cross-validation
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for cross-validating time series
 Home-page: https://github.com/biazotogabriel/deep_tracking
 Author: Gabriel Nuernberg Biazoto
 Author-email: biazotogabriel@gmail.com
 License: MIT
 Keywords: deep time series cross validation data science
 Classifier: Programming Language :: Python :: 3
```

