# Comparing `tmp/pylipd-1.1.3.tar.gz` & `tmp/pylipd-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylipd-1.1.3.tar", last modified: Tue Apr 11 02:59:59 2023, max compression
+gzip compressed data, was "pylipd-1.2.0.tar", last modified: Tue Apr 11 03:27:11 2023, max compression
```

## Comparing `pylipd-1.1.3.tar` & `pylipd-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:59:59.695376 pylipd-1.1.3/
--rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.1.3/LICENSE
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 02:59:59.695453 pylipd-1.1.3/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.1.3/README.md
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:59:59.692352 pylipd-1.1.3/pylipd/
--rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-11 02:59:51.000000 pylipd-1.1.3/pylipd/__init__.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:59:59.693524 pylipd-1.1.3/pylipd/globals/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.1.3/pylipd/globals/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)      409 2023-04-10 19:03:17.000000 pylipd-1.1.3/pylipd/globals/blacklist.py
--rw-r--r--   0 varun      (502) staff       (20)    14643 2023-04-10 19:06:28.000000 pylipd-1.1.3/pylipd/globals/schema.py
--rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.1.3/pylipd/globals/urls.py
--rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.1.3/pylipd/legacy_utils.py
--rw-r--r--   0 varun      (502) staff       (20)    31680 2023-04-11 02:59:29.000000 pylipd-1.1.3/pylipd/lipd.py
--rw-r--r--   0 varun      (502) staff       (20)    43704 2023-04-10 19:04:22.000000 pylipd-1.1.3/pylipd/lipd_to_rdf.py
--rw-r--r--   0 varun      (502) staff       (20)     1742 2023-04-07 05:39:21.000000 pylipd-1.1.3/pylipd/multi_processing.py
--rw-r--r--   0 varun      (502) staff       (20)    22294 2023-04-10 19:05:37.000000 pylipd-1.1.3/pylipd/rdf_to_lipd.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:59:59.693970 pylipd-1.1.3/pylipd/series/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.1.3/pylipd/series/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.1.3/pylipd/series/regexes.py
--rw-r--r--   0 varun      (502) staff       (20)     2270 2023-03-22 17:52:14.000000 pylipd-1.1.3/pylipd/test.py
--rw-r--r--   0 varun      (502) staff       (20)     5054 2023-04-10 12:38:55.000000 pylipd-1.1.3/pylipd/usage.py
--rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.1.3/pylipd/utils.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 02:59:59.695247 pylipd-1.1.3/pylipd.egg-info/
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 02:59:59.000000 pylipd-1.1.3/pylipd.egg-info/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      588 2023-04-11 02:59:59.000000 pylipd-1.1.3/pylipd.egg-info/SOURCES.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-11 02:59:59.000000 pylipd-1.1.3/pylipd.egg-info/dependency_links.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.1.3/pylipd.egg-info/not-zip-safe
--rw-r--r--   0 varun      (502) staff       (20)       35 2023-04-11 02:59:59.000000 pylipd-1.1.3/pylipd.egg-info/requires.txt
--rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-11 02:59:59.000000 pylipd-1.1.3/pylipd.egg-info/top_level.txt
--rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.1.3/pyproject.toml
--rw-r--r--   0 varun      (502) staff       (20)      693 2023-04-11 02:59:59.695764 pylipd-1.1.3/setup.cfg
--rw-r--r--   0 varun      (502) staff       (20)      973 2023-04-11 02:59:45.000000 pylipd-1.1.3/setup.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 03:27:11.469067 pylipd-1.2.0/
+-rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.2.0/LICENSE
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 03:27:11.469168 pylipd-1.2.0/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.2.0/README.md
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 03:27:11.465764 pylipd-1.2.0/pylipd/
+-rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-11 03:21:33.000000 pylipd-1.2.0/pylipd/__init__.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 03:27:11.466822 pylipd-1.2.0/pylipd/globals/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.2.0/pylipd/globals/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)      409 2023-04-10 19:03:17.000000 pylipd-1.2.0/pylipd/globals/blacklist.py
+-rw-r--r--   0 varun      (502) staff       (20)    14643 2023-04-10 19:06:28.000000 pylipd-1.2.0/pylipd/globals/schema.py
+-rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.2.0/pylipd/globals/urls.py
+-rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.2.0/pylipd/legacy_utils.py
+-rw-r--r--   0 varun      (502) staff       (20)    30545 2023-04-11 03:26:28.000000 pylipd-1.2.0/pylipd/lipd.py
+-rw-r--r--   0 varun      (502) staff       (20)    43172 2023-04-11 03:12:51.000000 pylipd-1.2.0/pylipd/lipd_to_rdf.py
+-rw-r--r--   0 varun      (502) staff       (20)     1576 2023-04-11 03:11:49.000000 pylipd-1.2.0/pylipd/multi_processing.py
+-rw-r--r--   0 varun      (502) staff       (20)    22021 2023-04-11 03:13:16.000000 pylipd-1.2.0/pylipd/rdf_to_lipd.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 03:27:11.467187 pylipd-1.2.0/pylipd/series/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.2.0/pylipd/series/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.2.0/pylipd/series/regexes.py
+-rw-r--r--   0 varun      (502) staff       (20)     2270 2023-03-22 17:52:14.000000 pylipd-1.2.0/pylipd/test.py
+-rw-r--r--   0 varun      (502) staff       (20)     5126 2023-04-11 03:19:24.000000 pylipd-1.2.0/pylipd/usage.py
+-rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.2.0/pylipd/utils.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 03:27:11.468822 pylipd-1.2.0/pylipd.egg-info/
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 03:27:11.000000 pylipd-1.2.0/pylipd.egg-info/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      588 2023-04-11 03:27:11.000000 pylipd-1.2.0/pylipd.egg-info/SOURCES.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-11 03:27:11.000000 pylipd-1.2.0/pylipd.egg-info/dependency_links.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.2.0/pylipd.egg-info/not-zip-safe
+-rw-r--r--   0 varun      (502) staff       (20)       35 2023-04-11 03:27:11.000000 pylipd-1.2.0/pylipd.egg-info/requires.txt
+-rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-11 03:27:11.000000 pylipd-1.2.0/pylipd.egg-info/top_level.txt
+-rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.2.0/pyproject.toml
+-rw-r--r--   0 varun      (502) staff       (20)      693 2023-04-11 03:27:11.469531 pylipd-1.2.0/setup.cfg
+-rw-r--r--   0 varun      (502) staff       (20)      973 2023-04-11 03:21:29.000000 pylipd-1.2.0/setup.py
```

### Comparing `pylipd-1.1.3/LICENSE` & `pylipd-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.3/PKG-INFO` & `pylipd-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.1.3
+Version: 1.2.0
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.3
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.2.0
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.1.3/README.md` & `pylipd-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.3/pylipd/globals/schema.py` & `pylipd-1.2.0/pylipd/globals/schema.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.3/pylipd/legacy_utils.py` & `pylipd-1.2.0/pylipd/legacy_utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.3/pylipd/lipd.py` & `pylipd-1.2.0/pylipd/lipd.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,30 +96,27 @@
 
         '''
 
         merged = self.copy()
         merged.graph.addN(lipd.graph.quads())
         return merged
     
-    def load_from_dir(self, dir_path, parallel=False, collection_id=None):
+    def load_from_dir(self, dir_path, parallel=False):
         '''Load LiPD files from a directory
         Note: This function creates multiple process to process lipd files in parallel, therefore it is important that this call be made under the "__main__" process
 
         Parameters
         ----------
 
         dir_path : str
             path to the directory containing lipd files
 
         parallel: bool
             (Optional) set to True to process lipd files in parallel. You *must* run this function under the "__main__" process for this to work
 
-        collection_id : str
-            (Optional) set a collection id for all lipd files in the directory
-
         Examples
         --------
         In this example, we load LiPD files from a directory.
 
         .. ipython:: python
             :okwarning:
             :okexcept:
@@ -136,33 +133,31 @@
             return
 
         lipdfiles = []
         for path in os.listdir(dir_path):
             file_path = os.path.join(dir_path, path)
             if os.path.isfile(file_path) and path.endswith(".lpd"):
                 lipdfiles.append(file_path)
-        self.load(lipdfiles, parallel, collection_id)
+        self.load(lipdfiles, parallel)
 
 
     # Allows loading http locations
-    def load(self, lipdfiles, parallel=False, collection_id=None):
+    def load(self, lipdfiles, parallel=False):
         '''Load LiPD files. 
         Note: This function creates multiple process to process lipd files in parallel, therefore it is important that this call be made under the "__main__" process
 
         Parameters
         ----------
 
-        lipdfiles : array
+        lipdfiles : list of str
             array of paths to lipd files (the paths could also be urls)
 
         parallel: bool
             (Optional) set to True to process lipd files in parallel. You *must* run this function under the "__main__" process for this to work
 
-        collection_id : str
-            (Optional) set a collection id for all lipd files in the directory
 
         Examples
         --------
         In this example, we load LiPD files for an array of paths.
 
         .. ipython:: python
             :okwarning:
@@ -188,17 +183,17 @@
             if not os.path.isfile(lipdfile) and not lipdfile.startswith("http"):
                 print(f"File {lipdfile} does not exist")
                 continue
 
             picklefile = tempfile.NamedTemporaryFile().name
             filemap[lipdfile] = picklefile
         
-        print(f"Loading {len(filemap.keys())} LiPD files" + (" from Collection: {collection_id}" if collection_id else ""))
+        print(f"Loading {len(filemap.keys())} LiPD files")
         
-        multi_convert_to_pickle(filemap, parallel, collection_id)
+        multi_convert_to_pickle(filemap, parallel)
         print("Conversion to RDF done..")
 
         print("Loading RDF into graph")
         for lipdfile in lipdfiles:
             picklefile = filemap[lipdfile]
             if os.path.exists(picklefile):
                 with open(picklefile, 'rb') as f:
@@ -237,28 +232,26 @@
             lipd_remote.load_remote_datasets(["Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001", "MD98_2181.Stott.2007", "Ant-WAIS-Divide.Severinghaus.2012"])
             print(lipd_remote.get_all_dataset_names())
 
         '''
         self.endpoint = endpoint
 
 
-    def convert_lipd_dir_to_rdf(self, lipd_dir, rdf_file, parallel=False, collection_id=None):
+    def convert_lipd_dir_to_rdf(self, lipd_dir, rdf_file, parallel=False):
         '''Convert a directory containing LiPD files into a single RDF file (to be used for uploading to Knowledge Bases like GraphDB)
 
         Parameters
         ----------
 
         lipd_dir : str
             Path to the directory containing lipd files
 
         rdf_file : str
             Path to the output rdf file
 
-        collection_id : str
-            (Optional) set a collection id for all lipd files in the directory
 
         Examples
         --------
 
         .. ipython:: python
             :okwarning:
             :okexcept:
@@ -275,15 +268,15 @@
         for path in os.listdir(lipd_dir):
             fullpath = os.path.join(lipd_dir, path)
             tmp_rdf_file = tempfile.NamedTemporaryFile().name
             filemap[fullpath] = tmp_rdf_file
         
         print(f"Starting conversion of {len(filemap.keys())} LiPD files")
 
-        multi_convert_to_rdf(filemap, parallel, collection_id)
+        multi_convert_to_rdf(filemap, parallel)
         
         print("Conversion to RDF done..")
 
         print("Writing to main RDF file..")
         with open(rdf_file, "a") as fout:
             for lipdfile in filemap.keys():
                 tmp_rdf_file = filemap[lipdfile]
@@ -674,15 +667,15 @@
         .. ipython:: python
             :okwarning:
             :okexcept:
 
             from pylipd.lipd import LiPD
 
             # Fetch LiPD data from remote RDF Graph
-            lipd = LiPD()
+            lipd = LiPD()git
             lipd.load([
                 "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
             ])
             lipd_json = lipd.get_lipd(lipd.get_all_dataset_names()[0])
             print(lipd_json)
         '''           
         converter = RDFToLiPD(self.graph)
@@ -716,25 +709,23 @@
             ])
             dsname = lipd.get_all_dataset_names()[0]
             lipd.create_lipd(dsname, "test.lpd")
         '''           
         converter = RDFToLiPD(self.graph)
         return converter.convert(dsname, lipdfile)
     
-    def pop(self, dsnames=None, collection_id=None):
-        '''Removes a dataset from the graph and returns a LiPD object
+    def pop(self, dsnames):
+        '''Pops dataset(s) from the graph and returns the popped LiPD object
 
         Parameters
         ----------
 
-        dsname : str or list of str
-            (Optional) Name of the dataset (Set to None to pop all datasets in a collection)
+        dsnames : str or list of str
+            dataset name(s) to be popped.
 
-        collection_id : str
-            (Optional) collection id for the dataset
 
         Examples
         --------
 
         .. ipython:: python
             :okwarning:
             :okexcept:
@@ -751,57 +742,47 @@
             print("Loaded datasets: " + str(all_datasets))
             popped = lipd.pop(all_datasets[0])
             print("Loaded datasets after pop: " + str(lipd.get_all_dataset_names()))
             print("Popped dataset: " + str(popped.get_all_dataset_names()))       
         '''
 
         popped = LiPD()
-        
+
         if type(dsnames) is not list:
             dsnames = [dsnames]
         
         graphurls=[]
-        
-        if dsnames:
-            for dsname in dsnames:
-                graphurls.append(NSURL + "/" + dsname)
-                if collection_id:
-                    graphurls.append(NSURL + "/" + collection_id + "/" + dsname)
-        elif collection_id:
-            graphurls.append(NSURL + "/" + collection_id)
+        for dsname in dsnames:
+            graphurls.append(NSURL + "/" + dsname)
 
         # Match subgraphs
-        for graphurl in graphurls:
-            for ctx in self.graph.contexts():
-                id = ctx.identifier
-                if id.startswith(graphurl):
-                    subgraph = copy.deepcopy(self.graph.get_context(id))
-                    for triple in subgraph.triples((None, None, None)):
-                        popped.graph.add((
-                            triple[0],
-                            triple[1],
-                            triple[2],
-                            URIRef(id)))
-    
-                    self.graph.remove((None, None, None, id))
+        for ctx in self.graph.contexts():
+            id = str(ctx.identifier)
+            if id in graphurls:
+                subgraph = copy.deepcopy(self.graph.get_context(id))
+                for triple in subgraph.triples((None, None, None)):
+                    popped.graph.add((
+                        triple[0],
+                        triple[1],
+                        triple[2],
+                        URIRef(id)))
+
+                self.graph.remove((None, None, None, id))
         
         return popped
 
-    def remove(self, dsname, collection_id=None):
-        '''Removes a dataset from the graph
+    def remove(self, dsnames):
+        '''Removes dataset(s) from the graph
 
         Parameters
         ----------
 
         dsnames : str or list of str
             dataset name(s) to be removed
 
-        collection_id : str
-            (Optional) collection id for the dataset
-
         Examples
         --------
 
         .. ipython:: python
             :okwarning:
             :okexcept:
 
@@ -815,25 +796,25 @@
             ])
             all_datasets = lipd.get_all_dataset_names()
             print("Loaded datasets: " + str(all_datasets))
             lipd.remove(all_datasets[0])
             print("Loaded datasets after remove: " + str(lipd.get_all_dataset_names()))
         '''
         
-        if dsname:
-            graphurl = NSURL + "/" + dsname
-            if collection_id:
-                graphurl = NSURL + "/" + collection_id + "/" + dsname
-        elif collection_id:
-            graphurl = NSURL + "/" + collection_id
+        if type(dsnames) is not list:
+            dsnames = [dsnames]
+        
+        graphurls=[]
+        for dsname in dsnames:
+            graphurls.append(NSURL + "/" + dsname)
 
         # Match subgraphs
         for ctx in self.graph.contexts():
-            id = ctx.identifier
-            if id.startswith(graphurl):        
+            id = str(ctx.identifier)
+            if id in graphurls:
                 self.graph.remove((None, None, None, id))       
 
 
     def get_rdf(self):
         '''Returns RDF serialization of the current Graph
         Examples
         --------
```

### Comparing `pylipd-1.1.3/pylipd/lipd_to_rdf.py` & `pylipd-1.2.0/pylipd/lipd_to_rdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,31 +26,22 @@
 
 from .utils import expand_schema, ucfirst, lcfirst, camelCase, unCamelCase, escape, uniqid, sanitizeId
 
 class LipdToRDF:
     """
     The LipdToRDF class helps in converting a LiPD file to an RDF Graph. 
     It uses the SCHEMA dictionary (from globals/schema.py) to do the conversion
-
-    Parameters
-    ----------
-    collection_id : str
-        (Optional) set a collection id for the lipd file
     """
 
-    def __init__(self, collection_id=None):
+    def __init__(self):
         self.graph = ConjunctiveGraph()
         self.lipd_csvs = {}
-        self.collection_id = collection_id
         self.graphurl = NSURL
         self.namespace = NSURL + "#"
-        self.schema = expand_schema(copy.deepcopy(SCHEMA))
-
-        if self.collection_id:
-            self.namespace = NSURL + "/" + collection_id + "#"        
+        self.schema = expand_schema(copy.deepcopy(SCHEMA))  
 
 
     def convert(self, lipdpath, topath, type="rdf"):
         '''Convert LiPD file to RDF (or Pickled Graph)
 
         Parameters
         ----------
@@ -67,16 +58,14 @@
 
         self.graph = ConjunctiveGraph()
         
         lpdname = os.path.basename(lipdpath).replace(".lpd", "")
         lpdname = re.sub("\?.+$", "", lpdname)
 
         self.graphurl = NSURL + "/" + lpdname
-        if self.collection_id:
-            self.graphurl = NSURL + "/" + self.collection_id + "/" + lpdname
 
         with tempfile.TemporaryDirectory(prefix="lipd_to_rdf_") as tmpdir:
             self._unzip_lipd_file(lipdpath, tmpdir)
             jsons = self._find_files_with_extension(tmpdir, 'jsonld')
             for jsonpath, _ in jsons:
                 jsondir = os.path.dirname(jsonpath)
                 csvs = self._find_files_with_extension(jsondir, 'csv')
@@ -1118,14 +1107,12 @@
         
         with open(jsonpath) as f:
             obj = json.load(f)
             
             self._map_lipd_to_json(obj, None, None, "Dataset", "Dataset", objhash)
             if url:
                 objhash[obj["@id"]]["hasUrl"] = url
-            elif self.collection_id:
-                objhash[obj["@id"]]["hasUrl"] = DATAURL + "/" + self.collection_id + "/" + obj["@id"] + ".lpd"
             else:
                 objhash[obj["@id"]]["hasUrl"] = DATAURL + "/" + obj["@id"] + ".lpd"
 
             for key, item in objhash.items():
                 self._create_individual_full(item)
```

### Comparing `pylipd-1.1.3/pylipd/multi_processing.py` & `pylipd-1.2.0/pylipd/multi_processing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from pylipd.lipd_to_rdf import LipdToRDF
 import multiprocessing as mp
 
-def convert_to_rdf(lipdfile, rdffile, collection_id=None):
-    converter = LipdToRDF(collection_id)    
+def convert_to_rdf(lipdfile, rdffile):
+    converter = LipdToRDF()    
     """Worker that converts one lipdfile to an rdffile"""
     try:
         converter.convert(lipdfile, rdffile)
     except Exception as e:
         print(f"ERROR: Could not convert LiPD file {lipdfile} to RDF")            
         raise e
 
-def multi_convert_to_rdf(filemap, parallel=True, collection_id=None):
+def multi_convert_to_rdf(filemap, parallel=True):
     if parallel:
         """Create a pool to convert all lipdfiles to rdffiles"""
         pool = mp.Pool(mp.cpu_count())
-        args = [(lipdfile, rdffile, collection_id) for lipdfile, rdffile in filemap.items()]
+        args = [(lipdfile, rdffile) for lipdfile, rdffile in filemap.items()]
         pool.starmap(convert_to_rdf, args, chunksize=1)
         pool.close()
     else:
         for lipdfile, rdffile in filemap.items():
-            convert_to_rdf(lipdfile, rdffile, collection_id)
+            convert_to_rdf(lipdfile, rdffile)
 
-def convert_to_pickle(lipdfile, tofile, collection_id=None):
-    converter = LipdToRDF(collection_id)    
+def convert_to_pickle(lipdfile, tofile):
+    converter = LipdToRDF()    
     """Worker that converts one lipdfile to an rdffile"""
     try:
         converter.convert(lipdfile, tofile, type="pickle")
     except Exception as e:
         print(f"ERROR: Could not convert LiPD file {lipdfile} to RDF")            
         raise e
 
-def multi_convert_to_pickle(filemap, parallel=True, collection_id=None):
+def multi_convert_to_pickle(filemap, parallel=True):
     """Create a pool to convert all lipdfiles to picklefiles"""
     if parallel:
         pool = mp.Pool(mp.cpu_count())
-        args = [(lipdfile, tofile, collection_id) for lipdfile, tofile in filemap.items()]
+        args = [(lipdfile, tofile) for lipdfile, tofile in filemap.items()]
         pool.starmap(convert_to_pickle, args, chunksize=1)
         pool.close()
     else:
         for lipdfile, tofile in filemap.items():
-            convert_to_pickle(lipdfile, tofile, collection_id)
+            convert_to_pickle(lipdfile, tofile)
```

### Comparing `pylipd-1.1.3/pylipd/rdf_to_lipd.py` & `pylipd-1.2.0/pylipd/rdf_to_lipd.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,20 @@
 
 from .utils import ucfirst, lcfirst, unCamelCase, unzip_string
 
 class RDFToLiPD:
     """
     The RDFToLiPD class helps in converting an RDF Graph to a LiPD file.
     It uses the SCHEMA dictionary (from globals/schema.py) to do the conversion
-
-    Parameters
-    ----------
-    collection_id : str
-        (Optional) set a collection id for the lipd file    
     """    
-    def __init__(self, graph, collection_id=None):
+    def __init__(self, graph):
         self.graph = graph
         self.lipd_csvs = {}
-        self.collection_id = collection_id
         self.graphurl = NSURL
         self.namespace = NSURL + "#"
-        if self.collection_id:
-            self.namespace = NSURL + "/" + collection_id + "#"
 
     def convert(self, dsname, lipdfile):
         '''Convert RDF graph to a LiPD file
 
         Parameters
         ----------
```

### Comparing `pylipd-1.1.3/pylipd/series/regexes.py` & `pylipd-1.2.0/pylipd/series/regexes.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.3/pylipd/test.py` & `pylipd-1.2.0/pylipd/test.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.3/pylipd/usage.py` & `pylipd-1.2.0/pylipd/usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,17 @@
 ts_list_remote = lipd.get_timeseries(lipd.get_all_dataset_names())
 for dsname, tsos in ts_list_remote.items():
     for tso in tsos:
         print(dsname+': '+str(tso['paleoData_variableName'])+': '+tso['archiveType'])
 '''
 
 print("Popping ...")
-poplipd = lipd.pop(lipd.get_all_dataset_names()[0])
+poplipd = lipd.pop(lipd.get_all_dataset_names())
+print(lipd.get_all_dataset_names())
+print(poplipd.get_all_dataset_names())
 
 print("Creating separate lipd file for popped")
 dsname = poplipd.get_all_dataset_names()[0]
 lipdfile = f"{dsname}.lpd"
 poplipd.create_lipd(dsname, lipdfile)
 
 print("Loading .. created lipd file: "+lipdfile)
```

### Comparing `pylipd-1.1.3/pylipd/utils.py` & `pylipd-1.2.0/pylipd/utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.3/pylipd.egg-info/PKG-INFO` & `pylipd-1.2.0/pylipd.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.1.3
+Version: 1.2.0
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.3
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.2.0
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.1.3/pylipd.egg-info/SOURCES.txt` & `pylipd-1.2.0/pylipd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylipd-1.1.3/setup.cfg` & `pylipd-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pylipd
-version = 1.1.3
+version = 1.2.0
 author = Varun Ratnakar
 author_email = varunratnakar@gmail.com
 description = Python utilities for handling LiPD data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/linkedearth/pylipd
 project_urls =
```

### Comparing `pylipd-1.1.3/setup.py` & `pylipd-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import setup, find_packages
 
 
-version = '1.1.3'
+version = '1.2.0'
 
 # Read the readme file contents into variable
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='pylipd',
```

