# Comparing `tmp/python_roborock-0.6.1.tar.gz` & `tmp/python_roborock-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.6.1.tar", max compression
+gzip compressed data, was "python_roborock-0.6.2.tar", max compression
```

## Comparing `python_roborock-0.6.1.tar` & `python_roborock-0.6.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-04-10 15:47:18.924247 python_roborock-0.6.1/LICENSE
--rw-r--r--   0        0        0     2221 2023-04-10 15:47:18.924247 python_roborock-0.6.1/README.md
--rw-r--r--   0        0        0     1204 2023-04-10 15:47:19.792261 python_roborock-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      300 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/__init__.py
--rw-r--r--   0        0        0    17099 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/api.py
--rw-r--r--   0        0        0     3957 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/cli.py
--rw-r--r--   0        0        0     8276 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/cloud_api.py
--rw-r--r--   0        0        0     3704 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/code_mappings.py
--rw-r--r--   0        0        0     9190 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/containers.py
--rw-r--r--   0        0        0     1022 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/exceptions.py
--rw-r--r--   0        0        0     7030 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/local_api.py
--rw-r--r--   0        0        0     1194 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/offline/offline.py
--rw-r--r--   0        0        0     6030 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/roborock_message.py
--rw-r--r--   0        0        0      644 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/roborock_queue.py
--rw-r--r--   0        0        0    12709 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/typing.py
--rw-r--r--   0        0        0      809 2023-04-10 15:47:18.924247 python_roborock-0.6.1/roborock/util.py
--rw-r--r--   0        0        0     3348 1970-01-01 00:00:00.000000 python_roborock-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 16:10:53.394092 python_roborock-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2221 2023-04-11 16:10:53.394092 python_roborock-0.6.2/README.md
+-rw-r--r--   0        0        0     1204 2023-04-11 16:10:54.490124 python_roborock-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-11 16:10:53.394092 python_roborock-0.6.2/roborock/__init__.py
+-rw-r--r--   0        0        0    17099 2023-04-11 16:10:53.394092 python_roborock-0.6.2/roborock/api.py
+-rw-r--r--   0        0        0     3957 2023-04-11 16:10:53.394092 python_roborock-0.6.2/roborock/cli.py
+-rw-r--r--   0        0        0     8276 2023-04-11 16:10:53.394092 python_roborock-0.6.2/roborock/cloud_api.py
+-rw-r--r--   0        0        0     3703 2023-04-11 16:10:53.394092 python_roborock-0.6.2/roborock/code_mappings.py
+-rw-r--r--   0        0        0     9190 2023-04-11 16:10:53.394092 python_roborock-0.6.2/roborock/containers.py
+-rw-r--r--   0        0        0     1022 2023-04-11 16:10:53.394092 python_roborock-0.6.2/roborock/exceptions.py
+-rw-r--r--   0        0        0     7030 2023-04-11 16:10:53.394092 python_roborock-0.6.2/roborock/local_api.py
+-rw-r--r--   0        0        0     1194 2023-04-11 16:10:53.394092 python_roborock-0.6.2/roborock/offline/offline.py
+-rw-r--r--   0        0        0     6030 2023-04-11 16:10:53.394092 python_roborock-0.6.2/roborock/roborock_message.py
+-rw-r--r--   0        0        0      644 2023-04-11 16:10:53.394092 python_roborock-0.6.2/roborock/roborock_queue.py
+-rw-r--r--   0        0        0    12709 2023-04-11 16:10:53.394092 python_roborock-0.6.2/roborock/typing.py
+-rw-r--r--   0        0        0      809 2023-04-11 16:10:53.394092 python_roborock-0.6.2/roborock/util.py
+-rw-r--r--   0        0        0     3348 1970-01-01 00:00:00.000000 python_roborock-0.6.2/PKG-INFO
```

### Comparing `python_roborock-0.6.1/LICENSE` & `python_roborock-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.1/README.md` & `python_roborock-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.1/pyproject.toml` & `python_roborock-0.6.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.6.1"
+version = "0.6.2"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `python_roborock-0.6.1/roborock/api.py` & `python_roborock-0.6.2/roborock/api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.1/roborock/cli.py` & `python_roborock-0.6.2/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.1/roborock/cloud_api.py` & `python_roborock-0.6.2/roborock/cloud_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.1/roborock/code_mappings.py` & `python_roborock-0.6.2/roborock/code_mappings.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         15: "wall_sensor_dirty",
         16: "robot_tilted",
         17: "side_brush_error",
         18: "fan_error",
         21: "vertical_bumper_pressed",
         22: "dock_locator_error",
         23: "return_to_dock_fail",
-        24: "no-go_zone_detected",
+        24: "nogo_zone_detected",
         27: "vibrarise_jammed",
         28: "robot_on_carpet",
         29: "filter_blocked",
         30: "invisible_wall_detected",
         31: "cannot_cross_carpet",
         32: "internal_error",
     },
```

### Comparing `python_roborock-0.6.1/roborock/containers.py` & `python_roborock-0.6.2/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.1/roborock/exceptions.py` & `python_roborock-0.6.2/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.1/roborock/local_api.py` & `python_roborock-0.6.2/roborock/local_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.1/roborock/offline/offline.py` & `python_roborock-0.6.2/roborock/offline/offline.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.1/roborock/roborock_message.py` & `python_roborock-0.6.2/roborock/roborock_message.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.1/roborock/roborock_queue.py` & `python_roborock-0.6.2/roborock/roborock_queue.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.1/roborock/typing.py` & `python_roborock-0.6.2/roborock/typing.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.1/roborock/util.py` & `python_roborock-0.6.2/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.1/PKG-INFO` & `python_roborock-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.6.1
+Version: 0.6.2
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 0.6.1 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 0.6.2 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
 humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

