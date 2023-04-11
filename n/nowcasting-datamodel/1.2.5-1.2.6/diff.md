# Comparing `tmp/nowcasting_datamodel-1.2.5.tar.gz` & `tmp/nowcasting_datamodel-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_datamodel-1.2.5.tar", last modified: Tue Apr 11 13:34:21 2023, max compression
+gzip compressed data, was "nowcasting_datamodel-1.2.6.tar", last modified: Tue Apr 11 16:47:53 2023, max compression
```

## Comparing `nowcasting_datamodel-1.2.5.tar` & `nowcasting_datamodel-1.2.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.479594 nowcasting_datamodel-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-11 13:34:21.479594 nowcasting_datamodel-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/diagram_pv.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.463594 nowcasting_datamodel-1.2.5/nowcasting_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.467594 nowcasting_datamodel-1.2.5/nowcasting_datamodel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/migrations/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.471594 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/national.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.475594 nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)    22415 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read_pv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.475594 nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.463594 nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-11 13:34:21.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-11 13:34:21.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:34:21.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 13:34:21.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 13:34:21.000000 nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:34:21.479594 nowcasting_datamodel-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:34:21.479594 nowcasting_datamodel-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/tests/test_databaseconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/tests/test_fake_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/tests/test_national.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-11 13:34:09.000000 nowcasting_datamodel-1.2.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:47:53.141743 nowcasting_datamodel-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-11 16:47:53.141743 nowcasting_datamodel-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/diagram_pv.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:47:53.137743 nowcasting_datamodel-1.2.6/nowcasting_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:47:53.137743 nowcasting_datamodel-1.2.6/nowcasting_datamodel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/migrations/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:47:53.137743 nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/national.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:47:53.141743 nowcasting_datamodel-1.2.6/nowcasting_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/read/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22415 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/read/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/read/read_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/read/read_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/read/read_pv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:47:53.141743 nowcasting_datamodel-1.2.6/nowcasting_datamodel/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/save/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/save/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:47:53.137743 nowcasting_datamodel-1.2.6/nowcasting_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-11 16:47:53.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-11 16:47:53.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:47:53.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 16:47:53.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 16:47:53.000000 nowcasting_datamodel-1.2.6/nowcasting_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 16:47:53.141743 nowcasting_datamodel-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:47:53.141743 nowcasting_datamodel-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/tests/test_databaseconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/tests/test_fake_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/tests/test_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-11 16:47:41.000000 nowcasting_datamodel-1.2.6/tests/test_utils.py
```

### Comparing `nowcasting_datamodel-1.2.5/PKG-INFO` & `nowcasting_datamodel-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_datamodel
-Version: 1.2.5
+Version: 1.2.6
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.2.5/README.md` & `nowcasting_datamodel-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/diagram.png` & `nowcasting_datamodel-1.2.6/diagram.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/diagram_pv.png` & `nowcasting_datamodel-1.2.6/diagram_pv.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/connection.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/fake.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/migrations/app.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/migrations/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/__init__.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/convert.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/convert.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/forecast.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/forecast.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/gsp.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/metric.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/models.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/models.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/pv.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/models/utils.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/national.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/blend.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/read/blend.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,14 @@
     # sort by target time
     forecast_values_blended.sort_values(by="target_time", inplace=True)
 
     # change in to list of ForecastValue objects
     forecast_values = []
     logger.debug(forecast_values_blended)
     for i, row in forecast_values_blended.iterrows():
-        print(row)
         forecast_value = ForecastValue(
             target_time=row.target_time,
             expected_power_generation_megawatts=row.expected_power_generation_megawatts,
         )
         forecast_value._adjust_mw = row.adjust_mw
         forecast_values.append(forecast_value)
```

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/read/read.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read_gsp.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/read/read_gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read_metric.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/read/read_metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/read/read_pv.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/read/read_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/adjust.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/save/adjust.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/save.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/save/save.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/save/update.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/save/update.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel/utils.py` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/PKG-INFO` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-datamodel
-Version: 1.2.5
+Version: 1.2.6
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.2.5/nowcasting_datamodel.egg-info/SOURCES.txt` & `nowcasting_datamodel-1.2.6/nowcasting_datamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/setup.py` & `nowcasting_datamodel-1.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/tests/test_databaseconnection.py` & `nowcasting_datamodel-1.2.6/tests/test_databaseconnection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/tests/test_fake.py` & `nowcasting_datamodel-1.2.6/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/tests/test_fake_pv.py` & `nowcasting_datamodel-1.2.6/tests/test_fake_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/tests/test_national.py` & `nowcasting_datamodel-1.2.6/tests/test_national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.2.5/tests/test_utils.py` & `nowcasting_datamodel-1.2.6/tests/test_utils.py`

 * *Files identical despite different names*

