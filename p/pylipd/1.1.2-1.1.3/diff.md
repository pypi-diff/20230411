# Comparing `tmp/pylipd-1.1.2.tar.gz` & `tmp/pylipd-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylipd-1.1.2.tar", last modified: Tue Apr 11 02:52:29 2023, max compression
+gzip compressed data, was "pylipd-1.1.3.tar", last modified: Tue Apr 11 02:59:59 2023, max compression
```

## Comparing `pylipd-1.1.2.tar` & `pylipd-1.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:52:29.124323 pylipd-1.1.2/
--rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.1.2/LICENSE
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 02:52:29.124405 pylipd-1.1.2/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.1.2/README.md
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:52:29.121569 pylipd-1.1.2/pylipd/
--rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-11 02:50:24.000000 pylipd-1.1.2/pylipd/__init__.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:52:29.122435 pylipd-1.1.2/pylipd/globals/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.1.2/pylipd/globals/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)      409 2023-04-10 19:03:17.000000 pylipd-1.1.2/pylipd/globals/blacklist.py
--rw-r--r--   0 varun      (502) staff       (20)    14643 2023-04-10 19:06:28.000000 pylipd-1.1.2/pylipd/globals/schema.py
--rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.1.2/pylipd/globals/urls.py
--rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.1.2/pylipd/legacy_utils.py
--rw-r--r--   0 varun      (502) staff       (20)    31780 2023-04-11 02:51:38.000000 pylipd-1.1.2/pylipd/lipd.py
--rw-r--r--   0 varun      (502) staff       (20)    43704 2023-04-10 19:04:22.000000 pylipd-1.1.2/pylipd/lipd_to_rdf.py
--rw-r--r--   0 varun      (502) staff       (20)     1742 2023-04-07 05:39:21.000000 pylipd-1.1.2/pylipd/multi_processing.py
--rw-r--r--   0 varun      (502) staff       (20)    22294 2023-04-10 19:05:37.000000 pylipd-1.1.2/pylipd/rdf_to_lipd.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:52:29.122874 pylipd-1.1.2/pylipd/series/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.1.2/pylipd/series/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.1.2/pylipd/series/regexes.py
--rw-r--r--   0 varun      (502) staff       (20)     2270 2023-03-22 17:52:14.000000 pylipd-1.1.2/pylipd/test.py
--rw-r--r--   0 varun      (502) staff       (20)     5054 2023-04-10 12:38:55.000000 pylipd-1.1.2/pylipd/usage.py
--rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.1.2/pylipd/utils.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:52:29.124191 pylipd-1.1.2/pylipd.egg-info/
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 02:52:29.000000 pylipd-1.1.2/pylipd.egg-info/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      588 2023-04-11 02:52:29.000000 pylipd-1.1.2/pylipd.egg-info/SOURCES.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-11 02:52:29.000000 pylipd-1.1.2/pylipd.egg-info/dependency_links.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.1.2/pylipd.egg-info/not-zip-safe
--rw-r--r--   0 varun      (502) staff       (20)       35 2023-04-11 02:52:29.000000 pylipd-1.1.2/pylipd.egg-info/requires.txt
--rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-11 02:52:29.000000 pylipd-1.1.2/pylipd.egg-info/top_level.txt
--rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.1.2/pyproject.toml
--rw-r--r--   0 varun      (502) staff       (20)      693 2023-04-11 02:52:29.124739 pylipd-1.1.2/setup.cfg
--rw-r--r--   0 varun      (502) staff       (20)      973 2023-04-11 02:50:17.000000 pylipd-1.1.2/setup.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:59:59.695376 pylipd-1.1.3/
+-rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.1.3/LICENSE
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 02:59:59.695453 pylipd-1.1.3/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.1.3/README.md
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:59:59.692352 pylipd-1.1.3/pylipd/
+-rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-11 02:59:51.000000 pylipd-1.1.3/pylipd/__init__.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:59:59.693524 pylipd-1.1.3/pylipd/globals/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.1.3/pylipd/globals/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)      409 2023-04-10 19:03:17.000000 pylipd-1.1.3/pylipd/globals/blacklist.py
+-rw-r--r--   0 varun      (502) staff       (20)    14643 2023-04-10 19:06:28.000000 pylipd-1.1.3/pylipd/globals/schema.py
+-rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.1.3/pylipd/globals/urls.py
+-rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.1.3/pylipd/legacy_utils.py
+-rw-r--r--   0 varun      (502) staff       (20)    31680 2023-04-11 02:59:29.000000 pylipd-1.1.3/pylipd/lipd.py
+-rw-r--r--   0 varun      (502) staff       (20)    43704 2023-04-10 19:04:22.000000 pylipd-1.1.3/pylipd/lipd_to_rdf.py
+-rw-r--r--   0 varun      (502) staff       (20)     1742 2023-04-07 05:39:21.000000 pylipd-1.1.3/pylipd/multi_processing.py
+-rw-r--r--   0 varun      (502) staff       (20)    22294 2023-04-10 19:05:37.000000 pylipd-1.1.3/pylipd/rdf_to_lipd.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:59:59.693970 pylipd-1.1.3/pylipd/series/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.1.3/pylipd/series/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.1.3/pylipd/series/regexes.py
+-rw-r--r--   0 varun      (502) staff       (20)     2270 2023-03-22 17:52:14.000000 pylipd-1.1.3/pylipd/test.py
+-rw-r--r--   0 varun      (502) staff       (20)     5054 2023-04-10 12:38:55.000000 pylipd-1.1.3/pylipd/usage.py
+-rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.1.3/pylipd/utils.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:59:59.695247 pylipd-1.1.3/pylipd.egg-info/
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 02:59:59.000000 pylipd-1.1.3/pylipd.egg-info/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      588 2023-04-11 02:59:59.000000 pylipd-1.1.3/pylipd.egg-info/SOURCES.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-11 02:59:59.000000 pylipd-1.1.3/pylipd.egg-info/dependency_links.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.1.3/pylipd.egg-info/not-zip-safe
+-rw-r--r--   0 varun      (502) staff       (20)       35 2023-04-11 02:59:59.000000 pylipd-1.1.3/pylipd.egg-info/requires.txt
+-rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-11 02:59:59.000000 pylipd-1.1.3/pylipd.egg-info/top_level.txt
+-rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.1.3/pyproject.toml
+-rw-r--r--   0 varun      (502) staff       (20)      693 2023-04-11 02:59:59.695764 pylipd-1.1.3/setup.cfg
+-rw-r--r--   0 varun      (502) staff       (20)      973 2023-04-11 02:59:45.000000 pylipd-1.1.3/setup.py
```

### Comparing `pylipd-1.1.2/LICENSE` & `pylipd-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.2/PKG-INFO` & `pylipd-1.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.2
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.3
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.1.2/README.md` & `pylipd-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.2/pylipd/globals/schema.py` & `pylipd-1.1.3/pylipd/globals/schema.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.2/pylipd/legacy_utils.py` & `pylipd-1.1.3/pylipd/legacy_utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.2/pylipd/lipd.py` & `pylipd-1.1.3/pylipd/lipd.py`

 * *Files 1% similar despite different names*

```diff
@@ -674,19 +674,19 @@
         .. ipython:: python
             :okwarning:
             :okexcept:
 
             from pylipd.lipd import LiPD
 
             # Fetch LiPD data from remote RDF Graph
-            lipd_remote = LiPD()
-            lipd_remote.set_endpoint("https://linkedearth.graphdb.mint.isi.edu/repositories/LiPDVerse2")
-            dsname = "Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001"
-            lipd_remote.load_remote_datasets([dsname])
-            lipd_json = lipd_remote.get_lipd(dsname)
+            lipd = LiPD()
+            lipd.load([
+                "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
+            ])
+            lipd_json = lipd.get_lipd(lipd.get_all_dataset_names()[0])
             print(lipd_json)
         '''           
         converter = RDFToLiPD(self.graph)
         return converter.convert_to_json(dsname, lipdfile)
 
     def create_lipd(self, dsname, lipdfile):
         '''Create LiPD file for a dataset
@@ -711,15 +711,15 @@
 
             # Fetch LiPD data from remote RDF Graph
             lipd = LiPD()
             lipd.load([
                 "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
             ])
             dsname = lipd.get_all_dataset_names()[0]
-            lipd_remote.create_lipd(dsname, "test.lpd")
+            lipd.create_lipd(dsname, "test.lpd")
         '''           
         converter = RDFToLiPD(self.graph)
         return converter.convert(dsname, lipdfile)
     
     def pop(self, dsnames=None, collection_id=None):
         '''Removes a dataset from the graph and returns a LiPD object
```

### Comparing `pylipd-1.1.2/pylipd/lipd_to_rdf.py` & `pylipd-1.1.3/pylipd/lipd_to_rdf.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.2/pylipd/multi_processing.py` & `pylipd-1.1.3/pylipd/multi_processing.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.2/pylipd/rdf_to_lipd.py` & `pylipd-1.1.3/pylipd/rdf_to_lipd.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.2/pylipd/series/regexes.py` & `pylipd-1.1.3/pylipd/series/regexes.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.2/pylipd/test.py` & `pylipd-1.1.3/pylipd/test.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.2/pylipd/usage.py` & `pylipd-1.1.3/pylipd/usage.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.2/pylipd/utils.py` & `pylipd-1.1.3/pylipd/utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.2/pylipd.egg-info/PKG-INFO` & `pylipd-1.1.3/pylipd.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.2
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.3
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.1.2/pylipd.egg-info/SOURCES.txt` & `pylipd-1.1.3/pylipd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.2/setup.cfg` & `pylipd-1.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pylipd
-version = 1.1.2
+version = 1.1.3
 author = Varun Ratnakar
 author_email = varunratnakar@gmail.com
 description = Python utilities for handling LiPD data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/linkedearth/pylipd
 project_urls =
```

### Comparing `pylipd-1.1.2/setup.py` & `pylipd-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import setup, find_packages
 
 
-version = '1.1.2'
+version = '1.1.3'
 
 # Read the readme file contents into variable
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='pylipd',
```

