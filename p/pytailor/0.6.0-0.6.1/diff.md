# Comparing `tmp/pytailor-0.6.0.tar.gz` & `tmp/pytailor-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytailor-0.6.0.tar", max compression
+gzip compressed data, was "pytailor-0.6.1.tar", max compression
```

## Comparing `pytailor-0.6.0.tar` & `pytailor-0.6.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1517 2023-03-29 19:41:08.700873 pytailor-0.6.0/LICENSE
--rw-r--r--   0        0        0      873 2023-03-29 19:41:08.712874 pytailor-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       68 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/__init__.py
--rw-r--r--   0        0        0      314 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/__init__.py
--rw-r--r--   0        0        0     1000 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/account.py
--rw-r--r--   0        0        0      104 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/base.py
--rw-r--r--   0        0        0    22572 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/dag.py
--rw-r--r--   0        0        0     2622 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/fileset.py
--rw-r--r--   0        0        0      844 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/local_files.py
--rw-r--r--   0        0        0     4260 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/parameterization.py
--rw-r--r--   0        0        0     3182 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/project.py
--rw-r--r--   0        0        0      173 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/schema/__init__.py
--rw-r--r--   0        0        0     5744 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/schema/description.py
--rw-r--r--   0        0        0     6199 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/schema/files_schema.py
--rw-r--r--   0        0        0     6976 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/schema/inputs_schema.py
--rw-r--r--   0        0        0        0 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/schema/strategies/__init__.py
--rw-r--r--   0        0        0     1080 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/schema/strategies/additionalProperties.py
--rw-r--r--   0        0        0      427 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/schema/strategies/tailorschemabuilder.py
--rw-r--r--   0        0        0    10825 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/workflow.py
--rw-r--r--   0        0        0     5221 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/api/workflow_definition.py
--rw-r--r--   0        0        0        0 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/cli/__init__.py
--rw-r--r--   0        0        0     3585 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/cli/main.py
--rw-r--r--   0        0        0      119 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/clients/__init__.py
--rw-r--r--   0        0        0     4141 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/clients/async_rest_client.py
--rw-r--r--   0        0        0     4303 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/clients/auth.py
--rw-r--r--   0        0        0     1439 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/clients/file_client.py
--rw-r--r--   0        0        0     3812 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/clients/handling.py
--rw-r--r--   0        0        0    10560 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/clients/rest_client.py
--rw-r--r--   0        0        0     1971 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/config.py
--rw-r--r--   0        0        0      371 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/exceptions.py
--rw-r--r--   0        0        0       74 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/execution/__init__.py
--rw-r--r--   0        0        0     1398 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/execution/serialrunner.py
--rw-r--r--   0        0        0    18170 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/execution/taskrunner.py
--rw-r--r--   0        0        0     3631 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/execution/worker.py
--rw-r--r--   0        0        0     3503 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/execution/worker_checks.py
--rw-r--r--   0        0        0    19407 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/models.py
--rw-r--r--   0        0        0     7721 2023-03-29 19:41:08.712874 pytailor-0.6.0/src/pytailor/utils.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 pytailor-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-04-11 12:43:15.550480 pytailor-0.6.1/LICENSE
+-rw-r--r--   0        0        0      873 2023-04-11 12:43:15.558480 pytailor-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/__init__.py
+-rw-r--r--   0        0        0      314 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/__init__.py
+-rw-r--r--   0        0        0     1000 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/account.py
+-rw-r--r--   0        0        0      104 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/base.py
+-rw-r--r--   0        0        0    22572 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/dag.py
+-rw-r--r--   0        0        0     2622 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/fileset.py
+-rw-r--r--   0        0        0      844 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/local_files.py
+-rw-r--r--   0        0        0     4260 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/parameterization.py
+-rw-r--r--   0        0        0     3182 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/project.py
+-rw-r--r--   0        0        0      173 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/schema/__init__.py
+-rw-r--r--   0        0        0     5744 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/schema/description.py
+-rw-r--r--   0        0        0     6199 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/schema/files_schema.py
+-rw-r--r--   0        0        0     6976 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/schema/inputs_schema.py
+-rw-r--r--   0        0        0        0 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/schema/strategies/__init__.py
+-rw-r--r--   0        0        0     1080 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/schema/strategies/additionalProperties.py
+-rw-r--r--   0        0        0      427 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/schema/strategies/tailorschemabuilder.py
+-rw-r--r--   0        0        0    10825 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/workflow.py
+-rw-r--r--   0        0        0     5221 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/api/workflow_definition.py
+-rw-r--r--   0        0        0        0 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/cli/__init__.py
+-rw-r--r--   0        0        0     3585 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/cli/main.py
+-rw-r--r--   0        0        0      119 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/clients/__init__.py
+-rw-r--r--   0        0        0     4141 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/clients/async_rest_client.py
+-rw-r--r--   0        0        0     4303 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/clients/auth.py
+-rw-r--r--   0        0        0     1439 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/clients/file_client.py
+-rw-r--r--   0        0        0     3812 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/clients/handling.py
+-rw-r--r--   0        0        0    10560 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/clients/rest_client.py
+-rw-r--r--   0        0        0     1971 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/config.py
+-rw-r--r--   0        0        0      371 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/exceptions.py
+-rw-r--r--   0        0        0       74 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/execution/__init__.py
+-rw-r--r--   0        0        0     1398 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/execution/serialrunner.py
+-rw-r--r--   0        0        0    18170 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/execution/taskrunner.py
+-rw-r--r--   0        0        0     3631 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/execution/worker.py
+-rw-r--r--   0        0        0     3503 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/execution/worker_checks.py
+-rw-r--r--   0        0        0    19407 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/models.py
+-rw-r--r--   0        0        0     7873 2023-04-11 12:43:15.558480 pytailor-0.6.1/src/pytailor/utils.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 pytailor-0.6.1/PKG-INFO
```

### Comparing `pytailor-0.6.0/LICENSE` & `pytailor-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/pyproject.toml` & `pytailor-0.6.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytailor"
-version = "0.6.0"
+version = "0.6.1"
 description = "pyTailor orchestrates your existing python code as *workflows*"
 authors = ["Audun Gravdal Johansen <audun@entail.no>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/entailor/pytailor/"
 include = [
     "LICENSE",
 ]
```

### Comparing `pytailor-0.6.0/src/pytailor/api/account.py` & `pytailor-0.6.1/src/pytailor/api/account.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/api/dag.py` & `pytailor-0.6.1/src/pytailor/api/dag.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/api/fileset.py` & `pytailor-0.6.1/src/pytailor/api/fileset.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/api/local_files.py` & `pytailor-0.6.1/src/pytailor/api/local_files.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/api/parameterization.py` & `pytailor-0.6.1/src/pytailor/api/parameterization.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/api/project.py` & `pytailor-0.6.1/src/pytailor/api/project.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/api/schema/description.py` & `pytailor-0.6.1/src/pytailor/api/schema/description.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/api/schema/files_schema.py` & `pytailor-0.6.1/src/pytailor/api/schema/files_schema.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/api/schema/inputs_schema.py` & `pytailor-0.6.1/src/pytailor/api/schema/inputs_schema.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/api/schema/strategies/additionalProperties.py` & `pytailor-0.6.1/src/pytailor/api/schema/strategies/additionalProperties.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/api/workflow.py` & `pytailor-0.6.1/src/pytailor/api/workflow.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/api/workflow_definition.py` & `pytailor-0.6.1/src/pytailor/api/workflow_definition.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/cli/main.py` & `pytailor-0.6.1/src/pytailor/cli/main.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/clients/async_rest_client.py` & `pytailor-0.6.1/src/pytailor/clients/async_rest_client.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/clients/auth.py` & `pytailor-0.6.1/src/pytailor/clients/auth.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/clients/file_client.py` & `pytailor-0.6.1/src/pytailor/clients/file_client.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/clients/handling.py` & `pytailor-0.6.1/src/pytailor/clients/handling.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/clients/rest_client.py` & `pytailor-0.6.1/src/pytailor/clients/rest_client.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/config.py` & `pytailor-0.6.1/src/pytailor/config.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/execution/serialrunner.py` & `pytailor-0.6.1/src/pytailor/execution/serialrunner.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/execution/taskrunner.py` & `pytailor-0.6.1/src/pytailor/execution/taskrunner.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/execution/worker.py` & `pytailor-0.6.1/src/pytailor/execution/worker.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/execution/worker_checks.py` & `pytailor-0.6.1/src/pytailor/execution/worker_checks.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/models.py` & `pytailor-0.6.1/src/pytailor/models.py`

 * *Files identical despite different names*

### Comparing `pytailor-0.6.0/src/pytailor/utils.py` & `pytailor-0.6.1/src/pytailor/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,18 @@
 
                 if val_cond and val_cond(v):
                     if key_apply_on == "val_cond":
                         new_key = key_apply(k)
                     if val_apply_on == "val_cond":
                         new_val = val_apply(v)
 
+                    if recurse_into_new_val:
+                        while val_cond(new_val):
+                            new_val = val_apply(new_val)
+
                 # update d_out
                 if not new_val is v:
                     if not new_key is k:
                         update_dict_key(d_out, k, new_key, new_val)
                     else:
                         d_out[k] = new_val
                 elif not new_key is k:
```

### Comparing `pytailor-0.6.0/PKG-INFO` & `pytailor-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytailor
-Version: 0.6.0
+Version: 0.6.1
 Summary: pyTailor orchestrates your existing python code as *workflows*
 Home-page: https://github.com/entailor/pytailor/
 License: BSD-3-Clause
 Author: Audun Gravdal Johansen
 Author-email: audun@entail.no
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

