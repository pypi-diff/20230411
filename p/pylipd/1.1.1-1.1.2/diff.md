# Comparing `tmp/pylipd-1.1.1.tar.gz` & `tmp/pylipd-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylipd-1.1.1.tar", last modified: Tue Apr 11 02:44:06 2023, max compression
+gzip compressed data, was "pylipd-1.1.2.tar", last modified: Tue Apr 11 02:52:29 2023, max compression
```

## Comparing `pylipd-1.1.1.tar` & `pylipd-1.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:44:06.418621 pylipd-1.1.1/
--rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.1.1/LICENSE
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 02:44:06.418670 pylipd-1.1.1/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.1.1/README.md
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:44:06.416421 pylipd-1.1.1/pylipd/
--rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-11 02:43:37.000000 pylipd-1.1.1/pylipd/__init__.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:44:06.417277 pylipd-1.1.1/pylipd/globals/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.1.1/pylipd/globals/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)      409 2023-04-10 19:03:17.000000 pylipd-1.1.1/pylipd/globals/blacklist.py
--rw-r--r--   0 varun      (502) staff       (20)    14643 2023-04-10 19:06:28.000000 pylipd-1.1.1/pylipd/globals/schema.py
--rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.1.1/pylipd/globals/urls.py
--rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.1.1/pylipd/legacy_utils.py
--rw-r--r--   0 varun      (502) staff       (20)    30758 2023-04-11 02:42:48.000000 pylipd-1.1.1/pylipd/lipd.py
--rw-r--r--   0 varun      (502) staff       (20)    43704 2023-04-10 19:04:22.000000 pylipd-1.1.1/pylipd/lipd_to_rdf.py
--rw-r--r--   0 varun      (502) staff       (20)     1742 2023-04-07 05:39:21.000000 pylipd-1.1.1/pylipd/multi_processing.py
--rw-r--r--   0 varun      (502) staff       (20)    22294 2023-04-10 19:05:37.000000 pylipd-1.1.1/pylipd/rdf_to_lipd.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:44:06.417612 pylipd-1.1.1/pylipd/series/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.1.1/pylipd/series/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.1.1/pylipd/series/regexes.py
--rw-r--r--   0 varun      (502) staff       (20)     2270 2023-03-22 17:52:14.000000 pylipd-1.1.1/pylipd/test.py
--rw-r--r--   0 varun      (502) staff       (20)     5054 2023-04-10 12:38:55.000000 pylipd-1.1.1/pylipd/usage.py
--rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.1.1/pylipd/utils.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:44:06.418526 pylipd-1.1.1/pylipd.egg-info/
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 02:44:06.000000 pylipd-1.1.1/pylipd.egg-info/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      588 2023-04-11 02:44:06.000000 pylipd-1.1.1/pylipd.egg-info/SOURCES.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-11 02:44:06.000000 pylipd-1.1.1/pylipd.egg-info/dependency_links.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.1.1/pylipd.egg-info/not-zip-safe
--rw-r--r--   0 varun      (502) staff       (20)       35 2023-04-11 02:44:06.000000 pylipd-1.1.1/pylipd.egg-info/requires.txt
--rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-11 02:44:06.000000 pylipd-1.1.1/pylipd.egg-info/top_level.txt
--rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.1.1/pyproject.toml
--rw-r--r--   0 varun      (502) staff       (20)      693 2023-04-11 02:44:06.418928 pylipd-1.1.1/setup.cfg
--rw-r--r--   0 varun      (502) staff       (20)      973 2023-04-11 02:43:32.000000 pylipd-1.1.1/setup.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:52:29.124323 pylipd-1.1.2/
+-rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.1.2/LICENSE
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 02:52:29.124405 pylipd-1.1.2/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.1.2/README.md
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:52:29.121569 pylipd-1.1.2/pylipd/
+-rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-11 02:50:24.000000 pylipd-1.1.2/pylipd/__init__.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:52:29.122435 pylipd-1.1.2/pylipd/globals/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.1.2/pylipd/globals/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)      409 2023-04-10 19:03:17.000000 pylipd-1.1.2/pylipd/globals/blacklist.py
+-rw-r--r--   0 varun      (502) staff       (20)    14643 2023-04-10 19:06:28.000000 pylipd-1.1.2/pylipd/globals/schema.py
+-rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.1.2/pylipd/globals/urls.py
+-rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.1.2/pylipd/legacy_utils.py
+-rw-r--r--   0 varun      (502) staff       (20)    31780 2023-04-11 02:51:38.000000 pylipd-1.1.2/pylipd/lipd.py
+-rw-r--r--   0 varun      (502) staff       (20)    43704 2023-04-10 19:04:22.000000 pylipd-1.1.2/pylipd/lipd_to_rdf.py
+-rw-r--r--   0 varun      (502) staff       (20)     1742 2023-04-07 05:39:21.000000 pylipd-1.1.2/pylipd/multi_processing.py
+-rw-r--r--   0 varun      (502) staff       (20)    22294 2023-04-10 19:05:37.000000 pylipd-1.1.2/pylipd/rdf_to_lipd.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:52:29.122874 pylipd-1.1.2/pylipd/series/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.1.2/pylipd/series/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.1.2/pylipd/series/regexes.py
+-rw-r--r--   0 varun      (502) staff       (20)     2270 2023-03-22 17:52:14.000000 pylipd-1.1.2/pylipd/test.py
+-rw-r--r--   0 varun      (502) staff       (20)     5054 2023-04-10 12:38:55.000000 pylipd-1.1.2/pylipd/usage.py
+-rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.1.2/pylipd/utils.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:52:29.124191 pylipd-1.1.2/pylipd.egg-info/
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 02:52:29.000000 pylipd-1.1.2/pylipd.egg-info/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      588 2023-04-11 02:52:29.000000 pylipd-1.1.2/pylipd.egg-info/SOURCES.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-11 02:52:29.000000 pylipd-1.1.2/pylipd.egg-info/dependency_links.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.1.2/pylipd.egg-info/not-zip-safe
+-rw-r--r--   0 varun      (502) staff       (20)       35 2023-04-11 02:52:29.000000 pylipd-1.1.2/pylipd.egg-info/requires.txt
+-rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-11 02:52:29.000000 pylipd-1.1.2/pylipd.egg-info/top_level.txt
+-rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.1.2/pyproject.toml
+-rw-r--r--   0 varun      (502) staff       (20)      693 2023-04-11 02:52:29.124739 pylipd-1.1.2/setup.cfg
+-rw-r--r--   0 varun      (502) staff       (20)      973 2023-04-11 02:50:17.000000 pylipd-1.1.2/setup.py
```

### Comparing `pylipd-1.1.1/LICENSE` & `pylipd-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.1/PKG-INFO` & `pylipd-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.1
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.2
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.1.1/README.md` & `pylipd-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.1/pylipd/globals/schema.py` & `pylipd-1.1.2/pylipd/globals/schema.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.1/pylipd/legacy_utils.py` & `pylipd-1.1.2/pylipd/legacy_utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.1/pylipd/lipd.py` & `pylipd-1.1.2/pylipd/lipd.py`

 * *Files 3% similar despite different names*

```diff
@@ -591,22 +591,34 @@
                 verbose = True
         
         if verbose == True:
             print(bibs)
         
         return bibs, df       
 
-    def get_timeseries(self, dsnames):
+    def get_timeseries(self, dsnames, to_dataframe=False):
         '''Get Legacy LiPD like Time Series Object (tso)
 
         Parameters
         ----------
 
-        dsnames : array
+        dsnames : list
             array of dataset id or name strings
+        
+        to_dataframe : bool {True; False}
+            Whether to return a dataframe along the dictionary. Default is False
+        
+        Returns
+        -------
+        
+        ts : dict
+            A dictionary containing Time Series Object
+            
+        df : Pandas.DataFrame
+            If to_dataframe is set to True, returns a queriable Pandas DataFrame
 
         Examples
         --------
 
         .. ipython:: python
             :okwarning:
             :okexcept:
@@ -619,15 +631,26 @@
             ts_list = lipd_remote.get_timeseries(["Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001", "MD98_2181.Stott.2007", "Ant-WAIS-Divide.Severinghaus.2012"])
             for dsname, tsos in ts_list.items():
                 for tso in tsos:
                     if 'paleoData_variableName' in tso:
                         print(dsname+': '+tso['paleoData_variableName']+': '+tso['archiveType'])
         '''
         ts = self._get_timeseries(dsnames)
-        return ts
+        if to_dataframe == False:
+            return ts
+        elif to_dataframe == True:
+            dict_list =[]
+
+            for item in ts.keys():
+                for dictionary in ts[item]:
+                    dict_list.append(dictionary)
+
+            df = pd.DataFrame.from_dict(dict_list, orient='columns')
+            
+            return ts, df
 
     def _get_timeseries(self, dsnames):
         timeseries = {}
         for dsname in dsnames:
             converter = RDFToLiPD(self.graph)
             d = converter.convert_to_json(dsname)
             print("Extracting timeseries from dataset: " + dsname + " ...")
@@ -693,21 +716,21 @@
             ])
             dsname = lipd.get_all_dataset_names()[0]
             lipd_remote.create_lipd(dsname, "test.lpd")
         '''           
         converter = RDFToLiPD(self.graph)
         return converter.convert(dsname, lipdfile)
     
-    def pop(self, dsname=None, collection_id=None):
+    def pop(self, dsnames=None, collection_id=None):
         '''Removes a dataset from the graph and returns a LiPD object
 
         Parameters
         ----------
 
-        dsname : str
+        dsname : str or list of str
             (Optional) Name of the dataset (Set to None to pop all datasets in a collection)
 
         collection_id : str
             (Optional) collection id for the dataset
 
         Examples
         --------
@@ -728,46 +751,53 @@
             print("Loaded datasets: " + str(all_datasets))
             popped = lipd.pop(all_datasets[0])
             print("Loaded datasets after pop: " + str(lipd.get_all_dataset_names()))
             print("Popped dataset: " + str(popped.get_all_dataset_names()))       
         '''
 
         popped = LiPD()
-
-        if dsname:
-            graphurl = NSURL + "/" + dsname
-            if collection_id:
-                graphurl = NSURL + "/" + collection_id + "/" + dsname
+        
+        if type(dsnames) is not list:
+            dsnames = [dsnames]
+        
+        graphurls=[]
+        
+        if dsnames:
+            for dsname in dsnames:
+                graphurls.append(NSURL + "/" + dsname)
+                if collection_id:
+                    graphurls.append(NSURL + "/" + collection_id + "/" + dsname)
         elif collection_id:
-            graphurl = NSURL + "/" + collection_id
+            graphurls.append(NSURL + "/" + collection_id)
 
         # Match subgraphs
-        for ctx in self.graph.contexts():
-            id = ctx.identifier
-            if id.startswith(graphurl):
-                subgraph = copy.deepcopy(self.graph.get_context(id))
-                for triple in subgraph.triples((None, None, None)):
-                    popped.graph.add((
-                        triple[0],
-                        triple[1],
-                        triple[2],
-                        URIRef(id)))
-
-                self.graph.remove((None, None, None, id))
+        for graphurl in graphurls:
+            for ctx in self.graph.contexts():
+                id = ctx.identifier
+                if id.startswith(graphurl):
+                    subgraph = copy.deepcopy(self.graph.get_context(id))
+                    for triple in subgraph.triples((None, None, None)):
+                        popped.graph.add((
+                            triple[0],
+                            triple[1],
+                            triple[2],
+                            URIRef(id)))
+    
+                    self.graph.remove((None, None, None, id))
         
         return popped
 
     def remove(self, dsname, collection_id=None):
         '''Removes a dataset from the graph
 
         Parameters
         ----------
 
-        dsname : str
-            Path to the directory containing lipd files
+        dsnames : str or list of str
+            dataset name(s) to be removed
 
         collection_id : str
             (Optional) collection id for the dataset
 
         Examples
         --------
```

### Comparing `pylipd-1.1.1/pylipd/lipd_to_rdf.py` & `pylipd-1.1.2/pylipd/lipd_to_rdf.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.1/pylipd/multi_processing.py` & `pylipd-1.1.2/pylipd/multi_processing.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.1/pylipd/rdf_to_lipd.py` & `pylipd-1.1.2/pylipd/rdf_to_lipd.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.1/pylipd/series/regexes.py` & `pylipd-1.1.2/pylipd/series/regexes.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.1/pylipd/test.py` & `pylipd-1.1.2/pylipd/test.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.1/pylipd/usage.py` & `pylipd-1.1.2/pylipd/usage.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.1/pylipd/utils.py` & `pylipd-1.1.2/pylipd/utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.1/pylipd.egg-info/PKG-INFO` & `pylipd-1.1.2/pylipd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.1
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.2
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.1.1/pylipd.egg-info/SOURCES.txt` & `pylipd-1.1.2/pylipd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.1/setup.cfg` & `pylipd-1.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pylipd
-version = 1.1.1
+version = 1.1.2
 author = Varun Ratnakar
 author_email = varunratnakar@gmail.com
 description = Python utilities for handling LiPD data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/linkedearth/pylipd
 project_urls =
```

### Comparing `pylipd-1.1.1/setup.py` & `pylipd-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import setup, find_packages
 
 
-version = '1.1.1'
+version = '1.1.2'
 
 # Read the readme file contents into variable
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='pylipd',
```

