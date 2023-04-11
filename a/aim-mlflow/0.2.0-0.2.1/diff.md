# Comparing `tmp/aim-mlflow-0.2.0.tar.gz` & `tmp/aim-mlflow-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/mvanyan/proj/aimlflow/dist/.tmp-5k0rhxyk/aim-mlflow-0.2.0.tar", last modified: Tue Feb 28 08:18:52 2023, max compression
+gzip compressed data, was "/Users/mvanyan/proj/aimlflow/dist/.tmp-sch8ttk_/aim-mlflow-0.2.1.tar", last modified: Tue Apr 11 12:36:30 2023, max compression
```

## Comparing `aim-mlflow-0.2.0.tar` & `aim-mlflow-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mvanyan    (502) staff       (20)        0 2023-02-28 08:18:52.000000 aim-mlflow-0.2.0/
--rw-r--r--   0 mvanyan    (502) staff       (20)    11357 2022-12-22 01:28:03.000000 aim-mlflow-0.2.0/LICENSE
--rw-r--r--   0 mvanyan    (502) staff       (20)     3304 2023-02-28 08:18:52.000000 aim-mlflow-0.2.0/PKG-INFO
--rw-r--r--   0 mvanyan    (502) staff       (20)     2706 2023-01-18 15:17:01.000000 aim-mlflow-0.2.0/README.md
-drwxr-xr-x   0 mvanyan    (502) staff       (20)        0 2023-02-28 08:18:52.000000 aim-mlflow-0.2.0/aim_mlflow.egg-info/
--rw-r--r--   0 mvanyan    (502) staff       (20)     3304 2023-02-28 08:18:52.000000 aim-mlflow-0.2.0/aim_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 mvanyan    (502) staff       (20)      324 2023-02-28 08:18:52.000000 aim-mlflow-0.2.0/aim_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 mvanyan    (502) staff       (20)        1 2023-02-28 08:18:52.000000 aim-mlflow-0.2.0/aim_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 mvanyan    (502) staff       (20)       58 2023-02-28 08:18:52.000000 aim-mlflow-0.2.0/aim_mlflow.egg-info/entry_points.txt
--rw-r--r--   0 mvanyan    (502) staff       (20)       16 2023-02-28 08:18:52.000000 aim-mlflow-0.2.0/aim_mlflow.egg-info/requires.txt
--rw-r--r--   0 mvanyan    (502) staff       (20)        9 2023-02-28 08:18:52.000000 aim-mlflow-0.2.0/aim_mlflow.egg-info/top_level.txt
-drwxr-xr-x   0 mvanyan    (502) staff       (20)        0 2023-02-28 08:18:52.000000 aim-mlflow-0.2.0/aimlflow/
--rw-r--r--   0 mvanyan    (502) staff       (20)        5 2023-02-28 08:17:49.000000 aim-mlflow-0.2.0/aimlflow/VERSION
--rw-r--r--   0 mvanyan    (502) staff       (20)        0 2023-01-10 23:12:31.000000 aim-mlflow-0.2.0/aimlflow/__init__.py
--rw-r--r--   0 mvanyan    (502) staff       (20)     1670 2023-02-28 08:16:00.000000 aim-mlflow-0.2.0/aimlflow/cli.py
--rw-r--r--   0 mvanyan    (502) staff       (20)     8616 2023-02-28 08:16:00.000000 aim-mlflow-0.2.0/aimlflow/utils.py
--rw-r--r--   0 mvanyan    (502) staff       (20)     4656 2023-02-28 08:16:00.000000 aim-mlflow-0.2.0/aimlflow/watcher.py
--rw-r--r--   0 mvanyan    (502) staff       (20)       38 2023-02-28 08:18:52.000000 aim-mlflow-0.2.0/setup.cfg
--rw-r--r--   0 mvanyan    (502) staff       (20)     2615 2023-01-18 15:22:52.000000 aim-mlflow-0.2.0/setup.py
+drwxr-xr-x   0 mvanyan    (502) staff       (20)        0 2023-04-11 12:36:30.000000 aim-mlflow-0.2.1/
+-rw-r--r--   0 mvanyan    (502) staff       (20)    11357 2022-12-22 01:28:03.000000 aim-mlflow-0.2.1/LICENSE
+-rw-r--r--   0 mvanyan    (502) staff       (20)     3304 2023-04-11 12:36:30.000000 aim-mlflow-0.2.1/PKG-INFO
+-rw-r--r--   0 mvanyan    (502) staff       (20)     2706 2023-01-18 15:17:01.000000 aim-mlflow-0.2.1/README.md
+drwxr-xr-x   0 mvanyan    (502) staff       (20)        0 2023-04-11 12:36:30.000000 aim-mlflow-0.2.1/aim_mlflow.egg-info/
+-rw-r--r--   0 mvanyan    (502) staff       (20)     3304 2023-04-11 12:36:30.000000 aim-mlflow-0.2.1/aim_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 mvanyan    (502) staff       (20)      324 2023-04-11 12:36:30.000000 aim-mlflow-0.2.1/aim_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 mvanyan    (502) staff       (20)        1 2023-04-11 12:36:30.000000 aim-mlflow-0.2.1/aim_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 mvanyan    (502) staff       (20)       58 2023-04-11 12:36:30.000000 aim-mlflow-0.2.1/aim_mlflow.egg-info/entry_points.txt
+-rw-r--r--   0 mvanyan    (502) staff       (20)       16 2023-04-11 12:36:30.000000 aim-mlflow-0.2.1/aim_mlflow.egg-info/requires.txt
+-rw-r--r--   0 mvanyan    (502) staff       (20)        9 2023-04-11 12:36:30.000000 aim-mlflow-0.2.1/aim_mlflow.egg-info/top_level.txt
+drwxr-xr-x   0 mvanyan    (502) staff       (20)        0 2023-04-11 12:36:30.000000 aim-mlflow-0.2.1/aimlflow/
+-rw-r--r--   0 mvanyan    (502) staff       (20)        5 2023-04-11 12:36:22.000000 aim-mlflow-0.2.1/aimlflow/VERSION
+-rw-r--r--   0 mvanyan    (502) staff       (20)        0 2023-01-10 23:12:31.000000 aim-mlflow-0.2.1/aimlflow/__init__.py
+-rw-r--r--   0 mvanyan    (502) staff       (20)     1670 2023-02-28 08:16:00.000000 aim-mlflow-0.2.1/aimlflow/cli.py
+-rw-r--r--   0 mvanyan    (502) staff       (20)     8620 2023-04-11 12:29:39.000000 aim-mlflow-0.2.1/aimlflow/utils.py
+-rw-r--r--   0 mvanyan    (502) staff       (20)     4656 2023-02-28 08:16:00.000000 aim-mlflow-0.2.1/aimlflow/watcher.py
+-rw-r--r--   0 mvanyan    (502) staff       (20)       38 2023-04-11 12:36:30.000000 aim-mlflow-0.2.1/setup.cfg
+-rw-r--r--   0 mvanyan    (502) staff       (20)     2615 2023-01-18 15:22:52.000000 aim-mlflow-0.2.1/setup.py
```

### Comparing `aim-mlflow-0.2.0/LICENSE` & `aim-mlflow-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aim-mlflow-0.2.0/PKG-INFO` & `aim-mlflow-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aim-mlflow
-Version: 0.2.0
+Version: 0.2.1
 Summary: Aim-MLflow integration
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `aim-mlflow-0.2.0/README.md` & `aim-mlflow-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aim-mlflow-0.2.0/aim_mlflow.egg-info/PKG-INFO` & `aim-mlflow-0.2.1/aim_mlflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aim-mlflow
-Version: 0.2.0
+Version: 0.2.1
 Summary: Aim-MLflow integration
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `aim-mlflow-0.2.0/aimlflow/cli.py` & `aim-mlflow-0.2.1/aimlflow/cli.py`

 * *Files identical despite different names*

### Comparing `aim-mlflow-0.2.0/aimlflow/utils.py` & `aim-mlflow-0.2.1/aimlflow/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
         while True:
             time.sleep(24 * 60 * 60)  # sleep for a day
     except KeyboardInterrupt:
         watcher.stop()
 
 
 def _map_nested_dicts(fun, tree):
-    if isinstance(tree, collections.Mapping):
+    if isinstance(tree, collections.abc.Mapping):
         return {k: _map_nested_dicts(fun, subtree) for k, subtree in tree.items()}
     else:
         return fun(tree)
 
 
 def _try_parse_str(s):
     assert isinstance(s, str), f'Expected a string, got {s} of type {type(s)}'
```

### Comparing `aim-mlflow-0.2.0/aimlflow/watcher.py` & `aim-mlflow-0.2.1/aimlflow/watcher.py`

 * *Files identical despite different names*

### Comparing `aim-mlflow-0.2.0/setup.py` & `aim-mlflow-0.2.1/setup.py`

 * *Files identical despite different names*

