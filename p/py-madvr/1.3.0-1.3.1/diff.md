# Comparing `tmp/py_madvr-1.3.0.tar.gz` & `tmp/py_madvr-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.3.0.tar", last modified: Tue Apr 11 02:02:41 2023, max compression
+gzip compressed data, was "py_madvr-1.3.1.tar", last modified: Tue Apr 11 02:28:50 2023, max compression
```

## Comparing `py_madvr-1.3.0.tar` & `py_madvr-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:02:41.058193 py_madvr-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 02:02:31.000000 py_madvr-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-11 02:02:41.058193 py_madvr-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-11 02:02:31.000000 py_madvr-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:02:41.058193 py_madvr-1.3.0/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-11 02:02:31.000000 py_madvr-1.3.0/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-11 02:02:31.000000 py_madvr-1.3.0/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-11 02:02:31.000000 py_madvr-1.3.0/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-04-11 02:02:31.000000 py_madvr-1.3.0/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:02:41.058193 py_madvr-1.3.0/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-11 02:02:41.000000 py_madvr-1.3.0/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-11 02:02:41.000000 py_madvr-1.3.0/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:02:41.000000 py_madvr-1.3.0/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 02:02:41.000000 py_madvr-1.3.0/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 02:02:41.058193 py_madvr-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-11 02:02:31.000000 py_madvr-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:02:41.058193 py_madvr-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 02:02:31.000000 py_madvr-1.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-11 02:02:31.000000 py_madvr-1.3.0/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:28:50.106267 py_madvr-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 02:28:39.000000 py_madvr-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-11 02:28:50.106267 py_madvr-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-11 02:28:39.000000 py_madvr-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:28:50.106267 py_madvr-1.3.1/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-11 02:28:39.000000 py_madvr-1.3.1/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-11 02:28:39.000000 py_madvr-1.3.1/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-11 02:28:39.000000 py_madvr-1.3.1/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21915 2023-04-11 02:28:39.000000 py_madvr-1.3.1/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:28:50.106267 py_madvr-1.3.1/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-11 02:28:50.000000 py_madvr-1.3.1/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-11 02:28:50.000000 py_madvr-1.3.1/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:28:50.000000 py_madvr-1.3.1/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 02:28:50.000000 py_madvr-1.3.1/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 02:28:50.106267 py_madvr-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-11 02:28:39.000000 py_madvr-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:28:50.106267 py_madvr-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 02:28:39.000000 py_madvr-1.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-11 02:28:39.000000 py_madvr-1.3.1/tests/testMadVR.py
```

### Comparing `py_madvr-1.3.0/LICENSE` & `py_madvr-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.0/PKG-INFO` & `py_madvr-1.3.1/py_madvr.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py_madvr
-Version: 1.3.0
+Name: py-madvr
+Version: 1.3.1
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.3.0/madvr/commands.py` & `py_madvr-1.3.1/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.0/madvr/madvr.py` & `py_madvr-1.3.1/madvr/madvr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Implements the MadVR protocol
 """
 
 import logging
 from typing import Final, Union
 import re
-import time
 import asyncio
 from madvr.commands import ACKs, Footer, Commands, Enum, Connections
 from madvr.errors import AckError, RetryExceededError, HeartBeatError
 
 
 class Madvr:
     """MadVR Control"""
@@ -418,27 +417,35 @@
         return ""
 
     async def start_read_notifications(self, wait_forever: bool) -> None:
         """
         Listen for notifications. Meant to run as a background task
         wait_forever: bool -> if true, it will block forever. False useful for testing
         """
-        # reconnect if client is not init or its off
-        if self.notification_reader is None or self.is_on is False:
-            await self._reconnect()
 
         # Receive data in a loop
         i = 0
         while wait_forever or i < 5:
+            # TODO: stop loop if remote is off, start when remote is on
+            if self.is_on is False:
+                self.logger.debug("envy is off")
+                asyncio.sleep(5)
+                continue
+
+            if self.notification_reader is None:
+                self.logger.debug("notifications waiting for connection to open")
+                asyncio.sleep(2)
+                continue
+
             try:
                 # send hearbeat
                 async with self.notification_writer_lock:
                     self.notification_writer.write(self.HEARTBEAT)
                     await self.notification_writer.drain()
-                
+
                 async with self.notification_reader_lock:
                     data = await asyncio.wait_for(
                         self.reader.readline(),
                         timeout=self.command_read_timeout,
                     )
 
                 asyncio.sleep(1)
```

### Comparing `py_madvr-1.3.0/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py-madvr
-Version: 1.3.0
+Name: py_madvr
+Version: 1.3.1
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.3.0/setup.py` & `py_madvr-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.3.0",
+    version="1.3.1",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.3.0/tests/testMadVR.py` & `py_madvr-1.3.1/tests/testMadVR.py`

 * *Files identical despite different names*

