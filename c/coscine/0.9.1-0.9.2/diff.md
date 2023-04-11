# Comparing `tmp/coscine-0.9.1.tar.gz` & `tmp/coscine-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coscine-0.9.1.tar", last modified: Tue Apr 11 13:21:26 2023, max compression
+gzip compressed data, was "dist/coscine-0.9.2.tar", last modified: Tue Apr 11 13:46:22 2023, max compression
```

## Comparing `coscine-0.9.1.tar` & `coscine-0.9.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:21:26.000000 coscine-0.9.1/
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-03-09 03:41:37.000000 coscine-0.9.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     7001 2023-04-11 13:21:26.000000 coscine-0.9.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5471 2023-03-09 03:41:37.000000 coscine-0.9.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 13:21:26.000000 coscine-0.9.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3905 2023-03-09 03:41:37.000000 coscine-0.9.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:21:26.000000 coscine-0.9.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine/
--rw-rw-rw-   0 root         (0) root         (0)     2949 2023-04-11 13:11:24.000000 coscine-0.9.1/src/coscine/__about__.py
--rw-rw-rw-   0 root         (0) root         (0)     2231 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6267 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    24288 2023-04-11 13:11:24.000000 coscine-0.9.1/src/coscine/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine/data/
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/data/project.json
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/data/resource.json
--rw-rw-rw-   0 root         (0) root         (0)     2276 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)    28275 2023-04-11 13:11:24.000000 coscine-0.9.1/src/coscine/form.py
--rw-rw-rw-   0 root         (0) root         (0)     6910 2023-03-09 03:59:25.000000 coscine-0.9.1/src/coscine/graph.py
--rw-rw-rw-   0 root         (0) root         (0)    19225 2023-04-11 13:18:30.000000 coscine-0.9.1/src/coscine/object.py
--rw-rw-rw-   0 root         (0) root         (0)    21761 2023-04-11 13:11:24.000000 coscine-0.9.1/src/coscine/project.py
--rw-rw-rw-   0 root         (0) root         (0)    26349 2023-04-11 13:18:30.000000 coscine-0.9.1/src/coscine/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     7402 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/s3.py
--rw-rw-rw-   0 root         (0) root         (0)    11884 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14870 2023-03-09 03:41:37.000000 coscine-0.9.1/src/coscine/vocabulary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7001 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 13:21:26.000000 coscine-0.9.1/src/coscine.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:46:22.000000 coscine-0.9.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2023-04-11 13:11:08.000000 coscine-0.9.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     7001 2023-04-11 13:46:22.000000 coscine-0.9.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5471 2023-04-11 13:11:08.000000 coscine-0.9.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 13:46:22.000000 coscine-0.9.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2023-04-11 13:11:08.000000 coscine-0.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:46:22.000000 coscine-0.9.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine/
+-rw-rw-rw-   0 root         (0) root         (0)     2949 2023-04-11 13:46:13.000000 coscine-0.9.2/src/coscine/__about__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2231 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6267 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    24288 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/data/project.json
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/data/resource.json
+-rw-rw-rw-   0 root         (0) root         (0)     2276 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)    28275 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/form.py
+-rw-rw-rw-   0 root         (0) root         (0)     6910 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    19225 2023-04-11 13:18:30.000000 coscine-0.9.2/src/coscine/object.py
+-rw-rw-rw-   0 root         (0) root         (0)    21761 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/project.py
+-rw-rw-rw-   0 root         (0) root         (0)    26362 2023-04-11 13:46:13.000000 coscine-0.9.2/src/coscine/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     7402 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)    11884 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14870 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/vocabulary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7001 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine.egg-info/top_level.txt
```

### Comparing `coscine-0.9.1/LICENSE.txt` & `coscine-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/PKG-INFO` & `coscine-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coscine
-Version: 0.9.1
+Version: 0.9.2
 Summary: The Coscine Python SDK provides a pythonic interface to the Coscine REST API.
 Home-page: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/
 Author: RWTH Aachen University
 Author-email: coscine@itc.rwth-aachen.de
 License: MIT License
 Project-URL: Issues, https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/issues
 Project-URL: Documentation, https://coscine.pages.rwth-aachen.de/community-features/coscine-python-sdk/
```

### Comparing `coscine-0.9.1/README.md` & `coscine-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/setup.py` & `coscine-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/src/coscine/__about__.py` & `coscine-0.9.2/src/coscine/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ###############################################################################
 
 # Package title/name as it would appear in PyPi
 __title__ = "coscine"
 
 # Current package version
 # Do not set version to 1.0.0 before Coscine end of pilot phase
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 # Short package description
 __summary__ = (
     "The Coscine Python SDK provides a pythonic interface to "
     "the Coscine REST API."
 )
```

### Comparing `coscine-0.9.1/src/coscine/__init__.py` & `coscine-0.9.2/src/coscine/__init__.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/src/coscine/cache.py` & `coscine-0.9.2/src/coscine/cache.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/src/coscine/client.py` & `coscine-0.9.2/src/coscine/client.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/src/coscine/data/project.json` & `coscine-0.9.2/src/coscine/data/project.json`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/src/coscine/data/resource.json` & `coscine-0.9.2/src/coscine/data/resource.json`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/src/coscine/defaults.py` & `coscine-0.9.2/src/coscine/defaults.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/src/coscine/form.py` & `coscine-0.9.2/src/coscine/form.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/src/coscine/graph.py` & `coscine-0.9.2/src/coscine/graph.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/src/coscine/object.py` & `coscine-0.9.2/src/coscine/object.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/src/coscine/project.py` & `coscine-0.9.2/src/coscine/project.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/src/coscine/resource.py` & `coscine-0.9.2/src/coscine/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -722,15 +722,15 @@
                 for key, values in metadata.items():
                     for value in values:
                         valtype: str = value["type"]
                         valuestr: str = value["value"]
                         if valtype == "uri":
                             rdf_object = rdflib.URIRef(valuestr)
                         else:
-                            rdflib.Literal(valuestr)
+                            rdf_object = rdflib.Literal(valuestr)
                         graph.add((
                             file_reference,
                             rdflib.URIRef(key),
                             rdf_object
                         ))
 
         #######################################################################
```

### Comparing `coscine-0.9.1/src/coscine/s3.py` & `coscine-0.9.2/src/coscine/s3.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/src/coscine/utils.py` & `coscine-0.9.2/src/coscine/utils.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/src/coscine/vocabulary.py` & `coscine-0.9.2/src/coscine/vocabulary.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.1/src/coscine.egg-info/PKG-INFO` & `coscine-0.9.2/src/coscine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coscine
-Version: 0.9.1
+Version: 0.9.2
 Summary: The Coscine Python SDK provides a pythonic interface to the Coscine REST API.
 Home-page: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/
 Author: RWTH Aachen University
 Author-email: coscine@itc.rwth-aachen.de
 License: MIT License
 Project-URL: Issues, https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/issues
 Project-URL: Documentation, https://coscine.pages.rwth-aachen.de/community-features/coscine-python-sdk/
```

### Comparing `coscine-0.9.1/src/coscine.egg-info/SOURCES.txt` & `coscine-0.9.2/src/coscine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

