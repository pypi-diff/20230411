# Comparing `tmp/arize-7.0.0rc4.tar.gz` & `tmp/arize-7.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arize-7.0.0rc4.tar", last modified: Fri Apr  7 22:52:10 2023, max compression
+gzip compressed data, was "arize-7.0.0rc5.tar", last modified: Tue Apr 11 17:47:12 2023, max compression
```

## Comparing `arize-7.0.0rc4.tar` & `arize-7.0.0rc5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.374084 arize-7.0.0rc4/
--rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-03-30 21:17:25.000000 arize-7.0.0rc4/LICENSE.md
--rw-r--r--   0 kiko       (501) staff       (20)       65 2023-03-30 21:17:25.000000 arize-7.0.0rc4/MANIFEST.in
--rw-r--r--   0 kiko       (501) staff       (20)    12608 2023-04-07 22:52:10.374690 arize-7.0.0rc4/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-03-30 21:17:25.000000 arize-7.0.0rc4/README.md
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.267353 arize-7.0.0rc4/arize/
--rw-r--r--   0 kiko       (501) staff       (20)       25 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    25743 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/api.py
--rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/bounded_executor.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.305116 arize-7.0.0rc4/arize/examples/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/examples/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/examples/bulk_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/examples/bulk_client_shap.py
--rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/examples/client_shap_values.py
--rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/examples/log_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/examples/log_pandas_dataframe.py
--rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/examples/preproduction_client.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.308253 arize-7.0.0rc4/arize/pandas/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.326610 arize-7.0.0rc4/arize/pandas/embeddings/
--rw-r--r--   0 kiko       (501) staff       (20)      124 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/embeddings/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     2279 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/embeddings/auto_generator.py
--rw-r--r--   0 kiko       (501) staff       (20)     6583 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/embeddings/base_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      213 2023-04-01 00:42:11.000000 arize-7.0.0rc4/arize/pandas/embeddings/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     1962 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/embeddings/cv_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      571 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/embeddings/models.py
--rw-r--r--   0 kiko       (501) staff       (20)     3576 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/pandas/embeddings/nlp_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)     5809 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/embeddings/tabular_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      412 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/pandas/embeddings/usecases.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.328141 arize-7.0.0rc4/arize/pandas/generative/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-01 00:42:11.000000 arize-7.0.0rc4/arize/pandas/generative/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.334591 arize-7.0.0rc4/arize/pandas/generative/llm_evaluation/
--rw-r--r--   0 kiko       (501) staff       (20)      160 2023-04-01 00:42:11.000000 arize-7.0.0rc4/arize/pandas/generative/llm_evaluation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      183 2023-04-01 00:42:11.000000 arize-7.0.0rc4/arize/pandas/generative/llm_evaluation/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)    11932 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/pandas/generative/llm_evaluation/hf_metrics.py
--rw-r--r--   0 kiko       (501) staff       (20)    21965 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/pandas/logger.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.354679 arize-7.0.0rc4/arize/pandas/surrogate_explainer/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/surrogate_explainer/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     4910 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/surrogate_explainer/mimic.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.359424 arize-7.0.0rc4/arize/pandas/validation/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/pandas/validation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    22704 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/pandas/validation/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)    59911 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/pandas/validation/validator.py
--rw-r--r--   0 kiko       (501) staff       (20)   167320 2023-04-07 22:16:19.000000 arize-7.0.0rc4/arize/public_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.369208 arize-7.0.0rc4/arize/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/utils/logging.py
--rw-r--r--   0 kiko       (501) staff       (20)     4177 2023-03-30 21:17:25.000000 arize-7.0.0rc4/arize/utils/model_mapping.json
--rw-r--r--   0 kiko       (501) staff       (20)    20830 2023-04-07 22:45:24.000000 arize-7.0.0rc4/arize/utils/types.py
--rw-r--r--   0 kiko       (501) staff       (20)     7196 2023-04-06 23:45:03.000000 arize-7.0.0rc4/arize/utils/utils.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.276765 arize-7.0.0rc4/arize.egg-info/
--rw-r--r--   0 kiko       (501) staff       (20)    12608 2023-04-07 22:52:10.000000 arize-7.0.0rc4/arize.egg-info/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)     1463 2023-04-07 22:52:10.000000 arize-7.0.0rc4/arize.egg-info/SOURCES.txt
--rw-r--r--   0 kiko       (501) staff       (20)        1 2023-04-07 22:52:10.000000 arize-7.0.0rc4/arize.egg-info/dependency_links.txt
--rw-r--r--   0 kiko       (501) staff       (20)      434 2023-04-07 22:52:10.000000 arize-7.0.0rc4/arize.egg-info/requires.txt
--rw-r--r--   0 kiko       (501) staff       (20)        6 2023-04-07 22:52:10.000000 arize-7.0.0rc4/arize.egg-info/top_level.txt
--rw-r--r--   0 kiko       (501) staff       (20)      167 2023-03-30 21:17:25.000000 arize-7.0.0rc4/pyproject.toml
--rw-r--r--   0 kiko       (501) staff       (20)     1561 2023-04-07 22:52:10.377092 arize-7.0.0rc4/setup.cfg
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-07 22:52:10.373013 arize-7.0.0rc4/tests/
--rw-r--r--   0 kiko       (501) staff       (20)    43569 2023-03-30 21:17:25.000000 arize-7.0.0rc4/tests/test_api.py
--rw-r--r--   0 kiko       (501) staff       (20)      952 2023-03-30 21:17:25.000000 arize-7.0.0rc4/tests/test_utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.976723 arize-7.0.0rc5/
+-rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-03-30 21:17:25.000000 arize-7.0.0rc5/LICENSE.md
+-rw-r--r--   0 kiko       (501) staff       (20)       65 2023-03-30 21:17:25.000000 arize-7.0.0rc5/MANIFEST.in
+-rw-r--r--   0 kiko       (501) staff       (20)    12608 2023-04-11 17:47:12.977262 arize-7.0.0rc5/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-03-30 21:17:25.000000 arize-7.0.0rc5/README.md
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.885802 arize-7.0.0rc5/arize/
+-rw-r--r--   0 kiko       (501) staff       (20)       25 2023-04-11 17:42:22.000000 arize-7.0.0rc5/arize/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    25743 2023-04-10 23:06:12.000000 arize-7.0.0rc5/arize/api.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/bounded_executor.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.898800 arize-7.0.0rc5/arize/examples/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/examples/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/examples/bulk_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/examples/bulk_client_shap.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/examples/client_shap_values.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/examples/log_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-04-10 03:28:13.000000 arize-7.0.0rc5/arize/examples/log_pandas_dataframe.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/examples/preproduction_client.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.918558 arize-7.0.0rc5/arize/pandas/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/pandas/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.931183 arize-7.0.0rc5/arize/pandas/embeddings/
+-rw-r--r--   0 kiko       (501) staff       (20)      124 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/pandas/embeddings/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-04-11 17:42:22.000000 arize-7.0.0rc5/arize/pandas/embeddings/auto_generator.py
+-rw-r--r--   0 kiko       (501) staff       (20)     6583 2023-04-10 21:49:18.000000 arize-7.0.0rc5/arize/pandas/embeddings/base_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      213 2023-04-10 22:55:57.000000 arize-7.0.0rc5/arize/pandas/embeddings/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1962 2023-04-10 03:28:13.000000 arize-7.0.0rc5/arize/pandas/embeddings/cv_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      571 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/pandas/embeddings/models.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3576 2023-04-10 22:55:57.000000 arize-7.0.0rc5/arize/pandas/embeddings/nlp_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5809 2023-04-10 03:28:13.000000 arize-7.0.0rc5/arize/pandas/embeddings/tabular_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      412 2023-04-10 22:55:57.000000 arize-7.0.0rc5/arize/pandas/embeddings/usecases.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.932173 arize-7.0.0rc5/arize/pandas/generative/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-10 22:55:57.000000 arize-7.0.0rc5/arize/pandas/generative/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.935576 arize-7.0.0rc5/arize/pandas/generative/llm_evaluation/
+-rw-r--r--   0 kiko       (501) staff       (20)      160 2023-04-10 22:55:57.000000 arize-7.0.0rc5/arize/pandas/generative/llm_evaluation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      183 2023-04-10 22:55:57.000000 arize-7.0.0rc5/arize/pandas/generative/llm_evaluation/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)    12188 2023-04-11 17:42:22.000000 arize-7.0.0rc5/arize/pandas/generative/llm_evaluation/hf_metrics.py
+-rw-r--r--   0 kiko       (501) staff       (20)    21965 2023-04-11 17:42:13.000000 arize-7.0.0rc5/arize/pandas/logger.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.938444 arize-7.0.0rc5/arize/pandas/surrogate_explainer/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/pandas/surrogate_explainer/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4910 2023-04-10 03:28:13.000000 arize-7.0.0rc5/arize/pandas/surrogate_explainer/mimic.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.941342 arize-7.0.0rc5/arize/pandas/validation/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/pandas/validation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    22704 2023-04-10 23:06:12.000000 arize-7.0.0rc5/arize/pandas/validation/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)    59911 2023-04-11 01:26:42.000000 arize-7.0.0rc5/arize/pandas/validation/validator.py
+-rw-r--r--   0 kiko       (501) staff       (20)   167320 2023-04-11 17:42:13.000000 arize-7.0.0rc5/arize/public_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.949832 arize-7.0.0rc5/arize/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/utils/logging.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4177 2023-04-10 23:06:12.000000 arize-7.0.0rc5/arize/utils/model_mapping.json
+-rw-r--r--   0 kiko       (501) staff       (20)    22046 2023-04-11 17:42:22.000000 arize-7.0.0rc5/arize/utils/types.py
+-rw-r--r--   0 kiko       (501) staff       (20)     7229 2023-04-11 17:42:22.000000 arize-7.0.0rc5/arize/utils/utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.890054 arize-7.0.0rc5/arize.egg-info/
+-rw-r--r--   0 kiko       (501) staff       (20)    12608 2023-04-11 17:47:12.000000 arize-7.0.0rc5/arize.egg-info/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)     1463 2023-04-11 17:47:12.000000 arize-7.0.0rc5/arize.egg-info/SOURCES.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        1 2023-04-11 17:47:12.000000 arize-7.0.0rc5/arize.egg-info/dependency_links.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      434 2023-04-11 17:47:12.000000 arize-7.0.0rc5/arize.egg-info/requires.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        6 2023-04-11 17:47:12.000000 arize-7.0.0rc5/arize.egg-info/top_level.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      167 2023-03-30 21:17:25.000000 arize-7.0.0rc5/pyproject.toml
+-rw-r--r--   0 kiko       (501) staff       (20)     1561 2023-04-11 17:47:12.979870 arize-7.0.0rc5/setup.cfg
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.975172 arize-7.0.0rc5/tests/
+-rw-r--r--   0 kiko       (501) staff       (20)    43569 2023-04-10 03:28:13.000000 arize-7.0.0rc5/tests/test_api.py
+-rw-r--r--   0 kiko       (501) staff       (20)      952 2023-03-30 21:17:25.000000 arize-7.0.0rc5/tests/test_utils.py
```

### Comparing `arize-7.0.0rc4/LICENSE.md` & `arize-7.0.0rc5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/PKG-INFO` & `arize-7.0.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.0rc4
+Version: 7.0.0rc5
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.0rc4/README.md` & `arize-7.0.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/api.py` & `arize-7.0.0rc5/arize/api.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/bounded_executor.py` & `arize-7.0.0rc5/arize/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/examples/bulk_client.py` & `arize-7.0.0rc5/arize/examples/bulk_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/examples/bulk_client_shap.py` & `arize-7.0.0rc5/arize/examples/bulk_client_shap.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/examples/client_shap_values.py` & `arize-7.0.0rc5/arize/examples/client_shap_values.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/examples/log_client.py` & `arize-7.0.0rc5/arize/examples/log_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/examples/log_pandas_dataframe.py` & `arize-7.0.0rc5/arize/examples/log_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/examples/preproduction_client.py` & `arize-7.0.0rc5/arize/examples/preproduction_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/pandas/embeddings/auto_generator.py` & `arize-7.0.0rc5/arize/pandas/embeddings/auto_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import pandas as pd
 
 from . import constants
 from .base_generators import BaseEmbeddingGenerator
 from .cv_generators import EmbeddingGeneratorForCVImageClassification
 from .models import CV_PRETRAINED_MODELS, NLP_PRETRAINED_MODELS
-from .nlp_generators import EmbeddingGeneratorForNLPSequenceClassification
+from .nlp_generators import (
+    EmbeddingGeneratorForNLPSequenceClassification,
+    EmbeddingGeneratorForNLPSummarization,
+)
 from .tabular_generators import EmbeddingGeneratorForTabularFeatures
 from .usecases import UseCases
 
 
 class EmbeddingGenerator:
     def __init__(self, **kwargs: str):
         raise EnvironmentError(
@@ -16,14 +19,16 @@
             f"`{self.__class__.__name__}.from_use_case(use_case, **kwargs)` method."
         )
 
     @staticmethod
     def from_use_case(use_case: str, **kwargs: str) -> BaseEmbeddingGenerator:
         if use_case == UseCases.NLP.SEQUENCE_CLASSIFICATION:
             return EmbeddingGeneratorForNLPSequenceClassification(**kwargs)
+        elif use_case == UseCases.NLP.SUMMARIZATION:
+            return EmbeddingGeneratorForNLPSummarization(**kwargs)
         elif use_case == UseCases.CV.IMAGE_CLASSIFICATION:
             return EmbeddingGeneratorForCVImageClassification(**kwargs)
         elif use_case == UseCases.STRUCTURED.TABULAR_EMBEDDINGS:
             return EmbeddingGeneratorForTabularFeatures(**kwargs)
         else:
             raise ValueError(f"Invalid use case {use_case}")
```

### Comparing `arize-7.0.0rc4/arize/pandas/embeddings/base_generators.py` & `arize-7.0.0rc5/arize/pandas/embeddings/base_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/pandas/embeddings/cv_generators.py` & `arize-7.0.0rc5/arize/pandas/embeddings/cv_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/pandas/embeddings/models.py` & `arize-7.0.0rc5/arize/pandas/embeddings/models.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/pandas/embeddings/nlp_generators.py` & `arize-7.0.0rc5/arize/pandas/embeddings/nlp_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/pandas/embeddings/tabular_generators.py` & `arize-7.0.0rc5/arize/pandas/embeddings/tabular_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/pandas/generative/llm_evaluation/hf_metrics.py` & `arize-7.0.0rc5/arize/pandas/generative/llm_evaluation/hf_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,36 +12,38 @@
     raise ImportError(IMPORT_ERROR_MESSAGE)
 
 
 # BLEU
 def bleu(
     response_col: pd.Series, references_col: pd.Series, max_order: int = 4, smooth: bool = False
 ) -> List[float]:
-    """BLEU (Bilingual Evaluation Understudy) is an algorithm used to evaluate the quality of machine
+    """
+    BLEU (Bilingual Evaluation Understudy) is an algorithm used to evaluate the quality of machine
     translated text from one natural language to another. The quality of machine translation is measured
     based on its similarity to human translation, with the goal being to achieve high correspondence between
     the two.
 
     BLEU calculates scores for individual translated segments, typically sentences, by comparing
     them to a set of high-quality reference translations. These scores are then averaged over the entire
     corpus to obtain an estimate of the overall quality of the translation. Notably, BLEU does not consider
     factors such as intelligibility or grammatical correctness when computing the scores.
 
-
     NOTE: This metric is a wrapper around the Hugging Face's implementation of BLEU:
         https://github.com/huggingface/evaluate/blob/main/metrics/bleu/bleu.py
 
-    Args:
+    Parameters:
+    -----------
         response_col (pd.Series): Pandas Series containing the translations (as strings) to score.
         references_col (pd.Series): Pandas Series containing a reference, or list of several references,
             for each translation.
         max_order (int, optional):  Maximum n-gram order to use when computing BLEU score. Defaults to 4.
         smooth (bool, optional): Whether or not to apply Lin et al. 2004 smoothing. Defaults to False.
 
     Returns:
+    --------
         List[float]: BLEU scores
     """
     logger.info("Loading metric: bleu")
     bleu = evaluate.load("bleu")
     logger.info("Computing bleu scores")
     return [
         bleu.compute(
@@ -62,22 +64,24 @@
     references_col: pd.Series,
     smooth_method: str = "exp",
     smooth_value: Optional[float] = None,
     lowercase: bool = False,
     force: bool = False,
     use_effective_order: bool = False,
 ) -> List[float]:
-    """SacreBLEU provides hassle-free computation of shareable, comparable, and reproducible BLEU scores.
-    Inspired by Rico Sennrich’s multi-bleu-detok.perl, it produces the official Workshop on Machine
+    """
+    SacreBLEU provides hassle-free computation of shareable, comparable, and reproducible BLEU scores.
+    Inspired by Rico Sennrich's multi-bleu-detok.perl, it produces the official Workshop on Machine
     Translation (WMT) scores but works with plain text.
 
     NOTE: This metric is a wrapper around the Hugging Face's implementation of SacreBLEU:
         https://github.com/huggingface/evaluate/blob/main/metrics/sacrebleu/sacrebleu.py
 
-    Args:
+    Parameters:
+    -----------
         response_col (pd.Series): Pandas Series containing translations (as strings) to score.
         references_col (pd.Series): Pandas Series containing a reference, or list of several references,
             per prediction. Note that there must be the same number of references for each prediction
             (i.e. all sub-lists must be of the same length).
         smooth_method (str, optional): The smoothing method to use, defaults to 'exp'. Possible values are:
             - 'none': no smoothing
             - 'floor': increment zero counts
@@ -90,14 +94,15 @@
             False.
         force (bool, optional): If True, insists that your tokenized input is actually de-tokenized. Defaults
             to False.
         use_effective_order (bool, optional): If True, stops including n-gram orders for which precision is 0.
             This should be True, if sentence-level BLEU will be computed. Defaults to False.
 
     Returns:
+    --------
         List[float]: SacreBLEU scores
     """
     logger.info("Loading metric: sacrebleu")
     s_bleu = evaluate.load("sacrebleu")
     logger.info("Computing sacrebleu scores")
     return [
         s_bleu.compute(
@@ -118,37 +123,40 @@
     ]
 
 
 # GOOGLE_BLEU
 def google_bleu(
     response_col: pd.Series, references_col: pd.Series, min_len: int = 1, max_len: int = 4
 ) -> List[float]:
-    """The BLEU score was designed to be used as a corpus measure, and it has some limitations when applied to
+    """
+    The BLEU score was designed to be used as a corpus measure, and it has some limitations when applied to
     single sentences. To overcome this issue in RL experiments, there exists a variation called the GLEU
     score. For GLEU, we analyze all the possible sub-sequences of 1, 2, 3, or 4 tokens in both the generated
     output and target sequences. We then calculate the recall and precision, where recall is the number of
     matching n-grams divided by the total number of n-grams in the target sequence, and precision is the
     number of matching n-grams divided by the total number of n-grams in the generated output sequence.
     The GLEU score is the minimum of recall and precision.
 
     The GLEU score ranges between 0 (no matches) and 1 (all matches), and it is symmetrical when we switch
     the output and target sequences. The GLEU score is highly correlated with the BLEU metric at the corpus
     level but does not have the limitations of the BLEU score for our per sentence reward objective.
 
     NOTE: This metric is a wrapper around the Hugging Face's implementation of Google BLEU:
         https://github.com/huggingface/evaluate/blob/main/metrics/google_bleu/google_bleu.py
 
-    Args:
+    Parameters:
+    -----------
         response_col (pd.Series): Pandas Series containing translations (as strings) to score.
         references_col (pd.Series): Pandas Series containing a reference, or list of several references,
             for each translation.
         min_len (int, optional): The minimum order of n-gram this function should extract. Defaults to 1.
         max_len (int, optional): The maximum order of n-gram this function should extract. Defaults to 4.
 
     Returns:
+    --------
         List[float]: google-BLEU scores
     """
     logger.info("Loading metric: google_bleu")
     g_bleu = evaluate.load("google_bleu")
     logger.info("Computing google_bleu scores")
     return [
         g_bleu.compute(predictions=[preds], references=[refs])["google_bleu"]  # type:ignore
@@ -159,90 +167,97 @@
 # ROUGE
 def rouge(
     response_col: pd.Series,
     references_col: pd.Series,
     rouge_types: List[str] = ["rougeL"],
     use_stemmer: bool = False,
 ) -> Dict[str, List[float]]:
-    """ROUGE, which stands for Recall-Oriented Understudy for Gisting Evaluation, is a software package and a
+    """
+    ROUGE, which stands for Recall-Oriented Understudy for Gisting Evaluation, is a software package and a
     set of metrics commonly used to evaluate machine translation and automatic summarization software in
     natural language processing. These metrics involve comparing a machine-produced summary or translation
     with a reference or set of references that have been human-produced. It's worth noting that ROUGE treats
     uppercase and lowercase letters as equivalent, making the evaluation case-insensitive. By providing a
     standardized way to assess the quality of machine-generated summaries and translations, ROUGE is a useful
     tool in the field of natural language processing.
 
     NOTE: This metric is a wrapper around the Hugging Face's implementation of ROUGE:
         https://github.com/huggingface/evaluate/blob/main/metrics/rouge/rouge.py
 
-    Args:
+    Parameters:
+    -----------
         response_col (pd.Series): Pandas Series containing predictions (as strings) to score.
         references_col (pd.Series): Pandas Series containing a reference, or list of several references,
             per prediction.
         rouge_types (List[str], optional): A list of rouge types to calculate. Defaults to ['rougeL']. Valid
             rouge types:
-            - "rouge1": unigram (1-gram) based scoring
-            - "rouge2": bigram (2-gram) based scoring
-            - "rougeL": Longest common subsequence based scoring.
-            - "rougeLSum": splits text using "\n"
+                - "rouge1": unigram (1-gram) based scoring
+                - "rouge2": bigram (2-gram) based scoring
+                - "rougeL": Longest common subsequence based scoring.
+                - "rougeLSum": splits text using '\n'
         use_stemmer (bool, optional): If True, uses Porter stemmer to strip word suffixes. Defaults to False.
 
     Returns:
+    --------
         Dict[str, List[float]]: The output is a dictionary with one entry for each rouge type in the input
             list rouge_types.
     """
     data: Dict[str, List[float]] = {k: [0] * len(response_col) for k in rouge_types}
     logger.info("Loading metric: rouge")
     rouge = evaluate.load("rouge")
     logger.info("Computing rouge scores")
     for idx, (preds, refs) in tqdm(
         enumerate(zip(response_col, references_col)),
         total=len(response_col),
     ):
-        r: Dict[str, float] = rouge.compute(
+        r: Dict[str, List[float]] = rouge.compute(
             predictions=[preds],
             references=[refs],
             rouge_types=rouge_types,
             use_stemmer=use_stemmer,
+            use_aggregator=False,
         )  # type:ignore
         for r_type in rouge_types:
-            data[r_type][idx] = r[r_type]
+            data[r_type][idx] = r[r_type][0]
     return data
 
 
 # METEOR
 def meteor(
     response_col: pd.Series,
     references_col: pd.Series,
     alpha: float = 0.9,
     beta: float = 3,
     gamma: float = 0.5,
 ) -> List[float]:
-    """METEOR is an automatic metric used to evaluate machine translation, which is based on a generalized
+    """
+    METEOR is an automatic metric used to evaluate machine translation, which is based on a generalized
     concept of unigram matching between the machine-produced translation and the reference human-produced
     translations. METEOR has the capability to match unigrams based on their surface forms, stemmed forms,
     and meanings. Moreover, advanced matching strategies can be easily integrated into METEOR. After finding
     all generalized unigram matches between the two strings, METEOR calculates a score for this matching using
     a combination of unigram-precision, unigram-recall, and a measure of fragmentation, which is specifically
     designed to assess the order of the matched words in the machine translation compared to the reference.
 
     NOTE: This metric is a wrapper around the Hugging Face's implementation of METEOR:
         https://github.com/huggingface/evaluate/blob/main/metrics/meteor/meteor.py
 
-    Args:
+    Parameters:
+    -----------
         response_col (pd.Series): Pandas Series containing predictions (as strings) to score.
         references_col (pd.Series): Pandas Series containing a reference, or list of several references,
             per prediction.
         alpha (float, optional): Parameter for controlling relative weights of precision and recall.
             Default is 0.9.
         beta (float, optional): Parameter for controlling shape of penalty as a function of fragmentation.
             Default is 3.
         gamma (float, optional): The relative weight assigned to fragmentation penalty. Default is 0.5.
 
     Returns:
+    --------
         List[float]: METEOR scores
     """
     logger.info("Loading metric: meteor")
     meteor = evaluate.load("meteor")
     logger.info("Computing meteor scores")
     return [
         meteor.compute(
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `arize-7.0.0rc4/arize/pandas/logger.py` & `arize-7.0.0rc5/arize/pandas/logger.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/pandas/surrogate_explainer/mimic.py` & `arize-7.0.0rc5/arize/pandas/surrogate_explainer/mimic.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/pandas/validation/errors.py` & `arize-7.0.0rc5/arize/pandas/validation/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/pandas/validation/validator.py` & `arize-7.0.0rc5/arize/pandas/validation/validator.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/public_pb2.py` & `arize-7.0.0rc5/arize/public_pb2.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/utils/logging.py` & `arize-7.0.0rc5/arize/utils/logging.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/utils/model_mapping.json` & `arize-7.0.0rc5/arize/utils/model_mapping.json`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/arize/utils/types.py` & `arize-7.0.0rc5/arize/utils/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from dataclasses import asdict, dataclass
-from dataclasses import replace as dataclass_replace
+from dataclasses import asdict, dataclass, replace
 from enum import Enum, unique
 from typing import Dict, List, NamedTuple, Optional, Sequence, Set, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 
 
@@ -88,21 +87,24 @@
 
 class Embedding(NamedTuple):
     vector: List[float]
     data: Optional[Union[str, List[str]]] = None
     link_to_data: Optional[str] = None
 
     def validate(self, emb_name: Union[str, int, float]) -> None:
-        """Validates that the embedding object passed is of the correct format. That is,
-        validations must be passed for vector, data & link_to_data.
+        """
+        Validates that the embedding object passed is of the correct format. That is, validations must
+        be passed for vector, data & link_to_data.
 
-        Args:
+        Parameters:
+        -----------
             emb_name (str, int, float): Name of the embedding feature the vector belongs to
 
         Raises:
+        -------
             TypeError: If the embedding fields are of the wrong type
         """
 
         if self.vector is not None:
             self._validate_embedding_vector(emb_name)
 
         # Validate embedding raw data, if present
@@ -115,23 +117,26 @@
 
         return None
 
     def _validate_embedding_vector(
         self,
         emb_name: Union[str, int, float],
     ) -> None:
-        """Validates that the embedding vector passed is of the correct format. That is:
-        1. Type must be list or convertible to list (like numpy arrays, pandas Series)
-        2. List must not be empty
-        3. Elements in list must be floats
+        """
+        Validates that the embedding vector passed is of the correct format. That is:
+            1. Type must be list or convertible to list (like numpy arrays, pandas Series)
+            2. List must not be empty
+            3. Elements in list must be floats
 
-        Args:
+        Parameters:
+        -----------
             emb_name (str, int, float): Name of the embedding feature the vector belongs to
 
         Raises:
+        -------
             TypeError: If the embedding does not satisfy requirements above
         """
 
         if not Embedding._is_valid_iterable(self.vector):
             raise TypeError(
                 f'Embedding feature "{emb_name}" has vector type {type(self.vector)}. Must be '
                 f"list, "
@@ -148,21 +153,24 @@
         if len(self.vector) == 1:
             raise ValueError("Embedding vector must not have a size of 1")
 
     def _validate_embedding_data(
         self,
         emb_name: Union[str, int, float],
     ) -> None:
-        """Validates that the embedding raw data field is of the correct format. That is:
-        1. Must be string or list of strings (NLP case)
+        """
+        Validates that the embedding raw data field is of the correct format. That is:
+            1. Must be string or list of strings (NLP case)
 
-        Args:
+        Parameters:
+        -----------
             emb_name (str, int, float): Name of the embedding feature the vector belongs to
 
         Raises:
+        -------
             TypeError: If the embedding does not satisfy requirements above
         """
         # Validate that data is a string or iterable of strings
         is_string = isinstance(self.data, str)
         is_allowed_iterable = not is_string and Embedding._is_valid_iterable(self.data)
         if not (is_string or is_allowed_iterable):
             raise TypeError(
@@ -172,40 +180,46 @@
 
         if is_allowed_iterable:
             # Fail if not all elements in iterable are strings
             if not all(isinstance(val, str) for val in self.data):
                 raise TypeError("Embedding data field must contain strings")
 
     def _validate_embedding_link_to_data(self, emb_name: Union[str, int, float]) -> None:
-        """Validates that the embedding link to data field is of the correct format. That is:
-        1. Must be string
+        """
+        Validates that the embedding link to data field is of the correct format. That is:
+            1. Must be string
 
-        Args:
+        Parameters:
+        -----------
             emb_name (str, int, float): Name of the embedding feature the vector belongs to
 
         Raises:
+        -------
             TypeError: If the embedding does not satisfy requirements above
         """
         if not isinstance(self.link_to_data, str):
             raise TypeError(
                 f'Embedding feature "{emb_name}" link_to_data field must be str and got '
                 f"{type(self.link_to_data)}"
             )
 
     @staticmethod
     def _is_valid_iterable(data: Union[str, List[str], List[float], np.ndarray, pd.Series]) -> bool:
-        """Validates that the input data field is of the correct iterable type. That is:
-        1. List or
-        2. numpy array or
-        3. pandas Series
+        """
+        Validates that the input data field is of the correct iterable type. That is:
+            1. List or
+            2. numpy array or
+            3. pandas Series
 
-        Args:
+        Parameters:
+        -----------
             data: input iterable
 
         Returns:
+        --------
             True if the data type is one of the accepted iterable types, false otherwise
         """
         return any(isinstance(data, t) for t in (list, np.ndarray, pd.Series))
 
 
 class ObjectDetectionColumnNames(NamedTuple):
     bounding_boxes_coordinates_column_name: str
@@ -396,56 +410,74 @@
     object_detection_actual_column_names: Optional[ObjectDetectionColumnNames] = None
     prompt_column_names: Optional[EmbeddingColumnNames] = None
     response_column_names: Optional[EmbeddingColumnNames] = None
     """
     Used to organize and map column names containing model data within your Pandas dataframe to
     Arize.
 
-    :param prediction_id_column_name (str, optional): Column name for the predictions unique
-    identifier. This value is used to match a prediction to delayed actuals in Arize. If predictions
-    are not provided, it will default to an empty string "" and Arize will create a random
-    prediction id on the server side.
-    Contents must be a string and indicate a unique prediction event. Limited to 128 characters.
-    :param feature_column_names (List[str], optional): List of column names for features. The
-    content of this column can be int, float, string.
-    :param tag_column_names (List[str], optional): List of column names for tags. The content of
-    this column can be int, float, string.
-    :param timestamp_column_name (str, optional): Column name for timestamps. The
-    content of this column must be int Unix Timestamps in seconds.
-    :param prediction_label_column_name (str, optional): Column name for categorical prediction
-    values. The content of this column must be convertible to string.
-    :param prediction_score_column_name (str, optional): Column name for numeric prediction values.
-    The content of this column must be int/float.
-    :param actual_label_column_name (str, optional): Column name for categorical ground truth
-    values. The content of this column must be convertible to string.
-    :param actual_score_column_name (str, optional): Column name for numeric ground truth values.
-    The content of this column must be int/float.
-    :param shap_values_column_names (Dict[str, str], optional): Dictionary mapping
-    human readable and debuggable model features keys and SHAP feature importance values.
-    Keys must be str, while values must be float.
-    :param embedding_feature_column_names (Dict[str, EmbeddingColumnNames], optional): Dictionary
-    mapping embedding display names to EmbeddingColumnNames objects.
-    :param prediction_group_id_column_name (str, optional): Column name for ranking groups or lists
-    in ranking models. The content of this column must be string and is limited to 128 characters.
-    :param rank_column_name (str, optional): Column name for rank of each element on the its group
-    or list. The content of this column must be integer between 1-100.
-    :param relevance_score_column_name (str, optional): Column name for ranking model type numeric
-    ground truth values. The content of this column must be int/float.
-    :param relevance_labels_column_name (str, optional): Column name for ranking model type
-    categorical ground truth values. The content of this column must be a string.
-    :param object_detection_prediction_column_name (ObjectDetectionColumnNames, optional):
-    ObjectDetectionColumnNames object containing information defining the predicted bounding boxes'
-    coordinates, categories, and scores.
-    :param object_detection_prediction_column_name (ObjectDetectionColumnNames, optional):
-    ObjectDetectionColumnNames object containing information defining the actual bounding boxes'
-    coordinates, categories, and scores.
+    Parameters:
+    -----------
+        prediction_id_column_name (str, optional): Column name for the predictions unique identifier.
+            This value is used to match a prediction to delayed actuals in Arize. If predictions are
+            not provided, it will default to an empty string "" and Arize will create a random
+            prediction id on the server side. Contents must be a string and indicate a unique
+            prediction event. Limited to 128 characters.
+        feature_column_names (List[str], optional): List of column names for features. The content
+            of this column can be int, float, string.
+        tag_column_names (List[str], optional): List of column names for tags. The content of this
+            column can be int, float, string.
+        timestamp_column_name (str, optional): Column name for timestamps. The content of this
+            column must be int Unix Timestamps in seconds.
+        prediction_label_column_name (str, optional): Column name for categorical prediction values.
+            The content of this column must be convertible to string.
+        prediction_score_column_name (str, optional): Column name for numeric prediction values. The
+            content of this column must be int/float.
+        actual_label_column_name (str, optional): Column name for categorical ground truth values.
+            The content of this column must be convertible to string.
+        actual_score_column_name (str, optional): Column name for numeric ground truth values. The
+            content of this column must be int/float.
+        shap_values_column_names (Dict[str, str], optional): Dictionary mapping human readable and
+            debuggable model features keys and SHAP feature importance values. Keys must be str,
+            while values must be float.
+        embedding_feature_column_names (Dict[str, EmbeddingColumnNames], optional): Dictionary
+            mapping embedding display names to EmbeddingColumnNames objects.
+        prediction_group_id_column_name (str, optional): Column name for ranking groups or lists in
+            ranking models. The content of this column must be string and is limited to 128 characters.
+        rank_column_name (str, optional): Column name for rank of each element on the its group or
+            list. The content of this column must be integer between 1-100.
+        relevance_score_column_name (str, optional): Column name for ranking model type numeric
+            ground truth values. The content of this column must be int/float.
+        relevance_labels_column_name (str, optional): Column name for ranking model type categorical
+            ground truth values. The content of this column must be a string.
+        object_detection_prediction_column_name (ObjectDetectionColumnNames, optional):
+            ObjectDetectionColumnNames object containing information defining the predicted bounding
+            boxes' coordinates, categories, and scores.
+        object_detection_prediction_column_name (ObjectDetectionColumnNames, optional):
+            ObjectDetectionColumnNames object containing information defining the actual bounding
+            boxes' coordinates, categories, and scores.
+        prompt_column_names (EmbeddingCoulumnNames, optional): EmbeddingCoulumnNames object containing
+            the embedding vector data (required) and raw text (optional) for the input text your
+            model acts on.
+        response_column_names (EmbeddingCoulumnNames, optional): EmbeddingCoulumnNames object
+            containing the embedding vector data (required) and raw text (optional) for the text
+            your model generates.
+
+    Methods:
+    --------
+        replace(**changes):
+            Replaces fields of the schema
+        asdict():
+            Returns the schema as a dictionary. Warning: the types are not maintained, fields are
+            converted to strings.
+        get_used_columns():
+            Returns a set with the unique collection of columns to be used from the dataframe.
     """
 
     def replace(self, **changes):
-        return dataclass_replace(self, **changes)
+        return replace(self, **changes)
 
     def asdict(self) -> Dict[str, str]:
         return asdict(self)
 
     def get_used_columns(self) -> Set[str]:
         columns_used = set()
```

### Comparing `arize-7.0.0rc4/arize/utils/utils.py` & `arize-7.0.0rc5/arize/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 
 def convert_dictionary(d):
     # Takes a dictionary and
     # - casts the keys as strings
     # - turns the values of the dictionary to our proto values pb2.Value()
     converted_dict = {}
-    for (k, v) in d.items():
+    for k, v in d.items():
         val = get_value_object(value=v, name=k)
         if val is not None:
             converted_dict[str(k)] = val
     return converted_dict
 
 
 def get_value_object(name: Union[str, int, float], value):
@@ -163,19 +163,21 @@
     return f"{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}"
 
 
 def overwrite_schema_fields(schema1: Schema, schema2: Schema) -> Schema:
     """This function overwrites a base Schema `schema1` with the fields of `schema2`
     that are not None
 
-    Args:
+    Parameters:
+    -----------
         schema1 (Schema): Base Schema with fields to be overwritten
         schema2 (Schema): New Schema used to overwrite schema1
 
     Returns:
+    --------
         Schema: The resulting schema
     """
     schema_dict_fields = (
         "embedding_feature_column_names",
         "shap_values_column_names",
         "prompt_column_names",
         "response_column_names",
```

### Comparing `arize-7.0.0rc4/arize.egg-info/PKG-INFO` & `arize-7.0.0rc5/arize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.0rc4
+Version: 7.0.0rc5
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.0rc4/arize.egg-info/SOURCES.txt` & `arize-7.0.0rc5/arize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/setup.cfg` & `arize-7.0.0rc5/setup.cfg`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/tests/test_api.py` & `arize-7.0.0rc5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc4/tests/test_utils.py` & `arize-7.0.0rc5/tests/test_utils.py`

 * *Files identical despite different names*

