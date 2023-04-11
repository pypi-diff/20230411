# Comparing `tmp/pylipd-1.1.0.tar.gz` & `tmp/pylipd-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylipd-1.1.0.tar", last modified: Mon Apr 10 19:07:34 2023, max compression
+gzip compressed data, was "pylipd-1.1.1.tar", last modified: Tue Apr 11 02:44:06 2023, max compression
```

## Comparing `pylipd-1.1.0.tar` & `pylipd-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-10 19:07:34.477273 pylipd-1.1.0/
--rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.1.0/LICENSE
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-10 19:07:34.477335 pylipd-1.1.0/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.1.0/README.md
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-10 19:07:34.474853 pylipd-1.1.0/pylipd/
--rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-10 12:31:16.000000 pylipd-1.1.0/pylipd/__init__.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-10 19:07:34.475643 pylipd-1.1.0/pylipd/globals/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.1.0/pylipd/globals/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)      409 2023-04-10 19:03:17.000000 pylipd-1.1.0/pylipd/globals/blacklist.py
--rw-r--r--   0 varun      (502) staff       (20)    14643 2023-04-10 19:06:28.000000 pylipd-1.1.0/pylipd/globals/schema.py
--rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.1.0/pylipd/globals/urls.py
--rw-r--r--   0 varun      (502) staff       (20)    15901 2023-04-10 05:47:05.000000 pylipd-1.1.0/pylipd/legacy_utils.py
--rw-r--r--   0 varun      (502) staff       (20)    30545 2023-04-10 07:14:07.000000 pylipd-1.1.0/pylipd/lipd.py
--rw-r--r--   0 varun      (502) staff       (20)    43704 2023-04-10 19:04:22.000000 pylipd-1.1.0/pylipd/lipd_to_rdf.py
--rw-r--r--   0 varun      (502) staff       (20)     1742 2023-04-07 05:39:21.000000 pylipd-1.1.0/pylipd/multi_processing.py
--rw-r--r--   0 varun      (502) staff       (20)    22294 2023-04-10 19:05:37.000000 pylipd-1.1.0/pylipd/rdf_to_lipd.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-10 19:07:34.475994 pylipd-1.1.0/pylipd/series/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.1.0/pylipd/series/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.1.0/pylipd/series/regexes.py
--rw-r--r--   0 varun      (502) staff       (20)     2270 2023-03-22 17:52:14.000000 pylipd-1.1.0/pylipd/test.py
--rw-r--r--   0 varun      (502) staff       (20)     5054 2023-04-10 12:38:55.000000 pylipd-1.1.0/pylipd/usage.py
--rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.1.0/pylipd/utils.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-10 19:07:34.477177 pylipd-1.1.0/pylipd.egg-info/
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-10 19:07:34.000000 pylipd-1.1.0/pylipd.egg-info/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      588 2023-04-10 19:07:34.000000 pylipd-1.1.0/pylipd.egg-info/SOURCES.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-10 19:07:34.000000 pylipd-1.1.0/pylipd.egg-info/dependency_links.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.1.0/pylipd.egg-info/not-zip-safe
--rw-r--r--   0 varun      (502) staff       (20)       35 2023-04-10 19:07:34.000000 pylipd-1.1.0/pylipd.egg-info/requires.txt
--rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-10 19:07:34.000000 pylipd-1.1.0/pylipd.egg-info/top_level.txt
--rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.1.0/pyproject.toml
--rw-r--r--   0 varun      (502) staff       (20)      693 2023-04-10 19:07:34.477604 pylipd-1.1.0/setup.cfg
--rw-r--r--   0 varun      (502) staff       (20)      973 2023-04-10 12:31:07.000000 pylipd-1.1.0/setup.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:44:06.418621 pylipd-1.1.1/
+-rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.1.1/LICENSE
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 02:44:06.418670 pylipd-1.1.1/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.1.1/README.md
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:44:06.416421 pylipd-1.1.1/pylipd/
+-rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-11 02:43:37.000000 pylipd-1.1.1/pylipd/__init__.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:44:06.417277 pylipd-1.1.1/pylipd/globals/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.1.1/pylipd/globals/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)      409 2023-04-10 19:03:17.000000 pylipd-1.1.1/pylipd/globals/blacklist.py
+-rw-r--r--   0 varun      (502) staff       (20)    14643 2023-04-10 19:06:28.000000 pylipd-1.1.1/pylipd/globals/schema.py
+-rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.1.1/pylipd/globals/urls.py
+-rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.1.1/pylipd/legacy_utils.py
+-rw-r--r--   0 varun      (502) staff       (20)    30758 2023-04-11 02:42:48.000000 pylipd-1.1.1/pylipd/lipd.py
+-rw-r--r--   0 varun      (502) staff       (20)    43704 2023-04-10 19:04:22.000000 pylipd-1.1.1/pylipd/lipd_to_rdf.py
+-rw-r--r--   0 varun      (502) staff       (20)     1742 2023-04-07 05:39:21.000000 pylipd-1.1.1/pylipd/multi_processing.py
+-rw-r--r--   0 varun      (502) staff       (20)    22294 2023-04-10 19:05:37.000000 pylipd-1.1.1/pylipd/rdf_to_lipd.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:44:06.417612 pylipd-1.1.1/pylipd/series/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.1.1/pylipd/series/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.1.1/pylipd/series/regexes.py
+-rw-r--r--   0 varun      (502) staff       (20)     2270 2023-03-22 17:52:14.000000 pylipd-1.1.1/pylipd/test.py
+-rw-r--r--   0 varun      (502) staff       (20)     5054 2023-04-10 12:38:55.000000 pylipd-1.1.1/pylipd/usage.py
+-rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.1.1/pylipd/utils.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:44:06.418526 pylipd-1.1.1/pylipd.egg-info/
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 02:44:06.000000 pylipd-1.1.1/pylipd.egg-info/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      588 2023-04-11 02:44:06.000000 pylipd-1.1.1/pylipd.egg-info/SOURCES.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-11 02:44:06.000000 pylipd-1.1.1/pylipd.egg-info/dependency_links.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.1.1/pylipd.egg-info/not-zip-safe
+-rw-r--r--   0 varun      (502) staff       (20)       35 2023-04-11 02:44:06.000000 pylipd-1.1.1/pylipd.egg-info/requires.txt
+-rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-11 02:44:06.000000 pylipd-1.1.1/pylipd.egg-info/top_level.txt
+-rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.1.1/pyproject.toml
+-rw-r--r--   0 varun      (502) staff       (20)      693 2023-04-11 02:44:06.418928 pylipd-1.1.1/setup.cfg
+-rw-r--r--   0 varun      (502) staff       (20)      973 2023-04-11 02:43:32.000000 pylipd-1.1.1/setup.py
```

### Comparing `pylipd-1.1.0/LICENSE` & `pylipd-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.0/PKG-INFO` & `pylipd-1.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.0
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.1
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.1.0/README.md` & `pylipd-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.0/pylipd/globals/schema.py` & `pylipd-1.1.1/pylipd/globals/schema.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.0/pylipd/legacy_utils.py` & `pylipd-1.1.1/pylipd/legacy_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             # Get author data first, since that's the most ambiguously structured data.
             _root = self._extract_authors(pub, idx, _root)
             # Go through data of this publication
             for k, v in pub.items():
                 # Case 1: DOI ID. Don't need the rest of 'identifier' dict
                 if k == 'identifier':
                     try:
-                        _root['pub' + str(idx + 1) + '_DOI'] = "hello"
+                        _root['pub' + str(idx + 1) + '_DOI'] = v
                     except KeyError as e:
                         raise e
                 # Case 2: All other string entries
                 else:
                     if k != 'authors' and k != 'author':
                         _root['pub' + str(idx + 1) + '_' + k] = v
         return _root
```

### Comparing `pylipd-1.1.0/pylipd/lipd.py` & `pylipd-1.1.1/pylipd/lipd.py`

 * *Files 2% similar despite different names*

```diff
@@ -683,18 +683,19 @@
         .. ipython:: python
             :okwarning:
             :okexcept:
 
             from pylipd.lipd import LiPD
 
             # Fetch LiPD data from remote RDF Graph
-            lipd_remote = LiPD()
-            lipd_remote.set_endpoint("https://linkedearth.graphdb.mint.isi.edu/repositories/LiPDVerse2")
-            dsname = "Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001"
-            lipd_remote.load_remote_datasets([dsname])
+            lipd = LiPD()
+            lipd.load([
+                "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
+            ])
+            dsname = lipd.get_all_dataset_names()[0]
             lipd_remote.create_lipd(dsname, "test.lpd")
         '''           
         converter = RDFToLiPD(self.graph)
         return converter.convert(dsname, lipdfile)
     
     def pop(self, dsname=None, collection_id=None):
         '''Removes a dataset from the graph and returns a LiPD object
@@ -783,18 +784,28 @@
                 "../examples/data/MD98_2181.Stott.2007.lpd"
             ])
             all_datasets = lipd.get_all_dataset_names()
             print("Loaded datasets: " + str(all_datasets))
             lipd.remove(all_datasets[0])
             print("Loaded datasets after remove: " + str(lipd.get_all_dataset_names()))
         '''
-        graphurl = NSURL + "/" + dsname
-        if collection_id:
-            graphurl = NSURL + "/" + collection_id + "/" + dsname
-        self.graph.remove((None, None, None, graphurl))       
+        
+        if dsname:
+            graphurl = NSURL + "/" + dsname
+            if collection_id:
+                graphurl = NSURL + "/" + collection_id + "/" + dsname
+        elif collection_id:
+            graphurl = NSURL + "/" + collection_id
+
+        # Match subgraphs
+        for ctx in self.graph.contexts():
+            id = ctx.identifier
+            if id.startswith(graphurl):        
+                self.graph.remove((None, None, None, id))       
+
 
     def get_rdf(self):
         '''Returns RDF serialization of the current Graph
         Examples
         --------
 
         .. ipython:: python
```

### Comparing `pylipd-1.1.0/pylipd/lipd_to_rdf.py` & `pylipd-1.1.1/pylipd/lipd_to_rdf.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.0/pylipd/multi_processing.py` & `pylipd-1.1.1/pylipd/multi_processing.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.0/pylipd/rdf_to_lipd.py` & `pylipd-1.1.1/pylipd/rdf_to_lipd.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.0/pylipd/series/regexes.py` & `pylipd-1.1.1/pylipd/series/regexes.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.0/pylipd/test.py` & `pylipd-1.1.1/pylipd/test.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.0/pylipd/usage.py` & `pylipd-1.1.1/pylipd/usage.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.0/pylipd/utils.py` & `pylipd-1.1.1/pylipd/utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.0/pylipd.egg-info/PKG-INFO` & `pylipd-1.1.1/pylipd.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.0
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.1
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.1.0/pylipd.egg-info/SOURCES.txt` & `pylipd-1.1.1/pylipd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.0/setup.cfg` & `pylipd-1.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pylipd
-version = 1.1.0
+version = 1.1.1
 author = Varun Ratnakar
 author_email = varunratnakar@gmail.com
 description = Python utilities for handling LiPD data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/linkedearth/pylipd
 project_urls =
```

### Comparing `pylipd-1.1.0/setup.py` & `pylipd-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import setup, find_packages
 
 
-version = '1.1.0'
+version = '1.1.1'
 
 # Read the readme file contents into variable
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='pylipd',
```

