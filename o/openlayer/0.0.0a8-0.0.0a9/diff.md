# Comparing `tmp/openlayer-0.0.0a8.tar.gz` & `tmp/openlayer-0.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlayer-0.0.0a8.tar", last modified: Mon Feb 27 16:39:20 2023, max compression
+gzip compressed data, was "openlayer-0.0.0a9.tar", last modified: Wed Mar  8 09:24:27 2023, max compression
```

## Comparing `openlayer-0.0.0a8.tar` & `openlayer-0.0.0a9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 16:39:20.191770 openlayer-0.0.0a8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-27 16:38:42.000000 openlayer-0.0.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-02-27 16:39:20.191770 openlayer-0.0.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-02-27 16:38:42.000000 openlayer-0.0.0a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 16:39:20.187770 openlayer-0.0.0a8/openlayer/
--rw-r--r--   0 runner    (1001) docker     (123)    48105 2023-02-27 16:38:43.000000 openlayer-0.0.0a8/openlayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-02-27 16:38:43.000000 openlayer-0.0.0a8/openlayer/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-02-27 16:38:43.000000 openlayer-0.0.0a8/openlayer/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-02-27 16:38:43.000000 openlayer-0.0.0a8/openlayer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-02-27 16:38:43.000000 openlayer-0.0.0a8/openlayer/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-02-27 16:38:43.000000 openlayer-0.0.0a8/openlayer/prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-02-27 16:38:43.000000 openlayer-0.0.0a8/openlayer/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-02-27 16:38:43.000000 openlayer-0.0.0a8/openlayer/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-02-27 16:38:43.000000 openlayer-0.0.0a8/openlayer/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-02-27 16:38:43.000000 openlayer-0.0.0a8/openlayer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    54792 2023-02-27 16:38:43.000000 openlayer-0.0.0a8/openlayer/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-27 16:38:43.000000 openlayer-0.0.0a8/openlayer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 16:39:20.191770 openlayer-0.0.0a8/openlayer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-02-27 16:39:20.000000 openlayer-0.0.0a8/openlayer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-02-27 16:39:20.000000 openlayer-0.0.0a8/openlayer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 16:39:20.000000 openlayer-0.0.0a8/openlayer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 16:39:20.000000 openlayer-0.0.0a8/openlayer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-27 16:39:20.000000 openlayer-0.0.0a8/openlayer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-27 16:39:20.000000 openlayer-0.0.0a8/openlayer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-27 16:38:43.000000 openlayer-0.0.0a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-02-27 16:39:20.191770 openlayer-0.0.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-27 16:38:43.000000 openlayer-0.0.0a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 09:24:27.829157 openlayer-0.0.0a9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-08 09:24:27.829157 openlayer-0.0.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 09:24:27.825157 openlayer-0.0.0a9/openlayer/
+-rw-r--r--   0 runner    (1001) docker     (123)    48105 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54794 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 09:24:27.829157 openlayer-0.0.0a9/openlayer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-08 09:24:27.000000 openlayer-0.0.0a9/openlayer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-08 09:24:27.000000 openlayer-0.0.0a9/openlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 09:24:27.000000 openlayer-0.0.0a9/openlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 09:24:27.000000 openlayer-0.0.0a9/openlayer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-08 09:24:27.000000 openlayer-0.0.0a9/openlayer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-08 09:24:27.000000 openlayer-0.0.0a9/openlayer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-08 09:24:27.829157 openlayer-0.0.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/setup.py
```

### Comparing `openlayer-0.0.0a8/LICENSE` & `openlayer-0.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `openlayer-0.0.0a8/PKG-INFO` & `openlayer-0.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlayer
-Version: 0.0.0a8
+Version: 0.0.0a9
 Summary: The official Python API library for Openlayer: the Testing and Debugging Platform for AI
 Home-page: https://github.com/openlayer-ai/openlayer-python
 Author: Unbox Inc.
 Project-URL: Documentation, https://docs.openlayer.com/
 Project-URL: Openlayer User Slack Group, https://l.linklyhq.com/l/1DG73
 Keywords: MLOps,AI,Openlayer
 Classifier: Operating System :: OS Independent
```

### Comparing `openlayer-0.0.0a8/README.md` & `openlayer-0.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `openlayer-0.0.0a8/openlayer/__init__.py` & `openlayer-0.0.0a9/openlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.0.0a8/openlayer/api.py` & `openlayer-0.0.0a9/openlayer/api.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.0.0a8/openlayer/datasets.py` & `openlayer-0.0.0a9/openlayer/datasets.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.0.0a8/openlayer/exceptions.py` & `openlayer-0.0.0a9/openlayer/exceptions.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.0.0a8/openlayer/models.py` & `openlayer-0.0.0a9/openlayer/models.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.0.0a8/openlayer/prediction_job.py` & `openlayer-0.0.0a9/openlayer/prediction_job.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.0.0a8/openlayer/projects.py` & `openlayer-0.0.0a9/openlayer/projects.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.0.0a8/openlayer/schemas.py` & `openlayer-0.0.0a9/openlayer/schemas.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.0.0a8/openlayer/tasks.py` & `openlayer-0.0.0a9/openlayer/tasks.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.0.0a8/openlayer/utils.py` & `openlayer-0.0.0a9/openlayer/utils.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.0.0a8/openlayer/validators.py` & `openlayer-0.0.0a9/openlayer/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
                 validation_dataset_config = self._load_dataset_config_from_bundle(
                     "validation"
                 )
 
                 sample_data = None
                 if "textColumnName" in validation_dataset_config:
                     sample_data = validation_dataset_df[
-                        validation_dataset_config["textColumnName"]
+                        [validation_dataset_config["textColumnName"]]
                     ].head()
 
                 else:
                     sample_data = validation_dataset_df[
                         validation_dataset_config["featureNames"]
                     ].head()
```

### Comparing `openlayer-0.0.0a8/openlayer.egg-info/PKG-INFO` & `openlayer-0.0.0a9/openlayer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlayer
-Version: 0.0.0a8
+Version: 0.0.0a9
 Summary: The official Python API library for Openlayer: the Testing and Debugging Platform for AI
 Home-page: https://github.com/openlayer-ai/openlayer-python
 Author: Unbox Inc.
 Project-URL: Documentation, https://docs.openlayer.com/
 Project-URL: Openlayer User Slack Group, https://l.linklyhq.com/l/1DG73
 Keywords: MLOps,AI,Openlayer
 Classifier: Operating System :: OS Independent
```

### Comparing `openlayer-0.0.0a8/setup.cfg` & `openlayer-0.0.0a9/setup.cfg`

 * *Files identical despite different names*

