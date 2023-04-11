# Comparing `tmp/idun_guardian_client-1.1b2.tar.gz` & `tmp/idun_guardian_client-1.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idun_guardian_client-1.1b2.tar", last modified: Fri Apr  7 15:59:20 2023, max compression
+gzip compressed data, was "idun_guardian_client-1.1b3.tar", last modified: Tue Apr 11 06:45:14 2023, max compression
```

## Comparing `idun_guardian_client-1.1b2.tar` & `idun_guardian_client-1.1b3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-07 15:59:20.694010 idun_guardian_client-1.1b2/
--rw-r--r--   0 waddaben   (501) staff       (20)     8728 2023-04-07 15:59:20.693788 idun_guardian_client-1.1b2/PKG-INFO
--rw-r--r--   0 waddaben   (501) staff       (20)     8163 2023-04-07 09:22:23.000000 idun_guardian_client-1.1b2/README.md
--rw-r--r--   0 waddaben   (501) staff       (20)      869 2023-04-07 15:57:28.000000 idun_guardian_client-1.1b2/pyproject.toml
--rw-r--r--   0 waddaben   (501) staff       (20)       38 2023-04-07 15:59:20.694062 idun_guardian_client-1.1b2/setup.cfg
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-07 15:59:20.687763 idun_guardian_client-1.1b2/src/
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-07 15:59:20.692133 idun_guardian_client-1.1b2/src/idun_guardian_client/
--rw-r--r--   0 waddaben   (501) staff       (20)      339 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b2/src/idun_guardian_client/__init__.py
--rw-r--r--   0 waddaben   (501) staff       (20)        0 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b2/src/idun_guardian_client/__main__.py
--rw-r--r--   0 waddaben   (501) staff       (20)     7083 2023-04-07 11:46:40.000000 idun_guardian_client-1.1b2/src/idun_guardian_client/client.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1797 2023-04-07 12:29:46.000000 idun_guardian_client-1.1b2/src/idun_guardian_client/config.py
--rw-r--r--   0 waddaben   (501) staff       (20)    11623 2023-04-07 15:53:12.000000 idun_guardian_client-1.1b2/src/idun_guardian_client/debug_logs.py
--rw-r--r--   0 waddaben   (501) staff       (20)    20707 2023-04-07 15:53:12.000000 idun_guardian_client-1.1b2/src/idun_guardian_client/igeb_api.py
--rw-r--r--   0 waddaben   (501) staff       (20)    30620 2023-04-07 15:53:12.000000 idun_guardian_client-1.1b2/src/idun_guardian_client/igeb_bluetooth.py
--rw-r--r--   0 waddaben   (501) staff       (20)     2846 2023-04-07 11:46:38.000000 idun_guardian_client-1.1b2/src/idun_guardian_client/igeb_utils.py
--rw-r--r--   0 waddaben   (501) staff       (20)      191 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b2/src/idun_guardian_client/mock_utils.py
--rw-r--r--   0 waddaben   (501) staff       (20)      164 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b2/src/idun_guardian_client/setup.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1214 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b2/src/idun_guardian_client/test_producer_consumer.py
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-07 15:59:20.693021 idun_guardian_client-1.1b2/src/idun_guardian_client.egg-info/
--rw-r--r--   0 waddaben   (501) staff       (20)     8728 2023-04-07 15:59:20.000000 idun_guardian_client-1.1b2/src/idun_guardian_client.egg-info/PKG-INFO
--rw-r--r--   0 waddaben   (501) staff       (20)      752 2023-04-07 15:59:20.000000 idun_guardian_client-1.1b2/src/idun_guardian_client.egg-info/SOURCES.txt
--rw-r--r--   0 waddaben   (501) staff       (20)        1 2023-04-07 15:59:20.000000 idun_guardian_client-1.1b2/src/idun_guardian_client.egg-info/dependency_links.txt
--rw-r--r--   0 waddaben   (501) staff       (20)      137 2023-04-07 15:59:20.000000 idun_guardian_client-1.1b2/src/idun_guardian_client.egg-info/requires.txt
--rw-r--r--   0 waddaben   (501) staff       (20)       21 2023-04-07 15:59:20.000000 idun_guardian_client-1.1b2/src/idun_guardian_client.egg-info/top_level.txt
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-07 15:59:20.693538 idun_guardian_client-1.1b2/tests/
--rw-r--r--   0 waddaben   (501) staff       (20)     1940 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b2/tests/test_ble.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1672 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b2/tests/test_ble_record.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1106 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b2/tests/test_utils.py
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 06:45:14.760188 idun_guardian_client-1.1b3/
+-rw-r--r--   0 waddaben   (501) staff       (20)     8728 2023-04-11 06:45:14.759907 idun_guardian_client-1.1b3/PKG-INFO
+-rw-r--r--   0 waddaben   (501) staff       (20)     8163 2023-04-07 09:22:23.000000 idun_guardian_client-1.1b3/README.md
+-rw-r--r--   0 waddaben   (501) staff       (20)      869 2023-04-11 06:44:41.000000 idun_guardian_client-1.1b3/pyproject.toml
+-rw-r--r--   0 waddaben   (501) staff       (20)       38 2023-04-11 06:45:14.760258 idun_guardian_client-1.1b3/setup.cfg
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 06:45:14.753930 idun_guardian_client-1.1b3/src/
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 06:45:14.757801 idun_guardian_client-1.1b3/src/idun_guardian_client/
+-rw-r--r--   0 waddaben   (501) staff       (20)      339 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/__init__.py
+-rw-r--r--   0 waddaben   (501) staff       (20)        0 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/__main__.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     8661 2023-04-11 06:43:23.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/client.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1797 2023-04-07 12:29:46.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/config.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    11623 2023-04-07 15:53:12.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/debug_logs.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    20783 2023-04-07 21:23:44.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/igeb_api.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    30620 2023-04-07 21:24:40.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/igeb_bluetooth.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     2846 2023-04-07 11:46:38.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/igeb_utils.py
+-rw-r--r--   0 waddaben   (501) staff       (20)      191 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/mock_utils.py
+-rw-r--r--   0 waddaben   (501) staff       (20)      164 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/setup.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1214 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/test_producer_consumer.py
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 06:45:14.758871 idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/
+-rw-r--r--   0 waddaben   (501) staff       (20)     8728 2023-04-11 06:45:14.000000 idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/PKG-INFO
+-rw-r--r--   0 waddaben   (501) staff       (20)      752 2023-04-11 06:45:14.000000 idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/SOURCES.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)        1 2023-04-11 06:45:14.000000 idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/dependency_links.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)      137 2023-04-11 06:45:14.000000 idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/requires.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)       21 2023-04-11 06:45:14.000000 idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/top_level.txt
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 06:45:14.759512 idun_guardian_client-1.1b3/tests/
+-rw-r--r--   0 waddaben   (501) staff       (20)     1940 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/tests/test_ble.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1672 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/tests/test_ble_record.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1106 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/tests/test_utils.py
```

### Comparing `idun_guardian_client-1.1b2/PKG-INFO` & `idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: idun_guardian_client
-Version: 1.1b2
+Name: idun-guardian-client
+Version: 1.1b3
 Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
 Author-email: IDUN Technologies <contact@iduntechnologies.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `idun_guardian_client-1.1b2/README.md` & `idun_guardian_client-1.1b3/README.md`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b2/pyproject.toml` & `idun_guardian_client-1.1b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "idun_guardian_client"
-version = "1.1.beta.2"
+version = "1.1.beta.3"
 authors = [
   { name="IDUN Technologies", email="contact@iduntechnologies.com" },
 ]
 description = "Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `idun_guardian_client-1.1b2/src/idun_guardian_client/client.py` & `idun_guardian_client-1.1b3/src/idun_guardian_client/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -118,31 +118,49 @@
     async def start_recording(
         self,
         recording_timer: int = 36000,
         led_sleep: bool = False,
         experiment: str = "None provided",
         impedance_measurement: bool = False,
         mains_freq_60hz: bool = False,
+        sending_timout: float = 1,
+        bi_directional_receiving_timeout: float = 5,
     ):
         """
         Start recording data from the Guardian Earbuds.
         Unidirectional websocket connection to the Guardian Cloud API.
 
         Args:
             recording_timer (int, optional): The duration of the recording in seconds. Defaults to 36000.
             led_sleep (bool, optional): Enable LED sleep mode. Defaults to False.
             experiment (str, optional): The name of the experiment. Defaults to "None provided". This will
                                         go to the log file.
             impedance_measurement (bool, optional): Enable impedance measurement. Defaults to False.
             mains_freq_60hz (bool, optional): Set to True if the mains frequency is 60Hz. Defaults to False.
+            sending_timout (float): The timeout in seconds for sending data to the cloud. Defaults to 1.
+                                    If no data is sent for a second the sending is interupted and the data
+                                    is buffered. If you have a fast internet and you do not want to lose any data,
+                                    then make 0.5 seconds. If you have slow internet and are fine with losing some data,
+                                    then make 5 seconds. The seconds will be the amount lost before noticing internet loss.
+            bi_directional_receiving_timeout (float): The timeout in seconds for receiving data from the cloud. Defaults to 4.
+                                                      If no data is received for 5 seconds the receiving is interupted and the data
+                                                      the connection will be re-established. If you have a fast internet and you do not want to lose
+                                                      bi-directional data, then make 5 seconds. If you have slow internet and are fine with losing some data,
+                                                      then make 10 seconds. The seconds will be the amount lost before noticing internet loss.
 
 
         Raises:
             ValueError: If the recording timer is not valid
         """
+        # set the timers
+        self.guardian_api.runtime_receipt_timeout = sending_timout
+        self.guardian_api.runtime_bi_directional_timeout = (
+            bi_directional_receiving_timeout
+        )
+
         if self.debug:
             logging.info(
                 "[CLIENT]: Recording timer set to: %s seconds", recording_timer
             )
             logging.info("[CLIENT]: Start recording")
 
         print(f"[CLIENT]: Recording timer set to: {recording_timer} seconds")
```

### Comparing `idun_guardian_client-1.1b2/src/idun_guardian_client/config.py` & `idun_guardian_client-1.1b3/src/idun_guardian_client/config.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b2/src/idun_guardian_client/debug_logs.py` & `idun_guardian_client-1.1b3/src/idun_guardian_client/debug_logs.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b2/src/idun_guardian_client/igeb_api.py` & `idun_guardian_client-1.1b3/src/idun_guardian_client/igeb_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,18 +49,18 @@
         self.encrypted_data_queue: asyncio.Queue = asyncio.Queue(
             maxsize=self.encrypted_buffer_size
         )
         self.decrypted_data_queue: asyncio.Queue = asyncio.Queue(
             maxsize=self.decrypted_buffer_size
         )
         self.initial_receipt_timeout = 15
-        self.runtime_receipt_timeout = 1
+        self.runtime_receipt_timeout: float = 1  # Increase if slow connection
         self.current_timeout = self.initial_receipt_timeout
         self.initial_bi_directional_timeout = 15
-        self.runtime_bi_directional_timeout = 4
+        self.runtime_bi_directional_timeout: float = 5  # Increase if slow connection
         self.sending_time_limit = 0.01
         self.bi_directional_timeout = self.initial_bi_directional_timeout
         self.last_saved_time = time.time()
         self.connected = False
         self.data_model = GuardianDataModel(None, None, None, None, None, False)
         self.websocket: Optional[websockets.WebSocketClientProtocol] = None  # type: ignore
         self.final_receipt_got = False
```

### Comparing `idun_guardian_client-1.1b2/src/idun_guardian_client/igeb_bluetooth.py` & `idun_guardian_client-1.1b3/src/idun_guardian_client/igeb_bluetooth.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b2/src/idun_guardian_client/igeb_utils.py` & `idun_guardian_client-1.1b3/src/idun_guardian_client/igeb_utils.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b2/src/idun_guardian_client/test_producer_consumer.py` & `idun_guardian_client-1.1b3/src/idun_guardian_client/test_producer_consumer.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b2/src/idun_guardian_client.egg-info/PKG-INFO` & `idun_guardian_client-1.1b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: idun-guardian-client
-Version: 1.1b2
+Name: idun_guardian_client
+Version: 1.1b3
 Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
 Author-email: IDUN Technologies <contact@iduntechnologies.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `idun_guardian_client-1.1b2/src/idun_guardian_client.egg-info/SOURCES.txt` & `idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b2/tests/test_ble.py` & `idun_guardian_client-1.1b3/tests/test_ble.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b2/tests/test_ble_record.py` & `idun_guardian_client-1.1b3/tests/test_ble_record.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b2/tests/test_utils.py` & `idun_guardian_client-1.1b3/tests/test_utils.py`

 * *Files identical despite different names*

