# Comparing `tmp/terra_ai_datasets-1.1.0.tar.gz` & `tmp/terra_ai_datasets-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terra_ai_datasets-1.1.0.tar", last modified: Mon Apr 10 00:25:13 2023, max compression
+gzip compressed data, was "terra_ai_datasets-1.1.1.tar", last modified: Tue Apr 11 10:42:44 2023, max compression
```

## Comparing `terra_ai_datasets-1.1.0.tar` & `terra_ai_datasets-1.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/terra_ai_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/create.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    24383 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/preprocessings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/creation_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/creation/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/terra_ai_datasets/load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/terra_ai_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-10 00:25:13.000000 terra_ai_datasets-1.1.0/terra_ai_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-10 00:25:13.000000 terra_ai_datasets-1.1.0/terra_ai_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 00:25:13.000000 terra_ai_datasets-1.1.0/terra_ai_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-10 00:25:13.000000 terra_ai_datasets-1.1.0/terra_ai_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 00:25:13.000000 terra_ai_datasets-1.1.0/terra_ai_datasets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:13.945727 terra_ai_datasets-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-10 00:24:51.000000 terra_ai_datasets-1.1.0/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:42:44.039624 terra_ai_datasets-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-11 10:42:44.039624 terra_ai_datasets-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:42:44.039624 terra_ai_datasets-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:42:44.031623 terra_ai_datasets-1.1.1/terra_ai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/create.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:42:44.035623 terra_ai_datasets-1.1.1/terra_ai_datasets/creation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/creation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/creation/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24383 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/creation/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/creation/preprocessings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/creation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:42:44.039624 terra_ai_datasets-1.1.1/terra_ai_datasets/creation/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/creation/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/creation/validators/creation_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/creation/validators/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/creation/validators/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/creation/validators/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/creation/validators/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/creation/validators/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/creation/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/terra_ai_datasets/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:42:44.035623 terra_ai_datasets-1.1.1/terra_ai_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-11 10:42:44.000000 terra_ai_datasets-1.1.1/terra_ai_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-11 10:42:44.000000 terra_ai_datasets-1.1.1/terra_ai_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:42:44.000000 terra_ai_datasets-1.1.1/terra_ai_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-11 10:42:44.000000 terra_ai_datasets-1.1.1/terra_ai_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-11 10:42:44.000000 terra_ai_datasets-1.1.1/terra_ai_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:42:44.039624 terra_ai_datasets-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-11 10:42:34.000000 terra_ai_datasets-1.1.1/tests/test_timeseries.py
```

### Comparing `terra_ai_datasets-1.1.0/setup.py` & `terra_ai_datasets-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 from setuptools import setup, find_packages
 
 DESCRIPTION = "Framework to create a dataset to train a neural network."
 LONG_DESCRIPTION = "terra_ai_datasets is a framework to create " \
                    "a dataset to train a neural network model based on a Keras."
```

### Comparing `terra_ai_datasets-1.1.0/terra_ai_datasets/create.py` & `terra_ai_datasets-1.1.1/terra_ai_datasets/create.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/arrays.py` & `terra_ai_datasets-1.1.1/terra_ai_datasets/creation/arrays.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/dataset.py` & `terra_ai_datasets-1.1.1/terra_ai_datasets/creation/dataset.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/preprocessings.py` & `terra_ai_datasets-1.1.1/terra_ai_datasets/creation/preprocessings.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 def create_embedding(parameters: TextValidator):
     return create_tokenizer(parameters)
 
 
 def create_word_to_vec(text_list: list, parameters: TextValidator):
 
     text_list = [elem.split(' ') for elem in text_list]
-    word2vec = Word2Vec(text_list, size=parameters.word2vec_size)
+    word2vec = Word2Vec(text_list, vector_size=parameters.word2vec_size)
     return word2vec
 
 
 # def inverse_data(self, options: dict):
 #     out_dict = {}
 #     for put_id, value in options.items():
 #         out_dict[put_id] = {}
```

### Comparing `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/utils.py` & `terra_ai_datasets-1.1.1/terra_ai_datasets/creation/utils.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/creation_data.py` & `terra_ai_datasets-1.1.1/terra_ai_datasets/creation/validators/creation_data.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/dataset.py` & `terra_ai_datasets-1.1.1/terra_ai_datasets/creation/validators/dataset.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/inputs.py` & `terra_ai_datasets-1.1.1/terra_ai_datasets/creation/validators/inputs.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/outputs.py` & `terra_ai_datasets-1.1.1/terra_ai_datasets/creation/validators/outputs.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/validators/tasks.py` & `terra_ai_datasets-1.1.1/terra_ai_datasets/creation/validators/tasks.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.0/terra_ai_datasets/creation/visualize.py` & `terra_ai_datasets-1.1.1/terra_ai_datasets/creation/visualize.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.0/terra_ai_datasets/load.py` & `terra_ai_datasets-1.1.1/terra_ai_datasets/load.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.0/terra_ai_datasets.egg-info/SOURCES.txt` & `terra_ai_datasets-1.1.1/terra_ai_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.0/tests/test_classification.py` & `terra_ai_datasets-1.1.1/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.0/tests/test_regression.py` & `terra_ai_datasets-1.1.1/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.0/tests/test_segmentation.py` & `terra_ai_datasets-1.1.1/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `terra_ai_datasets-1.1.0/tests/test_timeseries.py` & `terra_ai_datasets-1.1.1/tests/test_timeseries.py`

 * *Files identical despite different names*

