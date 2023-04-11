# Comparing `tmp/dequeai-0.698.tar.gz` & `tmp/dequeai-0.700.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.698.tar", last modified: Tue Apr 11 16:25:45 2023, max compression
+gzip compressed data, was "dequeai-0.700.tar", last modified: Tue Apr 11 16:27:39 2023, max compression
```

## Comparing `dequeai-0.698.tar` & `dequeai-0.700.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:25:45.537189 dequeai-0.698/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 16:25:45.537189 dequeai-0.698/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:25:45.537189 dequeai-0.698/dequeai/
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.698/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.698/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.698/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.698/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.698/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    20490 2023-04-11 16:19:53.000000 dequeai-0.698/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.698/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.698/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.698/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.698/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:25:45.537189 dequeai-0.698/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 16:25:45.000000 dequeai-0.698/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-11 16:25:45.000000 dequeai-0.698/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 16:25:45.000000 dequeai-0.698/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-11 16:25:45.000000 dequeai-0.698/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 16:25:45.000000 dequeai-0.698/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 16:25:45.537189 dequeai-0.698/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      470 2023-04-11 16:25:32.000000 dequeai-0.698/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:39.093743 dequeai-0.700/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 16:27:39.093743 dequeai-0.700/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:39.093743 dequeai-0.700/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.700/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.700/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.700/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.700/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.700/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    20492 2023-04-11 16:27:02.000000 dequeai-0.700/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.700/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.700/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.700/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.700/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:39.093743 dequeai-0.700/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 16:27:38.000000 dequeai-0.700/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-11 16:27:39.000000 dequeai-0.700/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 16:27:38.000000 dequeai-0.700/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-11 16:27:38.000000 dequeai-0.700/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 16:27:39.000000 dequeai-0.700/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 16:27:39.093743 dequeai-0.700/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      470 2023-04-11 16:27:24.000000 dequeai-0.700/setup.py
```

### Comparing `dequeai-0.698/dequeai/datatypes.py` & `dequeai-0.700/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.698/dequeai/dequeai.py` & `dequeai-0.700/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.698/dequeai/dequeai_run.py` & `dequeai-0.700/dequeai/dequeai_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from dequeai.rest_connect import RestConnect
 from dequeai.deque_environment import AGENT_API_SERVICE_URL
 #from deque.redis_services import RedisServices
 import pickle
 import multiprocessing
 from dequeai.parsing_service import ParsingService
-from dequeai.datatypes import Image, Audio, Histogram, BoundingBox2D, Table, Plot
+from dequeai.datatypes import Image, Audio, Histogram, BoundingBox2D, Table #, Plot
 from dequeai.util import MODEL, CODE, DATA, ENVIRONMENT, RESOURCES,TRACKING_ENDPOINT
 import requests
 import glob
 import time
 import psutil
 import GPUtil
 import socket
```

### Comparing `dequeai-0.698/dequeai/parsing_service.py` & `dequeai-0.700/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.698/dequeai/rest_connect.py` & `dequeai-0.700/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.698/dequeai/util.py` & `dequeai-0.700/dequeai/util.py`

 * *Files identical despite different names*

