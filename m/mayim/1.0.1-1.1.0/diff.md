# Comparing `tmp/mayim-1.0.1.tar.gz` & `tmp/mayim-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayim-1.0.1.tar", last modified: Tue Aug 16 21:50:20 2022, max compression
+gzip compressed data, was "mayim-1.1.0.tar", last modified: Tue Apr 11 12:29:07 2023, max compression
```

## Comparing `mayim-1.0.1.tar` & `mayim-1.1.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:20.169080 mayim-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-08-16 21:50:11.000000 mayim-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2052 2022-08-16 21:50:20.169080 mayim-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-08-16 21:50:11.000000 mayim-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-08-16 21:50:11.000000 mayim-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-08-16 21:50:20.169080 mayim-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-16 21:50:11.000000 mayim-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:20.161080 mayim-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:20.165080 mayim-1.0.1/src/mayim/
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:20.165080 mayim-1.0.1/src/mayim/base/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9444 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/base/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/base/hydrator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4824 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/base/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/base/query.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:20.165080 mayim-1.0.1/src/mayim/extension/
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/extension/quart_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)     3270 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/extension/sanic_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)     2363 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/extension/starlette_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)     3368 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/extension/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:20.169080 mayim-1.0.1/src/mayim/lazy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/lazy/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     8309 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/mayim.py
--rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:20.169080 mayim-1.0.1/src/mayim/sql/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11321 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/sql/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:20.169080 mayim-1.0.1/src/mayim/sql/mysql/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/sql/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/sql/mysql/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/sql/mysql/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/sql/mysql/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:20.169080 mayim-1.0.1/src/mayim/sql/postgres/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/sql/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/sql/postgres/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/sql/postgres/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/sql/postgres/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/sql/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:20.169080 mayim-1.0.1/src/mayim/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/sql/sqlite/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/sql/sqlite/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-08-16 21:50:11.000000 mayim-1.0.1/src/mayim/sql/sqlite/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 21:50:20.165080 mayim-1.0.1/src/mayim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2052 2022-08-16 21:50:20.000000 mayim-1.0.1/src/mayim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-08-16 21:50:20.000000 mayim-1.0.1/src/mayim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 21:50:20.000000 mayim-1.0.1/src/mayim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 21:50:20.000000 mayim-1.0.1/src/mayim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-08-16 21:50:20.000000 mayim-1.0.1/src/mayim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-08-16 21:50:20.000000 mayim-1.0.1/src/mayim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:29:07.086254 mayim-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 12:28:56.000000 mayim-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-11 12:29:07.086254 mayim-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-11 12:28:56.000000 mayim-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-11 12:28:56.000000 mayim-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-11 12:29:07.086254 mayim-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 12:28:56.000000 mayim-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:29:07.082254 mayim-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:29:07.082254 mayim-1.1.0/src/mayim/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:29:07.082254 mayim-1.1.0/src/mayim/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/base/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/base/hydrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/base/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/base/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:29:07.086254 mayim-1.1.0/src/mayim/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/extension/quart_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/extension/sanic_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/extension/starlette_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/extension/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:29:07.086254 mayim-1.1.0/src/mayim/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/lazy/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/mayim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:29:07.086254 mayim-1.1.0/src/mayim/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/sql/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:29:07.086254 mayim-1.1.0/src/mayim/sql/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/sql/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/sql/mysql/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/sql/mysql/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/sql/mysql/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:29:07.086254 mayim-1.1.0/src/mayim/sql/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/sql/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/sql/postgres/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/sql/postgres/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/sql/postgres/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/sql/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:29:07.086254 mayim-1.1.0/src/mayim/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/sql/sqlite/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/sql/sqlite/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-11 12:28:56.000000 mayim-1.1.0/src/mayim/sql/sqlite/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:29:07.082254 mayim-1.1.0/src/mayim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-11 12:29:07.000000 mayim-1.1.0/src/mayim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-11 12:29:07.000000 mayim-1.1.0/src/mayim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:29:07.000000 mayim-1.1.0/src/mayim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:29:07.000000 mayim-1.1.0/src/mayim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-11 12:29:07.000000 mayim-1.1.0/src/mayim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 12:29:07.000000 mayim-1.1.0/src/mayim.egg-info/top_level.txt
```

### Comparing `mayim-1.0.1/LICENSE` & `mayim-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/PKG-INFO` & `mayim-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayim
-Version: 1.0.1
+Version: 1.1.0
 Summary: The NOT ORM hydrator
 License: MIT
 Keywords: orm
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -55,15 +55,15 @@
         self, limit: int = 4, offset: int = 0
     ) -> List[Person]:
         ...
 
 async def run():
     executor = PersonExecutor()
     Mayim(dsn="postgres://...")
-    print(await executor.select_all_cities())
+    print(await executor.select_all_people())
 
 
 asyncio.run(run())
 ```
 
 ## Documentation
```

### Comparing `mayim-1.0.1/README.md` & `mayim-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self, limit: int = 4, offset: int = 0
     ) -> List[Person]:
         ...
 
 async def run():
     executor = PersonExecutor()
     Mayim(dsn="postgres://...")
-    print(await executor.select_all_cities())
+    print(await executor.select_all_people())
 
 
 asyncio.run(run())
 ```
 
 ## Documentation
```

### Comparing `mayim-1.0.1/pyproject.toml` & `mayim-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/setup.cfg` & `mayim-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mayim
-version = 1.0.1
+version = 1.1.0
 description = The NOT ORM hydrator
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = orm
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `mayim-1.0.1/src/mayim/__init__.py` & `mayim-1.1.0/src/mayim/__init__.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/base/executor.py` & `mayim-1.1.0/src/mayim/base/executor.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/base/hydrator.py` & `mayim-1.1.0/src/mayim/base/hydrator.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/base/interface.py` & `mayim-1.1.0/src/mayim/base/interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 URLPARSE_MAPPING = {
     "hostname": UrlMapping("_host", str),
     "username": UrlMapping("_user", str),
     "password": UrlMapping("_password", str),
     "port": UrlMapping("_port", int),
     "path": UrlMapping("_db", lambda value: value.replace("/", "")),
+    "query": UrlMapping("_query", str),
 }
 
 
 class BaseInterface(ABC):
     scheme = "dummy"
     registered_interfaces: Set[Type[BaseInterface]] = set()
 
@@ -48,23 +49,25 @@
         self,
         dsn: Optional[str] = None,
         host: Optional[int] = None,
         port: Optional[int] = None,
         user: Optional[str] = None,
         password: Optional[str] = None,
         db: Optional[int] = None,
+        query: Optional[str] = None,
     ) -> None:
         """DB class initialization.
 
         Args:
             dsn (str, optional): DB data source name
             host (str, optional): DB address URL or IP
             port (int, optional): DB port. Defaults to 6379
             password (str, optional): DB password
             db (int, optional): DB db. Defaults to 1
+            query (str, optional): DB query parameters. Defaults to None
         """
 
         if dsn and host:
             raise MayimError("Cannot connect to DB using host and dsn")
 
         if not dsn:
             if port and (
@@ -88,14 +91,15 @@
 
         self._dsn = dsn
         self._host = host
         self._port = port
         self._user = user
         self._password = password
         self._db = db
+        self._query = query
         self._full_dsn: Optional[str] = None
         self._connection: ContextVar[Any] = ContextVar(
             "connection", default=None
         )
         self._transaction: ContextVar[bool] = ContextVar(
             "transaction", default=False
         )
@@ -134,14 +138,15 @@
             (
                 f"{self.scheme}://{self.user}:{self.password}@"
                 f"{self.host}:{self.port}/{self.db}"
             )
             if self.password
             else self.dsn
         )
+        self._full_dsn += f"?{self._query}" if self._query else ""
 
     @property
     def dsn(self):
         return self._dsn
 
     @property
     def host(self):
```

### Comparing `mayim-1.0.1/src/mayim/convert.py` & `mayim-1.1.0/src/mayim/convert.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/decorator.py` & `mayim-1.1.0/src/mayim/decorator.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/extension/quart_extension.py` & `mayim-1.1.0/src/mayim/extension/quart_extension.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/extension/sanic_extension.py` & `mayim-1.1.0/src/mayim/extension/sanic_extension.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     from sanic_ext.extensions.base import Extension
 
     SANIC_INSTALLED = True
 except ModuleNotFoundError:
     SANIC_INSTALLED = False
     Extension = type("Extension", (), {})  # type: ignore
     Extend = type("Extend", (), {})  # type: ignore
+    Default = type("Default", (), {})  # type: ignore
+    _default = Default()
 
 
 class SanicMayimExtension(Extension):
     name = "mayim"
 
     def __init__(
         self,
```

### Comparing `mayim-1.0.1/src/mayim/extension/starlette_extension.py` & `mayim-1.1.0/src/mayim/extension/starlette_extension.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/extension/statistics.py` & `mayim-1.1.0/src/mayim/extension/statistics.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/lazy/interface.py` & `mayim-1.1.0/src/mayim/lazy/interface.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/mayim.py` & `mayim-1.1.0/src/mayim/mayim.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from asyncio import get_running_loop
+from contextlib import AsyncExitStack, asynccontextmanager
 from inspect import isclass
 from typing import Optional, Sequence, Type, TypeVar, Union
 from urllib.parse import urlparse
 
 from mayim.base import Executor, Hydrator
 from mayim.base.interface import BaseInterface
 from mayim.exception import MayimError
 from mayim.lazy.interface import LazyPool
 from mayim.registry import InterfaceRegistry, Registry
+from mayim.sql.executor import SQLExecutor
 from mayim.sql.postgres.interface import PostgresPool
 
 T = TypeVar("T", bound=Executor)
 DEFAULT_INTERFACE = PostgresPool
 
 
 class Mayim:
@@ -233,7 +235,36 @@
         for interface in InterfaceRegistry():
             await interface.open()
 
     async def disconnect(self) -> None:
         """Disconnect from all database interfaces"""
         for interface in InterfaceRegistry():
             await interface.close()
+
+    @classmethod
+    @asynccontextmanager
+    async def transaction(
+        cls, *executors: Union[SQLExecutor, Type[SQLExecutor]]
+    ):
+        if not executors:
+            executors = tuple(
+                (
+                    executor
+                    for executor in Registry().values()
+                    if (
+                        isclass(executor) and issubclass(executor, SQLExecutor)
+                    )
+                    or (
+                        not isclass(executor)
+                        and isinstance(executor, SQLExecutor)
+                    )
+                )
+            )
+        async with AsyncExitStack() as stack:
+            for maybe_executor in executors:
+                executor = (
+                    cls.get(maybe_executor)
+                    if isclass(maybe_executor)
+                    else maybe_executor
+                )
+                await stack.enter_async_context(executor.transaction())
+            yield
```

### Comparing `mayim-1.0.1/src/mayim/registry.py` & `mayim-1.1.0/src/mayim/registry.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/sql/executor.py` & `mayim-1.1.0/src/mayim/sql/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,18 +152,20 @@
         as_list: bool = False,
         no_result: bool = False,
         posargs: Optional[Sequence[Any]] = None,
         params: Optional[Dict[str, Any]] = None,
     ):
         ...
 
-    async def rollback(self) -> None:
+    async def rollback(self, *, silent: bool = False) -> None:
         existing = self.pool.existing_connection()
         transaction = self.pool.in_transaction()
         if not existing or not transaction:
+            if silent:
+                return
             raise MayimError("Cannot rollback non-existing transaction")
         await self._rollback(existing)
 
     async def _rollback(self, existing) -> None:
         self.pool._commit.set(False)
         await existing.rollback()
 
@@ -174,20 +176,21 @@
     async def transaction(self):
         self.pool._transaction.set(True)
         async with self.pool.connection() as conn:
             self.pool._connection.set(conn)
             try:
                 yield
             except Exception:
-                await self.rollback()
+                await self.rollback(silent=True)
                 raise
+            else:
+                self.pool._commit.set(True)
             finally:
                 self.pool._connection.set(None)
                 self.pool._transaction.set(False)
-                self.pool._commit.set(True)
 
     @classmethod
     def _load(cls, strict: bool) -> None:
         cls._queries = {}
         cls._hydrators = {}
 
         base_path = cls.get_base_path("queries")
```

### Comparing `mayim-1.0.1/src/mayim/sql/mysql/executor.py` & `mayim-1.1.0/src/mayim/sql/mysql/executor.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/sql/mysql/interface.py` & `mayim-1.1.0/src/mayim/sql/mysql/interface.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/sql/mysql/query.py` & `mayim-1.1.0/src/mayim/sql/mysql/query.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/sql/postgres/executor.py` & `mayim-1.1.0/src/mayim/sql/postgres/executor.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/sql/postgres/interface.py` & `mayim-1.1.0/src/mayim/sql/postgres/interface.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/sql/postgres/query.py` & `mayim-1.1.0/src/mayim/sql/postgres/query.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/sql/query.py` & `mayim-1.1.0/src/mayim/sql/query.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/sql/sqlite/executor.py` & `mayim-1.1.0/src/mayim/sql/sqlite/executor.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim/sql/sqlite/interface.py` & `mayim-1.1.0/src/mayim/sql/sqlite/interface.py`

 * *Files 18% similar despite different names*

```diff
@@ -48,16 +48,27 @@
 
         Returns:
             AsyncIterator[Connection]: Iterator that will yield a connection
 
         Yields:
             Iterator[AsyncIterator[Connection]]: A database connection
         """
+        existing = self.existing_connection()
         close_when_done = False
-        if not self._db:
-            close_when_done = True
-            await self.open()
 
-        yield self._db
+        if existing:
+            yield existing
+        else:
+            if not self._db:
+                close_when_done = True
+                await self.open()
+            yield self._db
+
+        transaction = self.in_transaction()
+        commit = self.do_commit()
+
+        if not transaction:
+            if commit:
+                await self._db.commit()  # type: ignore
 
         if close_when_done:
             await self.close()
```

### Comparing `mayim-1.0.1/src/mayim/sql/sqlite/query.py` & `mayim-1.1.0/src/mayim/sql/sqlite/query.py`

 * *Files identical despite different names*

### Comparing `mayim-1.0.1/src/mayim.egg-info/PKG-INFO` & `mayim-1.1.0/src/mayim.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayim
-Version: 1.0.1
+Version: 1.1.0
 Summary: The NOT ORM hydrator
 License: MIT
 Keywords: orm
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -55,15 +55,15 @@
         self, limit: int = 4, offset: int = 0
     ) -> List[Person]:
         ...
 
 async def run():
     executor = PersonExecutor()
     Mayim(dsn="postgres://...")
-    print(await executor.select_all_cities())
+    print(await executor.select_all_people())
 
 
 asyncio.run(run())
 ```
 
 ## Documentation
```

### Comparing `mayim-1.0.1/src/mayim.egg-info/SOURCES.txt` & `mayim-1.1.0/src/mayim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

