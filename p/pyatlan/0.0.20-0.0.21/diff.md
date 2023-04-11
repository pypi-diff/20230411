# Comparing `tmp/pyatlan-0.0.20.tar.gz` & `tmp/pyatlan-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.0.20.tar", last modified: Wed Apr  5 08:13:13 2023, max compression
+gzip compressed data, was "pyatlan-0.0.21.tar", last modified: Tue Apr 11 12:30:56 2023, max compression
```

## Comparing `pyatlan-0.0.20.tar` & `pyatlan-0.0.21.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:13:13.401250 pyatlan-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-04-05 08:13:03.000000 pyatlan-0.0.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-05 08:13:03.000000 pyatlan-0.0.20/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-05 08:13:03.000000 pyatlan-0.0.20/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-05 08:13:13.401250 pyatlan-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-05 08:13:03.000000 pyatlan-0.0.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:13:13.393250 pyatlan-0.0.20/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 08:13:03.000000 pyatlan-0.0.20/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:13:13.397250 pyatlan-0.0.20/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-05 08:13:03.000000 pyatlan-0.0.20/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-05 08:13:03.000000 pyatlan-0.0.20/pyatlan/cache/classification_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-04-05 08:13:03.000000 pyatlan-0.0.20/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-05 08:13:03.000000 pyatlan-0.0.20/pyatlan/cache/role_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:13:13.397250 pyatlan-0.0.20/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-05 08:13:03.000000 pyatlan-0.0.20/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19467 2023-04-05 08:13:03.000000 pyatlan-0.0.20/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-05 08:13:03.000000 pyatlan-0.0.20/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-05 08:13:03.000000 pyatlan-0.0.20/pyatlan/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-05 08:13:03.000000 pyatlan-0.0.20/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:13:13.397250 pyatlan-0.0.20/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 08:13:03.000000 pyatlan-0.0.20/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-05 08:13:03.000000 pyatlan-0.0.20/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:13:13.397250 pyatlan-0.0.20/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 08:13:03.000000 pyatlan-0.0.20/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:13:13.397250 pyatlan-0.0.20/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-05 08:13:03.000000 pyatlan-0.0.20/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   743514 2023-04-05 08:13:04.000000 pyatlan-0.0.20/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-05 08:13:04.000000 pyatlan-0.0.20/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-05 08:13:04.000000 pyatlan-0.0.20/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-05 08:13:04.000000 pyatlan-0.0.20/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-05 08:13:04.000000 pyatlan-0.0.20/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-05 08:13:04.000000 pyatlan-0.0.20/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    58604 2023-04-05 08:13:04.000000 pyatlan-0.0.20/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-05 08:13:04.000000 pyatlan-0.0.20/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-04-05 08:13:04.000000 pyatlan-0.0.20/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-05 08:13:04.000000 pyatlan-0.0.20/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-05 08:13:04.000000 pyatlan-0.0.20/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:13:13.397250 pyatlan-0.0.20/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-05 08:13:13.000000 pyatlan-0.0.20/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-05 08:13:13.000000 pyatlan-0.0.20/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 08:13:13.000000 pyatlan-0.0.20/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 08:13:13.000000 pyatlan-0.0.20/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-05 08:13:13.000000 pyatlan-0.0.20/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-05 08:13:13.000000 pyatlan-0.0.20/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 08:13:13.401250 pyatlan-0.0.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-05 08:13:04.000000 pyatlan-0.0.20/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:13:13.397250 pyatlan-0.0.20/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 08:13:04.000000 pyatlan-0.0.20/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:13:13.401250 pyatlan-0.0.20/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 08:13:04.000000 pyatlan-0.0.20/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-05 08:13:04.000000 pyatlan-0.0.20/tests/integration/classification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-05 08:13:04.000000 pyatlan-0.0.20/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-05 08:13:04.000000 pyatlan-0.0.20/tests/integration/role_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-05 08:13:04.000000 pyatlan-0.0.20/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27136 2023-04-05 08:13:04.000000 pyatlan-0.0.20/tests/integration/test_entity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-05 08:13:04.000000 pyatlan-0.0.20/tests/integration/test_index_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:13:13.401250 pyatlan-0.0.20/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 08:13:04.000000 pyatlan-0.0.20/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-05 08:13:04.000000 pyatlan-0.0.20/tests/unit/test_classification_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    47540 2023-04-05 08:13:04.000000 pyatlan-0.0.20/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31745 2023-04-05 08:13:04.000000 pyatlan-0.0.20/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-04-05 08:13:04.000000 pyatlan-0.0.20/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-05 08:13:04.000000 pyatlan-0.0.20/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.171042 pyatlan-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-04-11 12:30:46.000000 pyatlan-0.0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 12:30:46.000000 pyatlan-0.0.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-11 12:30:46.000000 pyatlan-0.0.21/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-11 12:30:56.167042 pyatlan-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 12:30:46.000000 pyatlan-0.0.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.163042 pyatlan-0.0.21/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.163042 pyatlan-0.0.21/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/cache/classification_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/cache/role_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.163042 pyatlan-0.0.21/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.163042 pyatlan-0.0.21/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.163042 pyatlan-0.0.21/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.167042 pyatlan-0.0.21/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   745939 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 12:30:46.000000 pyatlan-0.0.21/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.163042 pyatlan-0.0.21/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-11 12:30:56.000000 pyatlan-0.0.21/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-11 12:30:56.000000 pyatlan-0.0.21/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:30:56.000000 pyatlan-0.0.21/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:30:55.000000 pyatlan-0.0.21/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 12:30:56.000000 pyatlan-0.0.21/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 12:30:56.000000 pyatlan-0.0.21/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 12:30:56.171042 pyatlan-0.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-11 12:30:46.000000 pyatlan-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.167042 pyatlan-0.0.21/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.167042 pyatlan-0.0.21/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/integration/classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/integration/role_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29930 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/integration/test_entity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/integration/test_index_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:30:56.167042 pyatlan-0.0.21/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/unit/test_classification_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48559 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-11 12:30:46.000000 pyatlan-0.0.21/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.0.20/LICENSE` & `pyatlan-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/PKG-INFO` & `pyatlan-0.0.21/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.20
+Version: 0.0.21
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.20/README.md` & `pyatlan-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/pyatlan/cache/classification_cache.py` & `pyatlan-0.0.21/pyatlan/cache/classification_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.0.21/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/pyatlan/cache/role_cache.py` & `pyatlan-0.0.21/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/pyatlan/client/atlan.py` & `pyatlan-0.0.21/pyatlan/client/atlan.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,14 +152,15 @@
             self._criteria.dsl.from_ = self._start
             self._criteria.dsl.size = self._size
             raw_json = self._client._call_api(
                 INDEX_SEARCH,
                 request_obj=self._criteria,
             )
             if "entities" not in raw_json:
+                self._assets = []
                 return False
             self._assets = parse_obj_as(list[Asset], raw_json["entities"])
             return True
 
         def __iter__(self) -> Generator[Asset, None, None]:
             while True:
                 yield from self.current_page()
@@ -316,15 +317,15 @@
                     message=f"Asset with qualifiedName {qualified_name} "
                     f"is not of the type requested: {asset_type.__name__}.",
                     code="ATLAN-PYTHON-404-002",
                 )
             return asset
         except AtlanError as ae:
             if ae.status_code == HTTPStatus.NOT_FOUND:
-                raise NotFoundError(message=ae.user_message, code=ae.code)
+                raise NotFoundError(message=ae.user_message, code=ae.code) from ae
             raise ae
 
     @validate_arguments()
     def get_asset_by_guid(
         self,
         guid: str,
         asset_type: Type[A],
@@ -337,31 +338,44 @@
         }
 
         try:
             raw_json = self._call_api(
                 GET_ENTITY_BY_GUID.format_path_with_params(guid),
                 query_params,
             )
-            raw_json["entity"]["attributes"].update(
-                raw_json["entity"]["relationshipAttributes"]
-            )
+            if (
+                "relationshipAttributes" in raw_json["entity"]
+                and raw_json["entity"]["relationshipAttributes"]
+            ):
+                raw_json["entity"]["attributes"].update(
+                    raw_json["entity"]["relationshipAttributes"]
+                )
             raw_json["entity"]["relationshipAttributes"] = {}
             asset = AssetResponse[A](**raw_json).entity
             asset.is_incomplete = False
             if not isinstance(asset, asset_type):
                 raise NotFoundError(
                     message=f"Asset with GUID {guid} is not of the type requested: {asset_type.__name__}.",
                     code="ATLAN-PYTHON-404-002",
                 )
             return asset
         except AtlanError as ae:
             if ae.status_code == HTTPStatus.NOT_FOUND:
-                raise NotFoundError(message=ae.user_message, code=ae.code)
+                raise NotFoundError(message=ae.user_message, code=ae.code) from ae
             raise ae
 
+    @validate_arguments()
+    def retrieve_minimal(self, guid: str, asset_type: Type[A]) -> A:
+        return self.get_asset_by_guid(
+            guid=guid,
+            asset_type=asset_type,
+            min_ext_info=True,
+            ignore_relationships=True,
+        )
+
     def upsert(
         self,
         entity: Union[Asset, list[Asset]],
         replace_classifications: bool = False,
         replace_custom_metadata: bool = False,
     ) -> AssetMutationResponse:
         query_params = {
@@ -383,14 +397,21 @@
     def purge_entity_by_guid(self, guid) -> AssetMutationResponse:
         raw_json = self._call_api(
             DELETE_ENTITY_BY_GUID.format_path_with_params(guid),
             {"deleteType": AtlanDeleteType.HARD.value},
         )
         return AssetMutationResponse(**raw_json)
 
+    def delete_entity_by_guid(self, guid) -> AssetMutationResponse:
+        raw_json = self._call_api(
+            DELETE_ENTITY_BY_GUID.format_path_with_params(guid),
+            {"deleteType": AtlanDeleteType.SOFT.value},
+        )
+        return AssetMutationResponse(**raw_json)
+
     def search(self, criteria: IndexSearchRequest) -> SearchResults:
         raw_json = self._call_api(
             INDEX_SEARCH,
             request_obj=criteria,
         )
         if "entities" in raw_json:
             assets = parse_obj_as(list[Asset], raw_json["entities"])
@@ -415,15 +436,14 @@
         raw_json = self._call_api(
             GET_ALL_TYPE_DEFS.format_path_with_params(),
             query_params,
         )
         return TypeDefResponse(**raw_json)
 
     def create_typedef(self, typedef: TypeDef) -> TypeDefResponse:
-        payload = None
         if isinstance(typedef, ClassificationDef):
             # Set up the request payload...
             payload = TypeDefResponse(
                 classification_defs=[typedef],
                 enum_defs=[],
                 struct_defs=[],
                 entity_defs=[],
@@ -459,23 +479,23 @@
     def add_classifications(
         self,
         asset_type: Type[A],
         qualified_name: str,
         classification_names: list[str],
         propagate: bool = True,
         remove_propagation_on_delete: bool = True,
-        restrict_lineage_propogation: bool = True,
+        restrict_lineage_propagation: bool = True,
     ) -> None:
         classifications = Classifications(
             __root__=[
                 Classification(
                     type_name=ClassificationName(display_text=name),
                     propagate=propagate,
                     remove_propagations_on_entity_delete=remove_propagation_on_delete,
-                    restrict_propagation_through_lineage=restrict_lineage_propogation,
+                    restrict_propagation_through_lineage=restrict_lineage_propagation,
                 )
                 for name in classification_names
             ]
         )
         query_params = {"attr:qualifiedName": qualified_name}
         self._call_api(
             UPDATE_ENTITY_BY_ATTRIBUTE.format_path_with_params(
@@ -524,19 +544,17 @@
             PARTIAL_UPDATE_ENTITY_BY_ATTRIBUTE.format_path_with_params(
                 asset_type.__name__
             ),
             query_params,
             AssetRequest[Asset](entity=asset),
         )
         response = AssetMutationResponse(**raw_json)
-        assets = response.assets_partially_updated(asset_type=asset_type)
-        if assets:
+        if assets := response.assets_partially_updated(asset_type=asset_type):
             return assets[0]
-        assets = response.assets_updated(asset_type=asset_type)
-        if assets:
+        if assets := response.assets_updated(asset_type=asset_type):
             return assets[0]
         return None
 
     @validate_arguments()
     def remove_certificate(
         self, asset_type: Type[A], qualified_name: str, name: str
     ) -> Optional[A]:
```

### Comparing `pyatlan-0.0.20/pyatlan/client/constants.py` & `pyatlan-0.0.21/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/pyatlan/error.py` & `pyatlan-0.0.21/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/pyatlan/exceptions.py` & `pyatlan-0.0.21/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.0.21/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/pyatlan/model/assets.py` & `pyatlan-0.0.21/pyatlan/model/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,27 @@
     Histogram,
     KafkaTopicConsumption,
     PopularityInsights,
 )
 from pyatlan.utils import next_id
 
 
+def validate_single_required_field(field_names: list[str], values: list[Any]):
+    indexes = [idx for idx, value in enumerate(values) if value is not None]
+    if not indexes:
+        raise ValueError(
+            f"One of the following parameters are required: {', '.join(field_names)}"
+        )
+    if len(indexes) > 1:
+        names = [field_names[idx] for idx in indexes]
+        raise ValueError(
+            f"Only one of the following parameters are allowed: {', '.join(names)}"
+        )
+
+
 def validate_required_fields(field_names: list[str], values: list[Any]):
     for field_name, value in zip(field_names, values):
         if value is None:
             raise ValueError(f"{field_name} is required")
         if isinstance(value, str) and not value.strip():
             raise ValueError(f"{field_name} cannot be blank")
 
@@ -223,14 +236,16 @@
         None, description="", alias="customAttributes"
     )
     scrubbed: Optional[bool] = Field(
         None, description="", alias="fields removed from results"
     )
     pending_tasks: Optional[list[str]] = Field(None)
 
+    unique_attributes: Optional[dict[str, Any]] = Field(None)
+
     def validate_required(self):
         if not self.create_time or self.created_by:
             self.attributes.validate_required()
 
     def get_business_attributes(self, name: str) -> BusinessAttributes:
         from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
 
@@ -243,23 +258,24 @@
                 and a_type._meta_data_type_name == name
             ):
                 break
         else:
             raise ValueError(
                 f"Business attributes {name} are not applicable to {self.type_name}"
             )
-        ba_type = CustomMetadataCache.get_type_for_id(ba_id)
-        if not ba_type:
+        if ba_type := CustomMetadataCache.get_type_for_id(ba_id):
+            return (
+                ba_type(self.business_attributes[ba_id])
+                if self.business_attributes and ba_id in self.business_attributes
+                else ba_type()
+            )
+        else:
             raise ValueError(
                 f"Business attributes {name} are not applicable to {self.type_name}"
             )
-        if self.business_attributes and ba_id in self.business_attributes:
-            return ba_type(self.business_attributes[ba_id])
-        else:
-            return ba_type()
 
     def set_business_attribute(self, business_attributes: BusinessAttributes) -> None:
         from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
 
         if not isinstance(business_attributes, BusinessAttributes):
             raise ValueError(
                 "business_attributes must be an instance of BusinessAttributes"
@@ -1489,14 +1505,28 @@
         validate_required_fields(
             ["name", "qualified_name"],
             [name, qualified_name],
         )
         return cls(attributes=cls.Attributes(qualified_name=qualified_name, name=name))
 
     @classmethod
+    def ref_by_guid(cls: type[SelfAsset], guid: str) -> SelfAsset:
+        retval: SelfAsset = cls(attributes=cls.Attributes())
+        retval.guid = guid
+        return retval
+
+    @classmethod
+    def ref_by_qualified_name(cls: type[SelfAsset], qualified_name: str) -> SelfAsset:
+        ret_value: SelfAsset = cls(
+            attributes=cls.Attributes(qualified_name=qualified_name)
+        )
+        ret_value.unique_attributes = {"qualifiedName": qualified_name}
+        return ret_value
+
+    @classmethod
     def __get_validators__(cls):
         yield cls._convert_to_real_type_
 
     @classmethod
     def _convert_to_real_type_(cls, data):
 
         if isinstance(data, Asset):
@@ -1976,15 +2006,15 @@
         )  # relationship
         meanings: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="meanings"
         )  # relationship
 
         @classmethod
         # @validate_arguments()
-        def create(cls, name: StrictStr) -> AtlasGlossary.Attributes:
+        def create(cls, *, name: StrictStr) -> AtlasGlossary.Attributes:
             validate_required_fields(["name"], [name])
             return AtlasGlossary.Attributes(name=name, qualified_name=next_id())
 
     attributes: "AtlasGlossary.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
@@ -1998,17 +2028,17 @@
             and not values["attributes"].qualified_name
         ):
             values["attributes"].qualified_name = values["guid"]
         return values
 
     @classmethod
     # @validate_arguments()
-    def create(cls, name: StrictStr) -> AtlasGlossary:
+    def create(cls, *, name: StrictStr) -> AtlasGlossary:
         validate_required_fields(["name"], [name])
-        return AtlasGlossary(attributes=AtlasGlossary.Attributes.create(name))
+        return AtlasGlossary(attributes=AtlasGlossary.Attributes.create(name=name))
 
 
 class DataSet(Asset, type_name="DataSet"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in DataSet._convience_properties:
@@ -2204,19 +2234,32 @@
             None, description="", alias="preferredTerms"
         )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(
             cls,
+            *,
             name: StrictStr,
-            anchor: AtlasGlossary,
+            anchor: Optional[AtlasGlossary] = None,
+            glossary_qualified_name: Optional[StrictStr] = None,
+            glossary_guid: Optional[StrictStr] = None,
             categories: Optional[list[AtlasGlossaryCategory]] = None,
         ) -> AtlasGlossaryTerm.Attributes:
-            validate_required_fields(["name", "anchor"], [name, anchor])
+            validate_required_fields(["name"], [name])
+            validate_single_required_field(
+                ["anchor", "glossary_qualified_name", "glossary_guid"],
+                [anchor, glossary_qualified_name, glossary_guid],
+            )
+            if glossary_qualified_name:
+                anchor = AtlasGlossary()
+                anchor.unique_attributes = {"qualifiedName": glossary_qualified_name}
+            if glossary_guid:
+                anchor = AtlasGlossary()
+                anchor.guid = glossary_guid
             return AtlasGlossaryTerm.Attributes(
                 name=name,
                 anchor=anchor,
                 categories=categories,
                 qualified_name=next_id(),
             )
 
@@ -2236,22 +2279,29 @@
             values["attributes"].qualified_name = values["guid"]
         return values
 
     @classmethod
     # @validate_arguments()
     def create(
         cls,
+        *,
         name: StrictStr,
-        anchor: AtlasGlossary,
+        anchor: Optional[AtlasGlossary] = None,
+        glossary_qualified_name: Optional[StrictStr] = None,
+        glossary_guid: Optional[StrictStr] = None,
         categories: Optional[list[AtlasGlossaryCategory]] = None,
     ) -> AtlasGlossaryTerm:
-        validate_required_fields(["name", "anchor"], [name, anchor])
+        validate_required_fields(["name"], [name])
         return cls(
             attributes=AtlasGlossaryTerm.Attributes.create(
-                name=name, anchor=anchor, categories=categories
+                name=name,
+                anchor=anchor,
+                glossary_qualified_name=glossary_qualified_name,
+                glossary_guid=glossary_guid,
+                categories=categories,
             )
         )
 
     @classmethod
     def create_for_modification(
         cls: type[SelfAsset],
         qualified_name: str = "",
@@ -2642,14 +2692,15 @@
             if not self.connector_name:
                 raise ValueError("connector_name is required")
 
         @classmethod
         # @validate_arguments()
         def create(
             cls,
+            *,
             name: str,
             connector_type: AtlanConnectorType,
             admin_users: Optional[list[str]] = None,
             admin_groups: Optional[list[str]] = None,
             admin_roles: Optional[list[str]] = None,
         ) -> Connection.Attributes:
             if not name:
@@ -2676,14 +2727,15 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
     # @validate_arguments()
     def create(
         cls,
+        *,
         name: str,
         connector_type: AtlanConnectorType,
         admin_users: Optional[list[str]] = None,
         admin_groups: Optional[list[str]] = None,
         admin_roles: Optional[list[str]] = None,
     ) -> Connection:
         if not name:
@@ -2896,14 +2948,15 @@
             None, description="", alias="meanings"
         )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(
             cls,
+            *,
             name: StrictStr,
             anchor: AtlasGlossary,
             parent_category: Optional[AtlasGlossaryCategory] = None,
         ) -> AtlasGlossaryCategory.Attributes:
             validate_required_fields(["name", "anchor"], [name, anchor])
             return AtlasGlossaryCategory.Attributes(
                 name=name,
@@ -2928,14 +2981,15 @@
             values["attributes"].qualified_name = values["guid"]
         return values
 
     @classmethod
     # @validate_arguments()
     def create(
         cls,
+        *,
         name: StrictStr,
         anchor: AtlasGlossary,
         parent_category: Optional[AtlasGlossaryCategory] = None,
     ) -> AtlasGlossaryCategory:
         validate_required_fields(["name", "anchor"], [name, anchor])
         return cls(
             attributes=AtlasGlossaryCategory.Attributes.create(
@@ -9020,15 +9074,15 @@
         )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
 
         @classmethod
         # @validate_arguments()
-        def create(cls, name: str, schema_qualified_name: str) -> Table.Attributes:
+        def create(cls, *, name: str, schema_qualified_name: str) -> Table.Attributes:
             if not name:
                 raise ValueError("name cannot be blank")
             validate_required_fields(["schema_qualified_name"], [schema_qualified_name])
             fields = schema_qualified_name.split("/")
             if len(fields) != 5:
                 raise ValueError("Invalid schema_qualified_name")
             try:
@@ -9050,19 +9104,21 @@
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
     # @validate_arguments()
-    def create(cls, name: str, schema_qualified_name: str) -> Table:
+    def create(cls, *, name: str, schema_qualified_name: str) -> Table:
         validate_required_fields(
             ["name", "schema_qualified_name"], [name, schema_qualified_name]
         )
-        attributes = Table.Attributes.create(name, schema_qualified_name)
+        attributes = Table.Attributes.create(
+            name=name, schema_qualified_name=schema_qualified_name
+        )
         return cls(attributes=attributes)
 
 
 class Query(SQL):
     """Description"""
 
     def __setattr__(self, name, value):
@@ -10066,15 +10122,17 @@
         )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
 
         @classmethod
         # @validate_arguments()
-        def create(cls, name: str, database_qualified_name: str) -> Schema.Attributes:
+        def create(
+            cls, *, name: str, database_qualified_name: str
+        ) -> Schema.Attributes:
             if not name:
                 raise ValueError("name cannot be blank")
             validate_required_fields(
                 ["database_qualified_name"], [database_qualified_name]
             )
             fields = database_qualified_name.split("/")
             if len(fields) != 4:
@@ -10096,19 +10154,21 @@
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
     # @validate_arguments()
-    def create(cls, name: str, database_qualified_name: str) -> Schema:
+    def create(cls, *, name: str, database_qualified_name: str) -> Schema:
         validate_required_fields(
             ["name", "database_qualified_name"], [name, database_qualified_name]
         )
-        attributes = Schema.Attributes.create(name, database_qualified_name)
+        attributes = Schema.Attributes.create(
+            name=name, database_qualified_name=database_qualified_name
+        )
         return cls(attributes=attributes)
 
 
 class SnowflakeStream(SQL):
     """Description"""
 
     def __setattr__(self, name, value):
@@ -10444,15 +10504,15 @@
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
     # @validate_arguments()
-    def create(cls, name: str, connection_qualified_name: str) -> Database:
+    def create(cls, *, name: str, connection_qualified_name: str) -> Database:
         if not name:
             raise ValueError("name cannot be blank")
         validate_required_fields(
             ["connection_qualified_name"], [connection_qualified_name]
         )
         fields = connection_qualified_name.split("/")
         if len(fields) != 3:
@@ -10701,15 +10761,15 @@
         )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
 
         @classmethod
         # @validate_arguments()
-        def create(cls, name: str, schema_qualified_name: str) -> View.Attributes:
+        def create(cls, *, name: str, schema_qualified_name: str) -> View.Attributes:
             if not name:
                 raise ValueError("name cannot be blank")
             validate_required_fields(["schema_qualified_name"], [schema_qualified_name])
             fields = schema_qualified_name.split("/")
             if len(fields) != 5:
                 raise ValueError("Invalid schema_qualified_name")
             try:
@@ -10731,19 +10791,21 @@
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
     # @validate_arguments()
-    def create(cls, name: str, schema_qualified_name: str) -> View:
+    def create(cls, *, name: str, schema_qualified_name: str) -> View:
         validate_required_fields(
             ["name", "schema_qualified_name"], [name, schema_qualified_name]
         )
-        attributes = View.Attributes.create(name, schema_qualified_name)
+        attributes = View.Attributes.create(
+            name=name, schema_qualified_name=schema_qualified_name
+        )
         return cls(attributes=attributes)
 
 
 class MaterialisedView(SQL):
     """Description"""
 
     def __setattr__(self, name, value):
@@ -12106,15 +12168,15 @@
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(
-            cls, name: str, connection_qualified_name: str, aws_arn: str
+            cls, *, name: str, connection_qualified_name: str, aws_arn: str
         ) -> S3Bucket.Attributes:
             validate_required_fields(
                 ["name", "connection_qualified_name", "aws_arn"],
                 [name, connection_qualified_name, aws_arn],
             )
             fields = connection_qualified_name.split("/")
             if len(fields) != 3:
@@ -12140,22 +12202,24 @@
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
     # @validate_arguments()
     def create(
-        cls, name: str, connection_qualified_name: str, aws_arn: str
+        cls, *, name: str, connection_qualified_name: str, aws_arn: str
     ) -> S3Bucket:
         validate_required_fields(
             ["name", "connection_qualified_name", "aws_arn"],
             [name, connection_qualified_name, aws_arn],
         )
         attributes = S3Bucket.Attributes.create(
-            name, connection_qualified_name, aws_arn
+            name=name,
+            connection_qualified_name=connection_qualified_name,
+            aws_arn=aws_arn,
         )
         return cls(attributes=attributes)
 
 
 class S3Object(S3):
     """Description"""
 
@@ -12326,14 +12390,15 @@
             None, description="", alias="outputFromProcesses"
         )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(
             cls,
+            *,
             name: str,
             connection_qualified_name: str,
             aws_arn: str,
             s3_bucket_qualified_name: Optional[str] = None,
         ) -> S3Object.Attributes:
             validate_required_fields(
                 ["name", "connection_qualified_name", "aws_arn"],
@@ -12365,25 +12430,29 @@
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
     # @validate_arguments()
     def create(
         cls,
+        *,
         name: str,
         connection_qualified_name: str,
         aws_arn: str,
         s3_bucket_qualified_name: Optional[str] = None,
     ) -> S3Object:
         validate_required_fields(
             ["name", "connection_qualified_name", "aws_arn"],
             [name, connection_qualified_name, aws_arn],
         )
         attributes = S3Object.Attributes.create(
-            name, connection_qualified_name, aws_arn, s3_bucket_qualified_name
+            name=name,
+            connection_qualified_name=connection_qualified_name,
+            aws_arn=aws_arn,
+            s3_bucket_qualified_name=s3_bucket_qualified_name,
         )
         return cls(attributes=attributes)
 
 
 class KafkaTopic(Kafka):
     """Description"""
```

### Comparing `pyatlan-0.0.20/pyatlan/model/core.py` & `pyatlan-0.0.21/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/pyatlan/model/enums.py` & `pyatlan-0.0.21/pyatlan/model/enums.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/pyatlan/model/response.py` & `pyatlan-0.0.21/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/pyatlan/model/role.py` & `pyatlan-0.0.21/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/pyatlan/model/search.py` & `pyatlan-0.0.21/pyatlan/model/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1744,11 +1744,14 @@
         if not v and ("post_filter" not in values or not values["post_filter"]):
             raise ValueError("Either query or post_filter is required")
         return v
 
 
 class IndexSearchRequest(AtlanObject):
     dsl: DSL
-    attributes: list = Field(default_factory=list)
+    attributes: list[str] = Field(default_factory=list)
+    relation_attributes: list[str] = Field(
+        default_factory=list, alias="relationAttributes"
+    )
 
     class Config:
         json_encoders = {Query: lambda v: v.to_dict(), SortItem: lambda v: v.to_dict()}
```

### Comparing `pyatlan-0.0.20/pyatlan/model/structs.py` & `pyatlan-0.0.21/pyatlan/model/structs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,36 +25,36 @@
             None, description="", alias="awsCloudWatchMetricName"
         )
         aws_cloud_watch_metric_scope: str = Field(
             None, description="", alias="awsCloudWatchMetricScope"
         )
 
 
-class Histogram(AtlanObject):
-    """Description"""
-
-    class Attributes(AtlanObject):
-        boundaries: set[float] = Field(None, description="", alias="boundaries")
-        frequencies: set[float] = Field(None, description="", alias="frequencies")
-
-
 class KafkaTopicConsumption(AtlanObject):
     """Description"""
 
     class Attributes(AtlanObject):
         topic_name: Optional[str] = Field(None, description="", alias="topicName")
         topic_partition: Optional[str] = Field(
             None, description="", alias="topicPartition"
         )
         topic_lag: Optional[int] = Field(None, description="", alias="topicLag")
         topic_current_offset: Optional[int] = Field(
             None, description="", alias="topicCurrentOffset"
         )
 
 
+class Histogram(AtlanObject):
+    """Description"""
+
+    class Attributes(AtlanObject):
+        boundaries: set[float] = Field(None, description="", alias="boundaries")
+        frequencies: set[float] = Field(None, description="", alias="frequencies")
+
+
 class DbtMetricFilter(AtlanObject):
     """Description"""
 
     class Attributes(AtlanObject):
         dbt_metric_filter_column_qualified_name: Optional[str] = Field(
             None, description="", alias="dbtMetricFilterColumnQualifiedName"
         )
```

### Comparing `pyatlan-0.0.20/pyatlan/model/typedef.py` & `pyatlan-0.0.21/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/pyatlan/utils.py` & `pyatlan-0.0.21/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.0.21/pyatlan.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.20
+Version: 0.0.21
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.20/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.0.21/pyatlan.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,11 +40,12 @@
 tests/integration/custom_metadata_test.py
 tests/integration/role_test.py
 tests/integration/test_client.py
 tests/integration/test_entity_model.py
 tests/integration/test_index_search.py
 tests/unit/__init__.py
 tests/unit/test_classification_name.py
+tests/unit/test_glossary_term.py
 tests/unit/test_model.py
 tests/unit/test_search_model.py
 tests/unit/test_typedef_model.py
 tests/unit/test_utils.py
```

### Comparing `pyatlan-0.0.20/setup.py` & `pyatlan-0.0.21/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/tests/integration/classification_test.py` & `pyatlan-0.0.21/tests/integration/classification_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/tests/integration/custom_metadata_test.py` & `pyatlan-0.0.21/tests/integration/custom_metadata_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/tests/integration/role_test.py` & `pyatlan-0.0.21/tests/integration/role_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/tests/integration/test_entity_model.py` & `pyatlan-0.0.21/tests/integration/test_entity_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -252,15 +252,17 @@
     assert response.mutated_entities.DELETE
     assert len(response.mutated_entities.DELETE) == 1
     assert not response.mutated_entities.UPDATE
     assert not response.mutated_entities.CREATE
 
 
 def test_create_glossary(client: AtlanClient, increment_counter):
-    glossary = AtlasGlossary.create(f"Integration Test Glossary {increment_counter()}")
+    glossary = AtlasGlossary.create(
+        name=f"Integration Test Glossary {increment_counter()}"
+    )
     response = client.upsert(glossary)
     assert response.mutated_entities
     assert not response.mutated_entities.UPDATE
     assert response.mutated_entities.CREATE
     assert len(response.mutated_entities.CREATE) == 1
     guid = list(response.guid_assignments.values())[0]
     assert response.mutated_entities.CREATE
@@ -318,23 +320,23 @@
     assert len(response.mutated_entities.CREATE) == count
     for glossary in response.assets_created(AtlasGlossary):
         assert glossary.guid in response.guid_assignments.values()
 
 
 def test_create_glossary_category(client: AtlanClient, increment_counter):
     suffix = increment_counter()
-    glossary = AtlasGlossary.create(f"Integration Test Glossary {suffix}")
+    glossary = AtlasGlossary.create(name=f"Integration Test Glossary {suffix}")
     glossary.attributes.user_description = "This a test glossary"
     response = client.upsert(glossary)
     assert response.mutated_entities
     assert response.mutated_entities.CREATE
     assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossary)
     glossary = response.mutated_entities.CREATE[0]
     category = AtlasGlossaryCategory.create(
-        f"Integration Test Glossary Category {suffix}", anchor=glossary
+        name=f"Integration Test Glossary Category {suffix}", anchor=glossary
     )
     category.attributes.user_description = "This is a test glossary category"
     response = client.upsert(category)
     assert response.mutated_entities
     assert response.mutated_entities.UPDATE
     assert len(response.mutated_entities.UPDATE) == 1
     assert isinstance(response.mutated_entities.UPDATE[0], AtlasGlossary)
@@ -348,22 +350,22 @@
     category = client.get_asset_by_guid(guid, AtlasGlossaryCategory)
     assert isinstance(category, AtlasGlossaryCategory)
     assert category.guid == guid
 
 
 def test_create_glossary_term(client: AtlanClient, increment_counter):
     suffix = increment_counter()
-    glossary = AtlasGlossary.create(f"Integration Test Glossary {suffix}")
+    glossary = AtlasGlossary.create(name=f"Integration Test Glossary {suffix}")
     response = client.upsert(glossary)
     assert response.mutated_entities
     assert response.mutated_entities.CREATE
     assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossary)
     glossary = response.mutated_entities.CREATE[0]
     term = AtlasGlossaryTerm.create(
-        f"Integration Test Glossary Term {suffix}", anchor=glossary
+        name=f"Integration Test Glossary Term {suffix}", anchor=glossary
     )
     response = client.upsert(term)
     assert response.mutated_entities
     assert response.mutated_entities.UPDATE
     assert response.mutated_entities.UPDATE
     assert len(response.mutated_entities.UPDATE) == 1
     assert isinstance(response.mutated_entities.UPDATE[0], AtlasGlossary)
@@ -383,14 +385,75 @@
         glossary_guid=glossary.guid,
     )
     term.user_description = "This is an important term"
     response = client.upsert(term)
     assert 1 == len(response.assets_updated(AtlasGlossaryTerm))
 
 
+def test_create_glossary_term_with_glossary_guid(
+    client: AtlanClient, increment_counter
+):
+    suffix = increment_counter()
+    glossary = AtlasGlossary.create(name=f"Integration Test Glossary {suffix}")
+    response = client.upsert(glossary)
+    assert response.mutated_entities
+    assert response.mutated_entities.CREATE
+    assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossary)
+    glossary = response.mutated_entities.CREATE[0]
+    term = AtlasGlossaryTerm.create(
+        name=f"Integration Test Glossary Term {suffix}", glossary_guid=glossary.guid
+    )
+    response = client.upsert(term)
+    assert response.mutated_entities
+    assert response.mutated_entities.UPDATE
+    assert response.mutated_entities.UPDATE
+    assert len(response.mutated_entities.UPDATE) == 1
+    assert isinstance(response.mutated_entities.UPDATE[0], AtlasGlossary)
+    assert response.mutated_entities.CREATE
+    assert len(response.mutated_entities.CREATE) == 1
+    guid = list(response.guid_assignments.values())[0]
+    assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossaryTerm)
+    term = response.mutated_entities.CREATE[0]
+    assert guid == term.guid
+    term = client.get_asset_by_guid(guid, AtlasGlossaryTerm)
+    assert isinstance(term, AtlasGlossaryTerm)
+    assert term.guid == guid
+
+
+def test_create_glossary_term_with_glossary_qualified_name(
+    client: AtlanClient, increment_counter
+):
+    suffix = increment_counter()
+    glossary = AtlasGlossary.create(name=f"Integration Test Glossary {suffix}")
+    response = client.upsert(glossary)
+    assert response.mutated_entities
+    assert response.mutated_entities.CREATE
+    assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossary)
+    glossary = response.mutated_entities.CREATE[0]
+    term = AtlasGlossaryTerm.create(
+        name=f"Integration Test Glossary Term {suffix}",
+        glossary_qualified_name=glossary.qualified_name,
+    )
+    response = client.upsert(term)
+    assert response.mutated_entities
+    assert response.mutated_entities.UPDATE
+    assert response.mutated_entities.UPDATE
+    assert len(response.mutated_entities.UPDATE) == 1
+    assert isinstance(response.mutated_entities.UPDATE[0], AtlasGlossary)
+    assert response.mutated_entities.CREATE
+    assert len(response.mutated_entities.CREATE) == 1
+    guid = list(response.guid_assignments.values())[0]
+    assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossaryTerm)
+    term = response.mutated_entities.CREATE[0]
+    assert guid == term.guid
+    term = client.get_asset_by_guid(guid, AtlasGlossaryTerm)
+    assert isinstance(term, AtlasGlossaryTerm)
+    assert term.guid == guid
+
+
 def test_create_hierarchy(client: AtlanClient, increment_counter):
     suffix = increment_counter()
     glossary = AtlasGlossary(
         attributes=AtlasGlossary.Attributes(
             name=f"Integration Test Glossary {suffix}",
             user_description="This a test glossary",
         )
@@ -612,15 +675,15 @@
     )
     assert column.attributes.qualified_name == qualified_name
 
 
 @pytest.mark.skip("Connection creation is still intermittently failing")
 def test_create_view(client: AtlanClient, increment_counter):
     view = View.create(
-        f"Integration {increment_counter()}",
+        name=f"Integration {increment_counter()}",
         schema_qualified_name="default/snowflake/1658945299/ATLAN_SAMPLE_DATA/US_ECONOMIC_DATA",
     )
     response = client.upsert(view)
     assert response.mutated_entities
     assert response.mutated_entities.CREATE
     assert len(response.mutated_entities.CREATE) == 1
     assert isinstance(response.mutated_entities.CREATE[0], View)
@@ -628,19 +691,19 @@
     assert view.guid in response.guid_assignments
     guid = response.guid_assignments[view.guid]
     view = response.mutated_entities.CREATE[0]
     assert guid == view.guid
 
 
 def test_add_and_remove_classifications(client: AtlanClient):
-    glossary = AtlasGlossary.create("Integration Classification Test")
+    glossary = AtlasGlossary.create(name="Integration Classification Test")
     glossary.attributes.user_description = "This is a description of the glossary"
     glossary = client.upsert(glossary).assets_created(AtlasGlossary)[0]
     glossary_term = AtlasGlossaryTerm.create(
-        "Integration Classification Term", anchor=glossary
+        name="Integration Classification Term", anchor=glossary
     )
     glossary_term = client.upsert(glossary_term).assets_created(AtlasGlossaryTerm)[0]
     qualified_name = glossary_term.attributes.qualified_name
     classification_name = "TEST"
     client.add_classifications(AtlasGlossaryTerm, qualified_name, [classification_name])
     glossary_term = client.get_asset_by_guid(
         glossary_term.guid, asset_type=AtlasGlossaryTerm
@@ -662,21 +725,22 @@
     )
     classification_name = "TEST"
     client.add_classifications(Table, qualified_name, [classification_name])
     table = Table.create_for_modification(
         qualified_name=qualified_name, name="CONTRACT_STATUS"
     )
     response = client.upsert(table, replace_classifications=True)
-    tables = response.assets_updated(asset_type=Table)
+    assert (tables := response.assets_updated(asset_type=Table))
     assert 1 == len(tables)
+    assert tables[0].classifications is not None
     assert 0 == len(tables[0].classifications)
 
 
 def test_update_remove_certificate(client: AtlanClient):
-    glossary = AtlasGlossary.create("Integration Certificate Test")
+    glossary = AtlasGlossary.create(name="Integration Certificate Test")
     glossary.attributes.user_description = "This is a description of the glossary"
     glossary = client.upsert(glossary).assets_created(AtlasGlossary)[0]
     message = "An important message"
     asset = client.update_certificate(
         asset_type=AtlasGlossary,
         qualified_name=glossary.qualified_name,
         name=glossary.name,
@@ -693,15 +757,15 @@
     )
     assert asset is not None
     assert asset.certificate_status is None
     assert asset.certificate_status_message is None
 
 
 def test_update_remove_announcement(client: AtlanClient, announcement: Announcement):
-    glossary = AtlasGlossary.create("Integration Announcement Test")
+    glossary = AtlasGlossary.create(name="Integration Announcement Test")
     glossary.attributes.user_description = "This is a description of the glossary"
     glossary = client.upsert(glossary).assets_created(AtlasGlossary)[0]
     asset = client.update_announcement(
         asset_type=AtlasGlossary,
         qualified_name=glossary.qualified_name,
         name=glossary.name,
         announcement=announcement,
```

### Comparing `pyatlan-0.0.20/tests/integration/test_index_search.py` & `pyatlan-0.0.21/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/tests/unit/test_classification_name.py` & `pyatlan-0.0.21/tests/unit/test_classification_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.20/tests/unit/test_model.py` & `pyatlan-0.0.21/tests/unit/test_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     Histogram,
     PopularityInsights,
     S3Bucket,
     S3Object,
     Schema,
     Table,
     View,
+    validate_single_required_field,
 )
 from pyatlan.model.core import Announcement, AssetResponse
 from pyatlan.model.enums import (
     ADLSAccessTier,
     ADLSLeaseState,
     ADLSLeaseStatus,
     ADLSObjectArchiveStatus,
@@ -162,15 +163,16 @@
         announcement_type=AnnouncementType.ISSUE,
     )
 
 
 @pytest.fixture()
 def table():
     return Table.create(
-        "MKT_EXPENSES", "efault/snowflake/1646836521/ATLAN_SAMPLE_DATA/FOOD_BEVERAGE"
+        name="MKT_EXPENSES",
+        schema_qualified_name="default/snowflake/1646836521/ATLAN_SAMPLE_DATA/FOOD_BEVERAGE",
     )
 
 
 @pytest.fixture()
 def type_def_response():
     data = {
         "enumDefs": [],
@@ -978,49 +980,51 @@
 
 def test_glossary_attributes_create_when_missing_name_raises_validation_error():
     with pytest.raises(ValueError):
         AtlasGlossary.Attributes.create(name=None)
 
 
 def test_glossary_attributes_create_sets_name():
-    sut = AtlasGlossary.Attributes.create("Bob")
+    sut = AtlasGlossary.Attributes.create(name="Bob")
     assert sut.name == "Bob"
 
 
 @pytest.mark.parametrize(
-    "name, anchor", [("A Category", None), (None, AtlasGlossary.create("glossary"))]
+    "name, anchor",
+    [("A Category", None), (None, AtlasGlossary.create(name="glossary"))],
 )
 def test_glossary_category_attributes_create_when_missing_name_raises_validation_error(
     name, anchor
 ):
     with pytest.raises(ValueError):
         AtlasGlossaryCategory.Attributes.create(name=name, anchor=anchor)
 
 
 def test_glossary_category_attributes_create_sets_name_anchor():
-    glossary = AtlasGlossary.create("Glossary")
-    sut = AtlasGlossaryCategory.Attributes.create("Bob", anchor=glossary)
+    glossary = AtlasGlossary.create(name="Glossary")
+    sut = AtlasGlossaryCategory.Attributes.create(name="Bob", anchor=glossary)
     assert sut.name == "Bob"
     assert sut.anchor == glossary
 
 
 @pytest.mark.parametrize(
-    "name, anchor", [("A Category", None), (None, AtlasGlossary.create("glossary"))]
+    "name, anchor",
+    [("A Category", None), (None, AtlasGlossary.create(name="glossary"))],
 )
 def test_glossary_term_attributes_create_when_missing_name_raises_validation_error(
     name, anchor
 ):
     with pytest.raises(ValueError):
         a = AtlasGlossaryTerm.Attributes.create(name=name, anchor=anchor)
         a.validate_required()
 
 
 def test_glossary_term_attributes_create_sets_name_anchor():
-    glossary = AtlasGlossary.create("Glossary")
-    sut = AtlasGlossaryTerm.Attributes.create("Bob", anchor=glossary)
+    glossary = AtlasGlossary.create(name="Glossary")
+    sut = AtlasGlossaryTerm.Attributes.create(name="Bob", anchor=glossary)
     assert sut.name == "Bob"
     assert sut.anchor == glossary
 
 
 @patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
 def test_get_business_attributes_when_name_not_valid_raises_value_error(
     mock_client, table, type_def_response
@@ -1313,7 +1317,38 @@
     assert attribute_value == local_ns["ret_value"]
     exec(
         f"ret_value = sut.attributes.{property_name}",
         {"sut": sut, "property_name": property_name},
         local_ns,
     )
     assert attribute_value == local_ns["ret_value"]
+
+
+@pytest.mark.parametrize(
+    "names, values, message",
+    [
+        (
+            ("one", "two"),
+            (None, None),
+            "One of the following parameters are required: one, two",
+        ),
+        (
+            ("one", "two"),
+            (1, 2),
+            "Only one of the following parameters are allowed: one, two",
+        ),
+        (
+            ("one", "two", "three"),
+            (1, None, 3),
+            "Only one of the following parameters are allowed: one, three",
+        ),
+    ],
+)
+def test_validate_single_required_field_with_bad_values_raises_value_error(
+    names, values, message
+):
+    with pytest.raises(ValueError, match=message):
+        validate_single_required_field(names, values)
+
+
+def test_validate_single_required_field_with_only_one_field_does_not_raise_value_error():
+    validate_single_required_field(["One", "Two", "Three"], [None, None, 3])
```

### Comparing `pyatlan-0.0.20/tests/unit/test_search_model.py` & `pyatlan-0.0.21/tests/unit/test_search_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
     )
     request = IndexSearchRequest(dsl=dsl, attributes=["schemaName", "databaseName"])
     assert (
         request.json(by_alias=True, exclude_none=True)
         == '{"dsl": {"from": 0, "size": 100, "track_total_hits": true, '
         '"post_filter": {"term": {"databaseName.keyword": '
         '{"value": "ATLAN_SAMPLE_DATA"}}}, "query": {"term": {"__typeName.keyword": {"value": "Schema"}}}}, '
-        '"attributes": ["schemaName", "databaseName"]}'
+        '"attributes": ["schemaName", "databaseName"], "relationAttributes": []}'
     )
 
 
 def test_adding_terms_results_in_must_bool():
     term_1 = Term(field="name", value="Bob")
     term_2 = Term(field="name", value="Dave")
     result = term_1 + term_2
```

### Comparing `pyatlan-0.0.20/tests/unit/test_typedef_model.py` & `pyatlan-0.0.21/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

