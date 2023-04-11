# Comparing `tmp/muffin-0.97.1.tar.gz` & `tmp/muffin-0.97.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin-0.97.1.tar", max compression
+gzip compressed data, was "muffin-0.97.2.tar", max compression
```

## Comparing `muffin-0.97.1.tar` & `muffin-0.97.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     9874 2023-04-11 07:56:38.221341 muffin-0.97.1/README.rst
--rw-r--r--   0        0        0      982 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/__init__.py
--rw-r--r--   0        0        0     5130 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/app.py
--rw-r--r--   0        0        0       71 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/constants.py
--rw-r--r--   0        0        0      701 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/errors.py
--rw-r--r--   0        0        0     3754 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/handler.py
--rw-r--r--   0        0        0     8805 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/manage.py
--rw-r--r--   0        0        0     2857 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/plugins.py
--rw-r--r--   0        0        0        0 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/py.typed
--rw-r--r--   0        0        0     2705 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/pytest.py
--rw-r--r--   0        0        0      153 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/types.py
--rw-r--r--   0        0        0     2449 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/utils.py
--rw-r--r--   0        0        0     3038 2023-04-11 07:56:38.225341 muffin-0.97.1/pyproject.toml
--rw-r--r--   0        0        0    11614 1970-01-01 00:00:00.000000 muffin-0.97.1/PKG-INFO
+-rw-r--r--   0        0        0     9874 2023-04-11 12:30:09.537730 muffin-0.97.2/README.rst
+-rw-r--r--   0        0        0      982 2023-04-11 12:30:09.537730 muffin-0.97.2/muffin/__init__.py
+-rw-r--r--   0        0        0     5130 2023-04-11 12:30:09.537730 muffin-0.97.2/muffin/app.py
+-rw-r--r--   0        0        0       71 2023-04-11 12:30:09.537730 muffin-0.97.2/muffin/constants.py
+-rw-r--r--   0        0        0      701 2023-04-11 12:30:09.537730 muffin-0.97.2/muffin/errors.py
+-rw-r--r--   0        0        0     3754 2023-04-11 12:30:09.537730 muffin-0.97.2/muffin/handler.py
+-rw-r--r--   0        0        0     8805 2023-04-11 12:30:09.537730 muffin-0.97.2/muffin/manage.py
+-rw-r--r--   0        0        0     2857 2023-04-11 12:30:09.541730 muffin-0.97.2/muffin/plugins.py
+-rw-r--r--   0        0        0        0 2023-04-11 12:30:09.541730 muffin-0.97.2/muffin/py.typed
+-rw-r--r--   0        0        0     2705 2023-04-11 12:30:09.541730 muffin-0.97.2/muffin/pytest.py
+-rw-r--r--   0        0        0      153 2023-04-11 12:30:09.541730 muffin-0.97.2/muffin/types.py
+-rw-r--r--   0        0        0     2449 2023-04-11 12:30:09.541730 muffin-0.97.2/muffin/utils.py
+-rw-r--r--   0        0        0     3038 2023-04-11 12:30:09.541730 muffin-0.97.2/pyproject.toml
+-rw-r--r--   0        0        0    11614 1970-01-01 00:00:00.000000 muffin-0.97.2/PKG-INFO
```

### Comparing `muffin-0.97.1/README.rst` & `muffin-0.97.2/README.rst`

 * *Files identical despite different names*

### Comparing `muffin-0.97.1/muffin/__init__.py` & `muffin-0.97.2/muffin/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.1/muffin/app.py` & `muffin-0.97.2/muffin/app.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.1/muffin/errors.py` & `muffin-0.97.2/muffin/errors.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.1/muffin/handler.py` & `muffin-0.97.2/muffin/handler.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.1/muffin/manage.py` & `muffin-0.97.2/muffin/manage.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.1/muffin/plugins.py` & `muffin-0.97.2/muffin/plugins.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.1/muffin/pytest.py` & `muffin-0.97.2/muffin/pytest.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.1/muffin/utils.py` & `muffin-0.97.2/muffin/utils.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.1/pyproject.toml` & `muffin-0.97.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin"
-version = "0.97.1"
+version = "0.97.2"
 description = "Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)"
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["asgi", "web", "web framework", "asyncio", "trio", "curio"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
```

### Comparing `muffin-0.97.1/PKG-INFO` & `muffin-0.97.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin
-Version: 0.97.1
+Version: 0.97.2
 Summary: Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)
 Home-page: https://github.com/klen/muffin
 License: MIT
 Keywords: asgi,web,web framework,asyncio,trio,curio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

