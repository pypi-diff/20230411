# Comparing `tmp/muffin_grpc-0.5.4.tar.gz` & `tmp/muffin_grpc-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_grpc-0.5.4.tar", max compression
+gzip compressed data, was "muffin_grpc-0.5.5.tar", max compression
```

## Comparing `muffin_grpc-0.5.4.tar` & `muffin_grpc-0.5.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6014 2023-04-11 06:22:43.246803 muffin_grpc-0.5.4/README.rst
--rw-r--r--   0        0        0     6947 2023-04-11 06:22:43.246803 muffin_grpc-0.5.4/muffin_grpc/__init__.py
--rw-r--r--   0        0        0    11986 2023-04-11 06:22:43.246803 muffin_grpc-0.5.4/muffin_grpc/proto3.py
--rw-r--r--   0        0        0        0 2023-04-11 06:22:43.246803 muffin_grpc-0.5.4/muffin_grpc/py.typed
--rw-r--r--   0        0        0     1420 2023-04-11 06:22:43.246803 muffin_grpc-0.5.4/muffin_grpc/utils.py
--rw-r--r--   0        0        0     1969 2023-04-11 06:22:43.246803 muffin_grpc-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     7262 1970-01-01 00:00:00.000000 muffin_grpc-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     6014 2023-04-11 06:24:08.703393 muffin_grpc-0.5.5/README.rst
+-rw-r--r--   0        0        0     6947 2023-04-11 06:24:08.707393 muffin_grpc-0.5.5/muffin_grpc/__init__.py
+-rw-r--r--   0        0        0    11986 2023-04-11 06:24:08.707393 muffin_grpc-0.5.5/muffin_grpc/proto3.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:24:08.707393 muffin_grpc-0.5.5/muffin_grpc/py.typed
+-rw-r--r--   0        0        0     1420 2023-04-11 06:24:08.707393 muffin_grpc-0.5.5/muffin_grpc/utils.py
+-rw-r--r--   0        0        0     1969 2023-04-11 06:24:08.707393 muffin_grpc-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     7262 1970-01-01 00:00:00.000000 muffin_grpc-0.5.5/PKG-INFO
```

### Comparing `muffin_grpc-0.5.4/README.rst` & `muffin_grpc-0.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_grpc-0.5.4/muffin_grpc/__init__.py` & `muffin_grpc-0.5.5/muffin_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_grpc-0.5.4/muffin_grpc/proto3.py` & `muffin_grpc-0.5.5/muffin_grpc/proto3.py`

 * *Files identical despite different names*

### Comparing `muffin_grpc-0.5.4/muffin_grpc/utils.py` & `muffin_grpc-0.5.5/muffin_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_grpc-0.5.4/pyproject.toml` & `muffin_grpc-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-grpc"
-version = "0.5.4"
+version = "0.5.5"
 description = "GRPC support for Muffin framework."
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-grpc"
 repository = "https://github.com/klen/muffin-grpc"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["grpc", "muffin", "asyncio", "asgi", "web"]
```

### Comparing `muffin_grpc-0.5.4/PKG-INFO` & `muffin_grpc-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-grpc
-Version: 0.5.4
+Version: 0.5.5
 Summary: GRPC support for Muffin framework.
 Home-page: https://github.com/klen/muffin-grpc
 License: MIT
 Keywords: grpc,muffin,asyncio,asgi,web
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

