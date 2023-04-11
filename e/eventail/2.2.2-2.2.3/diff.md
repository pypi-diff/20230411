# Comparing `tmp/eventail-2.2.2.tar.gz` & `tmp/eventail-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventail-2.2.2.tar", last modified: Thu Mar 30 08:21:22 2023, max compression
+gzip compressed data, was "eventail-2.2.3.tar", last modified: Tue Apr 11 14:54:35 2023, max compression
```

## Comparing `eventail-2.2.2.tar` & `eventail-2.2.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-30 08:21:22.939557 eventail-2.2.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1079 2023-03-30 08:21:22.000000 eventail-2.2.2/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       65 2023-03-30 08:21:22.000000 eventail-2.2.2/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6853 2023-03-30 08:21:22.939557 eventail-2.2.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6154 2023-03-30 08:21:22.000000 eventail-2.2.2/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-30 08:21:22.939557 eventail-2.2.2/scripts/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4202 2023-03-30 08:21:22.000000 eventail-2.2.2/scripts/inspect_queue.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3742 2023-03-30 08:21:22.000000 eventail-2.2.2/scripts/logger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5376 2023-03-30 08:21:22.000000 eventail-2.2.2/scripts/monitor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2108 2023-03-30 08:21:22.000000 eventail-2.2.2/scripts/publish_configuration.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3098 2023-03-30 08:21:22.000000 eventail-2.2.2/scripts/publish_event.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5297 2023-03-30 08:21:22.000000 eventail-2.2.2/scripts/resurrect.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3447 2023-03-30 08:21:22.000000 eventail-2.2.2/scripts/send_command.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-03-30 08:21:22.939557 eventail-2.2.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1351 2023-03-30 08:21:22.000000 eventail-2.2.2/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-30 08:21:22.935557 eventail-2.2.2/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-30 08:21:22.939557 eventail-2.2.2/src/eventail/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1121 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-30 08:21:22.939557 eventail-2.2.2/src/eventail/async_service/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1121 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail/async_service/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-30 08:21:22.939557 eventail-2.2.2/src/eventail/async_service/aio/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1181 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail/async_service/aio/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23411 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail/async_service/aio/base.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-30 08:21:22.939557 eventail-2.2.2/src/eventail/async_service/pika/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1242 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail/async_service/pika/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    44832 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail/async_service/pika/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2811 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail/async_service/pika/supervisor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3576 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail/batch_processor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1534 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail/gelf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1380 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail/log_criticity.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail/py.typed
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7806 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail/sync_publisher.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7622 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail/tmp_store.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-30 08:21:22.939557 eventail-2.2.2/src/eventail.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6853 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      820 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       88 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-03-30 08:21:22.000000 eventail-2.2.2/src/eventail.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.953250 eventail-2.2.3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1079 2023-04-11 14:54:35.000000 eventail-2.2.3/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       65 2023-04-11 14:54:35.000000 eventail-2.2.3/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6853 2023-04-11 14:54:35.953250 eventail-2.2.3/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6154 2023-04-11 14:54:35.000000 eventail-2.2.3/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.953250 eventail-2.2.3/scripts/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4202 2023-04-11 14:54:35.000000 eventail-2.2.3/scripts/inspect_queue.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3742 2023-04-11 14:54:35.000000 eventail-2.2.3/scripts/logger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5376 2023-04-11 14:54:35.000000 eventail-2.2.3/scripts/monitor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2108 2023-04-11 14:54:35.000000 eventail-2.2.3/scripts/publish_configuration.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3098 2023-04-11 14:54:35.000000 eventail-2.2.3/scripts/publish_event.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5297 2023-04-11 14:54:35.000000 eventail-2.2.3/scripts/resurrect.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3447 2023-04-11 14:54:35.000000 eventail-2.2.3/scripts/send_command.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-11 14:54:35.953250 eventail-2.2.3/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1351 2023-04-11 14:54:35.000000 eventail-2.2.3/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.949250 eventail-2.2.3/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.953250 eventail-2.2.3/src/eventail/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1121 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.953250 eventail-2.2.3/src/eventail/async_service/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1121 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/async_service/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.953250 eventail-2.2.3/src/eventail/async_service/aio/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1181 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/async_service/aio/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23411 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/async_service/aio/base.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.953250 eventail-2.2.3/src/eventail/async_service/pika/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1242 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/async_service/pika/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    44831 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/async_service/pika/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2811 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/async_service/pika/supervisor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3576 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/batch_processor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1534 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/gelf.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1380 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/log_criticity.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/py.typed
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7806 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/sync_publisher.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7622 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/tmp_store.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.953250 eventail-2.2.3/src/eventail.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6853 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      820 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       88 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail.egg-info/top_level.txt
```

### Comparing `eventail-2.2.2/LICENSE` & `eventail-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/PKG-INFO` & `eventail-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventail
-Version: 2.2.2
+Version: 2.2.3
 Summary: A base class and utilities for AM service architecture
 Home-page: https://github.com/allo-media/eventail
 Author: Allo-Media
 Author-email: dev@allo-media.fr
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `eventail-2.2.2/README.md` & `eventail-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/scripts/inspect_queue.py` & `eventail-2.2.3/scripts/inspect_queue.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/scripts/logger.py` & `eventail-2.2.3/scripts/logger.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/scripts/monitor.py` & `eventail-2.2.3/scripts/monitor.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/scripts/publish_configuration.py` & `eventail-2.2.3/scripts/publish_configuration.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/scripts/publish_event.py` & `eventail-2.2.3/scripts/publish_event.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/scripts/resurrect.py` & `eventail-2.2.3/scripts/resurrect.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/scripts/send_command.py` & `eventail-2.2.3/scripts/send_command.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/setup.py` & `eventail-2.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="eventail",
-    version="2.2.2",
+    version="2.2.3",
     url="https://github.com/allo-media/eventail",
     author="Allo-Media",
     author_email="dev@allo-media.fr",
     description="A base class and utilities for AM service architecture",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `eventail-2.2.2/src/eventail/__init__.py` & `eventail-2.2.3/src/eventail/__init__.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/src/eventail/async_service/__init__.py` & `eventail-2.2.3/src/eventail/async_service/__init__.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/src/eventail/async_service/aio/__init__.py` & `eventail-2.2.3/src/eventail/async_service/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/src/eventail/async_service/aio/base.py` & `eventail-2.2.3/src/eventail/async_service/aio/base.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/src/eventail/async_service/pika/__init__.py` & `eventail-2.2.3/src/eventail/async_service/pika/__init__.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/src/eventail/async_service/pika/base.py` & `eventail-2.2.3/src/eventail/async_service/pika/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -608,21 +608,19 @@
 
         :param pika.channel.Channel ch: The channel object
         :param pika.Spec.Basic.Deliver: basic_deliver method
         :param pika.Spec.BasicProperties: properties
         :param bytes body: The message body
 
         """
-        headers: HEADER = properties.headers
+        headers: HEADER = properties.headers if properties.headers is not None else {}
         decoder = cbor if properties.content_type == "application/cbor" else json
         routing_key: str = basic_deliver.routing_key
         exchange: str = basic_deliver.exchange
-        if exchange != self.CONFIG_EXCHANGE and (
-            headers is None or "conversation_id" not in headers
-        ):
+        if exchange != self.CONFIG_EXCHANGE and "conversation_id" not in headers:
             self.log(EMERGENCY, f"Missing headers on {routing_key}")
             # unrecoverable error, send to dead letter
             ch.basic_nack(delivery_tag=basic_deliver.delivery_tag, requeue=False)
             return
         conversation_id = headers.pop("conversation_id", "")
 
         try:
```

### Comparing `eventail-2.2.2/src/eventail/async_service/pika/supervisor.py` & `eventail-2.2.3/src/eventail/async_service/pika/supervisor.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/src/eventail/batch_processor.py` & `eventail-2.2.3/src/eventail/batch_processor.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/src/eventail/gelf.py` & `eventail-2.2.3/src/eventail/gelf.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/src/eventail/log_criticity.py` & `eventail-2.2.3/src/eventail/log_criticity.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/src/eventail/sync_publisher.py` & `eventail-2.2.3/src/eventail/sync_publisher.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/src/eventail/tmp_store.py` & `eventail-2.2.3/src/eventail/tmp_store.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.2/src/eventail.egg-info/PKG-INFO` & `eventail-2.2.3/src/eventail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventail
-Version: 2.2.2
+Version: 2.2.3
 Summary: A base class and utilities for AM service architecture
 Home-page: https://github.com/allo-media/eventail
 Author: Allo-Media
 Author-email: dev@allo-media.fr
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `eventail-2.2.2/src/eventail.egg-info/SOURCES.txt` & `eventail-2.2.3/src/eventail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

