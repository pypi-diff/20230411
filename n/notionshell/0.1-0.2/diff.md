# Comparing `tmp/notionshell-0.1.tar.gz` & `tmp/notionshell-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/notionshell-0.1.tar", last modified: Tue Apr 11 00:04:22 2023, max compression
+gzip compressed data, was "dist/notionshell-0.2.tar", last modified: Tue Apr 11 00:13:13 2023, max compression
```

## Comparing `notionshell-0.1.tar` & `notionshell-0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 tomwright   (501) staff       (20)        0 2023-04-11 00:04:22.000000 notionshell-0.1/
--rw-r--r--   0 tomwright   (501) staff       (20)     1793 2023-04-11 00:04:22.000000 notionshell-0.1/PKG-INFO
-drwxr-xr-x   0 tomwright   (501) staff       (20)        0 2023-04-11 00:04:22.000000 notionshell-0.1/notionshell.egg-info/
--rw-r--r--   0 tomwright   (501) staff       (20)     1793 2023-04-11 00:04:22.000000 notionshell-0.1/notionshell.egg-info/PKG-INFO
--rw-r--r--   0 tomwright   (501) staff       (20)      220 2023-04-11 00:04:22.000000 notionshell-0.1/notionshell.egg-info/SOURCES.txt
--rw-r--r--   0 tomwright   (501) staff       (20)       50 2023-04-11 00:04:22.000000 notionshell-0.1/notionshell.egg-info/entry_points.txt
--rw-r--r--   0 tomwright   (501) staff       (20)       14 2023-04-11 00:04:22.000000 notionshell-0.1/notionshell.egg-info/requires.txt
--rw-r--r--   0 tomwright   (501) staff       (20)        1 2023-04-11 00:04:22.000000 notionshell-0.1/notionshell.egg-info/top_level.txt
--rw-r--r--   0 tomwright   (501) staff       (20)        1 2023-04-11 00:04:22.000000 notionshell-0.1/notionshell.egg-info/dependency_links.txt
--rw-r--r--   0 tomwright   (501) staff       (20)      510 2023-04-11 00:03:55.000000 notionshell-0.1/setup.py
--rw-r--r--   0 tomwright   (501) staff       (20)       38 2023-04-11 00:04:22.000000 notionshell-0.1/setup.cfg
+drwxr-xr-x   0 tomwright   (501) staff       (20)        0 2023-04-11 00:13:13.000000 notionshell-0.2/
+-rw-r--r--   0 tomwright   (501) staff       (20)     1793 2023-04-11 00:13:13.000000 notionshell-0.2/PKG-INFO
+drwxr-xr-x   0 tomwright   (501) staff       (20)        0 2023-04-11 00:13:13.000000 notionshell-0.2/notionshell.egg-info/
+-rw-r--r--   0 tomwright   (501) staff       (20)     1793 2023-04-11 00:13:13.000000 notionshell-0.2/notionshell.egg-info/PKG-INFO
+-rw-r--r--   0 tomwright   (501) staff       (20)      232 2023-04-11 00:13:13.000000 notionshell-0.2/notionshell.egg-info/SOURCES.txt
+-rw-r--r--   0 tomwright   (501) staff       (20)       50 2023-04-11 00:13:13.000000 notionshell-0.2/notionshell.egg-info/entry_points.txt
+-rw-r--r--   0 tomwright   (501) staff       (20)       14 2023-04-11 00:13:13.000000 notionshell-0.2/notionshell.egg-info/requires.txt
+-rw-r--r--   0 tomwright   (501) staff       (20)        1 2023-04-11 00:13:13.000000 notionshell-0.2/notionshell.egg-info/top_level.txt
+-rw-r--r--   0 tomwright   (501) staff       (20)        1 2023-04-11 00:13:13.000000 notionshell-0.2/notionshell.egg-info/dependency_links.txt
+-rw-r--r--   0 tomwright   (501) staff       (20)       10 2023-04-11 00:11:38.000000 notionshell-0.2/MANIFEST.in
+-rw-r--r--   0 tomwright   (501) staff       (20)      510 2023-04-11 00:13:04.000000 notionshell-0.2/setup.py
+-rw-r--r--   0 tomwright   (501) staff       (20)       38 2023-04-11 00:13:13.000000 notionshell-0.2/setup.cfg
```

### Comparing `notionshell-0.1/PKG-INFO` & `notionshell-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionshell
-Version: 0.1
+Version: 0.2
 Summary: Partial notion commad line. Introduction to api, using official library.
 Home-page: UNKNOWN
 Author: TalWrii
 Author-email: talwrii@gmail.com
 License: BSD
 Description: # notionshell
```

### Comparing `notionshell-0.1/notionshell.egg-info/PKG-INFO` & `notionshell-0.2/notionshell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionshell
-Version: 0.1
+Version: 0.2
 Summary: Partial notion commad line. Introduction to api, using official library.
 Home-page: UNKNOWN
 Author: TalWrii
 Author-email: talwrii@gmail.com
 License: BSD
 Description: # notionshell
```

