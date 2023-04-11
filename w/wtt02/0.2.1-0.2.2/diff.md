# Comparing `tmp/wtt02-0.2.1.tar.gz` & `tmp/wtt02-0.2.2.tar.gz`

## Comparing `wtt02-0.2.1.tar` & `wtt02-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt02-0.2.1/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt02-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 wtt02-0.2.1/tests/test_load.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 wtt02-0.2.1/wtt02/__about__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt02-0.2.1/wtt02/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt02-0.2.1/wtt02/_env.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 wtt02-0.2.1/wtt02/main.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wtt02-0.2.1/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt02-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt02-0.2.1/README.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 wtt02-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 wtt02-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt02-0.2.2/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt02-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 wtt02-0.2.2/tests/test_load.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 wtt02-0.2.2/wtt02/__about__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt02-0.2.2/wtt02/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt02-0.2.2/wtt02/_env.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 wtt02-0.2.2/wtt02/main.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wtt02-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt02-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt02-0.2.2/README.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 wtt02-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 wtt02-0.2.2/PKG-INFO
```

### Comparing `wtt02-0.2.1/tests/test_load.py` & `wtt02-0.2.2/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `wtt02-0.2.1/wtt02/main.py` & `wtt02-0.2.2/wtt02/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """Package for wtt02."""
 
 from pathlib import Path
 from typing import Optional, Union
 import os
+import logging
 
 import platform
 import zipfile
 import tempfile
 
 import urllib.request
 
 import duckdb
 
 from wtt02.__about__ import __version__, EXTENSION_NAME
 
 
 __all__ = ["get_connection", "run_query_file", "__version__"]
 
+logger = logging.getLogger(__name__)
+
 
 class WTTException(Exception):
     """Base exception for wtt02."""
 
 
 class WTT02ConfigurationException(WTTException):
     """Exception for wtt02 configuration."""
@@ -61,26 +64,30 @@
         config=config,
     )
 
     try:
         con.load_extension(EXTENSION_NAME)
         return con
     except duckdb.IOException:
-        if extension_path := os.environ.get("WTT02_EXTENSION_PATH"):
+        logger.info("Extension not found, installing. This only happens once per version/matchine.")
+        extension_path = os.getenv("WTT02_EXTENSION_PATH")
+
+        if extension_path:
             extension_path = Path(extension_path).absolute()
             con.install_extension(str(extension_path), force_install=True)
             con.load_extension(EXTENSION_NAME)
 
         elif file_path is not None and file_path.exists():
             con.install_extension(str(file_path.absolute()), force_install=True)
             con.load_extension(EXTENSION_NAME)
 
         elif s3_uri is not None:
             # download
             pass
+
         else:
             platform_uname = platform.uname()
             operating_system = platform_uname.system
             architecture = platform_uname.machine
             version = __version__
 
             from wtt02._env import ENVIRONMENT
@@ -88,14 +95,15 @@
             name = "wtt02"
             bucket = f"wtt-02-dist-{ENVIRONMENT}"
             filename = f"{name}-{version}-{operating_system}-{architecture}.zip"
 
             full_s3_path = (
                 f"http://{bucket}.s3.amazonaws.com/extension/{name}/{filename}"
             )
+            logger.info("Downloading extension from %s", full_s3_path)
 
             with tempfile.TemporaryDirectory() as temp_dir:
                 temp_dir_path = Path(temp_dir)
                 temp_file_name = temp_dir_path / filename
 
                 try:
                     urllib.request.urlretrieve(full_s3_path, temp_file_name)
@@ -109,12 +117,13 @@
 
                 output_file = temp_dir_path / f"{name}.duckdb_extension"
                 if not output_file.exists():
                     raise WTTException(
                         f"Unable to find extension file at {output_file}"
                     )
 
+                logging.info("Installing extension from %s", output_file)
                 con.install_extension(output_file.as_posix(), force_install=True)
 
                 con.load_extension(EXTENSION_NAME)
 
     return con
```

### Comparing `wtt02-0.2.1/LICENSE.txt` & `wtt02-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wtt02-0.2.1/pyproject.toml` & `wtt02-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wtt02-0.2.1/PKG-INFO` & `wtt02-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtt02
-Version: 0.2.1
+Version: 0.2.2
 Author-email: Trent Hauck <thauck@wheretrue.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

