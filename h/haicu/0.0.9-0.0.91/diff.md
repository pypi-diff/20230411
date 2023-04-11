# Comparing `tmp/haicu-0.0.9.tar.gz` & `tmp/haicu-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haicu-0.0.9.tar", last modified: Tue Apr 11 17:58:25 2023, max compression
+gzip compressed data, was "haicu-0.0.91.tar", last modified: Tue Apr 11 18:08:36 2023, max compression
```

## Comparing `haicu-0.0.9.tar` & `haicu-0.0.91.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 17:58:25.767795 haicu-0.0.9/
--rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 17:38:44.000000 haicu-0.0.9/LICENSE
--rw-rw-r--   0 bry       (1000) bry       (1000)     1725 2023-04-11 17:58:25.767795 haicu-0.0.9/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)      206 2023-04-11 17:39:56.000000 haicu-0.0.9/README.md
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 17:58:25.767795 haicu-0.0.9/haicu.egg-info/
--rw-rw-r--   0 bry       (1000) bry       (1000)     1725 2023-04-11 17:58:25.000000 haicu-0.0.9/haicu.egg-info/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)      176 2023-04-11 17:58:25.000000 haicu-0.0.9/haicu.egg-info/SOURCES.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-04-11 17:58:25.000000 haicu-0.0.9/haicu.egg-info/dependency_links.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-04-11 17:58:25.000000 haicu-0.0.9/haicu.egg-info/requires.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-04-11 17:58:25.000000 haicu-0.0.9/haicu.egg-info/top_level.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)      697 2023-04-11 17:40:31.000000 haicu-0.0.9/pyproject.toml
--rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-04-11 17:58:25.767795 haicu-0.0.9/setup.cfg
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:08:36.780707 haicu-0.0.91/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 17:38:44.000000 haicu-0.0.91/LICENSE
+-rw-rw-r--   0 bry       (1000) bry       (1000)     1726 2023-04-11 18:08:36.780707 haicu-0.0.91/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)      206 2023-04-11 17:39:56.000000 haicu-0.0.91/README.md
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 18:08:36.780707 haicu-0.0.91/haicu.egg-info/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     1726 2023-04-11 18:08:36.000000 haicu-0.0.91/haicu.egg-info/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)      176 2023-04-11 18:08:36.000000 haicu-0.0.91/haicu.egg-info/SOURCES.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-04-11 18:08:36.000000 haicu-0.0.91/haicu.egg-info/dependency_links.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-04-11 18:08:36.000000 haicu-0.0.91/haicu.egg-info/requires.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-04-11 18:08:36.000000 haicu-0.0.91/haicu.egg-info/top_level.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)      698 2023-04-11 18:08:29.000000 haicu-0.0.91/pyproject.toml
+-rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-04-11 18:08:36.780707 haicu-0.0.91/setup.cfg
```

### Comparing `haicu-0.0.9/LICENSE` & `haicu-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `haicu-0.0.9/PKG-INFO` & `haicu-0.0.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.0.9
+Version: 0.0.91
 Summary: haicu package for HAICU
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

### Comparing `haicu-0.0.9/haicu.egg-info/PKG-INFO` & `haicu-0.0.91/haicu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.0.9
+Version: 0.0.91
 Summary: haicu package for HAICU
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

### Comparing `haicu-0.0.9/pyproject.toml` & `haicu-0.0.91/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "haicu"
 description = "haicu package for HAICU"
-version = "0.0.9"
+version = "0.0.91"
 authors = [
     { name = "Bryerton Shaw", email = "bryerton@triumf.ca" }
 ]
 maintainers = [
     { name = "Bryerton Shaw", email = "bryerton@triumf.ca" }
 ]
 readme.file = "README.md"
```

