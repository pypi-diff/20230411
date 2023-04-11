# Comparing `tmp/pylipd-1.2.1.tar.gz` & `tmp/pylipd-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylipd-1.2.1.tar", last modified: Tue Apr 11 05:50:39 2023, max compression
+gzip compressed data, was "pylipd-1.2.2.tar", last modified: Tue Apr 11 06:34:45 2023, max compression
```

## Comparing `pylipd-1.2.1.tar` & `pylipd-1.2.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 05:50:39.133508 pylipd-1.2.1/
--rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.2.1/LICENSE
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 05:50:39.133574 pylipd-1.2.1/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.2.1/README.md
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 05:50:39.131158 pylipd-1.2.1/pylipd/
--rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-11 05:50:19.000000 pylipd-1.2.1/pylipd/__init__.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 05:50:39.132009 pylipd-1.2.1/pylipd/globals/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.2.1/pylipd/globals/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)      409 2023-04-10 19:03:17.000000 pylipd-1.2.1/pylipd/globals/blacklist.py
--rw-r--r--   0 varun      (502) staff       (20)    14643 2023-04-10 19:06:28.000000 pylipd-1.2.1/pylipd/globals/schema.py
--rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.2.1/pylipd/globals/urls.py
--rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.2.1/pylipd/legacy_utils.py
--rw-r--r--   0 varun      (502) staff       (20)    30542 2023-04-11 05:48:11.000000 pylipd-1.2.1/pylipd/lipd.py
--rw-r--r--   0 varun      (502) staff       (20)    43172 2023-04-11 03:12:51.000000 pylipd-1.2.1/pylipd/lipd_to_rdf.py
--rw-r--r--   0 varun      (502) staff       (20)     1576 2023-04-11 03:11:49.000000 pylipd-1.2.1/pylipd/multi_processing.py
--rw-r--r--   0 varun      (502) staff       (20)    22021 2023-04-11 03:13:16.000000 pylipd-1.2.1/pylipd/rdf_to_lipd.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 05:50:39.132339 pylipd-1.2.1/pylipd/series/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.2.1/pylipd/series/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.2.1/pylipd/series/regexes.py
--rw-r--r--   0 varun      (502) staff       (20)     2270 2023-03-22 17:52:14.000000 pylipd-1.2.1/pylipd/test.py
--rw-r--r--   0 varun      (502) staff       (20)     5126 2023-04-11 03:19:24.000000 pylipd-1.2.1/pylipd/usage.py
--rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.2.1/pylipd/utils.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 05:50:39.133392 pylipd-1.2.1/pylipd.egg-info/
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 05:50:39.000000 pylipd-1.2.1/pylipd.egg-info/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      588 2023-04-11 05:50:39.000000 pylipd-1.2.1/pylipd.egg-info/SOURCES.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-11 05:50:39.000000 pylipd-1.2.1/pylipd.egg-info/dependency_links.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.2.1/pylipd.egg-info/not-zip-safe
--rw-r--r--   0 varun      (502) staff       (20)       35 2023-04-11 05:50:39.000000 pylipd-1.2.1/pylipd.egg-info/requires.txt
--rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-11 05:50:39.000000 pylipd-1.2.1/pylipd.egg-info/top_level.txt
--rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.2.1/pyproject.toml
--rw-r--r--   0 varun      (502) staff       (20)      693 2023-04-11 05:50:39.133889 pylipd-1.2.1/setup.cfg
--rw-r--r--   0 varun      (502) staff       (20)      973 2023-04-11 05:50:12.000000 pylipd-1.2.1/setup.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 06:34:45.266512 pylipd-1.2.2/
+-rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.2.2/LICENSE
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 06:34:45.266557 pylipd-1.2.2/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.2.2/README.md
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 06:34:45.264463 pylipd-1.2.2/pylipd/
+-rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-11 06:33:18.000000 pylipd-1.2.2/pylipd/__init__.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 06:34:45.265300 pylipd-1.2.2/pylipd/globals/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.2.2/pylipd/globals/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)      409 2023-04-10 19:03:17.000000 pylipd-1.2.2/pylipd/globals/blacklist.py
+-rw-r--r--   0 varun      (502) staff       (20)     3673 2023-04-11 06:17:21.000000 pylipd-1.2.2/pylipd/globals/queries.py
+-rw-r--r--   0 varun      (502) staff       (20)    14643 2023-04-10 19:06:28.000000 pylipd-1.2.2/pylipd/globals/schema.py
+-rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.2.2/pylipd/globals/urls.py
+-rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.2.2/pylipd/legacy_utils.py
+-rw-r--r--   0 varun      (502) staff       (20)    30710 2023-04-11 06:32:51.000000 pylipd-1.2.2/pylipd/lipd.py
+-rw-r--r--   0 varun      (502) staff       (20)    43172 2023-04-11 03:12:51.000000 pylipd-1.2.2/pylipd/lipd_to_rdf.py
+-rw-r--r--   0 varun      (502) staff       (20)     1576 2023-04-11 03:11:49.000000 pylipd-1.2.2/pylipd/multi_processing.py
+-rw-r--r--   0 varun      (502) staff       (20)    22021 2023-04-11 03:13:16.000000 pylipd-1.2.2/pylipd/rdf_to_lipd.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 06:34:45.265617 pylipd-1.2.2/pylipd/series/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.2.2/pylipd/series/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.2.2/pylipd/series/regexes.py
+-rw-r--r--   0 varun      (502) staff       (20)     2259 2023-04-11 05:52:03.000000 pylipd-1.2.2/pylipd/test.py
+-rw-r--r--   0 varun      (502) staff       (20)     5306 2023-04-11 06:31:14.000000 pylipd-1.2.2/pylipd/usage.py
+-rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.2.2/pylipd/utils.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-11 06:34:45.266415 pylipd-1.2.2/pylipd.egg-info/
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-11 06:34:45.000000 pylipd-1.2.2/pylipd.egg-info/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      616 2023-04-11 06:34:45.000000 pylipd-1.2.2/pylipd.egg-info/SOURCES.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-11 06:34:45.000000 pylipd-1.2.2/pylipd.egg-info/dependency_links.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.2.2/pylipd.egg-info/not-zip-safe
+-rw-r--r--   0 varun      (502) staff       (20)       35 2023-04-11 06:34:45.000000 pylipd-1.2.2/pylipd.egg-info/requires.txt
+-rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-11 06:34:45.000000 pylipd-1.2.2/pylipd.egg-info/top_level.txt
+-rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.2.2/pyproject.toml
+-rw-r--r--   0 varun      (502) staff       (20)      693 2023-04-11 06:34:45.266801 pylipd-1.2.2/setup.cfg
+-rw-r--r--   0 varun      (502) staff       (20)      973 2023-04-11 06:33:10.000000 pylipd-1.2.2/setup.py
```

### Comparing `pylipd-1.2.1/LICENSE` & `pylipd-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.1/PKG-INFO` & `pylipd-1.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.2.1
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.2.2
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.2.1/README.md` & `pylipd-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.1/pylipd/globals/schema.py` & `pylipd-1.2.2/pylipd/globals/schema.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.1/pylipd/legacy_utils.py` & `pylipd-1.2.2/pylipd/legacy_utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.1/pylipd/lipd.py` & `pylipd-1.2.2/pylipd/lipd.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import tempfile
 import pandas as pd
 import random
 import string
 import io
 
 from rdflib import ConjunctiveGraph, Namespace, URIRef
+from pylipd.globals.queries import QUERY_BIBLIO, QUERY_DSID, QUERY_DSNAME, QUERY_ENSEMBLE_TABLE
 from pylipd.multi_processing import multi_convert_to_pickle, multi_convert_to_rdf
 
 from pylipd.rdf_to_lipd import RDFToLiPD
 from pylipd.legacy_utils import LiPD_Legacy
 from pylipd.utils import sanitizeId, sparql_results_to_df
 
 #import bibtexparser
@@ -523,44 +524,15 @@
             elif pub_type == 'chapter' or pub_type == 'report':
                 bib = BibliographyData({citation_key:Entry('inbook',entries)})
             elif pub_type == 'misc':
                 bib = BibliographyData({citation_key:Entry('misc',entries)})
             
             return bib  
         
-        query = """SELECT ?dsname ?title (GROUP_CONCAT(?authorName;separator=" and ") as ?authors) 
-                     ?doi ?pubyear ?year ?journal ?volume ?issue ?pages ?type ?publisher ?report ?citeKey ?edition ?institution ?url ?url2
-                     WHERE { 
-                         ?ds a le:Dataset .
-                         ?ds le:name ?dsname .
-                         ?ds le:publishedIn ?pub .
-                         OPTIONAL{?pub le:hasDOI ?doi .}
-                         OPTIONAL{
-                             ?pub le:author ?author .
-                             ?author le:name ?authorName .
-                         }
-                         OPTIONAL{?pub le:publicationYear ?year .}
-                         OPTIONAL{?pub le:pubYear ?pubyear .}
-                         OPTIONAL{?pub le:title ?title .}
-                         OPTIONAL{?pub le:journal ?journal .}
-                         OPTIONAL{?pub le:volume ?volume .}
-                         OPTIONAL{?pub le:issue ?issue .}
-                         OPTIONAL{?pub le:pages ?pages .}
-                         OPTIONAL{?pub le:type ?type .}
-                         OPTIONAL{?pub le:publisher ?publisher .}
-                         OPTIONAL{?pub le:report ?report .}
-                         OPTIONAL{?pub le:citeKey ?citeKey .}
-                         OPTIONAL{?pub le:edition ?edition .}
-                         OPTIONAL{?pub le:institution ?institution .}
-                         OPTIONAL{?pub le:hasLink ?url .}
-                         OPTIONAL{?pub le:url ?url2 .}
-                     }
-                     GROUP BY ?pub ?dsname ?title ?doi ?year ?pubyear ?journal ?volume ?issue ?pages ?type ?publisher ?report ?citeKey ?edition ?institution ?url ?url2
-         """
-        result, df = self.query(query)
+        result, df = self.query(QUERY_BIBLIO)
         
         bibs = []
 
         for idx,row in df.iterrows():
             if remote == True:
                 try: 
                     f = (crossref.get_bib(row['doi']))
@@ -861,21 +833,15 @@
             lipd = LiPD()
             lipd.load([
                 "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
                 "../examples/data/MD98_2181.Stott.2007.lpd"
             ])
             print(lipd.get_all_dataset_names())
         '''        
-        query = f"""
-            SELECT ?dsname WHERE {{ 
-                ?ds a le:Dataset .
-                ?ds le:name ?dsname
-            }}
-            """
-        qres, qres_df = self.query(query)
+        qres, qres_df = self.query(QUERY_DSNAME)
         return [sanitizeId(row.dsname) for row in qres]
 
     def get_all_dataset_ids(self):
         '''Get all Dataset ids
         
         Returns
         -------
@@ -896,28 +862,85 @@
             # Fetch LiPD data from remote RDF Graph
             lipd = LiPD()
             lipd.load([
                 "../examples/data/Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001.lpd",
                 "../examples/data/MD98_2181.Stott.2007.lpd"
             ])
             print(lipd.get_all_dataset_ids())
-        '''        
-        query = """
-            SELECT ?dsid WHERE {{ 
-                ?ds a le:Dataset .
-                OPTIONAL{?ds le:datasetId ?dsid}
-            }}
-            """
-        qres, qres_df = self.query(query)
+        '''
+        qres, qres_df = self.query(QUERY_DSID)
         return [sanitizeId(row.dsid) for row in qres]
     
+
     def search_datasets(variableName=[ ], archiveType=[ ], proxy=[ ], resolution = [ ],
                     ageUnits = [ ], ageBound = [ ], ageBoundType = [ ], 
                     lat = [ ], lon = [ ], alt = [ ], 
                     print_response = True, download_lipd = True,
                     download_folder = 'default'):
         pass
 
 
-    def find_ensemble_table_for_variable(self, ensemble_table):
-        pass
+    def get_ensemble_tables(self, archiveType, varName, timeVarName, depthVarName, ensembleVarName, ensembleDepthVarName):
+        '''Gets ensemble tables from the LiPD graph
+
+        Parameters
+        ----------
+
+        archiveType : str
+            archive type (Set to ".*" to match all archive types)
+        varName : str
+            variable name (Set to ".*" to match all variable names)
+        timeVarName : str
+            time variable name (Set to ".*" to match all time variable names)
+        depthVarName : str
+            depth variable name (Set to ".*" to match all depth variable names)
+        ensembleVarName : str
+            ensemble variable name (Set to ".*" to match all ensemble variable names)
+        ensembleDepthVarName : str
+            ensemble depth variable name (Set to ".*" to match all ensemble depth variable names)
+
+        Returns
+        -------
+
+        ensemble_tables : dataframe
+            A dataframe containing the ensemble tables
+
+
+        Examples
+        --------
+
+        .. ipython:: python
+            :okwarning:
+            :okexcept:
+
+            from pylipd.lipd import LiPD
+
+            lipd = LiPD()
+            lipd.load([
+                "../examples/data/ODP846.Lawrence.2006.lpd"
+            ])
+            all_datasets = lipd.get_all_dataset_names()
+            print("Loaded datasets: " + str(all_datasets))
+
+            ens_df = lipd.get_ensemble_tables(
+                archiveType=".*",
+                varName="c37",
+                timeVarName="age",
+                depthVarName="depth",
+                ensembleVarName="age",
+                ensembleDepthVarName="depth"
+            )
+            print("Ensemble tables:")
+            print(ens_df)
+        '''
+       
+        query = QUERY_ENSEMBLE_TABLE
+        query = query.replace("[archiveType]", archiveType)
+        query = query.replace("[varName]", varName)
+        query = query.replace("[timeVarName]", timeVarName)
+        query = query.replace("[depthVarName]", depthVarName)
+        query = query.replace("[ensembleVarName]", ensembleVarName)
+        query = query.replace("[ensembleDepthVarName]", ensembleDepthVarName)
+
+        qres, qres_df = self.query(query)
+        return qres_df
```

### Comparing `pylipd-1.2.1/pylipd/lipd_to_rdf.py` & `pylipd-1.2.2/pylipd/lipd_to_rdf.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.1/pylipd/multi_processing.py` & `pylipd-1.2.2/pylipd/multi_processing.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.1/pylipd/rdf_to_lipd.py` & `pylipd-1.2.2/pylipd/rdf_to_lipd.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.1/pylipd/series/regexes.py` & `pylipd-1.2.2/pylipd/series/regexes.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.1/pylipd/test.py` & `pylipd-1.2.2/pylipd/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,8 +55,8 @@
         ?ensdepthvar le:hasValues ?ensdepthval .
             OPTIONAL{?ensdepthvar le:hasUnits ?ensdepthunits .}
         
     }
         """  
     
     result, result_df = lipd.query(query)
-    print(result_df["varname"])
+    print(result_df)
```

### Comparing `pylipd-1.2.1/pylipd/usage.py` & `pylipd-1.2.2/pylipd/usage.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,31 +63,40 @@
 
 # Load from local
 lipd = LiPD()
 lipdfiles = [local_lipd_dir + "/" + dsname + ".lpd" for dsname in dsnames]
 #print(lipdfiles)
 
 #lipd.load(lipdfiles)
-#lipd.load_from_dir("examples/data")
-lipd.load(["/Users/varun/Downloads/ODP846.Lawrence.2006.lpd"])
+lipd.load_from_dir("examples/data")
 print(lipd.get_all_dataset_names())
-print(lipd.get_all_dataset_ids())
+#print(lipd.get_all_dataset_ids())
+ens_df = lipd.get_ensemble_tables(
+    archiveType=".*",
+    varName="c37",
+    timeVarName="age",
+    depthVarName="depth",
+    ensembleVarName="age",
+    ensembleDepthVarName="depth"
+)
+print(ens_df)
+exit()
 
 #lipd.load(["/Users/varun/Downloads/Arc-LakeNataujärvi.Ojala.2005.lpd"])
 #print(lipd.get_all_dataset_names())
 
 ts_list = lipd.get_timeseries(lipd.get_all_dataset_names())
 for dsname, tsos in ts_list.items():
     for tso in tsos:
         if 'paleoData_variableName' in tso:
             print(dsname+': '+str(tso['paleoData_variableName'])+': '+tso['archiveType'])
 
 
 # Fetch LiPD data from remote RDF Graph
-lipd.set_endpoint(remote_lipd_endpoint)
+#lipd.set_endpoint(remote_lipd_endpoint)
 #lipd.load_remote_datasets(remote_dsnames)
 
 # Convert to TSO object (as before)
 '''
 ts_list_remote = lipd.get_timeseries(lipd.get_all_dataset_names())
 for dsname, tsos in ts_list_remote.items():
     for tso in tsos:
@@ -108,14 +117,15 @@
 lpd2 = LiPD()
 lpd2.load([lipdfile])
 ts_list_remote = lpd2.get_timeseries(lpd2.get_all_dataset_names())
 for dsname, tsos in ts_list_remote.items():
     for tso in tsos:
         print(dsname+': '+str(tso['paleoData_variableName'])+': '+tso['archiveType'])
 
+print(lpd2.get_ensemble_tables())
 exit()
 
 print("After popping..")
 print(lipd.get_all_dataset_names())
 ts_list_remote = lipd.get_timeseries(lipd.get_all_dataset_names())
 for dsname, tsos in ts_list_remote.items():
     for tso in tsos:
```

### Comparing `pylipd-1.2.1/pylipd/utils.py` & `pylipd-1.2.2/pylipd/utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.2.1/pylipd.egg-info/PKG-INFO` & `pylipd-1.2.2/pylipd.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.2.1
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.2.2
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.2.1/pylipd.egg-info/SOURCES.txt` & `pylipd-1.2.2/pylipd.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ./pylipd/multi_processing.py
 ./pylipd/rdf_to_lipd.py
 ./pylipd/test.py
 ./pylipd/usage.py
 ./pylipd/utils.py
 ./pylipd/globals/__init__.py
 ./pylipd/globals/blacklist.py
+./pylipd/globals/queries.py
 ./pylipd/globals/schema.py
 ./pylipd/globals/urls.py
 ./pylipd/series/__init__.py
 ./pylipd/series/regexes.py
 pylipd.egg-info/PKG-INFO
 pylipd.egg-info/SOURCES.txt
 pylipd.egg-info/dependency_links.txt
```

### Comparing `pylipd-1.2.1/setup.cfg` & `pylipd-1.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pylipd
-version = 1.2.1
+version = 1.2.2
 author = Varun Ratnakar
 author_email = varunratnakar@gmail.com
 description = Python utilities for handling LiPD data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/linkedearth/pylipd
 project_urls =
```

### Comparing `pylipd-1.2.1/setup.py` & `pylipd-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import setup, find_packages
 
 
-version = '1.2.1'
+version = '1.2.2'
 
 # Read the readme file contents into variable
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='pylipd',
```

