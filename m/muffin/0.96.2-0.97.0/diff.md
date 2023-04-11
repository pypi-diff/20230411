# Comparing `tmp/muffin-0.96.2.tar.gz` & `tmp/muffin-0.97.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin-0.96.2.tar", max compression
+gzip compressed data, was "muffin-0.97.0.tar", max compression
```

## Comparing `muffin-0.96.2.tar` & `muffin-0.97.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     9874 2023-03-30 08:56:04.514470 muffin-0.96.2/README.rst
--rw-r--r--   0        0        0      982 2023-03-30 08:56:04.518470 muffin-0.96.2/muffin/__init__.py
--rw-r--r--   0        0        0     5130 2023-03-30 08:56:04.518470 muffin-0.96.2/muffin/app.py
--rw-r--r--   0        0        0       71 2023-03-30 08:56:04.518470 muffin-0.96.2/muffin/constants.py
--rw-r--r--   0        0        0      701 2023-03-30 08:56:04.518470 muffin-0.96.2/muffin/errors.py
--rw-r--r--   0        0        0     3754 2023-03-30 08:56:04.518470 muffin-0.96.2/muffin/handler.py
--rw-r--r--   0        0        0     8805 2023-03-30 08:56:04.518470 muffin-0.96.2/muffin/manage.py
--rw-r--r--   0        0        0     2724 2023-03-30 08:56:04.518470 muffin-0.96.2/muffin/plugins.py
--rw-r--r--   0        0        0        0 2023-03-30 08:56:04.518470 muffin-0.96.2/muffin/py.typed
--rw-r--r--   0        0        0     2705 2023-03-30 08:56:04.518470 muffin-0.96.2/muffin/pytest.py
--rw-r--r--   0        0        0      153 2023-03-30 08:56:04.518470 muffin-0.96.2/muffin/types.py
--rw-r--r--   0        0        0     2449 2023-03-30 08:56:04.518470 muffin-0.96.2/muffin/utils.py
--rw-r--r--   0        0        0     3038 2023-03-30 08:56:04.518470 muffin-0.96.2/pyproject.toml
--rw-r--r--   0        0        0    11614 1970-01-01 00:00:00.000000 muffin-0.96.2/PKG-INFO
+-rw-r--r--   0        0        0     9874 2023-04-11 05:53:15.754006 muffin-0.97.0/README.rst
+-rw-r--r--   0        0        0      982 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/__init__.py
+-rw-r--r--   0        0        0     5130 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/app.py
+-rw-r--r--   0        0        0       71 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/constants.py
+-rw-r--r--   0        0        0      701 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/errors.py
+-rw-r--r--   0        0        0     3754 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/handler.py
+-rw-r--r--   0        0        0     8805 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/manage.py
+-rw-r--r--   0        0        0     2857 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/plugins.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/py.typed
+-rw-r--r--   0        0        0     2705 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/pytest.py
+-rw-r--r--   0        0        0      153 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/types.py
+-rw-r--r--   0        0        0     2449 2023-04-11 05:53:15.754006 muffin-0.97.0/muffin/utils.py
+-rw-r--r--   0        0        0     3038 2023-04-11 05:53:15.758003 muffin-0.97.0/pyproject.toml
+-rw-r--r--   0        0        0    11614 1970-01-01 00:00:00.000000 muffin-0.97.0/PKG-INFO
```

### Comparing `muffin-0.96.2/README.rst` & `muffin-0.97.0/README.rst`

 * *Files identical despite different names*

### Comparing `muffin-0.96.2/muffin/__init__.py` & `muffin-0.97.0/muffin/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin-0.96.2/muffin/app.py` & `muffin-0.97.0/muffin/app.py`

 * *Files identical despite different names*

### Comparing `muffin-0.96.2/muffin/errors.py` & `muffin-0.97.0/muffin/errors.py`

 * *Files identical despite different names*

### Comparing `muffin-0.96.2/muffin/handler.py` & `muffin-0.97.0/muffin/handler.py`

 * *Files identical despite different names*

### Comparing `muffin-0.96.2/muffin/manage.py` & `muffin-0.97.0/muffin/manage.py`

 * *Files identical despite different names*

### Comparing `muffin-0.96.2/muffin/plugins.py` & `muffin-0.97.0/muffin/plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     def __init__(self, app: Optional[Application] = None, **options):
         """Save application and create he plugin's configuration."""
         if getattr(self, "name", None) is None:
             msg = "Plugin.name is required"
             raise TypeError(msg)
 
-        self.cfg = Config(config_config={"update_from_env": False}, **self.defaults)
+        self.cfg = Config(config_config={"update_from_env": False}, disabled=False, **self.defaults)
         self.__app__ = app
 
         if app is not None:
             self.setup(app, **options)
         else:
             self.cfg.update_from_dict(options, exist_only=True)
 
@@ -70,24 +70,28 @@
 
         return self.__app__
 
     def setup(self, app: Application, *, name: Optional[str] = None, **options):
         """Bind app and update the plugin's configuration."""
         # allow to redefine the name for multi plugins with same type
         self.name = name or self.name
-        self.__app__ = app
-        app.plugins[self.name] = self
 
         # Update configuration
         self.cfg.update_from_dict(
             dict(app.cfg),
             prefix=f"{self.name}_",
             exist_only=True,
         )
         self.cfg.update_from_dict(options)
+        if self.cfg.disabled:
+            app.logger.warning("Plugin %s is disabled", self.name)
+            return
+
+        app.plugins[self.name] = self
+        self.__app__ = app
 
         # Register a middleware
         if self.middleware:
             app.middleware(to_awaitable(self.middleware))
 
         # Bind startup
         if self.startup:
```

### Comparing `muffin-0.96.2/muffin/pytest.py` & `muffin-0.97.0/muffin/pytest.py`

 * *Files identical despite different names*

### Comparing `muffin-0.96.2/muffin/utils.py` & `muffin-0.97.0/muffin/utils.py`

 * *Files identical despite different names*

### Comparing `muffin-0.96.2/pyproject.toml` & `muffin-0.97.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin"
-version = "0.96.2"
+version = "0.97.0"
 description = "Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)"
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["asgi", "web", "web framework", "asyncio", "trio", "curio"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
```

### Comparing `muffin-0.96.2/PKG-INFO` & `muffin-0.97.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin
-Version: 0.96.2
+Version: 0.97.0
 Summary: Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)
 Home-page: https://github.com/klen/muffin
 License: MIT
 Keywords: asgi,web,web framework,asyncio,trio,curio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

