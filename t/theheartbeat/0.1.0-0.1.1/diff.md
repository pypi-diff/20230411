# Comparing `tmp/theheartbeat-0.1.0.tar.gz` & `tmp/theheartbeat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theheartbeat-0.1.0.tar", last modified: Thu Apr  6 06:32:43 2023, max compression
+gzip compressed data, was "theheartbeat-0.1.1.tar", last modified: Tue Apr 11 11:57:51 2023, max compression
```

## Comparing `theheartbeat-0.1.0.tar` & `theheartbeat-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-06 06:32:43.311631 theheartbeat-0.1.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1689 2023-04-06 06:24:02.000000 theheartbeat-0.1.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      497 2023-04-06 06:32:43.311631 theheartbeat-0.1.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1396 2023-04-06 06:10:19.000000 theheartbeat-0.1.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-06 06:32:43.307631 theheartbeat-0.1.0/heartbeat/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      393 2023-04-05 11:31:29.000000 theheartbeat-0.1.0/heartbeat/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2447 2023-04-05 11:59:19.000000 theheartbeat-0.1.0/heartbeat/heartbeat.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-04-06 06:32:43.311631 theheartbeat-0.1.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      606 2023-04-06 06:32:33.000000 theheartbeat-0.1.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-06 06:32:43.311631 theheartbeat-0.1.0/theheartbeat.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      497 2023-04-06 06:32:43.000000 theheartbeat-0.1.0/theheartbeat.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      260 2023-04-06 06:32:43.000000 theheartbeat-0.1.0/theheartbeat.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-06 06:32:43.000000 theheartbeat-0.1.0/theheartbeat.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-04-06 06:32:43.000000 theheartbeat-0.1.0/theheartbeat.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-04-06 06:32:43.000000 theheartbeat-0.1.0/theheartbeat.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-11 11:57:51.717871 theheartbeat-0.1.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1689 2023-04-06 06:24:02.000000 theheartbeat-0.1.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      517 2023-04-11 11:57:51.717871 theheartbeat-0.1.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1396 2023-04-06 06:10:19.000000 theheartbeat-0.1.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-11 11:57:51.713871 theheartbeat-0.1.1/heartbeat/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      393 2023-04-05 11:31:29.000000 theheartbeat-0.1.1/heartbeat/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2795 2023-04-11 11:56:28.000000 theheartbeat-0.1.1/heartbeat/heartbeat.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-04-11 11:57:51.717871 theheartbeat-0.1.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      626 2023-04-11 11:57:41.000000 theheartbeat-0.1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-11 11:57:51.717871 theheartbeat-0.1.1/theheartbeat.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      517 2023-04-11 11:57:51.000000 theheartbeat-0.1.1/theheartbeat.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      260 2023-04-11 11:57:51.000000 theheartbeat-0.1.1/theheartbeat.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-11 11:57:51.000000 theheartbeat-0.1.1/theheartbeat.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-04-11 11:57:51.000000 theheartbeat-0.1.1/theheartbeat.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-04-11 11:57:51.000000 theheartbeat-0.1.1/theheartbeat.egg-info/top_level.txt
```

### Comparing `theheartbeat-0.1.0/LICENSE` & `theheartbeat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `theheartbeat-0.1.0/README.md` & `theheartbeat-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `theheartbeat-0.1.0/heartbeat/heartbeat.py` & `theheartbeat-0.1.1/heartbeat/heartbeat.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,44 +3,51 @@
 import requests
 import os
 
 
 class HeartBeat:
     client_Token = None
     authorization_key = None
-
+    auth_token = None
     def client(self, access_key, access_token):
-        global client_Token, authorization_key
+        global client_Token, authorization_key, auth_token
+        url = 'https://zcq20sajf9.execute-api.ap-south-1.amazonaws.com/Prod/api/sdk-login'
         client_Token = access_key
         authorization_key = access_token
+        headers = {
+            'clientToken': client_Token,
+            'AuthorizationKey': authorization_key
+        }
+        response = requests.post(url, headers=headers).json()
+        auth_token = response['token']
         return HeartBeat()
 
     def upload_file(self, path=None):
-        url = 'https://ze3uixrwii.execute-api.ap-south-1.amazonaws.com/Prod/get-upload-url'
+        url = 'https://wdb8vf1vlf.execute-api.ap-south-1.amazonaws.com/Prod/api/get-upload-url'
         headers = {
-            'clientToken': client_Token,
-            'AuthorizationKey': authorization_key
+            'Authorization': auth_token,
+            'Content-Type': 'application/json'
         }
         filename = os.path.basename(path)
         body = {
             'fileName': filename
         }
         response = requests.post(url, headers=headers, data=json.dumps(body)).json()
         UUID = {'fileName':path, 'UUID': response.get('UUID')}
         if response.get('statusCode') != 200:
             return response
         with open(path, 'rb') as file:
             file_response = requests.put(response.get('presignedUrl'), data=file.read())
         return {'status': 200, 'message': 'Folder Successfully uploaded to S3', 'info': UUID}
 
     def upload_folder(self, path=None):
-        url = 'https://ze3uixrwii.execute-api.ap-south-1.amazonaws.com/Prod/get-upload-url'
+        url = 'https://wdb8vf1vlf.execute-api.ap-south-1.amazonaws.com/Prod/api/get-upload-url'
         headers = {
-            'clientToken': client_Token,
-            'AuthorizationKey': authorization_key
+            'Authorization': auth_token,
+            'Content-Type': 'application/json'
         }
         root_folder = os.path.dirname(path)
         arr = []
         for root, dirs, files in os.walk(path):
             for file in files:
                 file_path = os.path.join(root, file)
                 file_name = ''
```

### Comparing `theheartbeat-0.1.0/setup.py` & `theheartbeat-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='theheartbeat',
-    version='0.1.0',
-    description='A Python module for uploading files and folders to Amazon S3.',
+    version='0.1.1',
+    description='A Python module for uploading files and folders to Amazon S3 using preSigned URL.',
     author='Shubham Kumar',
     author_email='shubham@ioanyt.com',
     packages=['heartbeat'],
     install_requires=['requests'],
     classifiers=[
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5'
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9'
     ]
 )
```

