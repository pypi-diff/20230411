# Comparing `tmp/pylipd-1.2.3.tar.gz` & `tmp/pylipd-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylipd-1.2.3.tar", last modified: Tue Apr 11 07:07:13 2023, max compression
+gzip compressed data, was "pylipd-1.2.4.tar", last modified: Tue Apr 11 10:36:03 2023, max compression
```

## Comparing `pylipd-1.2.3.tar` & `pylipd-1.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 07:07:13.199609 pylipd-1.2.3/
--rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.2.3/LICENSE
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 07:07:13.199679 pylipd-1.2.3/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.2.3/README.md
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 07:07:13.196797 pylipd-1.2.3/pylipd/
--rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-11 07:06:44.000000 pylipd-1.2.3/pylipd/__init__.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 07:07:13.198026 pylipd-1.2.3/pylipd/globals/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.2.3/pylipd/globals/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)      409 2023-04-10 19:03:17.000000 pylipd-1.2.3/pylipd/globals/blacklist.py
--rw-r--r--   0 varun      (502) staff       (20)     3673 2023-04-11 06:17:21.000000 pylipd-1.2.3/pylipd/globals/queries.py
--rw-r--r--   0 varun      (502) staff       (20)    14643 2023-04-10 19:06:28.000000 pylipd-1.2.3/pylipd/globals/schema.py
--rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.2.3/pylipd/globals/urls.py
--rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.2.3/pylipd/legacy_utils.py
--rw-r--r--   0 varun      (502) staff       (20)    30860 2023-04-11 07:06:17.000000 pylipd-1.2.3/pylipd/lipd.py
--rw-r--r--   0 varun      (502) staff       (20)    43172 2023-04-11 03:12:51.000000 pylipd-1.2.3/pylipd/lipd_to_rdf.py
--rw-r--r--   0 varun      (502) staff       (20)     1576 2023-04-11 03:11:49.000000 pylipd-1.2.3/pylipd/multi_processing.py
--rw-r--r--   0 varun      (502) staff       (20)    22021 2023-04-11 03:13:16.000000 pylipd-1.2.3/pylipd/rdf_to_lipd.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 07:07:13.198453 pylipd-1.2.3/pylipd/series/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.2.3/pylipd/series/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.2.3/pylipd/series/regexes.py
--rw-r--r--   0 varun      (502) staff       (20)     2259 2023-04-11 05:52:03.000000 pylipd-1.2.3/pylipd/test.py
--rw-r--r--   0 varun      (502) staff       (20)     5306 2023-04-11 06:31:14.000000 pylipd-1.2.3/pylipd/usage.py
--rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.2.3/pylipd/utils.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 07:07:13.199504 pylipd-1.2.3/pylipd.egg-info/
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 07:07:13.000000 pylipd-1.2.3/pylipd.egg-info/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      616 2023-04-11 07:07:13.000000 pylipd-1.2.3/pylipd.egg-info/SOURCES.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-11 07:07:13.000000 pylipd-1.2.3/pylipd.egg-info/dependency_links.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.2.3/pylipd.egg-info/not-zip-safe
--rw-r--r--   0 varun      (502) staff       (20)       35 2023-04-11 07:07:13.000000 pylipd-1.2.3/pylipd.egg-info/requires.txt
--rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-11 07:07:13.000000 pylipd-1.2.3/pylipd.egg-info/top_level.txt
--rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.2.3/pyproject.toml
--rw-r--r--   0 varun      (502) staff       (20)      693 2023-04-11 07:07:13.199935 pylipd-1.2.3/setup.cfg
--rw-r--r--   0 varun      (502) staff       (20)      973 2023-04-11 07:06:34.000000 pylipd-1.2.3/setup.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 10:36:03.443864 pylipd-1.2.4/
+-rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.2.4/LICENSE
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 10:36:03.443935 pylipd-1.2.4/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.2.4/README.md
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 10:36:03.441003 pylipd-1.2.4/pylipd/
+-rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-11 10:33:50.000000 pylipd-1.2.4/pylipd/__init__.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 10:36:03.442242 pylipd-1.2.4/pylipd/globals/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.2.4/pylipd/globals/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)      409 2023-04-10 19:03:17.000000 pylipd-1.2.4/pylipd/globals/blacklist.py
+-rw-r--r--   0 varun      (502) staff       (20)     3673 2023-04-11 06:17:21.000000 pylipd-1.2.4/pylipd/globals/queries.py
+-rw-r--r--   0 varun      (502) staff       (20)    14643 2023-04-10 19:06:28.000000 pylipd-1.2.4/pylipd/globals/schema.py
+-rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.2.4/pylipd/globals/urls.py
+-rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.2.4/pylipd/legacy_utils.py
+-rw-r--r--   0 varun      (502) staff       (20)    30850 2023-04-11 10:33:34.000000 pylipd-1.2.4/pylipd/lipd.py
+-rw-r--r--   0 varun      (502) staff       (20)    43172 2023-04-11 03:12:51.000000 pylipd-1.2.4/pylipd/lipd_to_rdf.py
+-rw-r--r--   0 varun      (502) staff       (20)     1576 2023-04-11 03:11:49.000000 pylipd-1.2.4/pylipd/multi_processing.py
+-rw-r--r--   0 varun      (502) staff       (20)    22021 2023-04-11 03:13:16.000000 pylipd-1.2.4/pylipd/rdf_to_lipd.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 10:36:03.442579 pylipd-1.2.4/pylipd/series/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.2.4/pylipd/series/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.2.4/pylipd/series/regexes.py
+-rw-r--r--   0 varun      (502) staff       (20)     2259 2023-04-11 05:52:03.000000 pylipd-1.2.4/pylipd/test.py
+-rw-r--r--   0 varun      (502) staff       (20)     5306 2023-04-11 06:31:14.000000 pylipd-1.2.4/pylipd/usage.py
+-rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.2.4/pylipd/utils.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 10:36:03.443742 pylipd-1.2.4/pylipd.egg-info/
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 10:36:03.000000 pylipd-1.2.4/pylipd.egg-info/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      616 2023-04-11 10:36:03.000000 pylipd-1.2.4/pylipd.egg-info/SOURCES.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-11 10:36:03.000000 pylipd-1.2.4/pylipd.egg-info/dependency_links.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.2.4/pylipd.egg-info/not-zip-safe
+-rw-r--r--   0 varun      (502) staff       (20)       35 2023-04-11 10:36:03.000000 pylipd-1.2.4/pylipd.egg-info/requires.txt
+-rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-11 10:36:03.000000 pylipd-1.2.4/pylipd.egg-info/top_level.txt
+-rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.2.4/pyproject.toml
+-rw-r--r--   0 varun      (502) staff       (20)      693 2023-04-11 10:36:03.444295 pylipd-1.2.4/setup.cfg
+-rw-r--r--   0 varun      (502) staff       (20)      973 2023-04-11 10:33:44.000000 pylipd-1.2.4/setup.py
```

### Comparing `pylipd-1.2.3/LICENSE` & `pylipd-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.3/PKG-INFO` & `pylipd-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.2.3
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.2.4
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.2.3/README.md` & `pylipd-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.3/pylipd/globals/queries.py` & `pylipd-1.2.4/pylipd/globals/queries.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.3/pylipd/globals/schema.py` & `pylipd-1.2.4/pylipd/globals/schema.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.3/pylipd/legacy_utils.py` & `pylipd-1.2.4/pylipd/legacy_utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.3/pylipd/lipd.py` & `pylipd-1.2.4/pylipd/lipd.py`

 * *Files 0% similar despite different names*

```diff
@@ -653,15 +653,15 @@
             lipd.load([
                 "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
             ])
             lipd_json = lipd.get_lipd(lipd.get_all_dataset_names()[0])
             print(lipd_json)
         '''           
         converter = RDFToLiPD(self.graph)
-        return converter.convert_to_json(dsname, lipdfile)
+        return converter.convert_to_json(dsname)
 
     def create_lipd(self, dsname, lipdfile):
         '''Create LiPD file for a dataset
 
         Parameters
         ----------
```

### Comparing `pylipd-1.2.3/pylipd/lipd_to_rdf.py` & `pylipd-1.2.4/pylipd/lipd_to_rdf.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.3/pylipd/multi_processing.py` & `pylipd-1.2.4/pylipd/multi_processing.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.3/pylipd/rdf_to_lipd.py` & `pylipd-1.2.4/pylipd/rdf_to_lipd.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.3/pylipd/series/regexes.py` & `pylipd-1.2.4/pylipd/series/regexes.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.3/pylipd/test.py` & `pylipd-1.2.4/pylipd/test.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.3/pylipd/usage.py` & `pylipd-1.2.4/pylipd/usage.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.3/pylipd/utils.py` & `pylipd-1.2.4/pylipd/utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.3/pylipd.egg-info/PKG-INFO` & `pylipd-1.2.4/pylipd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.2.3
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.2.4
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.2.3/pylipd.egg-info/SOURCES.txt` & `pylipd-1.2.4/pylipd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.3/setup.cfg` & `pylipd-1.2.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pylipd
-version = 1.2.3
+version = 1.2.4
 author = Varun Ratnakar
 author_email = varunratnakar@gmail.com
 description = Python utilities for handling LiPD data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/linkedearth/pylipd
 project_urls =
```

### Comparing `pylipd-1.2.3/setup.py` & `pylipd-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import setup, find_packages
 
 
-version = '1.2.3'
+version = '1.2.4'
 
 # Read the readme file contents into variable
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='pylipd',
```

