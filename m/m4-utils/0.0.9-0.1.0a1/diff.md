# Comparing `tmp/m4-utils-0.0.9.tar.gz` & `tmp/m4-utils-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m4-utils-0.0.9.tar", last modified: Thu Dec 29 18:17:22 2022, max compression
+gzip compressed data, was "m4-utils-0.1.0a1.tar", last modified: Tue Apr 11 15:05:33 2023, max compression
```

## Comparing `m4-utils-0.0.9.tar` & `m4-utils-0.1.0a1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 luisfelipe  (1000) luisfelipe  (1000)        0 2022-12-29 18:17:22.247751 m4-utils-0.0.9/
--rwxrwxr-x   0 luisfelipe  (1000) luisfelipe  (1000)      178 2022-12-15 12:57:02.000000 m4-utils-0.0.9/MANIFEST.in
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)      241 2022-12-29 18:17:22.247751 m4-utils-0.0.9/PKG-INFO
-drwxrwxr-x   0 luisfelipe  (1000) luisfelipe  (1000)        0 2022-12-29 18:17:22.247751 m4-utils-0.0.9/m4_utils/
--rwxrwxr-x   0 luisfelipe  (1000) luisfelipe  (1000)      112 2022-12-15 16:17:41.000000 m4-utils-0.0.9/m4_utils/__init__.py
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)     1014 2022-12-15 22:46:59.000000 m4-utils-0.0.9/m4_utils/feature_calculators.py
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)     2762 2022-12-14 14:10:21.000000 m4-utils-0.0.9/m4_utils/metrics.py
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)     4504 2022-12-14 14:10:21.000000 m4-utils-0.0.9/m4_utils/plots.py
--rwxrwxr-x   0 luisfelipe  (1000) luisfelipe  (1000)     4206 2022-12-14 14:10:21.000000 m4-utils-0.0.9/m4_utils/s3_client.py
-drwxrwxr-x   0 luisfelipe  (1000) luisfelipe  (1000)        0 2022-12-29 18:17:22.247751 m4-utils-0.0.9/m4_utils/transformers/
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)      457 2022-12-19 16:32:28.000000 m4-utils-0.0.9/m4_utils/transformers/__init__.py
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)     2953 2022-12-19 16:14:44.000000 m4-utils-0.0.9/m4_utils/transformers/column_diff.py
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)     2967 2022-12-19 16:18:35.000000 m4-utils-0.0.9/m4_utils/transformers/column_equality.py
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)     3135 2022-12-19 16:17:58.000000 m4-utils-0.0.9/m4_utils/transformers/column_time_diff.py
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)     3809 2022-12-15 17:45:20.000000 m4-utils-0.0.9/m4_utils/transformers/feature_union.py
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)     4769 2022-12-19 16:20:08.000000 m4-utils-0.0.9/m4_utils/transformers/fill_na.py
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)     1484 2022-12-19 16:19:30.000000 m4-utils-0.0.9/m4_utils/transformers/identity.py
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)     5725 2022-12-15 19:22:24.000000 m4-utils-0.0.9/m4_utils/transformers/standard_scaler.py
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)     3402 2022-12-19 16:15:38.000000 m4-utils-0.0.9/m4_utils/transformers/time_normalization.py
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)     3025 2022-12-19 16:13:39.000000 m4-utils-0.0.9/m4_utils/transformers/time_period_features.py
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)     1175 2022-12-15 12:57:47.000000 m4-utils-0.0.9/m4_utils/utils.py
-drwxrwxr-x   0 luisfelipe  (1000) luisfelipe  (1000)        0 2022-12-29 18:17:22.247751 m4-utils-0.0.9/m4_utils.egg-info/
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)      241 2022-12-29 18:17:22.000000 m4-utils-0.0.9/m4_utils.egg-info/PKG-INFO
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)      718 2022-12-29 18:17:22.000000 m4-utils-0.0.9/m4_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)        1 2022-12-29 18:17:22.000000 m4-utils-0.0.9/m4_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)     3396 2022-12-29 18:17:22.000000 m4-utils-0.0.9/m4_utils.egg-info/requires.txt
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)        9 2022-12-29 18:17:22.000000 m4-utils-0.0.9/m4_utils.egg-info/top_level.txt
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)   164778 2022-12-29 18:16:50.000000 m4-utils-0.0.9/requirements.txt
--rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)       38 2022-12-29 18:17:22.247751 m4-utils-0.0.9/setup.cfg
--rwxrwxr-x   0 luisfelipe  (1000) luisfelipe  (1000)     1281 2022-12-29 13:52:27.000000 m4-utils-0.0.9/setup.py
+drwxrwxr-x   0 luisfelipe  (1000) luisfelipe  (1000)        0 2023-04-11 15:05:33.155440 m4-utils-0.1.0a1/
+-rwxrwxr-x   0 luisfelipe  (1000) luisfelipe  (1000)      178 2023-04-10 19:26:39.000000 m4-utils-0.1.0a1/MANIFEST.in
+-rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)      288 2023-04-11 15:05:33.155440 m4-utils-0.1.0a1/PKG-INFO
+drwxrwxr-x   0 luisfelipe  (1000) luisfelipe  (1000)        0 2023-04-11 15:05:33.151440 m4-utils-0.1.0a1/m4_utils/
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)      112 2023-04-10 20:27:04.000000 m4-utils-0.1.0a1/m4_utils/__init__.py
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     1170 2023-01-31 17:31:05.000000 m4-utils-0.1.0a1/m4_utils/feature_calculators.py
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     2762 2022-12-14 14:10:21.000000 m4-utils-0.1.0a1/m4_utils/metrics.py
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     4504 2022-12-14 14:10:21.000000 m4-utils-0.1.0a1/m4_utils/plots.py
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     4206 2022-12-14 14:10:21.000000 m4-utils-0.1.0a1/m4_utils/s3_client.py
+drwxrwxr-x   0 luisfelipe  (1000) luisfelipe  (1000)        0 2023-04-11 15:05:33.151440 m4-utils-0.1.0a1/m4_utils/transformers/
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)      493 2023-02-09 18:45:33.000000 m4-utils-0.1.0a1/m4_utils/transformers/__init__.py
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     2953 2022-12-19 16:14:44.000000 m4-utils-0.1.0a1/m4_utils/transformers/column_diff.py
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     2995 2023-01-31 19:39:59.000000 m4-utils-0.1.0a1/m4_utils/transformers/column_equality.py
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     3766 2023-01-31 20:33:18.000000 m4-utils-0.1.0a1/m4_utils/transformers/column_time_diff.py
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     3809 2022-12-15 17:45:20.000000 m4-utils-0.1.0a1/m4_utils/transformers/feature_union.py
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     4769 2022-12-19 16:20:08.000000 m4-utils-0.1.0a1/m4_utils/transformers/fill_na.py
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     2852 2023-02-02 16:55:26.000000 m4-utils-0.1.0a1/m4_utils/transformers/identity.py
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     5725 2023-02-02 16:04:49.000000 m4-utils-0.1.0a1/m4_utils/transformers/standard_scaler.py
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     3402 2022-12-19 16:15:38.000000 m4-utils-0.1.0a1/m4_utils/transformers/time_normalization.py
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     3025 2022-12-19 16:13:39.000000 m4-utils-0.1.0a1/m4_utils/transformers/time_period_features.py
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     2879 2023-02-09 21:08:35.000000 m4-utils-0.1.0a1/m4_utils/transformers/to_datetime.py
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     1175 2022-12-15 12:57:47.000000 m4-utils-0.1.0a1/m4_utils/utils.py
+drwxrwxr-x   0 luisfelipe  (1000) luisfelipe  (1000)        0 2023-04-11 15:05:33.151440 m4-utils-0.1.0a1/m4_utils.egg-info/
+-rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)      288 2023-04-11 15:05:33.000000 m4-utils-0.1.0a1/m4_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)      761 2023-04-11 15:05:33.000000 m4-utils-0.1.0a1/m4_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)        1 2023-04-11 15:05:33.000000 m4-utils-0.1.0a1/m4_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)      131 2023-04-11 15:05:33.000000 m4-utils-0.1.0a1/m4_utils.egg-info/requires.txt
+-rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)       14 2023-04-11 15:05:33.000000 m4-utils-0.1.0a1/m4_utils.egg-info/top_level.txt
+-rwxr-xr-x   0 luisfelipe  (1000) luisfelipe  (1000)     1347 2023-04-11 15:00:31.000000 m4-utils-0.1.0a1/pyproject.toml
+-rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)    32144 2023-04-10 20:15:14.000000 m4-utils-0.1.0a1/requirements.txt
+-rw-rw-r--   0 luisfelipe  (1000) luisfelipe  (1000)       38 2023-04-11 15:05:33.155440 m4-utils-0.1.0a1/setup.cfg
```

### Comparing `m4-utils-0.0.9/m4_utils/feature_calculators.py` & `m4-utils-0.1.0a1/m4_utils/feature_calculators.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     elapsed_time = (end_dt - start_dt).dt.total_seconds()
     # to hours
     elapsed_time /= 60**2
     #to days
     elapsed_time /= 24
     return elapsed_time
 
+def get_elapsed_time_in_seconds(end_dt: pd.Series, start_dt: pd.Series):
+    elapsed_time = (end_dt - start_dt).dt.total_seconds()
+    return elapsed_time
+
 def is_month_start(dt:pd.Series):
     return dt.dt.day <= 10
 
 def is_month_end(dt:pd.Series):
     return dt.dt.day >= 20
 
 def is_mid_month(dt:pd.Series):
```

### Comparing `m4-utils-0.0.9/m4_utils/metrics.py` & `m4-utils-0.1.0a1/m4_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `m4-utils-0.0.9/m4_utils/plots.py` & `m4-utils-0.1.0a1/m4_utils/plots.py`

 * *Files identical despite different names*

### Comparing `m4-utils-0.0.9/m4_utils/s3_client.py` & `m4-utils-0.1.0a1/m4_utils/s3_client.py`

 * *Files identical despite different names*

### Comparing `m4-utils-0.0.9/m4_utils/transformers/column_diff.py` & `m4-utils-0.1.0a1/m4_utils/transformers/column_diff.py`

 * *Files identical despite different names*

### Comparing `m4-utils-0.0.9/m4_utils/transformers/column_equality.py` & `m4-utils-0.1.0a1/m4_utils/transformers/column_equality.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 
     Parameters
     ----------
     columns : list of tuples
         List of (column1, column2, out_name) tuples specifying the
         transformer objects to be applied to subsets of the data.
 
-        column1 :  str
-            The name of the column1.
-        column2 :  str
-            The name of the column2.
-        
-        out_name : str
-            Normalized Column output name;
+            column1 :  str
+                The name of the column1.
+            column2 :  str
+                The name of the column2.
+            
+            out_name : str
+                Normalized Column output name;
     """
 
     def __init__(
         self,
         columns: list,
         dtype='bool'
     ):
```

### Comparing `m4-utils-0.0.9/m4_utils/transformers/column_time_diff.py` & `m4-utils-0.1.0a1/m4_utils/transformers/column_time_diff.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,46 +3,55 @@
 """Column Time Diff in Days custom transformer.
 """
 
 import os
 import pandas as pd
 import numpy as np
 from sklearn.base import BaseEstimator, TransformerMixin
-from ..feature_calculators import get_elapsed_time_in_days
+from ..feature_calculators import get_elapsed_time_in_days, get_elapsed_time_in_seconds
 
 
 class ColumnTimeDiff(TransformerMixin, BaseEstimator):
     """Column Time Diff in Days Transformer;
 
     TODO: Add type validation.
     Parameters
     ----------
     columns : list of tuples
         List of (column1, column2, out_name) tuples specifying the
         transformer objects to be applied to subsets of the data.
 
-        column1 :  str
-            The name of the column1.
-        column2 :  str
-            The name of the column2.
-        
-        out_name : str
-            Normalized Column output name;
+            column1 :  str
+                The name of the column1.
+            column2 :  str
+                The name of the column2.
+            
+            out_name : str
+                Normalized Column output name;
+    
+    in_ : str,  'days' | 'seconds'
+
+    dtype: np.DType or str
+        The output data type;
+    
+
     """
 
     def __init__(
         self,
         columns: list,
+        in_: str = 'days',
         dtype='float32'
     ):
         self._columns = columns
         self._feature_names_out = [
             c[2] for c in self._columns
         ]
         self._dtype = dtype
+        self._in = in_.lower()
     
     def fit(self, X: pd.DataFrame, y=None):
         """Fit transformer by checking X.
 
         Parameters
         ----------
         X : array-like, shape (n_samples, n_features)
@@ -69,18 +78,26 @@
         Returns
         -------
         X_out : array-like, shape (n_samples, n_features)
             Transformed input.
         """
         res = dict()
         for (col1, col2, c_name) in self._columns:
-            res[c_name] = get_elapsed_time_in_days(
-                end_dt=X[col2],
-                start_dt=X[col1],
-            ).astype(self._dtype)
+            if self._in == 'days':
+                res[c_name] = get_elapsed_time_in_days(
+                    end_dt=X[col2],
+                    start_dt=X[col1],
+                ).astype(self._dtype)
+            elif self._in == 'seconds':
+                res[c_name] = get_elapsed_time_in_seconds(
+                    end_dt=X[col2],
+                    start_dt=X[col1],
+                ).astype(self._dtype)
+            else:
+                raise ValueError('Time scale not recognizer. The class parameter \'in_\' must be one of : [\'days\', \'seconds\']')
         
         return pd.DataFrame(data=res)
 
     def inverse_transform(self, X):
         """[NOT IMPLEMENTED] Transform X using the inverse function.
 
         Parameters
```

### Comparing `m4-utils-0.0.9/m4_utils/transformers/feature_union.py` & `m4-utils-0.1.0a1/m4_utils/transformers/feature_union.py`

 * *Files identical despite different names*

### Comparing `m4-utils-0.0.9/m4_utils/transformers/fill_na.py` & `m4-utils-0.1.0a1/m4_utils/transformers/fill_na.py`

 * *Files identical despite different names*

### Comparing `m4-utils-0.0.9/m4_utils/transformers/standard_scaler.py` & `m4-utils-0.1.0a1/m4_utils/transformers/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `m4-utils-0.0.9/m4_utils/transformers/time_normalization.py` & `m4-utils-0.1.0a1/m4_utils/transformers/time_normalization.py`

 * *Files identical despite different names*

### Comparing `m4-utils-0.0.9/m4_utils/transformers/time_period_features.py` & `m4-utils-0.1.0a1/m4_utils/transformers/time_period_features.py`

 * *Files identical despite different names*

### Comparing `m4-utils-0.0.9/m4_utils/utils.py` & `m4-utils-0.1.0a1/m4_utils/utils.py`

 * *Files identical despite different names*

### Comparing `m4-utils-0.0.9/m4_utils.egg-info/SOURCES.txt` & `m4-utils-0.1.0a1/m4_utils.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MANIFEST.in
+pyproject.toml
 requirements.txt
-setup.py
 m4_utils/__init__.py
 m4_utils/feature_calculators.py
 m4_utils/metrics.py
 m4_utils/plots.py
 m4_utils/s3_client.py
 m4_utils/utils.py
 m4_utils.egg-info/PKG-INFO
@@ -17,8 +17,9 @@
 m4_utils/transformers/column_equality.py
 m4_utils/transformers/column_time_diff.py
 m4_utils/transformers/feature_union.py
 m4_utils/transformers/fill_na.py
 m4_utils/transformers/identity.py
 m4_utils/transformers/standard_scaler.py
 m4_utils/transformers/time_normalization.py
-m4_utils/transformers/time_period_features.py
+m4_utils/transformers/time_period_features.py
+m4_utils/transformers/to_datetime.py
```

