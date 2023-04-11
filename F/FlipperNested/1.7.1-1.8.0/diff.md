# Comparing `tmp/FlipperNested-1.7.1.tar.gz` & `tmp/FlipperNested-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlipperNested-1.7.1.tar", last modified: Mon Apr 10 20:26:40 2023, max compression
+gzip compressed data, was "FlipperNested-1.8.0.tar", last modified: Tue Apr 11 18:05:22 2023, max compression
```

## Comparing `FlipperNested-1.7.1.tar` & `FlipperNested-1.8.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/FlipperNested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/FlipperNested/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/proto/flipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/FlipperNested/proto/storage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/FlipperNested.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-10 20:26:40.000000 FlipperNested-1.7.1/FlipperNested.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-10 20:26:40.000000 FlipperNested-1.7.1/FlipperNested.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:26:40.000000 FlipperNested-1.7.1/FlipperNested.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-10 20:26:40.000000 FlipperNested-1.7.1/FlipperNested.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 20:26:40.000000 FlipperNested-1.7.1/FlipperNested.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-10 20:26:40.000000 FlipperNested-1.7.1/FlipperNested.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/NestedSolver/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/bucketsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/bucketsort.h
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/crapto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/crapto1.h
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/crypto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/library.c
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/library.h
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/parity.h
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/NestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:26:40.214461 FlipperNested-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/tests/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 20:26:29.000000 FlipperNested-1.7.1/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:22.282779 FlipperNested-1.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:22.278779 FlipperNested-1.8.0/FlipperNested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:22.278779 FlipperNested-1.8.0/FlipperNested/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/proto/flipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/FlipperNested/proto/storage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:22.278779 FlipperNested-1.8.0/FlipperNested.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-11 18:05:22.000000 FlipperNested-1.8.0/FlipperNested.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-11 18:05:22.000000 FlipperNested-1.8.0/FlipperNested.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:05:22.000000 FlipperNested-1.8.0/FlipperNested.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 18:05:22.000000 FlipperNested-1.8.0/FlipperNested.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 18:05:22.000000 FlipperNested-1.8.0/FlipperNested.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 18:05:22.000000 FlipperNested-1.8.0/FlipperNested.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:22.278779 FlipperNested-1.8.0/NestedSolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/bucketsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/bucketsort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/crapto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/crapto1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/crypto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/library.c
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/library.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/parity.h
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/progress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/progress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/NestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-11 18:05:22.282779 FlipperNested-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:05:22.282779 FlipperNested-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:22.282779 FlipperNested-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/tests/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 18:05:12.000000 FlipperNested-1.8.0/tests/test_parse.py
```

### Comparing `FlipperNested-1.7.1/FlipperNested/bridge.py` & `FlipperNested-1.8.0/FlipperNested/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     @staticmethod
     def get_port():
         ports = serial.tools.list_ports.comports()
         for port, desc, hwid in ports:
             a = hwid.split()
             if "VID:PID=0483:5740" in a or (
-                    hwid == "n/a" and input("Is {} your Flipper COM port? [y/n] > ".format(port)).lower() == "y"):
+                    hwid == "n/a" and input("Is {} your Flipper Zero serial port? [y/n] > ".format(port)).lower() == "y"):
                 return port
 
     def _read_varint_32(self) -> int:
         MASK = (1 << 32) - 1
 
         result = 0
         shift = 0
```

### Comparing `FlipperNested-1.7.1/FlipperNested/cli.py` & `FlipperNested-1.8.0/FlipperNested/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 
 from FlipperNested.main import FlipperNested
 
 
 def main():
     parser = argparse.ArgumentParser(description='Calculate keys after Nested attack')
     parser.add_argument('--uid', type=str, help='Recover only for this UID', default='')
-    parser.add_argument('--save', action='store_true', help='Debug: Save keys/nonces from Flipper')
-    parser.add_argument('--file', type=argparse.FileType('r'), help='Debug: recover keys from local .nonces file')
-    # parser.add_argument('--progress_bar', action='store_true', help='Debug: show key recovery progress')
+    parser.add_argument('--progress', action='store_true', help='Show key recovery progress bar')
+    parser.add_argument('--save', action='store_true', help='Debug: Save nonces/keys from Flipper')
+    parser.add_argument('--file', type=argparse.FileType('r'), help='Debug: Recover keys from local .nonces file')
     parser.set_defaults(debug=False)
     args = parser.parse_args()
     flipper = FlipperNested()
     flipper.run(args)
```

### Comparing `FlipperNested-1.7.1/FlipperNested/main.py` & `FlipperNested-1.8.0/FlipperNested/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,25 +17,26 @@
         self.filename = None
         self.nonces = None
         self.found_keys = None
         self.bruteforce_distance = [0, 0]
         self.progress_bar = False
 
     def run(self, args=None):
-        # if args and args.progress_bar:
-        #     self.progress_bar = True
+        if args and args.progress:
+            self.progress_bar = True
         if not args or args and not args.file:
             self.connection = FlipperBridge()
             self.extract_nonces_from_flipper(args)
         else:
             self.extract_nonces_from_file(args.file)
 
     def parse_file(self, contents):
         self.nonces = {"A": {}, "B": {}}
         self.found_keys = {"A": {}, "B": {}}
+        self.bruteforce_distance = [0, 0]
         lines = contents.splitlines()[1:]
         version_string = lines.pop(0)
         if "Version" not in version_string:
             print("No version info in", self.filename)
             return False
         file_version = int(version_string.split(": ")[1])
         if file_version != self.VERSION:
@@ -79,15 +80,16 @@
                 contents = self.connection.file_read("/ext/nfc/nested/" + file["name"]).decode()
                 if not self.parse_file(contents):
                     print("Failed to parse", file["name"])
                     continue
                 if args and args.save:
                     open(file["name"], "w+").write(contents)
                     print("Saved nonces to", file["name"])
-                self.crack_nonces()
+                if self.crack_nonces():
+                    break
                 self.save_keys_to_flipper(args and args.save)
 
     def extract_nonces_from_file(self, file):
         self.filename = file.name
         if not self.parse_file(file.read()):
             print("Failed to parse", self.filename)
             return
@@ -100,39 +102,40 @@
                 for info in self.nonces[key_type][sector]:
                     print("Calculating for key type", key_type + ", sector", sector)
                     m = Manager()
                     q = m.Queue()
 
                     value = info[:-2]
                     value.append(self.bruteforce_distance)
+                    value.append(self.progress_bar)
                     value.insert(0, q)
 
                     p = Process(target=wrapper, args=value)
                     p.start()
 
                     try:
                         p.join()
                     except KeyboardInterrupt:
                         print("Stopping...")
                         p.kill()
-                        return
+                        return True
 
                     try:
                         keys = q.get(timeout=1).split(";")
                     except _queue.Empty:
                         print("Something went VERY wrong in key recovery.\nYou MUST report this to developer!")
                         return
                     keys.pop()
 
                     print(f"Found {str(len(keys))} key(s):", keys)
 
                     if keys:
                         self.found_keys[key_type][sector] = keys
                         break
-                    elif value == self.nonces[key_type][sector][-1]:
+                    elif info == self.nonces[key_type][sector][-1]:
                         print("Failed to find keys for this sector, try running Nested attack again")
 
     def save_keys_to_string(self):
         output = ""
         for key_type in self.found_keys.keys():
             for sector in self.found_keys[key_type].keys():
                 for key in self.found_keys[key_type][sector]:
@@ -180,17 +183,17 @@
         key_type, sec = groups[0], int(groups[-1])
         values = list(map(lambda x: int(x, 16) if x.startswith("0x") else int(x), groups[1:-1]))
         values.append(sec)
         values.append(key_type)
         return values
 
     @staticmethod
-    def calculate_keys(uid, nt0, ks0, par0, nt1, ks1, par1, bruteforce_distance):
+    def calculate_keys(uid, nt0, ks0, par0, nt1, ks1, par1, bruteforce_distance, progress):
         import faulthandler
         faulthandler.enable()
         import nested
         if bruteforce_distance != [0, 0]:
             run = nested.run_full_nested(uid, nt0, ks0, par0, nt1, ks1, par1, bruteforce_distance[0],
-                                         bruteforce_distance[1])
+                                         bruteforce_distance[1], progress)
         else:
             run = nested.run_nested(uid, nt0, ks0, nt1, ks1)
         return run
```

### Comparing `FlipperNested-1.7.1/FlipperNested/proto/flipper_pb2.py` & `FlipperNested-1.8.0/FlipperNested/proto/flipper_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.7.1/FlipperNested/proto/storage_pb2.py` & `FlipperNested-1.8.0/FlipperNested/proto/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.7.1/FlipperNested.egg-info/PKG-INFO` & `FlipperNested-1.8.0/FlipperNested.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.7.1
+Version: 1.8.0
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -41,19 +41,22 @@
 ```bash
 $ FlipperNested
 Checking 12345678.nonces
 Calculating for key type A, sector 0
 Found 1 key(s): ['ffffffffffff']
 ...
 Found potential 32 keys, use "Check found keys" in app
+```
 
+```bash
 $ FlipperNested --help
-usage: FlipperNested [-h] [--uid UID] [--save | --no-save]
+usage: FlipperNested [-h] [--uid UID] [--progress] [--save] [--file FILE]
 
 Calculate keys after Nested attack
 
 options:
-  -h, --help         show this help message and exit
-  --uid UID          Recover only for this UID
-  --save, --no-save  Debug: Save keys/nonces from Flipper (default: False)
-
+  -h, --help   show this help message and exit
+  --uid UID    Recover only for this UID
+  --progress   Show key recovery progress bar
+  --save       Debug: Save nonces/keys from Flipper
+  --file FILE  Debug: Recover keys from local .nonces file
 ```
```

### Comparing `FlipperNested-1.7.1/FlipperNested.egg-info/SOURCES.txt` & `FlipperNested-1.8.0/FlipperNested.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -20,11 +20,13 @@
 NestedSolver/bucketsort.h
 NestedSolver/crapto1.c
 NestedSolver/crapto1.h
 NestedSolver/crypto1.c
 NestedSolver/library.c
 NestedSolver/library.h
 NestedSolver/parity.h
+NestedSolver/progress.c
+NestedSolver/progress.h
 NestedSolver/python.c
 tests/test_calculate.py
 tests/test_import.py
 tests/test_parse.py
```

### Comparing `FlipperNested-1.7.1/LICENSE.md` & `FlipperNested-1.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.7.1/NestedSolver/bucketsort.c` & `FlipperNested-1.8.0/NestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.7.1/NestedSolver/bucketsort.h` & `FlipperNested-1.8.0/NestedSolver/bucketsort.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.7.1/NestedSolver/crapto1.c` & `FlipperNested-1.8.0/NestedSolver/crapto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.7.1/NestedSolver/crapto1.h` & `FlipperNested-1.8.0/NestedSolver/crapto1.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.7.1/NestedSolver/crypto1.c` & `FlipperNested-1.8.0/NestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.7.1/NestedSolver/library.c` & `FlipperNested-1.8.0/NestedSolver/library.c`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 #include <inttypes.h>
 #include "library.h"
 #include "crapto1.h"
 #include "parity.h"
+#include "progress.h"
 
 static int compare_uint64(const void *a, const void *b) {
     if (*(uint64_t *) b == *(uint64_t *) a) return 0;
     if (*(uint64_t *) b < *(uint64_t *) a) return 1;
     return -1;
 }
 
@@ -190,26 +191,28 @@
     info->free = false;
     nested_calculate(info);
     return info->keys;
 }
 
 char *
 run_full_nested(uint32_t uid, uint32_t nt0, uint32_t ks0, uint32_t par0, uint32_t nt1, uint32_t ks1, uint32_t par1,
-                int from, int to) {
+                int from, int to, bool progress) {
     #if _MSC_VER
         pthread_t thread_id[16384];
         uint32_t found_second_array[16384];
     #else
         pthread_t thread_id[to];
         uint32_t found_second_array[to];
     #endif
     uint32_t found_first, found_second;
     bool found = false;
     uint32_t i;
+    if (progress) printf("\n");
     for (int first = from; first < to; first++) {
+        if (progress) print_progress(first - from, to - from);
         i = 0;
         void *status = NULL;
 
         for (int second = from; second < to; second++) {
             uint8_t *par0_decoded = decode_parity(par0);
             uint8_t *par1_decoded = decode_parity(par1);
             if (!valid_nonce(prng_successor(nt0, first), ks0, ks0 ^ prng_successor(nt0, first), par0_decoded) ||
@@ -250,13 +253,15 @@
             found_info->nt0 = prng_successor(nt0, found_first);
             found_info->ks0 = ks0 ^ found_info->nt0;
             found_info->nt1 = prng_successor(nt1, found_second);
             found_info->ks1 = ks1 ^ found_info->nt1;
             found_info->keys = calloc(256, sizeof(char) * 14);
             found_info->free = false;
             nested_calculate(found_info);
+            if (progress) exit_progress();
             return found_info->keys;
         }
     }
 
+    if (progress) exit_progress();
     return calloc(1, 1);
 }
```

### Comparing `FlipperNested-1.7.1/NestedSolver/library.h` & `FlipperNested-1.8.0/NestedSolver/library.h`

 * *Files 12% similar despite different names*

```diff
@@ -27,9 +27,9 @@
     uint32_t ks1;
     char *keys;
     bool free;
 } InfoList_t;
 
 char* run_nested(uint32_t uid, uint32_t nt0, uint32_t ks0, uint32_t nt1, uint32_t ks1);
 
-char* run_full_nested(uint32_t uid, uint32_t nt0, uint32_t ks0, uint32_t par0, uint32_t nt1, uint32_t ks1, uint32_t par1, int from, int to);
+char* run_full_nested(uint32_t uid, uint32_t nt0, uint32_t ks0, uint32_t par0, uint32_t nt1, uint32_t ks1, uint32_t par1, int from, int to, bool progress);
 #endif //MIFARE_LIB_LIBRARY_H
```

### Comparing `FlipperNested-1.7.1/NestedSolver/parity.h` & `FlipperNested-1.8.0/NestedSolver/parity.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.7.1/NestedSolver/python.c` & `FlipperNested-1.8.0/NestedSolver/python.c`

 * *Files 22% similar despite different names*

```diff
@@ -10,21 +10,21 @@
     char *output = run_nested((uint32_t) uid, (uint32_t) nt0, (uint32_t) ks0, (uint32_t) nt1, (uint32_t) ks1);
 
     return Py_BuildValue("s", output);
 }
 
 static PyObject *run_full_nested_python(PyObject *self, PyObject *args) {
     uint64_t uid, nt0, ks0, par0, nt1, ks1, par1;
-    int from, to;
-    if (!PyArg_ParseTuple(args, "kkkkkkkii", &uid, &nt0, &ks0, &par0, &nt1, &ks1, &par1, &from, &to)) {
+    int from, to, progress;
+    if (!PyArg_ParseTuple(args, "kkkkkkkiip", &uid, &nt0, &ks0, &par0, &nt1, &ks1, &par1, &from, &to, &progress)) {
         return NULL;
     }
 
     char *output = run_full_nested((uint32_t) uid, (uint32_t) nt0, (uint32_t) ks0, (uint32_t) par0, (uint32_t) nt1,
-                                   (uint32_t) ks1, (uint32_t) par1, from, to);
+                                   (uint32_t) ks1, (uint32_t) par1, from, to, progress);
 
     return Py_BuildValue("s", output);
 }
 
 static PyMethodDef nested_methods[] = {{"run_nested",      run_nested_python,      METH_VARARGS, "Run nested"},
                                        {"run_full_nested", run_full_nested_python, METH_VARARGS, "Run full nested"},
                                        {NULL, NULL,                                0, NULL}        /* Sentinel */
```

### Comparing `FlipperNested-1.7.1/PKG-INFO` & `FlipperNested-1.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.7.1
+Version: 1.8.0
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -41,19 +41,22 @@
 ```bash
 $ FlipperNested
 Checking 12345678.nonces
 Calculating for key type A, sector 0
 Found 1 key(s): ['ffffffffffff']
 ...
 Found potential 32 keys, use "Check found keys" in app
+```
 
+```bash
 $ FlipperNested --help
-usage: FlipperNested [-h] [--uid UID] [--save | --no-save]
+usage: FlipperNested [-h] [--uid UID] [--progress] [--save] [--file FILE]
 
 Calculate keys after Nested attack
 
 options:
-  -h, --help         show this help message and exit
-  --uid UID          Recover only for this UID
-  --save, --no-save  Debug: Save keys/nonces from Flipper (default: False)
-
+  -h, --help   show this help message and exit
+  --uid UID    Recover only for this UID
+  --progress   Show key recovery progress bar
+  --save       Debug: Save nonces/keys from Flipper
+  --file FILE  Debug: Recover keys from local .nonces file
 ```
```

### Comparing `FlipperNested-1.7.1/README.md` & `FlipperNested-1.8.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -23,19 +23,22 @@
 ```bash
 $ FlipperNested
 Checking 12345678.nonces
 Calculating for key type A, sector 0
 Found 1 key(s): ['ffffffffffff']
 ...
 Found potential 32 keys, use "Check found keys" in app
+```
 
+```bash
 $ FlipperNested --help
-usage: FlipperNested [-h] [--uid UID] [--save | --no-save]
+usage: FlipperNested [-h] [--uid UID] [--progress] [--save] [--file FILE]
 
 Calculate keys after Nested attack
 
 options:
-  -h, --help         show this help message and exit
-  --uid UID          Recover only for this UID
-  --save, --no-save  Debug: Save keys/nonces from Flipper (default: False)
-
+  -h, --help   show this help message and exit
+  --uid UID    Recover only for this UID
+  --progress   Show key recovery progress bar
+  --save       Debug: Save nonces/keys from Flipper
+  --file FILE  Debug: Recover keys from local .nonces file
 ```
```

### Comparing `FlipperNested-1.7.1/setup.py` & `FlipperNested-1.8.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 if os.name == 'nt':
     include_dirs = ['build\\pthreads']
     extra_compile_args = ['-DNEED_FTIME']
     libraries = ['pthreadVC2']
 
 nested_solver = Extension('nested',
                           sources=['NestedSolver/python.c', 'NestedSolver/crapto1.c', 'NestedSolver/library.c',
-                                   'NestedSolver/bucketsort.c', 'NestedSolver/crypto1.c'], include_dirs=include_dirs,
-                          library_dirs=include_dirs, extra_compile_args=extra_compile_args, libraries=libraries)
+                                   'NestedSolver/bucketsort.c', 'NestedSolver/crypto1.c', 'NestedSolver/progress.c'],
+                          include_dirs=include_dirs, library_dirs=include_dirs, extra_compile_args=extra_compile_args,
+                          libraries=libraries)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FlipperNested",
-    version="1.7.1",
+    version="1.8.0",
     author="AloneLiberty",
     description="Recover keys from collected nonces",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AloneLiberty/FlipperNestedRecovery",
     entry_points={'console_scripts': ['FlipperNested = FlipperNested.cli:main']},
     install_requires=['protobuf>4', 'pyserial'],
@@ -39,9 +40,10 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: MacOS",
         "Operating System :: POSIX :: Linux",
         "Operating System :: Microsoft :: Windows"
     ],
     headers=['NestedSolver/library.h', 'NestedSolver/parity.h',
-             'NestedSolver/crapto1.h', 'NestedSolver/bucketsort.h'],
+             'NestedSolver/crapto1.h', 'NestedSolver/bucketsort.h',
+             'NestedSolver/progress.h'],
 )
```

