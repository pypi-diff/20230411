# Comparing `tmp/scikit-duplo-0.1.3.tar.gz` & `tmp/scikit-duplo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-duplo-0.1.3.tar", last modified: Mon Apr 10 22:38:24 2023, max compression
+gzip compressed data, was "scikit-duplo-0.1.4.tar", last modified: Mon Apr 10 22:59:15 2023, max compression
```

## Comparing `scikit-duplo-0.1.3.tar` & `scikit-duplo-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 22:38:24.214688 scikit-duplo-0.1.3/
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1082 2023-04-06 00:11:51.000000 scikit-duplo-0.1.3/LICENSE
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1767 2023-04-10 22:38:24.214075 scikit-duplo-0.1.3/PKG-INFO
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1227 2023-04-10 06:17:16.000000 scikit-duplo-0.1.3/README.md
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 22:38:24.201212 scikit-duplo-0.1.3/scikit_duplo.egg-info/
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1767 2023-04-10 22:38:24.000000 scikit-duplo-0.1.3/scikit_duplo.egg-info/PKG-INFO
--rw-r--r--   0 johnhawkins   (501) staff       (20)      449 2023-04-10 22:38:24.000000 scikit-duplo-0.1.3/scikit_duplo.egg-info/SOURCES.txt
--rw-r--r--   0 johnhawkins   (501) staff       (20)        1 2023-04-10 22:38:24.000000 scikit-duplo-0.1.3/scikit_duplo.egg-info/dependency_links.txt
--rw-r--r--   0 johnhawkins   (501) staff       (20)       26 2023-04-10 22:38:24.000000 scikit-duplo-0.1.3/scikit_duplo.egg-info/requires.txt
--rw-r--r--   0 johnhawkins   (501) staff       (20)        8 2023-04-10 22:38:24.000000 scikit-duplo-0.1.3/scikit_duplo.egg-info/top_level.txt
--rw-r--r--   0 johnhawkins   (501) staff       (20)       38 2023-04-10 22:38:24.214842 scikit-duplo-0.1.3/setup.cfg
--rwxr-xr-x   0 johnhawkins   (501) staff       (20)     1163 2023-04-10 21:57:03.000000 scikit-duplo-0.1.3/setup.py
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 22:38:24.201785 scikit-duplo-0.1.3/skduplo/
--rw-r--r--   0 johnhawkins   (501) staff       (20)       22 2023-04-10 22:38:04.000000 scikit-duplo-0.1.3/skduplo/__init__.py
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 22:38:24.209982 scikit-duplo-0.1.3/skduplo/meta/
--rw-r--r--   0 johnhawkins   (501) staff       (20)      170 2023-04-10 22:37:28.000000 scikit-duplo-0.1.3/skduplo/meta/__init__.py
--rw-r--r--   0 johnhawkins   (501) staff       (20)     5862 2023-04-06 22:04:15.000000 scikit-duplo-0.1.3/skduplo/meta/quantile_stack_regressor.py
--rw-r--r--   0 johnhawkins   (501) staff       (20)     4893 2023-04-10 22:37:14.000000 scikit-duplo-0.1.3/skduplo/meta/regressor_stack.py
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 22:38:24.211805 scikit-duplo-0.1.3/skduplo/preprocessing/
--rw-r--r--   0 johnhawkins   (501) staff       (20)      172 2023-04-06 21:55:06.000000 scikit-duplo-0.1.3/skduplo/preprocessing/__init__.py
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1155 2023-04-06 00:24:35.000000 scikit-duplo-0.1.3/skduplo/preprocessing/column_concatenator.py
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1217 2023-04-06 00:20:02.000000 scikit-duplo-0.1.3/skduplo/preprocessing/two_column_ratio_diff.py
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 22:59:15.234074 scikit-duplo-0.1.4/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1082 2023-04-06 00:11:51.000000 scikit-duplo-0.1.4/LICENSE
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1767 2023-04-10 22:59:15.233707 scikit-duplo-0.1.4/PKG-INFO
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1227 2023-04-10 06:17:16.000000 scikit-duplo-0.1.4/README.md
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 22:59:15.228653 scikit-duplo-0.1.4/scikit_duplo.egg-info/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1767 2023-04-10 22:59:15.000000 scikit-duplo-0.1.4/scikit_duplo.egg-info/PKG-INFO
+-rw-r--r--   0 johnhawkins   (501) staff       (20)      449 2023-04-10 22:59:15.000000 scikit-duplo-0.1.4/scikit_duplo.egg-info/SOURCES.txt
+-rw-r--r--   0 johnhawkins   (501) staff       (20)        1 2023-04-10 22:59:15.000000 scikit-duplo-0.1.4/scikit_duplo.egg-info/dependency_links.txt
+-rw-r--r--   0 johnhawkins   (501) staff       (20)       26 2023-04-10 22:59:15.000000 scikit-duplo-0.1.4/scikit_duplo.egg-info/requires.txt
+-rw-r--r--   0 johnhawkins   (501) staff       (20)        8 2023-04-10 22:59:15.000000 scikit-duplo-0.1.4/scikit_duplo.egg-info/top_level.txt
+-rw-r--r--   0 johnhawkins   (501) staff       (20)       38 2023-04-10 22:59:15.234223 scikit-duplo-0.1.4/setup.cfg
+-rwxr-xr-x   0 johnhawkins   (501) staff       (20)     1163 2023-04-10 21:57:03.000000 scikit-duplo-0.1.4/setup.py
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 22:59:15.228925 scikit-duplo-0.1.4/skduplo/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)       22 2023-04-10 22:59:01.000000 scikit-duplo-0.1.4/skduplo/__init__.py
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 22:59:15.230845 scikit-duplo-0.1.4/skduplo/meta/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)      170 2023-04-10 22:37:28.000000 scikit-duplo-0.1.4/skduplo/meta/__init__.py
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     5862 2023-04-06 22:04:15.000000 scikit-duplo-0.1.4/skduplo/meta/quantile_stack_regressor.py
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     4869 2023-04-10 22:56:04.000000 scikit-duplo-0.1.4/skduplo/meta/regressor_stack.py
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2023-04-10 22:59:15.232740 scikit-duplo-0.1.4/skduplo/preprocessing/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)      172 2023-04-06 21:55:06.000000 scikit-duplo-0.1.4/skduplo/preprocessing/__init__.py
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1155 2023-04-06 00:24:35.000000 scikit-duplo-0.1.4/skduplo/preprocessing/column_concatenator.py
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1217 2023-04-06 00:20:02.000000 scikit-duplo-0.1.4/skduplo/preprocessing/two_column_ratio_diff.py
```

### Comparing `scikit-duplo-0.1.3/LICENSE` & `scikit-duplo-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.3/PKG-INFO` & `scikit-duplo-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-duplo
-Version: 0.1.3
+Version: 0.1.4
 Summary: Sci-kit learn tools for machine learning pipelines
 Home-page: http://getting-data-science-done.com
 Author: John Hawkins
 Author-email: johnc@getting-data-science-done.com
 License: MIT
 Project-URL: Documentation, http://scikit-duplo.readthedocs.io
 Project-URL: Source, https://github.com/getting-data-science-done/scikit-duplo
```

### Comparing `scikit-duplo-0.1.3/README.md` & `scikit-duplo-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.3/scikit_duplo.egg-info/PKG-INFO` & `scikit-duplo-0.1.4/scikit_duplo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-duplo
-Version: 0.1.3
+Version: 0.1.4
 Summary: Sci-kit learn tools for machine learning pipelines
 Home-page: http://getting-data-science-done.com
 Author: John Hawkins
 Author-email: johnc@getting-data-science-done.com
 License: MIT
 Project-URL: Documentation, http://scikit-duplo.readthedocs.io
 Project-URL: Source, https://github.com/getting-data-science-done/scikit-duplo
```

### Comparing `scikit-duplo-0.1.3/setup.py` & `scikit-duplo-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.3/skduplo/meta/quantile_stack_regressor.py` & `scikit-duplo-0.1.4/skduplo/meta/quantile_stack_regressor.py`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.3/skduplo/meta/regressor_stack.py` & `scikit-duplo-0.1.4/skduplo/meta/regressor_stack.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,20 +23,20 @@
     Examples
     --------
     >>> import numpy as np
     >>> from sklearn.ensemble import ExtraTreesClassifier, ExtraTreesRegressor
     >>> np.random.seed(0)
     >>> X = np.random.randn(10000, 4)
     >>> y = ((X[:, 0]>0) & (X[:, 1]>0)) * np.abs(X[:, 2] * X[:, 3]**2)
-    >>> z = StackedMultiRegressor(
-    ... classifier=ExtraTreesClassifier(random_state=0),
-    ... regressor=ExtraTreesRegressor(random_state=0)
+    >>> z = RegressorStack(
+    ...   [KNeighborsRegressor(), BayesianRidge()],
+    ...   regressor=ExtraTreesRegressor(random_state=0)
     ... )
     >>> z.fit(X, y)
-    StackedMultiRegressor(classifier=ExtraTreesClassifier(random_state=0),
+    RegressorStack([KNeighborsRegressor(), BayesianRidge()],
                           regressor=ExtraTreesRegressor(random_state=0))
     >>> z.predict(X)[:5]
     array([4.91483294, 0.        , 0.        , 0.04941909, 0.        ])
     """
 
     def __init__(self, regressor_list, regressor) -> None:
         """Initialize."""
```

### Comparing `scikit-duplo-0.1.3/skduplo/preprocessing/column_concatenator.py` & `scikit-duplo-0.1.4/skduplo/preprocessing/column_concatenator.py`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.3/skduplo/preprocessing/two_column_ratio_diff.py` & `scikit-duplo-0.1.4/skduplo/preprocessing/two_column_ratio_diff.py`

 * *Files identical despite different names*

