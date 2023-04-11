# Comparing `tmp/python_roborock-0.6.3.tar.gz` & `tmp/python_roborock-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.6.3.tar", max compression
+gzip compressed data, was "python_roborock-0.6.4.tar", max compression
```

## Comparing `python_roborock-0.6.3.tar` & `python_roborock-0.6.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-04-11 16:20:51.307845 python_roborock-0.6.3/LICENSE
--rw-r--r--   0        0        0     2221 2023-04-11 16:20:51.307845 python_roborock-0.6.3/README.md
--rw-r--r--   0        0        0     1152 2023-04-11 16:20:52.031854 python_roborock-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      300 2023-04-11 16:20:51.307845 python_roborock-0.6.3/roborock/__init__.py
--rw-r--r--   0        0        0    17099 2023-04-11 16:20:51.311845 python_roborock-0.6.3/roborock/api.py
--rw-r--r--   0        0        0     3957 2023-04-11 16:20:51.311845 python_roborock-0.6.3/roborock/cli.py
--rw-r--r--   0        0        0     8276 2023-04-11 16:20:51.311845 python_roborock-0.6.3/roborock/cloud_api.py
--rw-r--r--   0        0        0     3703 2023-04-11 16:20:51.311845 python_roborock-0.6.3/roborock/code_mappings.py
--rw-r--r--   0        0        0     9190 2023-04-11 16:20:51.311845 python_roborock-0.6.3/roborock/containers.py
--rw-r--r--   0        0        0     1022 2023-04-11 16:20:51.311845 python_roborock-0.6.3/roborock/exceptions.py
--rw-r--r--   0        0        0     7030 2023-04-11 16:20:51.311845 python_roborock-0.6.3/roborock/local_api.py
--rw-r--r--   0        0        0     1194 2023-04-11 16:20:51.311845 python_roborock-0.6.3/roborock/offline/offline.py
--rw-r--r--   0        0        0     6030 2023-04-11 16:20:51.311845 python_roborock-0.6.3/roborock/roborock_message.py
--rw-r--r--   0        0        0      644 2023-04-11 16:20:51.311845 python_roborock-0.6.3/roborock/roborock_queue.py
--rw-r--r--   0        0        0    12709 2023-04-11 16:20:51.311845 python_roborock-0.6.3/roborock/typing.py
--rw-r--r--   0        0        0      809 2023-04-11 16:20:51.311845 python_roborock-0.6.3/roborock/util.py
--rw-r--r--   0        0        0     3348 1970-01-01 00:00:00.000000 python_roborock-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 16:29:11.922855 python_roborock-0.6.4/LICENSE
+-rw-r--r--   0        0        0     2221 2023-04-11 16:29:11.922855 python_roborock-0.6.4/README.md
+-rw-r--r--   0        0        0     1152 2023-04-11 16:29:12.738876 python_roborock-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/__init__.py
+-rw-r--r--   0        0        0    17099 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/api.py
+-rw-r--r--   0        0        0     3957 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/cli.py
+-rw-r--r--   0        0        0     8276 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/cloud_api.py
+-rw-r--r--   0        0        0     3703 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/code_mappings.py
+-rw-r--r--   0        0        0     9190 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/containers.py
+-rw-r--r--   0        0        0     1022 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/exceptions.py
+-rw-r--r--   0        0        0     7066 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/local_api.py
+-rw-r--r--   0        0        0     1194 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/offline/offline.py
+-rw-r--r--   0        0        0     6030 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/roborock_message.py
+-rw-r--r--   0        0        0      644 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/roborock_queue.py
+-rw-r--r--   0        0        0    12709 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/typing.py
+-rw-r--r--   0        0        0      809 2023-04-11 16:29:11.922855 python_roborock-0.6.4/roborock/util.py
+-rw-r--r--   0        0        0     3348 1970-01-01 00:00:00.000000 python_roborock-0.6.4/PKG-INFO
```

### Comparing `python_roborock-0.6.3/LICENSE` & `python_roborock-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.3/README.md` & `python_roborock-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.3/pyproject.toml` & `python_roborock-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.6.3"
+version = "0.6.4"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `python_roborock-0.6.3/roborock/api.py` & `python_roborock-0.6.4/roborock/api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.3/roborock/cli.py` & `python_roborock-0.6.4/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.3/roborock/cloud_api.py` & `python_roborock-0.6.4/roborock/cloud_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.3/roborock/code_mappings.py` & `python_roborock-0.6.4/roborock/code_mappings.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.3/roborock/containers.py` & `python_roborock-0.6.4/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.3/roborock/exceptions.py` & `python_roborock-0.6.4/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.3/roborock/local_api.py` & `python_roborock-0.6.4/roborock/local_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,15 @@
         response = {}
         await self.connect()
         try:
             async with self._mutex:
                 async with async_timeout.timeout(self.timeout):
                     await self.loop.sock_sendall(self.socket, data)
         except (asyncio.TimeoutError, asyncio.CancelledError):
+            await self.disconnect()
             raise RoborockTimeout(
                 f"Timeout after {self.timeout} seconds waiting for response"
             ) from None
         except BrokenPipeError as e:
             _LOGGER.exception(e)
             await self.disconnect()
         return response
```

### Comparing `python_roborock-0.6.3/roborock/offline/offline.py` & `python_roborock-0.6.4/roborock/offline/offline.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.3/roborock/roborock_message.py` & `python_roborock-0.6.4/roborock/roborock_message.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.3/roborock/roborock_queue.py` & `python_roborock-0.6.4/roborock/roborock_queue.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.3/roborock/typing.py` & `python_roborock-0.6.4/roborock/typing.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.3/roborock/util.py` & `python_roborock-0.6.4/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.3/PKG-INFO` & `python_roborock-0.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.6.3
+Version: 0.6.4
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
-Metadata-Version: 2.1 Name: python-roborock Version: 0.6.3 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 0.6.4 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
 humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

