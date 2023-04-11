# Comparing `tmp/nowcasting_datamodel-1.2.4.tar.gz` & `tmp/nowcasting_datamodel-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_datamodel-1.2.4.tar", last modified: Thu Apr  6 13:15:45 2023, max compression
+gzip compressed data, was "nowcasting_datamodel-1.2.5.tar", last modified: Tue Apr 11 13:34:21 2023, max compression
```

## Comparing `nowcasting_datamodel-1.2.4.tar` & `nowcasting_datamodel-1.2.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:15:45.325997 nowcasting_datamodel-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-06 13:15:45.325997 nowcasting_datamodel-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/diagram_pv.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:15:45.321997 nowcasting_datamodel-1.2.4/nowcasting_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:15:45.321997 nowcasting_datamodel-1.2.4/nowcasting_datamodel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/migrations/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:15:45.325997 nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/national.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:15:45.325997 nowcasting_datamodel-1.2.4/nowcasting_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/read/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)    22415 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/read/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/read/read_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/read/read_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/read/read_pv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:15:45.325997 nowcasting_datamodel-1.2.4/nowcasting_datamodel/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/save/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/save/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/save/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:15:45.321997 nowcasting_datamodel-1.2.4/nowcasting_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-06 13:15:45.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-06 13:15:45.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 13:15:45.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-06 13:15:45.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-06 13:15:45.000000 nowcasting_datamodel-1.2.4/nowcasting_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 13:15:45.325997 nowcasting_datamodel-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:15:45.325997 nowcasting_datamodel-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/tests/test_databaseconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/tests/test_fake_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/tests/test_national.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-06 13:15:31.000000 nowcasting_datamodel-1.2.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.479594 nowcasting_datamodel-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-11 13:34:21.479594 nowcasting_datamodel-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/diagram_pv.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.463594 nowcasting_datamodel-1.2.5/nowcasting_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.467594 nowcasting_datamodel-1.2.5/nowcasting_datamodel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/migrations/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.471594 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/national.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.475594 nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22415 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read_pv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.475594 nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.463594 nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-11 13:34:21.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-11 13:34:21.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:34:21.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 13:34:21.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 13:34:21.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:34:21.479594 nowcasting_datamodel-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.479594 nowcasting_datamodel-1.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/tests/test_databaseconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/tests/test_fake_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/tests/test_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/tests/test_utils.py
```

### Comparing `nowcasting_datamodel-1.2.4/PKG-INFO` & `nowcasting_datamodel-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_datamodel
-Version: 1.2.4
+Version: 1.2.5
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.2.4/README.md` & `nowcasting_datamodel-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/diagram.png` & `nowcasting_datamodel-1.2.5/diagram.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/diagram_pv.png` & `nowcasting_datamodel-1.2.5/diagram_pv.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/connection.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/fake.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/migrations/app.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/migrations/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/__init__.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/convert.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/convert.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/forecast.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/forecast.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/gsp.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/metric.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/models.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/models.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/pv.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/models/utils.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/national.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/read/blend.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/blend.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/read/read.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/read/read_gsp.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read_gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/read/read_metric.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read_metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/read/read_pv.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/save/adjust.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/adjust.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/save/save.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/save.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/save/update.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     # 2. create forecast value latest
     forecast_values = []
     for forecast_value in forecast.forecast_values:
         forecast_value_latest = change_forecast_value_to_latest(
             forecast_value,
             gsp_id=forecast.location.gsp_id,
             forecast_id=forecast_historic.id,
-            model_id=forecast_historic.model_id,
+            model_id=forecast.model_id,
         )
         logger.debug(f"{forecast_historic.model_id=}")
         forecast_values.append(forecast_value_latest.__dict__)
 
     # upsert forecast values
     upsert(session=session, model=ForecastValueLatestSQL, rows=forecast_values)
```

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel/utils.py` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel.egg-info/PKG-INFO` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-datamodel
-Version: 1.2.4
+Version: 1.2.5
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.2.4/nowcasting_datamodel.egg-info/SOURCES.txt` & `nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/setup.py` & `nowcasting_datamodel-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/tests/test_databaseconnection.py` & `nowcasting_datamodel-1.2.5/tests/test_databaseconnection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/tests/test_fake.py` & `nowcasting_datamodel-1.2.5/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/tests/test_fake_pv.py` & `nowcasting_datamodel-1.2.5/tests/test_fake_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/tests/test_national.py` & `nowcasting_datamodel-1.2.5/tests/test_national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.4/tests/test_utils.py` & `nowcasting_datamodel-1.2.5/tests/test_utils.py`

 * *Files identical despite different names*

