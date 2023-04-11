# Comparing `tmp/openapify-0.3.tar.gz` & `tmp/openapify-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapify-0.3.tar", last modified: Tue Apr 11 15:01:19 2023, max compression
+gzip compressed data, was "openapify-0.3.1.tar", last modified: Tue Apr 11 15:15:12 2023, max compression
```

## Comparing `openapify-0.3.tar` & `openapify-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:01:19.765096 openapify-0.3/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      749 2023-04-11 15:01:19.764962 openapify-0.3/PKG-INFO
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    29266 2023-04-11 15:00:22.000000 openapify-0.3/README.md
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:01:19.762002 openapify-0.3/openapify/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      282 2023-04-09 19:40:13.000000 openapify-0.3/openapify/__init__.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:01:19.763783 openapify-0.3/openapify/core/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-04-03 13:14:57.000000 openapify-0.3/openapify/core/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    14737 2023-04-11 12:57:05.000000 openapify-0.3/openapify/core/builder.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       92 2023-03-20 20:50:13.000000 openapify-0.3/openapify/core/const.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     2002 2023-04-11 12:57:05.000000 openapify-0.3/openapify/core/document.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1630 2023-04-09 15:42:39.000000 openapify-0.3/openapify/core/jsonschema.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1748 2023-04-09 15:04:29.000000 openapify-0.3/openapify/core/models.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:01:19.764085 openapify-0.3/openapify/core/openapi/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-20 12:12:59.000000 openapify-0.3/openapify/core/openapi/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     5270 2023-04-09 09:42:43.000000 openapify-0.3/openapify/core/openapi/models.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     5208 2023-04-10 17:45:46.000000 openapify-0.3/openapify/decorators.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:01:19.764317 openapify-0.3/openapify/ext/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 15:48:32.000000 openapify-0.3/openapify/ext/__init__.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:01:19.764494 openapify-0.3/openapify/ext/web/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-18 09:45:46.000000 openapify-0.3/openapify/ext/web/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     4767 2023-04-11 10:22:05.000000 openapify-0.3/openapify/ext/web/aiohttp.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 11:19:37.000000 openapify-0.3/openapify/py.typed
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:01:19.762644 openapify-0.3/openapify.egg-info/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      749 2023-04-11 15:01:19.000000 openapify-0.3/openapify.egg-info/PKG-INFO
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      605 2023-04-11 15:01:19.000000 openapify-0.3/openapify.egg-info/SOURCES.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-11 15:01:19.000000 openapify-0.3/openapify.egg-info/dependency_links.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-11 15:01:19.000000 openapify-0.3/openapify.egg-info/not-zip-safe
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       42 2023-04-11 15:01:19.000000 openapify-0.3/openapify.egg-info/requires.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       10 2023-04-11 15:01:19.000000 openapify-0.3/openapify.egg-info/top_level.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      364 2023-04-07 11:44:47.000000 openapify-0.3/pyproject.toml
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       38 2023-04-11 15:01:19.765135 openapify-0.3/setup.cfg
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1132 2023-04-11 14:59:28.000000 openapify-0.3/setup.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:15:12.415802 openapify-0.3.1/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    10763 2023-04-11 15:10:01.000000 openapify-0.3.1/LICENSE
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    30080 2023-04-11 15:15:12.415659 openapify-0.3.1/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    29266 2023-04-11 15:00:22.000000 openapify-0.3.1/README.md
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:15:12.412589 openapify-0.3.1/openapify/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      282 2023-04-09 19:40:13.000000 openapify-0.3.1/openapify/__init__.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:15:12.414555 openapify-0.3.1/openapify/core/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-04-03 13:14:57.000000 openapify-0.3.1/openapify/core/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    14737 2023-04-11 12:57:05.000000 openapify-0.3.1/openapify/core/builder.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       92 2023-03-20 20:50:13.000000 openapify-0.3.1/openapify/core/const.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2002 2023-04-11 12:57:05.000000 openapify-0.3.1/openapify/core/document.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1630 2023-04-09 15:42:39.000000 openapify-0.3.1/openapify/core/jsonschema.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1748 2023-04-09 15:04:29.000000 openapify-0.3.1/openapify/core/models.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:15:12.414871 openapify-0.3.1/openapify/core/openapi/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-20 12:12:59.000000 openapify-0.3.1/openapify/core/openapi/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5270 2023-04-09 09:42:43.000000 openapify-0.3.1/openapify/core/openapi/models.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5208 2023-04-10 17:45:46.000000 openapify-0.3.1/openapify/decorators.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:15:12.415108 openapify-0.3.1/openapify/ext/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 15:48:32.000000 openapify-0.3.1/openapify/ext/__init__.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:15:12.415281 openapify-0.3.1/openapify/ext/web/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-18 09:45:46.000000 openapify-0.3.1/openapify/ext/web/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     4767 2023-04-11 10:22:05.000000 openapify-0.3.1/openapify/ext/web/aiohttp.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 11:19:37.000000 openapify-0.3.1/openapify/py.typed
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:15:12.413301 openapify-0.3.1/openapify.egg-info/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    30080 2023-04-11 15:15:12.000000 openapify-0.3.1/openapify.egg-info/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      613 2023-04-11 15:15:12.000000 openapify-0.3.1/openapify.egg-info/SOURCES.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-11 15:15:12.000000 openapify-0.3.1/openapify.egg-info/dependency_links.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-11 15:01:19.000000 openapify-0.3.1/openapify.egg-info/not-zip-safe
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       42 2023-04-11 15:15:12.000000 openapify-0.3.1/openapify.egg-info/requires.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       10 2023-04-11 15:15:12.000000 openapify-0.3.1/openapify.egg-info/top_level.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      364 2023-04-07 11:44:47.000000 openapify-0.3.1/pyproject.toml
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       38 2023-04-11 15:15:12.415840 openapify-0.3.1/setup.cfg
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1249 2023-04-11 15:11:19.000000 openapify-0.3.1/setup.py
```

### Comparing `openapify-0.3/README.md` & `openapify-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `openapify-0.3/openapify/core/builder.py` & `openapify-0.3.1/openapify/core/builder.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3/openapify/core/document.py` & `openapify-0.3.1/openapify/core/document.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3/openapify/core/jsonschema.py` & `openapify-0.3.1/openapify/core/jsonschema.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3/openapify/core/models.py` & `openapify-0.3.1/openapify/core/models.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3/openapify/core/openapi/models.py` & `openapify-0.3.1/openapify/core/openapi/models.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3/openapify/decorators.py` & `openapify-0.3.1/openapify/decorators.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3/openapify/ext/web/aiohttp.py` & `openapify-0.3.1/openapify/ext/web/aiohttp.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3/openapify.egg-info/SOURCES.txt` & `openapify-0.3.1/openapify.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 setup.py
 openapify/__init__.py
 openapify/decorators.py
 openapify/py.typed
 openapify.egg-info/PKG-INFO
```

