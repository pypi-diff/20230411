# Comparing `tmp/kondo_ml-0.0.4.tar.gz` & `tmp/kondo_ml-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kondo_ml-0.0.4.tar", last modified: Tue Apr 11 13:03:41 2023, max compression
+gzip compressed data, was "kondo_ml-0.0.5.tar", last modified: Tue Apr 11 13:22:41 2023, max compression
```

## Comparing `kondo_ml-0.0.4.tar` & `kondo_ml-0.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:03:41.013064 kondo_ml-0.0.4/
--rw-r--r--   0 rueck      (501) staff       (20)     1062 2023-03-06 04:08:33.000000 kondo_ml-0.0.4/LICENSE
--rw-r--r--   0 rueck      (501) staff       (20)      874 2023-04-11 13:03:41.012452 kondo_ml-0.0.4/PKG-INFO
--rw-r--r--   0 rueck      (501) staff       (20)      203 2023-04-11 10:02:29.000000 kondo_ml-0.0.4/README.md
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:03:40.982921 kondo_ml-0.0.4/kondo_ml/
--rw-r--r--   0 rueck      (501) staff       (20)      548 2023-04-11 13:03:28.000000 kondo_ml-0.0.4/kondo_ml/__init__.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:03:41.000987 kondo_ml-0.0.4/kondo_ml/instance_selection/
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:03:41.004372 kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/
--rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/__init__.py
--rw-r--r--   0 rueck      (501) staff       (20)     4284 2023-03-29 14:30:04.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/datasets.py
--rw-r--r--   0 rueck      (501) staff       (20)    30404 2023-03-29 14:30:04.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/linear.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:03:41.008020 kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/model/
--rw-r--r--   0 rueck      (501) staff       (20)     1182 2023-01-06 11:10:15.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/model/LinearRegression.py
--rw-r--r--   0 rueck      (501) staff       (20)    42909 2023-03-29 14:30:04.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/model/SELCON.py
--rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/model/__init__.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:03:41.011404 kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/utils/
--rw-r--r--   0 rueck      (501) staff       (20)    13606 2023-01-06 11:10:15.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py
--rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/utils/__init__.py
--rw-r--r--   0 rueck      (501) staff       (20)    14724 2023-01-06 11:10:15.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py
--rw-r--r--   0 rueck      (501) staff       (20)     4355 2023-01-06 11:10:15.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/utils/time_series.py
--rw-r--r--   0 rueck      (501) staff       (20)      894 2023-03-29 14:07:55.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/__init__.py
--rw-r--r--   0 rueck      (501) staff       (20)    21369 2023-04-11 13:03:10.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/_drop.py
--rw-r--r--   0 rueck      (501) staff       (20)     5394 2023-04-11 13:03:10.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/_fish.py
--rw-r--r--   0 rueck      (501) staff       (20)     1884 2023-03-21 13:25:30.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/_fixed_time_window.py
--rw-r--r--   0 rueck      (501) staff       (20)      747 2023-03-27 12:15:14.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/_full_set.py
--rw-r--r--   0 rueck      (501) staff       (20)     3292 2023-02-28 20:37:58.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/_gradient_shapley.py
--rw-r--r--   0 rueck      (501) staff       (20)      709 2023-02-07 23:08:48.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/_local_outlier_factor.py
--rw-r--r--   0 rueck      (501) staff       (20)     2923 2023-03-28 17:07:35.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/_mutual_information.py
--rw-r--r--   0 rueck      (501) staff       (20)      755 2023-02-24 21:17:58.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/_random_selection.py
--rw-r--r--   0 rueck      (501) staff       (20)     3277 2023-03-28 17:28:54.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/_reg_CNN.py
--rw-r--r--   0 rueck      (501) staff       (20)     8480 2023-04-11 13:03:10.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/_reg_ENN.py
--rw-r--r--   0 rueck      (501) staff       (20)     1382 2023-03-29 14:30:04.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/_selcon.py
--rw-r--r--   0 rueck      (501) staff       (20)      859 2023-02-17 14:38:57.000000 kondo_ml-0.0.4/kondo_ml/instance_selection/base.py
--rw-r--r--   0 rueck      (501) staff       (20)      460 2023-03-29 14:04:12.000000 kondo_ml-0.0.4/kondo_ml/kondo_ml.py
--rw-r--r--   0 rueck      (501) staff       (20)     1713 2023-03-21 13:36:29.000000 kondo_ml-0.0.4/kondo_ml/utils.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:03:40.986210 kondo_ml-0.0.4/kondo_ml.egg-info/
--rw-r--r--   0 rueck      (501) staff       (20)      874 2023-04-11 13:03:40.000000 kondo_ml-0.0.4/kondo_ml.egg-info/PKG-INFO
--rw-r--r--   0 rueck      (501) staff       (20)     1352 2023-04-11 13:03:40.000000 kondo_ml-0.0.4/kondo_ml.egg-info/SOURCES.txt
--rw-r--r--   0 rueck      (501) staff       (20)        1 2023-04-11 13:03:40.000000 kondo_ml-0.0.4/kondo_ml.egg-info/dependency_links.txt
--rw-r--r--   0 rueck      (501) staff       (20)       32 2023-04-11 13:03:40.000000 kondo_ml-0.0.4/kondo_ml.egg-info/requires.txt
--rw-r--r--   0 rueck      (501) staff       (20)        9 2023-04-11 13:03:40.000000 kondo_ml-0.0.4/kondo_ml.egg-info/top_level.txt
--rw-r--r--   0 rueck      (501) staff       (20)      620 2023-04-11 13:03:28.000000 kondo_ml-0.0.4/pyproject.toml
--rw-r--r--   0 rueck      (501) staff       (20)       38 2023-04-11 13:03:41.013250 kondo_ml-0.0.4/setup.cfg
--rw-r--r--   0 rueck      (501) staff       (20)     1874 2023-04-11 10:45:56.000000 kondo_ml-0.0.4/setup.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:22:41.807948 kondo_ml-0.0.5/
+-rw-r--r--   0 rueck      (501) staff       (20)     1062 2023-03-06 04:08:33.000000 kondo_ml-0.0.5/LICENSE
+-rw-r--r--   0 rueck      (501) staff       (20)      874 2023-04-11 13:22:41.805916 kondo_ml-0.0.5/PKG-INFO
+-rw-r--r--   0 rueck      (501) staff       (20)      203 2023-04-11 10:02:29.000000 kondo_ml-0.0.5/README.md
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:22:41.772849 kondo_ml-0.0.5/kondo_ml/
+-rw-r--r--   0 rueck      (501) staff       (20)      548 2023-04-11 13:22:25.000000 kondo_ml-0.0.5/kondo_ml/__init__.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:22:41.790703 kondo_ml-0.0.5/kondo_ml/instance_selection/
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:22:41.792705 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/
+-rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/__init__.py
+-rw-r--r--   0 rueck      (501) staff       (20)     4284 2023-03-29 14:30:04.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/datasets.py
+-rw-r--r--   0 rueck      (501) staff       (20)    30404 2023-03-29 14:30:04.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/linear.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:22:41.798341 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/model/
+-rw-r--r--   0 rueck      (501) staff       (20)     1182 2023-01-06 11:10:15.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/model/LinearRegression.py
+-rw-r--r--   0 rueck      (501) staff       (20)    42909 2023-03-29 14:30:04.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/model/SELCON.py
+-rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/model/__init__.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:22:41.802602 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/
+-rw-r--r--   0 rueck      (501) staff       (20)    13606 2023-01-06 11:10:15.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py
+-rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/__init__.py
+-rw-r--r--   0 rueck      (501) staff       (20)    14724 2023-01-06 11:10:15.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py
+-rw-r--r--   0 rueck      (501) staff       (20)     4355 2023-01-06 11:10:15.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/time_series.py
+-rw-r--r--   0 rueck      (501) staff       (20)      894 2023-03-29 14:07:55.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/__init__.py
+-rw-r--r--   0 rueck      (501) staff       (20)    21369 2023-04-11 13:03:10.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_drop.py
+-rw-r--r--   0 rueck      (501) staff       (20)     5394 2023-04-11 13:03:10.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_fish.py
+-rw-r--r--   0 rueck      (501) staff       (20)     1884 2023-03-21 13:25:30.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_fixed_time_window.py
+-rw-r--r--   0 rueck      (501) staff       (20)      747 2023-03-27 12:15:14.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_full_set.py
+-rw-r--r--   0 rueck      (501) staff       (20)     3292 2023-02-28 20:37:58.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_gradient_shapley.py
+-rw-r--r--   0 rueck      (501) staff       (20)      709 2023-02-07 23:08:48.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_local_outlier_factor.py
+-rw-r--r--   0 rueck      (501) staff       (20)     2923 2023-03-28 17:07:35.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_mutual_information.py
+-rw-r--r--   0 rueck      (501) staff       (20)      755 2023-02-24 21:17:58.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_random_selection.py
+-rw-r--r--   0 rueck      (501) staff       (20)     3277 2023-03-28 17:28:54.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_reg_CNN.py
+-rw-r--r--   0 rueck      (501) staff       (20)     8480 2023-04-11 13:03:10.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_reg_ENN.py
+-rw-r--r--   0 rueck      (501) staff       (20)     1382 2023-03-29 14:30:04.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_selcon.py
+-rw-r--r--   0 rueck      (501) staff       (20)      859 2023-02-17 14:38:57.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/base.py
+-rw-r--r--   0 rueck      (501) staff       (20)      460 2023-03-29 14:04:12.000000 kondo_ml-0.0.5/kondo_ml/kondo_ml.py
+-rw-r--r--   0 rueck      (501) staff       (20)     1713 2023-03-21 13:36:29.000000 kondo_ml-0.0.5/kondo_ml/utils.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:22:41.776126 kondo_ml-0.0.5/kondo_ml.egg-info/
+-rw-r--r--   0 rueck      (501) staff       (20)      874 2023-04-11 13:22:41.000000 kondo_ml-0.0.5/kondo_ml.egg-info/PKG-INFO
+-rw-r--r--   0 rueck      (501) staff       (20)     1352 2023-04-11 13:22:41.000000 kondo_ml-0.0.5/kondo_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 rueck      (501) staff       (20)        1 2023-04-11 13:22:41.000000 kondo_ml-0.0.5/kondo_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 rueck      (501) staff       (20)       32 2023-04-11 13:22:41.000000 kondo_ml-0.0.5/kondo_ml.egg-info/requires.txt
+-rw-r--r--   0 rueck      (501) staff       (20)        9 2023-04-11 13:22:41.000000 kondo_ml-0.0.5/kondo_ml.egg-info/top_level.txt
+-rw-r--r--   0 rueck      (501) staff       (20)      620 2023-04-11 13:22:25.000000 kondo_ml-0.0.5/pyproject.toml
+-rw-r--r--   0 rueck      (501) staff       (20)       38 2023-04-11 13:22:41.808144 kondo_ml-0.0.5/setup.cfg
+-rw-r--r--   0 rueck      (501) staff       (20)     1874 2023-04-11 10:45:56.000000 kondo_ml-0.0.5/setup.py
```

### Comparing `kondo_ml-0.0.4/LICENSE` & `kondo_ml-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/PKG-INFO` & `kondo_ml-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kondo_ml
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for instance selection algorithms
 Home-page: https://github.com/lurue101/instance-selection-for-regression
-Download-URL: https://github.com/lurue101/instance-selection-for-regression/archive/0.0.4.tar.gz
+Download-URL: https://github.com/lurue101/instance-selection-for-regression/archive/0.0.5.tar.gz
 Author: L.Rücker
 Author-email: Lukas Rücker <ruecker.lukas@gmail.com>
 Project-URL: Homepage, https://github.com/lurue101/instance-selection-for-regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `kondo_ml-0.0.4/kondo_ml/__init__.py` & `kondo_ml-0.0.5/kondo_ml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from kondo_ml.kondo_ml import KondoMLPackage
 
 __author__ = 'Lukas Rücker'
 __email__ = 'ruecker.lukas@gmail.com'
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 
 # module level doc-string
 __doc__ = """
 Kondo-ML
 ================
 
 Description
```

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/datasets.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/datasets.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/linear.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/linear.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/model/LinearRegression.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/model/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/model/SELCON.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/model/SELCON.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/SELCON/utils/time_series.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/time_series.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/__init__.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/_drop.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/_drop.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/_fish.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/_fish.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/_fixed_time_window.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/_fixed_time_window.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/_full_set.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/_full_set.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/_gradient_shapley.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/_gradient_shapley.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/_local_outlier_factor.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/_local_outlier_factor.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/_mutual_information.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/_mutual_information.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/_random_selection.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/_random_selection.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/_reg_CNN.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/_reg_CNN.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/_reg_ENN.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/_reg_ENN.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/_selcon.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/_selcon.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/instance_selection/base.py` & `kondo_ml-0.0.5/kondo_ml/instance_selection/base.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml/utils.py` & `kondo_ml-0.0.5/kondo_ml/utils.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/kondo_ml.egg-info/PKG-INFO` & `kondo_ml-0.0.5/kondo_ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kondo-ml
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for instance selection algorithms
 Home-page: https://github.com/lurue101/instance-selection-for-regression
-Download-URL: https://github.com/lurue101/instance-selection-for-regression/archive/0.0.4.tar.gz
+Download-URL: https://github.com/lurue101/instance-selection-for-regression/archive/0.0.5.tar.gz
 Author: L.Rücker
 Author-email: Lukas Rücker <ruecker.lukas@gmail.com>
 Project-URL: Homepage, https://github.com/lurue101/instance-selection-for-regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `kondo_ml-0.0.4/kondo_ml.egg-info/SOURCES.txt` & `kondo_ml-0.0.5/kondo_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.4/pyproject.toml` & `kondo_ml-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kondo_ml"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Lukas Rücker", email="ruecker.lukas@gmail.com" },
 ]
 description = "Python package for instance selection algorithms"
 readme = "README.md"
 dependencies = ['numpy','pandas','scikit-learn','torch']
 requires-python = ">=3.7"
```

### Comparing `kondo_ml-0.0.4/setup.py` & `kondo_ml-0.0.5/setup.py`

 * *Files identical despite different names*

