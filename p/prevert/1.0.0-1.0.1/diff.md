# Comparing `tmp/prevert-1.0.0.tar.gz` & `tmp/prevert-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prevert-1.0.0.tar", last modified: Tue Apr 11 13:51:11 2023, max compression
+gzip compressed data, was "prevert-1.0.1.tar", last modified: Tue Apr 11 14:29:07 2023, max compression
```

## Comparing `prevert-1.0.0.tar` & `prevert-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-11 13:51:11.181186 prevert-1.0.0/
--rw-rw-r--   0 peter     (1000) peter     (1000)    11558 2023-04-11 13:32:00.000000 prevert-1.0.0/LICENSE
--rw-rw-r--   0 peter     (1000) peter     (1000)       31 2023-04-11 13:47:00.000000 prevert-1.0.0/MANIFEST.in
--rw-rw-r--   0 peter     (1000) peter     (1000)    14533 2023-04-11 13:51:11.181186 prevert-1.0.0/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     1085 2023-04-11 13:20:47.000000 prevert-1.0.0/README.md
--rw-rw-r--   0 peter     (1000) peter     (1000)      764 2023-04-11 13:51:02.000000 prevert-1.0.0/pyproject.toml
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-04-11 13:51:11.181186 prevert-1.0.0/setup.cfg
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-11 13:51:11.177186 prevert-1.0.0/src/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-11 13:51:11.177186 prevert-1.0.0/src/prevert/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1810 2023-04-11 13:36:12.000000 prevert-1.0.0/src/prevert/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-11 13:51:11.181186 prevert-1.0.0/src/prevert.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)    14533 2023-04-11 13:51:11.000000 prevert-1.0.0/src/prevert.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      242 2023-04-11 13:51:11.000000 prevert-1.0.0/src/prevert.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-04-11 13:51:11.000000 prevert-1.0.0/src/prevert.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       44 2023-04-11 13:51:11.000000 prevert-1.0.0/src/prevert.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        8 2023-04-11 13:51:11.000000 prevert-1.0.0/src/prevert.egg-info/top_level.txt
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-11 14:29:07.324228 prevert-1.0.1/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    11558 2023-04-11 13:32:00.000000 prevert-1.0.1/LICENSE
+-rw-rw-r--   0 peter     (1000) peter     (1000)       31 2023-04-11 13:47:00.000000 prevert-1.0.1/MANIFEST.in
+-rw-rw-r--   0 peter     (1000) peter     (1000)    14555 2023-04-11 14:29:07.324228 prevert-1.0.1/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1107 2023-04-11 14:28:49.000000 prevert-1.0.1/README.md
+-rw-rw-r--   0 peter     (1000) peter     (1000)      756 2023-04-11 14:27:36.000000 prevert-1.0.1/pyproject.toml
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-04-11 14:29:07.324228 prevert-1.0.1/setup.cfg
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-11 14:29:07.324228 prevert-1.0.1/src/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-11 14:29:07.324228 prevert-1.0.1/src/prevert/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1910 2023-04-11 14:26:32.000000 prevert-1.0.1/src/prevert/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-11 14:29:07.324228 prevert-1.0.1/src/prevert.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    14555 2023-04-11 14:29:07.000000 prevert-1.0.1/src/prevert.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      242 2023-04-11 14:29:07.000000 prevert-1.0.1/src/prevert.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-04-11 14:29:07.000000 prevert-1.0.1/src/prevert.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-04-11 14:29:07.000000 prevert-1.0.1/src/prevert.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        8 2023-04-11 14:29:07.000000 prevert-1.0.1/src/prevert.egg-info/top_level.txt
```

### Comparing `prevert-1.0.0/LICENSE` & `prevert-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prevert-1.0.0/PKG-INFO` & `prevert-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prevert
-Version: 1.0.0
+Version: 1.0.1
 Summary: Iterator for prevert files
 Author-email: Peter Rupnik <peter.rupnik@ijs.si>, Nikola Ljubešić <nikola.ljubesic@ijs.si>, Taja Kuzman <taja.kuzman@ijs.si>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -216,32 +216,32 @@
 
 # Prevert iterator
 
 To use the prevert parser, copy the file `prevert.py` in your directory.
 
 ## Use
 
-```
+```python
 # import libraries
 from prevert import dataset
 import pandas as pd
 ```
 
 If you are using the MaCoCu corpora in the XML format, the method dataset() needs only the path of the file as the argument:
 
-```
+```python
 # Open the dataset with the prevert parser 
-dset=dataset("/data/monolingual/mk.xml")
+dset = dataset("/data/monolingual/mk.xml")
 ```
 
 
-dset consists of docs where you can access the metadata by `doc.meta['attribute_name']`. Docs consist of paragraphs where you can access the metadata by `par.meta['attribute_name']`.
+`dset` consists of docs where you can access the metadata by `doc.meta['attribute_name']`. Docs consist of paragraphs where you can access the metadata by `par.meta['attribute_name']`.
 
 Basic use:
-```
+```python
 for doc in dset: # iterating through documents of a dataset
     print(doc.meta) # all attributes
     print(eval(doc.meta['lang_distr'])[0][0]) # most prominent language in the document
     print(str(doc)) # whole document text
     for par in doc: # iterating through paragraphs of a document
         print(par.meta['id']) # specific attribute
         print(str(par)) # whole paragraph text
```

### Comparing `prevert-1.0.0/README.md` & `prevert-1.0.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # Prevert iterator
 
 To use the prevert parser, copy the file `prevert.py` in your directory.
 
 ## Use
 
-```
+```python
 # import libraries
 from prevert import dataset
 import pandas as pd
 ```
 
 If you are using the MaCoCu corpora in the XML format, the method dataset() needs only the path of the file as the argument:
 
-```
+```python
 # Open the dataset with the prevert parser 
-dset=dataset("/data/monolingual/mk.xml")
+dset = dataset("/data/monolingual/mk.xml")
 ```
 
 
-dset consists of docs where you can access the metadata by `doc.meta['attribute_name']`. Docs consist of paragraphs where you can access the metadata by `par.meta['attribute_name']`.
+`dset` consists of docs where you can access the metadata by `doc.meta['attribute_name']`. Docs consist of paragraphs where you can access the metadata by `par.meta['attribute_name']`.
 
 Basic use:
-```
+```python
 for doc in dset: # iterating through documents of a dataset
     print(doc.meta) # all attributes
     print(eval(doc.meta['lang_distr'])[0][0]) # most prominent language in the document
     print(str(doc)) # whole document text
     for par in doc: # iterating through paragraphs of a document
         print(par.meta['id']) # specific attribute
         print(str(par)) # whole paragraph text
```

### Comparing `prevert-1.0.0/pyproject.toml` & `prevert-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prevert"
-version = "1.0.0"
+version = "1.0.1"
 description = "Iterator for prevert files"
 readme = "README.md"
-authors = [{ name = "Peter Rupnik", email = "peter.rupnik@ijs.si" },
+authors = [
+{ name = "Peter Rupnik", email = "peter.rupnik@ijs.si" },
 { name = "Nikola Ljubešić", email = "nikola.ljubesic@ijs.si" },
-{ name = "Taja Kuzman", email = "taja.kuzman@ijs.si" }]
+{ name = "Taja Kuzman", email = "taja.kuzman@ijs.si" },
+]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["prevertical", "prevert", "macocu"]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
-dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
+dev = ["black", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/macocu/prevert/"
```

### Comparing `prevert-1.0.0/src/prevert.egg-info/PKG-INFO` & `prevert-1.0.1/src/prevert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prevert
-Version: 1.0.0
+Version: 1.0.1
 Summary: Iterator for prevert files
 Author-email: Peter Rupnik <peter.rupnik@ijs.si>, Nikola Ljubešić <nikola.ljubesic@ijs.si>, Taja Kuzman <taja.kuzman@ijs.si>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -216,32 +216,32 @@
 
 # Prevert iterator
 
 To use the prevert parser, copy the file `prevert.py` in your directory.
 
 ## Use
 
-```
+```python
 # import libraries
 from prevert import dataset
 import pandas as pd
 ```
 
 If you are using the MaCoCu corpora in the XML format, the method dataset() needs only the path of the file as the argument:
 
-```
+```python
 # Open the dataset with the prevert parser 
-dset=dataset("/data/monolingual/mk.xml")
+dset = dataset("/data/monolingual/mk.xml")
 ```
 
 
-dset consists of docs where you can access the metadata by `doc.meta['attribute_name']`. Docs consist of paragraphs where you can access the metadata by `par.meta['attribute_name']`.
+`dset` consists of docs where you can access the metadata by `doc.meta['attribute_name']`. Docs consist of paragraphs where you can access the metadata by `par.meta['attribute_name']`.
 
 Basic use:
-```
+```python
 for doc in dset: # iterating through documents of a dataset
     print(doc.meta) # all attributes
     print(eval(doc.meta['lang_distr'])[0][0]) # most prominent language in the document
     print(str(doc)) # whole document text
     for par in doc: # iterating through paragraphs of a document
         print(par.meta['id']) # specific attribute
         print(str(par)) # whole paragraph text
```

