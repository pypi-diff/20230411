# Comparing `tmp/brainframe_apps-0.3.18.tar.gz` & `tmp/brainframe_apps-0.3.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainframe_apps-0.3.18.tar", max compression
+gzip compressed data, was "brainframe_apps-0.3.19.tar", max compression
```

## Comparing `brainframe_apps-0.3.18.tar` & `brainframe_apps-0.3.19.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0      599 2023-04-09 00:36:44.237108 brainframe_apps-0.3.18/brainframe_apps/__init__.py
--rw-r--r--   0        0        0     4817 2023-04-09 00:36:34.917171 brainframe_apps-0.3.18/brainframe_apps/add_stream.py
--rw-r--r--   0        0        0      665 2022-12-19 23:19:56.515826 brainframe_apps-0.3.18/brainframe_apps/bf_log_print.py
--rw-r--r--   0        0        0    14973 2023-04-09 00:36:55.997030 brainframe_apps-0.3.18/brainframe_apps/capsule_control.py
--rw-r--r--   0        0        0     1115 2023-04-09 00:36:44.237108 brainframe_apps-0.3.18/brainframe_apps/cli.py
--rw-r--r--   0        0        0      571 2023-04-08 04:43:59.581232 brainframe_apps-0.3.18/brainframe_apps/command_utils.py
--rw-r--r--   0        0        0     2582 2023-04-09 00:36:34.917171 brainframe_apps-0.3.18/brainframe_apps/delete_stream.py
--rw-r--r--   0        0        0     4691 2022-12-19 23:19:56.515826 brainframe_apps-0.3.18/brainframe_apps/fps_report.py
--rw-r--r--   0        0        0     6343 2023-04-09 00:36:34.917171 brainframe_apps-0.3.18/brainframe_apps/get_configuration.py
--rw-r--r--   0        0        0     8070 2023-04-09 00:36:44.237108 brainframe_apps-0.3.18/brainframe_apps/get_zone_statuses.py
--rw-r--r--   0        0        0     4733 2023-04-09 00:36:34.917171 brainframe_apps-0.3.18/brainframe_apps/identity_control.py
--rw-r--r--   0        0        0     2434 2023-04-09 00:36:34.917171 brainframe_apps-0.3.18/brainframe_apps/license_control.py
--rw-r--r--   0        0        0     6284 2023-04-09 00:36:44.213108 brainframe_apps-0.3.18/brainframe_apps/list_stream.py
--rw-r--r--   0        0        0     2903 2023-04-09 00:36:34.917171 brainframe_apps-0.3.18/brainframe_apps/logger_factory.py
--rw-r--r--   0        0        0      734 2023-04-09 00:33:40.814733 brainframe_apps-0.3.18/brainframe_apps/print_utils.py
--rw-r--r--   0        0        0     4455 2023-04-09 00:36:34.917171 brainframe_apps-0.3.18/brainframe_apps/process_image.py
--rw-r--r--   0        0        0     9547 2023-04-09 00:36:34.917171 brainframe_apps-0.3.18/brainframe_apps/set_configuration.py
--rw-r--r--   0        0        0     1797 2023-04-08 01:22:50.977592 brainframe_apps-0.3.18/brainframe_apps/settings.json
--rw-r--r--   0        0        0     3919 2023-04-09 00:36:34.917171 brainframe_apps-0.3.18/brainframe_apps/start_analyzing.py
--rw-r--r--   0        0        0     2153 2023-04-09 00:36:34.917171 brainframe_apps-0.3.18/brainframe_apps/stop_analyzing.py
--rw-r--r--   0        0        0     1046 2022-12-19 23:19:56.519826 brainframe_apps-0.3.18/brainframe_apps/time_utils.py
--rw-r--r--   0        0        0      801 2023-04-09 00:36:44.237108 brainframe_apps-0.3.18/brainframe_apps/translations/portal.en.yml
--rw-r--r--   0        0        0     3064 2023-04-09 00:36:34.917171 brainframe_apps-0.3.18/brainframe_apps/urls.py
--rw-r--r--   0        0        0     1037 2023-04-09 00:36:34.917171 brainframe_apps-0.3.18/brainframe_apps/wait_for_ready.py
--rw-r--r--   0        0        0      783 2023-04-09 00:41:22.567931 brainframe_apps-0.3.18/pyproject.toml
--rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 brainframe_apps-0.3.18/setup.py
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 brainframe_apps-0.3.18/PKG-INFO
+-rw-r--r--   0        0        0      599 2023-04-09 00:36:44.237108 brainframe_apps-0.3.19/brainframe_apps/__init__.py
+-rw-r--r--   0        0        0     4847 2023-04-10 05:04:21.218631 brainframe_apps-0.3.19/brainframe_apps/add_stream.py
+-rw-r--r--   0        0        0      665 2022-12-19 23:19:56.515826 brainframe_apps-0.3.19/brainframe_apps/bf_log_print.py
+-rw-r--r--   0        0        0    14973 2023-04-09 00:36:55.997030 brainframe_apps-0.3.19/brainframe_apps/capsule_control.py
+-rw-r--r--   0        0        0     1115 2023-04-09 03:58:17.840070 brainframe_apps-0.3.19/brainframe_apps/cli.py
+-rw-r--r--   0        0        0      571 2023-04-08 04:43:59.581232 brainframe_apps-0.3.19/brainframe_apps/command_utils.py
+-rw-r--r--   0        0        0     2582 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/delete_stream.py
+-rw-r--r--   0        0        0     4691 2022-12-19 23:19:56.515826 brainframe_apps-0.3.19/brainframe_apps/fps_report.py
+-rw-r--r--   0        0        0     6343 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/get_configuration.py
+-rw-r--r--   0        0        0     8070 2023-04-09 00:36:44.237108 brainframe_apps-0.3.19/brainframe_apps/get_zone_statuses.py
+-rw-r--r--   0        0        0     4733 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/identity_control.py
+-rw-r--r--   0        0        0     2434 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/license_control.py
+-rw-r--r--   0        0        0     6284 2023-04-09 00:36:44.213108 brainframe_apps-0.3.19/brainframe_apps/list_stream.py
+-rw-r--r--   0        0        0     2903 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/logger_factory.py
+-rw-r--r--   0        0        0      734 2023-04-09 00:33:40.814733 brainframe_apps-0.3.19/brainframe_apps/print_utils.py
+-rw-r--r--   0        0        0     4455 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/process_image.py
+-rw-r--r--   0        0        0     9613 2023-04-10 05:04:21.218631 brainframe_apps-0.3.19/brainframe_apps/set_configuration.py
+-rw-r--r--   0        0        0     3909 2023-04-10 05:04:21.218631 brainframe_apps-0.3.19/brainframe_apps/start_analyzing.py
+-rw-r--r--   0        0        0     2153 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/stop_analyzing.py
+-rw-r--r--   0        0        0     1046 2022-12-19 23:19:56.519826 brainframe_apps-0.3.19/brainframe_apps/time_utils.py
+-rw-r--r--   0        0        0      862 2023-04-09 04:06:05.729507 brainframe_apps-0.3.19/brainframe_apps/translations/portal.en.yml
+-rw-r--r--   0        0        0     3064 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/urls.py
+-rw-r--r--   0        0        0     1037 2023-04-09 00:36:34.917171 brainframe_apps-0.3.19/brainframe_apps/wait_for_ready.py
+-rw-r--r--   0        0        0      783 2023-04-10 23:39:20.670023 brainframe_apps-0.3.19/pyproject.toml
+-rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 brainframe_apps-0.3.19/setup.py
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 brainframe_apps-0.3.19/PKG-INFO
```

### Comparing `brainframe_apps-0.3.18/brainframe_apps/__init__.py` & `brainframe_apps-0.3.19/brainframe_apps/__init__.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/add_stream.py` & `brainframe_apps-0.3.19/brainframe_apps/add_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,44 +92,46 @@
     server_url = args.server_url
     log.debug(
         f"{os.path.basename(sys.argv[0])} Waiting for BrainFrame server at '{server_url}'"
     )
     api = BrainFrameAPI(server_url)
     api.wait_for_server_initialization()
 
-    if args.stream_url_list is not None:
+    if args.stream_url is not None:
+        stream_url = args.stream_url
+        stream_configuration = add_stream(api, args.video_file, stream_url, False)
+    elif args.video_file is not None:
+        stream_configuration = add_stream(api, args.video_file, None, False)
+    elif args.stream_url_list is not None:
         stream_url_list = UrlList(args.stream_url_list)
         if stream_url_list:
             stream_configuration = None
             for stream_url in stream_url_list:
                 stream_configuration = add_stream(
                     api, args.video_file, stream_url, False
                 )
         else:
             log.debug(f"Read {args.stream_url_list} failed")
-    elif args.stream_url is not None:
-        stream_url = args.stream_url
-        stream_configuration = add_stream(api, args.video_file, stream_url, False)
-    elif args.video_file is not None:
-        stream_configuration = add_stream(api, args.video_file, None, False)
     else:
         log.debug("No video source input")
 
 
 def _add_stream_parse_args(parser):
     parser.add_argument(
-        "--video-file", default=None, help="video file name. Default: %(default)s"
+        "--video-file",
+        default=None,
+        help="video file name. Default: %(default)s",
     )
     parser.add_argument(
         "--stream-name",
         default="My video file",
         help="The name of the automatically-generated BrainFrame stream",
     )
     parser.add_argument(
         "--stream-url-list",
-        default=None,
+        default="stream-url.list",
         help="The name of the file with the list of stream urls. Default: %(default)s",
     )
 
 
 if __name__ == "__main__":
     by_name["add_stream"]()
```

### Comparing `brainframe_apps-0.3.18/brainframe_apps/bf_log_print.py` & `brainframe_apps-0.3.19/brainframe_apps/bf_log_print.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/capsule_control.py` & `brainframe_apps-0.3.19/brainframe_apps/capsule_control.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/cli.py` & `brainframe_apps-0.3.19/brainframe_apps/cli.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/command_utils.py` & `brainframe_apps-0.3.19/brainframe_apps/command_utils.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/delete_stream.py` & `brainframe_apps-0.3.19/brainframe_apps/delete_stream.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/fps_report.py` & `brainframe_apps-0.3.19/brainframe_apps/fps_report.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/get_configuration.py` & `brainframe_apps-0.3.19/brainframe_apps/get_configuration.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/get_zone_statuses.py` & `brainframe_apps-0.3.19/brainframe_apps/get_zone_statuses.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/identity_control.py` & `brainframe_apps-0.3.19/brainframe_apps/identity_control.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/license_control.py` & `brainframe_apps-0.3.19/brainframe_apps/license_control.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/list_stream.py` & `brainframe_apps-0.3.19/brainframe_apps/list_stream.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/logger_factory.py` & `brainframe_apps-0.3.19/brainframe_apps/logger_factory.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/print_utils.py` & `brainframe_apps-0.3.19/brainframe_apps/print_utils.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/process_image.py` & `brainframe_apps-0.3.19/brainframe_apps/process_image.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/set_configuration.py` & `brainframe_apps-0.3.19/brainframe_apps/set_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,19 +198,21 @@
 def _set_configuration_parse_args(parser):
     parser.add_argument(
         "--server-url",
         default="http://localhost",
         help="The BrainFrame server URL. Default: %(default)s",
     )
     parser.add_argument(
-        "--setting-file", required=True, help="File to store the server settings"
+        "--setting-file",
+        default="settings.json",
+        help="File to store the server settings",
     )
     parser.add_argument(
         "--stream-url-list",
-        default=None,
+        default="stream-url.list",
         help="The name of the file with the list of stream urls. Default: %(default)s",
     )
     parser.add_argument(
         "--video-file", default=None, help="video file name. Default: %(default)s"
     )
     parser.add_argument(
         "--stream-url", default=None, help="The ip camera URL. Default: %(default)s"
@@ -234,36 +236,36 @@
         api.wait_for_server_initialization(timeout=15)
     except (TimeoutError, bf_errors.ServerNotReadyError):
         log.error(f"BrainFrame server connection timeout")
         return
 
     set_conf_global(None, None, args.setting_file, api, False)
 
-    stream_url_list = UrlList(args.stream_url_list)
-    if stream_url_list:
-        for stream_url in stream_url_list:
-            stream_id = set_conf_stream(
-                args.video_file, stream_url, args.setting_file, api, False
-            )
-            if stream_id is not None:
-                log.debug(f"Loading for {stream_url} has succeeded")
-            else:
-                log.error(f"Loading for {stream_url} has failed.")
+    if args.stream_url is not None:
+        stream_url = args.stream_url.replace("localhost", str(get_ip()))
 
+        stream_id = set_conf_stream(
+            args.video_file, stream_url, args.setting_file, api, False
+        )
+        if stream_id is not None:
+            log.debug(f"Loading for {stream_url} has succeeded.")
+        else:
+            log.error(f"Loading for {stream_url} has failed.")
     else:
-        if args.stream_url is not None:
-            stream_url = args.stream_url.replace("localhost", str(get_ip()))
-
-            stream_id = set_conf_stream(
-                args.video_file, stream_url, args.setting_file, api, False
-            )
-            if stream_id is not None:
-                log.debug(f"Loaded for {stream_url}")
-            else:
-                log.error(f"Loading for {stream_url} has failed")
+        stream_url_list = UrlList(args.stream_url_list)
+        if stream_url_list:
+            for stream_url in stream_url_list:
+                stream_id = set_conf_stream(
+                    args.video_file, stream_url, args.setting_file, api, False
+                )
+                if stream_id is not None:
+                    log.debug(f"Loading for {stream_url} has succeeded.")
+                else:
+                    log.error(f"Loading for {stream_url} has failed.")
+    
         else:
             log.error(
                 "At least one of stream_url or stream_url_list has to be provided"
             )
 
 
 if __name__ == "__main__":
```

### Comparing `brainframe_apps-0.3.18/brainframe_apps/start_analyzing.py` & `brainframe_apps-0.3.19/brainframe_apps/start_analyzing.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     except (TimeoutError, bf_errors.ServerNotReadyError):
         log.error(f"BrainFrame server connection timeout")
         return
 
     if args.stream_url is not None:
         stream_url = args.stream_url.replace("localhost", str(get_ip()))
 
-        stream_id = start_analyzing(api, stream_persistent_id, True)
+        stream_id = start_analyzing(api, stream_url, True)
 
     else:
         stop_analyzing_all(api)
 
 
 if __name__ == "__main__":
     by_name["start_analyzing"]()
```

### Comparing `brainframe_apps-0.3.18/brainframe_apps/stop_analyzing.py` & `brainframe_apps-0.3.19/brainframe_apps/stop_analyzing.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/time_utils.py` & `brainframe_apps-0.3.19/brainframe_apps/time_utils.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/translations/portal.en.yml` & `brainframe_apps-0.3.19/brainframe_apps/translations/portal.en.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 en:
-  description: "Use Python API Apps to interact with brainframe server through
-  REST APIs. To see more options, run \"brainframe_apps {command} --help\"."
+  description: "brainframe-apps is a group of commands written in Python. They
+  use BrainFrame REST APIs to interact with brainframe server. To see options
+  of each command, run \"brainframe_apps {command} --help\"."
   usage: >-
     brainframe_apps <command> [<args>]
 
-    Commands:
+    commands:
       add_stream
       delete_stream
       list_stream
       load_settings
       save_settings
       start_analyzing
       stop_analyzing
@@ -19,10 +20,10 @@
       license_control
 
     Examples:
       brainframe_apps add_stream --server-url SERVER_URL --stream-url STREAM_URL
       brainframe_apps add_stream --help
       brainframe_apps start_analyzing
  
-  command-help: "The brainframe Python API App to run"
+  command-help: "The brainframe-apps command to run"
   unknown-command: "Unknown command: {command}"
   interrupted: "The operation was interrupted"
```

### Comparing `brainframe_apps-0.3.18/brainframe_apps/urls.py` & `brainframe_apps-0.3.19/brainframe_apps/urls.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/brainframe_apps/wait_for_ready.py` & `brainframe_apps-0.3.19/brainframe_apps/wait_for_ready.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.18/pyproject.toml` & `brainframe_apps-0.3.19/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brainframe-apps"
-version = "0.3.18"
+version = "0.3.19"
 description = "BrainFrame Apps use BrainFrame REST API to interact with the BrainFrame OS"
 authors = ["Stephen Li <stephen@dilililabs.com>"]
 license = "BSD License"
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `brainframe_apps-0.3.18/setup.py` & `brainframe_apps-0.3.19/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['brainframe-api>=0.29.1,<0.30.0']
 
 entry_points = \
 {'console_scripts': ['brainframe-apps = brainframe_apps.cli:cli_main']}
 
 setup_kwargs = {
     'name': 'brainframe-apps',
-    'version': '0.3.18',
+    'version': '0.3.19',
     'description': 'BrainFrame Apps use BrainFrame REST API to interact with the BrainFrame OS',
     'long_description': 'None',
     'author': 'Stephen Li',
     'author_email': 'stephen@dilililabs.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `brainframe_apps-0.3.18/PKG-INFO` & `brainframe_apps-0.3.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainframe-apps
-Version: 0.3.18
+Version: 0.3.19
 Summary: BrainFrame Apps use BrainFrame REST API to interact with the BrainFrame OS
 License: BSD License
 Author: Stephen Li
 Author-email: stephen@dilililabs.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
```

