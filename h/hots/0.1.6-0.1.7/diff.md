# Comparing `tmp/hots-0.1.6.tar.gz` & `tmp/hots-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hots-0.1.6.tar", last modified: Tue Apr 11 10:28:45 2023, max compression
+gzip compressed data, was "hots-0.1.7.tar", last modified: Tue Apr 11 14:15:42 2023, max compression
```

## Comparing `hots-0.1.6.tar` & `hots-0.1.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:45.111452 hots-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-11 10:28:28.000000 hots-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-11 10:28:45.111452 hots-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-11 10:28:28.000000 hots-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 10:28:28.000000 hots-0.1.6/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-11 10:28:28.000000 hots-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:28:45.111452 hots-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 10:28:28.000000 hots-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:45.107452 hots-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:45.107452 hots-0.1.6/src/hots/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/allocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19578 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    56171 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    32531 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    33462 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/placement.py
--rw-r--r--   0 runner    (1001) docker     (123)    23666 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:45.107452 hots-0.1.6/src/hots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-11 10:28:45.000000 hots-0.1.6/src/hots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-11 10:28:45.000000 hots-0.1.6/src/hots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:28:45.000000 hots-0.1.6/src/hots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-11 10:28:45.000000 hots-0.1.6/src/hots.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:28:44.000000 hots-0.1.6/src/hots.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-11 10:28:45.000000 hots-0.1.6/src/hots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 10:28:45.000000 hots-0.1.6/src/hots.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:45.107452 hots-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-11 10:28:28.000000 hots-0.1.6/tests/test_packaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:15:42.960068 hots-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-11 14:15:27.000000 hots-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-11 14:15:42.960068 hots-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-11 14:15:27.000000 hots-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 14:15:27.000000 hots-0.1.7/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-11 14:15:27.000000 hots-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 14:15:42.960068 hots-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 14:15:27.000000 hots-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:15:42.956068 hots-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:15:42.960068 hots-0.1.7/src/hots/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-11 14:15:27.000000 hots-0.1.7/src/hots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-04-11 14:15:27.000000 hots-0.1.7/src/hots/allocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19578 2023-04-11 14:15:27.000000 hots-0.1.7/src/hots/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-11 14:15:27.000000 hots-0.1.7/src/hots/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-11 14:15:27.000000 hots-0.1.7/src/hots/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-11 14:15:27.000000 hots-0.1.7/src/hots/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56171 2023-04-11 14:15:27.000000 hots-0.1.7/src/hots/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32531 2023-04-11 14:15:27.000000 hots-0.1.7/src/hots/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-04-11 14:15:27.000000 hots-0.1.7/src/hots/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33462 2023-04-11 14:15:27.000000 hots-0.1.7/src/hots/placement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23666 2023-04-11 14:15:27.000000 hots-0.1.7/src/hots/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-11 14:15:27.000000 hots-0.1.7/src/hots/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:15:42.960068 hots-0.1.7/src/hots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-11 14:15:42.000000 hots-0.1.7/src/hots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-11 14:15:42.000000 hots-0.1.7/src/hots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:15:42.000000 hots-0.1.7/src/hots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-11 14:15:42.000000 hots-0.1.7/src/hots.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:15:42.000000 hots-0.1.7/src/hots.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-11 14:15:42.000000 hots-0.1.7/src/hots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 14:15:42.000000 hots-0.1.7/src/hots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:15:42.960068 hots-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-11 14:15:27.000000 hots-0.1.7/tests/test_packaging.py
```

### Comparing `hots-0.1.6/LICENSE.txt` & `hots-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hots-0.1.6/PKG-INFO` & `hots-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hots
-Version: 0.1.6
+Version: 0.1.7
 Summary: Resource Allocation via Clustering
 Author-email: Smile R&D team <rnd@smile.fr>
 License: MIT
 Project-URL: Homepage, https://github.com/Smile-SA/hots
 Project-URL: Documentation, https://hots.readthedocs.io/en/latest/
 Keywords: Resource,Optimisation,Clustering,Planning
 Platform: any
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 <h1 align="center">
-<img src="doc/source/_static/hots_logo.png" width="250">
+<img src="https://github.com/Smile-SA/hots/raw/main/doc/source/_static/hots_logo.png" width="250">
 </h1><br>
 
 > Hybrid Optimization for Time Series (HOTS)  
 > HOTS solves problems presented as time series using machine learning and optimization methods.  
 > The library supports multiple resource related problems (placement, allocation), presented as one or more metrics.
 
 ## Requirements for running HOTS
```

### Comparing `hots-0.1.6/README.md` & `hots-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <h1 align="center">
-<img src="doc/source/_static/hots_logo.png" width="250">
+<img src="https://github.com/Smile-SA/hots/raw/main/doc/source/_static/hots_logo.png" width="250">
 </h1><br>
 
 > Hybrid Optimization for Time Series (HOTS)  
 > HOTS solves problems presented as time series using machine learning and optimization methods.  
 > The library supports multiple resource related problems (placement, allocation), presented as one or more metrics.
 
 ## Requirements for running HOTS
```

### Comparing `hots-0.1.6/pyproject.toml` & `hots-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hots-0.1.6/src/hots/__init__.py` & `hots-0.1.7/src/hots/__init__.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.6/src/hots/allocation.py` & `hots-0.1.7/src/hots/allocation.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.6/src/hots/clustering.py` & `hots-0.1.7/src/hots/clustering.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.6/src/hots/container.py` & `hots-0.1.7/src/hots/container.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.6/src/hots/init.py` & `hots-0.1.7/src/hots/init.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.6/src/hots/instance.py` & `hots-0.1.7/src/hots/instance.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.6/src/hots/main.py` & `hots-0.1.7/src/hots/main.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.6/src/hots/model.py` & `hots-0.1.7/src/hots/model.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.6/src/hots/node.py` & `hots-0.1.7/src/hots/node.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.6/src/hots/placement.py` & `hots-0.1.7/src/hots/placement.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.6/src/hots/plot.py` & `hots-0.1.7/src/hots/plot.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.6/src/hots/tools.py` & `hots-0.1.7/src/hots/tools.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.6/src/hots.egg-info/PKG-INFO` & `hots-0.1.7/src/hots.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hots
-Version: 0.1.6
+Version: 0.1.7
 Summary: Resource Allocation via Clustering
 Author-email: Smile R&D team <rnd@smile.fr>
 License: MIT
 Project-URL: Homepage, https://github.com/Smile-SA/hots
 Project-URL: Documentation, https://hots.readthedocs.io/en/latest/
 Keywords: Resource,Optimisation,Clustering,Planning
 Platform: any
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 <h1 align="center">
-<img src="doc/source/_static/hots_logo.png" width="250">
+<img src="https://github.com/Smile-SA/hots/raw/main/doc/source/_static/hots_logo.png" width="250">
 </h1><br>
 
 > Hybrid Optimization for Time Series (HOTS)  
 > HOTS solves problems presented as time series using machine learning and optimization methods.  
 > The library supports multiple resource related problems (placement, allocation), presented as one or more metrics.
 
 ## Requirements for running HOTS
```

### Comparing `hots-0.1.6/src/hots.egg-info/SOURCES.txt` & `hots-0.1.7/src/hots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hots-0.1.6/tests/test_packaging.py` & `hots-0.1.7/tests/test_packaging.py`

 * *Files identical despite different names*

