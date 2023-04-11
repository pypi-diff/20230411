# Comparing `tmp/loadconf-0.0.7.tar.gz` & `tmp/loadconf-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loadconf-0.0.7.tar", last modified: Thu Sep 22 06:01:22 2022, max compression
+gzip compressed data, was "loadconf-0.0.8.tar", last modified: Tue Apr 11 21:40:25 2023, max compression
```

## Comparing `loadconf-0.0.7.tar` & `loadconf-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2022-09-22 06:01:22.178653 loadconf-0.0.7/
--rw-r--r--   0 anon      (1000) wheel      (998)    34968 2022-09-15 21:42:18.000000 loadconf-0.0.7/LICENSE.md
--rw-r--r--   0 anon      (1000) wheel      (998)     4476 2022-09-22 06:01:22.178653 loadconf-0.0.7/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)     4125 2022-09-21 23:25:15.000000 loadconf-0.0.7/README.md
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2022-09-22 06:01:22.175320 loadconf-0.0.7/loadconf/
--rw-r--r--   0 anon      (1000) wheel      (998)       76 2022-09-15 21:33:19.000000 loadconf-0.0.7/loadconf/__init__.py
--rw-r--r--   0 anon      (1000) wheel      (998)     6966 2022-09-22 06:00:15.000000 loadconf-0.0.7/loadconf/loadconf.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2022-09-22 06:01:22.175320 loadconf-0.0.7/loadconf.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)     4476 2022-09-22 06:01:22.000000 loadconf-0.0.7/loadconf.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      205 2022-09-22 06:01:22.000000 loadconf-0.0.7/loadconf.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2022-09-22 06:01:22.000000 loadconf-0.0.7/loadconf.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        9 2022-09-22 06:01:22.000000 loadconf-0.0.7/loadconf.egg-info/top_level.txt
--rw-r--r--   0 anon      (1000) wheel      (998)      498 2022-09-22 06:01:07.000000 loadconf-0.0.7/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2022-09-22 06:01:22.178653 loadconf-0.0.7/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-11 21:40:25.866423 loadconf-0.0.8/
+-rw-r--r--   0 anon      (1000) wheel      (998)    34968 2022-09-15 21:42:18.000000 loadconf-0.0.8/LICENSE.md
+-rw-r--r--   0 anon      (1000) wheel      (998)     4476 2023-04-11 21:40:25.866423 loadconf-0.0.8/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)     4125 2022-09-21 23:25:15.000000 loadconf-0.0.8/README.md
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-11 21:40:25.866423 loadconf-0.0.8/loadconf/
+-rw-r--r--   0 anon      (1000) wheel      (998)       76 2022-09-15 21:33:19.000000 loadconf-0.0.8/loadconf/__init__.py
+-rw-r--r--   0 anon      (1000) wheel      (998)     9242 2023-04-11 21:36:04.000000 loadconf-0.0.8/loadconf/loadconf.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-11 21:40:25.866423 loadconf-0.0.8/loadconf.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)     4476 2023-04-11 21:40:25.000000 loadconf-0.0.8/loadconf.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      205 2023-04-11 21:40:25.000000 loadconf-0.0.8/loadconf.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-11 21:40:25.000000 loadconf-0.0.8/loadconf.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        9 2023-04-11 21:40:25.000000 loadconf-0.0.8/loadconf.egg-info/top_level.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)      498 2023-04-11 21:35:35.000000 loadconf-0.0.8/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-11 21:40:25.866423 loadconf-0.0.8/setup.cfg
```

### Comparing `loadconf-0.0.7/LICENSE.md` & `loadconf-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `loadconf-0.0.7/PKG-INFO` & `loadconf-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadconf
-Version: 0.0.7
+Version: 0.0.8
 Summary: Give users an easy way to define settings and personalize their use of your program.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/loadconf
 Keywords: shell,scripting
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `loadconf-0.0.7/README.md` & `loadconf-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `loadconf-0.0.7/loadconf/loadconf.py` & `loadconf-0.0.8/loadconf/loadconf.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,20 +16,18 @@
 
 import csv
 import json
 import os
 import pathlib
 import re
 import sys
-from argparse import ArgumentParser
 from typing import Optional, Iterable, List, Dict
 
 
 class Config:
-
     def __init__(
         self,
         program: str,
     ):
         self._program = program
         platform = sys.platform
         linux = ["linux", "linux2"]
@@ -38,37 +36,67 @@
         elif platform == "darwin":
             self._platform = "macos"
         else:
             self._platform = "windows"
         self.config_dir = None
         self.files = {}
         self.settings = {}
+        self.settings_files = {}
         self.stored = {}
+        self.created = {}
+
+    def associate_settings(
+        self,
+        settings: List,
+        file: str,
+    ):
+        if file in self.files.keys():
+            self.settings_files[file] = {}
+        for key, value in self.settings.items():
+            if key in settings:
+                self.settings_files[file][key] = value
 
     def create_files(
         self,
         create_files: List,
     ):
         """
         Test if config files exist and create them if needed.
         """
         if self.config_dir is not None:
             dir = pathlib.Path(self.config_dir)
-            if not dir.is_dir():
+            if not dir.is_dir() and not dir.is_file():
                 dir.mkdir(parents=True, exist_ok=True)
-        files = []
+            elif dir.is_file():
+                raise ValueError(f"ERROR: loadconf: config_dir is a file: {dir}")
+        files = {}
         for file in create_files:
             if file in self.files.keys():
-                files.append(self.files[file])
+                files[file] = self.files[file]
             elif os.path.isabs(file):
-                files.append(file)
-        for file in files:
-            f = pathlib.Path(file)
+                files[file] = file
+        for key, value in files.items():
+            f = pathlib.Path(value)
             if not f.is_file():
                 f.touch()
+                self.created[key] = f
+
+    def create_template(
+        self,
+        files: List,
+    ):
+        for key, value in self.settings_files.items():
+            # If not one of the given files, or a created file skip
+            if key not in files or key not in self.created.keys():
+                continue
+            file_path = self.created[key]
+            data = ""
+            for k, v in value.items():
+                data += f"{k} = {v}\n"
+            file_path.write_text(data)
 
     def define_files(
         self,
         user_files: Dict,
         config_dir: Optional[str] = None,
     ):
         """
@@ -95,16 +123,20 @@
     def define_settings(
         self,
         settings: Dict,
     ):
         """
         Users may not provide all settings that are relevant to your program.
         If you want to set some defaults, this makes it easy.
+        Acceptable settings values include str, bool, int, and float.
+        Other values will be ignored.
         """
         for key, value in settings.items():
+            if not isinstance(value, (str, bool, int, float)):
+                continue
             self.settings[key] = value
 
     def read_conf(
         self,
         user_settings: List,
         read_files: List,
         delimiter: str = "=",
@@ -112,15 +144,15 @@
     ):
         """
         Read a config file
         """
         files = []
         # File may be an actual file or a key value from defined_files
         for file in read_files:
-            if self.files:
+            if file in self.files.keys():
                 files.append(self.files[file])
             elif os.path.isfile(file):
                 files.append(file)
         # Regex object for subbing delimiter
         r = re.compile(rf"\\{delimiter}")
         # Read the desired files
         for file in files:
@@ -184,18 +216,49 @@
         for key, file in read_dict.items():
             if not os.path.isfile(file):
                 continue
             if not key in read_files:
                 continue
             if json_file:
                 try:
-                    with open(file, 'r') as data:
+                    with open(file, "r") as data:
                         jdata = json.load(data)
                 except json.decoder.JSONDecodeError:
                     jdata = {}
                 temp_dict[key] = jdata
             else:
                 with open(file) as f:
                     temp_dict[key] = []
                     for line in f:
                         temp_dict[key].append(line.rstrip())
         self.stored.update(temp_dict)
+
+
+if __name__ == "__main__":
+    # Create user object to read files and get settings
+    user = Config(program="test_program")
+    # Define some basic settings, files, etc.
+    user_settings = {
+        "test_bool": False,
+        "test_str": "Some string",
+        "test_int": 1,
+    }
+    config_files = {
+        "test_rc": "test_programrc",
+        "test_store": "test_program_store",
+    }
+    files = list(config_files.keys())
+    settings = list(user_settings.keys())
+    # Fill out user object
+    user.define_settings(settings=user_settings)
+    user.define_files(user_files=config_files)
+    user.associate_settings(settings, "test_rc")
+    user.create_files(create_files=files)
+    user.create_template(["test_rc"])
+    user.read_conf(user_settings=settings, read_files=["test_rc"])
+    user.store_files(files=["test_store"])
+    print(f"config_dir {user.config_dir}")
+    print(f"files: {user.files}")
+    print(f"settings: {user.settings}")
+    print(f"settings_files: {user.settings_files}")
+    print(f"stored: {user.stored}")
+    print(f"created: {user.created}")
```

### Comparing `loadconf-0.0.7/loadconf.egg-info/PKG-INFO` & `loadconf-0.0.8/loadconf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadconf
-Version: 0.0.7
+Version: 0.0.8
 Summary: Give users an easy way to define settings and personalize their use of your program.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/loadconf
 Keywords: shell,scripting
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

