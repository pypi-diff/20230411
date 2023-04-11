# Comparing `tmp/arthub_api-1.5.0.tar.gz` & `tmp/arthub_api-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_api-1.5.0.tar", last modified: Thu Mar 30 13:20:20 2023, max compression
+gzip compressed data, was "dist/arthub_api-1.5.1.tar", last modified: Tue Apr 11 14:21:34 2023, max compression
```

## Comparing `arthub_api-1.5.0.tar` & `arthub_api-1.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 13:20:20.511952 arthub_api-1.5.0/
--rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.5.0/LICENSE
--rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1217 2023-03-30 13:20:20.511952 arthub_api-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      676 2023-03-13 08:21:18.000000 arthub_api-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 13:20:20.496992 arthub_api-1.5.0/arthub_api/
--rw-rw-rw-   0        0        0      462 2023-03-13 11:08:42.000000 arthub_api-1.5.0/arthub_api/__init__.py
--rw-rw-rw-   0        0        0     2267 2023-02-08 16:32:42.000000 arthub_api-1.5.0/arthub_api/__main__.py
--rw-rw-rw-   0        0        0      241 2023-03-30 13:00:12.000000 arthub_api-1.5.0/arthub_api/__version__.py
--rw-rw-rw-   0        0        0    13661 2023-02-08 16:32:42.000000 arthub_api-1.5.0/arthub_api/_internal_utils.py
--rw-rw-rw-   0        0        0       35 2023-02-08 16:32:42.000000 arthub_api-1.5.0/arthub_api/arthub_api_config.py
--rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.5.0/arthub_api/asset_matrix.py
--rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.5.0/arthub_api/cli.py
--rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.5.0/arthub_api/config.py
--rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.5.0/arthub_api/exception.py
--rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.5.0/arthub_api/models.py
--rw-rw-rw-   0        0        0    41081 2023-03-30 10:39:24.000000 arthub_api-1.5.0/arthub_api/open_api.py
--rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.5.0/arthub_api/storage.py
--rw-rw-rw-   0        0        0     8151 2023-03-14 12:49:48.000000 arthub_api-1.5.0/arthub_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-30 13:20:20.505968 arthub_api-1.5.0/arthub_api.egg-info/
--rw-rw-rw-   0        0        0     1217 2023-03-30 13:20:19.000000 arthub_api-1.5.0/arthub_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      671 2023-03-30 13:20:20.000000 arthub_api-1.5.0/arthub_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 13:20:20.000000 arthub_api-1.5.0/arthub_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-03-30 13:20:20.000000 arthub_api-1.5.0/arthub_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.5.0/arthub_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       29 2023-03-30 13:20:20.000000 arthub_api-1.5.0/arthub_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-30 13:20:20.000000 arthub_api-1.5.0/arthub_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.5.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       42 2023-03-30 13:20:20.511952 arthub_api-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     2930 2023-02-08 12:46:33.000000 arthub_api-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 13:20:20.509995 arthub_api-1.5.0/tests/
--rw-rw-rw-   0        0        0       60 2023-02-08 16:32:42.000000 arthub_api-1.5.0/tests/__init__.py
--rw-rw-rw-   0        0        0     7080 2023-03-30 12:57:12.000000 arthub_api-1.5.0/tests/test_open_api.py
--rw-rw-rw-   0        0        0     3532 2023-03-30 12:40:48.000000 arthub_api-1.5.0/tests/test_storage.py
+drwxr-xr-x   0 joeyding   (501) staff       (20)        0 2023-04-11 14:21:34.000000 arthub_api-1.5.1/
+-rw-r--r--   0 joeyding   (501) staff       (20)     1439 2023-04-11 14:21:34.000000 arthub_api-1.5.1/PKG-INFO
+-rw-r--r--   0 joeyding   (501) staff       (20)     1060 2022-09-07 07:00:46.000000 arthub_api-1.5.1/LICENSE
+drwxr-xr-x   0 joeyding   (501) staff       (20)        0 2023-04-11 14:21:34.000000 arthub_api-1.5.1/tests/
+-rw-r--r--   0 joeyding   (501) staff       (20)     6867 2023-04-11 14:06:32.000000 arthub_api-1.5.1/tests/test_open_api.py
+-rw-r--r--   0 joeyding   (501) staff       (20)       58 2022-09-15 12:14:39.000000 arthub_api-1.5.1/tests/__init__.py
+-rw-r--r--   0 joeyding   (501) staff       (20)     3445 2023-04-11 14:06:32.000000 arthub_api-1.5.1/tests/test_storage.py
+-rw-r--r--   0 joeyding   (501) staff       (20)      105 2022-09-07 07:00:46.000000 arthub_api-1.5.1/MANIFEST.in
+-rw-r--r--   0 joeyding   (501) staff       (20)      676 2023-03-13 08:35:50.000000 arthub_api-1.5.1/README.md
+drwxr-xr-x   0 joeyding   (501) staff       (20)        0 2023-04-11 14:21:34.000000 arthub_api-1.5.1/arthub_api/
+-rw-r--r--   0 joeyding   (501) staff       (20)      498 2023-01-10 06:48:27.000000 arthub_api-1.5.1/arthub_api/exception.py
+-rw-r--r--   0 joeyding   (501) staff       (20)     1317 2022-09-28 09:32:10.000000 arthub_api-1.5.1/arthub_api/config.py
+-rw-r--r--   0 joeyding   (501) staff       (20)     1207 2023-04-11 14:06:32.000000 arthub_api-1.5.1/arthub_api/models.py
+-rw-r--r--   0 joeyding   (501) staff       (20)    39942 2023-04-11 14:06:32.000000 arthub_api-1.5.1/arthub_api/open_api.py
+-rw-r--r--   0 joeyding   (501) staff       (20)      462 2023-04-11 14:06:32.000000 arthub_api-1.5.1/arthub_api/__init__.py
+-rw-r--r--   0 joeyding   (501) staff       (20)      233 2023-04-11 14:19:14.000000 arthub_api-1.5.1/arthub_api/__version__.py
+-rw-r--r--   0 joeyding   (501) staff       (20)    13263 2023-01-10 06:48:27.000000 arthub_api-1.5.1/arthub_api/_internal_utils.py
+-rw-r--r--   0 joeyding   (501) staff       (20)       20 2022-09-25 13:57:22.000000 arthub_api-1.5.1/arthub_api/cli.py
+-rw-r--r--   0 joeyding   (501) staff       (20)     7872 2023-04-11 14:18:07.000000 arthub_api-1.5.1/arthub_api/utils.py
+-rw-r--r--   0 joeyding   (501) staff       (20)    41828 2023-04-11 14:06:32.000000 arthub_api-1.5.1/arthub_api/storage.py
+-rw-r--r--   0 joeyding   (501) staff       (20)      499 2023-04-11 14:06:32.000000 arthub_api-1.5.1/arthub_api/asset_matrix.py
+-rw-r--r--   0 joeyding   (501) staff       (20)       33 2022-09-15 11:19:06.000000 arthub_api-1.5.1/arthub_api/arthub_api_config.py
+-rw-r--r--   0 joeyding   (501) staff       (20)     2185 2023-01-10 06:48:27.000000 arthub_api-1.5.1/arthub_api/__main__.py
+-rw-r--r--   0 joeyding   (501) staff       (20)     2830 2023-03-13 08:35:50.000000 arthub_api-1.5.1/setup.py
+-rw-r--r--   0 joeyding   (501) staff       (20)       57 2022-09-26 09:04:30.000000 arthub_api-1.5.1/requirements-dev.txt
+-rw-r--r--   0 joeyding   (501) staff       (20)       38 2023-04-11 14:21:34.000000 arthub_api-1.5.1/setup.cfg
+drwxr-xr-x   0 joeyding   (501) staff       (20)        0 2023-04-11 14:21:34.000000 arthub_api-1.5.1/arthub_api.egg-info/
+-rw-r--r--   0 joeyding   (501) staff       (20)     1439 2023-04-11 14:21:34.000000 arthub_api-1.5.1/arthub_api.egg-info/PKG-INFO
+-rw-r--r--   0 joeyding   (501) staff       (20)        1 2022-09-15 12:23:18.000000 arthub_api-1.5.1/arthub_api.egg-info/not-zip-safe
+-rw-r--r--   0 joeyding   (501) staff       (20)      671 2023-04-11 14:21:34.000000 arthub_api-1.5.1/arthub_api.egg-info/SOURCES.txt
+-rw-r--r--   0 joeyding   (501) staff       (20)       50 2023-04-11 14:21:34.000000 arthub_api-1.5.1/arthub_api.egg-info/entry_points.txt
+-rw-r--r--   0 joeyding   (501) staff       (20)       29 2023-04-11 14:21:34.000000 arthub_api-1.5.1/arthub_api.egg-info/requires.txt
+-rw-r--r--   0 joeyding   (501) staff       (20)       11 2023-04-11 14:21:34.000000 arthub_api-1.5.1/arthub_api.egg-info/top_level.txt
+-rw-r--r--   0 joeyding   (501) staff       (20)        1 2023-04-11 14:21:34.000000 arthub_api-1.5.1/arthub_api.egg-info/dependency_links.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `arthub_api-1.5.0/LICENSE` & `arthub_api-1.5.1/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-MIT License
-Copyright (c) 2022 Tencent
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+Copyright (c) 2022 Tencent
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `arthub_api-1.5.0/README.md` & `arthub_api-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `arthub_api-1.5.0/arthub_api/__main__.py` & `arthub_api-1.5.1/arthub_api/__main__.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-import os
-import logging
-import logging.handlers
-from . import arthub_api_config
-from . import cli
-from . import utils
-
-
-def load_config(file_path=None):
-    UserError = type("UserError", (Exception,), {})
-
-    file_path = file_path or os.getenv("ARTHUB_API_CONFIG",
-                                       os.path.expanduser("~/Documents/ArtHub/arthub_api_config.py"))
-    if not os.path.isfile(file_path):
-        return
-
-    mod = {
-        "__file__": file_path,
-    }
-
-    try:
-        with open(file_path) as file_obj:
-            exec (compile(file_obj.read(), file_obj.name, "exec"), mod)
-    except IOError:
-        raise
-
-    except Exception:
-        raise UserError("Better double-check your user config.")
-
-    for key in dir(arthub_api_config):
-        if key.startswith("__"):
-            continue
-
-        try:
-            value = mod[key]
-        except KeyError:
-            continue
-        setattr(arthub_api_config, key, value)
-
-    return file_path
-
-
-def patch_config():
-    for member in dir(arthub_api_config):
-        if member.startswith("__"):
-            continue
-
-        setattr(arthub_api_config, "_%s" % member,
-                getattr(arthub_api_config, member))
-
-
-def setup_logging():
-    logger = logging.getLogger()
-    logger.setLevel(logging.DEBUG)
-
-    # to file
-    log_dir = os.path.expanduser("~/Documents/ArtHub/sdk_log")
-    if utils.mkdir(log_dir):
-        f_handler = logging.handlers.TimedRotatingFileHandler(os.path.join(log_dir, "arthub_api.log"),
-                                                              when='midnight', interval=1,
-                                                              backupCount=7)
-        f_handler.setLevel(logging.INFO)
-        f_handler.setFormatter(
-            logging.Formatter("%(asctime)s - %(levelname)s - %(filename)s[:%(lineno)d] - %(message)s"))
-        logger.addHandler(f_handler)
-
-    # to stdout
-    s_handler = logging.StreamHandler()
-    s_handler.setLevel(logging.DEBUG)
-    s_handler.setFormatter(logging.Formatter("%(message)s"))
-    logger.addHandler(s_handler)
-
-
-def init_cli():
-    setup_logging()
-    patch_config()
-    load_config()
-
-
-def main():
-    init_cli()
-    cli.cli()
+import os
+import logging
+import logging.handlers
+from . import arthub_api_config
+from . import cli
+from . import utils
+
+
+def load_config(file_path=None):
+    UserError = type("UserError", (Exception,), {})
+
+    file_path = file_path or os.getenv("ARTHUB_API_CONFIG",
+                                       os.path.expanduser("~/Documents/ArtHub/arthub_api_config.py"))
+    if not os.path.isfile(file_path):
+        return
+
+    mod = {
+        "__file__": file_path,
+    }
+
+    try:
+        with open(file_path) as file_obj:
+            exec (compile(file_obj.read(), file_obj.name, "exec"), mod)
+    except IOError:
+        raise
+
+    except Exception:
+        raise UserError("Better double-check your user config.")
+
+    for key in dir(arthub_api_config):
+        if key.startswith("__"):
+            continue
+
+        try:
+            value = mod[key]
+        except KeyError:
+            continue
+        setattr(arthub_api_config, key, value)
+
+    return file_path
+
+
+def patch_config():
+    for member in dir(arthub_api_config):
+        if member.startswith("__"):
+            continue
+
+        setattr(arthub_api_config, "_%s" % member,
+                getattr(arthub_api_config, member))
+
+
+def setup_logging():
+    logger = logging.getLogger()
+    logger.setLevel(logging.DEBUG)
+
+    # to file
+    log_dir = os.path.expanduser("~/Documents/ArtHub/sdk_log")
+    if utils.mkdir(log_dir):
+        f_handler = logging.handlers.TimedRotatingFileHandler(os.path.join(log_dir, "arthub_api.log"),
+                                                              when='midnight', interval=1,
+                                                              backupCount=7)
+        f_handler.setLevel(logging.INFO)
+        f_handler.setFormatter(
+            logging.Formatter("%(asctime)s - %(levelname)s - %(filename)s[:%(lineno)d] - %(message)s"))
+        logger.addHandler(f_handler)
+
+    # to stdout
+    s_handler = logging.StreamHandler()
+    s_handler.setLevel(logging.DEBUG)
+    s_handler.setFormatter(logging.Formatter("%(message)s"))
+    logger.addHandler(s_handler)
+
+
+def init_cli():
+    setup_logging()
+    patch_config()
+    load_config()
+
+
+def main():
+    init_cli()
+    cli.cli()
```

### Comparing `arthub_api-1.5.0/arthub_api/models.py` & `arthub_api-1.5.1/arthub_api/models.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-"""
-arthub_api.models
-~~~~~~~~~~~~~~~
-
-This module contains the primary objects.
-"""
-
-
-def failure_result(error_message):
-    return Result(succeeded=False, error_message=error_message)
-
-
-def success_result(data):
-    return Result(succeeded=True, data=data)
-
-
-class Result(object):
-    def __init__(self, succeeded, error_message="", data=None):
-        self._succeeded = succeeded
-        self._error_message = error_message
-        self._data = data
-
-    def __bool__(self):
-        return self.is_succeeded()
-
-    def is_succeeded(self):
-        return self._succeeded
-
-    def error_message(self):
-        return self._error_message
-
-    @property
-    def data(self):
-        return self._data
-
-    def set_data(self, data_):
-        self._data = data_
-
-
-class TaskResult(Result):
-    def __init__(self, succeeded, error_message="", data=None, progress_weight=0):
-        super(TaskResult, self).__init__(succeeded, error_message, data)
-        self._progress_weight = progress_weight
-
-    @property
-    def progress_weight(self):
-        return self._progress_weight
-
-
-def success_task_result(data, progress_weight=0):
-    return TaskResult(succeeded=True, data=data, progress_weight=progress_weight)
+"""
+arthub_api.models
+~~~~~~~~~~~~~~~
+
+This module contains the primary objects.
+"""
+
+
+def failure_result(error_message):
+    return Result(succeeded=False, error_message=error_message)
+
+
+def success_result(data):
+    return Result(succeeded=True, data=data)
+
+
+class Result(object):
+    def __init__(self, succeeded, error_message="", data=None):
+        self._succeeded = succeeded
+        self._error_message = error_message
+        self._data = data
+
+    def __bool__(self):
+        return self.is_succeeded()
+
+    def is_succeeded(self):
+        return self._succeeded
+
+    def error_message(self):
+        return self._error_message
+
+    @property
+    def data(self):
+        return self._data
+
+    def set_data(self, data_):
+        self._data = data_
+
+
+class TaskResult(Result):
+    def __init__(self, succeeded, error_message="", data=None, progress_weight=0):
+        super(TaskResult, self).__init__(succeeded, error_message, data)
+        self._progress_weight = progress_weight
+
+    @property
+    def progress_weight(self):
+        return self._progress_weight
+
+
+def success_task_result(data, progress_weight=0):
+    return TaskResult(succeeded=True, data=data, progress_weight=progress_weight)
```

### Comparing `arthub_api-1.5.0/arthub_api/open_api.py` & `arthub_api-1.5.1/arthub_api/open_api.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,1139 +1,1139 @@
-"""
-arthub_api.api
-~~~~~~~~~~~~~~
-
-This module encapsulates the ArtHub OpenAPI.
-For detailed interface doc: "https://arthub.aa.com/user_manual/index.html"
-"""
-import logging
-import requests
-from . import utils
-from . import models
-from . import _internal_utils
-from . import exception
-from xml.etree import ElementTree
-
-
-def _node_query_metas(simplified_meta=True):
-    metas = [
-        "name",
-        "file_format",
-        "node_type",
-        "permission_mask",
-        "direct_child_count",
-        "capacity",
-        "parent_id"
-    ]
-    if not simplified_meta:
-        metas += [
-            "full_path_id",
-            "full_path_name",
-            "confirmed_asset_id",
-            "preview_url",
-            "status",
-            "crc64",
-            "updated_date",
-            "description",
-            "total_leaf_count"
-        ]
-    return metas
-
-
-class APIResponse(object):
-    def __init__(self, http_response, network_connection_failed=False):
-        self._http_response = http_response
-        self._network_connection_failed = network_connection_failed
-        self._direct_result = None
-
-        self.api_result_code = -9999
-        self.api_item_result_code = -9999
-        self.api_error_message = "Unknown"
-        self.results = {}
-        self.errors = {}
-
-        self._preprocess()
-
-    def _preprocess(self):
-        if self._network_connection_failed:
-            return
-        if self._http_response is None:
-            return
-        if not self._http_response.ok:
-            logging.error("[API] request \"%s\" failed, code: %d" % (
-                self._http_response.url, self._http_response.status_code))
-            return
-        try:
-            # parse api response
-            _data = self._http_response.json()
-            # parse result code
-            self.api_result_code = _data["code"]
-            # parse result
-            self.parse_items(_data.get("result"), self.results)
-            # parse error
-            self.parse_items(_data.get("error"), self.errors)
-            # parse error message
-            self._parse_error()
-
-        except Exception:
-            logging.error("[API] parsing response exception, \"%s\"" % self._http_response.text)
-
-    def _parse_error(self):
-        if not self.errors:
-            return
-        e = self.errors.get(next(iter(self.errors)))
-        if e is None:
-            return
-        if type(e) is not dict:
-            self.api_error_message = e
-        else:
-            item_message = e.get("message")
-            item_error_code = e.get("error_code")
-            if item_message is not None:
-                self.api_error_message = item_message
-            if item_error_code is not None:
-                self.api_item_result_code = item_error_code
-
-    @property
-    def url(self):
-        if self._http_response is None:
-            return ""
-        return self._http_response.url
-
-    @property
-    def direct_result(self):
-        return self._direct_result
-
-    @property
-    def result(self):
-        return self._direct_result
-
-    def first_result(self, key=None):
-        if key:
-            return self.results.get(0).get(key)
-        else:
-            return self.results.get(0)
-
-    def set_direct_result_by_key(self, direct_result_key):
-        if self.is_succeeded():
-            self._direct_result = self.first_result(direct_result_key)
-
-    def set_direct_result(self, direct_result):
-        self._direct_result = direct_result
-
-    def set_result(self, result):
-        self._direct_result = result
-
-    @staticmethod
-    def parse_items(items_in, items_out):
-        if items_in is None:
-            return
-        t = type(items_in)
-        # example: "result": 123
-        if t != list and t != dict:
-            items_out[0] = items_in
-            return
-
-        items_list = []
-        if t == list:
-            # example: "result": []
-            items_list = items_in
-        else:
-            items_ = items_in.get("items")
-            if type(items_) == list:
-                # example: "result": {"items": []}
-                items_list = items_
-            else:
-                # example: "result": {}
-                items_out[0] = items_in
-                return
-
-        for i, item in enumerate(items_list):
-            if type(item) != dict:
-                items_out[i] = item
-                continue
-            param_index = item.get("param_index")
-            if type(param_index) == int:
-                items_out[param_index] = item
-            else:
-                items_out[i] = item
-
-    def is_http_request_succeeded(self):
-        if not self._http_response:
-            return False
-        return True
-
-    def is_succeeded(self):
-        r"""Batch call, all return success.
-        """
-
-        if not self.is_http_request_succeeded():
-            return False
-        return self.api_result_code == 0
-
-    def is_partial_succeeded(self):
-        r"""Batch call, partial success.
-        """
-
-        if not self.is_http_request_succeeded():
-            return False
-        return self.api_result_code == 1
-
-    def is_api_authentication_failed(self):
-        r"""Authentication failed.
-        """
-
-        if not self.is_http_request_succeeded():
-            return False
-        return self.api_result_code == -1
-
-    def is_no_permission(self):
-        r"""No access to target node, please contact the administrator.
-        """
-
-        if not self.is_http_request_succeeded():
-            return False
-        return self.api_result_code == -19 or self.api_item_result_code == -19
-
-    def is_node_not_exist(self):
-        r"""Node does not exist.
-        """
-
-        if not self.is_http_request_succeeded():
-            return False
-        return self.api_result_code == -10 or self.api_item_result_code == -10
-
-    def is_account_not_exist(self):
-        r"""User does not exist.
-        """
-
-        if not self.is_http_request_succeeded():
-            return False
-        return self.api_result_code == -6
-
-    def error_message(self):
-        if self._network_connection_failed:
-            return "network connection failed"
-        if not self._http_response.ok:
-            return "http request failed, code: %d" % self._http_response.status_code
-        if self.is_succeeded():
-            return "no error"
-        if self.is_api_authentication_failed():
-            return "authentication failed"
-        if self.is_no_permission():
-            return "no permission"
-        if self.is_node_not_exist():
-            return "node not exist"
-
-        return self.api_error_message
-
-
-class OpenAPI(object):
-    def __init__(self, config, get_token_from_cache=True):
-        r"""Used to call ArtHub openapi.
-        for detailed interface doc: "https://arthub.qq.com/user_manual/index.html"
-
-        :param config: from arthub_api.config.
-        """
-
-        self._config = config
-        self._token = ""
-        self._public_token = ""
-        self._cookies = None
-        self._api_version_depot = "v2"
-        self._api_version_blade = "v1"
-        self._api_version_gateway = "v2"
-        self._api_version_account = "v3"
-        self._cached_account_name = ""
-        self._cached_password = ""
-        self._auto_login = False
-        if get_token_from_cache:
-            self.get_token_from_cache()
-
-    @property
-    def config(self):
-        return self._config
-
-    @property
-    def api_host(self):
-        return self.config["host"]
-
-    @property
-    def http_scheme(self):
-        return self.config["http_scheme"]
-
-    @staticmethod
-    def get_node_permission_group(node_brief):
-        p = node_brief.get("permission_mask")
-        if p is None:
-            raise exception.Error(value="node brief does not contain field \"permission_mask\"")
-        permission_group = []
-        if p & (1 << 2) > 0:
-            permission_group.append("admin")
-        if p & (1 << 4) > 0:
-            permission_group.append("editor")
-        if p & (1 << 6) > 0:
-            permission_group.append("uploader")
-        if p & (1 << 8) > 0:
-            permission_group.append("downloader")
-        if p & (1 << 10) > 0:
-            permission_group.append("visitor")
-        if p & (1 << 12) > 0:
-            permission_group.append("pass")
-        return permission_group
-
-    def clear_token(self):
-        self._token = ""
-        self._public_token = ""
-
-    def clear_token_cache(self):
-        utils.remove_token_cache_file(self.api_host)
-
-    def logout(self):
-        self.clear_token()
-        self.clear_token_cache()
-
-    def get_token_from_cache(self):
-        token = utils.get_token_from_cache(self.api_host)
-        if token:
-            self._token = token
-
-    def save_token_to_cache(self):
-        if self._token:
-            utils.save_token_to_cache(self._token, self.api_host)
-
-    @property
-    def token(self):
-        return self._token
-
-    def set_token(self, token, save_to_cache=True):
-        r"""Set arthub token which is used to call api
-
-        :param token: str, a token obtained by API:login.
-        :param save_to_cache: (optional) bool. save the token to local cache
-        """
-
-        self._token = token
-        if save_to_cache:
-            self.save_token_to_cache()
-
-    def set_public_token(self, token):
-        r"""Set public token which is used to call api of data service
-
-        :param token: str, a public token issued by the administrator.
-        """
-
-        self._public_token = token
-
-    def set_cookies(self, cookie):
-        r"""Set cookies which is used to call api
-
-        :param cookie: str or dict, cookie from browser.
-        """
-
-        if type(cookie) is str:
-            self._cookies = utils.parse_cookies(cookie)
-        elif type(cookie) is dict:
-            self._cookies = cookie
-
-    def _depot_url(self, asset_hub, api_method):
-        return "%s//%s/%s/data/openapi/%s/core/%s" % (
-            self.http_scheme, self.api_host, asset_hub, self._api_version_depot, api_method)
-
-    def _blade_url(self, api_method):
-        return "%s//%s/blade/blade/openapi/%s/core/%s" % (
-            self.http_scheme, self.api_host, self._api_version_blade, api_method)
-
-    def _gateway_url(self, api_method):
-        return "%s//%s/gateway/gateway/openapi/%s/core/%s" % (
-            self.http_scheme, self.api_host, self._api_version_gateway, api_method)
-
-    def _account_url(self, api_method):
-        return "%s//%s/account/account/openapi/%s/core/%s" % (
-            self.http_scheme, self.api_host, self._api_version_account, api_method)
-
-    def _try_auto_login(self):
-        # Use the cached account password to log in again to get the token
-        if not self._auto_login:
-            return False
-        if len(self._cached_password) == 0 or len(self._cached_account_name) == 0:
-            return False
-        return self.login(self._cached_account_name, self._cached_password).is_succeeded()
-
-    def _make_api_request(self, url, data=None, method='POST', content_type='application/json',
-                          try_login_on_expired=True):
-        # set token to headers
-        headers = {}
-        if self._token:
-            headers["arthubtoken"] = self._token
-        if self._public_token:
-            headers["publictoken"] = self._public_token
-        headers["content-type"] = content_type
-
-        # send request
-        try:
-            res = requests.request(method=method, url=url, headers=headers, json=data, cookies=self._cookies)
-        except Exception as e:
-            logging.error("[API] send request \"%s\" exception: %s" % (url, e))
-            response = APIResponse(None, True)
-            return response
-
-        response = APIResponse(res)
-        if response.is_api_authentication_failed() and try_login_on_expired:
-            # Try to log in again due to authentication failure
-            if self._try_auto_login():
-                response = self._make_api_request(url, data, method, content_type, try_login_on_expired=False)
-
-        return response
-
-    def login(self, account_name, password, set_auto_login=True, save_token_to_cache=True):
-        r"""Login by email/mobile and password. You can visit https://arthub.qq.com to register.
-
-        :param account_name: str. email or mobile.
-        :param password: str. If you forget, visit https://arthub.qq.com/reset-password to reset
-        :param set_auto_login: (optional) bool. After successful login, save the account and password,
-               and login automatically after the login status expires
-        :param save_token_to_cache: (optional) bool. After successful login, save the token to local cache
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._account_url("login")
-        req_payload = {
-            "account_name": account_name,
-            "account_type": "mobile" if account_name.isdigit() else "email",
-            "password": password,
-            "current_time": utils.current_milli_time(),
-            "nounce": utils.get_random_string(8),
-            "oauth_type": "password",
-            "login_type": "arthub_token"
-        }
-        res = self._make_api_request(url, req_payload, try_login_on_expired=False)
-        if res.is_succeeded():
-            r = res.results.get(0)
-            token = r["arthub_token"]
-            self.set_token(token, save_token_to_cache)
-
-            self._auto_login = set_auto_login
-            # save account and password for auto login
-            if set_auto_login:
-                self._cached_account_name = account_name
-                self._cached_password = password
-
-        return res
-
-    def get_account_email(self):
-        r"""Get the email of the log-in account.
-
-        :rtype: str or None. Example: "XXX@tencent.com".
-        """
-
-        res = self.get_account_detail()
-        if not res.is_succeeded():
-            return None
-        return res.first_result("email")
-
-    def get_account_icon_url(self):
-        r"""Get the icon url of the log-in account.
-
-        :rtype: str or None.
-        """
-
-        res = self.get_account_detail()
-        if not res.is_succeeded():
-            return None
-        return res.first_result("icon_url")
-
-    def get_account_company(self):
-        r"""Get the company of the log-in account.
-
-        :rtype: str or None.
-        """
-
-        res = self.get_account_detail()
-        if not res.is_succeeded():
-            return None
-        return res.first_result("company")
-
-    def get_account_department(self):
-        r"""Get the department of the log-in account.
-
-        :rtype: str or None.
-        """
-
-        res = self.get_account_detail()
-        if not res.is_succeeded():
-            return None
-        return res.first_result("department")
-
-    def get_account_detail(self):
-        r"""Get the detail of user's account.
-
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._account_url("get-account-detail-by-account-name")
-        return self._make_api_request(url, method="GET")
-
-    def is_login(self):
-        r"""Check the login status.
-
-        :rtype: bool
-        """
-
-        if self._token == "" and self._public_token == "" and self._cookies is None:
-            return False
-
-        return self.get_account_detail().is_succeeded()
-
-    def get_ticket(self):
-        r"""Get the ticket to request websocket.
-
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._account_url("get-ticket")
-        return self._make_api_request(url, method="GET")
-
-    def set_last_access_location_by_account(self, last_location):
-        r"""Set the last access location of user's account.
-
-        :param last_location: str. Example: "gas/pan?node=120259084289".
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._account_url("set-last-access-location-by-account")
-        req_payload = {
-            "last_location": last_location
-        }
-        return self._make_api_request(url, req_payload)
-
-    def get_last_access_location_by_account(self):
-        r"""Get the user's last access location.
-
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._account_url("get-last-access-location-by-account")
-        return self._make_api_request(url, method="GET")
-
-    # depot
-    def depot_get_node_brief_by_ids(self, asset_hub, ids, simplified_meta=False):
-        r"""Get the brief of node by id in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param ids: list<int>. Example: [1234].
-        :param simplified_meta: (optional) bool. Just basic meta, lower bandwidth consumption.
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "get-node-brief-by-id")
-        req_payload = {
-            "ids": ids,
-            "meta": _node_query_metas(simplified_meta)
-        }
-        return self._make_api_request(url, req_payload)
-
-    def depot_get_download_signature(self, asset_hub, nodes):
-        r"""Get the download url of asset in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param nodes: list<node (dict) >. Example: [{"object_id": 110347249345024, "object_meta": "origin_url"}].
-                {
-                    "object_id": int, node id,
-                    "object_meta": str, Example: "origin_url"|"preview_url"
-                }
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "get-download-signature")
-        req_payload = {
-            "items": nodes
-        }
-        res = self._make_api_request(url, req_payload)
-        signed_url = "%s%s" % (self.http_scheme, res.first_result("signed_url"))
-        res.set_direct_result(signed_url)
-        return res
-
-    def depot_get_upload_signature(self, asset_hub, nodes):
-        r"""Get the upload url of asset in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param nodes: list<node (dict) >. Example: [{"object_id": 110347249345024, "object_meta": "origin_url"}].
-                {
-                    "object_id": int, node id,
-                    "object_meta": str, Example: "origin_url"|"preview_url",
-                    "file_name": file name to upload
-                }
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "get-upload-signature")
-        req_payload = {
-            "items": nodes
-        }
-        res = self._make_api_request(url, req_payload)
-        signed_url = "%s%s" % (self.http_scheme, res.first_result("signed_url"))
-        res.set_direct_result(signed_url)
-        return res
-
-    def depot_create_empty_file(self, asset_hub, asset_id, file_name):
-        r"""Create the empty file on storage of asset in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param asset_id: int. Example: 1234.
-        :param file_name: str. Example: "1.jpg".
-        :rtype: arthub_api.Result::data: {"origin_url": str}
-        """
-
-        api_res = self.depot_get_upload_signature(asset_hub, [{
-            "object_id": asset_id,
-            "object_meta": "origin_url",
-            "file_name": file_name
-        }])
-        if not api_res.is_succeeded():
-            return models.failure_result("get upload signature url of %d to create empty file failed, %s" % (
-                asset_id, api_res.error_message()))
-        signed_upload_url = api_res.direct_result
-        origin_url = api_res.first_result()["origin_url"]
-
-        # send signature url
-        try:
-            upload_res = requests.put(url=signed_upload_url, headers={"content-length": str(0)})
-        except Exception as e:
-            return models.failure_result("request \"%s\" exception, %s" % (
-                signed_upload_url, e))
-        if not upload_res.ok:
-            return models.failure_result("upload to \"%s\" failed, status code: %d" % (
-                signed_upload_url, upload_res.status_code))
-
-        return models.success_result({
-            "origin_url": origin_url
-        })
-
-    def depot_get_create_multipart_upload_signature(self, asset_hub, nodes):
-        r"""Get the multipart upload url to visit S3 in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param nodes: list<node (dict) >. Example: [{"object_id": 110347249345024, "object_meta": "origin_url"}].
-                {
-                    "object_id": int, node id,
-                    "object_meta": str, Example: "origin_url"|"preview_url",
-                    "file_name": file name to upload
-                }
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "create-multipart-upload-signature")
-        req_payload = {
-            "items": nodes
-        }
-        res = self._make_api_request(url, req_payload)
-        signed_url = "%s%s" % (self.http_scheme, res.first_result("signed_url"))
-        res.set_direct_result(signed_url)
-        return res
-
-    def depot_get_multipart_upload_id(self, asset_hub, asset_id, file_name):
-        r"""Get the multipart upload id to in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param asset_id: int. Example: 1234.
-        :param file_name: str. Example: "1.jpg".
-
-        :rtype: arthub_api.Result::data: {"upload_id": str, "origin_url": str}
-        """
-
-        # create multipart upload task
-        api_res = self.depot_get_create_multipart_upload_signature(asset_hub, [{
-            "object_id": asset_id,
-            "object_meta": "origin_url",
-            "file_name": file_name
-        }])
-        if not api_res.is_succeeded():
-            return models.failure_result("get create multipart upload signature url of %d failed, %s" % (
-                asset_id, api_res.error_message()))
-        signed_url = api_res.direct_result
-        origin_url = api_res.first_result()["origin_url"]
-        logging.info("[API] get begin multipart upload signed url: %s" % signed_url)
-
-        # send signature url
-        try:
-            res = requests.post(signed_url,
-                            headers={"content-type": _internal_utils.get_content_type_from_file_name(file_name)})
-        except Exception as e:
-            error_message = "request S3 multipart by url %s upload id exception: %s" % (signed_url, e)
-            logging.error("[API] %s" % error_message)
-            return models.failure_result(error_message)
-
-        if not res or not res.ok:
-            error_message = "request S3 multipart upload id failed, url: %s, code: %d" % (signed_url, res.status_code)
-            logging.error("[API] %s" % error_message)
-            return models.failure_result(error_message)
-
-        try:
-            xml_tree = ElementTree.fromstring(res.content)
-            upload_id = xml_tree.find("UploadId").text
-
-            logging.info("[API] get multipart upload id: %s" % upload_id)
-        except Exception as e:
-            error_message = "parsing S3 multipart upload id from \"%s\" exception, %s" % (res.text, e)
-            logging.error("[API] %s" % error_message)
-            return models.failure_result(error_message)
-        return models.success_result({
-            "origin_url": origin_url,
-            "upload_id": upload_id
-        })
-
-    def depot_get_part_upload_signature(self, asset_hub, nodes):
-        r"""Get the S3 part upload url.
-
-        :param asset_hub: str. Example: "trial".
-        :param nodes: list<node (dict) >. Example: [{"object_id": 110347249345024, "object_meta": "origin_url"}].
-                {
-                    "object_id": int, node id,
-                    "object_meta": str, Example: "origin_url"|"preview_url",
-                    "file_name": file name to upload,
-                    "upload_id": str, upload id of S3 multipart upload task,
-                    "origin_url": str, origin url,
-                    "part_number": int, upload part number, begin with 1
-                }
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "upload-part-signature")
-        req_payload = {
-            "items": nodes
-        }
-        res = self._make_api_request(url, req_payload)
-        signed_url = "%s%s" % (self.http_scheme, res.first_result("signed_url"))
-
-        logging.info("[API] get multipart upload signed url: %s" % signed_url)
-
-        res.set_direct_result(signed_url)
-        return res
-
-    def depot_get_complete_multipart_upload_signature(self, asset_hub, nodes):
-        r"""Get the multipart upload url to visit S3 in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param nodes: list<node (dict) >. Example: [{"object_id": 110347249345024, "object_meta": "origin_url"}].
-                {
-                    "object_id": int, node id,
-                    "object_meta": str, Example: "origin_url"|"preview_url",
-                    "object_id": str, origin url
-                    "file_name": file name to upload,
-                    "upload_id": str, upload id of S3 multipart upload task
-                }
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "complete-multipart-upload-signature")
-        req_payload = {
-            "items": nodes
-        }
-        res = self._make_api_request(url, req_payload)
-        signed_url = "%s%s" % (self.http_scheme, res.first_result("signed_url"))
-        res.set_direct_result(signed_url)
-        return res
-
-    def depot_complete_multipart_upload(self, asset_hub, asset_id, file_name, upload_id, origin_url, etag_data):
-        r"""Get the multipart upload id to in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param asset_id: int. Example: 1234.
-        :param file_name: str. Example: "1.jpg".
-        :param upload_id: str. upload id of S3 multipart upload task
-        :param origin_url: str. origin url
-        :param etag_data: object
-        :rtype: arthub_api.Result::data: {"upload_id": str, "origin_url": str}
-        """
-
-        # complete multipart upload task
-        api_res = self.depot_get_complete_multipart_upload_signature(asset_hub, [{
-            "object_id": asset_id,
-            "object_meta": "origin_url",
-            "file_name": file_name,
-            "upload_id": upload_id,
-            "origin_url": origin_url
-        }])
-        if not api_res.is_succeeded():
-            return models.failure_result("get complete multipart upload signature url of %d failed, %s" % (
-                asset_id, api_res.error_message()))
-        signed_url = api_res.direct_result
-
-        # send signature url
-        try:
-            res = requests.post(signed_url,
-                                headers={"content-type": "application/xml"}, data=etag_data)
-        except Exception as e:
-            error_message = "request complete S3 multipart upload by url %s exception: %s" % (signed_url, e)
-            logging.error("[API] %s" % error_message)
-            return models.failure_result(error_message)
-
-        if not res or not res.ok:
-            error_message = "request complete S3 multipart upload failed, url: %s, code: %d" % (
-                signed_url, res.status_code)
-            logging.error("[API] %s" % error_message)
-            return models.failure_result(error_message)
-        return models.success_result(None)
-
-    def depot_get_child_node_count(self, asset_hub, ids, query_filters=[], is_recursive=False):
-        r"""Get the child node count of node in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param ids: list<int>. Example: [1234].
-        :param query_filters: (optional) list<query_filter (dict) >. Example: [{"meta": "type", "condition": "x != project"}].
-                {
-                    "meta": filters meta,
-                    "condition": filters condition
-                }
-        :param is_recursive: (optional) bool, Whether to query recursively
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "get-child-node-count")
-        req_payload = {
-            "ids": ids,
-            "filter": query_filters,
-            "is_recursive": is_recursive
-        }
-        res = self._make_api_request(url, req_payload)
-        res.set_direct_result_by_key("count")
-        return res
-
-    def depot_get_child_node_id_in_range(self, asset_hub, parent_id, offset, count, query_filters=[],
-                                         is_recursive=False):
-        r"""Get the child node count of node in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param parent_id: int. Example: 1234.
-        :param offset: int. range offset: 0.
-        :param count: int. range count: 100.
-        :param query_filters: list<query_filter (dict) >. Example: [{"meta": "type", "condition": "x != project"}].
-                {
-                    "meta": filters meta,
-                    "condition": filters condition
-                }
-        :param is_recursive: (optional) bool, Whether to query recursively
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "get-child-node-id-in-range")
-        req_payload = {
-            "parent_id": parent_id,
-            "offset": offset,
-            "count": count,
-            "filter": query_filters,
-            "is_recursive": is_recursive
-        }
-        res = self._make_api_request(url, req_payload)
-        res.set_direct_result_by_key("nodes")
-        return res
-
-    def depot_get_node_brief_by_path(self, asset_hub, root_id, path, simplified_meta=False):
-        r"""Get the brief of node by path in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param root_id: int. Example: 1234.
-        :param path: str. Example: "1/2.jpg".
-        :param simplified_meta: (optional) bool. Just basic meta, lower bandwidth consumption.
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "get-node-brief-by-path")
-
-        path = path.replace('\\', '/')
-        req_payload = {
-            "root_id": root_id,
-            "path": [path],
-            "meta": _node_query_metas(simplified_meta)
-        }
-        return self._make_api_request(url, req_payload)
-
-    def depot_delete_node_by_ids(self, asset_hub, ids):
-        r"""delete the node in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param ids: list<int>. Example: [1234].
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "delete-node-by-id")
-        req_payload = {
-            "ids": ids
-        }
-        return self._make_api_request(url, req_payload)
-
-    def depot_move_node(self, asset_hub, ids, other_parent_id):
-        r"""move the node in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param ids: list<int>. Example: [1234, 3456].
-        :param other_parent_id: int.
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "move-node")
-        req_payload = {
-            "ids": ids,
-            "other_parent_id": other_parent_id
-        }
-        return self._make_api_request(url, req_payload)
-
-    def depot_create_project(self, asset_hub, name, parent_id, return_existing_id=True, show_detail_column=True,
-                             show_version_column=True,
-                             watermark=False):
-        r"""create project in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param name: str. project name. Example: "test".
-        :param parent_id: int. depot root id. Example: 304942678017.
-        :param return_existing_id: (optional) bool.
-        :param show_detail_column: (optional) bool.
-        :param show_version_column: (optional) bool.
-        :param watermark: (optional) bool.
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "create-project")
-        req_payload = [{
-            "name": name,
-            "parent_id": parent_id,
-            "return_existing_id": return_existing_id,
-            "show_detail_column": show_detail_column,
-            "show_version_column": show_version_column,
-            "watermark": watermark,
-        }]
-
-        res = self._make_api_request(url, req_payload)
-        res.set_direct_result_by_key("id")
-        return res
-
-    def depot_create_directory(self, asset_hub, payloads):
-        r"""create dirs in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param payloads: list<payload (dict) >.
-                {
-                    "parent_id": parent dir id,
-                    "name": name of new dir to create,
-                    "allowed_rename": allow renaming new dir to "name(<index>)" when a dir with the same name exists,
-                    "return_existing_id": returns the id of an existing dir with the same name
-                }
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "create-directory")
-        req_payload = {
-            "items": payloads
-        }
-
-        res = self._make_api_request(url, req_payload)
-        res.set_direct_result_by_key("id")
-        return res
-
-    def depot_create_asset(self, asset_hub, payloads):
-        r"""create assets in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param payloads: list<payload (dict) >.
-                {
-                    "parent_id": parent dir id,
-                    "name": name of new asset to create,
-                    "add_new_version": add a version when an asset with the same name exists,
-                }
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "create-asset")
-        req_payload = {
-            "items": payloads
-        }
-        res = self._make_api_request(url, req_payload)
-        res.set_direct_result_by_key("id")
-        return res
-
-    def depot_create_multi_asset(self, asset_hub, payloads):
-        r"""create multi asset (version container) in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param payloads: list<payload (dict) >.
-                {
-                    "parent_id": parent dir id,
-                    "name": name of new multi asset to create,
-                }
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "create-multi-asset")
-        req_payload = {
-            "items": payloads
-        }
-        return self._make_api_request(url, req_payload)
-
-    def depot_update_asset_by_id(self, asset_hub, payloads):
-        r"""update metas of asset in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param payloads: list<payload (dict) >.
-                {
-                    "id": int, node id,
-                    "name": str, node name,
-                    "origin_url": origin url,
-                    "description": description of node
-                }
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "update-asset-by-id")
-        req_payload = {
-            "items": payloads
-        }
-        return self._make_api_request(url, req_payload)
-
-    def depot_convert_asset(self, asset_hub, asset_files, asset_ids):
-        r"""convert asset in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param asset_files: list<str>. Example: ["//ahs_cos_guangzhou_1/assethub-trial-1258344700/cospri/download/110347249345/110347249345067/1.png"].
-        :param asset_ids: list<int>. Example: [110347249345067].
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "convert-asset")
-        req_payload = {
-            "asset_files": asset_files,
-            "asset_ids": asset_ids
-        }
-        return self._make_api_request(url, req_payload)
-
-    def depot_create_tsa(self, asset_hub, asset_id, company, description, title, tsa_info):
-        r"""convert asset in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param asset_id: int. Example: 110347249345071.
-        :param company: str. Example: "Tencent".
-        :param description: str. Example: "New weapon".
-        :param title: str. Example: "Christmas".
-        :param tsa_info: str. Example: "Characters; Web design".
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "create-tsa")
-        req_payload = {
-            "asset_id": asset_id,
-            "company": company,
-            "description": description,
-            "title": title,
-            "tsa_info": tsa_info
-        }
-        return self._make_api_request(url, req_payload)
-
-    def depot_add_asset_tag(self, asset_hub, asset_id, tag_name):
-        r"""add tags to asset node in depot.
-
-        :param asset_hub: str. Example: "trial".
-        :param asset_id: int. Example: 110347249345071.
-        :param tag_name: list<str>. Example: ["tag_1", "tag_2"].
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "add-asset-tag")
-        req_payload = {
-            "asset_id": asset_id,
-            "tag_name": tag_name
-        }
-        return self._make_api_request(url, req_payload)
-
-    def depot_update_directory_by_id(self, asset_hub, payloads):
-        r"""update metas of directory in depot .
-
-        :param asset_hub: str. Example: "trial".
-        :param payloads: list<payload (dict) >.
-                {
-                    "id": int, node id,
-                    "name": str, node name,
-                    "origin_url": origin url,
-                    "description": description of node
-                }
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "update-directory-by-id")
-        req_payload = {
-            "items": payloads
-        }
-        return self._make_api_request(url, req_payload)
-
-    def depot_update_project_by_id(self, asset_hub, payloads):
-        r"""update metas of project in depot .
-
-        :param asset_hub: str. Example: "trial".
-        :param payloads: list<payload (dict) >.
-                {
-                    "id": int, node id,
-                    "name": str, node name,
-                    "origin_url": origin url,
-                    "description": description of node
-                }
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "update-project-by-id")
-        req_payload = {
-            "items": payloads
-        }
-        return self._make_api_request(url, req_payload)
-
-    def depot_update_multi_asset_by_id(self, asset_hub, payloads):
-        r"""update metas of multi asset in depot .
-
-        :param asset_hub: str. Example: "trial".
-        :param payloads: list<payload (dict) >.
-                {
-                    "id": int, node id,
-                    "name": str, node name,
-                    "origin_url": origin url,
-                    "description": description of node
-                }
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "update-multi-asset-by-id")
-        req_payload = {
-            "items": payloads
-        }
-        return self._make_api_request(url, req_payload)
-
-    def depot_get_root_id(self, asset_hub):
-        r"""get the depot root id of asset hub.
-
-        :param asset_hub: str. Example: "trial".
-        :rtype: arthub_api.APIResponse
-        """
-
-        url = self._depot_url(asset_hub, "get-depot-id")
-        return self._make_api_request(url)
-
-    # blade
-    def blade_get_account_if_exist(self, user_name):
-        r"""get the account detail by user name.
-
-        :param user_name: str. Example: "joeyding".
-        :rtype: arthub_api.APIResponse
-                result: {
-                    "nick_name": string,
-                    "email": string,
-                    "company": string,
-                    "department": string,
-                    ...}
-        """
-
-        url = self._blade_url("get-account-if-exist")
-        req_payload = {
-            "account_name": user_name
-        }
-        res = self._make_api_request(url, req_payload)
-        res.set_result(res.first_result())
-        return res
-
-    def reset_config(self, config):
-        self._config = config
+"""
+arthub_api.api
+~~~~~~~~~~~~~~
+
+This module encapsulates the ArtHub OpenAPI.
+For detailed interface doc: "https://arthub.aa.com/user_manual/index.html"
+"""
+import logging
+import requests
+from . import utils
+from . import models
+from . import _internal_utils
+from . import exception
+from xml.etree import ElementTree
+
+
+def _node_query_metas(simplified_meta=True):
+    metas = [
+        "name",
+        "file_format",
+        "node_type",
+        "permission_mask",
+        "direct_child_count",
+        "capacity",
+        "parent_id"
+    ]
+    if not simplified_meta:
+        metas += [
+            "full_path_id",
+            "full_path_name",
+            "confirmed_asset_id",
+            "preview_url",
+            "status",
+            "crc64",
+            "updated_date",
+            "description",
+            "total_leaf_count"
+        ]
+    return metas
+
+
+class APIResponse(object):
+    def __init__(self, http_response, network_connection_failed=False):
+        self._http_response = http_response
+        self._network_connection_failed = network_connection_failed
+        self._direct_result = None
+
+        self.api_result_code = -9999
+        self.api_item_result_code = -9999
+        self.api_error_message = "Unknown"
+        self.results = {}
+        self.errors = {}
+
+        self._preprocess()
+
+    def _preprocess(self):
+        if self._network_connection_failed:
+            return
+        if self._http_response is None:
+            return
+        if not self._http_response.ok:
+            logging.error("[API] request \"%s\" failed, code: %d" % (
+                self._http_response.url, self._http_response.status_code))
+            return
+        try:
+            # parse api response
+            _data = self._http_response.json()
+            # parse result code
+            self.api_result_code = _data["code"]
+            # parse result
+            self.parse_items(_data.get("result"), self.results)
+            # parse error
+            self.parse_items(_data.get("error"), self.errors)
+            # parse error message
+            self._parse_error()
+
+        except Exception:
+            logging.error("[API] parsing response exception, \"%s\"" % self._http_response.text)
+
+    def _parse_error(self):
+        if not self.errors:
+            return
+        e = self.errors.get(next(iter(self.errors)))
+        if e is None:
+            return
+        if type(e) is not dict:
+            self.api_error_message = e
+        else:
+            item_message = e.get("message")
+            item_error_code = e.get("error_code")
+            if item_message is not None:
+                self.api_error_message = item_message
+            if item_error_code is not None:
+                self.api_item_result_code = item_error_code
+
+    @property
+    def url(self):
+        if self._http_response is None:
+            return ""
+        return self._http_response.url
+
+    @property
+    def direct_result(self):
+        return self._direct_result
+
+    @property
+    def result(self):
+        return self._direct_result
+
+    def first_result(self, key=None):
+        if key:
+            return self.results.get(0).get(key)
+        else:
+            return self.results.get(0)
+
+    def set_direct_result_by_key(self, direct_result_key):
+        if self.is_succeeded():
+            self._direct_result = self.first_result(direct_result_key)
+
+    def set_direct_result(self, direct_result):
+        self._direct_result = direct_result
+
+    def set_result(self, result):
+        self._direct_result = result
+
+    @staticmethod
+    def parse_items(items_in, items_out):
+        if items_in is None:
+            return
+        t = type(items_in)
+        # example: "result": 123
+        if t != list and t != dict:
+            items_out[0] = items_in
+            return
+
+        items_list = []
+        if t == list:
+            # example: "result": []
+            items_list = items_in
+        else:
+            items_ = items_in.get("items")
+            if type(items_) == list:
+                # example: "result": {"items": []}
+                items_list = items_
+            else:
+                # example: "result": {}
+                items_out[0] = items_in
+                return
+
+        for i, item in enumerate(items_list):
+            if type(item) != dict:
+                items_out[i] = item
+                continue
+            param_index = item.get("param_index")
+            if type(param_index) == int:
+                items_out[param_index] = item
+            else:
+                items_out[i] = item
+
+    def is_http_request_succeeded(self):
+        if not self._http_response:
+            return False
+        return True
+
+    def is_succeeded(self):
+        r"""Batch call, all return success.
+        """
+
+        if not self.is_http_request_succeeded():
+            return False
+        return self.api_result_code == 0
+
+    def is_partial_succeeded(self):
+        r"""Batch call, partial success.
+        """
+
+        if not self.is_http_request_succeeded():
+            return False
+        return self.api_result_code == 1
+
+    def is_api_authentication_failed(self):
+        r"""Authentication failed.
+        """
+
+        if not self.is_http_request_succeeded():
+            return False
+        return self.api_result_code == -1
+
+    def is_no_permission(self):
+        r"""No access to target node, please contact the administrator.
+        """
+
+        if not self.is_http_request_succeeded():
+            return False
+        return self.api_result_code == -19 or self.api_item_result_code == -19
+
+    def is_node_not_exist(self):
+        r"""Node does not exist.
+        """
+
+        if not self.is_http_request_succeeded():
+            return False
+        return self.api_result_code == -10 or self.api_item_result_code == -10
+
+    def is_account_not_exist(self):
+        r"""User does not exist.
+        """
+
+        if not self.is_http_request_succeeded():
+            return False
+        return self.api_result_code == -6
+
+    def error_message(self):
+        if self._network_connection_failed:
+            return "network connection failed"
+        if not self._http_response.ok:
+            return "http request failed, code: %d" % self._http_response.status_code
+        if self.is_succeeded():
+            return "no error"
+        if self.is_api_authentication_failed():
+            return "authentication failed"
+        if self.is_no_permission():
+            return "no permission"
+        if self.is_node_not_exist():
+            return "node not exist"
+
+        return self.api_error_message
+
+
+class OpenAPI(object):
+    def __init__(self, config, get_token_from_cache=True):
+        r"""Used to call ArtHub openapi.
+        for detailed interface doc: "https://arthub.qq.com/user_manual/index.html"
+
+        :param config: from arthub_api.config.
+        """
+
+        self._config = config
+        self._token = ""
+        self._public_token = ""
+        self._cookies = None
+        self._api_version_depot = "v2"
+        self._api_version_blade = "v1"
+        self._api_version_gateway = "v2"
+        self._api_version_account = "v3"
+        self._cached_account_name = ""
+        self._cached_password = ""
+        self._auto_login = False
+        if get_token_from_cache:
+            self.get_token_from_cache()
+
+    @property
+    def config(self):
+        return self._config
+
+    @property
+    def api_host(self):
+        return self.config["host"]
+
+    @property
+    def http_scheme(self):
+        return self.config["http_scheme"]
+
+    @staticmethod
+    def get_node_permission_group(node_brief):
+        p = node_brief.get("permission_mask")
+        if p is None:
+            raise exception.Error(value="node brief does not contain field \"permission_mask\"")
+        permission_group = []
+        if p & (1 << 2) > 0:
+            permission_group.append("admin")
+        if p & (1 << 4) > 0:
+            permission_group.append("editor")
+        if p & (1 << 6) > 0:
+            permission_group.append("uploader")
+        if p & (1 << 8) > 0:
+            permission_group.append("downloader")
+        if p & (1 << 10) > 0:
+            permission_group.append("visitor")
+        if p & (1 << 12) > 0:
+            permission_group.append("pass")
+        return permission_group
+
+    def clear_token(self):
+        self._token = ""
+        self._public_token = ""
+
+    def clear_token_cache(self):
+        utils.remove_token_cache_file(self.api_host)
+
+    def logout(self):
+        self.clear_token()
+        self.clear_token_cache()
+
+    def get_token_from_cache(self):
+        token = utils.get_token_from_cache(self.api_host)
+        if token:
+            self._token = token
+
+    def save_token_to_cache(self):
+        if self._token:
+            utils.save_token_to_cache(self._token, self.api_host)
+
+    @property
+    def token(self):
+        return self._token
+
+    def set_token(self, token, save_to_cache=True):
+        r"""Set arthub token which is used to call api
+
+        :param token: str, a token obtained by API:login.
+        :param save_to_cache: (optional) bool. save the token to local cache
+        """
+
+        self._token = token
+        if save_to_cache:
+            self.save_token_to_cache()
+
+    def set_public_token(self, token):
+        r"""Set public token which is used to call api of data service
+
+        :param token: str, a public token issued by the administrator.
+        """
+
+        self._public_token = token
+
+    def set_cookies(self, cookie):
+        r"""Set cookies which is used to call api
+
+        :param cookie: str or dict, cookie from browser.
+        """
+
+        if type(cookie) is str:
+            self._cookies = utils.parse_cookies(cookie)
+        elif type(cookie) is dict:
+            self._cookies = cookie
+
+    def _depot_url(self, asset_hub, api_method):
+        return "%s//%s/%s/data/openapi/%s/core/%s" % (
+            self.http_scheme, self.api_host, asset_hub, self._api_version_depot, api_method)
+
+    def _blade_url(self, api_method):
+        return "%s//%s/blade/blade/openapi/%s/core/%s" % (
+            self.http_scheme, self.api_host, self._api_version_blade, api_method)
+
+    def _gateway_url(self, api_method):
+        return "%s//%s/gateway/gateway/openapi/%s/core/%s" % (
+            self.http_scheme, self.api_host, self._api_version_gateway, api_method)
+
+    def _account_url(self, api_method):
+        return "%s//%s/account/account/openapi/%s/core/%s" % (
+            self.http_scheme, self.api_host, self._api_version_account, api_method)
+
+    def _try_auto_login(self):
+        # Use the cached account password to log in again to get the token
+        if not self._auto_login:
+            return False
+        if len(self._cached_password) == 0 or len(self._cached_account_name) == 0:
+            return False
+        return self.login(self._cached_account_name, self._cached_password).is_succeeded()
+
+    def _make_api_request(self, url, data=None, method='POST', content_type='application/json',
+                          try_login_on_expired=True):
+        # set token to headers
+        headers = {}
+        if self._token:
+            headers["arthubtoken"] = self._token
+        if self._public_token:
+            headers["publictoken"] = self._public_token
+        headers["content-type"] = content_type
+
+        # send request
+        try:
+            res = requests.request(method=method, url=url, headers=headers, json=data, cookies=self._cookies)
+        except Exception as e:
+            logging.error("[API] send request \"%s\" exception: %s" % (url, e))
+            response = APIResponse(None, True)
+            return response
+
+        response = APIResponse(res)
+        if response.is_api_authentication_failed() and try_login_on_expired:
+            # Try to log in again due to authentication failure
+            if self._try_auto_login():
+                response = self._make_api_request(url, data, method, content_type, try_login_on_expired=False)
+
+        return response
+
+    def login(self, account_name, password, set_auto_login=True, save_token_to_cache=True):
+        r"""Login by email/mobile and password. You can visit https://arthub.qq.com to register.
+
+        :param account_name: str. email or mobile.
+        :param password: str. If you forget, visit https://arthub.qq.com/reset-password to reset
+        :param set_auto_login: (optional) bool. After successful login, save the account and password,
+               and login automatically after the login status expires
+        :param save_token_to_cache: (optional) bool. After successful login, save the token to local cache
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._account_url("login")
+        req_payload = {
+            "account_name": account_name,
+            "account_type": "mobile" if account_name.isdigit() else "email",
+            "password": password,
+            "current_time": utils.current_milli_time(),
+            "nounce": utils.get_random_string(8),
+            "oauth_type": "password",
+            "login_type": "arthub_token"
+        }
+        res = self._make_api_request(url, req_payload, try_login_on_expired=False)
+        if res.is_succeeded():
+            r = res.results.get(0)
+            token = r["arthub_token"]
+            self.set_token(token, save_token_to_cache)
+
+            self._auto_login = set_auto_login
+            # save account and password for auto login
+            if set_auto_login:
+                self._cached_account_name = account_name
+                self._cached_password = password
+
+        return res
+
+    def get_account_email(self):
+        r"""Get the email of the log-in account.
+
+        :rtype: str or None. Example: "XXX@tencent.com".
+        """
+
+        res = self.get_account_detail()
+        if not res.is_succeeded():
+            return None
+        return res.first_result("email")
+
+    def get_account_icon_url(self):
+        r"""Get the icon url of the log-in account.
+
+        :rtype: str or None.
+        """
+
+        res = self.get_account_detail()
+        if not res.is_succeeded():
+            return None
+        return res.first_result("icon_url")
+
+    def get_account_company(self):
+        r"""Get the company of the log-in account.
+
+        :rtype: str or None.
+        """
+
+        res = self.get_account_detail()
+        if not res.is_succeeded():
+            return None
+        return res.first_result("company")
+
+    def get_account_department(self):
+        r"""Get the department of the log-in account.
+
+        :rtype: str or None.
+        """
+
+        res = self.get_account_detail()
+        if not res.is_succeeded():
+            return None
+        return res.first_result("department")
+
+    def get_account_detail(self):
+        r"""Get the detail of user's account.
+
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._account_url("get-account-detail-by-account-name")
+        return self._make_api_request(url, method="GET")
+
+    def is_login(self):
+        r"""Check the login status.
+
+        :rtype: bool
+        """
+
+        if self._token == "" and self._public_token == "" and self._cookies is None:
+            return False
+
+        return self.get_account_detail().is_succeeded()
+
+    def get_ticket(self):
+        r"""Get the ticket to request websocket.
+
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._account_url("get-ticket")
+        return self._make_api_request(url, method="GET")
+
+    def set_last_access_location_by_account(self, last_location):
+        r"""Set the last access location of user's account.
+
+        :param last_location: str. Example: "gas/pan?node=120259084289".
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._account_url("set-last-access-location-by-account")
+        req_payload = {
+            "last_location": last_location
+        }
+        return self._make_api_request(url, req_payload)
+
+    def get_last_access_location_by_account(self):
+        r"""Get the user's last access location.
+
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._account_url("get-last-access-location-by-account")
+        return self._make_api_request(url, method="GET")
+
+    # depot
+    def depot_get_node_brief_by_ids(self, asset_hub, ids, simplified_meta=False):
+        r"""Get the brief of node by id in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param ids: list<int>. Example: [1234].
+        :param simplified_meta: (optional) bool. Just basic meta, lower bandwidth consumption.
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "get-node-brief-by-id")
+        req_payload = {
+            "ids": ids,
+            "meta": _node_query_metas(simplified_meta)
+        }
+        return self._make_api_request(url, req_payload)
+
+    def depot_get_download_signature(self, asset_hub, nodes):
+        r"""Get the download url of asset in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param nodes: list<node (dict) >. Example: [{"object_id": 110347249345024, "object_meta": "origin_url"}].
+                {
+                    "object_id": int, node id,
+                    "object_meta": str, Example: "origin_url"|"preview_url"
+                }
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "get-download-signature")
+        req_payload = {
+            "items": nodes
+        }
+        res = self._make_api_request(url, req_payload)
+        signed_url = "%s%s" % (self.http_scheme, res.first_result("signed_url"))
+        res.set_direct_result(signed_url)
+        return res
+
+    def depot_get_upload_signature(self, asset_hub, nodes):
+        r"""Get the upload url of asset in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param nodes: list<node (dict) >. Example: [{"object_id": 110347249345024, "object_meta": "origin_url"}].
+                {
+                    "object_id": int, node id,
+                    "object_meta": str, Example: "origin_url"|"preview_url",
+                    "file_name": file name to upload
+                }
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "get-upload-signature")
+        req_payload = {
+            "items": nodes
+        }
+        res = self._make_api_request(url, req_payload)
+        signed_url = "%s%s" % (self.http_scheme, res.first_result("signed_url"))
+        res.set_direct_result(signed_url)
+        return res
+
+    def depot_create_empty_file(self, asset_hub, asset_id, file_name):
+        r"""Create the empty file on storage of asset in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param asset_id: int. Example: 1234.
+        :param file_name: str. Example: "1.jpg".
+        :rtype: arthub_api.Result::data: {"origin_url": str}
+        """
+
+        api_res = self.depot_get_upload_signature(asset_hub, [{
+            "object_id": asset_id,
+            "object_meta": "origin_url",
+            "file_name": file_name
+        }])
+        if not api_res.is_succeeded():
+            return models.failure_result("get upload signature url of %d to create empty file failed, %s" % (
+                asset_id, api_res.error_message()))
+        signed_upload_url = api_res.direct_result
+        origin_url = api_res.first_result()["origin_url"]
+
+        # send signature url
+        try:
+            upload_res = requests.put(url=signed_upload_url, headers={"content-length": str(0)})
+        except Exception as e:
+            return models.failure_result("request \"%s\" exception, %s" % (
+                signed_upload_url, e))
+        if not upload_res.ok:
+            return models.failure_result("upload to \"%s\" failed, status code: %d" % (
+                signed_upload_url, upload_res.status_code))
+
+        return models.success_result({
+            "origin_url": origin_url
+        })
+
+    def depot_get_create_multipart_upload_signature(self, asset_hub, nodes):
+        r"""Get the multipart upload url to visit S3 in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param nodes: list<node (dict) >. Example: [{"object_id": 110347249345024, "object_meta": "origin_url"}].
+                {
+                    "object_id": int, node id,
+                    "object_meta": str, Example: "origin_url"|"preview_url",
+                    "file_name": file name to upload
+                }
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "create-multipart-upload-signature")
+        req_payload = {
+            "items": nodes
+        }
+        res = self._make_api_request(url, req_payload)
+        signed_url = "%s%s" % (self.http_scheme, res.first_result("signed_url"))
+        res.set_direct_result(signed_url)
+        return res
+
+    def depot_get_multipart_upload_id(self, asset_hub, asset_id, file_name):
+        r"""Get the multipart upload id to in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param asset_id: int. Example: 1234.
+        :param file_name: str. Example: "1.jpg".
+
+        :rtype: arthub_api.Result::data: {"upload_id": str, "origin_url": str}
+        """
+
+        # create multipart upload task
+        api_res = self.depot_get_create_multipart_upload_signature(asset_hub, [{
+            "object_id": asset_id,
+            "object_meta": "origin_url",
+            "file_name": file_name
+        }])
+        if not api_res.is_succeeded():
+            return models.failure_result("get create multipart upload signature url of %d failed, %s" % (
+                asset_id, api_res.error_message()))
+        signed_url = api_res.direct_result
+        origin_url = api_res.first_result()["origin_url"]
+        logging.info("[API] get begin multipart upload signed url: %s" % signed_url)
+
+        # send signature url
+        try:
+            res = requests.post(signed_url,
+                            headers={"content-type": _internal_utils.get_content_type_from_file_name(file_name)})
+        except Exception as e:
+            error_message = "request S3 multipart by url %s upload id exception: %s" % (signed_url, e)
+            logging.error("[API] %s" % error_message)
+            return models.failure_result(error_message)
+
+        if not res or not res.ok:
+            error_message = "request S3 multipart upload id failed, url: %s, code: %d" % (signed_url, res.status_code)
+            logging.error("[API] %s" % error_message)
+            return models.failure_result(error_message)
+
+        try:
+            xml_tree = ElementTree.fromstring(res.content)
+            upload_id = xml_tree.find("UploadId").text
+
+            logging.info("[API] get multipart upload id: %s" % upload_id)
+        except Exception as e:
+            error_message = "parsing S3 multipart upload id from \"%s\" exception, %s" % (res.text, e)
+            logging.error("[API] %s" % error_message)
+            return models.failure_result(error_message)
+        return models.success_result({
+            "origin_url": origin_url,
+            "upload_id": upload_id
+        })
+
+    def depot_get_part_upload_signature(self, asset_hub, nodes):
+        r"""Get the S3 part upload url.
+
+        :param asset_hub: str. Example: "trial".
+        :param nodes: list<node (dict) >. Example: [{"object_id": 110347249345024, "object_meta": "origin_url"}].
+                {
+                    "object_id": int, node id,
+                    "object_meta": str, Example: "origin_url"|"preview_url",
+                    "file_name": file name to upload,
+                    "upload_id": str, upload id of S3 multipart upload task,
+                    "origin_url": str, origin url,
+                    "part_number": int, upload part number, begin with 1
+                }
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "upload-part-signature")
+        req_payload = {
+            "items": nodes
+        }
+        res = self._make_api_request(url, req_payload)
+        signed_url = "%s%s" % (self.http_scheme, res.first_result("signed_url"))
+
+        logging.info("[API] get multipart upload signed url: %s" % signed_url)
+
+        res.set_direct_result(signed_url)
+        return res
+
+    def depot_get_complete_multipart_upload_signature(self, asset_hub, nodes):
+        r"""Get the multipart upload url to visit S3 in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param nodes: list<node (dict) >. Example: [{"object_id": 110347249345024, "object_meta": "origin_url"}].
+                {
+                    "object_id": int, node id,
+                    "object_meta": str, Example: "origin_url"|"preview_url",
+                    "object_id": str, origin url
+                    "file_name": file name to upload,
+                    "upload_id": str, upload id of S3 multipart upload task
+                }
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "complete-multipart-upload-signature")
+        req_payload = {
+            "items": nodes
+        }
+        res = self._make_api_request(url, req_payload)
+        signed_url = "%s%s" % (self.http_scheme, res.first_result("signed_url"))
+        res.set_direct_result(signed_url)
+        return res
+
+    def depot_complete_multipart_upload(self, asset_hub, asset_id, file_name, upload_id, origin_url, etag_data):
+        r"""Get the multipart upload id to in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param asset_id: int. Example: 1234.
+        :param file_name: str. Example: "1.jpg".
+        :param upload_id: str. upload id of S3 multipart upload task
+        :param origin_url: str. origin url
+        :param etag_data: object
+        :rtype: arthub_api.Result::data: {"upload_id": str, "origin_url": str}
+        """
+
+        # complete multipart upload task
+        api_res = self.depot_get_complete_multipart_upload_signature(asset_hub, [{
+            "object_id": asset_id,
+            "object_meta": "origin_url",
+            "file_name": file_name,
+            "upload_id": upload_id,
+            "origin_url": origin_url
+        }])
+        if not api_res.is_succeeded():
+            return models.failure_result("get complete multipart upload signature url of %d failed, %s" % (
+                asset_id, api_res.error_message()))
+        signed_url = api_res.direct_result
+
+        # send signature url
+        try:
+            res = requests.post(signed_url,
+                                headers={"content-type": "application/xml"}, data=etag_data)
+        except Exception as e:
+            error_message = "request complete S3 multipart upload by url %s exception: %s" % (signed_url, e)
+            logging.error("[API] %s" % error_message)
+            return models.failure_result(error_message)
+
+        if not res or not res.ok:
+            error_message = "request complete S3 multipart upload failed, url: %s, code: %d" % (
+                signed_url, res.status_code)
+            logging.error("[API] %s" % error_message)
+            return models.failure_result(error_message)
+        return models.success_result(None)
+
+    def depot_get_child_node_count(self, asset_hub, ids, query_filters=[], is_recursive=False):
+        r"""Get the child node count of node in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param ids: list<int>. Example: [1234].
+        :param query_filters: (optional) list<query_filter (dict) >. Example: [{"meta": "type", "condition": "x != project"}].
+                {
+                    "meta": filters meta,
+                    "condition": filters condition
+                }
+        :param is_recursive: (optional) bool, Whether to query recursively
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "get-child-node-count")
+        req_payload = {
+            "ids": ids,
+            "filter": query_filters,
+            "is_recursive": is_recursive
+        }
+        res = self._make_api_request(url, req_payload)
+        res.set_direct_result_by_key("count")
+        return res
+
+    def depot_get_child_node_id_in_range(self, asset_hub, parent_id, offset, count, query_filters=[],
+                                         is_recursive=False):
+        r"""Get the child node count of node in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param parent_id: int. Example: 1234.
+        :param offset: int. range offset: 0.
+        :param count: int. range count: 100.
+        :param query_filters: list<query_filter (dict) >. Example: [{"meta": "type", "condition": "x != project"}].
+                {
+                    "meta": filters meta,
+                    "condition": filters condition
+                }
+        :param is_recursive: (optional) bool, Whether to query recursively
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "get-child-node-id-in-range")
+        req_payload = {
+            "parent_id": parent_id,
+            "offset": offset,
+            "count": count,
+            "filter": query_filters,
+            "is_recursive": is_recursive
+        }
+        res = self._make_api_request(url, req_payload)
+        res.set_direct_result_by_key("nodes")
+        return res
+
+    def depot_get_node_brief_by_path(self, asset_hub, root_id, path, simplified_meta=False):
+        r"""Get the brief of node by path in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param root_id: int. Example: 1234.
+        :param path: str. Example: "1/2.jpg".
+        :param simplified_meta: (optional) bool. Just basic meta, lower bandwidth consumption.
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "get-node-brief-by-path")
+
+        path = path.replace('\\', '/')
+        req_payload = {
+            "root_id": root_id,
+            "path": [path],
+            "meta": _node_query_metas(simplified_meta)
+        }
+        return self._make_api_request(url, req_payload)
+
+    def depot_delete_node_by_ids(self, asset_hub, ids):
+        r"""delete the node in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param ids: list<int>. Example: [1234].
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "delete-node-by-id")
+        req_payload = {
+            "ids": ids
+        }
+        return self._make_api_request(url, req_payload)
+
+    def depot_move_node(self, asset_hub, ids, other_parent_id):
+        r"""move the node in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param ids: list<int>. Example: [1234, 3456].
+        :param other_parent_id: int.
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "move-node")
+        req_payload = {
+            "ids": ids,
+            "other_parent_id": other_parent_id
+        }
+        return self._make_api_request(url, req_payload)
+
+    def depot_create_project(self, asset_hub, name, parent_id, return_existing_id=True, show_detail_column=True,
+                             show_version_column=True,
+                             watermark=False):
+        r"""create project in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param name: str. project name. Example: "test".
+        :param parent_id: int. depot root id. Example: 304942678017.
+        :param return_existing_id: (optional) bool.
+        :param show_detail_column: (optional) bool.
+        :param show_version_column: (optional) bool.
+        :param watermark: (optional) bool.
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "create-project")
+        req_payload = [{
+            "name": name,
+            "parent_id": parent_id,
+            "return_existing_id": return_existing_id,
+            "show_detail_column": show_detail_column,
+            "show_version_column": show_version_column,
+            "watermark": watermark,
+        }]
+
+        res = self._make_api_request(url, req_payload)
+        res.set_direct_result_by_key("id")
+        return res
+
+    def depot_create_directory(self, asset_hub, payloads):
+        r"""create dirs in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param payloads: list<payload (dict) >.
+                {
+                    "parent_id": parent dir id,
+                    "name": name of new dir to create,
+                    "allowed_rename": allow renaming new dir to "name(<index>)" when a dir with the same name exists,
+                    "return_existing_id": returns the id of an existing dir with the same name
+                }
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "create-directory")
+        req_payload = {
+            "items": payloads
+        }
+
+        res = self._make_api_request(url, req_payload)
+        res.set_direct_result_by_key("id")
+        return res
+
+    def depot_create_asset(self, asset_hub, payloads):
+        r"""create assets in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param payloads: list<payload (dict) >.
+                {
+                    "parent_id": parent dir id,
+                    "name": name of new asset to create,
+                    "add_new_version": add a version when an asset with the same name exists,
+                }
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "create-asset")
+        req_payload = {
+            "items": payloads
+        }
+        res = self._make_api_request(url, req_payload)
+        res.set_direct_result_by_key("id")
+        return res
+
+    def depot_create_multi_asset(self, asset_hub, payloads):
+        r"""create multi asset (version container) in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param payloads: list<payload (dict) >.
+                {
+                    "parent_id": parent dir id,
+                    "name": name of new multi asset to create,
+                }
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "create-multi-asset")
+        req_payload = {
+            "items": payloads
+        }
+        return self._make_api_request(url, req_payload)
+
+    def depot_update_asset_by_id(self, asset_hub, payloads):
+        r"""update metas of asset in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param payloads: list<payload (dict) >.
+                {
+                    "id": int, node id,
+                    "name": str, node name,
+                    "origin_url": origin url,
+                    "description": description of node
+                }
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "update-asset-by-id")
+        req_payload = {
+            "items": payloads
+        }
+        return self._make_api_request(url, req_payload)
+
+    def depot_convert_asset(self, asset_hub, asset_files, asset_ids):
+        r"""convert asset in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param asset_files: list<str>. Example: ["//ahs_cos_guangzhou_1/assethub-trial-1258344700/cospri/download/110347249345/110347249345067/1.png"].
+        :param asset_ids: list<int>. Example: [110347249345067].
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "convert-asset")
+        req_payload = {
+            "asset_files": asset_files,
+            "asset_ids": asset_ids
+        }
+        return self._make_api_request(url, req_payload)
+
+    def depot_create_tsa(self, asset_hub, asset_id, company, description, title, tsa_info):
+        r"""convert asset in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param asset_id: int. Example: 110347249345071.
+        :param company: str. Example: "Tencent".
+        :param description: str. Example: "New weapon".
+        :param title: str. Example: "Christmas".
+        :param tsa_info: str. Example: "Characters; Web design".
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "create-tsa")
+        req_payload = {
+            "asset_id": asset_id,
+            "company": company,
+            "description": description,
+            "title": title,
+            "tsa_info": tsa_info
+        }
+        return self._make_api_request(url, req_payload)
+
+    def depot_add_asset_tag(self, asset_hub, asset_id, tag_name):
+        r"""add tags to asset node in depot.
+
+        :param asset_hub: str. Example: "trial".
+        :param asset_id: int. Example: 110347249345071.
+        :param tag_name: list<str>. Example: ["tag_1", "tag_2"].
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "add-asset-tag")
+        req_payload = {
+            "asset_id": asset_id,
+            "tag_name": tag_name
+        }
+        return self._make_api_request(url, req_payload)
+
+    def depot_update_directory_by_id(self, asset_hub, payloads):
+        r"""update metas of directory in depot .
+
+        :param asset_hub: str. Example: "trial".
+        :param payloads: list<payload (dict) >.
+                {
+                    "id": int, node id,
+                    "name": str, node name,
+                    "origin_url": origin url,
+                    "description": description of node
+                }
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "update-directory-by-id")
+        req_payload = {
+            "items": payloads
+        }
+        return self._make_api_request(url, req_payload)
+
+    def depot_update_project_by_id(self, asset_hub, payloads):
+        r"""update metas of project in depot .
+
+        :param asset_hub: str. Example: "trial".
+        :param payloads: list<payload (dict) >.
+                {
+                    "id": int, node id,
+                    "name": str, node name,
+                    "origin_url": origin url,
+                    "description": description of node
+                }
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "update-project-by-id")
+        req_payload = {
+            "items": payloads
+        }
+        return self._make_api_request(url, req_payload)
+
+    def depot_update_multi_asset_by_id(self, asset_hub, payloads):
+        r"""update metas of multi asset in depot .
+
+        :param asset_hub: str. Example: "trial".
+        :param payloads: list<payload (dict) >.
+                {
+                    "id": int, node id,
+                    "name": str, node name,
+                    "origin_url": origin url,
+                    "description": description of node
+                }
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "update-multi-asset-by-id")
+        req_payload = {
+            "items": payloads
+        }
+        return self._make_api_request(url, req_payload)
+
+    def depot_get_root_id(self, asset_hub):
+        r"""get the depot root id of asset hub.
+
+        :param asset_hub: str. Example: "trial".
+        :rtype: arthub_api.APIResponse
+        """
+
+        url = self._depot_url(asset_hub, "get-depot-id")
+        return self._make_api_request(url)
+
+    # blade
+    def blade_get_account_if_exist(self, user_name):
+        r"""get the account detail by user name.
+
+        :param user_name: str. Example: "joeyding".
+        :rtype: arthub_api.APIResponse
+                result: {
+                    "nick_name": string,
+                    "email": string,
+                    "company": string,
+                    "department": string,
+                    ...}
+        """
+
+        url = self._blade_url("get-account-if-exist")
+        req_payload = {
+            "account_name": user_name
+        }
+        res = self._make_api_request(url, req_payload)
+        res.set_result(res.first_result())
+        return res
+
+    def reset_config(self, config):
+        self._config = config
```

### Comparing `arthub_api-1.5.0/arthub_api/storage.py` & `arthub_api-1.5.1/arthub_api/storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.5.0/arthub_api/utils.py` & `arthub_api-1.5.1/arthub_api/utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,279 +1,279 @@
-"""
-arthub_api.utils
-~~~~~~~~~~~~~~
-
-This module provides utilities that are used within API
-"""
-import logging
-import os
-import shutil
-import time
-import random
-import string
-import requests
-from . import models
-from platformdirs import user_cache_dir
-
-
-def _path_preprocess(path):
-    path = path.strip()
-    path = path.rstrip("\\/")
-    return path
-
-
-def create_empty_file(path):
-    try:
-        open(path, "w").close()
-        return True
-    except Exception:
-        return False
-
-
-def mkdir(path):
-    path = _path_preprocess(path)
-    if os.path.isdir(path):
-        return True
-    if os.path.isfile(path):
-        return False
-    try:
-        os.makedirs(path)
-    except Exception as e:
-        return False
-    return True
-
-
-def remove(path):
-    path = _path_preprocess(path)
-    if not os.path.exists(path):
-        return True
-    try:
-        if os.path.isfile(path):
-            os.remove(path)
-        elif os.path.isdir(path):
-            shutil.rmtree(path)
-    except Exception as e:
-        return False
-    return True
-
-
-def current_milli_time():
-    return (lambda: int(round(time.time() * 1000)))()
-
-
-def get_random_string(length):
-    return ''.join(random.sample(string.ascii_letters + string.digits, length))
-
-
-class UploadFilePartReader(object):
-    def __init__(self, file_, offset, length):
-        self._file = file_
-        self._file.seek(offset)
-        self._total_size = length
-        self._completed_size = 0
-        self._finished = False
-
-    def read(self, size=-1):
-        if size == -1:
-            self._finished = True
-            return ""
-        uncompleted_size = self._total_size - self._completed_size
-        size_to_read = min(uncompleted_size, size)
-        if size_to_read == 0:
-            self._finished = True
-            return ""
-        content = self._file.read(size_to_read)
-        self._completed_size += len(content)
-        return content
-
-
-def upload_part_of_file(url, file_path, offset, length):
-    try:
-        if not os.path.isfile(file_path):
-            return models.Result(False, error_message="file \"%s\" not exist" % file_path)
-        with open(file_path, 'rb') as file_:
-            res = requests.put(url, data=UploadFilePartReader(file_, offset, length), headers={
-                "Accept": "application/json",
-                "Accept-Encoding": "gzip, deflate, br",
-                "Connection": "keep-alive",
-                "Content-Type": "application/octet-stream",
-                "Content-Length": str(length)
-            })
-            if not res.ok:
-                return models.Result(False, error_message="status code: %d" % res.status_code)
-            return models.Result(True, data=res)
-    except Exception as e:
-        error_message = "send request \"%s\" exception" % url
-        logging.error("[UploadFilePart] %s" % error_message)
-        return models.Result(False, error_message=error_message)
-
-
-class UploadFileReader(object):
-    def __init__(self, file_):
-        self._file = file_
-        self._file.seek(0)
-        self._completed_size = 0
-        self._finished = False
-
-    def read(self, size=-1):
-        if size == -1:
-            self._finished = True
-            return ""
-        content = self._file.read(size)
-        self._completed_size += len(content)
-        return content
-
-
-def upload_file(url, file_path):
-    try:
-        if not os.path.isfile(file_path):
-            return models.Result(False, error_message="file \"%s\" not exist" % file_path)
-        with open(file_path, 'rb') as file_:
-            res = requests.put(url, data=UploadFileReader(file_), headers={
-                "Accept-Encoding": "gzip, deflate, br",
-                "Connection": "keep-alive",
-                "Content-Type": "application/octet-stream",
-                "Content-Length": str(os.path.getsize(file_path))
-            })
-            if not res.ok:
-                return models.Result(False, error_message="status code: %d" % res.status_code)
-            return models.Result(True, data=res)
-    except Exception as e:
-        error_message = "send request \"%s\" exception" % url
-        logging.error("[UploadFile] %s" % error_message)
-        return models.Result(False, error_message=error_message)
-
-
-def download_file(url, file_path):
-    try:
-        if os.path.exists(file_path):
-            remove(file_path)
-
-        if not create_empty_file(file_path):
-            return models.Result(False, error_message="create \"%s\" failed" % file_path)
-
-        # download file
-        download_dir_path = os.path.dirname(file_path)
-        if not mkdir(download_dir_path):
-            return models.Result(False, error_message="create directory \"%s\" failed" % download_dir_path)
-
-        res_download = requests.get(url, stream=True)
-
-        if not res_download:
-            return models.Result(False, error_message="request \"%s\" failed" % url)
-        with open(file_path, "ab") as f:
-            for chunk in res_download.iter_content(chunk_size=1024):
-                f.write(chunk)
-                f.flush()
-
-        return models.Result(True)
-
-    except Exception as e:
-        return models.Result(False, error_message=e)
-
-
-def splite_path(path_):
-    path_list = []
-    while path_:
-        l = os.path.split(path_)
-        path_ = l[0]
-        if l[1]:
-            path_list.insert(0, l[1])
-    return path_list
-
-
-def rename_path_text(path_):
-    path_ = _path_preprocess(path_)
-    path_without_ext, ext = os.path.splitext(path_)
-    suffix_number = 1
-    while os.path.exists(path_):
-        path_ = "%s (%d)%s" % (path_without_ext, suffix_number, ext)
-        suffix_number += 1
-    return path_
-
-
-def parse_cookies(cookie_str):
-    cookies = {}
-    cookie_strs = cookie_str.split(';')
-    for _item in cookie_strs:
-        _item = _item.strip()
-        _pair = _item.split('=')
-        if len(_pair) == 2:
-            cookies[_pair[0]] = _pair[1]
-    return cookies
-
-
-def rename_path(src, dest):
-    if not mkdir(os.path.dirname(dest)):
-        return False
-    if os.path.exists(dest):
-        remove(dest)
-    try:
-        os.rename(src, dest)
-    except Exception:
-        return False
-    return True
-
-
-def count_files(root_path):
-    total_files = 0
-    if not os.path.exists(root_path):
-        return total_files
-    item_list = os.listdir(root_path)
-    if len(item_list) == 0:
-        return total_files
-    for item in item_list:
-        next_path = os.path.join(root_path, item)
-        if os.path.isfile(next_path):
-            total_files += 1
-        else:
-            total_files += count_files(next_path)
-    return total_files
-
-
-def read_file(file_path):
-    with open(file_path, "r") as file_obj:
-        return file_obj.read()
-
-
-def write_file(file_path, data):
-    with open(file_path, "w") as file_obj:
-        file_obj.write(data)
-
-
-def get_cache_dir(api_host):
-    root = user_cache_dir(appname="arthub", opinion=False)
-    d = os.path.join(root, api_host)
-    try:
-        os.makedirs(d)
-    except (IOError, WindowsError):
-        pass
-    return d
-
-
-def get_token_cache_file(api_host):
-    root = get_cache_dir(api_host)
-    return os.path.join(root, "arthub_token")
-
-
-def get_token_from_cache(api_host):
-    token_file = get_token_cache_file(api_host)
-    try:
-        if os.path.exists(token_file):
-            return read_file(token_file)
-    except (IOError, WindowsError) as e:
-        logging.warning("[TokenCache] get token from file \"%s\" error: %s",
-                        token_file, str(e))
-    return ""
-
-
-def save_token_to_cache(token, api_host):
-    token_file = get_token_cache_file(api_host)
-    try:
-        write_file(token_file, token)
-    except (IOError, WindowsError) as e:
-        logging.warning("[TokenCache] save token to file \"%s\" error: %s",
-                        token_file, str(e))
-
-
-def remove_token_cache_file(api_host):
-    remove(get_token_cache_file(api_host))
+"""
+arthub_api.utils
+~~~~~~~~~~~~~~
+
+This module provides utilities that are used within API
+"""
+import logging
+import os
+import shutil
+import time
+import random
+import string
+import requests
+from . import models
+from platformdirs import user_cache_dir
+
+
+def _path_preprocess(path):
+    path = path.strip()
+    path = path.rstrip("\\/")
+    return path
+
+
+def create_empty_file(path):
+    try:
+        open(path, "w").close()
+        return True
+    except Exception:
+        return False
+
+
+def mkdir(path):
+    path = _path_preprocess(path)
+    if os.path.isdir(path):
+        return True
+    if os.path.isfile(path):
+        return False
+    try:
+        os.makedirs(path)
+    except Exception as e:
+        return False
+    return True
+
+
+def remove(path):
+    path = _path_preprocess(path)
+    if not os.path.exists(path):
+        return True
+    try:
+        if os.path.isfile(path):
+            os.remove(path)
+        elif os.path.isdir(path):
+            shutil.rmtree(path)
+    except Exception as e:
+        return False
+    return True
+
+
+def current_milli_time():
+    return (lambda: int(round(time.time() * 1000)))()
+
+
+def get_random_string(length):
+    return ''.join(random.sample(string.ascii_letters + string.digits, length))
+
+
+class UploadFilePartReader(object):
+    def __init__(self, file_, offset, length):
+        self._file = file_
+        self._file.seek(offset)
+        self._total_size = length
+        self._completed_size = 0
+        self._finished = False
+
+    def read(self, size=-1):
+        if size == -1:
+            self._finished = True
+            return ""
+        uncompleted_size = self._total_size - self._completed_size
+        size_to_read = min(uncompleted_size, size)
+        if size_to_read == 0:
+            self._finished = True
+            return ""
+        content = self._file.read(size_to_read)
+        self._completed_size += len(content)
+        return content
+
+
+def upload_part_of_file(url, file_path, offset, length):
+    try:
+        if not os.path.isfile(file_path):
+            return models.Result(False, error_message="file \"%s\" not exist" % file_path)
+        with open(file_path, 'rb') as file_:
+            res = requests.put(url, data=UploadFilePartReader(file_, offset, length), headers={
+                "Accept": "application/json",
+                "Accept-Encoding": "gzip, deflate, br",
+                "Connection": "keep-alive",
+                "Content-Type": "application/octet-stream",
+                "Content-Length": str(length)
+            })
+            if not res.ok:
+                return models.Result(False, error_message="status code: %d" % res.status_code)
+            return models.Result(True, data=res)
+    except Exception as e:
+        error_message = "send request \"%s\" exception" % url
+        logging.error("[UploadFilePart] %s" % error_message)
+        return models.Result(False, error_message=error_message)
+
+
+class UploadFileReader(object):
+    def __init__(self, file_):
+        self._file = file_
+        self._file.seek(0)
+        self._completed_size = 0
+        self._finished = False
+
+    def read(self, size=-1):
+        if size == -1:
+            self._finished = True
+            return ""
+        content = self._file.read(size)
+        self._completed_size += len(content)
+        return content
+
+
+def upload_file(url, file_path):
+    try:
+        if not os.path.isfile(file_path):
+            return models.Result(False, error_message="file \"%s\" not exist" % file_path)
+        with open(file_path, 'rb') as file_:
+            res = requests.put(url, data=UploadFileReader(file_), headers={
+                "Accept-Encoding": "gzip, deflate, br",
+                "Connection": "keep-alive",
+                "Content-Type": "application/octet-stream",
+                "Content-Length": str(os.path.getsize(file_path))
+            })
+            if not res.ok:
+                return models.Result(False, error_message="status code: %d" % res.status_code)
+            return models.Result(True, data=res)
+    except Exception as e:
+        error_message = "send request \"%s\" exception" % url
+        logging.error("[UploadFile] %s" % error_message)
+        return models.Result(False, error_message=error_message)
+
+
+def download_file(url, file_path):
+    try:
+        if os.path.exists(file_path):
+            remove(file_path)
+
+        if not create_empty_file(file_path):
+            return models.Result(False, error_message="create \"%s\" failed" % file_path)
+
+        # download file
+        download_dir_path = os.path.dirname(file_path)
+        if not mkdir(download_dir_path):
+            return models.Result(False, error_message="create directory \"%s\" failed" % download_dir_path)
+
+        res_download = requests.get(url, stream=True)
+
+        if not res_download:
+            return models.Result(False, error_message="request \"%s\" failed" % url)
+        with open(file_path, "ab") as f:
+            for chunk in res_download.iter_content(chunk_size=1024):
+                f.write(chunk)
+                f.flush()
+
+        return models.Result(True)
+
+    except Exception as e:
+        return models.Result(False, error_message=e)
+
+
+def splite_path(path_):
+    path_list = []
+    while path_:
+        l = os.path.split(path_)
+        path_ = l[0]
+        if l[1]:
+            path_list.insert(0, l[1])
+    return path_list
+
+
+def rename_path_text(path_):
+    path_ = _path_preprocess(path_)
+    path_without_ext, ext = os.path.splitext(path_)
+    suffix_number = 1
+    while os.path.exists(path_):
+        path_ = "%s (%d)%s" % (path_without_ext, suffix_number, ext)
+        suffix_number += 1
+    return path_
+
+
+def parse_cookies(cookie_str):
+    cookies = {}
+    cookie_strs = cookie_str.split(';')
+    for _item in cookie_strs:
+        _item = _item.strip()
+        _pair = _item.split('=')
+        if len(_pair) == 2:
+            cookies[_pair[0]] = _pair[1]
+    return cookies
+
+
+def rename_path(src, dest):
+    if not mkdir(os.path.dirname(dest)):
+        return False
+    if os.path.exists(dest):
+        remove(dest)
+    try:
+        os.rename(src, dest)
+    except Exception:
+        return False
+    return True
+
+
+def count_files(root_path):
+    total_files = 0
+    if not os.path.exists(root_path):
+        return total_files
+    item_list = os.listdir(root_path)
+    if len(item_list) == 0:
+        return total_files
+    for item in item_list:
+        next_path = os.path.join(root_path, item)
+        if os.path.isfile(next_path):
+            total_files += 1
+        else:
+            total_files += count_files(next_path)
+    return total_files
+
+
+def read_file(file_path):
+    with open(file_path, "r") as file_obj:
+        return file_obj.read()
+
+
+def write_file(file_path, data):
+    with open(file_path, "w") as file_obj:
+        file_obj.write(data)
+
+
+def get_cache_dir(api_host):
+    root = user_cache_dir(appname="arthub", opinion=False)
+    d = os.path.join(root, api_host)
+    try:
+        os.makedirs(d)
+    except (IOError, WindowsError):
+        pass
+    return d
+
+
+def get_token_cache_file(api_host):
+    root = get_cache_dir(api_host)
+    return os.path.join(root, "arthub_token")
+
+
+def get_token_from_cache(api_host):
+    token_file = get_token_cache_file(api_host)
+    try:
+        if os.path.exists(token_file):
+            return read_file(token_file)
+    except (IOError, WindowsError) as e:
+        logging.warning("[TokenCache] get token from file \"%s\" error: %s",
+                        token_file, str(e))
+    return ""
+
+
+def save_token_to_cache(token, api_host):
+    token_file = get_token_cache_file(api_host)
+    try:
+        write_file(token_file, token)
+    except (IOError, WindowsError) as e:
+        logging.warning("[TokenCache] save token to file \"%s\" error: %s",
+                        token_file, str(e))
+
+
+def remove_token_cache_file(api_host):
+    remove(get_token_cache_file(api_host))
```

### Comparing `arthub_api-1.5.0/arthub_api.egg-info/SOURCES.txt` & `arthub_api-1.5.1/arthub_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arthub_api-1.5.0/setup.py` & `arthub_api-1.5.1/setup.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-#!/usr/bin/env python
-import os
-import sys
-from codecs import open
-
-from setuptools import setup, find_packages
-from setuptools.command.test import test as TestCommand
-
-
-# CURRENT_PYTHON = sys.version_info[:2]
-# REQUIRED_PYTHON = (3, 7)
-
-# if CURRENT_PYTHON < REQUIRED_PYTHON:
-#     sys.stderr.write("""
-# ==========================
-# Unsupported Python version
-# ==========================
-# This version of arthub_api requires at least Python {}.{}, but
-# you're trying to install it on Python {}.{}. To resolve this,
-# consider upgrading to a supported Python version.
-# """.format(*(REQUIRED_PYTHON + CURRENT_PYTHON)))
-#     sys.exit(1)
-
-
-class PyTest(TestCommand):
-    user_options = [("pytest-args=", "a", "Arguments to pass into py.test")]
-
-    def initialize_options(self):
-        TestCommand.initialize_options(self)
-        try:
-            from multiprocessing import cpu_count
-
-            self.pytest_args = ["-n", str(cpu_count()), "--boxed"]
-        except (ImportError, NotImplementedError):
-            self.pytest_args = ["-n", "1", "--boxed"]
-
-    def finalize_options(self):
-        TestCommand.finalize_options(self)
-        self.test_args = []
-        self.test_suite = True
-
-    def run_tests(self):
-        import pytest
-
-        errno = pytest.main(self.pytest_args)
-        sys.exit(errno)
-
-
-# 'setup.py publish' shortcut.
-if sys.argv[-1] == "publish":
-    os.system("python setup.py sdist bdist_wheel")
-    os.system("twine upload dist/*")
-    sys.exit()
-
-requires = [
-    "requests",
-    "platformdirs==2.0.2"
-]
-
-test_requirements = [
-    "pytest",
-]
-
-about = {}
-here = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(here, "arthub_api", "__version__.py"), "r",
-          "utf-8") as f:
-    exec(f.read(), about)
-
-with open("README.md", "r", "utf-8") as f:
-    readme = f.read()
-
-setup(name=about["__title__"],
-      version=about["__version__"],
-      description=about["__description__"],
-      long_description=readme,
-      long_description_content_type="text/markdown",
-      author=about["__author__"],
-      author_email=about["__author_email__"],
-      url=about["__url__"],
-      package_dir={'arthub_api': 'arthub_api'},
-      packages=['arthub_api'],
-      package_data={"": ["LICENSE", "NOTICE"]},
-      include_package_data=True,
-      install_requires=requires,
-      license=about["__license__"],
-      zip_safe=False,
-      classifiers=[
-          "Development Status :: 5 - Production/Stable",
-          "Environment :: Web Environment",
-          "Intended Audience :: Developers",
-          "Natural Language :: English",
-          "Operating System :: OS Independent"],
-      cmdclass={"test": PyTest},
-      tests_require=test_requirements,
-      entry_points={
-          "console_scripts": [
-              "aha = arthub_api.__main__:main",
-          ]
-      })
+#!/usr/bin/env python
+import os
+import sys
+from codecs import open
+
+from setuptools import setup, find_packages
+from setuptools.command.test import test as TestCommand
+
+
+# CURRENT_PYTHON = sys.version_info[:2]
+# REQUIRED_PYTHON = (3, 7)
+
+# if CURRENT_PYTHON < REQUIRED_PYTHON:
+#     sys.stderr.write("""
+# ==========================
+# Unsupported Python version
+# ==========================
+# This version of arthub_api requires at least Python {}.{}, but
+# you're trying to install it on Python {}.{}. To resolve this,
+# consider upgrading to a supported Python version.
+# """.format(*(REQUIRED_PYTHON + CURRENT_PYTHON)))
+#     sys.exit(1)
+
+
+class PyTest(TestCommand):
+    user_options = [("pytest-args=", "a", "Arguments to pass into py.test")]
+
+    def initialize_options(self):
+        TestCommand.initialize_options(self)
+        try:
+            from multiprocessing import cpu_count
+
+            self.pytest_args = ["-n", str(cpu_count()), "--boxed"]
+        except (ImportError, NotImplementedError):
+            self.pytest_args = ["-n", "1", "--boxed"]
+
+    def finalize_options(self):
+        TestCommand.finalize_options(self)
+        self.test_args = []
+        self.test_suite = True
+
+    def run_tests(self):
+        import pytest
+
+        errno = pytest.main(self.pytest_args)
+        sys.exit(errno)
+
+
+# 'setup.py publish' shortcut.
+if sys.argv[-1] == "publish":
+    os.system("python setup.py sdist bdist_wheel")
+    os.system("twine upload dist/*")
+    sys.exit()
+
+requires = [
+    "requests",
+    "platformdirs==2.0.2"
+]
+
+test_requirements = [
+    "pytest",
+]
+
+about = {}
+here = os.path.abspath(os.path.dirname(__file__))
+with open(os.path.join(here, "arthub_api", "__version__.py"), "r",
+          "utf-8") as f:
+    exec(f.read(), about)
+
+with open("README.md", "r", "utf-8") as f:
+    readme = f.read()
+
+setup(name=about["__title__"],
+      version=about["__version__"],
+      description=about["__description__"],
+      long_description=readme,
+      long_description_content_type="text/markdown",
+      author=about["__author__"],
+      author_email=about["__author_email__"],
+      url=about["__url__"],
+      package_dir={'arthub_api': 'arthub_api'},
+      packages=['arthub_api'],
+      package_data={"": ["LICENSE", "NOTICE"]},
+      include_package_data=True,
+      install_requires=requires,
+      license=about["__license__"],
+      zip_safe=False,
+      classifiers=[
+          "Development Status :: 5 - Production/Stable",
+          "Environment :: Web Environment",
+          "Intended Audience :: Developers",
+          "Natural Language :: English",
+          "Operating System :: OS Independent"],
+      cmdclass={"test": PyTest},
+      tests_require=test_requirements,
+      entry_points={
+          "console_scripts": [
+              "aha = arthub_api.__main__:main",
+          ]
+      })
```

### Comparing `arthub_api-1.5.0/tests/test_open_api.py` & `arthub_api-1.5.1/tests/test_open_api.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,213 +1,213 @@
-import arthub_api
-import pytest
-import logging
-from arthub_api import arthub_api_config
-from arthub_api import (
-    OpenAPI,
-    api_config_qq,
-    api_config_oa_test
-)
-
-TEST_DEPOT_NAME = "apg"
-
-open_api = OpenAPI(api_config_qq)
-
-
-def on_api_failed(res):
-    logging.error("[TEST][API] \"%s\" failed, error: %s" % (res.url, res.error_message()))
-
-
-@pytest.mark.run(order=1)
-def test_login():
-    res = open_api.login(arthub_api_config.account_email, arthub_api_config.password)
-    if not res.is_succeeded():
-        on_api_failed(res)
-        pytest.exit("login failed, exit test", returncode=1)
-
-    logging.info("[TEST][API] \"%s\" success, token: %s" % (res.url, res.results.get(0)["arthub_token"]))
-
-
-@pytest.mark.run(order=2)
-def test_token_cache():
-    # use cache
-    open_api_new = OpenAPI(api_config_qq)
-    assert open_api_new.is_login()
-    assert open_api_new.get_account_email() == open_api.get_account_email()
-    assert open_api_new.token == open_api.token
-    # log out
-    open_api_new.logout()
-    assert not open_api_new.is_login()
-    open_api_new_2 = OpenAPI(api_config_qq)
-    assert not open_api_new_2.is_login()
-
-
-def test_depot_get_root_id():
-    res = open_api.depot_get_root_id(TEST_DEPOT_NAME)
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, depot id: %d" % (res.url, res.results.get(0)))
-
-
-def test_depot_get_node_brief_by_ids():
-    res = open_api.depot_get_node_brief_by_ids(TEST_DEPOT_NAME, [120347220059298, 120347220059299])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    node_1 = res.results.get(0)
-    node_2 = res.results.get(1)
-    logging.info("[TEST][API] \"%s\" success, name_1: %s, name_2: %s" % (res.url, node_1["name"], node_2["name"]))
-
-
-def test_depot_get_child_node_count():
-    res = open_api.depot_get_child_node_count(TEST_DEPOT_NAME, [120347220059339])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, count: %d" % (res.url, res.results.get(0)["count"]))
-
-
-def test_depot_get_download_signature():
-    res = open_api.depot_get_download_signature(TEST_DEPOT_NAME,
-                                                nodes=[{"object_id": 120347220059338, "object_meta": "origin_url"}])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, signed url: %s" % (res.url, res.results.get(0)["signed_url"]))
-
-
-def test_depot_get_upload_signature():
-    file_name = "new_asset_to_upload"
-    res_0 = open_api.depot_create_asset(TEST_DEPOT_NAME, [{
-        "parent_id": 120347220059339,
-        "name": file_name,
-        "add_new_version": False
-    }])
-    if not res_0.is_succeeded():
-        on_api_failed(res_0)
-        assert 0
-
-    asset_id = res_0.results.get(0)["id"]
-
-    res_1 = open_api.depot_get_upload_signature(TEST_DEPOT_NAME, nodes=[
-        {"object_id": asset_id, "object_meta": "origin_url", "file_name": file_name}])
-    if not res_1.is_succeeded():
-        on_api_failed(res_1)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, signed url: %s" % (res_1.url, res_1.results.get(0)["signed_url"]))
-
-
-def test_depot_get_child_node_id_in_range():
-    res = open_api.depot_get_child_node_id_in_range(TEST_DEPOT_NAME, parent_id=120347220059339, offset=0, count=2,
-                                                    query_filters=[{"meta": "type", "condition": "x != directory"}],
-                                                    is_recursive=True)
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    nodes = res.results.get(0)["nodes"]
-    logging.info("[TEST][API] \"%s\" success" % res.url)
-
-
-def test_depot_get_node_brief_by_path():
-    res = open_api.depot_get_node_brief_by_path(TEST_DEPOT_NAME, root_id=120347220059296, path="open_api_test/asset.jpg")
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    node = res.results.get(0)
-    logging.info("[TEST][API] \"%s\" success, name: %s" % (res.url, node["name"]))
-
-
-def test_depot_add_asset_tag():
-    res = open_api.depot_add_asset_tag(TEST_DEPOT_NAME, asset_id=120347220059344, tag_name=["tag_1", "tag_2"])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    node = res.results.get(0)
-    logging.info("[TEST][API] \"%s\" success, tag id: %d" % (res.url, node))
-
-
-def test_get_account_detail():
-    res = open_api.get_account_detail()
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, email: %s" % (res.url, res.results.get(0)["email"]))
-
-
-def test_get_ticket():
-    res = open_api.get_ticket()
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, ticket: %s" % (res.url, res.results.get(0)))
-
-
-def test_get_last_access_location_by_account():
-    res = open_api.get_last_access_location_by_account()
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, last access location: %s" % (res.url, res.results.get(0)))
-
-
-def test_depot_create_directory():
-    res = open_api.depot_create_directory(TEST_DEPOT_NAME, [{
-        "parent_id": 120347220059339,
-        "name": "new_dir",
-        "allowed_rename": True,
-        "return_existing_id": False
-    }])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, new dir id: %s" % (res.url, res.results.get(0)["id"]))
-
-
-def test_depot_create_multi_asset():
-    res = open_api.depot_create_multi_asset(TEST_DEPOT_NAME, [{
-        "parent_id": 120347220059339,
-        "name": "new_multi_asset"
-    }])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, new multi asset id: %s" % (res.url, res.results.get(0)["id"]))
-
-
-def test_depot_move_node():
-    res = open_api.depot_move_node(TEST_DEPOT_NAME, ids=[120347220064827], other_parent_id=120347220064825)
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success" % res.url)
-
-
-def test_blade_get_account_if_exist():
-    open_api_test = OpenAPI(api_config_oa_test)
-    res = open_api_test.blade_get_account_if_exist("joeyding")
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-    assert res.result.get("email") == "joeyding@tencent.com"
-    logging.info("[TEST][API] \"%s\" success" % res.url)
-
-
-def test_blade_get_account_if_not_exist():
-    open_api_test = OpenAPI(api_config_oa_test)
-    res = open_api_test.blade_get_account_if_exist("joeyd123")
-    assert (not res.is_succeeded()) and (res.is_account_not_exist())
-    logging.info("[TEST][API] \"%s\" success" % res.url)
+import arthub_api
+import pytest
+import logging
+from arthub_api import arthub_api_config
+from arthub_api import (
+    OpenAPI,
+    api_config_qq,
+    api_config_oa_test
+)
+
+TEST_DEPOT_NAME = "apg"
+
+open_api = OpenAPI(api_config_qq)
+
+
+def on_api_failed(res):
+    logging.error("[TEST][API] \"%s\" failed, error: %s" % (res.url, res.error_message()))
+
+
+@pytest.mark.run(order=1)
+def test_login():
+    res = open_api.login(arthub_api_config.account_email, arthub_api_config.password)
+    if not res.is_succeeded():
+        on_api_failed(res)
+        pytest.exit("login failed, exit test", returncode=1)
+
+    logging.info("[TEST][API] \"%s\" success, token: %s" % (res.url, res.results.get(0)["arthub_token"]))
+
+
+@pytest.mark.run(order=2)
+def test_token_cache():
+    # use cache
+    open_api_new = OpenAPI(api_config_qq)
+    assert open_api_new.is_login()
+    assert open_api_new.get_account_email() == open_api.get_account_email()
+    assert open_api_new.token == open_api.token
+    # log out
+    open_api_new.logout()
+    assert not open_api_new.is_login()
+    open_api_new_2 = OpenAPI(api_config_qq)
+    assert not open_api_new_2.is_login()
+
+
+def test_depot_get_root_id():
+    res = open_api.depot_get_root_id(TEST_DEPOT_NAME)
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, depot id: %d" % (res.url, res.results.get(0)))
+
+
+def test_depot_get_node_brief_by_ids():
+    res = open_api.depot_get_node_brief_by_ids(TEST_DEPOT_NAME, [120347220059298, 120347220059299])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    node_1 = res.results.get(0)
+    node_2 = res.results.get(1)
+    logging.info("[TEST][API] \"%s\" success, name_1: %s, name_2: %s" % (res.url, node_1["name"], node_2["name"]))
+
+
+def test_depot_get_child_node_count():
+    res = open_api.depot_get_child_node_count(TEST_DEPOT_NAME, [120347220059339])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, count: %d" % (res.url, res.results.get(0)["count"]))
+
+
+def test_depot_get_download_signature():
+    res = open_api.depot_get_download_signature(TEST_DEPOT_NAME,
+                                                nodes=[{"object_id": 120347220059338, "object_meta": "origin_url"}])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, signed url: %s" % (res.url, res.results.get(0)["signed_url"]))
+
+
+def test_depot_get_upload_signature():
+    file_name = "new_asset_to_upload"
+    res_0 = open_api.depot_create_asset(TEST_DEPOT_NAME, [{
+        "parent_id": 120347220059339,
+        "name": file_name,
+        "add_new_version": False
+    }])
+    if not res_0.is_succeeded():
+        on_api_failed(res_0)
+        assert 0
+
+    asset_id = res_0.results.get(0)["id"]
+
+    res_1 = open_api.depot_get_upload_signature(TEST_DEPOT_NAME, nodes=[
+        {"object_id": asset_id, "object_meta": "origin_url", "file_name": file_name}])
+    if not res_1.is_succeeded():
+        on_api_failed(res_1)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, signed url: %s" % (res_1.url, res_1.results.get(0)["signed_url"]))
+
+
+def test_depot_get_child_node_id_in_range():
+    res = open_api.depot_get_child_node_id_in_range(TEST_DEPOT_NAME, parent_id=120347220059339, offset=0, count=2,
+                                                    query_filters=[{"meta": "type", "condition": "x != directory"}],
+                                                    is_recursive=True)
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    nodes = res.results.get(0)["nodes"]
+    logging.info("[TEST][API] \"%s\" success" % res.url)
+
+
+def test_depot_get_node_brief_by_path():
+    res = open_api.depot_get_node_brief_by_path(TEST_DEPOT_NAME, root_id=120347220059296, path="open_api_test/asset.jpg")
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    node = res.results.get(0)
+    logging.info("[TEST][API] \"%s\" success, name: %s" % (res.url, node["name"]))
+
+
+def test_depot_add_asset_tag():
+    res = open_api.depot_add_asset_tag(TEST_DEPOT_NAME, asset_id=120347220059344, tag_name=["tag_1", "tag_2"])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    node = res.results.get(0)
+    logging.info("[TEST][API] \"%s\" success, tag id: %d" % (res.url, node))
+
+
+def test_get_account_detail():
+    res = open_api.get_account_detail()
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, email: %s" % (res.url, res.results.get(0)["email"]))
+
+
+def test_get_ticket():
+    res = open_api.get_ticket()
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, ticket: %s" % (res.url, res.results.get(0)))
+
+
+def test_get_last_access_location_by_account():
+    res = open_api.get_last_access_location_by_account()
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, last access location: %s" % (res.url, res.results.get(0)))
+
+
+def test_depot_create_directory():
+    res = open_api.depot_create_directory(TEST_DEPOT_NAME, [{
+        "parent_id": 120347220059339,
+        "name": "new_dir",
+        "allowed_rename": True,
+        "return_existing_id": False
+    }])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, new dir id: %s" % (res.url, res.results.get(0)["id"]))
+
+
+def test_depot_create_multi_asset():
+    res = open_api.depot_create_multi_asset(TEST_DEPOT_NAME, [{
+        "parent_id": 120347220059339,
+        "name": "new_multi_asset"
+    }])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, new multi asset id: %s" % (res.url, res.results.get(0)["id"]))
+
+
+def test_depot_move_node():
+    res = open_api.depot_move_node(TEST_DEPOT_NAME, ids=[120347220064827], other_parent_id=120347220064825)
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success" % res.url)
+
+
+def test_blade_get_account_if_exist():
+    open_api_test = OpenAPI(api_config_oa_test)
+    res = open_api_test.blade_get_account_if_exist("joeyding")
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+    assert res.result.get("email") == "joeyding@tencent.com"
+    logging.info("[TEST][API] \"%s\" success" % res.url)
+
+
+def test_blade_get_account_if_not_exist():
+    open_api_test = OpenAPI(api_config_oa_test)
+    res = open_api_test.blade_get_account_if_exist("joeyd123")
+    assert (not res.is_succeeded()) and (res.is_account_not_exist())
+    logging.info("[TEST][API] \"%s\" success" % res.url)
```

### Comparing `arthub_api-1.5.0/tests/test_storage.py` & `arthub_api-1.5.1/tests/test_storage.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-import os.path
-
-import pytest
-import logging
-from arthub_api import arthub_api_config
-from arthub_api import (
-    OpenAPI,
-    Storage,
-    api_config_qq
-)
-import time
-
-TEST_DEPOT_NAME = "apg"
-
-open_api = OpenAPI(api_config_qq)
-storage = Storage(open_api)
-
-
-def on_api_failed(res):
-    logging.error("[TEST][STORAGE] \"%s\" failed, error: %s" % (res.url, res.error_message()))
-
-
-def on_operation_failed(operation, error_message):
-    logging.error("[TEST][STORAGE] %s failed, error: %s" % (operation, error_message))
-
-
-@pytest.mark.run(order=1)
-def test_login():
-    res = open_api.login(arthub_api_config.account_email, arthub_api_config.password)
-    if not res.is_succeeded():
-        on_api_failed(res)
-        pytest.exit("login failed, exit test", returncode=1)
-
-    logging.info("[TEST][STORAGE] \"%s\" success, token: %s" % (res.url, res.results.get(0)["arthub_token"]))
-
-
-@pytest.mark.run(order=2)
-def test_transfer(tmp_path):
-    # download
-    def download_progress_cb(completed, total):
-        print("download progress: %d/%d" % (completed, total))
-
-    since = time.time()
-    res = storage.download_by_path(asset_hub=TEST_DEPOT_NAME,
-                                   remote_node_path="arthub_api_test/storage_test/download",
-                                   local_dir_path=str(tmp_path),
-                                   same_name_override=False,
-                                   progress_cb=download_progress_cb)
-    if not res.is_succeeded():
-        on_operation_failed("download", res.error_message())
-        assert 0
-    local_downloaded_path = res.data[0]
-    logging.info("[TEST][STORAGE] download success, local downloaded path: %s, spend: %f s"
-                 % (local_downloaded_path, time.time() - since))
-    since = time.time()
-
-    # upload downloaded dir
-    def upload_progress_cb(completed, total):
-        print("upload progress: %d/%d" % (completed, total))
-    res = storage.upload_to_directory_by_path(asset_hub=TEST_DEPOT_NAME,
-                                              remote_dir_path="arthub_api_test/storage_test/upload",
-                                              local_path=local_downloaded_path,
-                                              tags_to_create=["sdk_test"],
-                                              same_name_override=False,
-                                              need_convert=True,
-                                              progress_cb=upload_progress_cb)
-    if not res.is_succeeded():
-        on_operation_failed("upload", res.error_message())
-        assert 0
-    logging.info("[TEST][STORAGE] upload success, remote uploaded id: %d, spend: %f s"
-                 % (res.data[0], time.time() - since))
-
-
-def test_get_node_by_path():
-    res = storage.get_node_by_path(asset_hub=TEST_DEPOT_NAME, remote_node_path="arthub_api_test/storage_test/download")
-    if not res.is_succeeded():
-        on_operation_failed("get remote node info", res.error_message())
-        assert 0
-    logging.info("[TEST][STORAGE] get remote node info success, id: %d, type: %s" % (res.data["id"], res.data["type"]))
-
-
-def test_delete_node_by_path():
-    res = storage.delete_node_by_path(asset_hub=TEST_DEPOT_NAME, remote_node_path="arthub_api_test/storage_test/upload")
-    if not res.is_succeeded():
-        on_operation_failed("delete remote node info", res.error_message())
-        assert 0
-    logging.info("[TEST][STORAGE] delete remote node %d success" % res.data)
+import os.path
+
+import pytest
+import logging
+from arthub_api import arthub_api_config
+from arthub_api import (
+    OpenAPI,
+    Storage,
+    api_config_qq
+)
+import time
+
+TEST_DEPOT_NAME = "apg"
+
+open_api = OpenAPI(api_config_qq)
+storage = Storage(open_api)
+
+
+def on_api_failed(res):
+    logging.error("[TEST][STORAGE] \"%s\" failed, error: %s" % (res.url, res.error_message()))
+
+
+def on_operation_failed(operation, error_message):
+    logging.error("[TEST][STORAGE] %s failed, error: %s" % (operation, error_message))
+
+
+@pytest.mark.run(order=1)
+def test_login():
+    res = open_api.login(arthub_api_config.account_email, arthub_api_config.password)
+    if not res.is_succeeded():
+        on_api_failed(res)
+        pytest.exit("login failed, exit test", returncode=1)
+
+    logging.info("[TEST][STORAGE] \"%s\" success, token: %s" % (res.url, res.results.get(0)["arthub_token"]))
+
+
+@pytest.mark.run(order=2)
+def test_transfer(tmp_path):
+    # download
+    def download_progress_cb(completed, total):
+        print("download progress: %d/%d" % (completed, total))
+
+    since = time.time()
+    res = storage.download_by_path(asset_hub=TEST_DEPOT_NAME,
+                                   remote_node_path="arthub_api_test/storage_test/download",
+                                   local_dir_path=str(tmp_path),
+                                   same_name_override=False,
+                                   progress_cb=download_progress_cb)
+    if not res.is_succeeded():
+        on_operation_failed("download", res.error_message())
+        assert 0
+    local_downloaded_path = res.data[0]
+    logging.info("[TEST][STORAGE] download success, local downloaded path: %s, spend: %f s"
+                 % (local_downloaded_path, time.time() - since))
+    since = time.time()
+
+    # upload downloaded dir
+    def upload_progress_cb(completed, total):
+        print("upload progress: %d/%d" % (completed, total))
+    res = storage.upload_to_directory_by_path(asset_hub=TEST_DEPOT_NAME,
+                                              remote_dir_path="arthub_api_test/storage_test/upload",
+                                              local_path=local_downloaded_path,
+                                              tags_to_create=["sdk_test"],
+                                              same_name_override=False,
+                                              need_convert=True,
+                                              progress_cb=upload_progress_cb)
+    if not res.is_succeeded():
+        on_operation_failed("upload", res.error_message())
+        assert 0
+    logging.info("[TEST][STORAGE] upload success, remote uploaded id: %d, spend: %f s"
+                 % (res.data[0], time.time() - since))
+
+
+def test_get_node_by_path():
+    res = storage.get_node_by_path(asset_hub=TEST_DEPOT_NAME, remote_node_path="arthub_api_test/storage_test/download")
+    if not res.is_succeeded():
+        on_operation_failed("get remote node info", res.error_message())
+        assert 0
+    logging.info("[TEST][STORAGE] get remote node info success, id: %d, type: %s" % (res.data["id"], res.data["type"]))
+
+
+def test_delete_node_by_path():
+    res = storage.delete_node_by_path(asset_hub=TEST_DEPOT_NAME, remote_node_path="arthub_api_test/storage_test/upload")
+    if not res.is_succeeded():
+        on_operation_failed("delete remote node info", res.error_message())
+        assert 0
+    logging.info("[TEST][STORAGE] delete remote node %d success" % res.data)
```

