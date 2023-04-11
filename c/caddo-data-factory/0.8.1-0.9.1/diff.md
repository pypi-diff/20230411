# Comparing `tmp/caddo-data-factory-0.8.1.tar.gz` & `tmp/caddo-data-factory-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caddo-data-factory-0.8.1.tar", last modified: Sun Apr  2 20:19:38 2023, max compression
+gzip compressed data, was "caddo-data-factory-0.9.1.tar", last modified: Mon Apr  3 15:06:41 2023, max compression
```

## Comparing `caddo-data-factory-0.8.1.tar` & `caddo-data-factory-0.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:19:38.709498 caddo-data-factory-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-02 20:19:38.709498 caddo-data-factory-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-02 20:19:24.000000 caddo-data-factory-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:19:38.705498 caddo-data-factory-0.8.1/caddo_data_factory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 20:19:24.000000 caddo-data-factory-0.8.1/caddo_data_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-02 20:19:24.000000 caddo-data-factory-0.8.1/caddo_data_factory/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:19:38.709498 caddo-data-factory-0.8.1/caddo_data_factory/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 20:19:24.000000 caddo-data-factory-0.8.1/caddo_data_factory/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-02 20:19:24.000000 caddo-data-factory-0.8.1/caddo_data_factory/functions/folding_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-02 20:19:24.000000 caddo-data-factory-0.8.1/caddo_data_factory/functions/folding_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-02 20:19:24.000000 caddo-data-factory-0.8.1/caddo_data_factory/functions/folds_preparation.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-02 20:19:24.000000 caddo-data-factory-0.8.1/caddo_data_factory/functions/functions_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:19:38.709498 caddo-data-factory-0.8.1/caddo_data_factory/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 20:19:24.000000 caddo-data-factory-0.8.1/caddo_data_factory/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-02 20:19:24.000000 caddo-data-factory-0.8.1/caddo_data_factory/settings/settings_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 20:19:38.709498 caddo-data-factory-0.8.1/caddo_data_factory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-02 20:19:38.000000 caddo-data-factory-0.8.1/caddo_data_factory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-02 20:19:38.000000 caddo-data-factory-0.8.1/caddo_data_factory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 20:19:38.000000 caddo-data-factory-0.8.1/caddo_data_factory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-02 20:19:38.000000 caddo-data-factory-0.8.1/caddo_data_factory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-02 20:19:38.000000 caddo-data-factory-0.8.1/caddo_data_factory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-02 20:19:25.000000 caddo-data-factory-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 20:19:38.709498 caddo-data-factory-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:06:41.146135 caddo-data-factory-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-03 15:06:41.146135 caddo-data-factory-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-03 15:06:26.000000 caddo-data-factory-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:06:41.146135 caddo-data-factory-0.9.1/caddo_data_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 15:06:26.000000 caddo-data-factory-0.9.1/caddo_data_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-03 15:06:26.000000 caddo-data-factory-0.9.1/caddo_data_factory/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:06:41.146135 caddo-data-factory-0.9.1/caddo_data_factory/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 15:06:26.000000 caddo-data-factory-0.9.1/caddo_data_factory/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-03 15:06:26.000000 caddo-data-factory-0.9.1/caddo_data_factory/functions/folding_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-03 15:06:26.000000 caddo-data-factory-0.9.1/caddo_data_factory/functions/folding_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-03 15:06:26.000000 caddo-data-factory-0.9.1/caddo_data_factory/functions/folds_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-03 15:06:26.000000 caddo-data-factory-0.9.1/caddo_data_factory/functions/functions_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:06:41.146135 caddo-data-factory-0.9.1/caddo_data_factory/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 15:06:26.000000 caddo-data-factory-0.9.1/caddo_data_factory/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-03 15:06:26.000000 caddo-data-factory-0.9.1/caddo_data_factory/settings/settings_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:06:41.146135 caddo-data-factory-0.9.1/caddo_data_factory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-03 15:06:41.000000 caddo-data-factory-0.9.1/caddo_data_factory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-03 15:06:41.000000 caddo-data-factory-0.9.1/caddo_data_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 15:06:41.000000 caddo-data-factory-0.9.1/caddo_data_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-03 15:06:41.000000 caddo-data-factory-0.9.1/caddo_data_factory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-03 15:06:41.000000 caddo-data-factory-0.9.1/caddo_data_factory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-03 15:06:26.000000 caddo-data-factory-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 15:06:41.146135 caddo-data-factory-0.9.1/setup.cfg
```

### Comparing `caddo-data-factory-0.8.1/PKG-INFO` & `caddo-data-factory-0.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caddo-data-factory
-Version: 0.8.1
+Version: 0.9.1
 Summary: Data Factpry for CaddoBenchmark Project
 Author-email: Piotr Tylczyński <piotr@ptl.cloud>, Katarzyna Kulesa <katarzyna.kulesa@kasiait.pl>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `caddo-data-factory-0.8.1/caddo_data_factory/__main__.py` & `caddo-data-factory-0.9.1/caddo_data_factory/__main__.py`

 * *Files identical despite different names*

### Comparing `caddo-data-factory-0.8.1/caddo_data_factory/functions/folds_preparation.py` & `caddo-data-factory-0.9.1/caddo_data_factory/functions/folds_preparation.py`

 * *Files identical despite different names*

### Comparing `caddo-data-factory-0.8.1/caddo_data_factory/settings/settings_reader.py` & `caddo-data-factory-0.9.1/caddo_data_factory/settings/settings_reader.py`

 * *Files identical despite different names*

### Comparing `caddo-data-factory-0.8.1/caddo_data_factory.egg-info/PKG-INFO` & `caddo-data-factory-0.9.1/caddo_data_factory.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caddo-data-factory
-Version: 0.8.1
+Version: 0.9.1
 Summary: Data Factpry for CaddoBenchmark Project
 Author-email: Piotr Tylczyński <piotr@ptl.cloud>, Katarzyna Kulesa <katarzyna.kulesa@kasiait.pl>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `caddo-data-factory-0.8.1/caddo_data_factory.egg-info/SOURCES.txt` & `caddo-data-factory-0.9.1/caddo_data_factory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

