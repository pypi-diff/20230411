# Comparing `tmp/erich-0.0.1.tar.gz` & `tmp/erich-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erich-0.0.1.tar", last modified: Fri Apr  7 17:02:18 2023, max compression
+gzip compressed data, was "erich-0.0.2.tar", last modified: Tue Apr 11 19:01:10 2023, max compression
```

## Comparing `erich-0.0.1.tar` & `erich-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2023-04-07 17:02:18.851402 erich-0.0.1/
--rw-r--r--   0 robin     (1000) robin     (1000)     1211 2023-04-07 16:16:09.000000 erich-0.0.1/LICENSE
--rw-r--r--   0 robin     (1000) robin     (1000)     1764 2023-04-07 17:02:18.852402 erich-0.0.1/PKG-INFO
--rw-r--r--   0 robin     (1000) robin     (1000)     1293 2023-04-07 17:02:06.000000 erich-0.0.1/README.md
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2023-04-07 17:02:18.850402 erich-0.0.1/erich/
--rw-r--r--   0 robin     (1000) robin     (1000)       44 2023-04-07 16:38:59.000000 erich-0.0.1/erich/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4053 2023-04-07 16:58:55.000000 erich-0.0.1/erich/erich.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2023-04-07 17:02:18.851402 erich-0.0.1/erich.egg-info/
--rw-r--r--   0 robin     (1000) robin     (1000)     1764 2023-04-07 17:02:18.000000 erich-0.0.1/erich.egg-info/PKG-INFO
--rw-r--r--   0 robin     (1000) robin     (1000)      215 2023-04-07 17:02:18.000000 erich-0.0.1/erich.egg-info/SOURCES.txt
--rw-r--r--   0 robin     (1000) robin     (1000)        1 2023-04-07 17:02:18.000000 erich-0.0.1/erich.egg-info/dependency_links.txt
--rw-r--r--   0 robin     (1000) robin     (1000)        6 2023-04-07 17:02:18.000000 erich-0.0.1/erich.egg-info/top_level.txt
--rw-r--r--   0 robin     (1000) robin     (1000)        1 2023-04-07 16:54:48.000000 erich-0.0.1/erich.egg-info/zip-safe
--rw-r--r--   0 robin     (1000) robin     (1000)      489 2023-04-07 16:35:23.000000 erich-0.0.1/pyproject.toml
--rw-r--r--   0 robin     (1000) robin     (1000)      416 2023-04-07 17:02:18.852402 erich-0.0.1/setup.cfg
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2023-04-11 19:01:10.037172 erich-0.0.2/
+-rw-r--r--   0 robin     (1000) robin     (1000)     1211 2023-04-07 16:16:09.000000 erich-0.0.2/LICENSE
+-rw-r--r--   0 robin     (1000) robin     (1000)     1916 2023-04-11 19:01:10.038172 erich-0.0.2/PKG-INFO
+-rw-r--r--   0 robin     (1000) robin     (1000)     1445 2023-04-07 20:18:59.000000 erich-0.0.2/README.md
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2023-04-11 19:01:10.024172 erich-0.0.2/erich/
+-rw-r--r--   0 robin     (1000) robin     (1000)       44 2023-04-11 18:58:54.000000 erich-0.0.2/erich/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6343 2023-04-11 18:51:01.000000 erich-0.0.2/erich/erich.py
+drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2023-04-11 19:01:10.037172 erich-0.0.2/erich.egg-info/
+-rw-r--r--   0 robin     (1000) robin     (1000)     1916 2023-04-11 19:01:10.000000 erich-0.0.2/erich.egg-info/PKG-INFO
+-rw-r--r--   0 robin     (1000) robin     (1000)      215 2023-04-11 19:01:10.000000 erich-0.0.2/erich.egg-info/SOURCES.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)        1 2023-04-11 19:01:10.000000 erich-0.0.2/erich.egg-info/dependency_links.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)        6 2023-04-11 19:01:10.000000 erich-0.0.2/erich.egg-info/top_level.txt
+-rw-r--r--   0 robin     (1000) robin     (1000)        1 2023-04-07 16:54:48.000000 erich-0.0.2/erich.egg-info/zip-safe
+-rw-r--r--   0 robin     (1000) robin     (1000)      489 2023-04-11 18:58:42.000000 erich-0.0.2/pyproject.toml
+-rw-r--r--   0 robin     (1000) robin     (1000)      416 2023-04-11 19:01:10.039172 erich-0.0.2/setup.cfg
```

### Comparing `erich-0.0.1/LICENSE` & `erich-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `erich-0.0.1/PKG-INFO` & `erich-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erich
-Version: 0.0.1
+Version: 0.0.2
 Summary: Decorators for better error handling
 Author: Robin Bergewski
 License: unlicense
 Project-URL: Homepage, https://github.com/Sojamann/erich
 Keywords: decorator,decorators,error,errors
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,15 +28,15 @@
 # be present in the function signature.
 @erich.fmt("Tried starting task {name} ({desc})")
 def start_task(name: str, prio: int, fn: Callable, desc: str = None):
     schedule(prio, fn)
 
 # Print that this function has been called but only include the prio
 # in the output
-@erich.with_args("prio")
+@erich.signature("prio")
 def schedule(prio: int, fn: Callable):
     can_schedule(prio)
     fn()
 
 # add some nicer output to the final result
 @erich.fmt("Cannot schedule task due to")
 def can_schedule(prio: int):
@@ -62,11 +62,17 @@
 Tried starting task test (very important)
 ↳ during call of schedule(prio = -1)
  ↳ Cannot schedule task due to
   ↳ Cannot schedule something with prio -1. It's invalid
 ```
 
 
-## Build
+## Release
+1. update version in setup.cfg, pyproject.toml and root \_\_init\_\_.py
+2. build
 ```sh
 python -m build
 ```
+3. upload
+```sh
+python3 -m twine upload --repository pypi dist/*
+```
```

### Comparing `erich-0.0.1/erich.egg-info/PKG-INFO` & `erich-0.0.2/erich.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erich
-Version: 0.0.1
+Version: 0.0.2
 Summary: Decorators for better error handling
 Author: Robin Bergewski
 License: unlicense
 Project-URL: Homepage, https://github.com/Sojamann/erich
 Keywords: decorator,decorators,error,errors
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,15 +28,15 @@
 # be present in the function signature.
 @erich.fmt("Tried starting task {name} ({desc})")
 def start_task(name: str, prio: int, fn: Callable, desc: str = None):
     schedule(prio, fn)
 
 # Print that this function has been called but only include the prio
 # in the output
-@erich.with_args("prio")
+@erich.signature("prio")
 def schedule(prio: int, fn: Callable):
     can_schedule(prio)
     fn()
 
 # add some nicer output to the final result
 @erich.fmt("Cannot schedule task due to")
 def can_schedule(prio: int):
@@ -62,11 +62,17 @@
 Tried starting task test (very important)
 ↳ during call of schedule(prio = -1)
  ↳ Cannot schedule task due to
   ↳ Cannot schedule something with prio -1. It's invalid
 ```
 
 
-## Build
+## Release
+1. update version in setup.cfg, pyproject.toml and root \_\_init\_\_.py
+2. build
 ```sh
 python -m build
 ```
+3. upload
+```sh
+python3 -m twine upload --repository pypi dist/*
+```
```

