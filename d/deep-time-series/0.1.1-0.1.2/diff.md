# Comparing `tmp/deep_time_series-0.1.1.tar.gz` & `tmp/deep_time_series-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_time_series-0.1.1.tar", max compression
+gzip compressed data, was "deep_time_series-0.1.2.tar", max compression
```

## Comparing `deep_time_series-0.1.1.tar` & `deep_time_series-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0      359 2023-03-06 15:40:31.585298 deep_time_series-0.1.1/deep_time_series/__init__.py
--rw-r--r--   0        0        0     6929 2023-03-20 14:19:08.282696 deep_time_series-0.1.1/deep_time_series/chunk.py
--rw-r--r--   0        0        0    15261 2023-03-22 02:57:16.078114 deep_time_series-0.1.1/deep_time_series/core.py
--rw-r--r--   0        0        0     1572 2023-03-06 15:40:31.589296 deep_time_series-0.1.1/deep_time_series/dataset.py
--rw-r--r--   0        0        0       18 2023-03-06 15:40:31.590296 deep_time_series-0.1.1/deep_time_series/function.py
--rw-r--r--   0        0        0     1712 2023-03-06 15:40:31.591298 deep_time_series-0.1.1/deep_time_series/layer.py
--rw-r--r--   0        0        0      189 2023-03-06 15:40:31.593306 deep_time_series-0.1.1/deep_time_series/model/__init__.py
--rw-r--r--   0        0        0     5328 2023-03-06 15:40:31.594297 deep_time_series-0.1.1/deep_time_series/model/dilated_cnn.py
--rw-r--r--   0        0        0     4698 2023-03-06 15:40:31.595300 deep_time_series-0.1.1/deep_time_series/model/mlp.py
--rw-r--r--   0        0        0     4266 2023-03-06 15:40:31.596853 deep_time_series-0.1.1/deep_time_series/model/rnn.py
--rw-r--r--   0        0        0     5561 2023-03-06 15:40:31.597882 deep_time_series-0.1.1/deep_time_series/model/single_shot_transformer.py
--rw-r--r--   0        0        0      655 2023-03-06 15:40:31.598859 deep_time_series-0.1.1/deep_time_series/plotting.py
--rw-r--r--   0        0        0     3809 2023-03-06 15:40:31.599859 deep_time_series-0.1.1/deep_time_series/transform.py
--rw-r--r--   0        0        0     1045 2022-07-27 11:44:42.699971 deep_time_series-0.1.1/deep_time_series/util.py
--rw-r--r--   0        0        0     1038 2023-03-22 03:01:26.349373 deep_time_series-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1699 2023-03-20 15:32:34.113787 deep_time_series-0.1.1/README.md
--rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 deep_time_series-0.1.1/setup.py
--rw-r--r--   0        0        0     2552 1970-01-01 00:00:00.000000 deep_time_series-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      359 2023-03-06 15:40:31.585298 deep_time_series-0.1.2/deep_time_series/__init__.py
+-rw-r--r--   0        0        0     6929 2023-03-20 14:19:08.282696 deep_time_series-0.1.2/deep_time_series/chunk.py
+-rw-r--r--   0        0        0    15261 2023-03-22 02:57:16.078114 deep_time_series-0.1.2/deep_time_series/core.py
+-rw-r--r--   0        0        0     1572 2023-03-06 15:40:31.589296 deep_time_series-0.1.2/deep_time_series/dataset.py
+-rw-r--r--   0        0        0       18 2023-03-06 15:40:31.590296 deep_time_series-0.1.2/deep_time_series/function.py
+-rw-r--r--   0        0        0     1712 2023-03-06 15:40:31.591298 deep_time_series-0.1.2/deep_time_series/layer.py
+-rw-r--r--   0        0        0      189 2023-03-06 15:40:31.593306 deep_time_series-0.1.2/deep_time_series/model/__init__.py
+-rw-r--r--   0        0        0     5328 2023-03-06 15:40:31.594297 deep_time_series-0.1.2/deep_time_series/model/dilated_cnn.py
+-rw-r--r--   0        0        0     4698 2023-03-06 15:40:31.595300 deep_time_series-0.1.2/deep_time_series/model/mlp.py
+-rw-r--r--   0        0        0     4266 2023-03-06 15:40:31.596853 deep_time_series-0.1.2/deep_time_series/model/rnn.py
+-rw-r--r--   0        0        0     5561 2023-03-06 15:40:31.597882 deep_time_series-0.1.2/deep_time_series/model/single_shot_transformer.py
+-rw-r--r--   0        0        0      655 2023-03-06 15:40:31.598859 deep_time_series-0.1.2/deep_time_series/plotting.py
+-rw-r--r--   0        0        0     3809 2023-03-06 15:40:31.599859 deep_time_series-0.1.2/deep_time_series/transform.py
+-rw-r--r--   0        0        0     1045 2022-07-27 11:44:42.699971 deep_time_series-0.1.2/deep_time_series/util.py
+-rw-r--r--   0        0        0     1038 2023-04-11 12:36:58.225954 deep_time_series-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1699 2023-03-20 15:32:34.113787 deep_time_series-0.1.2/README.md
+-rw-r--r--   0        0        0     2552 1970-01-01 00:00:00.000000 deep_time_series-0.1.2/PKG-INFO
```

### Comparing `deep_time_series-0.1.1/deep_time_series/chunk.py` & `deep_time_series-0.1.2/deep_time_series/chunk.py`

 * *Files identical despite different names*

### Comparing `deep_time_series-0.1.1/deep_time_series/core.py` & `deep_time_series-0.1.2/deep_time_series/core.py`

 * *Files identical despite different names*

### Comparing `deep_time_series-0.1.1/deep_time_series/dataset.py` & `deep_time_series-0.1.2/deep_time_series/dataset.py`

 * *Files identical despite different names*

### Comparing `deep_time_series-0.1.1/deep_time_series/layer.py` & `deep_time_series-0.1.2/deep_time_series/layer.py`

 * *Files identical despite different names*

### Comparing `deep_time_series-0.1.1/deep_time_series/model/dilated_cnn.py` & `deep_time_series-0.1.2/deep_time_series/model/dilated_cnn.py`

 * *Files identical despite different names*

### Comparing `deep_time_series-0.1.1/deep_time_series/model/mlp.py` & `deep_time_series-0.1.2/deep_time_series/model/mlp.py`

 * *Files identical despite different names*

### Comparing `deep_time_series-0.1.1/deep_time_series/model/rnn.py` & `deep_time_series-0.1.2/deep_time_series/model/rnn.py`

 * *Files identical despite different names*

### Comparing `deep_time_series-0.1.1/deep_time_series/model/single_shot_transformer.py` & `deep_time_series-0.1.2/deep_time_series/model/single_shot_transformer.py`

 * *Files identical despite different names*

### Comparing `deep_time_series-0.1.1/deep_time_series/plotting.py` & `deep_time_series-0.1.2/deep_time_series/plotting.py`

 * *Files identical despite different names*

### Comparing `deep_time_series-0.1.1/deep_time_series/transform.py` & `deep_time_series-0.1.2/deep_time_series/transform.py`

 * *Files identical despite different names*

### Comparing `deep_time_series-0.1.1/deep_time_series/util.py` & `deep_time_series-0.1.2/deep_time_series/util.py`

 * *Files identical despite different names*

### Comparing `deep_time_series-0.1.1/pyproject.toml` & `deep_time_series-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deep-time-series"
-version = "0.1.1"
+version = "0.1.2"
 description = """Deep learning library for time series \
 forecasting based on PyTorch."""
 authors = ["Sangwon <lsw91.main@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "deep_time_series"}]
 
@@ -12,15 +12,15 @@
 python = "^3.10"
 torch = {version = "^2.0.0", source = "torch"}
 torchvision = {version = "^0.15.1", source = "torch"}
 torchaudio = {version = "^2.0.1", source = "torch"}
 lightning = "^2.0.0"
 numpy = "^1.24.2"
 pandas = "^1.5.3"
-matplotlib = "^3.7.1"
+matplotlib = "^3.5.1"
 xarray = "^2023.2.0"
 rich = "^13.3.2"
 scikit-learn = "^1.2.2"
 
 
 [[tool.poetry.source]]
 name = "torch"
```

### Comparing `deep_time_series-0.1.1/README.md` & `deep_time_series-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `deep_time_series-0.1.1/PKG-INFO` & `deep_time_series-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: deep-time-series
-Version: 0.1.1
+Version: 0.1.2
 Summary: Deep learning library for time series forecasting based on PyTorch.
 License: MIT
 Author: Sangwon
 Author-email: lsw91.main@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lightning (>=2.0.0,<3.0.0)
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: torchaudio (>=2.0.1,<3.0.0)
 Requires-Dist: torchvision (>=0.15.1,<0.16.0)
```

