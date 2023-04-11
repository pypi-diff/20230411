# Comparing `tmp/notionshell-0.3.tar.gz` & `tmp/notionshell-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/notionshell-0.3.tar", last modified: Tue Apr 11 00:14:13 2023, max compression
+gzip compressed data, was "dist/notionshell-0.4.tar", last modified: Tue Apr 11 00:17:25 2023, max compression
```

## Comparing `notionshell-0.3.tar` & `notionshell-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 tomwright   (501) staff       (20)        0 2023-04-11 00:14:13.000000 notionshell-0.3/
--rw-r--r--   0 tomwright   (501) staff       (20)     1793 2023-04-11 00:14:13.000000 notionshell-0.3/PKG-INFO
-drwxr-xr-x   0 tomwright   (501) staff       (20)        0 2023-04-11 00:14:13.000000 notionshell-0.3/notionshell.egg-info/
--rw-r--r--   0 tomwright   (501) staff       (20)     1793 2023-04-11 00:14:13.000000 notionshell-0.3/notionshell.egg-info/PKG-INFO
--rw-r--r--   0 tomwright   (501) staff       (20)      242 2023-04-11 00:14:13.000000 notionshell-0.3/notionshell.egg-info/SOURCES.txt
--rw-r--r--   0 tomwright   (501) staff       (20)       50 2023-04-11 00:14:13.000000 notionshell-0.3/notionshell.egg-info/entry_points.txt
--rw-r--r--   0 tomwright   (501) staff       (20)       14 2023-04-11 00:14:13.000000 notionshell-0.3/notionshell.egg-info/requires.txt
--rw-r--r--   0 tomwright   (501) staff       (20)        1 2023-04-11 00:14:13.000000 notionshell-0.3/notionshell.egg-info/top_level.txt
--rw-r--r--   0 tomwright   (501) staff       (20)        1 2023-04-11 00:14:13.000000 notionshell-0.3/notionshell.egg-info/dependency_links.txt
--rw-r--r--   0 tomwright   (501) staff       (20)       18 2023-04-11 00:14:00.000000 notionshell-0.3/MANIFEST.in
--rw-r--r--   0 tomwright   (501) staff       (20)     1226 2023-04-10 23:55:02.000000 notionshell-0.3/readme.md
--rw-r--r--   0 tomwright   (501) staff       (20)      510 2023-04-11 00:14:08.000000 notionshell-0.3/setup.py
--rw-r--r--   0 tomwright   (501) staff       (20)       38 2023-04-11 00:14:13.000000 notionshell-0.3/setup.cfg
+drwxr-xr-x   0 tomwright   (501) staff       (20)        0 2023-04-11 00:17:25.000000 notionshell-0.4/
+-rw-r--r--   0 tomwright   (501) staff       (20)     1793 2023-04-11 00:17:25.000000 notionshell-0.4/PKG-INFO
+drwxr-xr-x   0 tomwright   (501) staff       (20)        0 2023-04-11 00:17:25.000000 notionshell-0.4/notionshell.egg-info/
+-rw-r--r--   0 tomwright   (501) staff       (20)     1793 2023-04-11 00:17:25.000000 notionshell-0.4/notionshell.egg-info/PKG-INFO
+-rw-r--r--   0 tomwright   (501) staff       (20)      242 2023-04-11 00:17:25.000000 notionshell-0.4/notionshell.egg-info/SOURCES.txt
+-rw-r--r--   0 tomwright   (501) staff       (20)       50 2023-04-11 00:17:25.000000 notionshell-0.4/notionshell.egg-info/entry_points.txt
+-rw-r--r--   0 tomwright   (501) staff       (20)       14 2023-04-11 00:17:25.000000 notionshell-0.4/notionshell.egg-info/requires.txt
+-rw-r--r--   0 tomwright   (501) staff       (20)        1 2023-04-11 00:17:25.000000 notionshell-0.4/notionshell.egg-info/top_level.txt
+-rw-r--r--   0 tomwright   (501) staff       (20)        1 2023-04-11 00:17:25.000000 notionshell-0.4/notionshell.egg-info/dependency_links.txt
+-rw-r--r--   0 tomwright   (501) staff       (20)       18 2023-04-11 00:14:00.000000 notionshell-0.4/MANIFEST.in
+-rw-r--r--   0 tomwright   (501) staff       (20)     1226 2023-04-10 23:55:02.000000 notionshell-0.4/readme.md
+-rw-r--r--   0 tomwright   (501) staff       (20)      539 2023-04-11 00:17:24.000000 notionshell-0.4/setup.py
+-rw-r--r--   0 tomwright   (501) staff       (20)       38 2023-04-11 00:17:25.000000 notionshell-0.4/setup.cfg
```

### Comparing `notionshell-0.3/PKG-INFO` & `notionshell-0.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionshell
-Version: 0.3
+Version: 0.4
 Summary: Partial notion commad line. Introduction to api, using official library.
 Home-page: UNKNOWN
 Author: TalWrii
 Author-email: talwrii@gmail.com
 License: BSD
 Description: # notionshell
```

### Comparing `notionshell-0.3/notionshell.egg-info/PKG-INFO` & `notionshell-0.4/notionshell.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionshell
-Version: 0.3
+Version: 0.4
 Summary: Partial notion commad line. Introduction to api, using official library.
 Home-page: UNKNOWN
 Author: TalWrii
 Author-email: talwrii@gmail.com
 License: BSD
 Description: # notionshell
```

### Comparing `notionshell-0.3/readme.md` & `notionshell-0.4/readme.md`

 * *Files identical despite different names*

