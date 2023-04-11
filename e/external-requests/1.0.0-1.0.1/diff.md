# Comparing `tmp/external_requests-1.0.0.tar.gz` & `tmp/external_requests-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "external_requests-1.0.0.tar", last modified: Tue Apr 11 14:13:30 2023, max compression
+gzip compressed data, was "external_requests-1.0.1.tar", last modified: Tue Apr 11 14:27:12 2023, max compression
```

## Comparing `external_requests-1.0.0.tar` & `external_requests-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 14:13:30.624520 external_requests-1.0.0/
--rw-rw-rw-   0        0        0      184 2023-04-11 14:13:30.624520 external_requests-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3225 2023-04-11 14:09:55.000000 external_requests-1.0.0/README.md
--rw-rw-rw-   0        0        0       86 2023-04-11 14:13:30.626520 external_requests-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      386 2023-04-11 14:10:23.000000 external_requests-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:13:30.544475 external_requests-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 14:13:30.595522 external_requests-1.0.0/src/external_requests/
--rw-rw-rw-   0        0        0        0 2023-04-11 10:28:27.000000 external_requests-1.0.0/src/external_requests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:13:30.612518 external_requests-1.0.0/src/external_requests/base_requests/
--rw-rw-rw-   0        0        0        0 2023-04-11 10:37:43.000000 external_requests-1.0.0/src/external_requests/base_requests/__init__.py
--rw-rw-rw-   0        0        0     1773 2023-04-11 11:01:40.000000 external_requests-1.0.0/src/external_requests/base_requests/external_request.py
--rw-rw-rw-   0        0        0      623 2023-04-11 11:01:40.000000 external_requests-1.0.0/src/external_requests/base_requests/external_request_with_body.py
--rw-rw-rw-   0        0        0       54 2023-04-11 10:51:07.000000 external_requests-1.0.0/src/external_requests/exceptions.py
--rw-rw-rw-   0        0        0      158 2023-04-11 10:48:26.000000 external_requests-1.0.0/src/external_requests/external_response.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:13:30.623520 external_requests-1.0.0/src/external_requests/method_requests/
--rw-rw-rw-   0        0        0        0 2023-04-11 11:02:21.000000 external_requests-1.0.0/src/external_requests/method_requests/__init__.py
--rw-rw-rw-   0        0        0      433 2023-04-11 11:08:43.000000 external_requests-1.0.0/src/external_requests/method_requests/delete_request.py
--rw-rw-rw-   0        0        0      424 2023-04-11 11:55:31.000000 external_requests-1.0.0/src/external_requests/method_requests/get_request.py
--rw-rw-rw-   0        0        0      310 2023-04-11 11:08:43.000000 external_requests-1.0.0/src/external_requests/method_requests/head_request.py
--rw-rw-rw-   0        0        0      316 2023-04-11 11:09:45.000000 external_requests-1.0.0/src/external_requests/method_requests/options_request.py
--rw-rw-rw-   0        0        0      454 2023-04-11 11:08:43.000000 external_requests-1.0.0/src/external_requests/method_requests/patch_request.py
--rw-rw-rw-   0        0        0      457 2023-04-11 11:07:14.000000 external_requests-1.0.0/src/external_requests/method_requests/post_request.py
--rw-rw-rw-   0        0        0      450 2023-04-11 11:10:11.000000 external_requests-1.0.0/src/external_requests/method_requests/put_request.py
--rw-rw-rw-   0        0        0      197 2023-04-11 10:41:11.000000 external_requests-1.0.0/src/external_requests/request_methods.py
--rw-rw-rw-   0        0        0      354 2023-04-11 11:33:25.000000 external_requests-1.0.0/src/external_requests/serialization_schema.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:13:30.608519 external_requests-1.0.0/src/external_requests.egg-info/
--rw-rw-rw-   0        0        0      184 2023-04-11 14:13:30.000000 external_requests-1.0.0/src/external_requests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1054 2023-04-11 14:13:30.000000 external_requests-1.0.0/src/external_requests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 14:13:30.000000 external_requests-1.0.0/src/external_requests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-11 14:13:30.000000 external_requests-1.0.0/src/external_requests.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-11 14:13:30.000000 external_requests-1.0.0/src/external_requests.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 14:27:12.955052 external_requests-1.0.1/
+-rw-rw-rw-   0        0        0     3549 2023-04-11 14:27:12.955052 external_requests-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3322 2023-04-11 14:24:01.000000 external_requests-1.0.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-11 14:27:12.957054 external_requests-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-04-11 14:27:05.000000 external_requests-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:27:12.873053 external_requests-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 14:27:12.924053 external_requests-1.0.1/src/external_requests/
+-rw-rw-rw-   0        0        0        0 2023-04-11 10:28:27.000000 external_requests-1.0.1/src/external_requests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:27:12.939052 external_requests-1.0.1/src/external_requests/base_requests/
+-rw-rw-rw-   0        0        0        0 2023-04-11 10:37:43.000000 external_requests-1.0.1/src/external_requests/base_requests/__init__.py
+-rw-rw-rw-   0        0        0     1773 2023-04-11 11:01:40.000000 external_requests-1.0.1/src/external_requests/base_requests/external_request.py
+-rw-rw-rw-   0        0        0      623 2023-04-11 11:01:40.000000 external_requests-1.0.1/src/external_requests/base_requests/external_request_with_body.py
+-rw-rw-rw-   0        0        0       54 2023-04-11 10:51:07.000000 external_requests-1.0.1/src/external_requests/exceptions.py
+-rw-rw-rw-   0        0        0      158 2023-04-11 10:48:26.000000 external_requests-1.0.1/src/external_requests/external_response.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:27:12.954052 external_requests-1.0.1/src/external_requests/method_requests/
+-rw-rw-rw-   0        0        0        0 2023-04-11 11:02:21.000000 external_requests-1.0.1/src/external_requests/method_requests/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-04-11 11:08:43.000000 external_requests-1.0.1/src/external_requests/method_requests/delete_request.py
+-rw-rw-rw-   0        0        0      424 2023-04-11 11:55:31.000000 external_requests-1.0.1/src/external_requests/method_requests/get_request.py
+-rw-rw-rw-   0        0        0      310 2023-04-11 11:08:43.000000 external_requests-1.0.1/src/external_requests/method_requests/head_request.py
+-rw-rw-rw-   0        0        0      316 2023-04-11 11:09:45.000000 external_requests-1.0.1/src/external_requests/method_requests/options_request.py
+-rw-rw-rw-   0        0        0      454 2023-04-11 11:08:43.000000 external_requests-1.0.1/src/external_requests/method_requests/patch_request.py
+-rw-rw-rw-   0        0        0      457 2023-04-11 11:07:14.000000 external_requests-1.0.1/src/external_requests/method_requests/post_request.py
+-rw-rw-rw-   0        0        0      450 2023-04-11 11:10:11.000000 external_requests-1.0.1/src/external_requests/method_requests/put_request.py
+-rw-rw-rw-   0        0        0      197 2023-04-11 10:41:11.000000 external_requests-1.0.1/src/external_requests/request_methods.py
+-rw-rw-rw-   0        0        0      354 2023-04-11 11:33:25.000000 external_requests-1.0.1/src/external_requests/serialization_schema.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:27:12.936053 external_requests-1.0.1/src/external_requests.egg-info/
+-rw-rw-rw-   0        0        0     3549 2023-04-11 14:27:12.000000 external_requests-1.0.1/src/external_requests.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2023-04-11 14:27:12.000000 external_requests-1.0.1/src/external_requests.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 14:27:12.000000 external_requests-1.0.1/src/external_requests.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-11 14:27:12.000000 external_requests-1.0.1/src/external_requests.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-11 14:27:12.000000 external_requests-1.0.1/src/external_requests.egg-info/top_level.txt
```

### Comparing `external_requests-1.0.0/README.md` & `external_requests-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,24 @@
+Metadata-Version: 2.1
+Name: external_requests
+Version: 1.0.1
+Home-page: https://gitlab.com/VenfiOranai/external-requests
+Author: Venfi Oranai
+Author-email: venfioranai@gmail.com
+Description-Content-Type: text/markdown
+
 # External Requests
 A class based alternative to making HTTP requests in Python.
 
+### Installation
+Installation can be done with pip:
+```
+pip install external-requests
+```
+
 ### Basic Usage
 In order to use external requests, you must implement one of the abstract classes provided by the package, create an 
 instance of your new class, and call the request function.
 
 ```python
 from typing import List
 from external_requests.base_requests.external_request import ExternalRequest
```

### Comparing `external_requests-1.0.0/src/external_requests/base_requests/external_request.py` & `external_requests-1.0.1/src/external_requests/base_requests/external_request.py`

 * *Files identical despite different names*

### Comparing `external_requests-1.0.0/src/external_requests/base_requests/external_request_with_body.py` & `external_requests-1.0.1/src/external_requests/base_requests/external_request_with_body.py`

 * *Files identical despite different names*

### Comparing `external_requests-1.0.0/src/external_requests.egg-info/SOURCES.txt` & `external_requests-1.0.1/src/external_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

