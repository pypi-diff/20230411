# Comparing `tmp/kondo_ml-0.0.1.tar.gz` & `tmp/kondo_ml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kondo_ml-0.0.1.tar", last modified: Tue Apr 11 09:46:22 2023, max compression
+gzip compressed data, was "kondo_ml-0.0.2.tar", last modified: Tue Apr 11 10:31:44 2023, max compression
```

## Comparing `kondo_ml-0.0.1.tar` & `kondo_ml-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 09:46:22.432697 kondo_ml-0.0.1/
--rw-r--r--   0 rueck      (501) staff       (20)     1062 2023-03-06 04:08:33.000000 kondo_ml-0.0.1/LICENSE
--rw-r--r--   0 rueck      (501) staff       (20)     1041 2023-04-11 09:46:22.430416 kondo_ml-0.0.1/PKG-INFO
--rw-r--r--   0 rueck      (501) staff       (20)      413 2023-03-06 04:14:38.000000 kondo_ml-0.0.1/README.md
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 09:46:22.396327 kondo_ml-0.0.1/kondo_ml/
--rw-r--r--   0 rueck      (501) staff       (20)      729 2023-03-29 14:04:12.000000 kondo_ml-0.0.1/kondo_ml/__init__.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 09:46:22.413650 kondo_ml-0.0.1/kondo_ml/instance_selection/
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 09:46:22.418016 kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/
--rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/__init__.py
--rw-r--r--   0 rueck      (501) staff       (20)     4284 2023-03-29 14:30:04.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/datasets.py
--rw-r--r--   0 rueck      (501) staff       (20)    30404 2023-03-29 14:30:04.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/linear.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 09:46:22.424361 kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/model/
--rw-r--r--   0 rueck      (501) staff       (20)     1182 2023-01-06 11:10:15.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/model/LinearRegression.py
--rw-r--r--   0 rueck      (501) staff       (20)    42909 2023-03-29 14:30:04.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/model/SELCON.py
--rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/model/__init__.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 09:46:22.428697 kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/utils/
--rw-r--r--   0 rueck      (501) staff       (20)    13606 2023-01-06 11:10:15.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py
--rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/utils/__init__.py
--rw-r--r--   0 rueck      (501) staff       (20)    14724 2023-01-06 11:10:15.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py
--rw-r--r--   0 rueck      (501) staff       (20)     4355 2023-01-06 11:10:15.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/utils/time_series.py
--rw-r--r--   0 rueck      (501) staff       (20)      894 2023-03-29 14:07:55.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/__init__.py
--rw-r--r--   0 rueck      (501) staff       (20)    21360 2023-03-29 14:06:59.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/_drop.py
--rw-r--r--   0 rueck      (501) staff       (20)     5385 2023-03-29 14:06:59.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/_fish.py
--rw-r--r--   0 rueck      (501) staff       (20)     1884 2023-03-21 13:25:30.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/_fixed_time_window.py
--rw-r--r--   0 rueck      (501) staff       (20)      747 2023-03-27 12:15:14.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/_full_set.py
--rw-r--r--   0 rueck      (501) staff       (20)     3292 2023-02-28 20:37:58.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/_gradient_shapley.py
--rw-r--r--   0 rueck      (501) staff       (20)      709 2023-02-07 23:08:48.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/_local_outlier_factor.py
--rw-r--r--   0 rueck      (501) staff       (20)     2923 2023-03-28 17:07:35.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/_mutual_information.py
--rw-r--r--   0 rueck      (501) staff       (20)      755 2023-02-24 21:17:58.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/_random_selection.py
--rw-r--r--   0 rueck      (501) staff       (20)     3277 2023-03-28 17:28:54.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/_reg_CNN.py
--rw-r--r--   0 rueck      (501) staff       (20)     8471 2023-03-29 14:06:59.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/_reg_ENN.py
--rw-r--r--   0 rueck      (501) staff       (20)     1382 2023-03-29 14:30:04.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/_selcon.py
--rw-r--r--   0 rueck      (501) staff       (20)      859 2023-02-17 14:38:57.000000 kondo_ml-0.0.1/kondo_ml/instance_selection/base.py
--rw-r--r--   0 rueck      (501) staff       (20)      460 2023-03-29 14:04:12.000000 kondo_ml-0.0.1/kondo_ml/kondo_ml.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 09:46:22.400137 kondo_ml-0.0.1/kondo_ml.egg-info/
--rw-r--r--   0 rueck      (501) staff       (20)     1041 2023-04-11 09:46:22.000000 kondo_ml-0.0.1/kondo_ml.egg-info/PKG-INFO
--rw-r--r--   0 rueck      (501) staff       (20)     1334 2023-04-11 09:46:22.000000 kondo_ml-0.0.1/kondo_ml.egg-info/SOURCES.txt
--rw-r--r--   0 rueck      (501) staff       (20)        1 2023-04-11 09:46:22.000000 kondo_ml-0.0.1/kondo_ml.egg-info/dependency_links.txt
--rw-r--r--   0 rueck      (501) staff       (20)       32 2023-04-11 09:46:22.000000 kondo_ml-0.0.1/kondo_ml.egg-info/requires.txt
--rw-r--r--   0 rueck      (501) staff       (20)        9 2023-04-11 09:46:22.000000 kondo_ml-0.0.1/kondo_ml.egg-info/top_level.txt
--rw-r--r--   0 rueck      (501) staff       (20)      595 2023-04-11 09:39:06.000000 kondo_ml-0.0.1/pyproject.toml
--rw-r--r--   0 rueck      (501) staff       (20)       38 2023-04-11 09:46:22.433019 kondo_ml-0.0.1/setup.cfg
--rw-r--r--   0 rueck      (501) staff       (20)     1859 2023-03-29 14:30:04.000000 kondo_ml-0.0.1/setup.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 10:31:44.058964 kondo_ml-0.0.2/
+-rw-r--r--   0 rueck      (501) staff       (20)     1062 2023-03-06 04:08:33.000000 kondo_ml-0.0.2/LICENSE
+-rw-r--r--   0 rueck      (501) staff       (20)      849 2023-04-11 10:31:44.058351 kondo_ml-0.0.2/PKG-INFO
+-rw-r--r--   0 rueck      (501) staff       (20)      203 2023-04-11 10:02:29.000000 kondo_ml-0.0.2/README.md
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 10:31:44.036127 kondo_ml-0.0.2/kondo_ml/
+-rw-r--r--   0 rueck      (501) staff       (20)      539 2023-04-11 10:27:11.000000 kondo_ml-0.0.2/kondo_ml/__init__.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 10:31:44.050975 kondo_ml-0.0.2/kondo_ml/instance_selection/
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 10:31:44.053013 kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/
+-rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/__init__.py
+-rw-r--r--   0 rueck      (501) staff       (20)     4284 2023-03-29 14:30:04.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/datasets.py
+-rw-r--r--   0 rueck      (501) staff       (20)    30404 2023-03-29 14:30:04.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/linear.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 10:31:44.055265 kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/model/
+-rw-r--r--   0 rueck      (501) staff       (20)     1182 2023-01-06 11:10:15.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/model/LinearRegression.py
+-rw-r--r--   0 rueck      (501) staff       (20)    42909 2023-03-29 14:30:04.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/model/SELCON.py
+-rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/model/__init__.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 10:31:44.057608 kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/utils/
+-rw-r--r--   0 rueck      (501) staff       (20)    13606 2023-01-06 11:10:15.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py
+-rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/utils/__init__.py
+-rw-r--r--   0 rueck      (501) staff       (20)    14724 2023-01-06 11:10:15.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py
+-rw-r--r--   0 rueck      (501) staff       (20)     4355 2023-01-06 11:10:15.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/utils/time_series.py
+-rw-r--r--   0 rueck      (501) staff       (20)      894 2023-03-29 14:07:55.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/__init__.py
+-rw-r--r--   0 rueck      (501) staff       (20)    21360 2023-03-29 14:06:59.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/_drop.py
+-rw-r--r--   0 rueck      (501) staff       (20)     5385 2023-03-29 14:06:59.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/_fish.py
+-rw-r--r--   0 rueck      (501) staff       (20)     1884 2023-03-21 13:25:30.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/_fixed_time_window.py
+-rw-r--r--   0 rueck      (501) staff       (20)      747 2023-03-27 12:15:14.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/_full_set.py
+-rw-r--r--   0 rueck      (501) staff       (20)     3292 2023-02-28 20:37:58.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/_gradient_shapley.py
+-rw-r--r--   0 rueck      (501) staff       (20)      709 2023-02-07 23:08:48.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/_local_outlier_factor.py
+-rw-r--r--   0 rueck      (501) staff       (20)     2923 2023-03-28 17:07:35.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/_mutual_information.py
+-rw-r--r--   0 rueck      (501) staff       (20)      755 2023-02-24 21:17:58.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/_random_selection.py
+-rw-r--r--   0 rueck      (501) staff       (20)     3277 2023-03-28 17:28:54.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/_reg_CNN.py
+-rw-r--r--   0 rueck      (501) staff       (20)     8471 2023-03-29 14:06:59.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/_reg_ENN.py
+-rw-r--r--   0 rueck      (501) staff       (20)     1382 2023-03-29 14:30:04.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/_selcon.py
+-rw-r--r--   0 rueck      (501) staff       (20)      859 2023-02-17 14:38:57.000000 kondo_ml-0.0.2/kondo_ml/instance_selection/base.py
+-rw-r--r--   0 rueck      (501) staff       (20)      460 2023-03-29 14:04:12.000000 kondo_ml-0.0.2/kondo_ml/kondo_ml.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 10:31:44.039761 kondo_ml-0.0.2/kondo_ml.egg-info/
+-rw-r--r--   0 rueck      (501) staff       (20)      849 2023-04-11 10:31:44.000000 kondo_ml-0.0.2/kondo_ml.egg-info/PKG-INFO
+-rw-r--r--   0 rueck      (501) staff       (20)     1334 2023-04-11 10:31:44.000000 kondo_ml-0.0.2/kondo_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 rueck      (501) staff       (20)        1 2023-04-11 10:31:44.000000 kondo_ml-0.0.2/kondo_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 rueck      (501) staff       (20)       32 2023-04-11 10:31:44.000000 kondo_ml-0.0.2/kondo_ml.egg-info/requires.txt
+-rw-r--r--   0 rueck      (501) staff       (20)        9 2023-04-11 10:31:44.000000 kondo_ml-0.0.2/kondo_ml.egg-info/top_level.txt
+-rw-r--r--   0 rueck      (501) staff       (20)      595 2023-04-11 10:31:31.000000 kondo_ml-0.0.2/pyproject.toml
+-rw-r--r--   0 rueck      (501) staff       (20)       38 2023-04-11 10:31:44.059325 kondo_ml-0.0.2/setup.cfg
+-rw-r--r--   0 rueck      (501) staff       (20)     1877 2023-04-11 10:17:34.000000 kondo_ml-0.0.2/setup.py
```

### Comparing `kondo_ml-0.0.1/LICENSE` & `kondo_ml-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/PKG-INFO` & `kondo_ml-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: kondo_ml
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/lurue101/instance-selection-for-regression
-Download-URL: https://github.com/erdogant/relevantpackage/archive/0.0.1.tar.gz
+Download-URL: https://github.com/lurue101/instance-selection-for-regression/archive/0.0.2.tar.gz
 Author: L.Rücker
 Author-email: Lukas Rücker <ruecker.lukas@gmail.com>
 Project-URL: Homepage, https://github.com/lurue101/instance-selection-for-regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# instance-selection-for-regression
-This repo contains the code for various instance selection algorithms
-usable with regression models. The implementations are compatible with sklearn and follow
-its outlier detection interface.
-The repo is not yet finished. More documentation and examples will be added soon.
+# kondo-ML
 
-The SelCon algorithm is taken from the authors and their repo here: https://github.com/abir-de/SELCOn
+kondo-ML is a package containing various instance selection algorithms
+usable with regression modelsThe implementations are compatible with sklearn and follow
+its outlier detection interface.
```

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/datasets.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/datasets.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/linear.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/linear.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/model/LinearRegression.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/model/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/model/SELCON.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/model/SELCON.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/SELCON/utils/time_series.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/SELCON/utils/time_series.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/__init__.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/_drop.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/_drop.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/_fish.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/_fish.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/_fixed_time_window.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/_fixed_time_window.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/_full_set.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/_full_set.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/_gradient_shapley.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/_gradient_shapley.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/_local_outlier_factor.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/_local_outlier_factor.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/_mutual_information.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/_mutual_information.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/_random_selection.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/_random_selection.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/_reg_CNN.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/_reg_CNN.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/_reg_ENN.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/_reg_ENN.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/_selcon.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/_selcon.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml/instance_selection/base.py` & `kondo_ml-0.0.2/kondo_ml/instance_selection/base.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/kondo_ml.egg-info/PKG-INFO` & `kondo_ml-0.0.2/kondo_ml.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: kondo-ml
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/lurue101/instance-selection-for-regression
-Download-URL: https://github.com/erdogant/relevantpackage/archive/0.0.1.tar.gz
+Download-URL: https://github.com/lurue101/instance-selection-for-regression/archive/0.0.2.tar.gz
 Author: L.Rücker
 Author-email: Lukas Rücker <ruecker.lukas@gmail.com>
 Project-URL: Homepage, https://github.com/lurue101/instance-selection-for-regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# instance-selection-for-regression
-This repo contains the code for various instance selection algorithms
-usable with regression models. The implementations are compatible with sklearn and follow
-its outlier detection interface.
-The repo is not yet finished. More documentation and examples will be added soon.
+# kondo-ML
 
-The SelCon algorithm is taken from the authors and their repo here: https://github.com/abir-de/SELCOn
+kondo-ML is a package containing various instance selection algorithms
+usable with regression modelsThe implementations are compatible with sklearn and follow
+its outlier detection interface.
```

### Comparing `kondo_ml-0.0.1/kondo_ml.egg-info/SOURCES.txt` & `kondo_ml-0.0.2/kondo_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.1/pyproject.toml` & `kondo_ml-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kondo_ml"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Lukas Rücker", email="ruecker.lukas@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 dependencies = ['numpy','pandas','scikit-learn','torch']
 requires-python = ">=3.7"
```

### Comparing `kondo_ml-0.0.1/setup.py` & `kondo_ml-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
      version=new_version,                                     # Version
      author="L.Rücker",                                     # Author name
      author_email="ruecker.lukas@gmail.com",                           # Author mail
      description="Python package for my instace selection algorithms.",    # Short package description
      long_description=long_description,                       # Long package description
      long_description_content_type="text/markdown",
      url="https://github.com/lurue101/instance-selection-for-regression",       # Url to your Git Repo
-     download_url = 'https://github.com/erdogant/relevantpackage/archive/'+new_version+'.tar.gz',
+     download_url = 'https://github.com/lurue101/instance-selection-for-regression/archive/'+new_version+'.tar.gz',
      packages=setuptools.find_packages(),                     # Searches throughout all dirs for files to include
      include_package_data=True,                               # Must be true to include files depicted in MANIFEST.in
      license_files=["LICENSE"],                               # License file
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: MIT License",
          "Operating System :: OS Independent",
```

