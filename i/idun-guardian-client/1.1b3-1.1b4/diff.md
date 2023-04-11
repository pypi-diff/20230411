# Comparing `tmp/idun_guardian_client-1.1b3.tar.gz` & `tmp/idun_guardian_client-1.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idun_guardian_client-1.1b3.tar", last modified: Tue Apr 11 06:45:14 2023, max compression
+gzip compressed data, was "idun_guardian_client-1.1b4.tar", last modified: Tue Apr 11 07:28:50 2023, max compression
```

## Comparing `idun_guardian_client-1.1b3.tar` & `idun_guardian_client-1.1b4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 06:45:14.760188 idun_guardian_client-1.1b3/
--rw-r--r--   0 waddaben   (501) staff       (20)     8728 2023-04-11 06:45:14.759907 idun_guardian_client-1.1b3/PKG-INFO
--rw-r--r--   0 waddaben   (501) staff       (20)     8163 2023-04-07 09:22:23.000000 idun_guardian_client-1.1b3/README.md
--rw-r--r--   0 waddaben   (501) staff       (20)      869 2023-04-11 06:44:41.000000 idun_guardian_client-1.1b3/pyproject.toml
--rw-r--r--   0 waddaben   (501) staff       (20)       38 2023-04-11 06:45:14.760258 idun_guardian_client-1.1b3/setup.cfg
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 06:45:14.753930 idun_guardian_client-1.1b3/src/
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 06:45:14.757801 idun_guardian_client-1.1b3/src/idun_guardian_client/
--rw-r--r--   0 waddaben   (501) staff       (20)      339 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/__init__.py
--rw-r--r--   0 waddaben   (501) staff       (20)        0 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/__main__.py
--rw-r--r--   0 waddaben   (501) staff       (20)     8661 2023-04-11 06:43:23.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/client.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1797 2023-04-07 12:29:46.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/config.py
--rw-r--r--   0 waddaben   (501) staff       (20)    11623 2023-04-07 15:53:12.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/debug_logs.py
--rw-r--r--   0 waddaben   (501) staff       (20)    20783 2023-04-07 21:23:44.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/igeb_api.py
--rw-r--r--   0 waddaben   (501) staff       (20)    30620 2023-04-07 21:24:40.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/igeb_bluetooth.py
--rw-r--r--   0 waddaben   (501) staff       (20)     2846 2023-04-07 11:46:38.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/igeb_utils.py
--rw-r--r--   0 waddaben   (501) staff       (20)      191 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/mock_utils.py
--rw-r--r--   0 waddaben   (501) staff       (20)      164 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/setup.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1214 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/src/idun_guardian_client/test_producer_consumer.py
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 06:45:14.758871 idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/
--rw-r--r--   0 waddaben   (501) staff       (20)     8728 2023-04-11 06:45:14.000000 idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/PKG-INFO
--rw-r--r--   0 waddaben   (501) staff       (20)      752 2023-04-11 06:45:14.000000 idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/SOURCES.txt
--rw-r--r--   0 waddaben   (501) staff       (20)        1 2023-04-11 06:45:14.000000 idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/dependency_links.txt
--rw-r--r--   0 waddaben   (501) staff       (20)      137 2023-04-11 06:45:14.000000 idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/requires.txt
--rw-r--r--   0 waddaben   (501) staff       (20)       21 2023-04-11 06:45:14.000000 idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/top_level.txt
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 06:45:14.759512 idun_guardian_client-1.1b3/tests/
--rw-r--r--   0 waddaben   (501) staff       (20)     1940 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/tests/test_ble.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1672 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/tests/test_ble_record.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1106 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b3/tests/test_utils.py
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 07:28:50.205638 idun_guardian_client-1.1b4/
+-rw-r--r--   0 waddaben   (501) staff       (20)     8991 2023-04-11 07:28:50.205391 idun_guardian_client-1.1b4/PKG-INFO
+-rw-r--r--   0 waddaben   (501) staff       (20)     8426 2023-04-11 07:25:03.000000 idun_guardian_client-1.1b4/README.md
+-rw-r--r--   0 waddaben   (501) staff       (20)      869 2023-04-11 07:25:34.000000 idun_guardian_client-1.1b4/pyproject.toml
+-rw-r--r--   0 waddaben   (501) staff       (20)       38 2023-04-11 07:28:50.205692 idun_guardian_client-1.1b4/setup.cfg
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 07:28:50.199288 idun_guardian_client-1.1b4/src/
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 07:28:50.203341 idun_guardian_client-1.1b4/src/idun_guardian_client/
+-rw-r--r--   0 waddaben   (501) staff       (20)      339 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/__init__.py
+-rw-r--r--   0 waddaben   (501) staff       (20)        0 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/__main__.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     8661 2023-04-11 07:10:00.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/client.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1797 2023-04-07 12:29:46.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/config.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    11623 2023-04-07 15:53:12.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/debug_logs.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    20783 2023-04-07 21:23:44.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/igeb_api.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    30620 2023-04-07 21:24:40.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/igeb_bluetooth.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     2846 2023-04-07 11:46:38.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/igeb_utils.py
+-rw-r--r--   0 waddaben   (501) staff       (20)      191 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/mock_utils.py
+-rw-r--r--   0 waddaben   (501) staff       (20)      164 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/setup.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1214 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/test_producer_consumer.py
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 07:28:50.204411 idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/
+-rw-r--r--   0 waddaben   (501) staff       (20)     8991 2023-04-11 07:28:50.000000 idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/PKG-INFO
+-rw-r--r--   0 waddaben   (501) staff       (20)      752 2023-04-11 07:28:50.000000 idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/SOURCES.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)        1 2023-04-11 07:28:50.000000 idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/dependency_links.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)      137 2023-04-11 07:28:50.000000 idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/requires.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)       21 2023-04-11 07:28:50.000000 idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/top_level.txt
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 07:28:50.205055 idun_guardian_client-1.1b4/tests/
+-rw-r--r--   0 waddaben   (501) staff       (20)     1940 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/tests/test_ble.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1672 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/tests/test_ble_record.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1106 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/tests/test_utils.py
```

### Comparing `idun_guardian_client-1.1b3/PKG-INFO` & `idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: idun_guardian_client
-Version: 1.1b3
+Name: idun-guardian-client
+Version: 1.1b4
 Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
 Author-email: IDUN Technologies <contact@iduntechnologies.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
@@ -190,25 +190,29 @@
 ```python
 import asyncio
 from idun_guardian_client import GuardianClient
 
 EXPERIMENT: str = "Sleeping"
 RECORDING_TIMER: int = 36000 # 10 hours in seconds
 LED_SLEEP: bool = False
+SENDING_TIMEOUT: float = 2 # No sending receipt time before interrupt
+BI_DIRECTIONAL_TIMEOUT: float = 20 # No bi-directional data receiving before interrupt
 
 # start a recording session
 bci = GuardianClient()
 bci.address = asyncio.run(bci.search_device())
 
 # start a recording session
 asyncio.run(
     bci.start_recording(
         recording_timer=RECORDING_TIMER,
         led_sleep=LED_SLEEP,
-        experiment=EXPERIMENT
+        experiment=EXPERIMENT,
+        sending_timout=SENDING_TIMEOUT,
+        bi_directional_receiving_timeout=BI_DIRECTIONAL_TIMEOUT,
     )
 )
 
 ```
 
 - To stop the recording, either wait for the timer to run out or interrupt the recording
     - with Mac OS enter the cancellation command in the terminal running the script, this would be `Ctrl+.` or `Ctrl+C`
```

### Comparing `idun_guardian_client-1.1b3/README.md` & `idun_guardian_client-1.1b4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: idun_guardian_client
+Version: 1.1b4
+Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
+Author-email: IDUN Technologies <contact@iduntechnologies.com>
+Classifier: Development Status :: 1 - Planning
+Classifier: License :: Other/Proprietary License
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Natural Language :: English
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
 # User guide and documentation
 
 ## What can you do with the Python SDK?
 
 1. You can use the Python SDK to search for the device.
 2. You can use the Python SDK to connect and record data from the earbud.
 3. You can download the data to your local machine.
@@ -176,25 +190,29 @@
 ```python
 import asyncio
 from idun_guardian_client import GuardianClient
 
 EXPERIMENT: str = "Sleeping"
 RECORDING_TIMER: int = 36000 # 10 hours in seconds
 LED_SLEEP: bool = False
+SENDING_TIMEOUT: float = 2 # No sending receipt time before interrupt
+BI_DIRECTIONAL_TIMEOUT: float = 20 # No bi-directional data receiving before interrupt
 
 # start a recording session
 bci = GuardianClient()
 bci.address = asyncio.run(bci.search_device())
 
 # start a recording session
 asyncio.run(
     bci.start_recording(
         recording_timer=RECORDING_TIMER,
         led_sleep=LED_SLEEP,
-        experiment=EXPERIMENT
+        experiment=EXPERIMENT,
+        sending_timout=SENDING_TIMEOUT,
+        bi_directional_receiving_timeout=BI_DIRECTIONAL_TIMEOUT,
     )
 )
 
 ```
 
 - To stop the recording, either wait for the timer to run out or interrupt the recording
     - with Mac OS enter the cancellation command in the terminal running the script, this would be `Ctrl+.` or `Ctrl+C`
```

### Comparing `idun_guardian_client-1.1b3/pyproject.toml` & `idun_guardian_client-1.1b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "idun_guardian_client"
-version = "1.1.beta.3"
+version = "1.1.beta.4"
 authors = [
   { name="IDUN Technologies", email="contact@iduntechnologies.com" },
 ]
 description = "Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `idun_guardian_client-1.1b3/src/idun_guardian_client/client.py` & `idun_guardian_client-1.1b4/src/idun_guardian_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     async def start_recording(
         self,
         recording_timer: int = 36000,
         led_sleep: bool = False,
         experiment: str = "None provided",
         impedance_measurement: bool = False,
         mains_freq_60hz: bool = False,
-        sending_timout: float = 1,
+        sending_timout: float = 2,
         bi_directional_receiving_timeout: float = 5,
     ):
         """
         Start recording data from the Guardian Earbuds.
         Unidirectional websocket connection to the Guardian Cloud API.
 
         Args:
```

### Comparing `idun_guardian_client-1.1b3/src/idun_guardian_client/config.py` & `idun_guardian_client-1.1b4/src/idun_guardian_client/config.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b3/src/idun_guardian_client/debug_logs.py` & `idun_guardian_client-1.1b4/src/idun_guardian_client/debug_logs.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b3/src/idun_guardian_client/igeb_api.py` & `idun_guardian_client-1.1b4/src/idun_guardian_client/igeb_api.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b3/src/idun_guardian_client/igeb_bluetooth.py` & `idun_guardian_client-1.1b4/src/idun_guardian_client/igeb_bluetooth.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b3/src/idun_guardian_client/igeb_utils.py` & `idun_guardian_client-1.1b4/src/idun_guardian_client/igeb_utils.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b3/src/idun_guardian_client/test_producer_consumer.py` & `idun_guardian_client-1.1b4/src/idun_guardian_client/test_producer_consumer.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/PKG-INFO` & `idun_guardian_client-1.1b4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: idun-guardian-client
-Version: 1.1b3
-Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
-Author-email: IDUN Technologies <contact@iduntechnologies.com>
-Classifier: Development Status :: 1 - Planning
-Classifier: License :: Other/Proprietary License
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Natural Language :: English
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # User guide and documentation
 
 ## What can you do with the Python SDK?
 
 1. You can use the Python SDK to search for the device.
 2. You can use the Python SDK to connect and record data from the earbud.
 3. You can download the data to your local machine.
@@ -190,25 +176,29 @@
 ```python
 import asyncio
 from idun_guardian_client import GuardianClient
 
 EXPERIMENT: str = "Sleeping"
 RECORDING_TIMER: int = 36000 # 10 hours in seconds
 LED_SLEEP: bool = False
+SENDING_TIMEOUT: float = 2 # No sending receipt time before interrupt
+BI_DIRECTIONAL_TIMEOUT: float = 20 # No bi-directional data receiving before interrupt
 
 # start a recording session
 bci = GuardianClient()
 bci.address = asyncio.run(bci.search_device())
 
 # start a recording session
 asyncio.run(
     bci.start_recording(
         recording_timer=RECORDING_TIMER,
         led_sleep=LED_SLEEP,
-        experiment=EXPERIMENT
+        experiment=EXPERIMENT,
+        sending_timout=SENDING_TIMEOUT,
+        bi_directional_receiving_timeout=BI_DIRECTIONAL_TIMEOUT,
     )
 )
 
 ```
 
 - To stop the recording, either wait for the timer to run out or interrupt the recording
     - with Mac OS enter the cancellation command in the terminal running the script, this would be `Ctrl+.` or `Ctrl+C`
```

### Comparing `idun_guardian_client-1.1b3/src/idun_guardian_client.egg-info/SOURCES.txt` & `idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b3/tests/test_ble.py` & `idun_guardian_client-1.1b4/tests/test_ble.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b3/tests/test_ble_record.py` & `idun_guardian_client-1.1b4/tests/test_ble_record.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b3/tests/test_utils.py` & `idun_guardian_client-1.1b4/tests/test_utils.py`

 * *Files identical despite different names*

