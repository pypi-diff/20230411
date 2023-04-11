# Comparing `tmp/cellar_extractor-1.0.48.tar.gz` & `tmp/cellar_extractor-1.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellar_extractor-1.0.48.tar", last modified: Tue Apr 11 13:57:34 2023, max compression
+gzip compressed data, was "cellar_extractor-1.0.49.tar", last modified: Tue Apr 11 14:51:27 2023, max compression
```

## Comparing `cellar_extractor-1.0.48.tar` & `cellar_extractor-1.0.49.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 13:57:34.975862 cellar_extractor-1.0.48/
--rw-rw-rw-   0        0        0     6851 2023-04-11 13:57:34.974862 cellar_extractor-1.0.48/PKG-INFO
--rw-rw-rw-   0        0        0     6361 2023-04-11 13:57:30.000000 cellar_extractor-1.0.48/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 13:57:34.964862 cellar_extractor-1.0.48/cellar_extractor/
--rw-rw-rw-   0        0        0      704 2023-04-10 10:34:04.000000 cellar_extractor-1.0.48/cellar_extractor/Testing_file.py
--rw-rw-rw-   0        0        0      163 2023-04-11 13:37:46.000000 cellar_extractor-1.0.48/cellar_extractor/__init__.py
--rw-rw-rw-   0        0        0     3179 2023-04-11 13:57:30.000000 cellar_extractor-1.0.48/cellar_extractor/cellar.py
--rw-rw-rw-   0        0        0     1005 2022-12-16 13:13:01.000000 cellar_extractor-1.0.48/cellar_extractor/cellar_extra_extract.py
--rw-rw-rw-   0        0        0     5227 2023-02-26 11:01:55.000000 cellar_extractor-1.0.48/cellar_extractor/cellar_queries.py
--rw-rw-rw-   0        0        0    11264 2023-01-09 12:41:12.000000 cellar_extractor-1.0.48/cellar_extractor/citations_adder.py
--rw-rw-rw-   0        0        0     1334 2022-11-18 14:10:12.000000 cellar_extractor-1.0.48/cellar_extractor/csv_extractor.py
--rw-rw-rw-   0        0        0    16726 2023-03-24 12:49:14.000000 cellar_extractor-1.0.48/cellar_extractor/eurlex_scraping.py
--rw-rw-rw-   0        0        0     6403 2023-03-24 12:49:14.000000 cellar_extractor-1.0.48/cellar_extractor/fulltext_saving.py
--rw-rw-rw-   0        0        0     5411 2022-12-06 21:17:47.000000 cellar_extractor-1.0.48/cellar_extractor/json_to_csv.py
--rw-rw-rw-   0        0        0     1040 2023-04-11 13:52:52.000000 cellar_extractor-1.0.48/cellar_extractor/nodes_and_edges.py
--rw-rw-rw-   0        0        0     6834 2022-11-15 12:42:07.000000 cellar_extractor-1.0.48/cellar_extractor/sparql.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:57:34.972862 cellar_extractor-1.0.48/cellar_extractor.egg-info/
--rw-rw-rw-   0        0        0     6851 2023-04-11 13:57:34.000000 cellar_extractor-1.0.48/cellar_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-04-11 13:57:34.000000 cellar_extractor-1.0.48/cellar_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 13:57:34.000000 cellar_extractor-1.0.48/cellar_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-04-11 13:57:34.000000 cellar_extractor-1.0.48/cellar_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-11 13:57:34.000000 cellar_extractor-1.0.48/cellar_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 13:57:34.975862 cellar_extractor-1.0.48/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-04-11 13:57:30.000000 cellar_extractor-1.0.48/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:51:27.066101 cellar_extractor-1.0.49/
+-rw-rw-rw-   0        0        0     6964 2023-04-11 14:51:27.065101 cellar_extractor-1.0.49/PKG-INFO
+-rw-rw-rw-   0        0        0     6474 2023-04-11 14:51:21.000000 cellar_extractor-1.0.49/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 14:51:27.055101 cellar_extractor-1.0.49/cellar_extractor/
+-rw-rw-rw-   0        0        0      704 2023-04-10 10:34:04.000000 cellar_extractor-1.0.49/cellar_extractor/Testing_file.py
+-rw-rw-rw-   0        0        0      163 2023-04-11 13:37:46.000000 cellar_extractor-1.0.49/cellar_extractor/__init__.py
+-rw-rw-rw-   0        0        0     3329 2023-04-11 14:51:21.000000 cellar_extractor-1.0.49/cellar_extractor/cellar.py
+-rw-rw-rw-   0        0        0     1005 2022-12-16 13:13:01.000000 cellar_extractor-1.0.49/cellar_extractor/cellar_extra_extract.py
+-rw-rw-rw-   0        0        0     5227 2023-02-26 11:01:55.000000 cellar_extractor-1.0.49/cellar_extractor/cellar_queries.py
+-rw-rw-rw-   0        0        0    11264 2023-01-09 12:41:12.000000 cellar_extractor-1.0.49/cellar_extractor/citations_adder.py
+-rw-rw-rw-   0        0        0     1334 2022-11-18 14:10:12.000000 cellar_extractor-1.0.49/cellar_extractor/csv_extractor.py
+-rw-rw-rw-   0        0        0    16726 2023-03-24 12:49:14.000000 cellar_extractor-1.0.49/cellar_extractor/eurlex_scraping.py
+-rw-rw-rw-   0        0        0     6403 2023-03-24 12:49:14.000000 cellar_extractor-1.0.49/cellar_extractor/fulltext_saving.py
+-rw-rw-rw-   0        0        0     5411 2022-12-06 21:17:47.000000 cellar_extractor-1.0.49/cellar_extractor/json_to_csv.py
+-rw-rw-rw-   0        0        0     1040 2023-04-11 13:52:52.000000 cellar_extractor-1.0.49/cellar_extractor/nodes_and_edges.py
+-rw-rw-rw-   0        0        0     6834 2022-11-15 12:42:07.000000 cellar_extractor-1.0.49/cellar_extractor/sparql.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:51:27.064102 cellar_extractor-1.0.49/cellar_extractor.egg-info/
+-rw-rw-rw-   0        0        0     6964 2023-04-11 14:51:26.000000 cellar_extractor-1.0.49/cellar_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-04-11 14:51:27.000000 cellar_extractor-1.0.49/cellar_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 14:51:26.000000 cellar_extractor-1.0.49/cellar_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-04-11 14:51:26.000000 cellar_extractor-1.0.49/cellar_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-11 14:51:26.000000 cellar_extractor-1.0.49/cellar_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 14:51:27.067101 cellar_extractor-1.0.49/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-04-11 14:51:21.000000 cellar_extractor-1.0.49/setup.py
```

### Comparing `cellar_extractor-1.0.48/PKG-INFO` & `cellar_extractor-1.0.49/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellar_extractor
-Version: 1.0.48
+Version: 1.0.49
 Summary: Library for extracting cellar data
 Home-page: UNKNOWN
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
@@ -110,15 +110,16 @@
         <li><strong>password: string, optional, default empty string</strong></li>
         The password to the eurlex webservices.
         <br>
     </ul>
     <li><code>get_nodes_and_edges_lists</code></li>
     <ul>
         <li><strong>df: DataFrame object, required, default None</strong></li>
-        DataFrame of cellar metadata acquired from the get_cellar_extra method.
+        DataFrame of cellar metadata acquired from the get_cellar_extra method with eurlex webservice credentials passed.
+        This method will only work on dataframes with citations data.
     </ul>
 </ol>
 
 
 ## Examples
 ```
 import cellar_extractor as cell
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.48 Summary: Library
+Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.49 Summary: Library
 for extracting cellar data Home-page: UNKNOWN Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Platform: UNKNOWN Description-Content-Type: text/
 markdown ## Cellar extractor This library contains two functions to get cellar
 case law data from eurlex. ## Version Python 3.9 ## Contributors
@@ -59,15 +59,16 @@
           o username: string, optional, default empty string
           o The username to the eurlex webservices.
           o password: string, optional, default empty string
           o The password to the eurlex webservices.
    4. get_nodes_and_edges_lists
           o df: DataFrame object, required, default None
           o DataFrame of cellar metadata acquired from the get_cellar_extra
-            method.
+            method with eurlex webservice credentials passed. This method will
+            only work on dataframes with citations data.
 ## Examples ``` import cellar_extractor as cell Below are examples for in-file
 saving: cell.get_cellar(save_file='y', max_ecli=200, sd='2022-01-01',
 file_format='csv') cell.get_cellar_extra(max_ecli=100, sd='2022-01-01',
 threads=10) Below are examples for in-memory saving: df = cell.get_cellar
 (save_file='n', file_format='csv', sd='2022-01-01', max_ecli=1000) df,json =
 cell.get_cellar_extra(save_file='n', max_ecli=100, sd='2022-01-01', threads=10)
 ``` ## License [![License: Apache 2.0](https://img.shields.io/github/license/
```

### Comparing `cellar_extractor-1.0.48/README.md` & `cellar_extractor-1.0.49/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,16 @@
         <li><strong>password: string, optional, default empty string</strong></li>
         The password to the eurlex webservices.
         <br>
     </ul>
     <li><code>get_nodes_and_edges_lists</code></li>
     <ul>
         <li><strong>df: DataFrame object, required, default None</strong></li>
-        DataFrame of cellar metadata acquired from the get_cellar_extra method.
+        DataFrame of cellar metadata acquired from the get_cellar_extra method with eurlex webservice credentials passed.
+        This method will only work on dataframes with citations data.
     </ul>
 </ol>
 
 
 ## Examples
 ```
 import cellar_extractor as cell
```

#### html2text {}

```diff
@@ -53,15 +53,16 @@
           o username: string, optional, default empty string
           o The username to the eurlex webservices.
           o password: string, optional, default empty string
           o The password to the eurlex webservices.
    4. get_nodes_and_edges_lists
           o df: DataFrame object, required, default None
           o DataFrame of cellar metadata acquired from the get_cellar_extra
-            method.
+            method with eurlex webservice credentials passed. This method will
+            only work on dataframes with citations data.
 ## Examples ``` import cellar_extractor as cell Below are examples for in-file
 saving: cell.get_cellar(save_file='y', max_ecli=200, sd='2022-01-01',
 file_format='csv') cell.get_cellar_extra(max_ecli=100, sd='2022-01-01',
 threads=10) Below are examples for in-memory saving: df = cell.get_cellar
 (save_file='n', file_format='csv', sd='2022-01-01', max_ecli=1000) df,json =
 cell.get_cellar_extra(save_file='n', max_ecli=100, sd='2022-01-01', threads=10)
 ``` ## License [![License: Apache 2.0](https://img.shields.io/github/license/
```

### Comparing `cellar_extractor-1.0.48/cellar_extractor/Testing_file.py` & `cellar_extractor-1.0.49/cellar_extractor/Testing_file.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.48/cellar_extractor/cellar.py` & `cellar_extractor-1.0.49/cellar_extractor/cellar.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,9 +72,13 @@
         return data,json
 
 def get_nodes_and_edges_lists(df = None):
     if df is None:
         print("No dataframe passed!")
         return
     else:
-        nodes,edges = get_nodes_and_edges(df)
+        try:
+            nodes,edges = get_nodes_and_edges(df)
+        except:
+            print('Something went wrong. Nodes and edges creation unsuccessful.')
+            return False,False
         return nodes,edges
```

### Comparing `cellar_extractor-1.0.48/cellar_extractor/cellar_extra_extract.py` & `cellar_extractor-1.0.49/cellar_extractor/cellar_extra_extract.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.48/cellar_extractor/cellar_queries.py` & `cellar_extractor-1.0.49/cellar_extractor/cellar_queries.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.48/cellar_extractor/citations_adder.py` & `cellar_extractor-1.0.49/cellar_extractor/citations_adder.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.48/cellar_extractor/csv_extractor.py` & `cellar_extractor-1.0.49/cellar_extractor/csv_extractor.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.48/cellar_extractor/eurlex_scraping.py` & `cellar_extractor-1.0.49/cellar_extractor/eurlex_scraping.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.48/cellar_extractor/fulltext_saving.py` & `cellar_extractor-1.0.49/cellar_extractor/fulltext_saving.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.48/cellar_extractor/json_to_csv.py` & `cellar_extractor-1.0.49/cellar_extractor/json_to_csv.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.48/cellar_extractor/nodes_and_edges.py` & `cellar_extractor-1.0.49/cellar_extractor/nodes_and_edges.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.48/cellar_extractor/sparql.py` & `cellar_extractor-1.0.49/cellar_extractor/sparql.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.48/cellar_extractor.egg-info/PKG-INFO` & `cellar_extractor-1.0.49/cellar_extractor.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellar-extractor
-Version: 1.0.48
+Version: 1.0.49
 Summary: Library for extracting cellar data
 Home-page: UNKNOWN
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
@@ -110,15 +110,16 @@
         <li><strong>password: string, optional, default empty string</strong></li>
         The password to the eurlex webservices.
         <br>
     </ul>
     <li><code>get_nodes_and_edges_lists</code></li>
     <ul>
         <li><strong>df: DataFrame object, required, default None</strong></li>
-        DataFrame of cellar metadata acquired from the get_cellar_extra method.
+        DataFrame of cellar metadata acquired from the get_cellar_extra method with eurlex webservice credentials passed.
+        This method will only work on dataframes with citations data.
     </ul>
 </ol>
 
 
 ## Examples
 ```
 import cellar_extractor as cell
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.48 Summary: Library
+Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.49 Summary: Library
 for extracting cellar data Home-page: UNKNOWN Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Platform: UNKNOWN Description-Content-Type: text/
 markdown ## Cellar extractor This library contains two functions to get cellar
 case law data from eurlex. ## Version Python 3.9 ## Contributors
@@ -59,15 +59,16 @@
           o username: string, optional, default empty string
           o The username to the eurlex webservices.
           o password: string, optional, default empty string
           o The password to the eurlex webservices.
    4. get_nodes_and_edges_lists
           o df: DataFrame object, required, default None
           o DataFrame of cellar metadata acquired from the get_cellar_extra
-            method.
+            method with eurlex webservice credentials passed. This method will
+            only work on dataframes with citations data.
 ## Examples ``` import cellar_extractor as cell Below are examples for in-file
 saving: cell.get_cellar(save_file='y', max_ecli=200, sd='2022-01-01',
 file_format='csv') cell.get_cellar_extra(max_ecli=100, sd='2022-01-01',
 threads=10) Below are examples for in-memory saving: df = cell.get_cellar
 (save_file='n', file_format='csv', sd='2022-01-01', max_ecli=1000) df,json =
 cell.get_cellar_extra(save_file='n', max_ecli=100, sd='2022-01-01', threads=10)
 ``` ## License [![License: Apache 2.0](https://img.shields.io/github/license/
```

### Comparing `cellar_extractor-1.0.48/cellar_extractor.egg-info/SOURCES.txt` & `cellar_extractor-1.0.49/cellar_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.48/setup.py` & `cellar_extractor-1.0.49/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='cellar_extractor',
     packages=find_packages(include=['cellar_extractor']),
-    version='1.0.48',
+    version='1.0.49',
     description='Library for extracting cellar data',
     author='LawTech Lab',
     license='MIT',
     install_requires=['bs4','SPARQLWrapper==2.0.0', 'requests==2.26.0', 'pandas','lxml==4.6.3','xmltodict==0.13.0','tqdm'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['cellar', 'extractor'],
     long_description=long_descr,
```

