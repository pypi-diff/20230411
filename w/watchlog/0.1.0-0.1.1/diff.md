# Comparing `tmp/watchlog-0.1.0.tar.gz` & `tmp/watchlog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchlog-0.1.0.tar", max compression
+gzip compressed data, was "watchlog-0.1.1.tar", max compression
```

## Comparing `watchlog-0.1.0.tar` & `watchlog-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rwxr-xr-x   0        0        0     2328 2023-04-11 05:51:59.149720 watchlog-0.1.0/README.md
--rwxr-xr-x   0        0        0      637 2023-04-11 05:55:10.452471 watchlog-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-04-11 05:12:32.140833 watchlog-0.1.0/watchlog/__init__.py
--rwxr-xr-x   0        0        0     5046 2023-04-11 05:50:31.458099 watchlog-0.1.0/watchlog/watchlog.py
--rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 watchlog-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1086 2023-04-11 06:24:22.861180 watchlog-0.1.1/LICENSE
+-rwxr-xr-x   0        0        0     2328 2023-04-11 05:51:59.149720 watchlog-0.1.1/README.md
+-rwxr-xr-x   0        0        0      638 2023-04-11 06:27:29.054519 watchlog-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-04-11 05:12:32.140833 watchlog-0.1.1/watchlog/__init__.py
+-rwxr-xr-x   0        0        0     5140 2023-04-11 06:26:49.304008 watchlog-0.1.1/watchlog/watchlog.py
+-rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 watchlog-0.1.1/PKG-INFO
```

### Comparing `watchlog-0.1.0/README.md` & `watchlog-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `watchlog-0.1.0/pyproject.toml` & `watchlog-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "watchlog"
-version = "0.1.0"
+version = "0.1.1"
 description = "monitoring log files and sending parsed logs to a specified URL"
 authors = ["euraxluo <euraxluo@outlook.com>"]
 license = "The MIT LICENSE"
 readme = "README.md"
 homepage = "https://github.com/Euraxluo/watchlog"
 repository = "https://github.com/Euraxluo/watchlog"
 keywords = ["log monitor","loguru","watchdog"]
@@ -19,8 +19,8 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry.scripts]
-watchlog = 'watchlog.watchlog:cli'
+watchlog = 'watchlog.watchlog:cli'
```

### Comparing `watchlog-0.1.0/watchlog/watchlog.py` & `watchlog-0.1.1/watchlog/watchlog.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,11 +148,14 @@
         observer.stop()
     observer.join()
 
 
 def cli():
     import sys
     loop = asyncio.get_event_loop()
+    if len(sys.argv)!=2:
+        print("Useage: watchlog path/to/config.json")
+        return
     loop.run_until_complete(start(sys.argv[1]))
 
 
 __all__ = ["start", "cli"]
```

### Comparing `watchlog-0.1.0/PKG-INFO` & `watchlog-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchlog
-Version: 0.1.0
+Version: 0.1.1
 Summary: monitoring log files and sending parsed logs to a specified URL
 Home-page: https://github.com/Euraxluo/watchlog
 License: The MIT LICENSE
 Keywords: log monitor,loguru,watchdog
 Author: euraxluo
 Author-email: euraxluo@outlook.com
 Requires-Python: >=3.8,<4.0
```

