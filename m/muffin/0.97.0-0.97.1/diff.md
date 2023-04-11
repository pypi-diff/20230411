# Comparing `tmp/muffin-0.97.0.tar.gz` & `tmp/muffin-0.97.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin-0.97.0.tar", max compression
+gzip compressed data, was "muffin-0.97.1.tar", max compression
```

## Comparing `muffin-0.97.0.tar` & `muffin-0.97.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     9874 2023-04-11 05:53:15.754006 muffin-0.97.0/README.rst
--rw-r--r--   0        0        0      982 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/__init__.py
--rw-r--r--   0        0        0     5130 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/app.py
--rw-r--r--   0        0        0       71 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/constants.py
--rw-r--r--   0        0        0      701 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/errors.py
--rw-r--r--   0        0        0     3754 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/handler.py
--rw-r--r--   0        0        0     8805 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/manage.py
--rw-r--r--   0        0        0     2857 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/plugins.py
--rw-r--r--   0        0        0        0 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/py.typed
--rw-r--r--   0        0        0     2705 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/pytest.py
--rw-r--r--   0        0        0      153 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/types.py
--rw-r--r--   0        0        0     2449 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/utils.py
--rw-r--r--   0        0        0     3038 2023-04-11 05:53:15.758003 muffin-0.97.0/pyproject.toml
--rw-r--r--   0        0        0    11614 1970-01-01 00:00:00.000000 muffin-0.97.0/PKG-INFO
+-rw-r--r--   0        0        0     9874 2023-04-11 07:56:38.221341 muffin-0.97.1/README.rst
+-rw-r--r--   0        0        0      982 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/__init__.py
+-rw-r--r--   0        0        0     5130 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/app.py
+-rw-r--r--   0        0        0       71 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/constants.py
+-rw-r--r--   0        0        0      701 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/errors.py
+-rw-r--r--   0        0        0     3754 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/handler.py
+-rw-r--r--   0        0        0     8805 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/manage.py
+-rw-r--r--   0        0        0     2857 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/plugins.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/py.typed
+-rw-r--r--   0        0        0     2705 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/pytest.py
+-rw-r--r--   0        0        0      153 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/types.py
+-rw-r--r--   0        0        0     2449 2023-04-11 07:56:38.225341 muffin-0.97.1/muffin/utils.py
+-rw-r--r--   0        0        0     3038 2023-04-11 07:56:38.225341 muffin-0.97.1/pyproject.toml
+-rw-r--r--   0        0        0    11614 1970-01-01 00:00:00.000000 muffin-0.97.1/PKG-INFO
```

### Comparing `muffin-0.97.0/README.rst` & `muffin-0.97.1/README.rst`

 * *Files identical despite different names*

### Comparing `muffin-0.97.0/muffin/__init__.py` & `muffin-0.97.1/muffin/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.0/muffin/app.py` & `muffin-0.97.1/muffin/app.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -71,28 +71,28 @@
 
         # Setup CLI
         from muffin.manage import Manager
 
         self.manage = Manager(self)
 
         # Setup logging
-        log_config = self.cfg.get("LOG_CONFIG")
-        if log_config and isinstance(log_config, dict) and log_config.get("version"):
-            dictConfig(log_config)
-
         self.logger = logging.getLogger("muffin")
         self.logger.setLevel(self.cfg.LOG_LEVEL)
         self.logger.propagate = False
         if not self.logger.handlers:
             ch = logging.StreamHandler()
             ch.setFormatter(
                 logging.Formatter(self.cfg.LOG_FORMAT, self.cfg.LOG_DATE_FORMAT),
             )
             self.logger.addHandler(ch)
 
+        log_config = self.cfg.get("LOG_CONFIG")
+        if log_config and isinstance(log_config, dict) and log_config.get("version"):
+            dictConfig(log_config)
+
         super().__init__(
             debug=self.cfg.DEBUG,
             logger=self.logger,
             trim_last_slash=self.cfg.TRIM_LAST_SLASH,
             static_folders=self.cfg.STATIC_FOLDERS,
             static_url_prefix=self.cfg.STATIC_URL_PREFIX,
         )
```

### Comparing `muffin-0.97.0/muffin/errors.py` & `muffin-0.97.1/muffin/errors.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.0/muffin/handler.py` & `muffin-0.97.1/muffin/handler.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.0/muffin/manage.py` & `muffin-0.97.1/muffin/manage.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.0/muffin/plugins.py` & `muffin-0.97.1/muffin/plugins.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.0/muffin/pytest.py` & `muffin-0.97.1/muffin/pytest.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.0/muffin/utils.py` & `muffin-0.97.1/muffin/utils.py`

 * *Files identical despite different names*

### Comparing `muffin-0.97.0/pyproject.toml` & `muffin-0.97.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin"
-version = "0.97.0"
+version = "0.97.1"
 description = "Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)"
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["asgi", "web", "web framework", "asyncio", "trio", "curio"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
```

### Comparing `muffin-0.97.0/PKG-INFO` & `muffin-0.97.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin
-Version: 0.97.0
+Version: 0.97.1
 Summary: Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)
 Home-page: https://github.com/klen/muffin
 License: MIT
 Keywords: asgi,web,web framework,asyncio,trio,curio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

