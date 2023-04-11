# Comparing `tmp/haicu-0.8.0.tar.gz` & `tmp/haicu-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haicu-0.8.0.tar", last modified: Tue Apr 11 19:58:36 2023, max compression
+gzip compressed data, was "haicu-0.8.1.tar", last modified: Tue Apr 11 20:00:21 2023, max compression
```

## Comparing `haicu-0.8.0.tar` & `haicu-0.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 19:58:36.397771 haicu-0.8.0/
--rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-0.8.0/LICENSE
--rw-rw-r--   0 bry       (1000) bry       (1000)     3555 2023-04-11 19:58:36.397771 haicu-0.8.0/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)     2042 2023-04-11 19:58:00.000000 haicu-0.8.0/README.md
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 19:58:36.397771 haicu-0.8.0/haicu/
--rw-rw-r--   0 bry       (1000) bry       (1000)        0 2023-03-10 00:08:52.000000 haicu-0.8.0/haicu/__init__.py
--rwxrwxr-x   0 bry       (1000) bry       (1000)    28539 2023-04-11 19:32:04.000000 haicu-0.8.0/haicu/__main__.py
--rwxrwxr-x   0 bry       (1000) bry       (1000)    12563 2023-04-11 18:21:24.000000 haicu-0.8.0/haicu/format.py
--rw-rw-r--   0 bry       (1000) bry       (1000)    11443 2023-04-11 18:13:59.000000 haicu-0.8.0/haicu/ftdi.py
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 19:58:36.397771 haicu-0.8.0/haicu.egg-info/
--rw-rw-r--   0 bry       (1000) bry       (1000)     3555 2023-04-11 19:58:36.000000 haicu-0.8.0/haicu.egg-info/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)      274 2023-04-11 19:58:36.000000 haicu-0.8.0/haicu.egg-info/SOURCES.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-04-11 19:58:36.000000 haicu-0.8.0/haicu.egg-info/dependency_links.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       50 2023-04-11 19:58:36.000000 haicu-0.8.0/haicu.egg-info/entry_points.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-04-11 19:58:36.000000 haicu-0.8.0/haicu.egg-info/requires.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-04-11 19:58:36.000000 haicu-0.8.0/haicu.egg-info/top_level.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)      742 2023-04-11 19:58:26.000000 haicu-0.8.0/pyproject.toml
--rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-04-11 19:58:36.397771 haicu-0.8.0/setup.cfg
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:00:21.881911 haicu-0.8.1/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-0.8.1/LICENSE
+-rw-rw-r--   0 bry       (1000) bry       (1000)     3555 2023-04-11 20:00:21.881911 haicu-0.8.1/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)     2042 2023-04-11 19:58:00.000000 haicu-0.8.1/README.md
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:00:21.881911 haicu-0.8.1/haicu/
+-rw-rw-r--   0 bry       (1000) bry       (1000)        0 2023-03-10 00:08:52.000000 haicu-0.8.1/haicu/__init__.py
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    28538 2023-04-11 20:00:06.000000 haicu-0.8.1/haicu/__main__.py
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    12563 2023-04-11 18:21:24.000000 haicu-0.8.1/haicu/format.py
+-rw-rw-r--   0 bry       (1000) bry       (1000)    11443 2023-04-11 18:13:59.000000 haicu-0.8.1/haicu/ftdi.py
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:00:21.881911 haicu-0.8.1/haicu.egg-info/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     3555 2023-04-11 20:00:21.000000 haicu-0.8.1/haicu.egg-info/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)      274 2023-04-11 20:00:21.000000 haicu-0.8.1/haicu.egg-info/SOURCES.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-04-11 20:00:21.000000 haicu-0.8.1/haicu.egg-info/dependency_links.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       50 2023-04-11 20:00:21.000000 haicu-0.8.1/haicu.egg-info/entry_points.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-04-11 20:00:21.000000 haicu-0.8.1/haicu.egg-info/requires.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-04-11 20:00:21.000000 haicu-0.8.1/haicu.egg-info/top_level.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)      742 2023-04-11 20:00:16.000000 haicu-0.8.1/pyproject.toml
+-rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-04-11 20:00:21.881911 haicu-0.8.1/setup.cfg
```

### Comparing `haicu-0.8.0/LICENSE` & `haicu-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `haicu-0.8.0/PKG-INFO` & `haicu-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.8.0
+Version: 0.8.1
 Summary: package for HAICU
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

### Comparing `haicu-0.8.0/README.md` & `haicu-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `haicu-0.8.0/haicu/__main__.py` & `haicu-0.8.1/haicu/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     except:
         print("Device '" + str(args.serial) + "' not found!")
         print()
         arg_list(args, None)
         sys.exit(-1)
 
     if(args.command == None):
-        parser.print_usage()
+        parser.print_help()
         sys.exit(0)
 
     args.func(args, ftdi_dev)
 
 def arg_list(args, ftdi_dev):
     print("Available devices:")
     result = haicu_ftdi.list_devices()
```

### Comparing `haicu-0.8.0/haicu/format.py` & `haicu-0.8.1/haicu/format.py`

 * *Files identical despite different names*

### Comparing `haicu-0.8.0/haicu/ftdi.py` & `haicu-0.8.1/haicu/ftdi.py`

 * *Files identical despite different names*

### Comparing `haicu-0.8.0/haicu.egg-info/PKG-INFO` & `haicu-0.8.1/haicu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.8.0
+Version: 0.8.1
 Summary: package for HAICU
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

### Comparing `haicu-0.8.0/pyproject.toml` & `haicu-0.8.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "haicu"
 description = "package for HAICU"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
     { name = "Bryerton Shaw", email = "bryerton@triumf.ca" }
 ]
 maintainers = [
     { name = "Bryerton Shaw", email = "bryerton@triumf.ca" }
 ]
 readme.file = "README.md"
```

