# Comparing `tmp/tap-google-search-console-0.2.1.tar.gz` & `tmp/tap-google-search-console-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-google-search-console-0.2.1.tar", last modified: Tue Apr  4 04:41:30 2023, max compression
+gzip compressed data, was "dist/tap-google-search-console-1.0.0.tar", last modified: Tue Apr 11 10:52:30 2023, max compression
```

## Comparing `tap-google-search-console-0.2.1.tar` & `tap-google-search-console-1.0.0.tar`

### file list

```diff
@@ -1,36 +1,47 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-04 04:41:30.000000 tap-google-search-console-0.2.1/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-04 04:41:30.000000 tap-google-search-console-0.2.1/tap_google_search_console.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       73 2023-04-04 04:41:30.000000 tap-google-search-console-0.2.1/tap_google_search_console.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-04 04:41:30.000000 tap-google-search-console-0.2.1/tap_google_search_console.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-04 04:41:30.000000 tap-google-search-console-0.2.1/tap_google_search_console.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-04-04 04:41:30.000000 tap-google-search-console-0.2.1/tap_google_search_console.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1313 2023-04-04 04:41:30.000000 tap-google-search-console-0.2.1/tap_google_search_console.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-04-04 04:41:30.000000 tap-google-search-console-0.2.1/tap_google_search_console.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       65 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2023-04-04 04:41:30.000000 tap-google-search-console-0.2.1/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-04 04:41:30.000000 tap-google-search-console-0.2.1/tap_google_search_console/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-04 04:41:30.000000 tap-google-search-console-0.2.1/tap_google_search_console/streams/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15067 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/streams/abstract.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1285 2023-04-04 04:41:11.000000 tap-google-search-console-0.2.1/tap_google_search_console/streams/sitemaps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      984 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/streams/sites.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2323 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/streams/performance_reports.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      751 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/streams/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3857 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/transform.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4628 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4993 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4859 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-04 04:41:30.000000 tap-google-search-console-0.2.1/tap_google_search_console/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      812 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/schemas/performance_report_device.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1143 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/schemas/performance_report_custom.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1606 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/schemas/sitemaps.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      811 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/schemas/performance_report_query.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      732 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/schemas/performance_report_date.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      250 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/schemas/sites.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      813 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/schemas/performance_report_country.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      810 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/schemas/performance_report_page.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1162 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      985 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1200 2023-04-04 02:49:16.000000 tap-google-search-console-0.2.1/tap_google_search_console/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-04-04 04:41:30.000000 tap-google-search-console-0.2.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      779 2023-04-04 04:41:11.000000 tap-google-search-console-0.2.1/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2022-07-15 09:05:10.000000 tap-google-search-console-0.2.1/LICENSE
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-11 10:52:30.000000 tap-google-search-console-1.0.0/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-11 10:52:29.000000 tap-google-search-console-1.0.0/tap_google_search_console.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       73 2023-04-11 10:52:29.000000 tap-google-search-console-1.0.0/tap_google_search_console.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-11 10:52:29.000000 tap-google-search-console-1.0.0/tap_google_search_console.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-11 10:52:29.000000 tap-google-search-console-1.0.0/tap_google_search_console.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2023-04-11 10:52:29.000000 tap-google-search-console-1.0.0/tap_google_search_console.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1586 2023-04-11 10:52:29.000000 tap-google-search-console-1.0.0/tap_google_search_console.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-04-11 10:52:29.000000 tap-google-search-console-1.0.0/tap_google_search_console.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       65 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/MANIFEST.in
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-11 10:52:30.000000 tap-google-search-console-1.0.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3013 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tests/test_gsc_automatic_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6760 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tests/test_gsc_start_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12154 2023-04-11 10:47:08.000000 tap-google-search-console-1.0.0/tests/test_gsc_bookmarks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2275 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tests/test_gsc_pagination_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10677 2023-04-11 10:47:08.000000 tap-google-search-console-1.0.0/tests/test_gsc_interrupted_sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5806 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tests/test_gsc_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tests/test_gsc_sync_canary.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3782 2023-04-11 10:47:08.000000 tap-google-search-console-1.0.0/tests/test_gsc_all_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      262 2023-04-11 10:52:30.000000 tap-google-search-console-1.0.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-11 10:52:29.000000 tap-google-search-console-1.0.0/tap_google_search_console/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-11 10:52:29.000000 tap-google-search-console-1.0.0/tap_google_search_console/streams/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16235 2023-04-11 10:47:08.000000 tap-google-search-console-1.0.0/tap_google_search_console/streams/abstract.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1285 2023-04-04 04:41:11.000000 tap-google-search-console-1.0.0/tap_google_search_console/streams/sitemaps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      984 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/streams/sites.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2894 2023-04-11 10:47:08.000000 tap-google-search-console-1.0.0/tap_google_search_console/streams/performance_reports.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      751 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/streams/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3857 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/transform.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4628 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4993 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4859 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-11 10:52:29.000000 tap-google-search-console-1.0.0/tap_google_search_console/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      812 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/schemas/performance_report_device.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1143 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/schemas/performance_report_custom.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1606 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/schemas/sitemaps.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      811 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/schemas/performance_report_query.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      732 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/schemas/performance_report_date.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      250 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/schemas/sites.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      813 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/schemas/performance_report_country.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      810 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/schemas/performance_report_page.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1162 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      985 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1200 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/tap_google_search_console/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2023-04-11 10:52:30.000000 tap-google-search-console-1.0.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      360 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      779 2023-04-11 10:47:08.000000 tap-google-search-console-1.0.0/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2022-07-15 09:05:10.000000 tap-google-search-console-1.0.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16227 2023-04-04 02:49:16.000000 tap-google-search-console-1.0.0/README.md
```

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/streams/abstract.py` & `tap-google-search-console-1.0.0/tap_google_search_console/streams/abstract.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 class IncrementalTableStream(BaseStream, ABC):
     """Base Class for Incremental Stream."""
 
     replication_method = "INCREMENTAL"
     forced_replication_method = "INCREMENTAL"
     replication_key = "date"
     pagination = "body"
-    sub_types = ["web", "image", "video"]
+    sub_types = ["discover", "googleNews", "image", "news", "video", "web"]
     row_limit = 10000
     path = "sites/{}/searchAnalytics/query"
     data_key = "rows"
     now_dt_tm = utils.now()
     dimension_list = []
     body_params = {}
 
@@ -162,14 +162,29 @@
                 selected_dimensions.append(dimension)
         return selected_dimensions
 
     def make_payload(self, sub_type: str, start_date: str, end_date: str, stream_metadata: Dict) -> Dict:
         """Creates payload for POST API Call."""
         if self.tap_stream_id == "performance_report_custom":
             self.body_params["dimensions"] = self.set_dimensions_in_payload(stream_metadata)
+            # Remove discover dimension from dimension_list if sub_type is discover
+            # Requests for Discover cannot be grouped by device
+            if sub_type == "discover" and "device" in self.body_params["dimensions"]:
+                LOGGER.info(f"Removing the device dimension/field since it is incompatible with"
+                            f" {sub_type} sub_type for custom report")
+                self.body_params["dimensions"].remove("device")
+        if sub_type in {"discover", "googleNews"}:
+            self.body_params["aggregationType"] = "auto"
+            # Remove query from dimension list if the sub_type is either discover or googleNews
+            # query seems to be an invalid argument while grouping data for discover and googleNews
+            if self.tap_stream_id == "performance_report_custom" and \
+                    "query" in self.body_params["dimensions"]:
+                LOGGER.info(f"Removing the query dimension/field since it is incompatible with"
+                            f" {sub_type} sub_type for custom report")
+                self.body_params["dimensions"].remove("query")
 
         return {"type": sub_type, "startDate": start_date, "endDate": end_date, **self.body_params}
 
     def validate_keys_in_data(self, extracted_data: List) -> None:
         """Validates the data by checking the primary keys in extracted
         data."""
         for record in extracted_data:
```

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/streams/sitemaps.py` & `tap-google-search-console-1.0.0/tap_google_search_console/streams/sitemaps.py`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/streams/sites.py` & `tap-google-search-console-1.0.0/tap_google_search_console/streams/sites.py`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/streams/__init__.py` & `tap-google-search-console-1.0.0/tap_google_search_console/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/transform.py` & `tap-google-search-console-1.0.0/tap_google_search_console/transform.py`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/helpers.py` & `tap-google-search-console-1.0.0/tap_google_search_console/helpers.py`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/exceptions.py` & `tap-google-search-console-1.0.0/tap_google_search_console/exceptions.py`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/client.py` & `tap-google-search-console-1.0.0/tap_google_search_console/client.py`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/schemas/performance_report_device.json` & `tap-google-search-console-1.0.0/tap_google_search_console/schemas/performance_report_device.json`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/schemas/performance_report_custom.json` & `tap-google-search-console-1.0.0/tap_google_search_console/schemas/performance_report_custom.json`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/schemas/sitemaps.json` & `tap-google-search-console-1.0.0/tap_google_search_console/schemas/sitemaps.json`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/schemas/performance_report_query.json` & `tap-google-search-console-1.0.0/tap_google_search_console/schemas/performance_report_query.json`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/schemas/performance_report_date.json` & `tap-google-search-console-1.0.0/tap_google_search_console/schemas/performance_report_date.json`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/schemas/performance_report_country.json` & `tap-google-search-console-1.0.0/tap_google_search_console/schemas/performance_report_country.json`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/schemas/performance_report_page.json` & `tap-google-search-console-1.0.0/tap_google_search_console/schemas/performance_report_page.json`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/__init__.py` & `tap-google-search-console-1.0.0/tap_google_search_console/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/sync.py` & `tap-google-search-console-1.0.0/tap_google_search_console/sync.py`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/tap_google_search_console/discover.py` & `tap-google-search-console-1.0.0/tap_google_search_console/discover.py`

 * *Files identical despite different names*

### Comparing `tap-google-search-console-0.2.1/setup.py` & `tap-google-search-console-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="tap-google-search-console",
-    version="0.2.1",
+    version="1.0.0",
     description="Singer.io tap for extracting data from the Google Search Console API",
     author="jeff.huth@bytecode.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["tap_google_search_console"],
     install_requires=["backoff==1.8.0", "requests==2.22.0", "singer-python==5.13.0"],
     extras_require={
         "dev": [
```

### Comparing `tap-google-search-console-0.2.1/LICENSE` & `tap-google-search-console-1.0.0/LICENSE`

 * *Files identical despite different names*

