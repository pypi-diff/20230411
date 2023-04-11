# Comparing `tmp/nornir_napalm-0.3.0.tar.gz` & `tmp/nornir_napalm-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_napalm-0.3.0.tar", max compression
+gzip compressed data, was "nornir_napalm-0.4.0.tar", max compression
```

## Comparing `nornir_napalm-0.3.0.tar` & `nornir_napalm-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0    11343 2021-02-27 09:12:47.109607 nornir_napalm-0.3.0/LICENSE
--rw-r--r--   0        0        0        0 2021-02-27 09:12:47.162613 nornir_napalm-0.3.0/nornir_napalm/__init__.py
--rw-r--r--   0        0        0        0 2021-02-27 09:12:47.162659 nornir_napalm-0.3.0/nornir_napalm/plugins/__init__.py
--rw-r--r--   0        0        0     1639 2021-02-27 09:12:47.162746 nornir_napalm-0.3.0/nornir_napalm/plugins/connections/__init__.py
--rw-r--r--   0        0        0      317 2021-02-27 09:12:47.162819 nornir_napalm-0.3.0/nornir_napalm/plugins/tasks/__init__.py
--rw-r--r--   0        0        0      596 2021-02-27 09:12:47.162881 nornir_napalm-0.3.0/nornir_napalm/plugins/tasks/napalm_cli.py
--rw-r--r--   0        0        0     1511 2022-03-29 12:31:12.351450 nornir_napalm-0.3.0/nornir_napalm/plugins/tasks/napalm_configure.py
--rw-r--r--   0        0        0     1427 2021-02-27 09:12:47.162975 nornir_napalm-0.3.0/nornir_napalm/plugins/tasks/napalm_get.py
--rw-r--r--   0        0        0     1433 2021-02-27 09:12:47.163026 nornir_napalm-0.3.0/nornir_napalm/plugins/tasks/napalm_ping.py
--rw-r--r--   0        0        0     1040 2021-02-27 09:12:47.163076 nornir_napalm-0.3.0/nornir_napalm/plugins/tasks/napalm_validate.py
--rw-r--r--   0        0        0      785 2022-07-14 06:33:52.026507 nornir_napalm-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      904 2022-07-14 06:35:40.517317 nornir_napalm-0.3.0/setup.py
--rw-r--r--   0        0        0      576 2022-07-14 06:35:40.517469 nornir_napalm-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-07-12 22:03:27.501240 nornir_napalm-0.4.0/LICENSE
+-rw-r--r--   0        0        0        0 2022-07-12 22:03:27.565240 nornir_napalm-0.4.0/nornir_napalm/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-12 22:03:27.565240 nornir_napalm-0.4.0/nornir_napalm/plugins/__init__.py
+-rw-r--r--   0        0        0     1639 2023-02-09 01:20:54.828948 nornir_napalm-0.4.0/nornir_napalm/plugins/connections/__init__.py
+-rw-r--r--   0        0        0      470 2023-03-28 17:39:55.345838 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/__init__.py
+-rw-r--r--   0        0        0      596 2022-07-12 22:03:27.565240 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_cli.py
+-rw-r--r--   0        0        0     1767 2023-03-28 17:39:55.349838 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_configure.py
+-rw-r--r--   0        0        0      995 2023-03-28 17:39:55.349838 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_confirm_commit.py
+-rw-r--r--   0        0        0     1427 2022-07-12 22:03:27.565240 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_get.py
+-rw-r--r--   0        0        0     1433 2022-07-12 22:03:27.565240 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_ping.py
+-rw-r--r--   0        0        0      674 2023-03-28 17:39:55.349838 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_rollback.py
+-rw-r--r--   0        0        0     1040 2022-07-12 22:03:27.565240 nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_validate.py
+-rw-r--r--   0        0        0      801 2023-03-28 17:39:55.353838 nornir_napalm-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 nornir_napalm-0.4.0/setup.py
+-rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 nornir_napalm-0.4.0/PKG-INFO
```

### Comparing `nornir_napalm-0.3.0/LICENSE` & `nornir_napalm-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nornir_napalm-0.3.0/nornir_napalm/plugins/connections/__init__.py` & `nornir_napalm-0.4.0/nornir_napalm/plugins/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_napalm-0.3.0/nornir_napalm/plugins/tasks/napalm_cli.py` & `nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_cli.py`

 * *Files identical despite different names*

### Comparing `nornir_napalm-0.3.0/nornir_napalm/plugins/tasks/napalm_configure.py` & `nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_configure.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from typing import Optional
+from typing import Optional, Dict, Any
 
 from nornir.core.task import Result, Task
-
 from nornir_napalm.plugins.connections import CONNECTION_NAME
 
 
 def napalm_configure(
     task: Task,
     dry_run: Optional[bool] = None,
     filename: Optional[str] = None,
     configuration: Optional[str] = None,
     replace: bool = False,
-    commit_message: str = None,
+    commit_message: Optional[str] = None,
+    revert_in: Optional[int] = None,
 ) -> Result:
     """
     Loads configuration into a network devices using napalm
 
     Arguments:
         dry_run: Whether to apply changes or not
         filename: filename containing the configuration to load into the device
         configuration: configuration to load into the device
         replace: whether to replace or merge the configuration
+        revert_in: amount of time in seconds after which to revert the commit, None to disable
 
     Returns:
         Result object with the following attributes set:
           * changed (``bool``): whether the task is changing the system or not
           * diff (``string``): change in the system
     """
     device = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
@@ -32,15 +33,19 @@
     if replace:
         device.load_replace_candidate(filename=filename, config=configuration)
     else:
         device.load_merge_candidate(filename=filename, config=configuration)
     diff = device.compare_config()
 
     dry_run = task.is_dry_run(dry_run)
+
+    commit_kwargs: Dict[str, Any] = {}
+    if commit_message:
+        commit_kwargs["message"] = commit_message
+    if revert_in is not None:
+        commit_kwargs["revert_in"] = revert_in
+
     if not dry_run and diff:
-        if commit_message:
-            device.commit_config(message=commit_message)
-        else:
-            device.commit_config()
+        device.commit_config(**commit_kwargs)
     else:
         device.discard_config()
     return Result(host=task.host, diff=diff, changed=len(diff) > 0)
```

### Comparing `nornir_napalm-0.3.0/nornir_napalm/plugins/tasks/napalm_get.py` & `nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_get.py`

 * *Files identical despite different names*

### Comparing `nornir_napalm-0.3.0/nornir_napalm/plugins/tasks/napalm_ping.py` & `nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_ping.py`

 * *Files identical despite different names*

### Comparing `nornir_napalm-0.3.0/nornir_napalm/plugins/tasks/napalm_validate.py` & `nornir_napalm-0.4.0/nornir_napalm/plugins/tasks/napalm_validate.py`

 * *Files identical despite different names*

### Comparing `nornir_napalm-0.3.0/pyproject.toml` & `nornir_napalm-0.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [tool.poetry]
 name = "nornir_napalm"
-version = "0.3.0"
+version = "0.4.0"
 description = "NAPALM's plugins for nornir"
 authors = ["David Barroso <dbarrosop@dravetech.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.plugins."nornir.plugins.connections"]
 "napalm" = "nornir_napalm.plugins.connections:Napalm"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 napalm = "^4"
 nornir = { version = "~3", allow-prereleases = true }
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
-mypy = "*"
-pylama = "*"
-pytest = "*"
+mypy = "1.0.0"
+pylama = "8.4.1"
+pytest = "7.2.1"
 nbval = "*"
 jupyter = "^1"
 sphinx = "^4"
 sphinxcontrib-napoleon = "^0.7"
 nbsphinx = "^0.8"
 sphinx-issues = "^3.0"
 sphinx_rtd_theme = "^1.0"
 nornir_utils = { version = "*", allow-prereleases = true }
-pytest-cov = "*"
-
+pytest-cov = "4.0.0"
 
 [build-system]
-requires = ["poetry>=0.12"]
+requires = ["poetry>=1.3.2"]
 build-backend = "poetry.masonry.api"
```

### Comparing `nornir_napalm-0.3.0/setup.py` & `nornir_napalm-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 
 entry_points = \
 {'nornir.plugins.connections': ['napalm = '
                                 'nornir_napalm.plugins.connections:Napalm']}
 
 setup_kwargs = {
     'name': 'nornir-napalm',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': "NAPALM's plugins for nornir",
-    'long_description': None,
+    'long_description': 'None',
     'author': 'David Barroso',
     'author_email': 'dbarrosop@dravetech.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `nornir_napalm-0.3.0/PKG-INFO` & `nornir_napalm-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: nornir-napalm
-Version: 0.3.0
+Version: 0.4.0
 Summary: NAPALM's plugins for nornir
 License: Apache-2.0
 Author: David Barroso
 Author-email: dbarrosop@dravetech.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: napalm (>=4,<5)
 Requires-Dist: nornir (>=3,<4)
```

