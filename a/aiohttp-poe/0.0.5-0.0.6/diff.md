# Comparing `tmp/aiohttp_poe-0.0.5.tar.gz` & `tmp/aiohttp_poe-0.0.6.tar.gz`

## Comparing `aiohttp_poe-0.0.5.tar` & `aiohttp_poe-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.5/src/aiohttp_poe/__init__.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.5/src/aiohttp_poe/__main__.py
--rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.5/src/aiohttp_poe/base.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.5/src/aiohttp_poe/types.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.5/src/aiohttp_poe/samples/catbot.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.5/src/aiohttp_poe/samples/echo.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.5/.gitignore
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.5/README.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/src/aiohttp_poe/__init__.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/src/aiohttp_poe/__main__.py
+-rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/src/aiohttp_poe/base.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/src/aiohttp_poe/types.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/src/aiohttp_poe/samples/catbot.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/src/aiohttp_poe/samples/echo.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/README.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/PKG-INFO
```

### Comparing `aiohttp_poe-0.0.5/src/aiohttp_poe/base.py` & `aiohttp_poe-0.0.6/src/aiohttp_poe/base.py`

 * *Files identical despite different names*

### Comparing `aiohttp_poe-0.0.5/src/aiohttp_poe/types.py` & `aiohttp_poe-0.0.6/src/aiohttp_poe/types.py`

 * *Files identical despite different names*

### Comparing `aiohttp_poe-0.0.5/src/aiohttp_poe/samples/catbot.py` & `aiohttp_poe-0.0.6/src/aiohttp_poe/samples/catbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             yield self.text_event("\n")
             yield self.text_event("A table:\n\n")
             yield self.text_event("| animal | cuteness |\n")
             yield self.text_event("|--------|----------|\n")
             yield self.text_event("| cat    | 10       |\n")
             yield self.text_event("| dog    | 1        |\n")
             yield self.text_event("\n")
-        if "cardbord" in last_message:
+        if "cardboard" in last_message:
             yield self.text_event("crunch ")
             yield self.text_event("crunch")
         elif (
             "kitchen" in last_message
             or "meal" in last_message
             or "food" in last_message
         ):
```

### Comparing `aiohttp_poe-0.0.5/src/aiohttp_poe/samples/echo.py` & `aiohttp_poe-0.0.6/src/aiohttp_poe/samples/echo.py`

 * *Files identical despite different names*

### Comparing `aiohttp_poe-0.0.5/README.md` & `aiohttp_poe-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aiohttp_poe-0.0.5/pyproject.toml` & `aiohttp_poe-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aiohttp_poe"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Jelle Zijlstra", email="jelle@quora.com" },
 ]
 description = "A demonstration of the Poe protocol using aiohttp"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aiohttp_poe-0.0.5/PKG-INFO` & `aiohttp_poe-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp_poe
-Version: 0.0.5
+Version: 0.0.6
 Summary: A demonstration of the Poe protocol using aiohttp
 Project-URL: Homepage, https://github.com/quora/poe-protocol
 Author-email: Jelle Zijlstra <jelle@quora.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

