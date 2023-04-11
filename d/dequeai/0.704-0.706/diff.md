# Comparing `tmp/dequeai-0.704.tar.gz` & `tmp/dequeai-0.706.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.704.tar", last modified: Tue Apr 11 20:08:43 2023, max compression
+gzip compressed data, was "dequeai-0.706.tar", last modified: Tue Apr 11 20:12:09 2023, max compression
```

## Comparing `dequeai-0.704.tar` & `dequeai-0.706.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:08:43.394833 dequeai-0.704/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 20:08:43.394833 dequeai-0.704/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:08:43.394833 dequeai-0.704/dequeai/
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.704/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.704/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.704/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.704/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.704/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    21010 2023-04-11 20:07:20.000000 dequeai-0.704/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.704/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.704/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.704/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.704/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:08:43.394833 dequeai-0.704/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 20:08:42.000000 dequeai-0.704/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-11 20:08:43.000000 dequeai-0.704/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 20:08:42.000000 dequeai-0.704/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-11 20:08:43.000000 dequeai-0.704/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 20:08:43.000000 dequeai-0.704/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 20:08:43.394833 dequeai-0.704/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      470 2023-04-11 20:08:29.000000 dequeai-0.704/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:12:09.679859 dequeai-0.706/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 20:12:09.679859 dequeai-0.706/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:12:09.679859 dequeai-0.706/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.706/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.706/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.706/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.706/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.706/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    21101 2023-04-11 20:11:48.000000 dequeai-0.706/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.706/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.706/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.706/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.706/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:12:09.679859 dequeai-0.706/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 20:12:09.000000 dequeai-0.706/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-11 20:12:09.000000 dequeai-0.706/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 20:12:09.000000 dequeai-0.706/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-11 20:12:09.000000 dequeai-0.706/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 20:12:09.000000 dequeai-0.706/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 20:12:09.679859 dequeai-0.706/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      470 2023-04-11 20:11:56.000000 dequeai-0.706/setup.py
```

### Comparing `dequeai-0.704/dequeai/datatypes.py` & `dequeai-0.706/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.704/dequeai/dequeai.py` & `dequeai-0.706/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.704/dequeai/dequeai_run.py` & `dequeai-0.706/dequeai/dequeai_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,18 +493,20 @@
     def _authenticate(self):
         # Download the artifacts using the artifact URIs
 
             req_data = {
                 "user_name": self.user_name,
                 "api_key": self._api_key
             }
+            print(AGENT_API_SERVICE_URL + "/fex/authenticate/sdk/")
             resp = self._rest.post(url=AGENT_API_SERVICE_URL + "/fex/authenticate/sdk/", json=req_data)
 
             res = resp.json()
 
+            print(res)
             # Download the artifact using the pre-signed URL
             if "authenticated" in res:
                 return res["authenticated"]
             else:
                 return False
```

### Comparing `dequeai-0.704/dequeai/parsing_service.py` & `dequeai-0.706/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.704/dequeai/rest_connect.py` & `dequeai-0.706/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.704/dequeai/util.py` & `dequeai-0.706/dequeai/util.py`

 * *Files identical despite different names*

