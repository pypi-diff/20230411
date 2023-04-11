# Comparing `tmp/cellar_extractor-1.0.45.tar.gz` & `tmp/cellar_extractor-1.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellar_extractor-1.0.45.tar", last modified: Mon Apr 10 10:38:55 2023, max compression
+gzip compressed data, was "cellar_extractor-1.0.46.tar", last modified: Tue Apr 11 13:37:50 2023, max compression
```

## Comparing `cellar_extractor-1.0.45.tar` & `cellar_extractor-1.0.46.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 10:38:55.842426 cellar_extractor-1.0.45/
--rw-rw-rw-   0        0        0     7020 2023-04-10 10:38:55.840426 cellar_extractor-1.0.45/PKG-INFO
--rw-rw-rw-   0        0        0     6530 2023-04-10 10:34:04.000000 cellar_extractor-1.0.45/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 10:38:55.830425 cellar_extractor-1.0.45/cellar_extractor/
--rw-rw-rw-   0        0        0      704 2023-04-10 10:34:04.000000 cellar_extractor-1.0.45/cellar_extractor/Testing_file.py
--rw-rw-rw-   0        0        0      100 2022-11-04 13:15:55.000000 cellar_extractor-1.0.45/cellar_extractor/__init__.py
--rw-rw-rw-   0        0        0     3423 2023-04-10 10:34:04.000000 cellar_extractor-1.0.45/cellar_extractor/cellar.py
--rw-rw-rw-   0        0        0     1005 2022-12-16 13:13:01.000000 cellar_extractor-1.0.45/cellar_extractor/cellar_extra_extract.py
--rw-rw-rw-   0        0        0     5227 2023-02-26 11:01:55.000000 cellar_extractor-1.0.45/cellar_extractor/cellar_queries.py
--rw-rw-rw-   0        0        0    11264 2023-01-09 12:41:12.000000 cellar_extractor-1.0.45/cellar_extractor/citations_adder.py
--rw-rw-rw-   0        0        0     1334 2022-11-18 14:10:12.000000 cellar_extractor-1.0.45/cellar_extractor/csv_extractor.py
--rw-rw-rw-   0        0        0    16726 2023-03-24 12:49:14.000000 cellar_extractor-1.0.45/cellar_extractor/eurlex_scraping.py
--rw-rw-rw-   0        0        0     6403 2023-03-24 12:49:14.000000 cellar_extractor-1.0.45/cellar_extractor/fulltext_saving.py
--rw-rw-rw-   0        0        0     5411 2022-12-06 21:17:47.000000 cellar_extractor-1.0.45/cellar_extractor/json_to_csv.py
--rw-rw-rw-   0        0        0     1524 2023-04-10 10:34:04.000000 cellar_extractor-1.0.45/cellar_extractor/nodes_and_edges.py
--rw-rw-rw-   0        0        0     6834 2022-11-15 12:42:07.000000 cellar_extractor-1.0.45/cellar_extractor/sparql.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:38:55.839425 cellar_extractor-1.0.45/cellar_extractor.egg-info/
--rw-rw-rw-   0        0        0     7020 2023-04-10 10:38:55.000000 cellar_extractor-1.0.45/cellar_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-04-10 10:38:55.000000 cellar_extractor-1.0.45/cellar_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 10:38:55.000000 cellar_extractor-1.0.45/cellar_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-04-10 10:38:55.000000 cellar_extractor-1.0.45/cellar_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-10 10:38:55.000000 cellar_extractor-1.0.45/cellar_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 10:38:55.842426 cellar_extractor-1.0.45/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-04-10 10:34:04.000000 cellar_extractor-1.0.45/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:37:50.836905 cellar_extractor-1.0.46/
+-rw-rw-rw-   0        0        0     7020 2023-04-11 13:37:50.834903 cellar_extractor-1.0.46/PKG-INFO
+-rw-rw-rw-   0        0        0     6530 2023-04-10 10:34:04.000000 cellar_extractor-1.0.46/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 13:37:50.824903 cellar_extractor-1.0.46/cellar_extractor/
+-rw-rw-rw-   0        0        0      704 2023-04-10 10:34:04.000000 cellar_extractor-1.0.46/cellar_extractor/Testing_file.py
+-rw-rw-rw-   0        0        0      163 2023-04-11 13:37:46.000000 cellar_extractor-1.0.46/cellar_extractor/__init__.py
+-rw-rw-rw-   0        0        0     3423 2023-04-10 10:34:04.000000 cellar_extractor-1.0.46/cellar_extractor/cellar.py
+-rw-rw-rw-   0        0        0     1005 2022-12-16 13:13:01.000000 cellar_extractor-1.0.46/cellar_extractor/cellar_extra_extract.py
+-rw-rw-rw-   0        0        0     5227 2023-02-26 11:01:55.000000 cellar_extractor-1.0.46/cellar_extractor/cellar_queries.py
+-rw-rw-rw-   0        0        0    11264 2023-01-09 12:41:12.000000 cellar_extractor-1.0.46/cellar_extractor/citations_adder.py
+-rw-rw-rw-   0        0        0     1334 2022-11-18 14:10:12.000000 cellar_extractor-1.0.46/cellar_extractor/csv_extractor.py
+-rw-rw-rw-   0        0        0    16726 2023-03-24 12:49:14.000000 cellar_extractor-1.0.46/cellar_extractor/eurlex_scraping.py
+-rw-rw-rw-   0        0        0     6403 2023-03-24 12:49:14.000000 cellar_extractor-1.0.46/cellar_extractor/fulltext_saving.py
+-rw-rw-rw-   0        0        0     5411 2022-12-06 21:17:47.000000 cellar_extractor-1.0.46/cellar_extractor/json_to_csv.py
+-rw-rw-rw-   0        0        0     1524 2023-04-10 10:34:04.000000 cellar_extractor-1.0.46/cellar_extractor/nodes_and_edges.py
+-rw-rw-rw-   0        0        0     6834 2022-11-15 12:42:07.000000 cellar_extractor-1.0.46/cellar_extractor/sparql.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:37:50.833903 cellar_extractor-1.0.46/cellar_extractor.egg-info/
+-rw-rw-rw-   0        0        0     7020 2023-04-11 13:37:50.000000 cellar_extractor-1.0.46/cellar_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-04-11 13:37:50.000000 cellar_extractor-1.0.46/cellar_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 13:37:50.000000 cellar_extractor-1.0.46/cellar_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-04-11 13:37:50.000000 cellar_extractor-1.0.46/cellar_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-11 13:37:50.000000 cellar_extractor-1.0.46/cellar_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 13:37:50.836905 cellar_extractor-1.0.46/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-04-11 13:37:46.000000 cellar_extractor-1.0.46/setup.py
```

### Comparing `cellar_extractor-1.0.45/PKG-INFO` & `cellar_extractor-1.0.46/cellar_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cellar_extractor
-Version: 1.0.45
+Name: cellar-extractor
+Version: 1.0.46
 Summary: Library for extracting cellar data
 Home-page: UNKNOWN
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.45 Summary: Library
+Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.46 Summary: Library
 for extracting cellar data Home-page: UNKNOWN Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Platform: UNKNOWN Description-Content-Type: text/
 markdown ## Cellar extractor This library contains two functions to get cellar
 case law data from eurlex. ## Version Python 3.9 ## Contributors
```

### Comparing `cellar_extractor-1.0.45/README.md` & `cellar_extractor-1.0.46/README.md`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.45/cellar_extractor/Testing_file.py` & `cellar_extractor-1.0.46/cellar_extractor/Testing_file.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.45/cellar_extractor/cellar.py` & `cellar_extractor-1.0.46/cellar_extractor/cellar.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.45/cellar_extractor/cellar_extra_extract.py` & `cellar_extractor-1.0.46/cellar_extractor/cellar_extra_extract.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.45/cellar_extractor/cellar_queries.py` & `cellar_extractor-1.0.46/cellar_extractor/cellar_queries.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.45/cellar_extractor/citations_adder.py` & `cellar_extractor-1.0.46/cellar_extractor/citations_adder.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.45/cellar_extractor/csv_extractor.py` & `cellar_extractor-1.0.46/cellar_extractor/csv_extractor.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.45/cellar_extractor/eurlex_scraping.py` & `cellar_extractor-1.0.46/cellar_extractor/eurlex_scraping.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.45/cellar_extractor/fulltext_saving.py` & `cellar_extractor-1.0.46/cellar_extractor/fulltext_saving.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.45/cellar_extractor/json_to_csv.py` & `cellar_extractor-1.0.46/cellar_extractor/json_to_csv.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.45/cellar_extractor/nodes_and_edges.py` & `cellar_extractor-1.0.46/cellar_extractor/nodes_and_edges.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.45/cellar_extractor/sparql.py` & `cellar_extractor-1.0.46/cellar_extractor/sparql.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.45/cellar_extractor.egg-info/PKG-INFO` & `cellar_extractor-1.0.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cellar-extractor
-Version: 1.0.45
+Name: cellar_extractor
+Version: 1.0.46
 Summary: Library for extracting cellar data
 Home-page: UNKNOWN
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.45 Summary: Library
+Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.46 Summary: Library
 for extracting cellar data Home-page: UNKNOWN Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Platform: UNKNOWN Description-Content-Type: text/
 markdown ## Cellar extractor This library contains two functions to get cellar
 case law data from eurlex. ## Version Python 3.9 ## Contributors
```

### Comparing `cellar_extractor-1.0.45/cellar_extractor.egg-info/SOURCES.txt` & `cellar_extractor-1.0.46/cellar_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.45/setup.py` & `cellar_extractor-1.0.46/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='cellar_extractor',
     packages=find_packages(include=['cellar_extractor']),
-    version='1.0.45',
+    version='1.0.46',
     description='Library for extracting cellar data',
     author='LawTech Lab',
     license='MIT',
     install_requires=['bs4','SPARQLWrapper==2.0.0', 'requests==2.26.0', 'pandas','lxml==4.6.3','xmltodict==0.13.0','tqdm'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['cellar', 'extractor'],
     long_description=long_descr,
```

