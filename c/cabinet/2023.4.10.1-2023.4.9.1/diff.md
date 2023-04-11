# Comparing `tmp/cabinet-2023.4.10.1.tar.gz` & `tmp/cabinet-2023.4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2023.4.10.1.tar", last modified: Tue Apr 11 01:21:26 2023, max compression
+gzip compressed data, was "cabinet-2023.4.9.1.tar", last modified: Mon Apr 10 04:09:49 2023, max compression
```

## Comparing `cabinet-2023.4.10.1.tar` & `cabinet-2023.4.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-11 01:21:26.822042 cabinet-2023.4.10.1/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.4.10.1/LICENSE
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     4366 2023-04-11 01:21:26.822042 cabinet-2023.4.10.1/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     4014 2023-03-25 22:04:50.000000 cabinet-2023.4.10.1/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.4.10.1/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-04-11 01:21:26.822042 cabinet-2023.4.10.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-11 01:21:26.818042 cabinet-2023.4.10.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-11 01:21:26.822042 cabinet-2023.4.10.1/src/cabinet/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    20789 2023-04-11 01:20:59.000000 cabinet-2023.4.10.1/src/cabinet/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-03-25 22:04:50.000000 cabinet-2023.4.10.1/src/cabinet/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2737 2023-03-25 22:04:50.000000 cabinet-2023.4.10.1/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-11 01:21:26.822042 cabinet-2023.4.10.1/src/cabinet.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     4366 2023-04-11 01:21:26.000000 cabinet-2023.4.10.1/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      288 2023-04-11 01:21:26.000000 cabinet-2023.4.10.1/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-04-11 01:21:26.000000 cabinet-2023.4.10.1/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-04-11 01:21:26.000000 cabinet-2023.4.10.1/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-04-11 01:21:26.000000 cabinet-2023.4.10.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.4.9.1/LICENSE
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4365 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4014 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.4.9.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/src/cabinet/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    20802 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/src/cabinet/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/src/cabinet/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2737 2023-03-25 22:04:50.000000 cabinet-2023.4.9.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-10 04:09:49.754821 cabinet-2023.4.9.1/src/cabinet.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4365 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      288 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-04-10 04:09:49.000000 cabinet-2023.4.9.1/src/cabinet.egg-info/top_level.txt
```

### Comparing `cabinet-2023.4.10.1/LICENSE` & `cabinet-2023.4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2023.4.10.1/PKG-INFO` & `cabinet-2023.4.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.4.10.1
+Version: 2023.4.9.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cabinet-2023.4.10.1/README.md` & `cabinet-2023.4.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cabinet-2023.4.10.1/setup.cfg` & `cabinet-2023.4.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2023.04.10.1
+version = 2023.04.09.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2023.4.10.1/src/cabinet/__init__.py` & `cabinet-2023.4.9.1/src/cabinet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,15 +425,15 @@
 
         with open(path_full, 'w+', encoding="utf8") as file:
             json.dump(_settings, file, indent=4)
 
         return value
 
     def get_file_as_array(self, item: str, file_path=None, strip: bool = True,
-                          ignore_not_found: bool = False):
+                          ignore_not_found: bool = False) -> list[str]:
         """
         Reads a file and returns its contents as a list of lines.
         The file is assumed to be encoded in UTF-8.
 
         Args:
             - item (str): The filename to read.
             - file_path (str, optional): The path to the directory containing the file.
```

### Comparing `cabinet-2023.4.10.1/src/cabinet/mail.py` & `cabinet-2023.4.9.1/src/cabinet/mail.py`

 * *Files identical despite different names*

### Comparing `cabinet-2023.4.10.1/src/cabinet.egg-info/PKG-INFO` & `cabinet-2023.4.9.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.4.10.1
+Version: 2023.4.9.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

