# Comparing `tmp/cellar_extractor-1.0.47.tar.gz` & `tmp/cellar_extractor-1.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellar_extractor-1.0.47.tar", last modified: Tue Apr 11 13:53:55 2023, max compression
+gzip compressed data, was "cellar_extractor-1.0.48.tar", last modified: Tue Apr 11 13:57:34 2023, max compression
```

## Comparing `cellar_extractor-1.0.47.tar` & `cellar_extractor-1.0.48.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 13:53:55.734538 cellar_extractor-1.0.47/
--rw-rw-rw-   0        0        0     7020 2023-04-11 13:53:55.733538 cellar_extractor-1.0.47/PKG-INFO
--rw-rw-rw-   0        0        0     6530 2023-04-10 10:34:04.000000 cellar_extractor-1.0.47/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 13:53:55.722538 cellar_extractor-1.0.47/cellar_extractor/
--rw-rw-rw-   0        0        0      704 2023-04-10 10:34:04.000000 cellar_extractor-1.0.47/cellar_extractor/Testing_file.py
--rw-rw-rw-   0        0        0      163 2023-04-11 13:37:46.000000 cellar_extractor-1.0.47/cellar_extractor/__init__.py
--rw-rw-rw-   0        0        0     3423 2023-04-10 10:34:04.000000 cellar_extractor-1.0.47/cellar_extractor/cellar.py
--rw-rw-rw-   0        0        0     1005 2022-12-16 13:13:01.000000 cellar_extractor-1.0.47/cellar_extractor/cellar_extra_extract.py
--rw-rw-rw-   0        0        0     5227 2023-02-26 11:01:55.000000 cellar_extractor-1.0.47/cellar_extractor/cellar_queries.py
--rw-rw-rw-   0        0        0    11264 2023-01-09 12:41:12.000000 cellar_extractor-1.0.47/cellar_extractor/citations_adder.py
--rw-rw-rw-   0        0        0     1334 2022-11-18 14:10:12.000000 cellar_extractor-1.0.47/cellar_extractor/csv_extractor.py
--rw-rw-rw-   0        0        0    16726 2023-03-24 12:49:14.000000 cellar_extractor-1.0.47/cellar_extractor/eurlex_scraping.py
--rw-rw-rw-   0        0        0     6403 2023-03-24 12:49:14.000000 cellar_extractor-1.0.47/cellar_extractor/fulltext_saving.py
--rw-rw-rw-   0        0        0     5411 2022-12-06 21:17:47.000000 cellar_extractor-1.0.47/cellar_extractor/json_to_csv.py
--rw-rw-rw-   0        0        0     1040 2023-04-11 13:52:52.000000 cellar_extractor-1.0.47/cellar_extractor/nodes_and_edges.py
--rw-rw-rw-   0        0        0     6834 2022-11-15 12:42:07.000000 cellar_extractor-1.0.47/cellar_extractor/sparql.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:53:55.731538 cellar_extractor-1.0.47/cellar_extractor.egg-info/
--rw-rw-rw-   0        0        0     7020 2023-04-11 13:53:55.000000 cellar_extractor-1.0.47/cellar_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-04-11 13:53:55.000000 cellar_extractor-1.0.47/cellar_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 13:53:55.000000 cellar_extractor-1.0.47/cellar_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-04-11 13:53:55.000000 cellar_extractor-1.0.47/cellar_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-11 13:53:55.000000 cellar_extractor-1.0.47/cellar_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 13:53:55.734538 cellar_extractor-1.0.47/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-04-11 13:53:49.000000 cellar_extractor-1.0.47/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:57:34.975862 cellar_extractor-1.0.48/
+-rw-rw-rw-   0        0        0     6851 2023-04-11 13:57:34.974862 cellar_extractor-1.0.48/PKG-INFO
+-rw-rw-rw-   0        0        0     6361 2023-04-11 13:57:30.000000 cellar_extractor-1.0.48/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 13:57:34.964862 cellar_extractor-1.0.48/cellar_extractor/
+-rw-rw-rw-   0        0        0      704 2023-04-10 10:34:04.000000 cellar_extractor-1.0.48/cellar_extractor/Testing_file.py
+-rw-rw-rw-   0        0        0      163 2023-04-11 13:37:46.000000 cellar_extractor-1.0.48/cellar_extractor/__init__.py
+-rw-rw-rw-   0        0        0     3179 2023-04-11 13:57:30.000000 cellar_extractor-1.0.48/cellar_extractor/cellar.py
+-rw-rw-rw-   0        0        0     1005 2022-12-16 13:13:01.000000 cellar_extractor-1.0.48/cellar_extractor/cellar_extra_extract.py
+-rw-rw-rw-   0        0        0     5227 2023-02-26 11:01:55.000000 cellar_extractor-1.0.48/cellar_extractor/cellar_queries.py
+-rw-rw-rw-   0        0        0    11264 2023-01-09 12:41:12.000000 cellar_extractor-1.0.48/cellar_extractor/citations_adder.py
+-rw-rw-rw-   0        0        0     1334 2022-11-18 14:10:12.000000 cellar_extractor-1.0.48/cellar_extractor/csv_extractor.py
+-rw-rw-rw-   0        0        0    16726 2023-03-24 12:49:14.000000 cellar_extractor-1.0.48/cellar_extractor/eurlex_scraping.py
+-rw-rw-rw-   0        0        0     6403 2023-03-24 12:49:14.000000 cellar_extractor-1.0.48/cellar_extractor/fulltext_saving.py
+-rw-rw-rw-   0        0        0     5411 2022-12-06 21:17:47.000000 cellar_extractor-1.0.48/cellar_extractor/json_to_csv.py
+-rw-rw-rw-   0        0        0     1040 2023-04-11 13:52:52.000000 cellar_extractor-1.0.48/cellar_extractor/nodes_and_edges.py
+-rw-rw-rw-   0        0        0     6834 2022-11-15 12:42:07.000000 cellar_extractor-1.0.48/cellar_extractor/sparql.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:57:34.972862 cellar_extractor-1.0.48/cellar_extractor.egg-info/
+-rw-rw-rw-   0        0        0     6851 2023-04-11 13:57:34.000000 cellar_extractor-1.0.48/cellar_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-04-11 13:57:34.000000 cellar_extractor-1.0.48/cellar_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 13:57:34.000000 cellar_extractor-1.0.48/cellar_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-04-11 13:57:34.000000 cellar_extractor-1.0.48/cellar_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-11 13:57:34.000000 cellar_extractor-1.0.48/cellar_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 13:57:34.975862 cellar_extractor-1.0.48/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-04-11 13:57:30.000000 cellar_extractor-1.0.48/setup.py
```

### Comparing `cellar_extractor-1.0.47/PKG-INFO` & `cellar_extractor-1.0.48/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellar_extractor
-Version: 1.0.47
+Version: 1.0.48
 Summary: Library for extracting cellar data
 Home-page: UNKNOWN
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
@@ -65,16 +65,16 @@
     <br>
     <li><code>get_cellar_extra</code></li>
     Gets all the ECLI data from the eurlex sparql endpoint, and on top of that scrapes the eurlex websites to acquire 
     the full text, keywords, case law directory code and eurovoc identifiers. If the user does have an eurlex account with access to the eurlex webservices, he can also 
     pass his webservices login credentials to the method, in order to extract data about works citing work and works 
     being cited by work. The full text is returned as a JSON file, rest of data as a CSV.  Can be in-memory or as saved files.
     <li><code>get_nodes_and_edges_lists</code></li>
-    Gets 2 dataframe objects, one for the nodes and edges of the citations within the passed dataframe.
-    Allows the creation of a network graph of the citations. Can be saved in-memory or in the data folder as csv files.
+    Gets 2 list objects, one for the nodes and edges of the citations within the passed dataframe.
+    Allows the creation of a network graph of the citations. Can only be returned in-memory.
     <br>
 </ol>
 
 ## What are the parameters?
 <ol>
     <li><code>get_cellar</code></li>
     <strong>Parameters:</strong>
@@ -111,16 +111,14 @@
         The password to the eurlex webservices.
         <br>
     </ul>
     <li><code>get_nodes_and_edges_lists</code></li>
     <ul>
         <li><strong>df: DataFrame object, required, default None</strong></li>
         DataFrame of cellar metadata acquired from the get_cellar_extra method.
-        <li><strong>save_file: ['y', 'n'],optional, default 'y'</strong></li>
-        Save data in a data folder, or return in-memory.
     </ul>
 </ol>
 
 
 ## Examples
 ```
 import cellar_extractor as cell
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.47 Summary: Library
+Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.48 Summary: Library
 for extracting cellar data Home-page: UNKNOWN Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Platform: UNKNOWN Description-Content-Type: text/
 markdown ## Cellar extractor This library contains two functions to get cellar
 case law data from eurlex. ## Version Python 3.9 ## Contributors
@@ -18,18 +18,17 @@
       law directory code and eurovoc identifiers. If the user does have an
       eurlex account with access to the eurlex webservices, he can also pass
       his webservices login credentials to the method, in order to extract data
       about works citing work and works being cited by work. The full text is
       returned as a JSON file, rest of data as a CSV. Can be in-memory or as
       saved files.
    5. get_nodes_and_edges_lists
-   6. Gets 2 dataframe objects, one for the nodes and edges of the citations
-      within the passed dataframe. Allows the creation of a network graph of
-      the citations. Can be saved in-memory or in the data folder as csv files.
-
+   6. Gets 2 list objects, one for the nodes and edges of the citations within
+      the passed dataframe. Allows the creation of a network graph of the
+      citations. Can only be returned in-memory.
 ## What are the parameters?
    1. get_cellar
    2. Parameters:
           o max_ecli: int, optional, default 100
           o Maximum number of ECLIs to retrieve.
           o sd: date, optional, default '2022-05-01'
           o The start last modification date (yyyy-mm-dd).
@@ -61,16 +60,14 @@
           o The username to the eurlex webservices.
           o password: string, optional, default empty string
           o The password to the eurlex webservices.
    4. get_nodes_and_edges_lists
           o df: DataFrame object, required, default None
           o DataFrame of cellar metadata acquired from the get_cellar_extra
             method.
-          o save_file: ['y', 'n'],optional, default 'y'
-          o Save data in a data folder, or return in-memory.
 ## Examples ``` import cellar_extractor as cell Below are examples for in-file
 saving: cell.get_cellar(save_file='y', max_ecli=200, sd='2022-01-01',
 file_format='csv') cell.get_cellar_extra(max_ecli=100, sd='2022-01-01',
 threads=10) Below are examples for in-memory saving: df = cell.get_cellar
 (save_file='n', file_format='csv', sd='2022-01-01', max_ecli=1000) df,json =
 cell.get_cellar_extra(save_file='n', max_ecli=100, sd='2022-01-01', threads=10)
 ``` ## License [![License: Apache 2.0](https://img.shields.io/github/license/
```

### Comparing `cellar_extractor-1.0.47/README.md` & `cellar_extractor-1.0.48/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     <br>
     <li><code>get_cellar_extra</code></li>
     Gets all the ECLI data from the eurlex sparql endpoint, and on top of that scrapes the eurlex websites to acquire 
     the full text, keywords, case law directory code and eurovoc identifiers. If the user does have an eurlex account with access to the eurlex webservices, he can also 
     pass his webservices login credentials to the method, in order to extract data about works citing work and works 
     being cited by work. The full text is returned as a JSON file, rest of data as a CSV.  Can be in-memory or as saved files.
     <li><code>get_nodes_and_edges_lists</code></li>
-    Gets 2 dataframe objects, one for the nodes and edges of the citations within the passed dataframe.
-    Allows the creation of a network graph of the citations. Can be saved in-memory or in the data folder as csv files.
+    Gets 2 list objects, one for the nodes and edges of the citations within the passed dataframe.
+    Allows the creation of a network graph of the citations. Can only be returned in-memory.
     <br>
 </ol>
 
 ## What are the parameters?
 <ol>
     <li><code>get_cellar</code></li>
     <strong>Parameters:</strong>
@@ -97,16 +97,14 @@
         The password to the eurlex webservices.
         <br>
     </ul>
     <li><code>get_nodes_and_edges_lists</code></li>
     <ul>
         <li><strong>df: DataFrame object, required, default None</strong></li>
         DataFrame of cellar metadata acquired from the get_cellar_extra method.
-        <li><strong>save_file: ['y', 'n'],optional, default 'y'</strong></li>
-        Save data in a data folder, or return in-memory.
     </ul>
 </ol>
 
 
 ## Examples
 ```
 import cellar_extractor as cell
```

#### html2text {}

```diff
@@ -12,18 +12,17 @@
       law directory code and eurovoc identifiers. If the user does have an
       eurlex account with access to the eurlex webservices, he can also pass
       his webservices login credentials to the method, in order to extract data
       about works citing work and works being cited by work. The full text is
       returned as a JSON file, rest of data as a CSV. Can be in-memory or as
       saved files.
    5. get_nodes_and_edges_lists
-   6. Gets 2 dataframe objects, one for the nodes and edges of the citations
-      within the passed dataframe. Allows the creation of a network graph of
-      the citations. Can be saved in-memory or in the data folder as csv files.
-
+   6. Gets 2 list objects, one for the nodes and edges of the citations within
+      the passed dataframe. Allows the creation of a network graph of the
+      citations. Can only be returned in-memory.
 ## What are the parameters?
    1. get_cellar
    2. Parameters:
           o max_ecli: int, optional, default 100
           o Maximum number of ECLIs to retrieve.
           o sd: date, optional, default '2022-05-01'
           o The start last modification date (yyyy-mm-dd).
@@ -55,16 +54,14 @@
           o The username to the eurlex webservices.
           o password: string, optional, default empty string
           o The password to the eurlex webservices.
    4. get_nodes_and_edges_lists
           o df: DataFrame object, required, default None
           o DataFrame of cellar metadata acquired from the get_cellar_extra
             method.
-          o save_file: ['y', 'n'],optional, default 'y'
-          o Save data in a data folder, or return in-memory.
 ## Examples ``` import cellar_extractor as cell Below are examples for in-file
 saving: cell.get_cellar(save_file='y', max_ecli=200, sd='2022-01-01',
 file_format='csv') cell.get_cellar_extra(max_ecli=100, sd='2022-01-01',
 threads=10) Below are examples for in-memory saving: df = cell.get_cellar
 (save_file='n', file_format='csv', sd='2022-01-01', max_ecli=1000) df,json =
 cell.get_cellar_extra(save_file='n', max_ecli=100, sd='2022-01-01', threads=10)
 ``` ## License [![License: Apache 2.0](https://img.shields.io/github/license/
```

### Comparing `cellar_extractor-1.0.47/cellar_extractor/Testing_file.py` & `cellar_extractor-1.0.48/cellar_extractor/Testing_file.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.47/cellar_extractor/cellar.py` & `cellar_extractor-1.0.48/cellar_extractor/cellar.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,19 +67,14 @@
 
     else:
         data,json = extra_cellar(data= data, threads = threads, username= username,password=password)
         print("\n--- DONE ---")
 
         return data,json
 
-def get_nodes_and_edges_lists(df = None,save_file='y'):
+def get_nodes_and_edges_lists(df = None):
     if df is None:
         print("No dataframe passed!")
         return
     else:
         nodes,edges = get_nodes_and_edges(df)
-        if save_file == 'y':
-            Path('data').mkdir(parents=True, exist_ok=True)
-            nodes.to_csv(join('data','nodes'),index=False)
-            edges.to_csv(join('data','edges'),index=False)
-        else:
-            return nodes,edges
+        return nodes,edges
```

### Comparing `cellar_extractor-1.0.47/cellar_extractor/cellar_extra_extract.py` & `cellar_extractor-1.0.48/cellar_extractor/cellar_extra_extract.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.47/cellar_extractor/cellar_queries.py` & `cellar_extractor-1.0.48/cellar_extractor/cellar_queries.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.47/cellar_extractor/citations_adder.py` & `cellar_extractor-1.0.48/cellar_extractor/citations_adder.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.47/cellar_extractor/csv_extractor.py` & `cellar_extractor-1.0.48/cellar_extractor/csv_extractor.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.47/cellar_extractor/eurlex_scraping.py` & `cellar_extractor-1.0.48/cellar_extractor/eurlex_scraping.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.47/cellar_extractor/fulltext_saving.py` & `cellar_extractor-1.0.48/cellar_extractor/fulltext_saving.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.47/cellar_extractor/json_to_csv.py` & `cellar_extractor-1.0.48/cellar_extractor/json_to_csv.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.47/cellar_extractor/nodes_and_edges.py` & `cellar_extractor-1.0.48/cellar_extractor/nodes_and_edges.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.47/cellar_extractor/sparql.py` & `cellar_extractor-1.0.48/cellar_extractor/sparql.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.47/cellar_extractor.egg-info/PKG-INFO` & `cellar_extractor-1.0.48/cellar_extractor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellar-extractor
-Version: 1.0.47
+Version: 1.0.48
 Summary: Library for extracting cellar data
 Home-page: UNKNOWN
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
@@ -65,16 +65,16 @@
     <br>
     <li><code>get_cellar_extra</code></li>
     Gets all the ECLI data from the eurlex sparql endpoint, and on top of that scrapes the eurlex websites to acquire 
     the full text, keywords, case law directory code and eurovoc identifiers. If the user does have an eurlex account with access to the eurlex webservices, he can also 
     pass his webservices login credentials to the method, in order to extract data about works citing work and works 
     being cited by work. The full text is returned as a JSON file, rest of data as a CSV.  Can be in-memory or as saved files.
     <li><code>get_nodes_and_edges_lists</code></li>
-    Gets 2 dataframe objects, one for the nodes and edges of the citations within the passed dataframe.
-    Allows the creation of a network graph of the citations. Can be saved in-memory or in the data folder as csv files.
+    Gets 2 list objects, one for the nodes and edges of the citations within the passed dataframe.
+    Allows the creation of a network graph of the citations. Can only be returned in-memory.
     <br>
 </ol>
 
 ## What are the parameters?
 <ol>
     <li><code>get_cellar</code></li>
     <strong>Parameters:</strong>
@@ -111,16 +111,14 @@
         The password to the eurlex webservices.
         <br>
     </ul>
     <li><code>get_nodes_and_edges_lists</code></li>
     <ul>
         <li><strong>df: DataFrame object, required, default None</strong></li>
         DataFrame of cellar metadata acquired from the get_cellar_extra method.
-        <li><strong>save_file: ['y', 'n'],optional, default 'y'</strong></li>
-        Save data in a data folder, or return in-memory.
     </ul>
 </ol>
 
 
 ## Examples
 ```
 import cellar_extractor as cell
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.47 Summary: Library
+Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.48 Summary: Library
 for extracting cellar data Home-page: UNKNOWN Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Platform: UNKNOWN Description-Content-Type: text/
 markdown ## Cellar extractor This library contains two functions to get cellar
 case law data from eurlex. ## Version Python 3.9 ## Contributors
@@ -18,18 +18,17 @@
       law directory code and eurovoc identifiers. If the user does have an
       eurlex account with access to the eurlex webservices, he can also pass
       his webservices login credentials to the method, in order to extract data
       about works citing work and works being cited by work. The full text is
       returned as a JSON file, rest of data as a CSV. Can be in-memory or as
       saved files.
    5. get_nodes_and_edges_lists
-   6. Gets 2 dataframe objects, one for the nodes and edges of the citations
-      within the passed dataframe. Allows the creation of a network graph of
-      the citations. Can be saved in-memory or in the data folder as csv files.
-
+   6. Gets 2 list objects, one for the nodes and edges of the citations within
+      the passed dataframe. Allows the creation of a network graph of the
+      citations. Can only be returned in-memory.
 ## What are the parameters?
    1. get_cellar
    2. Parameters:
           o max_ecli: int, optional, default 100
           o Maximum number of ECLIs to retrieve.
           o sd: date, optional, default '2022-05-01'
           o The start last modification date (yyyy-mm-dd).
@@ -61,16 +60,14 @@
           o The username to the eurlex webservices.
           o password: string, optional, default empty string
           o The password to the eurlex webservices.
    4. get_nodes_and_edges_lists
           o df: DataFrame object, required, default None
           o DataFrame of cellar metadata acquired from the get_cellar_extra
             method.
-          o save_file: ['y', 'n'],optional, default 'y'
-          o Save data in a data folder, or return in-memory.
 ## Examples ``` import cellar_extractor as cell Below are examples for in-file
 saving: cell.get_cellar(save_file='y', max_ecli=200, sd='2022-01-01',
 file_format='csv') cell.get_cellar_extra(max_ecli=100, sd='2022-01-01',
 threads=10) Below are examples for in-memory saving: df = cell.get_cellar
 (save_file='n', file_format='csv', sd='2022-01-01', max_ecli=1000) df,json =
 cell.get_cellar_extra(save_file='n', max_ecli=100, sd='2022-01-01', threads=10)
 ``` ## License [![License: Apache 2.0](https://img.shields.io/github/license/
```

### Comparing `cellar_extractor-1.0.47/cellar_extractor.egg-info/SOURCES.txt` & `cellar_extractor-1.0.48/cellar_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.47/setup.py` & `cellar_extractor-1.0.48/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='cellar_extractor',
     packages=find_packages(include=['cellar_extractor']),
-    version='1.0.47',
+    version='1.0.48',
     description='Library for extracting cellar data',
     author='LawTech Lab',
     license='MIT',
     install_requires=['bs4','SPARQLWrapper==2.0.0', 'requests==2.26.0', 'pandas','lxml==4.6.3','xmltodict==0.13.0','tqdm'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['cellar', 'extractor'],
     long_description=long_descr,
```

