# Comparing `tmp/pytest-embedded-1.2.4.tar.gz` & `tmp/pytest-embedded-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-1.2.4.tar", last modified: Fri Mar 10 07:12:29 2023, max compression
+gzip compressed data, was "dist/pytest-embedded-1.2.5.tar", last modified: Tue Apr 11 05:40:50 2023, max compression
```

## Comparing `pytest-embedded-1.2.4.tar` & `pytest-embedded-1.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 07:12:29.000000 pytest-embedded-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-10 07:12:29.000000 pytest-embedded-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-10 07:12:19.000000 pytest-embedded-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 07:12:29.000000 pytest-embedded-1.2.4/pytest_embedded/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-10 07:12:19.000000 pytest-embedded-1.2.4/pytest_embedded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-10 07:12:19.000000 pytest-embedded-1.2.4/pytest_embedded/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-03-10 07:12:19.000000 pytest-embedded-1.2.4/pytest_embedded/dut.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-03-10 07:12:19.000000 pytest-embedded-1.2.4/pytest_embedded/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    49307 2023-03-10 07:12:19.000000 pytest-embedded-1.2.4/pytest_embedded/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-03-10 07:12:19.000000 pytest-embedded-1.2.4/pytest_embedded/unity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-03-10 07:12:19.000000 pytest-embedded-1.2.4/pytest_embedded/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 07:12:29.000000 pytest-embedded-1.2.4/pytest_embedded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-10 07:12:28.000000 pytest-embedded-1.2.4/pytest_embedded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-10 07:12:28.000000 pytest-embedded-1.2.4/pytest_embedded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 07:12:28.000000 pytest-embedded-1.2.4/pytest_embedded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-10 07:12:28.000000 pytest-embedded-1.2.4/pytest_embedded.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-10 07:12:28.000000 pytest-embedded-1.2.4/pytest_embedded.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-10 07:12:28.000000 pytest-embedded-1.2.4/pytest_embedded.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 07:12:29.000000 pytest-embedded-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-10 07:12:19.000000 pytest-embedded-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/pytest_embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/pytest_embedded/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/pytest_embedded/dut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/pytest_embedded/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49307 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/pytest_embedded/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/pytest_embedded/unity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/pytest_embedded/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/pytest_embedded.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 05:40:50.000000 pytest-embedded-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-11 05:40:39.000000 pytest-embedded-1.2.5/setup.py
```

### Comparing `pytest-embedded-1.2.4/PKG-INFO` & `pytest-embedded-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pytest-embedded
-Version: 1.2.4
+Version: 1.2.5
 Summary: pytest embedded plugin
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded
```

### Comparing `pytest-embedded-1.2.4/pytest_embedded/app.py` & `pytest-embedded-1.2.5/pytest_embedded/app.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-1.2.4/pytest_embedded/dut.py` & `pytest-embedded-1.2.5/pytest_embedded/dut.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-1.2.4/pytest_embedded/log.py` & `pytest-embedded-1.2.5/pytest_embedded/log.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-1.2.4/pytest_embedded/plugin.py` & `pytest-embedded-1.2.5/pytest_embedded/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-1.2.4/pytest_embedded/unity.py` & `pytest-embedded-1.2.5/pytest_embedded/unity.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,17 @@
     (0xBFFFE, 0xBFFFF),
     (0xCFFFE, 0xCFFFF),
     (0xDFFFE, 0xDFFFF),
     (0xEFFFE, 0xEFFFF),
     (0xFFFFE, 0xFFFFF),
     (0x10FFFE, 0x10FFFF),
 ]
-ILLEGAL_XML_CHAR_REGEX = re.compile(f"[{''.join([f'{chr(l)}-{chr(r)}' for l, r in _avoid_compatibility_chars])}]")
+ILLEGAL_XML_CHAR_REGEX = re.compile(
+    f"[{''.join([f'{chr(lower)}-{chr(upper)}' for lower, upper in _avoid_compatibility_chars])}]"
+)
 
 
 def escape_illegal_xml_chars(s: str) -> str:
     return ILLEGAL_XML_CHAR_REGEX.sub('', s)
 
 
 def escape_dict_value(d: Dict[str, Any]) -> Dict[str, str]:
```

### Comparing `pytest-embedded-1.2.4/pytest_embedded/utils.py` & `pytest-embedded-1.2.5/pytest_embedded/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import dataclasses
+import importlib
 import logging
 import os
 import re
 import typing as t
 
-from . import App
+if t.TYPE_CHECKING:
+    from . import App
 
 #############
 # Constants #
 #############
 BASE_LIB_NAME = 'pytest-embedded'
 
 SERVICE_LIB_NAMES = {
@@ -172,24 +174,74 @@
     def drop_port_target_cache(self, port: str) -> None:
         try:
             self.port_target_cache.pop(port)
             logging.debug('drop port-target cache with port %s', port)
         except KeyError:
             logging.warning('no port-target cache with port %s', port)
 
-    def hit_port_app_cache(self, port: str, app: App) -> bool:
+    def hit_port_app_cache(self, port: str, app: 'App') -> bool:
         if self.port_app_cache.get(port, None) == app.binary_path:
             logging.debug('hit port-app cache: %s - %s', port, app.binary_path)
             return True
 
         return False
 
-    def set_port_app_cache(self, port: str, app: App) -> None:
+    def set_port_app_cache(self, port: str, app: 'App') -> None:
         self.port_app_cache[port] = app.binary_path
         logging.debug('set port-app cache: %s - %s', port, app.binary_path)
 
     def drop_port_app_cache(self, port: str) -> None:
         try:
             self.port_app_cache.pop(port)
             logging.debug('drop port-app cache with port %s', port)
         except KeyError:
             logging.warning('no port-app cache with port %s', port)
+
+
+_ModuleType = type(importlib)
+
+
+def lazy_load(
+    base_module: _ModuleType, name_obj_dict: t.Dict[str, t.Any], obj_module_dict: t.Dict[str, str]
+) -> t.Callable[[str], t.Any]:
+    """
+    use __getattr__ in the __init__.py file to lazy load some objects
+
+    Args:
+        base_module (ModuleType): base package module
+        name_obj_dict (dict[str, any]): name, real object dict, used to store real objects,
+            no need to add lazy-load objects
+        obj_module_dict (dict[str, str]): dict of object name and module name
+
+    Returns:
+        __getattr__ function
+
+    Examples:
+        ```python
+        __getattr__ = lazy_load(
+            importlib.import_module(__name__),
+            {
+                'IdfApp': IdfApp,
+                'LinuxDut': LinuxDut,
+                'LinuxSerial': LinuxSerial,
+                'CaseTester': CaseTester,
+            },
+            {
+                'IdfSerial': '.serial',
+                'IdfDut': '.dut',
+            },
+        )
+        ```
+    """
+
+    def __getattr__(object_name):
+        if object_name in name_obj_dict:
+            return name_obj_dict[object_name]
+        elif object_name in obj_module_dict:
+            module = importlib.import_module(obj_module_dict[object_name], base_module.__name__)
+            imported = getattr(module, object_name)
+            name_obj_dict[object_name] = imported
+            return imported
+        else:
+            raise AttributeError('Attribute %s not found in module %s', object_name, base_module.__name__)
+
+    return __getattr__
```

### Comparing `pytest-embedded-1.2.4/pytest_embedded.egg-info/PKG-INFO` & `pytest-embedded-1.2.5/pytest_embedded.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pytest-embedded
-Version: 1.2.4
+Version: 1.2.5
 Summary: pytest embedded plugin
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded
```

### Comparing `pytest-embedded-1.2.4/setup.py` & `pytest-embedded-1.2.5/setup.py`

 * *Files identical despite different names*

