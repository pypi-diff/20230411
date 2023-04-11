# Comparing `tmp/FlipperNested-1.8.2.tar.gz` & `tmp/FlipperNested-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlipperNested-1.8.2.tar", last modified: Tue Apr 11 20:20:32 2023, max compression
+gzip compressed data, was "FlipperNested-1.8.3.tar", last modified: Tue Apr 11 21:23:59 2023, max compression
```

## Comparing `FlipperNested-1.8.2.tar` & `FlipperNested-1.8.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:32.514052 FlipperNested-1.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:32.510052 FlipperNested-1.8.2/FlipperNested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/FlipperNested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/FlipperNested/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/FlipperNested/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/FlipperNested/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/FlipperNested/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:32.510052 FlipperNested-1.8.2/FlipperNested/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/FlipperNested/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/FlipperNested/proto/flipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/FlipperNested/proto/storage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:32.510052 FlipperNested-1.8.2/FlipperNested.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-11 20:20:32.000000 FlipperNested-1.8.2/FlipperNested.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-11 20:20:32.000000 FlipperNested-1.8.2/FlipperNested.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:20:32.000000 FlipperNested-1.8.2/FlipperNested.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 20:20:32.000000 FlipperNested-1.8.2/FlipperNested.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 20:20:32.000000 FlipperNested-1.8.2/FlipperNested.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 20:20:32.000000 FlipperNested-1.8.2/FlipperNested.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:32.514052 FlipperNested-1.8.2/NestedSolver/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/NestedSolver/bucketsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/NestedSolver/bucketsort.h
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/NestedSolver/crapto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/NestedSolver/crapto1.h
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/NestedSolver/crypto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/NestedSolver/library.c
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/NestedSolver/library.h
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/NestedSolver/parity.h
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/NestedSolver/progress.c
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/NestedSolver/progress.h
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/NestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-11 20:20:32.514052 FlipperNested-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 20:20:32.514052 FlipperNested-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:32.514052 FlipperNested-1.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/tests/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 20:20:22.000000 FlipperNested-1.8.2/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:59.364143 FlipperNested-1.8.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:59.360143 FlipperNested-1.8.3/FlipperNested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:59.360143 FlipperNested-1.8.3/FlipperNested/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/proto/flipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/proto/storage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:59.360143 FlipperNested-1.8.3/FlipperNested.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-11 21:23:59.000000 FlipperNested-1.8.3/FlipperNested.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-11 21:23:59.000000 FlipperNested-1.8.3/FlipperNested.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:23:59.000000 FlipperNested-1.8.3/FlipperNested.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 21:23:59.000000 FlipperNested-1.8.3/FlipperNested.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 21:23:59.000000 FlipperNested-1.8.3/FlipperNested.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 21:23:59.000000 FlipperNested-1.8.3/FlipperNested.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:59.364143 FlipperNested-1.8.3/NestedSolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/bucketsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/bucketsort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/crapto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/crapto1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/crypto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/library.c
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/library.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/parity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/progress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/progress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-11 21:23:59.364143 FlipperNested-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 21:23:59.364143 FlipperNested-1.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:59.364143 FlipperNested-1.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/tests/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/tests/test_parse.py
```

### Comparing `FlipperNested-1.8.2/FlipperNested/bridge.py` & `FlipperNested-1.8.3/FlipperNested/bridge.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/FlipperNested/cli.py` & `FlipperNested-1.8.3/FlipperNested/cli.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/FlipperNested/main.py` & `FlipperNested-1.8.3/FlipperNested/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,31 +80,31 @@
                 contents = self.connection.file_read("/ext/nfc/nested/" + file["name"]).decode()
                 if not self.parse_file(contents):
                     print("Failed to parse", file["name"])
                     continue
                 if args and args.save:
                     open(file["name"], "w+").write(contents)
                     print("Saved nonces to", file["name"])
-                if self.crack_nonces():
+                if self.recover_keys():
                     break
                 self.save_keys_to_flipper(args and args.save)
 
     def extract_nonces_from_file(self, file):
         self.filename = file.name
         if not self.parse_file(file.read()):
             print("Failed to parse", self.filename)
             return
-        self.crack_nonces()
+        self.recover_keys()
         self.save_keys_to_file()
 
-    def crack_nonces(self):
+    def recover_keys(self):
         for key_type in self.nonces.keys():
             for sector in self.nonces[key_type].keys():
                 for info in self.nonces[key_type][sector]:
-                    print("Calculating for key type", key_type + ", sector", sector)
+                    print("Recovering key type", key_type + ", sector", sector)
                     m = Manager()
                     q = m.Queue()
 
                     value = info[:-2]
                     value.append(self.bruteforce_distance)
                     value.append(self.progress_bar)
                     value.insert(0, q)
```

### Comparing `FlipperNested-1.8.2/FlipperNested/proto/flipper_pb2.py` & `FlipperNested-1.8.3/FlipperNested/proto/flipper_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/FlipperNested/proto/storage_pb2.py` & `FlipperNested-1.8.3/FlipperNested/proto/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/FlipperNested.egg-info/PKG-INFO` & `FlipperNested-1.8.3/FlipperNested.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.8.2
+Version: 1.8.3
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-1.8.2/FlipperNested.egg-info/SOURCES.txt` & `FlipperNested-1.8.3/FlipperNested.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/LICENSE.md` & `FlipperNested-1.8.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/NestedSolver/bucketsort.c` & `FlipperNested-1.8.3/NestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/NestedSolver/bucketsort.h` & `FlipperNested-1.8.3/NestedSolver/bucketsort.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/NestedSolver/crapto1.c` & `FlipperNested-1.8.3/NestedSolver/crapto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/NestedSolver/crapto1.h` & `FlipperNested-1.8.3/NestedSolver/crapto1.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/NestedSolver/crypto1.c` & `FlipperNested-1.8.3/NestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/NestedSolver/library.c` & `FlipperNested-1.8.3/NestedSolver/library.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/NestedSolver/library.h` & `FlipperNested-1.8.3/NestedSolver/library.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/NestedSolver/parity.h` & `FlipperNested-1.8.3/NestedSolver/parity.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/NestedSolver/progress.c` & `FlipperNested-1.8.3/NestedSolver/progress.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/NestedSolver/python.c` & `FlipperNested-1.8.3/NestedSolver/python.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/PKG-INFO` & `FlipperNested-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.8.2
+Version: 1.8.3
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-1.8.2/README.md` & `FlipperNested-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.2/setup.py` & `FlipperNested-1.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                           libraries=libraries)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FlipperNested",
-    version="1.8.2",
+    version="1.8.3",
     author="AloneLiberty",
     description="Recover keys from collected nonces",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AloneLiberty/FlipperNestedRecovery",
     entry_points={'console_scripts': ['FlipperNested = FlipperNested.cli:main']},
     install_requires=['protobuf>4', 'pyserial'],
```

### Comparing `FlipperNested-1.8.2/tests/test_calculate.py` & `FlipperNested-1.8.3/tests/test_calculate.py`

 * *Files identical despite different names*

