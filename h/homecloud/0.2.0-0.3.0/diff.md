# Comparing `tmp/homecloud-0.2.0.tar.gz` & `tmp/homecloud-0.3.0.tar.gz`

## Comparing `homecloud-0.2.0.tar` & `homecloud-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 homecloud-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 homecloud-0.2.0/src/homecloud/__init__.py
--rw-r--r--   0        0        0     6542 2020-02-02 00:00:00.000000 homecloud-0.2.0/src/homecloud/client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 homecloud-0.2.0/src/homecloud/client_settings.toml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 homecloud-0.2.0/src/homecloud/client_subclass.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 homecloud-0.2.0/src/homecloud/get_routes.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 homecloud-0.2.0/src/homecloud/homecloud_config.toml
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 homecloud-0.2.0/src/homecloud/homecloud_generator.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 homecloud-0.2.0/src/homecloud/homecloud_logging.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 homecloud-0.2.0/src/homecloud/homecloud_utils.py
--rw-r--r--   0        0        0    10837 2020-02-02 00:00:00.000000 homecloud-0.2.0/src/homecloud/module_to_api.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 homecloud-0.2.0/src/homecloud/post_routes.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 homecloud-0.2.0/src/homecloud/request_models.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 homecloud-0.2.0/src/homecloud/router_template.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 homecloud-0.2.0/src/homecloud/server.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 homecloud-0.2.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 homecloud-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 homecloud-0.2.0/README.md
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 homecloud-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 homecloud-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 homecloud-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/__init__.py
+-rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/client_settings.toml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/client_subclass.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/get_routes.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/homecloud_config.toml
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/homecloud_generator.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/homecloud_logging.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/homecloud_utils.py
+-rw-r--r--   0        0        0    10837 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/module_to_api.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/post_routes.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/request_models.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/router_template.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/server.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 homecloud-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 homecloud-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 homecloud-0.3.0/README.md
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 homecloud-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 homecloud-0.3.0/PKG-INFO
```

### Comparing `homecloud-0.2.0/CHANGELOG.md` & `homecloud-0.3.0/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,30 @@
 # Changelog
 
-## 0.1.0 (2023-03-11)
+## 0.2.0 (2023-04-03)
+
+#### New Features
+
+* add log_path param to client and logging files to override default behavior
+#### Refactorings
+
+* replace pathlib.Path with pathier.Pathier
+#### Others
+
+* remove unused imports from client.py
+
+
+## v0.1.1 (2023-03-22)
+
+#### Others
+
+* build v0.1.1
+
+
+## v0.1.0 (2023-03-11)
 
 #### New Features
 
 * check for previous server before scanning
 * add check to see if previous server is active
 * add save_server func
 * add func to save config
@@ -15,14 +35,16 @@
 
 * fix request_model import replacement
 #### Performance improvements
 
 * shrink default port range
 #### Others
 
+* build v0.1.0
+* update changelog
 * update test
 
 
 ## v0.0.0 (2023-03-06)
 
 #### New Features
```

### Comparing `homecloud-0.2.0/src/homecloud/client.py` & `homecloud-0.3.0/src/homecloud/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,24 @@
         counter = 0
         while True:
             try:
                 output = func(self, *args, **kwargs)
                 break
             except Exception as e:
                 print("Error contacting server")
-                print(str(e))
+                print(e)
                 print(f"Retrying in {counter}s")
                 time.sleep(counter)
                 if counter < 60:
                     counter += 1
                 # After three consecutive fails,
                 # start scanning for the server running
                 # on a different ip and/or port
                 if counter > 2:
                     self.server_url = self.wheres_my_server()
-        if self.send_logs and (
-            len(self.log_stream.getvalue().splitlines()) >= self.log_send_thresh
-        ):
-            self.push_logs()
         return output
 
     return inner
 
 
 class HomeCloudClient:
     def __init__(
@@ -157,22 +153,26 @@
 
         :param resource: The path location of the requested resource
         (e.g. /users/me).
 
         :param data: The request body.
 
         :param params: Url parameters."""
+        # Push logs if applicable
+        if self.send_logs and (
+            len(self.log_stream.getvalue().splitlines()) >= self.log_send_thresh
+        ):
+            self.push_logs()
         data |= self.base_payload
         url = f"{self.server_url}{resource}"
         data = json.dumps(data)
         return requests.request(
             method, url, data=data, params=params, timeout=self.timeout
         )
 
     def push_logs(self):
         """Push log stream to the server."""
         self.logger.info(f"Pushing log stream to {self.app_name} server.")
-        self.send_request(
-            "post", "/clientlogs", data={"log_stream": self.log_stream.getvalue()}
-        )
+        log_stream = self.log_stream.getvalue()
         self.log_stream.truncate(0)
         self.log_stream.seek(0)
+        self.send_request("post", "/clientlogs", data={"log_stream": log_stream})
```

### Comparing `homecloud-0.2.0/src/homecloud/client_subclass.py` & `homecloud-0.3.0/src/homecloud/client_subclass.py`

 * *Files identical despite different names*

### Comparing `homecloud-0.2.0/src/homecloud/get_routes.py` & `homecloud-0.3.0/src/homecloud/get_routes.py`

 * *Files identical despite different names*

### Comparing `homecloud-0.2.0/src/homecloud/homecloud_generator.py` & `homecloud-0.3.0/src/homecloud/homecloud_generator.py`

 * *Files identical despite different names*

### Comparing `homecloud-0.2.0/src/homecloud/homecloud_logging.py` & `homecloud-0.3.0/src/homecloud/homecloud_logging.py`

 * *Files identical despite different names*

### Comparing `homecloud-0.2.0/src/homecloud/homecloud_utils.py` & `homecloud-0.3.0/src/homecloud/homecloud_utils.py`

 * *Files identical despite different names*

### Comparing `homecloud-0.2.0/src/homecloud/module_to_api.py` & `homecloud-0.3.0/src/homecloud/module_to_api.py`

 * *Files identical despite different names*

### Comparing `homecloud-0.2.0/src/homecloud/server.py` & `homecloud-0.3.0/src/homecloud/server.py`

 * *Files identical despite different names*

### Comparing `homecloud-0.2.0/LICENSE.txt` & `homecloud-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `homecloud-0.2.0/README.md` & `homecloud-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `homecloud-0.2.0/pyproject.toml` & `homecloud-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 000000a0: 7468 6520 7465 6d70 6c61 7465 2066 696c  the template fil
 000000b0: 6573 206e 6565 6465 6420 746f 2069 6e74  es needed to int
 000000c0: 6567 7261 7465 2066 6173 7461 7069 2c20  egrate fastapi, 
 000000d0: 7576 6963 6f72 6e2c 2061 6e64 2061 2072  uvicorn, and a r
 000000e0: 6571 7565 7374 7320 6261 7365 6420 636c  equests based cl
 000000f0: 6965 6e74 2069 6e74 6f20 6120 5079 7468  ient into a Pyth
 00000100: 6f6e 2070 726f 6a65 6374 2e22 0d0a 7665  on project."..ve
-00000110: 7273 696f 6e20 3d20 2230 2e32 2e30 220d  rsion = "0.2.0".
+00000110: 7273 696f 6e20 3d20 2230 2e33 2e30 220d  rsion = "0.3.0".
 00000120: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
 00000130: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 00000140: 656e 6465 6e63 6965 7320 3d20 5b22 7265  endencies = ["re
 00000150: 7175 6573 7473 222c 2022 746f 6d6c 6b69  quests", "tomlki
 00000160: 7422 2c20 2270 7964 616e 7469 6322 2c20  t", "pydantic", 
 00000170: 2262 6c61 636b 222c 2022 6661 7374 6170  "black", "fastap
 00000180: 6922 2c20 226c 616e 7574 696c 7322 2c20  i", "lanutils",
```

### Comparing `homecloud-0.2.0/PKG-INFO` & `homecloud-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homecloud
-Version: 0.2.0
+Version: 0.3.0
 Summary: A command line tool for generating the template files needed to integrate fastapi, uvicorn, and a requests based client into a Python project.
 Project-URL: Homepage, https://github.com/matt-manes/homecloud
 Project-URL: Documentation, https://github.com/matt-manes/homecloud/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/homecloud/tree/main/src/homecloud
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: api,client,fastapi,network,server
```

