# Comparing `tmp/infra_flow-1.0.10-py3-none-any.whl.zip` & `tmp/infra_flow-1.0.11-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3170 bytes, number of entries: 9
+Zip file size: 3246 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 08:03 infra_enver/__init__.py
--rw-r--r--  2.0 unx      319 b- defN 23-Apr-11 09:05 infra_enver/cache.py
--rw-r--r--  2.0 unx      138 b- defN 23-Apr-11 09:05 infra_enver/config.py
--rw-r--r--  2.0 unx     2133 b- defN 23-Apr-11 09:35 infra_enver/infra_enver.py
+-rw-r--r--  2.0 unx      319 b- defN 23-Apr-11 13:06 infra_enver/cache.py
+-rw-r--r--  2.0 unx       75 b- defN 23-Apr-11 13:02 infra_enver/config.py
+-rw-r--r--  2.0 unx     2556 b- defN 23-Apr-11 13:06 infra_enver/infra_enver.py
 -rw-r--r--  2.0 unx       47 b- defN 23-Apr-11 08:03 infra_enver/infra_enver_exceptions.py
--rw-r--r--  2.0 unx      574 b- defN 23-Apr-11 12:04 infra_flow-1.0.10.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 12:04 infra_flow-1.0.10.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-11 12:04 infra_flow-1.0.10.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      718 b- defN 23-Apr-11 12:04 infra_flow-1.0.10.dist-info/RECORD
-9 files, 4033 bytes uncompressed, 1922 bytes compressed:  52.3%
+-rw-r--r--  2.0 unx      597 b- defN 23-Apr-11 13:10 infra_flow-1.0.11.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 13:10 infra_flow-1.0.11.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-11 13:10 infra_flow-1.0.11.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      717 b- defN 23-Apr-11 13:10 infra_flow-1.0.11.dist-info/RECORD
+9 files, 4415 bytes uncompressed, 1998 bytes compressed:  54.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: infra_enver/infra_enver.py
 Comment: 
 
 Filename: infra_enver/infra_enver_exceptions.py
 Comment: 
 
-Filename: infra_flow-1.0.10.dist-info/METADATA
+Filename: infra_flow-1.0.11.dist-info/METADATA
 Comment: 
 
-Filename: infra_flow-1.0.10.dist-info/WHEEL
+Filename: infra_flow-1.0.11.dist-info/WHEEL
 Comment: 
 
-Filename: infra_flow-1.0.10.dist-info/top_level.txt
+Filename: infra_flow-1.0.11.dist-info/top_level.txt
 Comment: 
 
-Filename: infra_flow-1.0.10.dist-info/RECORD
+Filename: infra_flow-1.0.11.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## infra_enver/config.py

```diff
@@ -1,3 +1,2 @@
-BASE_URL = 'infra_backend'
-SETTINGS_URL = f'http://{BASE_URL}/setting/project/'
-EXPERIMENT_URL = f'http://{BASE_URL}/experiment/project/'
+SETTINGS_URL = '/setting/project/'
+EXPERIMENT_URL = '/experiment/project/'
```

## infra_enver/infra_enver.py

```diff
@@ -5,15 +5,22 @@
 from . import cache
 import redis
 
 REQUEST_TIME_OUT = 5
 
 
 class Enver(object):
-    """infra_enver class"""
+    """
+    Attributes:
+        service_url - url of settings service.
+
+        is_fallback_enabled - if lib can't get setting from redis,
+            infra_enver will try to get setting directly from settings service.
+    """
+
     project_name: str
     secret_key: str
     is_fallback_enabled: bool
     redis_connection: redis.Redis
 
     def __getattr__(self, item):
         return self.get_setting(item)
@@ -21,44 +28,49 @@
     def __init__(
             self,
             project_name: str,
             secret_key: str,
             redis_host: str,
             redis_db_num: int,
             redis_password: str,
+            service_url: str,
             is_fallback_enabled: bool = False,
     ):
         self.project_name = project_name
         self.secret_key = secret_key
         self.is_fallback_enabled = is_fallback_enabled
         self.redis_connection = redis.Redis(host=redis_host, port=6379, db=redis_db_num, password=redis_password)
+        self.settings_service_url = service_url + config.SETTINGS_URL
+        self.experiments_service_url = service_url + config.EXPERIMENT_URL
 
     def get_setting(self, setting_name: str):
         try:
             return cache.get_value(self.redis_connection, setting_name)
         except Exception as ex:
             if self.is_fallback_enabled:
                 json = {
                     "project_name": self.project_name,
                     "secret_key": self.secret_key
                 }
-                r = requests.post(config.SETTINGS_URL + setting_name, json=json, timeout=REQUEST_TIME_OUT)
+                r = requests.post(self.settings_service_url + setting_name, json=json, timeout=REQUEST_TIME_OUT)
                 if not r.ok:
                     raise ee.InfraEnverException(r.text)
                 return r.json()['value']
             raise ee.InfraEnverException(ex)
 
     def get_experiment(self, experiment_name: str, arg: t.Any, fallback_value: t.Any = None):
         json = {
             "project_name": self.project_name,
             "secret_key": self.secret_key,
             "experiment_name": experiment_name,
             "arg": arg
         }
         try:
-            r = requests.post(config.EXPERIMENT_URL, json=json, timeout=REQUEST_TIME_OUT)
-            return r.json() if r.ok else fallback_value
+            r = requests.post(self.experiments_service_url, json=json, timeout=REQUEST_TIME_OUT)
+            if not r.ok:
+                return fallback_value
+            return r.json()
         except Exception as ex:
             if fallback_value is not None:
                 return fallback_value
             else:
                 raise ee.InfraEnverException(str(ex))
```

## Comparing `infra_flow-1.0.10.dist-info/METADATA` & `infra_flow-1.0.11.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infra-flow
-Version: 1.0.10
+Version: 1.0.11
 Summary: Infra Enver
 Author: Daniil Vladimirov
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: pydantic
 Requires-Dist: redis
@@ -14,15 +14,15 @@
 example
 ```py
 from infra_enver import infra_enver
 import random
 
 
 if __name__ == '__main__':
-    env = infra_enver.Enver("galaxy", "pass", "localhost", 2, "pass")
+    env = infra_enver.Enver("galaxy", "pass", "localhost", 2, "pass", "https://service.com")
 
     # get setting
     print(env.MY_SETT)
 
     # experiment
     for i in range(10):
         print(env.get_experiment("TEST_EXP_2", random.randint(3, 1000000)))
```

