# Comparing `tmp/notionshell-0.4.tar.gz` & `tmp/notionshell-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/notionshell-0.4.tar", last modified: Tue Apr 11 00:17:25 2023, max compression
+gzip compressed data, was "dist/notionshell-0.5.tar", last modified: Tue Apr 11 00:21:16 2023, max compression
```

## Comparing `notionshell-0.4.tar` & `notionshell-0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 tomwright   (501) staff       (20)        0 2023-04-11 00:17:25.000000 notionshell-0.4/
--rw-r--r--   0 tomwright   (501) staff       (20)     1793 2023-04-11 00:17:25.000000 notionshell-0.4/PKG-INFO
-drwxr-xr-x   0 tomwright   (501) staff       (20)        0 2023-04-11 00:17:25.000000 notionshell-0.4/notionshell.egg-info/
--rw-r--r--   0 tomwright   (501) staff       (20)     1793 2023-04-11 00:17:25.000000 notionshell-0.4/notionshell.egg-info/PKG-INFO
--rw-r--r--   0 tomwright   (501) staff       (20)      242 2023-04-11 00:17:25.000000 notionshell-0.4/notionshell.egg-info/SOURCES.txt
--rw-r--r--   0 tomwright   (501) staff       (20)       50 2023-04-11 00:17:25.000000 notionshell-0.4/notionshell.egg-info/entry_points.txt
--rw-r--r--   0 tomwright   (501) staff       (20)       14 2023-04-11 00:17:25.000000 notionshell-0.4/notionshell.egg-info/requires.txt
--rw-r--r--   0 tomwright   (501) staff       (20)        1 2023-04-11 00:17:25.000000 notionshell-0.4/notionshell.egg-info/top_level.txt
--rw-r--r--   0 tomwright   (501) staff       (20)        1 2023-04-11 00:17:25.000000 notionshell-0.4/notionshell.egg-info/dependency_links.txt
--rw-r--r--   0 tomwright   (501) staff       (20)       18 2023-04-11 00:14:00.000000 notionshell-0.4/MANIFEST.in
--rw-r--r--   0 tomwright   (501) staff       (20)     1226 2023-04-10 23:55:02.000000 notionshell-0.4/readme.md
--rw-r--r--   0 tomwright   (501) staff       (20)      539 2023-04-11 00:17:24.000000 notionshell-0.4/setup.py
--rw-r--r--   0 tomwright   (501) staff       (20)       38 2023-04-11 00:17:25.000000 notionshell-0.4/setup.cfg
+drwxr-xr-x   0 tomwright   (501) staff       (20)        0 2023-04-11 00:21:16.000000 notionshell-0.5/
+-rw-r--r--   0 tomwright   (501) staff       (20)     1793 2023-04-11 00:21:16.000000 notionshell-0.5/PKG-INFO
+-rw-r--r--   0 tomwright   (501) staff       (20)     3807 2023-04-11 00:00:20.000000 notionshell-0.5/notionshell.py
+drwxr-xr-x   0 tomwright   (501) staff       (20)        0 2023-04-11 00:21:16.000000 notionshell-0.5/notionshell.egg-info/
+-rw-r--r--   0 tomwright   (501) staff       (20)     1793 2023-04-11 00:21:16.000000 notionshell-0.5/notionshell.egg-info/PKG-INFO
+-rw-r--r--   0 tomwright   (501) staff       (20)      257 2023-04-11 00:21:16.000000 notionshell-0.5/notionshell.egg-info/SOURCES.txt
+-rw-r--r--   0 tomwright   (501) staff       (20)       50 2023-04-11 00:21:16.000000 notionshell-0.5/notionshell.egg-info/entry_points.txt
+-rw-r--r--   0 tomwright   (501) staff       (20)       14 2023-04-11 00:21:16.000000 notionshell-0.5/notionshell.egg-info/requires.txt
+-rw-r--r--   0 tomwright   (501) staff       (20)       12 2023-04-11 00:21:16.000000 notionshell-0.5/notionshell.egg-info/top_level.txt
+-rw-r--r--   0 tomwright   (501) staff       (20)        1 2023-04-11 00:21:16.000000 notionshell-0.5/notionshell.egg-info/dependency_links.txt
+-rw-r--r--   0 tomwright   (501) staff       (20)       18 2023-04-11 00:14:00.000000 notionshell-0.5/MANIFEST.in
+-rw-r--r--   0 tomwright   (501) staff       (20)     1226 2023-04-10 23:55:02.000000 notionshell-0.5/readme.md
+-rw-r--r--   0 tomwright   (501) staff       (20)      542 2023-04-11 00:21:14.000000 notionshell-0.5/setup.py
+-rw-r--r--   0 tomwright   (501) staff       (20)       38 2023-04-11 00:21:16.000000 notionshell-0.5/setup.cfg
```

### Comparing `notionshell-0.4/PKG-INFO` & `notionshell-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionshell
-Version: 0.4
+Version: 0.5
 Summary: Partial notion commad line. Introduction to api, using official library.
 Home-page: UNKNOWN
 Author: TalWrii
 Author-email: talwrii@gmail.com
 License: BSD
 Description: # notionshell
```

### Comparing `notionshell-0.4/notionshell.egg-info/PKG-INFO` & `notionshell-0.5/notionshell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionshell
-Version: 0.4
+Version: 0.5
 Summary: Partial notion commad line. Introduction to api, using official library.
 Home-page: UNKNOWN
 Author: TalWrii
 Author-email: talwrii@gmail.com
 License: BSD
 Description: # notionshell
```

### Comparing `notionshell-0.4/readme.md` & `notionshell-0.5/readme.md`

 * *Files identical despite different names*

### Comparing `notionshell-0.4/setup.py` & `notionshell-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 setuptools.setup(
     name="notionshell",
-    version=0.4,
+    version=0.5,
     author="TalWrii",
     long_description_content_type="text/markdown",
     author_email="talwrii@gmail.com",
     description=(
         "Partial notion commad line. Introduction to api, using official library."
     ),
     license="BSD",
-    modules=["notionshell"],
+    py_modules=["notionshell"],
     long_description=open("readme.md").read(),
     install_requires=["notion_client"],
     entry_points={"console_scripts": ["notionshell=notionshell:main"]},
     test_suite="nose.collector",
 )
```

