# Comparing `tmp/FlipperNested-1.8.0.tar.gz` & `tmp/FlipperNested-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlipperNested-1.8.0.tar", last modified: Tue Apr 11 18:05:22 2023, max compression
+gzip compressed data, was "FlipperNested-1.8.1.tar", last modified: Tue Apr 11 18:23:12 2023, max compression
```

## Comparing `FlipperNested-1.8.0.tar` & `FlipperNested-1.8.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:22.282779 FlipperNested-1.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:22.278779 FlipperNested-1.8.0/FlipperNested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:22.278779 FlipperNested-1.8.0/FlipperNested/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/proto/flipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/proto/storage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:22.278779 FlipperNested-1.8.0/FlipperNested.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-11 18:05:22.000000 FlipperNested-1.8.0/FlipperNested.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-11 18:05:22.000000 FlipperNested-1.8.0/FlipperNested.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:05:22.000000 FlipperNested-1.8.0/FlipperNested.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 18:05:22.000000 FlipperNested-1.8.0/FlipperNested.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 18:05:22.000000 FlipperNested-1.8.0/FlipperNested.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 18:05:22.000000 FlipperNested-1.8.0/FlipperNested.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:22.278779 FlipperNested-1.8.0/NestedSolver/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/bucketsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/bucketsort.h
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/crapto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/crapto1.h
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/crypto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/library.c
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/library.h
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/parity.h
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/progress.c
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/progress.h
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-11 18:05:22.282779 FlipperNested-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:05:22.282779 FlipperNested-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:22.282779 FlipperNested-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/tests/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:23:12.714075 FlipperNested-1.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:23:12.710075 FlipperNested-1.8.1/FlipperNested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/FlipperNested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/FlipperNested/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/FlipperNested/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/FlipperNested/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/FlipperNested/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:23:12.714075 FlipperNested-1.8.1/FlipperNested/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/FlipperNested/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/FlipperNested/proto/flipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/FlipperNested/proto/storage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:23:12.714075 FlipperNested-1.8.1/FlipperNested.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-11 18:23:12.000000 FlipperNested-1.8.1/FlipperNested.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-11 18:23:12.000000 FlipperNested-1.8.1/FlipperNested.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:23:12.000000 FlipperNested-1.8.1/FlipperNested.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 18:23:12.000000 FlipperNested-1.8.1/FlipperNested.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 18:23:12.000000 FlipperNested-1.8.1/FlipperNested.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 18:23:12.000000 FlipperNested-1.8.1/FlipperNested.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:23:12.714075 FlipperNested-1.8.1/NestedSolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/NestedSolver/bucketsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/NestedSolver/bucketsort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/NestedSolver/crapto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/NestedSolver/crapto1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/NestedSolver/crypto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/NestedSolver/library.c
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/NestedSolver/library.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/NestedSolver/parity.h
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/NestedSolver/progress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/NestedSolver/progress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/NestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-11 18:23:12.714075 FlipperNested-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:23:12.714075 FlipperNested-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:23:12.714075 FlipperNested-1.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/tests/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 18:23:05.000000 FlipperNested-1.8.1/tests/test_parse.py
```

### Comparing `FlipperNested-1.8.0/FlipperNested/bridge.py` & `FlipperNested-1.8.1/FlipperNested/bridge.py`

 * *Files 21% similar despite different names*

```diff
@@ -29,32 +29,51 @@
         return flipper
 
     def start_rpc_session(self) -> None:
         self._serial.read_until(b">: ")
         self._serial.write(b"start_rpc_session\r")
         self._serial.read_until(b"\n")
 
-    @staticmethod
-    def get_port():
+    def get_port(self):
         ports = serial.tools.list_ports.comports()
+        potential_ports = []
         for port, desc, hwid in ports:
             a = hwid.split()
-            if "VID:PID=0483:5740" in a or (
-                    hwid == "n/a" and input("Is {} your Flipper Zero serial port? [y/n] > ".format(port)).lower() == "y"):
+            if "VID:PID=0483:5740" in a:
+                return port
+            elif hwid == "n/a":
+                potential_ports.append(port)
+        for port in potential_ports:
+            if self.check_port(port):
                 return port
+        if len(potential_ports):
+            print("[Error] Can't guess Flipper Zero serial port. Fallback to manual mode")
+            print("Make sure Flipper Zero is connected and not used by any other software")
+            for port in potential_ports:
+                if input("Is {} your Flipper Zero serial port? [y/n] > ".format(port)).lower() == "y":
+                    return port
+
+    @staticmethod
+    def check_port(port):
+        try:
+            flipper = serial.Serial(port, timeout=1)
+            flipper.flushOutput()
+            flipper.flushInput()
+            if b"Flipper Zero Command Line Interface!" in flipper.read_until(b">: "):
+                return True
+        except:
+            pass
 
     def _read_varint_32(self) -> int:
         MASK = (1 << 32) - 1
 
         result = 0
         shift = 0
         while 1:
-            b = int.from_bytes(
-                self._serial.read(size=1), byteorder="little", signed=False
-            )
+            b = int.from_bytes(self._serial.read(size=1), byteorder="little", signed=False)
             result |= (b & 0x7F) << shift
 
             if not b & 0x80:
                 result &= MASK
                 result = int(result)
                 return result
             shift += 7
@@ -69,18 +88,15 @@
         flipper_message.command_id = command_id
         if not command_id:
             flipper_message.command_id = self.get_command_id()
         flipper_message.has_next = has_next
 
         flipper_message.command_status = flipper_pb2.CommandStatus.Value("OK")
         getattr(flipper_message, cmd_name).CopyFrom(cmd_data)
-        data = bytearray(
-            _VarintBytes(flipper_message.ByteSize())
-            + flipper_message.SerializeToString()
-        )
+        data = bytearray(_VarintBytes(flipper_message.ByteSize()) + flipper_message.SerializeToString())
 
         self._serial.write(data)
 
     def _rpc_read_answer(self):
         while True:
             data = self._rpc_read_any()
             if data.command_id == self.command_id:
@@ -98,33 +114,23 @@
         return data
 
     def get_files(self, path="/ext") -> list:
         storage_response = []
         cmd_data = storage_pb2.ListRequest()
 
         cmd_data.path = path
-        rep_data = self._rpc_send_and_read_answer(
-            cmd_data, "storage_list_request"
-        )
+        rep_data = self._rpc_send_and_read_answer(cmd_data, "storage_list_request")
 
         storage_response.extend(
-            MessageToDict(
-                message=rep_data.storage_list_response,
-                including_default_value_fields=True,
-            )["file"]
-        )
+            MessageToDict(message=rep_data.storage_list_response, including_default_value_fields=True, )["file"])
 
         while rep_data.has_next:
             rep_data = self._rpc_read_answer()
             storage_response.extend(
-                MessageToDict(
-                    message=rep_data.storage_list_response,
-                    including_default_value_fields=True,
-                )["file"]
-            )
+                MessageToDict(message=rep_data.storage_list_response, including_default_value_fields=True, )["file"])
 
         return storage_response
 
     def file_read(self, path=None):
         storage_response = []
         cmd_data = storage_pb2.ReadRequest()
         cmd_data.path = path
@@ -152,23 +158,13 @@
         for chunk in range(0, data_len, chunk_size):
 
             chunk_data = data[chunk: chunk + chunk_size]
 
             cmd_data.file.data = chunk_data
 
             if (chunk + chunk_size) < data_len:
-                self._rpc_send(
-                    cmd_data,
-                    "storage_write_request",
-                    has_next=True,
-                    command_id=command_id,
-                )
+                self._rpc_send(cmd_data, "storage_write_request", has_next=True, command_id=command_id, )
             else:
-                self._rpc_send(
-                    cmd_data,
-                    "storage_write_request",
-                    has_next=False,
-                    command_id=command_id,
-                )
+                self._rpc_send(cmd_data, "storage_write_request", has_next=False, command_id=command_id, )
                 break
 
         self._rpc_read_answer()
```

### Comparing `FlipperNested-1.8.0/FlipperNested/cli.py` & `FlipperNested-1.8.1/FlipperNested/cli.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/FlipperNested/main.py` & `FlipperNested-1.8.1/FlipperNested/main.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/FlipperNested/proto/flipper_pb2.py` & `FlipperNested-1.8.1/FlipperNested/proto/flipper_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/FlipperNested/proto/storage_pb2.py` & `FlipperNested-1.8.1/FlipperNested/proto/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/FlipperNested.egg-info/PKG-INFO` & `FlipperNested-1.8.1/FlipperNested.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.8.0
+Version: 1.8.1
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-1.8.0/FlipperNested.egg-info/SOURCES.txt` & `FlipperNested-1.8.1/FlipperNested.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/LICENSE.md` & `FlipperNested-1.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/NestedSolver/bucketsort.c` & `FlipperNested-1.8.1/NestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/NestedSolver/bucketsort.h` & `FlipperNested-1.8.1/NestedSolver/bucketsort.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/NestedSolver/crapto1.c` & `FlipperNested-1.8.1/NestedSolver/crapto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/NestedSolver/crapto1.h` & `FlipperNested-1.8.1/NestedSolver/crapto1.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/NestedSolver/crypto1.c` & `FlipperNested-1.8.1/NestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/NestedSolver/library.c` & `FlipperNested-1.8.1/NestedSolver/library.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/NestedSolver/library.h` & `FlipperNested-1.8.1/NestedSolver/library.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/NestedSolver/parity.h` & `FlipperNested-1.8.1/NestedSolver/parity.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/NestedSolver/progress.c` & `FlipperNested-1.8.1/NestedSolver/progress.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/NestedSolver/python.c` & `FlipperNested-1.8.1/NestedSolver/python.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/PKG-INFO` & `FlipperNested-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.8.0
+Version: 1.8.1
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-1.8.0/README.md` & `FlipperNested-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.0/setup.py` & `FlipperNested-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                           libraries=libraries)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FlipperNested",
-    version="1.8.0",
+    version="1.8.1",
     author="AloneLiberty",
     description="Recover keys from collected nonces",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AloneLiberty/FlipperNestedRecovery",
     entry_points={'console_scripts': ['FlipperNested = FlipperNested.cli:main']},
     install_requires=['protobuf>4', 'pyserial'],
```

### Comparing `FlipperNested-1.8.0/tests/test_calculate.py` & `FlipperNested-1.8.1/tests/test_calculate.py`

 * *Files identical despite different names*

