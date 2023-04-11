# Comparing `tmp/cgiw-0.1.3.tar.gz` & `tmp/cgiw-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgiw-0.1.3.tar", last modified: Tue Apr  4 11:47:59 2023, max compression
+gzip compressed data, was "cgiw-0.1.4.tar", last modified: Tue Apr 11 13:08:37 2023, max compression
```

## Comparing `cgiw-0.1.3.tar` & `cgiw-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-04-04 11:47:59.606538 cgiw-0.1.3/
--rw-rw-r--   0 james     (1000) james     (1000)    35149 2023-01-05 15:28:28.000000 cgiw-0.1.3/LICENSE
--rw-rw-r--   0 james     (1000) james     (1000)     1629 2023-04-04 11:47:59.606538 cgiw-0.1.3/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)     1117 2023-01-22 20:57:29.000000 cgiw-0.1.3/README.md
--rw-rw-r--   0 james     (1000) james     (1000)      584 2023-04-04 11:47:37.000000 cgiw-0.1.3/pyproject.toml
--rw-rw-r--   0 james     (1000) james     (1000)       38 2023-04-04 11:47:59.606538 cgiw-0.1.3/setup.cfg
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-04-04 11:47:59.598538 cgiw-0.1.3/src/
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-04-04 11:47:59.602538 cgiw-0.1.3/src/cgiw/
--rw-rw-r--   0 james     (1000) james     (1000)       21 2023-01-16 23:30:07.000000 cgiw-0.1.3/src/cgiw/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)      238 2023-01-22 20:04:01.000000 cgiw-0.1.3/src/cgiw/composers.py
--rw-rw-r--   0 james     (1000) james     (1000)      872 2023-01-22 20:45:17.000000 cgiw-0.1.3/src/cgiw/decorators.py
--rw-rw-r--   0 james     (1000) james     (1000)      506 2023-01-22 20:50:23.000000 cgiw-0.1.3/src/cgiw/handler.py
--rw-rw-r--   0 james     (1000) james     (1000)     1230 2023-04-04 11:47:17.000000 cgiw-0.1.3/src/cgiw/parsers.py
--rw-rw-r--   0 james     (1000) james     (1000)      581 2023-02-24 22:19:27.000000 cgiw-0.1.3/src/cgiw/responses.py
--rw-rw-r--   0 james     (1000) james     (1000)      638 2023-01-16 23:31:26.000000 cgiw-0.1.3/src/cgiw/run.py
--rw-rw-r--   0 james     (1000) james     (1000)      516 2023-01-22 20:49:49.000000 cgiw-0.1.3/src/cgiw/types.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-04-04 11:47:59.602538 cgiw-0.1.3/src/cgiw.egg-info/
--rw-rw-r--   0 james     (1000) james     (1000)     1629 2023-04-04 11:47:59.000000 cgiw-0.1.3/src/cgiw.egg-info/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)      457 2023-04-04 11:47:59.000000 cgiw-0.1.3/src/cgiw.egg-info/SOURCES.txt
--rw-rw-r--   0 james     (1000) james     (1000)        1 2023-04-04 11:47:59.000000 cgiw-0.1.3/src/cgiw.egg-info/dependency_links.txt
--rw-rw-r--   0 james     (1000) james     (1000)        5 2023-04-04 11:47:59.000000 cgiw-0.1.3/src/cgiw.egg-info/top_level.txt
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-04-04 11:47:59.606538 cgiw-0.1.3/tests/
--rw-rw-r--   0 james     (1000) james     (1000)      529 2023-01-22 20:02:27.000000 cgiw-0.1.3/tests/test_composers.py
--rw-rw-r--   0 james     (1000) james     (1000)     1054 2023-01-22 20:45:06.000000 cgiw-0.1.3/tests/test_decorators.py
--rw-rw-r--   0 james     (1000) james     (1000)      876 2023-01-07 17:23:45.000000 cgiw-0.1.3/tests/test_handler.py
--rw-rw-r--   0 james     (1000) james     (1000)     1033 2023-01-09 23:56:09.000000 cgiw-0.1.3/tests/test_parsers.py
--rw-rw-r--   0 james     (1000) james     (1000)      700 2023-01-22 20:49:00.000000 cgiw-0.1.3/tests/test_responses.py
--rw-rw-r--   0 james     (1000) james     (1000)      642 2023-01-22 20:09:59.000000 cgiw-0.1.3/tests/test_run.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-04-11 13:08:37.633652 cgiw-0.1.4/
+-rw-rw-r--   0 james     (1000) james     (1000)    35149 2023-01-05 15:28:28.000000 cgiw-0.1.4/LICENSE
+-rw-rw-r--   0 james     (1000) james     (1000)     1629 2023-04-11 13:08:37.633652 cgiw-0.1.4/PKG-INFO
+-rw-rw-r--   0 james     (1000) james     (1000)     1117 2023-01-22 20:57:29.000000 cgiw-0.1.4/README.md
+-rw-rw-r--   0 james     (1000) james     (1000)      584 2023-04-11 13:08:06.000000 cgiw-0.1.4/pyproject.toml
+-rw-rw-r--   0 james     (1000) james     (1000)       38 2023-04-11 13:08:37.633652 cgiw-0.1.4/setup.cfg
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-04-11 13:08:37.629652 cgiw-0.1.4/src/
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-04-11 13:08:37.629652 cgiw-0.1.4/src/cgiw/
+-rw-rw-r--   0 james     (1000) james     (1000)       21 2023-01-16 23:30:07.000000 cgiw-0.1.4/src/cgiw/__init__.py
+-rw-rw-r--   0 james     (1000) james     (1000)      238 2023-01-22 20:04:01.000000 cgiw-0.1.4/src/cgiw/composers.py
+-rw-rw-r--   0 james     (1000) james     (1000)      872 2023-01-22 20:45:17.000000 cgiw-0.1.4/src/cgiw/decorators.py
+-rw-rw-r--   0 james     (1000) james     (1000)      438 2023-04-11 12:49:00.000000 cgiw-0.1.4/src/cgiw/exceptions.py
+-rw-rw-r--   0 james     (1000) james     (1000)      741 2023-04-11 12:52:19.000000 cgiw-0.1.4/src/cgiw/handler.py
+-rw-rw-r--   0 james     (1000) james     (1000)     1364 2023-04-11 13:07:34.000000 cgiw-0.1.4/src/cgiw/parsers.py
+-rw-rw-r--   0 james     (1000) james     (1000)      581 2023-02-24 22:19:27.000000 cgiw-0.1.4/src/cgiw/responses.py
+-rw-rw-r--   0 james     (1000) james     (1000)      749 2023-04-11 12:44:30.000000 cgiw-0.1.4/src/cgiw/run.py
+-rw-rw-r--   0 james     (1000) james     (1000)      516 2023-01-22 20:49:49.000000 cgiw-0.1.4/src/cgiw/types.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-04-11 13:08:37.633652 cgiw-0.1.4/src/cgiw.egg-info/
+-rw-rw-r--   0 james     (1000) james     (1000)     1629 2023-04-11 13:08:37.000000 cgiw-0.1.4/src/cgiw.egg-info/PKG-INFO
+-rw-rw-r--   0 james     (1000) james     (1000)      480 2023-04-11 13:08:37.000000 cgiw-0.1.4/src/cgiw.egg-info/SOURCES.txt
+-rw-rw-r--   0 james     (1000) james     (1000)        1 2023-04-11 13:08:37.000000 cgiw-0.1.4/src/cgiw.egg-info/dependency_links.txt
+-rw-rw-r--   0 james     (1000) james     (1000)        5 2023-04-11 13:08:37.000000 cgiw-0.1.4/src/cgiw.egg-info/top_level.txt
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-04-11 13:08:37.633652 cgiw-0.1.4/tests/
+-rw-rw-r--   0 james     (1000) james     (1000)      529 2023-01-22 20:02:27.000000 cgiw-0.1.4/tests/test_composers.py
+-rw-rw-r--   0 james     (1000) james     (1000)     1054 2023-04-11 13:03:07.000000 cgiw-0.1.4/tests/test_decorators.py
+-rw-rw-r--   0 james     (1000) james     (1000)      876 2023-04-11 13:04:06.000000 cgiw-0.1.4/tests/test_handler.py
+-rw-rw-r--   0 james     (1000) james     (1000)     1033 2023-01-09 23:56:09.000000 cgiw-0.1.4/tests/test_parsers.py
+-rw-rw-r--   0 james     (1000) james     (1000)      700 2023-01-22 20:49:00.000000 cgiw-0.1.4/tests/test_responses.py
+-rw-rw-r--   0 james     (1000) james     (1000)     1127 2023-04-11 12:55:38.000000 cgiw-0.1.4/tests/test_run.py
```

### Comparing `cgiw-0.1.3/LICENSE` & `cgiw-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.3/PKG-INFO` & `cgiw-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgiw
-Version: 0.1.3
+Version: 0.1.4
 Summary: A framework for building python cgi scripts
 Author-email: James Rao <jamesnarayanrao@gmail.com>
 Project-URL: Homepage, https://github.com/JamesRao98/cgiw
 Project-URL: Bug Tracker, https://github.com/JamesRao98/cgiw/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cgiw-0.1.3/README.md` & `cgiw-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.3/pyproject.toml` & `cgiw-0.1.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cgiw"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="James Rao", email="jamesnarayanrao@gmail.com" },
 ]
 description = "A framework for building python cgi scripts"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cgiw-0.1.3/src/cgiw/decorators.py` & `cgiw-0.1.4/src/cgiw/decorators.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.3/src/cgiw/parsers.py` & `cgiw-0.1.4/src/cgiw/parsers.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,20 +17,24 @@
     return parse_qs(getenv('QUERY_STRING'))
 
 
 def parse_headers() -> HeadersType:
     def format_key(k: str):
         return '-'.join([p.capitalize() for p in k.split('_')][1:])
 
-    return {
-        'Content-Type': getenv('CONTENT_TYPE', ''),
-        'Content-Length': getenv('CONTENT_LENGTH', ''),
-        'Remote-User': getenv('REMOTE_USER', ''),
-        **{format_key(k): v for k, v in environ.items() if k.startswith('HTTP_')}
-    }
+    headers = {format_key(k): v for k, v in environ.items() if k.startswith('HTTP_')}
+
+    if content_type := getenv('CONTENT_TYPE'):
+        headers['Content-Type'] = content_type
+    if content_length := getenv('CONTENT_LENGTH'):
+        headers['Content-Length'] = content_length
+    if remote_user := getenv('REMOTE_USER'):
+        headers['Remote-User'] = remote_user
+
+    return headers
 
 
 def parse_body(headers: HeadersType) -> str:
     if not(length := int(headers.get('Content-Length') or 0)):
         return str()
 
     raw_data = stdin.read(length)
```

### Comparing `cgiw-0.1.3/src/cgiw/responses.py` & `cgiw-0.1.4/src/cgiw/responses.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.3/src/cgiw/types.py` & `cgiw-0.1.4/src/cgiw/types.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.3/src/cgiw.egg-info/PKG-INFO` & `cgiw-0.1.4/src/cgiw.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgiw
-Version: 0.1.3
+Version: 0.1.4
 Summary: A framework for building python cgi scripts
 Author-email: James Rao <jamesnarayanrao@gmail.com>
 Project-URL: Homepage, https://github.com/JamesRao98/cgiw
 Project-URL: Bug Tracker, https://github.com/JamesRao98/cgiw/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cgiw-0.1.3/tests/test_composers.py` & `cgiw-0.1.4/tests/test_composers.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.3/tests/test_decorators.py` & `cgiw-0.1.4/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.3/tests/test_handler.py` & `cgiw-0.1.4/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.3/tests/test_parsers.py` & `cgiw-0.1.4/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `cgiw-0.1.3/tests/test_responses.py` & `cgiw-0.1.4/tests/test_responses.py`

 * *Files identical despite different names*

