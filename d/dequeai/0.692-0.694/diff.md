# Comparing `tmp/dequeai-0.692.tar.gz` & `tmp/dequeai-0.694.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.692.tar", last modified: Sun Apr  9 14:40:09 2023, max compression
+gzip compressed data, was "dequeai-0.694.tar", last modified: Tue Apr 11 16:20:07 2023, max compression
```

## Comparing `dequeai-0.692.tar` & `dequeai-0.694.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:40:09.833147 dequeai-0.692/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-09 14:40:09.833147 dequeai-0.692/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:40:09.833147 dequeai-0.692/dequeai/
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.692/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15374 2023-03-27 20:38:54.000000 dequeai-0.692/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.692/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.692/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.692/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    20356 2023-04-09 14:39:36.000000 dequeai-0.692/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.692/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.692/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.692/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.692/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:40:09.833147 dequeai-0.692/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-09 14:40:09.000000 dequeai-0.692/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-09 14:40:09.000000 dequeai-0.692/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 14:40:09.000000 dequeai-0.692/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-09 14:40:09.000000 dequeai-0.692/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-09 14:40:09.000000 dequeai-0.692/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 14:40:09.833147 dequeai-0.692/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-09 14:39:56.000000 dequeai-0.692/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:20:07.455488 dequeai-0.694/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 16:20:07.455488 dequeai-0.694/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:20:07.451488 dequeai-0.694/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.694/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15374 2023-03-27 20:38:54.000000 dequeai-0.694/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.694/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.694/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.694/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    20490 2023-04-11 16:19:53.000000 dequeai-0.694/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.694/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.694/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.694/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.694/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:20:07.455488 dequeai-0.694/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 16:20:06.000000 dequeai-0.694/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-11 16:20:07.000000 dequeai-0.694/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 16:20:07.000000 dequeai-0.694/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-04-11 16:20:07.000000 dequeai-0.694/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 16:20:07.000000 dequeai-0.694/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 16:20:07.455488 dequeai-0.694/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-11 16:19:53.000000 dequeai-0.694/setup.py
```

### Comparing `dequeai-0.692/dequeai/datatypes.py` & `dequeai-0.694/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.692/dequeai/dequeai.py` & `dequeai-0.694/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.692/dequeai/dequeai_run.py` & `dequeai-0.694/dequeai/dequeai_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,15 +419,16 @@
                              json=req_data)
         res = resp.json()
         print(res)
 
     def load_artifact(self,  artifact_type, run_id):
         # Fetch artifact metadata
 
-
+        if self.user_name is None:
+            raise ValueError("Please initialize using dequeai.init() before calling load_artifact")
         req_data = {
             "user_name": self.user_name,
             "run_id": run_id,
             "artifact_type": artifact_type
         }
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/artifact/metadata/read/", json=req_data)
         metadata = resp.json()
```

### Comparing `dequeai-0.692/dequeai/parsing_service.py` & `dequeai-0.694/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.692/dequeai/rest_connect.py` & `dequeai-0.694/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.692/dequeai/util.py` & `dequeai-0.694/dequeai/util.py`

 * *Files identical despite different names*

