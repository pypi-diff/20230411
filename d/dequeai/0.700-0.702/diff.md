# Comparing `tmp/dequeai-0.700.tar.gz` & `tmp/dequeai-0.702.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.700.tar", last modified: Tue Apr 11 16:27:39 2023, max compression
+gzip compressed data, was "dequeai-0.702.tar", last modified: Tue Apr 11 17:33:28 2023, max compression
```

## Comparing `dequeai-0.700.tar` & `dequeai-0.702.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:39.093743 dequeai-0.700/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 16:27:39.093743 dequeai-0.700/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:39.093743 dequeai-0.700/dequeai/
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.700/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.700/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.700/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.700/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.700/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    20492 2023-04-11 16:27:02.000000 dequeai-0.700/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.700/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.700/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.700/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.700/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:39.093743 dequeai-0.700/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 16:27:38.000000 dequeai-0.700/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-11 16:27:39.000000 dequeai-0.700/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 16:27:38.000000 dequeai-0.700/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-11 16:27:38.000000 dequeai-0.700/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 16:27:39.000000 dequeai-0.700/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 16:27:39.093743 dequeai-0.700/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      470 2023-04-11 16:27:24.000000 dequeai-0.700/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:33:28.547530 dequeai-0.702/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 17:33:28.547530 dequeai-0.702/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:33:28.547530 dequeai-0.702/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.702/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.702/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.702/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.702/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.702/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    21008 2023-04-11 17:28:02.000000 dequeai-0.702/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.702/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.702/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.702/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.702/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:33:28.547530 dequeai-0.702/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 17:33:28.000000 dequeai-0.702/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-11 17:33:28.000000 dequeai-0.702/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 17:33:28.000000 dequeai-0.702/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-11 17:33:28.000000 dequeai-0.702/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 17:33:28.000000 dequeai-0.702/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 17:33:28.547530 dequeai-0.702/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      470 2023-04-11 17:33:15.000000 dequeai-0.702/setup.py
```

### Comparing `dequeai-0.700/dequeai/datatypes.py` & `dequeai-0.702/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.700/dequeai/dequeai.py` & `dequeai-0.702/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.700/dequeai/dequeai_run.py` & `dequeai-0.702/dequeai/dequeai_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,26 +82,29 @@
         self._running = False
         self._environment_logged = False
 
         self._resources_logged = False
         self._res_monitor = None
         self._run_start_time =None
 
-    def init(self, user_name, project_name=None, api_key=None):
+    def init(self, user_name, api_key,project_name=None):
         os.environ["running"] = "yes"
-        self._run_start_time = datetime.datetime.now()
-        self._running = True
+
         self.user_name = user_name
 
         self._api_key = api_key
 
         is_authenticated = self._authenticate()
         if not is_authenticated:
+            self.user_name = None
             raise ValueError("Invalid user and/or api key")
 
+        self._run_start_time = datetime.datetime.now()
+        self._running = True
+
         self._workload_type = os.getenv("workload_type")
         self._workload_id = os.getenv("workload_id")
         self._submission_id = os.getenv("submission_id")
         self._agent_id = os.getenv("agent_id")
 
         if project_name is None:
             if self._workload_id is None:
@@ -462,15 +465,15 @@
     def _validate_data(self, data):
         for key, value in data.items():
             if type(value) is dict:
                 self._validate_data(value)
             else:
                 # print(type(value))
                 if type(value) in [Audio, BoundingBox2D, Histogram,Table,
-                                   Image, Plot] or type(value) in types.__builtins__.values():
+                                   Image] or type(value) in types.__builtins__.values():
                     pass
                 else:
                     raise ValueError(
                         "Invalid type in dictionary. Allowed values include builtin types and Deque data types " + str(
                             type(value)) + " " + str(value.__class__.__module__))
 
     def _validate_hyperparams(self, hyperparams):
@@ -484,15 +487,33 @@
                         type(value)) + " " + str(value.__class__.__module__))
 
     def _send_upstream(self):
         self._rest.post(url=AGENT_API_SERVICE_URL + "/fex/python/track/", json=self._history)
         self._history = dict()
 
     def _authenticate(self):
-        return True
+        # Download the artifacts using the artifact URIs
+
+            req_data = {
+                "user_name": self.user_name,
+                "api_key": self._api_key
+            }
+            resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/authenticate/sdk/", json=req_data)
+
+            res = resp.json()
+
+            # Download the artifact using the pre-signed URL
+            if "authenticated" in res:
+                return res["authenticated"]
+            else:
+                return False
+
+
+
+
 
 
 if __name__ == "__main__":
     deque = Run()
     deque._validate_hyperparams({"train": {"accuracy": "1.3", "loss": "2.2"}})
     #deque.log_artifact_task(artifact_type=RESOURCES, path="//dequeapp.egg-info",
        #                     run_meta_data=None)
```

### Comparing `dequeai-0.700/dequeai/parsing_service.py` & `dequeai-0.702/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.700/dequeai/rest_connect.py` & `dequeai-0.702/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.700/dequeai/util.py` & `dequeai-0.702/dequeai/util.py`

 * *Files identical despite different names*

