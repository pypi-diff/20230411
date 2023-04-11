# Comparing `tmp/haicu-0.0.94.tar.gz` & `tmp/haicu-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haicu-0.0.94.tar", last modified: Tue Apr 11 18:15:51 2023, max compression
+gzip compressed data, was "haicu-0.0.95.tar", last modified: Tue Apr 11 18:16:31 2023, max compression
```

## Comparing `haicu-0.0.94.tar` & `haicu-0.0.95.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:15:51.385247 haicu-0.0.94/
--rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-0.0.94/LICENSE
--rw-rw-r--   0 bry       (1000) bry       (1000)     2593 2023-04-11 18:15:51.385247 haicu-0.0.94/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)     1073 2023-04-11 17:00:57.000000 haicu-0.0.94/README.md
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:15:51.385247 haicu-0.0.94/haicu/
--rw-rw-r--   0 bry       (1000) bry       (1000)        0 2023-03-10 00:08:52.000000 haicu-0.0.94/haicu/__init__.py
--rwxrwxr-x   0 bry       (1000) bry       (1000)    28623 2023-04-11 18:14:35.000000 haicu-0.0.94/haicu/__main__.py
--rwxrwxr-x   0 bry       (1000) bry       (1000)    12563 2023-04-11 18:13:59.000000 haicu-0.0.94/haicu/format.py
--rw-rw-r--   0 bry       (1000) bry       (1000)    11443 2023-04-11 18:13:59.000000 haicu-0.0.94/haicu/ftdi.py
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:15:51.385247 haicu-0.0.94/haicu.egg-info/
--rw-rw-r--   0 bry       (1000) bry       (1000)     2593 2023-04-11 18:15:51.000000 haicu-0.0.94/haicu.egg-info/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)      274 2023-04-11 18:15:51.000000 haicu-0.0.94/haicu.egg-info/SOURCES.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-04-11 18:15:51.000000 haicu-0.0.94/haicu.egg-info/dependency_links.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       50 2023-04-11 18:15:51.000000 haicu-0.0.94/haicu.egg-info/entry_points.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-04-11 18:15:51.000000 haicu-0.0.94/haicu.egg-info/requires.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-04-11 18:15:51.000000 haicu-0.0.94/haicu.egg-info/top_level.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)      709 2023-04-11 18:15:10.000000 haicu-0.0.94/pyproject.toml
--rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-04-11 18:15:51.385247 haicu-0.0.94/setup.cfg
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:16:31.493294 haicu-0.0.95/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-0.0.95/LICENSE
+-rw-rw-r--   0 bry       (1000) bry       (1000)     2593 2023-04-11 18:16:31.493294 haicu-0.0.95/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)     1073 2023-04-11 17:00:57.000000 haicu-0.0.95/README.md
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:16:31.493294 haicu-0.0.95/haicu/
+-rw-rw-r--   0 bry       (1000) bry       (1000)        0 2023-03-10 00:08:52.000000 haicu-0.0.95/haicu/__init__.py
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    28623 2023-04-11 18:14:35.000000 haicu-0.0.95/haicu/__main__.py
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    12563 2023-04-11 18:13:59.000000 haicu-0.0.95/haicu/format.py
+-rw-rw-r--   0 bry       (1000) bry       (1000)    11443 2023-04-11 18:13:59.000000 haicu-0.0.95/haicu/ftdi.py
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:16:31.493294 haicu-0.0.95/haicu.egg-info/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     2593 2023-04-11 18:16:31.000000 haicu-0.0.95/haicu.egg-info/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)      274 2023-04-11 18:16:31.000000 haicu-0.0.95/haicu.egg-info/SOURCES.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-04-11 18:16:31.000000 haicu-0.0.95/haicu.egg-info/dependency_links.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       50 2023-04-11 18:16:31.000000 haicu-0.0.95/haicu.egg-info/entry_points.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-04-11 18:16:31.000000 haicu-0.0.95/haicu.egg-info/requires.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-04-11 18:16:31.000000 haicu-0.0.95/haicu.egg-info/top_level.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)      709 2023-04-11 18:16:25.000000 haicu-0.0.95/pyproject.toml
+-rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-04-11 18:16:31.493294 haicu-0.0.95/setup.cfg
```

### Comparing `haicu-0.0.94/LICENSE` & `haicu-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `haicu-0.0.94/PKG-INFO` & `haicu-0.0.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.0.94
+Version: 0.0.95
 Summary: haicu package for HAICU
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

### Comparing `haicu-0.0.94/README.md` & `haicu-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `haicu-0.0.94/haicu/__main__.py` & `haicu-0.0.95/haicu/__main__.py`

 * *Files identical despite different names*

### Comparing `haicu-0.0.94/haicu/format.py` & `haicu-0.0.95/haicu/format.py`

 * *Files identical despite different names*

### Comparing `haicu-0.0.94/haicu/ftdi.py` & `haicu-0.0.95/haicu/ftdi.py`

 * *Files identical despite different names*

### Comparing `haicu-0.0.94/haicu.egg-info/PKG-INFO` & `haicu-0.0.95/haicu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.0.94
+Version: 0.0.95
 Summary: haicu package for HAICU
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

### Comparing `haicu-0.0.94/pyproject.toml` & `haicu-0.0.95/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "haicu"
 description = "haicu package for HAICU"
-version = "0.0.94"
+version = "0.0.95"
 authors = [
     { name = "Bryerton Shaw", email = "bryerton@triumf.ca" }
 ]
 maintainers = [
     { name = "Bryerton Shaw", email = "bryerton@triumf.ca" }
 ]
 readme.file = "README.md"
```

