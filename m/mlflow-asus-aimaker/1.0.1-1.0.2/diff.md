# Comparing `tmp/mlflow-asus-aimaker-1.0.1.tar.gz` & `tmp/mlflow-asus-aimaker-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow-asus-aimaker-1.0.1.tar", last modified: Thu Mar 30 03:25:53 2023, max compression
+gzip compressed data, was "mlflow-asus-aimaker-1.0.2.tar", last modified: Tue Apr 11 02:27:08 2023, max compression
```

## Comparing `mlflow-asus-aimaker-1.0.1.tar` & `mlflow-asus-aimaker-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 delg       (501) staff       (20)        0 2023-03-30 03:25:53.738298 mlflow-asus-aimaker-1.0.1/
--rw-r--r--   0 delg       (501) staff       (20)      104 2023-03-30 03:25:53.738138 mlflow-asus-aimaker-1.0.1/PKG-INFO
-drwxr-xr-x   0 delg       (501) staff       (20)        0 2023-03-30 03:25:53.737574 mlflow-asus-aimaker-1.0.1/mlflow_asus_aimaker.egg-info/
--rw-r--r--   0 delg       (501) staff       (20)      104 2023-03-30 03:25:53.000000 mlflow-asus-aimaker-1.0.1/mlflow_asus_aimaker.egg-info/PKG-INFO
--rw-r--r--   0 delg       (501) staff       (20)      370 2023-03-30 03:25:53.000000 mlflow-asus-aimaker-1.0.1/mlflow_asus_aimaker.egg-info/SOURCES.txt
--rw-r--r--   0 delg       (501) staff       (20)        1 2023-03-30 03:25:53.000000 mlflow-asus-aimaker-1.0.1/mlflow_asus_aimaker.egg-info/dependency_links.txt
--rw-r--r--   0 delg       (501) staff       (20)      193 2023-03-30 03:25:53.000000 mlflow-asus-aimaker-1.0.1/mlflow_asus_aimaker.egg-info/entry_points.txt
--rw-r--r--   0 delg       (501) staff       (20)       51 2023-03-30 03:25:53.000000 mlflow-asus-aimaker-1.0.1/mlflow_asus_aimaker.egg-info/requires.txt
--rw-r--r--   0 delg       (501) staff       (20)       14 2023-03-30 03:25:53.000000 mlflow-asus-aimaker-1.0.1/mlflow_asus_aimaker.egg-info/top_level.txt
-drwxr-xr-x   0 delg       (501) staff       (20)        0 2023-03-30 03:25:53.737962 mlflow-asus-aimaker-1.0.1/mlflow_plugin/
--rw-r--r--   0 delg       (501) staff       (20)        0 2022-01-14 07:00:01.000000 mlflow-asus-aimaker-1.0.1/mlflow_plugin/__init__.py
--rw-r--r--   0 delg       (501) staff       (20)     1672 2022-08-30 07:37:16.000000 mlflow-asus-aimaker-1.0.1/mlflow_plugin/plugin_model_rest_store.py
--rw-r--r--   0 delg       (501) staff       (20)     3711 2022-09-15 03:20:55.000000 mlflow-asus-aimaker-1.0.1/mlflow_plugin/plugin_rest_store.py
--rw-r--r--   0 delg       (501) staff       (20)       38 2023-03-30 03:25:53.738343 mlflow-asus-aimaker-1.0.1/setup.cfg
--rw-r--r--   0 delg       (501) staff       (20)      511 2023-03-30 03:25:02.000000 mlflow-asus-aimaker-1.0.1/setup.py
+drwxr-xr-x   0 delg       (501) staff       (20)        0 2023-04-11 02:27:08.541209 mlflow-asus-aimaker-1.0.2/
+-rw-r--r--   0 delg       (501) staff       (20)      104 2023-04-11 02:27:08.540990 mlflow-asus-aimaker-1.0.2/PKG-INFO
+drwxr-xr-x   0 delg       (501) staff       (20)        0 2023-04-11 02:27:08.538493 mlflow-asus-aimaker-1.0.2/mlflow_asus_aimaker.egg-info/
+-rw-r--r--   0 delg       (501) staff       (20)      104 2023-04-11 02:27:08.000000 mlflow-asus-aimaker-1.0.2/mlflow_asus_aimaker.egg-info/PKG-INFO
+-rw-r--r--   0 delg       (501) staff       (20)      370 2023-04-11 02:27:08.000000 mlflow-asus-aimaker-1.0.2/mlflow_asus_aimaker.egg-info/SOURCES.txt
+-rw-r--r--   0 delg       (501) staff       (20)        1 2023-04-11 02:27:08.000000 mlflow-asus-aimaker-1.0.2/mlflow_asus_aimaker.egg-info/dependency_links.txt
+-rw-r--r--   0 delg       (501) staff       (20)      193 2023-04-11 02:27:08.000000 mlflow-asus-aimaker-1.0.2/mlflow_asus_aimaker.egg-info/entry_points.txt
+-rw-r--r--   0 delg       (501) staff       (20)       59 2023-04-11 02:27:08.000000 mlflow-asus-aimaker-1.0.2/mlflow_asus_aimaker.egg-info/requires.txt
+-rw-r--r--   0 delg       (501) staff       (20)       14 2023-04-11 02:27:08.000000 mlflow-asus-aimaker-1.0.2/mlflow_asus_aimaker.egg-info/top_level.txt
+drwxr-xr-x   0 delg       (501) staff       (20)        0 2023-04-11 02:27:08.540528 mlflow-asus-aimaker-1.0.2/mlflow_plugin/
+-rw-r--r--   0 delg       (501) staff       (20)        0 2022-01-14 07:00:01.000000 mlflow-asus-aimaker-1.0.2/mlflow_plugin/__init__.py
+-rw-r--r--   0 delg       (501) staff       (20)     1672 2022-08-30 07:37:16.000000 mlflow-asus-aimaker-1.0.2/mlflow_plugin/plugin_model_rest_store.py
+-rw-r--r--   0 delg       (501) staff       (20)     3711 2022-09-15 03:20:55.000000 mlflow-asus-aimaker-1.0.2/mlflow_plugin/plugin_rest_store.py
+-rw-r--r--   0 delg       (501) staff       (20)       38 2023-04-11 02:27:08.541316 mlflow-asus-aimaker-1.0.2/setup.cfg
+-rw-r--r--   0 delg       (501) staff       (20)      519 2023-04-11 02:26:47.000000 mlflow-asus-aimaker-1.0.2/setup.py
```

### Comparing `mlflow-asus-aimaker-1.0.1/mlflow_plugin/plugin_model_rest_store.py` & `mlflow-asus-aimaker-1.0.2/mlflow_plugin/plugin_model_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-asus-aimaker-1.0.1/mlflow_plugin/plugin_rest_store.py` & `mlflow-asus-aimaker-1.0.2/mlflow_plugin/plugin_rest_store.py`

 * *Files identical despite different names*

