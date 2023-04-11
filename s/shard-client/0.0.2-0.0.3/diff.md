# Comparing `tmp/shard_client-0.0.2.tar.gz` & `tmp/shard_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shard_client-0.0.2.tar", last modified: Mon Apr 10 23:26:58 2023, max compression
+gzip compressed data, was "shard_client-0.0.3.tar", last modified: Tue Apr 11 00:49:35 2023, max compression
```

## Comparing `shard_client-0.0.2.tar` & `shard_client-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-10 23:26:58.500715 shard_client-0.0.2/
--rw-r--r--   0 anon      (1000) anon      (1000)      375 2023-04-10 23:26:58.500715 shard_client-0.0.2/PKG-INFO
--rw-r--r--   0 anon      (1000) anon      (1000)      385 2023-04-10 23:26:37.000000 shard_client-0.0.2/pyproject.toml
--rw-r--r--   0 anon      (1000) anon      (1000)       38 2023-04-10 23:26:58.500715 shard_client-0.0.2/setup.cfg
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-10 23:26:58.500715 shard_client-0.0.2/src/
--rw-r--r--   0 anon      (1000) anon      (1000)        0 2023-04-10 21:12:34.000000 shard_client-0.0.2/src/__init__.py
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-10 23:26:58.500715 shard_client-0.0.2/src/lib/
--rw-r--r--   0 anon      (1000) anon      (1000)     1590 2023-04-04 22:34:06.000000 shard_client-0.0.2/src/lib/color_printer.py
--rw-r--r--   0 anon      (1000) anon      (1000)      766 2023-04-01 20:15:34.000000 shard_client-0.0.2/src/lib/logclass.py
--rw-r--r--   0 anon      (1000) anon      (1000)     3432 2023-04-05 01:55:08.000000 shard_client-0.0.2/src/lib/mqlib.py
--rw-r--r--   0 anon      (1000) anon      (1000)      304 2023-03-31 23:23:46.000000 shard_client-0.0.2/src/lib/mqtt_queue.py
--rw-r--r--   0 anon      (1000) anon      (1000)       59 2023-04-01 19:54:16.000000 shard_client-0.0.2/src/lib/status.py
--rwxr-xr-x   0 anon      (1000) anon      (1000)     7291 2023-04-10 21:11:13.000000 shard_client-0.0.2/src/scanner.py
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-10 23:26:58.500715 shard_client-0.0.2/src/shard_client.egg-info/
--rw-r--r--   0 anon      (1000) anon      (1000)      375 2023-04-10 23:26:58.000000 shard_client-0.0.2/src/shard_client.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) anon      (1000)      307 2023-04-10 23:26:58.000000 shard_client-0.0.2/src/shard_client.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) anon      (1000)        1 2023-04-10 23:26:58.000000 shard_client-0.0.2/src/shard_client.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) anon      (1000)       26 2023-04-10 23:26:58.000000 shard_client-0.0.2/src/shard_client.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-11 00:49:35.192878 shard_client-0.0.3/
+-rw-r--r--   0 anon      (1000) anon      (1000)      375 2023-04-11 00:49:35.192878 shard_client-0.0.3/PKG-INFO
+-rw-r--r--   0 anon      (1000) anon      (1000)      460 2023-04-11 00:48:32.000000 shard_client-0.0.3/pyproject.toml
+-rw-r--r--   0 anon      (1000) anon      (1000)       38 2023-04-11 00:49:35.192878 shard_client-0.0.3/setup.cfg
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-11 00:49:35.192878 shard_client-0.0.3/src/
+-rw-r--r--   0 anon      (1000) anon      (1000)        0 2023-04-10 21:12:34.000000 shard_client-0.0.3/src/__init__.py
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-11 00:49:35.192878 shard_client-0.0.3/src/lib/
+-rw-r--r--   0 anon      (1000) anon      (1000)     1590 2023-04-04 22:34:06.000000 shard_client-0.0.3/src/lib/color_printer.py
+-rw-r--r--   0 anon      (1000) anon      (1000)      766 2023-04-01 20:15:34.000000 shard_client-0.0.3/src/lib/logclass.py
+-rw-r--r--   0 anon      (1000) anon      (1000)     3432 2023-04-05 01:55:08.000000 shard_client-0.0.3/src/lib/mqlib.py
+-rw-r--r--   0 anon      (1000) anon      (1000)      304 2023-03-31 23:23:46.000000 shard_client-0.0.3/src/lib/mqtt_queue.py
+-rw-r--r--   0 anon      (1000) anon      (1000)       59 2023-04-01 19:54:16.000000 shard_client-0.0.3/src/lib/status.py
+-rwxr-xr-x   0 anon      (1000) anon      (1000)     7311 2023-04-11 00:49:22.000000 shard_client-0.0.3/src/scanner.py
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-11 00:49:35.192878 shard_client-0.0.3/src/shard_client.egg-info/
+-rw-r--r--   0 anon      (1000) anon      (1000)      375 2023-04-11 00:49:35.000000 shard_client-0.0.3/src/shard_client.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) anon      (1000)      346 2023-04-11 00:49:35.000000 shard_client-0.0.3/src/shard_client.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)        1 2023-04-11 00:49:35.000000 shard_client-0.0.3/src/shard_client.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)       44 2023-04-11 00:49:35.000000 shard_client-0.0.3/src/shard_client.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)       26 2023-04-11 00:49:35.000000 shard_client-0.0.3/src/shard_client.egg-info/top_level.txt
```

### Comparing `shard_client-0.0.2/src/lib/color_printer.py` & `shard_client-0.0.3/src/lib/color_printer.py`

 * *Files identical despite different names*

### Comparing `shard_client-0.0.2/src/lib/logclass.py` & `shard_client-0.0.3/src/lib/logclass.py`

 * *Files identical despite different names*

### Comparing `shard_client-0.0.2/src/lib/mqlib.py` & `shard_client-0.0.3/src/lib/mqlib.py`

 * *Files identical despite different names*

### Comparing `shard_client-0.0.2/src/scanner.py` & `shard_client-0.0.3/src/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 import random
 import string
 import time
 
 import aiofiles
 import dotenv
 
-import scanner_node.lib.mqlib
-import scanner_node.lib.status
-from scanner_node.lib.logclass import CustomLogger
+import scanner_node.src.lib.mqlib
+import scanner_node.src.lib.status
+from scanner_node.src.lib.logclass import CustomLogger
 
 
 class Scanner:
     def __init__(self, mq_broker_address: str, loop: asyncio.AbstractEventLoop):
         host, port = self.parse_address_port(mq_broker_address)
         self.loop = loop
         self.client_id = self.generate_slug()
         self.subscriptions = [f'/client/{self.client_id}/+']
-        self.mq = scanner_node.lib.mqlib.MqttClient(host, port, self.subscriptions, self.client_id, 0)
+        self.mq = scanner_node.src.lib.mqlib.MqttClient(host, port, self.subscriptions, self.client_id, 0)
         self.outgoing_queue = self.mq.outgoing_queue
         self.incoming_queue = self.mq.incoming_queue
-        self.status_messages = scanner_node.lib.status.Status
+        self.status_messages = scanner_node.src.lib.status.Status
         self.system_status = self.status_messages.AVAILABLE
         logger = CustomLogger()
         logger.setup_file_handler('coordinator')
         self.tasks = set()
         self.logger = logger.logger
         self.running = True
```

