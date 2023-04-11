# Comparing `tmp/upyog-0.6.1.tar.gz` & `tmp/upyog-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upyog-0.6.1.tar", last modified: Mon Mar  6 08:33:51 2023, max compression
+gzip compressed data, was "upyog-0.6.2.tar", last modified: Tue Apr 11 17:05:12 2023, max compression
```

## Comparing `upyog-0.6.1.tar` & `upyog-0.6.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-03-06 08:33:51.480238 upyog-0.6.1/
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3011 2023-02-28 09:06:18.000000 upyog-0.6.1/CHANGELOG.md
--rw-r--r--   0 rahulsomani   (501) staff       (20)      133 2022-01-27 18:07:46.000000 upyog-0.6.1/MANIFEST.in
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-03-06 08:33:51.480340 upyog-0.6.1/PKG-INFO
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)      618 2022-01-15 04:03:41.000000 upyog-0.6.1/README.md
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-03-06 08:33:51.470977 upyog-0.6.1/assets/
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-03-06 08:33:51.472621 upyog-0.6.1/assets/fonts/
--rw-rwxrwx   0 rahulsomani   (501) staff       (20)    28432 2022-01-27 13:15:35.000000 upyog-0.6.1/assets/fonts/EuroStyleNormal.ttf
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)     1300 2023-03-06 08:33:51.480983 upyog-0.6.1/setup.cfg
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)      251 2022-01-17 09:53:10.000000 upyog-0.6.1/setup.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-03-06 08:33:51.473832 upyog-0.6.1/upyog/
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)       28 2022-10-28 02:44:32.000000 upyog-0.6.1/upyog/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      644 2023-01-24 04:50:27.000000 upyog-0.6.1/upyog/all.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-03-06 08:33:51.475719 upyog-0.6.1/upyog/ann/
--rw-r--r--   0 rahulsomani   (501) staff       (20)        0 2022-01-22 05:11:22.000000 upyog-0.6.1/upyog/ann/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     4426 2022-01-22 20:02:13.000000 upyog-0.6.1/upyog/ann/annoy.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3040 2023-01-31 06:04:25.000000 upyog-0.6.1/upyog/cli.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-03-06 08:33:51.477471 upyog-0.6.1/upyog/image/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      141 2022-09-04 09:39:14.000000 upyog-0.6.1/upyog/image/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3037 2022-01-19 13:36:07.000000 upyog-0.6.1/upyog/image/cli.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2286 2022-09-01 09:27:43.000000 upyog-0.6.1/upyog/image/composition.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)    17228 2023-03-06 08:32:51.000000 upyog-0.6.1/upyog/image/draw.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1305 2022-03-25 10:21:09.000000 upyog-0.6.1/upyog/image/io.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1442 2023-02-28 09:04:05.000000 upyog-0.6.1/upyog/image/pil_operators.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1159 2023-02-28 09:04:22.000000 upyog-0.6.1/upyog/image/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     7939 2023-02-28 09:16:20.000000 upyog-0.6.1/upyog/image/visualiser.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1102 2023-03-06 08:33:02.000000 upyog-0.6.1/upyog/imports.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1198 2022-06-01 05:03:09.000000 upyog-0.6.1/upyog/nb2script.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-03-06 08:33:51.478599 upyog-0.6.1/upyog/os/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      137 2022-10-26 00:24:39.000000 upyog-0.6.1/upyog/os/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     6238 2022-10-31 02:57:45.000000 upyog-0.6.1/upyog/os/cli.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-08-03 15:10:12.000000 upyog-0.6.1/upyog/os/patch_pathlib.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3356 2022-10-26 00:24:37.000000 upyog-0.6.1/upyog/os/read_files.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2917 2023-02-17 08:22:48.000000 upyog-0.6.1/upyog/os/utils.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-03-06 08:33:51.480058 upyog-0.6.1/upyog/utils/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      118 2022-10-28 03:18:43.000000 upyog-0.6.1/upyog/utils/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-04-05 12:59:08.000000 upyog-0.6.1/upyog/utils/boxes.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)    14495 2023-01-11 07:05:00.000000 upyog-0.6.1/upyog/utils/download.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1324 2023-01-12 17:22:00.000000 upyog-0.6.1/upyog/utils/prettify_df.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2992 2023-01-09 14:47:17.000000 upyog-0.6.1/upyog/utils/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      556 2022-08-08 14:04:02.000000 upyog-0.6.1/upyog/utils/zip_utils.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-03-06 08:33:51.475384 upyog-0.6.1/upyog.egg-info/
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-03-06 08:33:51.000000 upyog-0.6.1/upyog.egg-info/PKG-INFO
--rw-r--r--   0 rahulsomani   (501) staff       (20)      841 2023-03-06 08:33:51.000000 upyog-0.6.1/upyog.egg-info/SOURCES.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2023-03-06 08:33:51.000000 upyog-0.6.1/upyog.egg-info/dependency_links.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)      454 2023-03-06 08:33:51.000000 upyog-0.6.1/upyog.egg-info/entry_points.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2022-01-17 09:58:14.000000 upyog-0.6.1/upyog.egg-info/not-zip-safe
--rw-r--r--   0 rahulsomani   (501) staff       (20)      179 2023-03-06 08:33:51.000000 upyog-0.6.1/upyog.egg-info/requires.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)       12 2023-03-06 08:33:51.000000 upyog-0.6.1/upyog.egg-info/top_level.txt
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.692442 upyog-0.6.2/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3053 2023-04-11 17:04:59.000000 upyog-0.6.2/CHANGELOG.md
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      133 2022-01-27 18:07:46.000000 upyog-0.6.2/MANIFEST.in
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-04-11 17:05:12.692537 upyog-0.6.2/PKG-INFO
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)      618 2022-01-15 04:03:41.000000 upyog-0.6.2/README.md
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.686092 upyog-0.6.2/assets/
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.687449 upyog-0.6.2/assets/fonts/
+-rw-rwxrwx   0 rahulsomani   (501) staff       (20)    28432 2022-01-27 13:15:35.000000 upyog-0.6.2/assets/fonts/EuroStyleNormal.ttf
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)     1300 2023-04-11 17:05:12.692967 upyog-0.6.2/setup.cfg
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)      251 2022-01-17 09:53:10.000000 upyog-0.6.2/setup.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.688433 upyog-0.6.2/upyog/
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)       28 2022-10-28 02:44:32.000000 upyog-0.6.2/upyog/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      644 2023-01-24 04:50:27.000000 upyog-0.6.2/upyog/all.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.689791 upyog-0.6.2/upyog/ann/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        0 2022-01-22 05:11:22.000000 upyog-0.6.2/upyog/ann/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     4426 2022-01-22 20:02:13.000000 upyog-0.6.2/upyog/ann/annoy.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3040 2023-01-31 06:04:25.000000 upyog-0.6.2/upyog/cli.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.690908 upyog-0.6.2/upyog/image/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      141 2022-09-04 09:39:14.000000 upyog-0.6.2/upyog/image/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3037 2022-01-19 13:36:07.000000 upyog-0.6.2/upyog/image/cli.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2286 2022-09-01 09:27:43.000000 upyog-0.6.2/upyog/image/composition.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)    17228 2023-03-06 08:32:51.000000 upyog-0.6.2/upyog/image/draw.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1305 2022-03-25 10:21:09.000000 upyog-0.6.2/upyog/image/io.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1442 2023-02-28 09:04:05.000000 upyog-0.6.2/upyog/image/pil_operators.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1159 2023-02-28 09:04:22.000000 upyog-0.6.2/upyog/image/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     7939 2023-02-28 09:16:20.000000 upyog-0.6.2/upyog/image/visualiser.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1102 2023-03-06 08:33:02.000000 upyog-0.6.2/upyog/imports.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1198 2022-06-01 05:03:09.000000 upyog-0.6.2/upyog/nb2script.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.691554 upyog-0.6.2/upyog/os/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      137 2022-10-26 00:24:39.000000 upyog-0.6.2/upyog/os/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     6196 2023-04-11 16:53:41.000000 upyog-0.6.2/upyog/os/cli.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-08-03 15:10:12.000000 upyog-0.6.2/upyog/os/patch_pathlib.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3356 2022-10-26 00:24:37.000000 upyog-0.6.2/upyog/os/read_files.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3149 2023-04-11 16:54:06.000000 upyog-0.6.2/upyog/os/utils.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.692323 upyog-0.6.2/upyog/utils/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      118 2022-10-28 03:18:43.000000 upyog-0.6.2/upyog/utils/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-04-05 12:59:08.000000 upyog-0.6.2/upyog/utils/boxes.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)    14495 2023-01-11 07:05:00.000000 upyog-0.6.2/upyog/utils/download.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1324 2023-01-12 17:22:00.000000 upyog-0.6.2/upyog/utils/prettify_df.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2992 2023-01-09 14:47:17.000000 upyog-0.6.2/upyog/utils/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      556 2022-08-08 14:04:02.000000 upyog-0.6.2/upyog/utils/zip_utils.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-04-11 17:05:12.689540 upyog-0.6.2/upyog.egg-info/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-04-11 17:05:12.000000 upyog-0.6.2/upyog.egg-info/PKG-INFO
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      841 2023-04-11 17:05:12.000000 upyog-0.6.2/upyog.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2023-04-11 17:05:12.000000 upyog-0.6.2/upyog.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      454 2023-04-11 17:05:12.000000 upyog-0.6.2/upyog.egg-info/entry_points.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2022-01-17 09:58:14.000000 upyog-0.6.2/upyog.egg-info/not-zip-safe
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      179 2023-04-11 17:05:12.000000 upyog-0.6.2/upyog.egg-info/requires.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)       12 2023-04-11 17:05:12.000000 upyog-0.6.2/upyog.egg-info/top_level.txt
```

### Comparing `upyog-0.6.1/CHANGELOG.md` & `upyog-0.6.2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-## Unreleased
-* Fix default font path (hacky fix, but works)
+## 0.6.2 -- 11 Apr 2023
+* Myriad bugfixes
+
+## 0.6.1 -- 6 Mar 2023
+* Fix default font path (hacky but works)
 * Bugfix `write_json`
 * Add `title` func to `Visualiser`
-* Better error messages
+* Add `write_text`
 
-## 0.5.9 -- 31 January 2022
+## 0.5.9 -- 31 January 2023
 * `print_df` now accepts a dict as input also
 * Add `write_json`
 * cleaner imports in the `upyog.cli` module
 
 ## 0.5.8 -- 31 October 2022
 * Bugfixes
 * Simplify printing `pd.DataFrame` (not using `rich` anymore)
```

### Comparing `upyog-0.6.1/PKG-INFO` & `upyog-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upyog
-Version: 0.6.1
+Version: 0.6.2
 Summary: Myriad Utilities
 Author: Rahul Somani
 Author-email: rsomani95@gmail.com
 License: MIT
 Keywords: utilities
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `upyog-0.6.1/README.md` & `upyog-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/assets/fonts/EuroStyleNormal.ttf` & `upyog-0.6.2/assets/fonts/EuroStyleNormal.ttf`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/setup.cfg` & `upyog-0.6.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = upyog
-version = 0.6.1
+version = 0.6.2
 author = Rahul Somani
 author_email = rsomani95@gmail.com
 description = Myriad Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = utilities
 license = MIT
```

### Comparing `upyog-0.6.1/upyog/all.py` & `upyog-0.6.2/upyog/all.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/ann/annoy.py` & `upyog-0.6.2/upyog/ann/annoy.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/cli.py` & `upyog-0.6.2/upyog/cli.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/image/cli.py` & `upyog-0.6.2/upyog/image/cli.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/image/composition.py` & `upyog-0.6.2/upyog/image/composition.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/image/draw.py` & `upyog-0.6.2/upyog/image/draw.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/image/io.py` & `upyog-0.6.2/upyog/image/io.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/image/pil_operators.py` & `upyog-0.6.2/upyog/image/pil_operators.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/image/utils.py` & `upyog-0.6.2/upyog/image/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/image/visualiser.py` & `upyog-0.6.2/upyog/image/visualiser.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/imports.py` & `upyog-0.6.2/upyog/imports.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/nb2script.py` & `upyog-0.6.2/upyog/nb2script.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/os/cli.py` & `upyog-0.6.2/upyog/os/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,18 +193,16 @@
 
     for folder in parent_folders:
         freq = {}
         folder = Path(folder)
         for subdir in sorted(folder.list_dirs()):
             freq[subdir.name] = len(get_files(subdir, recurse=True))
 
-        # rich.print(f"----- {folder} -----\n")
-        # rich.print_json(data=freq)
-        # breakpoint()
-
         freq = pd.DataFrame([freq]).T.reset_index()
         freq.columns = ["Sub Folders", "Frequency"]
-        freq = print_df(freq, title = folder.name)
+        rich.print()
+        rich.print(f"---------- {folder.name.upper()} ----------")
+        freq = print_df(freq)
 
         results[folder.name] = freq
 
     return results
```

### Comparing `upyog-0.6.1/upyog/os/read_files.py` & `upyog-0.6.2/upyog/os/read_files.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/os/utils.py` & `upyog-0.6.2/upyog/os/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 from upyog.imports import *
 from upyog.os.read_files import PathLike, get_files
 
 __all__ = [
-    "load_json", "check_pil_simd_usage", "sanitise_filename", "get_file_size",
-    "get_file_creation_date", "write_json",
+    "load_json", "read_json", "check_pil_simd_usage", "sanitise_filename", "get_file_size",
+    "get_file_creation_date", "write_json", "write_text",
 ]
 
 
 def load_json(path: PathLike):
     "Load a JSON file"
     return json.loads(Path(path).read_bytes())
 
 
+def read_json(path: PathLike):
+    return load_json(path)
+
+
 def write_json(json_data: dict, path: PathLike, indent=4):
     "Write `json_data` to `path`"
     with open(path, "w") as f:
         json.dump(json_data, f, indent=indent)
 
 
+def write_text(text: str, save_path: PathLike):
+    "Write text to a text file"
+    with open(str(save_path), 'w') as f:
+        f.write(text)
+
+
 def check_pil_simd_usage():
     pil_version = PIL.__version__
 
     if not "post" in pil_version:
         msg = f"Pillow-SIMD not installed. Using PIL {pil_version} instead"
         warnings.warn(msg)
```

### Comparing `upyog-0.6.1/upyog/utils/download.py` & `upyog-0.6.2/upyog/utils/download.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/utils/prettify_df.py` & `upyog-0.6.2/upyog/utils/prettify_df.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/utils/utils.py` & `upyog-0.6.2/upyog/utils/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog/utils/zip_utils.py` & `upyog-0.6.2/upyog/utils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.6.1/upyog.egg-info/PKG-INFO` & `upyog-0.6.2/upyog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upyog
-Version: 0.6.1
+Version: 0.6.2
 Summary: Myriad Utilities
 Author: Rahul Somani
 Author-email: rsomani95@gmail.com
 License: MIT
 Keywords: utilities
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `upyog-0.6.1/upyog.egg-info/SOURCES.txt` & `upyog-0.6.2/upyog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

