# Comparing `tmp/jefferson-street-singer-ingest-2.8.0.tar.gz` & `tmp/jefferson-street-singer-ingest-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jefferson-street-singer-ingest-2.8.0.tar", max compression
+gzip compressed data, was "jefferson-street-singer-ingest-2.8.1.tar", max compression
```

## Comparing `jefferson-street-singer-ingest-2.8.0.tar` & `jefferson-street-singer-ingest-2.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-01-29 20:58:43.197928 jefferson-street-singer-ingest-2.8.0/README.md
--rw-r--r--   0        0        0      178 2023-01-29 20:58:43.198639 jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/__init__.py
--rw-r--r--   0        0        0      370 2023-01-29 20:58:43.199118 jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/__init__.py
--rw-r--r--   0        0        0      114 2023-01-29 20:58:43.199575 jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/entry/__init__.py
--rw-r--r--   0        0        0     3928 2023-04-01 21:43:00.357768 jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/entry/run_command.py
--rw-r--r--   0        0        0      863 2023-03-06 06:51:51.165998 jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/state/ingest_bookmark.py
--rw-r--r--   0        0        0     2952 2023-03-06 06:51:51.166128 jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/state/state_management.py
--rw-r--r--   0        0        0      186 2023-01-29 20:58:43.200092 jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/stream/__init__.py
--rw-r--r--   0        0        0     4323 2023-03-06 06:51:51.166341 jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/stream/base_tap_stream.py
--rw-r--r--   0        0        0     5683 2023-03-06 06:51:51.166543 jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/stream/rest_stream.py
--rw-r--r--   0        0        0       88 2023-01-29 20:58:43.201272 jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/tap/__init__.py
--rw-r--r--   0        0        0     7917 2023-01-29 20:58:43.201522 jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/tap/base_tap.py
--rw-r--r--   0        0        0      145 2023-01-29 20:58:43.201963 jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/target/__init__.py
--rw-r--r--   0        0        0     1009 2023-01-29 20:58:43.202097 jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/target/avro_generator.py
--rw-r--r--   0        0        0     2111 2023-01-29 20:58:43.202352 jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/target/base_google_cloud_storage_target.py
--rw-r--r--   0        0        0      632 2023-04-01 22:06:56.084349 jefferson-street-singer-ingest-2.8.0/pyproject.toml
--rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 jefferson-street-singer-ingest-2.8.0/setup.py
--rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 jefferson-street-singer-ingest-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-01-29 20:58:43.197928 jefferson-street-singer-ingest-2.8.1/README.md
+-rw-r--r--   0        0        0      178 2023-01-29 20:58:43.198639 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/__init__.py
+-rw-r--r--   0        0        0      370 2023-01-29 20:58:43.199118 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/__init__.py
+-rw-r--r--   0        0        0      114 2023-01-29 20:58:43.199575 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/entry/__init__.py
+-rw-r--r--   0        0        0     3026 2023-04-03 18:38:45.473683 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/entry/run_command.py
+-rw-r--r--   0        0        0      863 2023-03-06 06:51:51.165998 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/state/ingest_bookmark.py
+-rw-r--r--   0        0        0     3146 2023-04-11 01:01:56.530521 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/state/state_management.py
+-rw-r--r--   0        0        0      186 2023-01-29 20:58:43.200092 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/stream/__init__.py
+-rw-r--r--   0        0        0     4323 2023-03-06 06:51:51.166341 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/stream/base_tap_stream.py
+-rw-r--r--   0        0        0     5413 2023-04-11 00:54:06.673010 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/stream/rest_stream.py
+-rw-r--r--   0        0        0       88 2023-01-29 20:58:43.201272 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/tap/__init__.py
+-rw-r--r--   0        0        0     7917 2023-01-29 20:58:43.201522 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/tap/base_tap.py
+-rw-r--r--   0        0        0      145 2023-01-29 20:58:43.201963 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/target/__init__.py
+-rw-r--r--   0        0        0     1009 2023-01-29 20:58:43.202097 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/target/avro_generator.py
+-rw-r--r--   0        0        0     2111 2023-01-29 20:58:43.202352 jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/target/base_google_cloud_storage_target.py
+-rw-r--r--   0        0        0      632 2023-04-11 01:05:28.425111 jefferson-street-singer-ingest-2.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 jefferson-street-singer-ingest-2.8.1/setup.py
+-rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 jefferson-street-singer-ingest-2.8.1/PKG-INFO
```

### Comparing `jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/entry/run_command.py` & `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/entry/run_command.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,36 +26,14 @@
     if value is None and default_value is not None:
         value = default_value
 
     if not value:
         raise ValueError(f"Env variable {name} was not set")
     return value
 
-# class SingerCustomImageTapCommand(RunSingerPythonTapCommand):
-#     """
-#     Represents a tap which exists in our standard project layout under bin/ingest
-#     Assumes our tap was written under bin/ingest/<project>/services/taps
-#     If the file is not specified, assumes the tap is in <project>_tap.py
-#     """
-
-#     def __init__(self, project_name: str, config: Dict[str, Any], file: File = None):
-#         if not project_name:
-#             raise ValueError("Project name is required!")
-#         self.project_name = project_name
-#         if not file:
-#             file = File(f"{self.project_name}_tap.py")
-#         super().__init__(file, config)
-
-#     def get_scripts_folder(self) -> FolderPath:
-#         return FolderPath(f"./{self.project_name}/services/taps")
-
-#     def get_config_folder(self) -> FolderPath:
-#         return self.get_scripts_folder().add_sub_folder("configs")
-
-
 def run_custom_image_tap_and_target(project_name: str = "", config: Dict = {}):
     with open("config.json", "w") as config_file:
         config_file.write(json.dumps(config))
 
     tap_cmd = f"python {project_name}/tap/{project_name}_tap.py --config config.json"
     target_cmd = f"python {project_name}/target/{project_name}_target.py --config config.json"
```

### Comparing `jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/state/ingest_bookmark.py` & `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/state/ingest_bookmark.py`

 * *Files identical despite different names*

### Comparing `jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/state/state_management.py` & `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/state/state_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,20 @@
 
     def write_bookmark_to_state(
         self,
         source_uri: str = "",
         timestamp: str = datetime.strftime(datetime.utcnow(), "%Y%m%d%H%M%S"),
         additional_data: Dict[str, str] = {},
     ):
+        if not self.pipeline_name:
+            logging.info(
+                f"pipeline_name not set for state management, skipping writing bookmark to state."
+            )
+            return
+
         state_file_name = f"state_{timestamp}"
         cloud_storage_destination = f"ingest_states/raw/{state_file_name}.json"
 
         updated_state_content = self.merge_state_and_bookmark(
             ingest_bookmark=IngestBookmark(
                 pipeline_name=self.pipeline_name,
                 source_uri=source_uri,
```

### Comparing `jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/stream/base_tap_stream.py` & `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/stream/base_tap_stream.py`

 * *Files identical despite different names*

### Comparing `jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/stream/rest_stream.py` & `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/stream/rest_stream.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,24 +111,17 @@
             time.sleep(self.request_delay)
 
         try:
             for row in self.request_records(partition):
                 row = self.post_process(row)
                 flat = self.flatten_object(row)
                 yield flat
-            # self.bookmark_service.write_url_read_bookmark(
-            #     self.url_base, success=True, stream_name=self.name
-            # )
+                
+            self.bookmark_service.write_bookmark_to_state(self.get_url(partition))
         except Exception as e:
-            # self.bookmark_service.write_url_read_bookmark(
-            #     url_base=self.url_base,
-            #     success=False,
-            #     exception=e,
-            #     stream_name=self.name,
-            # )
             logging.error(e)
             raise
 
     def get_schema(self) -> Schema:
         first = None
         if not self._found_schema_object:
             for rec in self.get_records():
```

### Comparing `jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/tap/base_tap.py` & `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/tap/base_tap.py`

 * *Files identical despite different names*

### Comparing `jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/target/avro_generator.py` & `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/target/avro_generator.py`

 * *Files identical despite different names*

### Comparing `jefferson-street-singer-ingest-2.8.0/jefferson_street_singer_ingest/services/target/base_google_cloud_storage_target.py` & `jefferson-street-singer-ingest-2.8.1/jefferson_street_singer_ingest/services/target/base_google_cloud_storage_target.py`

 * *Files identical despite different names*

### Comparing `jefferson-street-singer-ingest-2.8.0/pyproject.toml` & `jefferson-street-singer-ingest-2.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jefferson-street-singer-ingest"
-version = "2.8.0"
+version = "2.8.1"
 description = "Library holding the taps and targets for Jefferson Street Ingestion"
 authors = ["Nikolai McFall <nikolai@jeffersonst.io>"]
 readme = "README.md"
 packages = [{include = "jefferson_street_singer_ingest"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.9"
```

### Comparing `jefferson-street-singer-ingest-2.8.0/setup.py` & `jefferson-street-singer-ingest-2.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'pandas>=1.4.4,<2.0.0',
  'rec-avro>=0.0.4,<0.0.5',
  'requests>=2.28.1,<3.0.0',
  'singer-sdk==0.1.6']
 
 setup_kwargs = {
     'name': 'jefferson-street-singer-ingest',
-    'version': '2.8.0',
+    'version': '2.8.1',
     'description': 'Library holding the taps and targets for Jefferson Street Ingestion',
     'long_description': '',
     'author': 'Nikolai McFall',
     'author_email': 'nikolai@jeffersonst.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `jefferson-street-singer-ingest-2.8.0/PKG-INFO` & `jefferson-street-singer-ingest-2.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jefferson-street-singer-ingest
-Version: 2.8.0
+Version: 2.8.1
 Summary: Library holding the taps and targets for Jefferson Street Ingestion
 Author: Nikolai McFall
 Author-email: nikolai@jeffersonst.io
 Requires-Python: >=3.8,<3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: fastavro (>=1.6.1,<2.0.0)
```

