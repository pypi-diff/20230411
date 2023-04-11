# Comparing `tmp/clipped-0.0.2.tar.gz` & `tmp/clipped-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipped-0.0.2.tar", last modified: Thu Apr  6 15:18:06 2023, max compression
+gzip compressed data, was "clipped-0.0.3.tar", last modified: Tue Apr 11 18:51:24 2023, max compression
```

## Comparing `clipped-0.0.2.tar` & `clipped-0.0.3.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-06 15:18:06.021237 clipped-0.0.2/
--rw-r--r--   0 mourad     (501) staff       (20)      174 2023-04-06 15:16:50.000000 clipped-0.0.2/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-06 15:18:06.021334 clipped-0.0.2/PKG-INFO
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-06 15:18:06.020470 clipped-0.0.2/clipped/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/bool_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/cached_property.py
--rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/click_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/cmd.py
--rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/coroutine.py
--rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/csv_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/date_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     4349 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/deprecated_decorators.py
--rw-r--r--   0 mourad     (501) staff       (20)     3354 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/dict_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/encoding.py
--rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/enums_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     1995 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/env.py
--rw-r--r--   0 mourad     (501) staff       (20)     6222 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/formatting.py
--rw-r--r--   0 mourad     (501) staff       (20)     4731 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/git_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     1825 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/hashing.py
--rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/http_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     3323 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/humanize.py
--rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/imports.py
--rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/indentation.py
--rw-r--r--   0 mourad     (501) staff       (20)      894 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/list_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/logging_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/manager_interface.py
--rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/memoize_decorators.py
--rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/np_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     8482 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/path_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/pkg.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/py.typed
--rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/query_params.py
--rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/requests_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/response_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      559 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/sanitizers.py
--rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/serialization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/signal_decorators.py
--rw-r--r--   0 mourad     (501) staff       (20)     2339 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/string_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/tz_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/units_processors.py
--rw-r--r--   0 mourad     (501) staff       (20)      269 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/urls_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      613 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/validation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/versions.py
--rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/workers_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-06 15:16:50.000000 clipped-0.0.2/clipped/yaml_utils.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-06 15:18:06.021095 clipped-0.0.2/clipped.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-06 15:18:05.000000 clipped-0.0.2/clipped.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1142 2023-04-06 15:18:05.000000 clipped-0.0.2/clipped.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-06 15:18:05.000000 clipped-0.0.2/clipped.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-06 15:18:05.000000 clipped-0.0.2/clipped.egg-info/top_level.txt
--rw-r--r--   0 mourad     (501) staff       (20)     1032 2023-04-06 15:18:06.021846 clipped-0.0.2/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-06 15:16:50.000000 clipped-0.0.2/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-11 18:51:24.042803 clipped-0.0.3/
+-rw-r--r--   0 mourad     (501) staff       (20)      174 2023-04-11 18:44:55.000000 clipped-0.0.3/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-11 18:51:24.042894 clipped-0.0.3/PKG-INFO
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-11 18:51:24.041782 clipped-0.0.3/clipped/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/bool_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/cached_property.py
+-rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/click_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/cmd.py
+-rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/coroutine.py
+-rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/csv_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/date_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4349 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/deprecated_decorators.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3354 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/dict_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/encoding.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/enums_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1995 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/env.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6222 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/formatting.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4731 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/git_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1825 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/hashing.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/http_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3367 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/humanize.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/imports.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/indentation.py
+-rw-r--r--   0 mourad     (501) staff       (20)      256 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/json_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      894 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/list_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/logging_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/manager_interface.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/memoize_decorators.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/np_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8482 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/path_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-11 18:50:38.000000 clipped-0.0.3/clipped/pkg.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/py.typed
+-rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/query_params.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/requests_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/response_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      559 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/sanitizers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/serialization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/signal_decorators.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2339 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/string_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/tz_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/units_processors.py
+-rw-r--r--   0 mourad     (501) staff       (20)      269 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/urls_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      613 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/validation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/versions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/workers_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-11 18:44:55.000000 clipped-0.0.3/clipped/yaml_utils.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-11 18:51:24.042641 clipped-0.0.3/clipped.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-11 18:51:23.000000 clipped-0.0.3/clipped.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1164 2023-04-11 18:51:23.000000 clipped-0.0.3/clipped.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-11 18:51:23.000000 clipped-0.0.3/clipped.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-11 18:51:23.000000 clipped-0.0.3/clipped.egg-info/top_level.txt
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-11 18:51:24.043379 clipped-0.0.3/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-11 18:44:55.000000 clipped-0.0.3/setup.py
```

### Comparing `clipped-0.0.2/PKG-INFO` & `clipped-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.0.2
+Version: 0.0.3
 Summary: Common shortcuts and utils.
 Home-page: https://github.com/mmourafiq/clipped
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipped Version: 0.0.2 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.0.3 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.0.2/clipped/bool_utils.py` & `clipped-0.0.3/clipped/bool_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/cached_property.py` & `clipped-0.0.3/clipped/cached_property.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/cmd.py` & `clipped-0.0.3/clipped/cmd.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/coroutine.py` & `clipped-0.0.3/clipped/coroutine.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/csv_utils.py` & `clipped-0.0.3/clipped/csv_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/date_utils.py` & `clipped-0.0.3/clipped/date_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/deprecated_decorators.py` & `clipped-0.0.3/clipped/deprecated_decorators.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/dict_utils.py` & `clipped-0.0.3/clipped/dict_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/enums_utils.py` & `clipped-0.0.3/clipped/enums_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/env.py` & `clipped-0.0.3/clipped/env.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/formatting.py` & `clipped-0.0.3/clipped/formatting.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/git_utils.py` & `clipped-0.0.3/clipped/git_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/hashing.py` & `clipped-0.0.3/clipped/hashing.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/http_utils.py` & `clipped-0.0.3/clipped/http_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/humanize.py` & `clipped-0.0.3/clipped/humanize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from datetime import datetime
 from typing import Any, Union
 
-import ujson
-
 from clipped.date_utils import DateTimeFormatter, parse_datetime
+from clipped.json_utils import orjson_dumps
 from clipped.tz_utils import now
 from clipped.units_processors import to_percentage, to_unit_memory
 
 
 def humanize_timestamp(
     timestamp: Union[str, datetime],
 ) -> str:
@@ -92,15 +91,17 @@
         if seconds:
             result += " {}s".format(seconds)
         return result
 
     return "{}s".format(seconds)
 
 
-def humanize_attrs(key: str, value: Any, rounding: int = 2, timesince: bool = True):
+def humanize_attrs(
+    key: str, value: Any, rounding: int = 2, timesince: bool = True
+) -> str:
     if key in [
         "created_at",
         "updated_at",
         "started_at",
         "finished_at",
         "schedule_at",
         "last_update_time",
@@ -113,8 +114,8 @@
         return to_percentage(value, rounding)
     if key in ["memory_free", "memory_used", "memory_total"]:
         return to_unit_memory(value)
     if isinstance(value, str):
         return value
     if value is None:
         return ""
-    return ujson.dumps(value)
+    return orjson_dumps(value)
```

### Comparing `clipped-0.0.2/clipped/imports.py` & `clipped-0.0.3/clipped/imports.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/indentation.py` & `clipped-0.0.3/clipped/indentation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/list_utils.py` & `clipped-0.0.3/clipped/list_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/manager_interface.py` & `clipped-0.0.3/clipped/manager_interface.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/memoize_decorators.py` & `clipped-0.0.3/clipped/memoize_decorators.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/np_utils.py` & `clipped-0.0.3/clipped/np_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/path_utils.py` & `clipped-0.0.3/clipped/path_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/query_params.py` & `clipped-0.0.3/clipped/query_params.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/requests_utils.py` & `clipped-0.0.3/clipped/requests_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/response_utils.py` & `clipped-0.0.3/clipped/response_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/sanitizers.py` & `clipped-0.0.3/clipped/sanitizers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/serialization.py` & `clipped-0.0.3/clipped/serialization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/signal_decorators.py` & `clipped-0.0.3/clipped/signal_decorators.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/string_utils.py` & `clipped-0.0.3/clipped/string_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/tz_utils.py` & `clipped-0.0.3/clipped/tz_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/units_processors.py` & `clipped-0.0.3/clipped/units_processors.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/validation.py` & `clipped-0.0.3/clipped/validation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/versions.py` & `clipped-0.0.3/clipped/versions.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/workers_utils.py` & `clipped-0.0.3/clipped/workers_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped/yaml_utils.py` & `clipped-0.0.3/clipped/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.2/clipped.egg-info/PKG-INFO` & `clipped-0.0.3/clipped.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.0.2
+Version: 0.0.3
 Summary: Common shortcuts and utils.
 Home-page: https://github.com/mmourafiq/clipped
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipped Version: 0.0.2 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.0.3 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.0.2/clipped.egg-info/SOURCES.txt` & `clipped-0.0.3/clipped.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 clipped/formatting.py
 clipped/git_utils.py
 clipped/hashing.py
 clipped/http_utils.py
 clipped/humanize.py
 clipped/imports.py
 clipped/indentation.py
+clipped/json_utils.py
 clipped/list_utils.py
 clipped/logging_utils.py
 clipped/manager_interface.py
 clipped/memoize_decorators.py
 clipped/np_utils.py
 clipped/path_utils.py
 clipped/pkg.py
```

### Comparing `clipped-0.0.2/setup.cfg` & `clipped-0.0.3/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 profile = black
 line_length = 88
 lines_between_sections = 1
 lines_between_types = 1
 order_by_type = true
 known_future_library = future,pies
 extra_standard_library = typing,typing_extensions,mock,pytest,factory,faker,flaky,numpy,pandas,requests,websocket,jinja2,yaml,pytz
-known_third_party = rest_framework,scipy,sklearn,datadog,docker,corsheaders,celery,picklefield,sentry_sdk,ujson,pydantic,clipped
+known_third_party = rest_framework,scipy,sklearn,datadog,docker,corsheaders,celery,picklefield,sentry_sdk,orjson,pydantic,clipped
 known_first_party = clipped
 indent = '    '
 multi_line_output = 3
 include_trailing_comma = True
 force_grid_wrap = 0
 use_parentheses = True
 known_django = django
```

### Comparing `clipped-0.0.2/setup.py` & `clipped-0.0.3/setup.py`

 * *Files identical despite different names*

