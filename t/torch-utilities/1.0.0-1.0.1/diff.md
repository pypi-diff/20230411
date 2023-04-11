# Comparing `tmp/torch_utilities-1.0.0.tar.gz` & `tmp/torch_utilities-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_utilities-1.0.0.tar", last modified: Tue Apr 11 20:33:33 2023, max compression
+gzip compressed data, was "torch_utilities-1.0.1.tar", last modified: Tue Apr 11 20:43:41 2023, max compression
```

## Comparing `torch_utilities-1.0.0.tar` & `torch_utilities-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-11 20:33:33.569064 torch_utilities-1.0.0/
--rw-rw-r--   0 deema     (1000) deema     (1000)     1074 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/LICENSE
--rw-rw-r--   0 deema     (1000) deema     (1000)     5183 2023-04-11 20:33:33.569064 torch_utilities-1.0.0/PKG-INFO
--rw-rw-r--   0 deema     (1000) deema     (1000)     4846 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/README.md
--rw-rw-r--   0 deema     (1000) deema     (1000)       80 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/pyproject.toml
--rw-rw-r--   0 deema     (1000) deema     (1000)      829 2023-04-11 20:33:33.569064 torch_utilities-1.0.0/setup.cfg
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-11 20:33:33.569064 torch_utilities-1.0.0/tests/
--rw-rw-r--   0 deema     (1000) deema     (1000)      196 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/tests/__init__.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     3514 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/tests/generate_test_data.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    10294 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/tests/test_audio.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     2179 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/tests/test_augmentation.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     5321 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/tests/test_common.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     5870 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/tests/test_data_loading.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     4081 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/tests/test_io.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     1228 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/tests/test_metrics.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     9425 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/tests/test_model_trainer.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    33857 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/tests/test_modules.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     3675 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/tests/test_pytorch.py
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-11 20:33:33.569064 torch_utilities-1.0.0/torch_utilities/
--rw-rw-r--   0 deema     (1000) deema     (1000)      373 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/torch_utilities/__init__.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    19083 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/torch_utilities/audio.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     6376 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/torch_utilities/augmentation.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     6300 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/torch_utilities/common.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    13302 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/torch_utilities/data_loading.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     4664 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/torch_utilities/io.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     3777 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/torch_utilities/metrics.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    28889 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/torch_utilities/model_trainer.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    42064 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/torch_utilities/modules.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    11611 2023-04-11 20:08:44.000000 torch_utilities-1.0.0/torch_utilities/pytorch.py
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-11 20:33:33.569064 torch_utilities-1.0.0/torch_utilities.egg-info/
--rw-rw-r--   0 deema     (1000) deema     (1000)     5183 2023-04-11 20:33:33.000000 torch_utilities-1.0.0/torch_utilities.egg-info/PKG-INFO
--rw-rw-r--   0 deema     (1000) deema     (1000)     1057 2023-04-11 20:33:33.000000 torch_utilities-1.0.0/torch_utilities.egg-info/SOURCES.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)        1 2023-04-11 20:33:33.000000 torch_utilities-1.0.0/torch_utilities.egg-info/dependency_links.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)      147 2023-04-11 20:33:33.000000 torch_utilities-1.0.0/torch_utilities.egg-info/entry_points.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)      146 2023-04-11 20:33:33.000000 torch_utilities-1.0.0/torch_utilities.egg-info/requires.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)       22 2023-04-11 20:33:33.000000 torch_utilities-1.0.0/torch_utilities.egg-info/top_level.txt
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-11 20:43:41.056931 torch_utilities-1.0.1/
+-rw-rw-r--   0 deema     (1000) deema     (1000)     1074 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/LICENSE
+-rw-rw-r--   0 deema     (1000) deema     (1000)     5061 2023-04-11 20:43:41.056931 torch_utilities-1.0.1/PKG-INFO
+-rw-rw-r--   0 deema     (1000) deema     (1000)     4724 2023-04-11 20:36:41.000000 torch_utilities-1.0.1/README.md
+-rw-rw-r--   0 deema     (1000) deema     (1000)       80 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/pyproject.toml
+-rw-rw-r--   0 deema     (1000) deema     (1000)      837 2023-04-11 20:43:41.056931 torch_utilities-1.0.1/setup.cfg
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-11 20:43:41.056931 torch_utilities-1.0.1/tests/
+-rw-rw-r--   0 deema     (1000) deema     (1000)      196 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/tests/__init__.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     3514 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/tests/generate_test_data.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    10294 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/tests/test_audio.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     2179 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/tests/test_augmentation.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     5321 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/tests/test_common.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     5870 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/tests/test_data_loading.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     4081 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/tests/test_io.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     1228 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/tests/test_metrics.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     9425 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/tests/test_model_trainer.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    33857 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/tests/test_modules.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     3675 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/tests/test_pytorch.py
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-11 20:43:41.056931 torch_utilities-1.0.1/torch_utilities/
+-rw-rw-r--   0 deema     (1000) deema     (1000)      373 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/torch_utilities/__init__.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    19083 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/torch_utilities/audio.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     6376 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/torch_utilities/augmentation.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     6300 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/torch_utilities/common.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    13302 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/torch_utilities/data_loading.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     4664 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/torch_utilities/io.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     3777 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/torch_utilities/metrics.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    28889 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/torch_utilities/model_trainer.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    42064 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/torch_utilities/modules.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    11611 2023-04-11 20:08:44.000000 torch_utilities-1.0.1/torch_utilities/pytorch.py
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-11 20:43:41.056931 torch_utilities-1.0.1/torch_utilities.egg-info/
+-rw-rw-r--   0 deema     (1000) deema     (1000)     5061 2023-04-11 20:43:41.000000 torch_utilities-1.0.1/torch_utilities.egg-info/PKG-INFO
+-rw-rw-r--   0 deema     (1000) deema     (1000)     1057 2023-04-11 20:43:41.000000 torch_utilities-1.0.1/torch_utilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)        1 2023-04-11 20:43:41.000000 torch_utilities-1.0.1/torch_utilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)      147 2023-04-11 20:43:41.000000 torch_utilities-1.0.1/torch_utilities.egg-info/entry_points.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)      154 2023-04-11 20:43:41.000000 torch_utilities-1.0.1/torch_utilities.egg-info/requires.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)       22 2023-04-11 20:43:41.000000 torch_utilities-1.0.1/torch_utilities.egg-info/top_level.txt
```

### Comparing `torch_utilities-1.0.0/LICENSE` & `torch_utilities-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/PKG-INFO` & `torch_utilities-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_utilities
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simplifying audio and deep learning with PyTorch.
 Home-page: https://github.com/FedericoDiMarzo/torch_utilities
 Author: Federico Di Marzo
 Author-email: federicodimarzo@protonmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,21 +12,17 @@
 # Torch Utilities
 **Torch Utilities**  is a Python module that provides various tools related to audio and deep learning using the PyTorch framework. The module simplifies the process of building and training deep learning models for audio data, making it easier to experiment and develop custom models and pipelines. With its *user-friendly API*, the module also enables researchers and engineers to quickly prototype new ideas and evaluate their performance. Whether you're an experienced deep learning practitioner or just starting out, **Torch Utilities** has the tools you need to get the job done efficiently.
 
 ## Disclaimer
 **Torch Utilities** is developed as a personal set of tools and is provided as-it-is, without any warranties or guarantees. The API and utilities may change in the future as the module continues to evolve. While effort is made to maintain compatibility with previous versions, users are advised to carefully consider the stability of the API before using **Torch Utilities** in production environments.
 
 ## Installation
-To install **Torch Utilities** clone it and install it with pip
+You can install **Torch Utilities** using pip
 ```bash
-# clone the repo
-git clone git@github.com:FedericoDiMarzo/torch_utilities.git
-
-# install it with pip
-pip install -e torch_utilities
+pip install torch_utilities
 ```
 
 A pypi package will be provided in the future when the API will be more stable.
 
 ## Running The Tests
 To verify the correctness of the code and run the tests, simply run the following line in a bash console:
 ```bash
```

### Comparing `torch_utilities-1.0.0/README.md` & `torch_utilities-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # Torch Utilities
 **Torch Utilities**  is a Python module that provides various tools related to audio and deep learning using the PyTorch framework. The module simplifies the process of building and training deep learning models for audio data, making it easier to experiment and develop custom models and pipelines. With its *user-friendly API*, the module also enables researchers and engineers to quickly prototype new ideas and evaluate their performance. Whether you're an experienced deep learning practitioner or just starting out, **Torch Utilities** has the tools you need to get the job done efficiently.
 
 ## Disclaimer
 **Torch Utilities** is developed as a personal set of tools and is provided as-it-is, without any warranties or guarantees. The API and utilities may change in the future as the module continues to evolve. While effort is made to maintain compatibility with previous versions, users are advised to carefully consider the stability of the API before using **Torch Utilities** in production environments.
 
 ## Installation
-To install **Torch Utilities** clone it and install it with pip
+You can install **Torch Utilities** using pip
 ```bash
-# clone the repo
-git clone git@github.com:FedericoDiMarzo/torch_utilities.git
-
-# install it with pip
-pip install -e torch_utilities
+pip install torch_utilities
 ```
 
 A pypi package will be provided in the future when the API will be more stable.
 
 ## Running The Tests
 To verify the correctness of the code and run the tests, simply run the following line in a bash console:
 ```bash
```

### Comparing `torch_utilities-1.0.0/setup.cfg` & `torch_utilities-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torch_utilities
-version = 1.0.0
+version = 1.0.1
 author = Federico Di Marzo
 author_email = federicodimarzo@protonmail.com
 description = Simplifying audio and deep learning with PyTorch.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/FedericoDiMarzo/torch_utilities
 
@@ -14,15 +14,15 @@
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	h5py
 	tqdm
 	pdoc
 	pyyaml
-	torch
+	torch==1.13.1
 	torchaudio
 	tensorboard
 	multiprocess
 	onnxruntime
 	matplotlib
 	pathimport
 	soundfile
```

### Comparing `torch_utilities-1.0.0/tests/generate_test_data.py` & `torch_utilities-1.0.1/tests/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/tests/test_audio.py` & `torch_utilities-1.0.1/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/tests/test_augmentation.py` & `torch_utilities-1.0.1/tests/test_augmentation.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/tests/test_common.py` & `torch_utilities-1.0.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/tests/test_data_loading.py` & `torch_utilities-1.0.1/tests/test_data_loading.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/tests/test_io.py` & `torch_utilities-1.0.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/tests/test_metrics.py` & `torch_utilities-1.0.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/tests/test_model_trainer.py` & `torch_utilities-1.0.1/tests/test_model_trainer.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/tests/test_modules.py` & `torch_utilities-1.0.1/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/tests/test_pytorch.py` & `torch_utilities-1.0.1/tests/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/torch_utilities/audio.py` & `torch_utilities-1.0.1/torch_utilities/audio.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/torch_utilities/augmentation.py` & `torch_utilities-1.0.1/torch_utilities/augmentation.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/torch_utilities/common.py` & `torch_utilities-1.0.1/torch_utilities/common.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/torch_utilities/data_loading.py` & `torch_utilities-1.0.1/torch_utilities/data_loading.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/torch_utilities/io.py` & `torch_utilities-1.0.1/torch_utilities/io.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/torch_utilities/metrics.py` & `torch_utilities-1.0.1/torch_utilities/metrics.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/torch_utilities/model_trainer.py` & `torch_utilities-1.0.1/torch_utilities/model_trainer.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/torch_utilities/modules.py` & `torch_utilities-1.0.1/torch_utilities/modules.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/torch_utilities/pytorch.py` & `torch_utilities-1.0.1/torch_utilities/pytorch.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.0/torch_utilities.egg-info/PKG-INFO` & `torch_utilities-1.0.1/torch_utilities.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-utilities
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simplifying audio and deep learning with PyTorch.
 Home-page: https://github.com/FedericoDiMarzo/torch_utilities
 Author: Federico Di Marzo
 Author-email: federicodimarzo@protonmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,21 +12,17 @@
 # Torch Utilities
 **Torch Utilities**  is a Python module that provides various tools related to audio and deep learning using the PyTorch framework. The module simplifies the process of building and training deep learning models for audio data, making it easier to experiment and develop custom models and pipelines. With its *user-friendly API*, the module also enables researchers and engineers to quickly prototype new ideas and evaluate their performance. Whether you're an experienced deep learning practitioner or just starting out, **Torch Utilities** has the tools you need to get the job done efficiently.
 
 ## Disclaimer
 **Torch Utilities** is developed as a personal set of tools and is provided as-it-is, without any warranties or guarantees. The API and utilities may change in the future as the module continues to evolve. While effort is made to maintain compatibility with previous versions, users are advised to carefully consider the stability of the API before using **Torch Utilities** in production environments.
 
 ## Installation
-To install **Torch Utilities** clone it and install it with pip
+You can install **Torch Utilities** using pip
 ```bash
-# clone the repo
-git clone git@github.com:FedericoDiMarzo/torch_utilities.git
-
-# install it with pip
-pip install -e torch_utilities
+pip install torch_utilities
 ```
 
 A pypi package will be provided in the future when the API will be more stable.
 
 ## Running The Tests
 To verify the correctness of the code and run the tests, simply run the following line in a bash console:
 ```bash
```

### Comparing `torch_utilities-1.0.0/torch_utilities.egg-info/SOURCES.txt` & `torch_utilities-1.0.1/torch_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

