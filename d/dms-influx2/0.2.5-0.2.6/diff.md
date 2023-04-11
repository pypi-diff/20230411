# Comparing `tmp/dms-influx2-0.2.5.tar.gz` & `tmp/dms-influx2-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dms-influx2-0.2.5.tar", last modified: Wed Mar 22 11:23:54 2023, max compression
+gzip compressed data, was "dist\dms-influx2-0.2.6.tar", last modified: Tue Apr 11 05:37:48 2023, max compression
```

## Comparing `dms-influx2-0.2.5.tar` & `dms-influx2-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 11:23:54.605795 dms-influx2-0.2.5/
--rw-rw-rw-   0        0        0      556 2023-03-22 11:23:54.605795 dms-influx2-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-22 11:23:54.595285 dms-influx2-0.2.5/dms_influx2/
--rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.2.5/dms_influx2/__init__.py
--rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.2.5/dms_influx2/authorizations.py
--rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.2.5/dms_influx2/buckets.py
--rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.2.5/dms_influx2/checks.py
--rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.2.5/dms_influx2/decorators.py
--rw-rw-rw-   0        0        0     2384 2023-03-22 11:20:22.000000 dms-influx2-0.2.5/dms_influx2/delete.py
--rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.2.5/dms_influx2/dtv_files.py
--rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.2.5/dms_influx2/exceptions.py
--rw-rw-rw-   0        0        0    21385 2023-03-22 11:19:56.000000 dms-influx2-0.2.5/dms_influx2/lib.py
--rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.2.5/dms_influx2/notifications.py
--rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.2.5/dms_influx2/organisations.py
--rw-rw-rw-   0        0        0     6753 2023-02-01 19:51:32.000000 dms-influx2-0.2.5/dms_influx2/query.py
--rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.2.5/dms_influx2/sync.py
--rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.2.5/dms_influx2/tasks.py
--rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.2.5/dms_influx2/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-22 11:23:54.604793 dms-influx2-0.2.5/dms_influx2.egg-info/
--rw-rw-rw-   0        0        0      556 2023-03-22 11:23:54.000000 dms-influx2-0.2.5/dms_influx2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-03-22 11:23:54.000000 dms-influx2-0.2.5/dms_influx2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 11:23:54.000000 dms-influx2-0.2.5/dms_influx2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-03-22 11:23:54.000000 dms-influx2-0.2.5/dms_influx2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-22 11:23:54.000000 dms-influx2-0.2.5/dms_influx2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-22 11:23:54.605795 dms-influx2-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     3023 2023-03-22 11:23:02.000000 dms-influx2-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:37:48.833691 dms-influx2-0.2.6/
+-rw-rw-rw-   0        0        0      556 2023-04-11 05:37:48.833691 dms-influx2-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 05:37:48.829659 dms-influx2-0.2.6/dms_influx2/
+-rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/dms_influx2/__init__.py
+-rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/dms_influx2/authorizations.py
+-rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.2.6/dms_influx2/buckets.py
+-rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.2.6/dms_influx2/checks.py
+-rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/dms_influx2/decorators.py
+-rw-rw-rw-   0        0        0     2384 2023-03-22 11:20:22.000000 dms-influx2-0.2.6/dms_influx2/delete.py
+-rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.2.6/dms_influx2/dtv_files.py
+-rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/dms_influx2/exceptions.py
+-rw-rw-rw-   0        0        0    21426 2023-04-11 04:55:31.000000 dms-influx2-0.2.6/dms_influx2/lib.py
+-rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/dms_influx2/notifications.py
+-rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/dms_influx2/organisations.py
+-rw-rw-rw-   0        0        0     7217 2023-04-11 05:18:02.000000 dms-influx2-0.2.6/dms_influx2/query.py
+-rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.2.6/dms_influx2/sync.py
+-rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/dms_influx2/tasks.py
+-rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.2.6/dms_influx2/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:37:48.833691 dms-influx2-0.2.6/dms_influx2.egg-info/
+-rw-rw-rw-   0        0        0      556 2023-04-11 05:37:48.000000 dms-influx2-0.2.6/dms_influx2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-04-11 05:37:48.000000 dms-influx2-0.2.6/dms_influx2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 05:37:48.000000 dms-influx2-0.2.6/dms_influx2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-04-11 05:37:48.000000 dms-influx2-0.2.6/dms_influx2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-11 05:37:48.000000 dms-influx2-0.2.6/dms_influx2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 05:37:48.833691 dms-influx2-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     3023 2023-04-11 05:37:05.000000 dms-influx2-0.2.6/setup.py
```

### Comparing `dms-influx2-0.2.5/PKG-INFO` & `dms-influx2-0.2.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.2.5
+Version: 0.2.6
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.2.5/dms_influx2/authorizations.py` & `dms-influx2-0.2.6/dms_influx2/authorizations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.5/dms_influx2/buckets.py` & `dms-influx2-0.2.6/dms_influx2/buckets.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.5/dms_influx2/checks.py` & `dms-influx2-0.2.6/dms_influx2/checks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.5/dms_influx2/decorators.py` & `dms-influx2-0.2.6/dms_influx2/decorators.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.5/dms_influx2/delete.py` & `dms-influx2-0.2.6/dms_influx2/delete.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.5/dms_influx2/dtv_files.py` & `dms-influx2-0.2.6/dms_influx2/dtv_files.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.5/dms_influx2/lib.py` & `dms-influx2-0.2.6/dms_influx2/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
 
         return self.to_one_value_format(data)
 
     def get_values_from_device_id(self, bucket, measurement, device_id, description=None,
                                   time_range=None, time_from=None, time_to=None,
                                   aggregate_window=None, aggregate_func=None, aggregate_create_empty=False,
                                   value_type=None, value=None, value_within=None, value_min=None, value_max=None,
-                                  sort='desc', limit=None, window_count=None):
+                                  sort='desc', limit=None, window_count=None, errors_filter=None):
 
         if measurement is None:
             raise ValueError("Invalid value for `measurement`, must not be `None`")
 
         if device_id is None:
             raise ValueError("Invalid value for `device_id`, must not be `None`")
 
@@ -294,15 +294,15 @@
 
         return values[0]['values'] if values else None
 
     def get_data_from_device_id(self, bucket, measurement, device_id, description=None,
                                 time_range=None, time_from=None, time_to=None,
                                 aggregate_window=None, aggregate_func=None, aggregate_create_empty=False,
                                 value_type=None, value=None, value_within=None, value_min=None, value_max=None,
-                                sort='desc', limit=None, window_count=None) -> dict:
+                                sort='desc', limit=None, window_count=None, errors_filter=False) -> dict:
 
         if measurement is None:
             raise ValueError("Invalid value for `measurement`, must not be `None`")
 
         if device_id is None:
             raise ValueError("Invalid value for `device_id`, must not be `None`")
```

### Comparing `dms-influx2-0.2.5/dms_influx2/notifications.py` & `dms-influx2-0.2.6/dms_influx2/notifications.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.5/dms_influx2/organisations.py` & `dms-influx2-0.2.6/dms_influx2/organisations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.5/dms_influx2/query.py` & `dms-influx2-0.2.6/dms_influx2/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from datetime import datetime
-from typing import Union
+from typing import Union, Literal
 
 from dms_influx2.utils import timestamp_to_influx_string, localize_dt
 
 
 def get_flux_query(bucket=None,
                    measurement=None,
                    device_id=None,
@@ -30,15 +30,16 @@
                    time_shift=None,
                    time_offset: int = None,
                    window_count: str = None,
                    value_type: str = None,
                    value: float = None,
                    value_within: bool = None,
                    value_min: float = None,
-                   value_max: float = None) -> str:
+                   value_max: float = None,
+                   errors_filter: Literal['keep', 'drop', 'only'] = 'drop') -> str:
     """
 
     :param first:
     :param window_count:
     :param time_offset:
     :param time_shift:
     :param field:
@@ -63,14 +64,15 @@
     :param bucket_to:
     :param org_to:
     :param value_type:
     :param value_within:
     :param value_min:
     :param value_max:
     :param value:
+    :param errors_filter: Errors are all values == 55M; Keep errors, drop values, query only errors
     :return:
     """
 
     if bucket is None:
         raise ValueError("Invalid value for `bucket`, must not be `None`")
 
     stop = None
@@ -111,14 +113,21 @@
 
     if device_id:
         query_str += f'''\n\t|> filter(fn: (r) => r["device_id"] == "{device_id}")'''
 
     if description:
         query_str += f'''\n\t|> filter(fn: (r) => r["description"] == "{description}")'''
 
+    if errors_filter == 'keep':
+        pass
+    elif errors_filter == 'drop':
+        query_str += f'''\n\t|> filter(fn: (r) => r["_value"] != 55000000)'''
+    elif errors_filter == 'only':
+        query_str += f'''\n\t|> filter(fn: (r) => r["_value"] == 55000000)'''
+
     if value_type:
         if value_type == 'lesser' or value_type == 'greater' and value is not None:
             sign = '<' if value_type == 'lesser' else '>'
             query_str += f'''\n\t|> filter(fn: (r) => r["_value"] {sign} {value})'''
         if value_type == 'range':
             if value_within:
                 query_str += f'''\n\t|> filter(fn: (r) => r["_value"] > {value_min} and r["_value"] < {value_max})'''
```

### Comparing `dms-influx2-0.2.5/dms_influx2/tasks.py` & `dms-influx2-0.2.6/dms_influx2/tasks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.5/dms_influx2/utils.py` & `dms-influx2-0.2.6/dms_influx2/utils.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.5/dms_influx2.egg-info/PKG-INFO` & `dms-influx2-0.2.6/dms_influx2.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.2.5
+Version: 0.2.6
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.2.5/dms_influx2.egg-info/SOURCES.txt` & `dms-influx2-0.2.6/dms_influx2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.5/setup.py` & `dms-influx2-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'dms-influx2'
 DESCRIPTION = 'Library to connect and retrieve data from DMS influxdb'
 URL = 'https://github.com/belingarb/dms-influx2'
 EMAIL = 'bozidar.belingar@gmail.com'
 AUTHOR = 'Bozidar Belingar'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.2.5'
+VERSION = '0.2.6'
 
 # Get required packages from requirements.txt file
 with open('requirements/base.txt') as f:
     REQUIRED = f.read().splitlines()
 
 dir_path = os.path.abspath(os.path.dirname(__file__))
```

