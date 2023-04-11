# Comparing `tmp/dms-influx2-0.2.6.tar.gz` & `tmp/dms-influx2-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dms-influx2-0.2.6.tar", last modified: Tue Apr 11 05:37:48 2023, max compression
+gzip compressed data, was "dist\dms-influx2-0.2.7.tar", last modified: Tue Apr 11 13:19:12 2023, max compression
```

## Comparing `dms-influx2-0.2.6.tar` & `dms-influx2-0.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 05:37:48.833691 dms-influx2-0.2.6/
--rw-rw-rw-   0        0        0      556 2023-04-11 05:37:48.833691 dms-influx2-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 05:37:48.829659 dms-influx2-0.2.6/dms_influx2/
--rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/dms_influx2/__init__.py
--rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/dms_influx2/authorizations.py
--rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.2.6/dms_influx2/buckets.py
--rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.2.6/dms_influx2/checks.py
--rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/dms_influx2/decorators.py
--rw-rw-rw-   0        0        0     2384 2023-03-22 11:20:22.000000 dms-influx2-0.2.6/dms_influx2/delete.py
--rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.2.6/dms_influx2/dtv_files.py
--rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/dms_influx2/exceptions.py
--rw-rw-rw-   0        0        0    21426 2023-04-11 04:55:31.000000 dms-influx2-0.2.6/dms_influx2/lib.py
--rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/dms_influx2/notifications.py
--rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/dms_influx2/organisations.py
--rw-rw-rw-   0        0        0     7217 2023-04-11 05:18:02.000000 dms-influx2-0.2.6/dms_influx2/query.py
--rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.2.6/dms_influx2/sync.py
--rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.2.6/dms_influx2/tasks.py
--rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.2.6/dms_influx2/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 05:37:48.833691 dms-influx2-0.2.6/dms_influx2.egg-info/
--rw-rw-rw-   0        0        0      556 2023-04-11 05:37:48.000000 dms-influx2-0.2.6/dms_influx2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-04-11 05:37:48.000000 dms-influx2-0.2.6/dms_influx2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 05:37:48.000000 dms-influx2-0.2.6/dms_influx2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-04-11 05:37:48.000000 dms-influx2-0.2.6/dms_influx2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-11 05:37:48.000000 dms-influx2-0.2.6/dms_influx2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 05:37:48.833691 dms-influx2-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     3023 2023-04-11 05:37:05.000000 dms-influx2-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:19:12.719582 dms-influx2-0.2.7/
+-rw-rw-rw-   0        0        0      556 2023-04-11 13:19:12.719582 dms-influx2-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 13:19:12.715580 dms-influx2-0.2.7/dms_influx2/
+-rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.2.7/dms_influx2/__init__.py
+-rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.2.7/dms_influx2/authorizations.py
+-rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.2.7/dms_influx2/buckets.py
+-rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.2.7/dms_influx2/checks.py
+-rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.2.7/dms_influx2/decorators.py
+-rw-rw-rw-   0        0        0     2384 2023-03-22 11:20:22.000000 dms-influx2-0.2.7/dms_influx2/delete.py
+-rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.2.7/dms_influx2/dtv_files.py
+-rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.2.7/dms_influx2/exceptions.py
+-rw-rw-rw-   0        0        0    21500 2023-04-11 13:17:17.000000 dms-influx2-0.2.7/dms_influx2/lib.py
+-rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.2.7/dms_influx2/notifications.py
+-rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.2.7/dms_influx2/organisations.py
+-rw-rw-rw-   0        0        0     7217 2023-04-11 05:18:02.000000 dms-influx2-0.2.7/dms_influx2/query.py
+-rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.2.7/dms_influx2/sync.py
+-rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.2.7/dms_influx2/tasks.py
+-rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.2.7/dms_influx2/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:19:12.719582 dms-influx2-0.2.7/dms_influx2.egg-info/
+-rw-rw-rw-   0        0        0      556 2023-04-11 13:19:12.000000 dms-influx2-0.2.7/dms_influx2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-04-11 13:19:12.000000 dms-influx2-0.2.7/dms_influx2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 13:19:12.000000 dms-influx2-0.2.7/dms_influx2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-04-11 13:19:12.000000 dms-influx2-0.2.7/dms_influx2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-11 13:19:12.000000 dms-influx2-0.2.7/dms_influx2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 13:19:12.719582 dms-influx2-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     3023 2023-04-11 13:18:29.000000 dms-influx2-0.2.7/setup.py
```

### Comparing `dms-influx2-0.2.6/PKG-INFO` & `dms-influx2-0.2.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.2.6
+Version: 0.2.7
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.2.6/dms_influx2/authorizations.py` & `dms-influx2-0.2.7/dms_influx2/authorizations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.6/dms_influx2/buckets.py` & `dms-influx2-0.2.7/dms_influx2/buckets.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.6/dms_influx2/checks.py` & `dms-influx2-0.2.7/dms_influx2/checks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.6/dms_influx2/decorators.py` & `dms-influx2-0.2.7/dms_influx2/decorators.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.6/dms_influx2/delete.py` & `dms-influx2-0.2.7/dms_influx2/delete.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.6/dms_influx2/dtv_files.py` & `dms-influx2-0.2.7/dms_influx2/dtv_files.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.6/dms_influx2/lib.py` & `dms-influx2-0.2.7/dms_influx2/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,24 +249,25 @@
             item['timestamp'] = item['values'][-1][0]
             item['value'] = item['values'][-1][1]
             item.pop('values')
             _data.append(item)
         return _data
 
     def get_one_value(self, bucket, measurement=None, device_id=None, description=None,
-                      time_range=None, time_from=None, time_to=None, sort='desc', last=True) -> list:
+                      time_range=None, time_from=None, time_to=None, sort='desc', last=True,
+                      errors_filter='keep') -> list:
         """Get only one value per table (last or first)"""
 
         if time_range is None and time_from is None and time_to is None:
             time_range = 'all'
 
         tables = self._get_tables(bucket=bucket, measurement=measurement, device_id=device_id, description=description,
                                   time_range=time_range, time_from=time_from, time_to=time_to, last=last,
                                   value_type=None, value=None, value_within=None, value_min=None, value_max=None,
-                                  first=not last, group_columns=["device_id"])
+                                  first=not last, group_columns=["device_id"], errors_filter=errors_filter)
 
         data = self._extract_tables(tables)
 
         if sort == 'desc' or sort == 'asc':
             data.sort(key=self.pop_timestamp_from_values, reverse=sort == 'desc')
 
         return self.to_one_value_format(data)
```

### Comparing `dms-influx2-0.2.6/dms_influx2/notifications.py` & `dms-influx2-0.2.7/dms_influx2/notifications.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.6/dms_influx2/organisations.py` & `dms-influx2-0.2.7/dms_influx2/organisations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.6/dms_influx2/query.py` & `dms-influx2-0.2.7/dms_influx2/query.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.6/dms_influx2/tasks.py` & `dms-influx2-0.2.7/dms_influx2/tasks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.6/dms_influx2/utils.py` & `dms-influx2-0.2.7/dms_influx2/utils.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.6/dms_influx2.egg-info/PKG-INFO` & `dms-influx2-0.2.7/dms_influx2.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.2.6
+Version: 0.2.7
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.2.6/dms_influx2.egg-info/SOURCES.txt` & `dms-influx2-0.2.7/dms_influx2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.6/setup.py` & `dms-influx2-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'dms-influx2'
 DESCRIPTION = 'Library to connect and retrieve data from DMS influxdb'
 URL = 'https://github.com/belingarb/dms-influx2'
 EMAIL = 'bozidar.belingar@gmail.com'
 AUTHOR = 'Bozidar Belingar'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.2.6'
+VERSION = '0.2.7'
 
 # Get required packages from requirements.txt file
 with open('requirements/base.txt') as f:
     REQUIRED = f.read().splitlines()
 
 dir_path = os.path.abspath(os.path.dirname(__file__))
```

