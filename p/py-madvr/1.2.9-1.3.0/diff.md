# Comparing `tmp/py_madvr-1.2.9.tar.gz` & `tmp/py_madvr-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.2.9.tar", last modified: Tue Apr 11 01:45:18 2023, max compression
+gzip compressed data, was "py_madvr-1.3.0.tar", last modified: Tue Apr 11 02:02:41 2023, max compression
```

## Comparing `py_madvr-1.2.9.tar` & `py_madvr-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:45:18.185502 py_madvr-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 01:45:07.000000 py_madvr-1.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-11 01:45:18.185502 py_madvr-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-11 01:45:07.000000 py_madvr-1.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:45:18.185502 py_madvr-1.2.9/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-11 01:45:07.000000 py_madvr-1.2.9/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-11 01:45:07.000000 py_madvr-1.2.9/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-11 01:45:07.000000 py_madvr-1.2.9/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20776 2023-04-11 01:45:07.000000 py_madvr-1.2.9/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:45:18.185502 py_madvr-1.2.9/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-11 01:45:18.000000 py_madvr-1.2.9/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-11 01:45:18.000000 py_madvr-1.2.9/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:45:18.000000 py_madvr-1.2.9/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 01:45:18.000000 py_madvr-1.2.9/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:45:18.185502 py_madvr-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-11 01:45:07.000000 py_madvr-1.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:45:18.185502 py_madvr-1.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:45:07.000000 py_madvr-1.2.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-11 01:45:07.000000 py_madvr-1.2.9/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:02:41.058193 py_madvr-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 02:02:31.000000 py_madvr-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-11 02:02:41.058193 py_madvr-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-11 02:02:31.000000 py_madvr-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:02:41.058193 py_madvr-1.3.0/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-11 02:02:31.000000 py_madvr-1.3.0/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-11 02:02:31.000000 py_madvr-1.3.0/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-11 02:02:31.000000 py_madvr-1.3.0/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-04-11 02:02:31.000000 py_madvr-1.3.0/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:02:41.058193 py_madvr-1.3.0/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-11 02:02:41.000000 py_madvr-1.3.0/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-11 02:02:41.000000 py_madvr-1.3.0/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:02:41.000000 py_madvr-1.3.0/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 02:02:41.000000 py_madvr-1.3.0/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 02:02:41.058193 py_madvr-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-11 02:02:31.000000 py_madvr-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:02:41.058193 py_madvr-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 02:02:31.000000 py_madvr-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-11 02:02:31.000000 py_madvr-1.3.0/tests/testMadVR.py
```

### Comparing `py_madvr-1.2.9/LICENSE` & `py_madvr-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.2.9/PKG-INFO` & `py_madvr-1.3.0/py_madvr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py_madvr
-Version: 1.2.9
+Name: py-madvr
+Version: 1.3.0
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.2.9/madvr/commands.py` & `py_madvr-1.3.0/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.2.9/madvr/madvr.py` & `py_madvr-1.3.0/madvr/madvr.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,17 +57,21 @@
         self.outgoing_colorimetry = ""
         self.outgoing_hdr_flag = False
         self.outgoing_black_levels = ""
 
         # Sockets
         self.reader = None
         self.writer = None
+        self.reader_lock = asyncio.Lock()
+        self.writer_lock = asyncio.Lock()
 
         self.notification_reader = None
         self.notification_writer = None
+        self.notification_reader_lock = asyncio.Lock()
+        self.notification_writer_lock = asyncio.Lock()
         self.is_closed = False
         # Envy does not have an are you on cmd, just assuming its on based on active connection
         self.is_on = False
         self.read_limit = 8000
         self.command_read_timeout = 3
         self.logger.debug("Running in debug mode")
 
@@ -99,40 +103,40 @@
         self.outgoing_bit_depth = ""
         self.outgoing_colorimetry = ""
         self.outgoing_hdr_flag = False
         self.outgoing_black_levels = ""
 
     async def close_connection(self) -> None:
         """close the connection"""
-        try:
-            self.writer.close()
-            await self.writer.wait_closed()
-        except AttributeError:
-            # means its already closed
-            pass
-
-        try:
-            self.notification_writer.close()
-            await self.notification_writer.wait_closed()
-        except AttributeError:
-            # means its already closed
-            pass
+        async with self.writer_lock:
+            try:
+                self.writer.close()
+                await self.writer.wait_closed()
+            except AttributeError:
+                # means its already closed
+                pass
+        async with self.notification_writer_lock:
+            try:
+                self.notification_writer.close()
+                await self.notification_writer.wait_closed()
+            except AttributeError:
+                # means its already closed
+                pass
 
         self.reader = None
         self.notification_reader = None
 
         self.is_closed = True
 
         # Clear attr
         await self._clear_attr()
 
     async def open_connection(self) -> None:
         """Open a connection"""
         self.logger.debug("Starting open connection")
-
         try:
             await self._reconnect()
         except AckError as err:
             self.logger.error(err)
 
     async def _reconnect(self) -> None:
         """
@@ -142,47 +146,50 @@
         """
 
         while True:
             try:
                 self.logger.info("Connecting to Envy: %s:%s", self.host, self.port)
 
                 # Command client
-                self.reader, self.writer = await asyncio.wait_for(
-                    asyncio.open_connection(self.host, self.port),
-                    timeout=self.command_read_timeout,
-                )
+                async with self.reader_lock, self.notification_reader_lock:
+                    self.reader, self.writer = await asyncio.wait_for(
+                        asyncio.open_connection(self.host, self.port),
+                        timeout=self.command_read_timeout,
+                    )
 
-                # Notifications client
-                (
-                    self.notification_reader,
-                    self.notification_writer,
-                ) = await asyncio.wait_for(
-                    asyncio.open_connection(self.host, self.port), timeout=20
-                )
+                    # Notifications client
+                    (
+                        self.notification_reader,
+                        self.notification_writer,
+                    ) = await asyncio.wait_for(
+                        asyncio.open_connection(self.host, self.port), timeout=20
+                    )
 
                 # Test heartbeat
                 self.logger.debug("Handshaking")
 
                 # Make sure first message says WELCOME
-                msg_envy = await asyncio.wait_for(
-                    self.reader.readline(),
-                    timeout=10,
-                )
+                async with self.reader_lock:
+                    msg_envy = await asyncio.wait_for(
+                        self.reader.readline(),
+                        timeout=10,
+                    )
 
                 # Check if first 7 char match
                 if self.MADVR_OK != msg_envy[:7]:
                     # This is fatal, and should not retry. If it doesn't respond as expected something is wrong
                     raise AckError(
                         f"Notification did not reply with correct greeting: {msg_envy}"
                     )
 
                 # Make sure first message says WELCOME for notifications
-                msg_envy = await asyncio.wait_for(
-                    self.notification_reader.readline(), timeout=20
-                )
+                async with self.notification_reader_lock:
+                    msg_envy = await asyncio.wait_for(
+                        self.notification_reader.readline(), timeout=20
+                    )
 
                 # Check if first 7 char match
                 if self.MADVR_OK != msg_envy[:7]:
                     raise AckError(
                         f"Notification did not reply with correct greeting: {msg_envy}"
                     )
                 self.logger.info("Waiting for envy to be available")
@@ -231,39 +238,33 @@
         """
         i = 0
 
         while i < 3:
             # confirm can send heartbeat, ready for commands
             self.logger.debug("Sending heartbeats")
 
-            self.writer.write(self.HEARTBEAT)
-            await self.writer.drain()
+            async with self.writer_lock:
+                self.writer.write(self.HEARTBEAT)
+                await self.writer.drain()
 
             # Recv until we find ok or timeout
             if not await self._read_until_ok(self.reader):
                 i += 1
                 continue
 
             # send heartbeat with notification and read ack and then regular client
             # ensure both work one after the next
-            self.notification_writer.write(self.HEARTBEAT)
-            await self.notification_writer.drain()
+            async with self.notification_writer_lock:
+                self.notification_writer.write(self.HEARTBEAT)
+                await self.notification_writer.drain()
 
             if not await self._read_until_ok(self.notification_reader):
                 i += 1
                 continue
 
-            # send again on regular client to make sure both clients work
-            self.writer.write(self.HEARTBEAT)
-            await self.writer.drain()
-
-            if not await self._read_until_ok(self.reader):
-                i += 1
-                continue
-
             self.logger.debug("Handshakes complete")
 
             return
 
         raise HeartBeatError("Sending heartbeat fatal error")
 
     async def _construct_command(
@@ -342,16 +343,17 @@
         """
         Read the buffer until we get ok or timeout because a timeout means no more to read
         """
         counter = 0
         # exit loop if exceed maximum checks for ok or retries
         while True:
             try:
-                data = await asyncio.wait_for(client.readline(), timeout=10)
-                self.logger.debug("_read_until_ok: data found: %s", data)
+                async with self.reader_lock, self.notification_reader_lock:
+                    data = await asyncio.wait_for(client.readline(), timeout=10)
+                    self.logger.debug("_read_until_ok: data found: %s", data)
 
                 if ACKs.reply.value not in data:
                     self.logger.debug("OK not found yet counter: %s", counter)
                     counter += 1
                     continue
 
                 self.logger.debug("OK found counter: %s", counter)
@@ -388,16 +390,17 @@
 
         # simple retry logic
         retry_count = 0
 
         while retry_count < 5:
             # Send the command
             try:
-                self.writer.write(cmd)
-                await self.writer.drain()
+                async with self.writer_lock:
+                    self.writer.write(cmd)
+                    await self.writer.drain()
 
             except asyncio.TimeoutError:
                 self.logger.debug("OK receipt timed out, retrying")
                 retry_count += 1
                 continue
 
             # should catch connection is closed
@@ -424,43 +427,49 @@
             await self._reconnect()
 
         # Receive data in a loop
         i = 0
         while wait_forever or i < 5:
             try:
                 # send hearbeat
-                self.notification_writer.write(self.HEARTBEAT)
-                await self.notification_writer.drain()
-                data = await asyncio.wait_for(
-                    self.reader.readline(),
-                    timeout=self.command_read_timeout,
-                )
+                async with self.notification_writer_lock:
+                    self.notification_writer.write(self.HEARTBEAT)
+                    await self.notification_writer.drain()
+                
+                async with self.notification_reader_lock:
+                    data = await asyncio.wait_for(
+                        self.reader.readline(),
+                        timeout=self.command_read_timeout,
+                    )
 
                 asyncio.sleep(1)
 
                 i += 1
 
                 if data:
                     # process data which will get added as class attr
                     await self._process_notifications(data)
                 else:
                     # just wait forever for data
                     # send heartbeat keep conn open
-                    self.notification_writer.write(self.HEARTBEAT)
-                    await self.notification_writer.drain()
+                    async with self.notification_writer_lock:
+                        self.notification_writer.write(self.HEARTBEAT)
+                        await self.notification_writer.drain()
                     continue
             except asyncio.TimeoutError:
                 self.logger.debug("Connection timed out")
-                self.notification_writer.write(self.HEARTBEAT)
-                await self.notification_writer.drain()
+                async with self.notification_writer_lock:
+                    self.notification_writer.write(self.HEARTBEAT)
+                    await self.notification_writer.drain()
                 continue
             except OSError:
                 self.logger.debug("Connection error")
-                self.notification_writer.write(self.HEARTBEAT)
-                await self.notification_writer.drain()
+                async with self.notification_writer_lock:
+                    self.notification_writer.write(self.HEARTBEAT)
+                    await self.notification_writer.drain()
                 continue
             except AttributeError:
                 await self._reconnect()
 
     async def _process_notifications(self, input_data: Union[bytes, str]) -> None:
         """
         Process arbitrary stream of notifications and set them as instance attr
```

### Comparing `py_madvr-1.2.9/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py-madvr
-Version: 1.2.9
+Name: py_madvr
+Version: 1.3.0
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.2.9/setup.py` & `py_madvr-1.3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.2.9",
+    version="1.3.0",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.2.9/tests/testMadVR.py` & `py_madvr-1.3.0/tests/testMadVR.py`

 * *Files identical despite different names*

