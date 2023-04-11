# Comparing `tmp/ndtiff-1.9.0.tar.gz` & `tmp/ndtiff-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndtiff-1.9.0.tar", last modified: Thu Jan 12 00:50:13 2023, max compression
+gzip compressed data, was "ndtiff-1.9.1.tar", last modified: Mon Feb  6 21:29:19 2023, max compression
```

## Comparing `ndtiff-1.9.0.tar` & `ndtiff-1.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:50:13.085492 ndtiff-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-12 00:50:13.085492 ndtiff-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-12 00:50:00.000000 ndtiff-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:50:13.085492 ndtiff-1.9.0/ndtiff/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-12 00:50:00.000000 ndtiff-1.9.0/ndtiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-01-12 00:50:00.000000 ndtiff-1.9.0/ndtiff/_superclass.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-12 00:50:00.000000 ndtiff-1.9.0/ndtiff/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    45349 2023-01-12 00:50:00.000000 ndtiff-1.9.0/ndtiff/nd_tiff_current.py
--rw-r--r--   0 runner    (1001) docker     (123)    28487 2023-01-12 00:50:00.000000 ndtiff-1.9.0/ndtiff/nd_tiff_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    45349 2023-01-12 00:50:00.000000 ndtiff-1.9.0/ndtiff/ndtiff_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:50:13.085492 ndtiff-1.9.0/ndtiff/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 00:50:00.000000 ndtiff-1.9.0/ndtiff/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-01-12 00:50:00.000000 ndtiff-1.9.0/ndtiff/test/data_loading_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:50:13.085492 ndtiff-1.9.0/ndtiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-12 00:50:12.000000 ndtiff-1.9.0/ndtiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-12 00:50:13.000000 ndtiff-1.9.0/ndtiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 00:50:12.000000 ndtiff-1.9.0/ndtiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-12 00:50:12.000000 ndtiff-1.9.0/ndtiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-12 00:50:12.000000 ndtiff-1.9.0/ndtiff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-12 00:50:00.000000 ndtiff-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 00:50:13.085492 ndtiff-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-01-12 00:50:00.000000 ndtiff-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 21:29:19.118307 ndtiff-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-06 21:29:19.118307 ndtiff-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-06 21:29:08.000000 ndtiff-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 21:29:19.114307 ndtiff-1.9.1/ndtiff/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/_superclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45349 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/nd_tiff_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28496 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/nd_tiff_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45349 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/ndtiff_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 21:29:19.118307 ndtiff-1.9.1/ndtiff/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-02-06 21:29:08.000000 ndtiff-1.9.1/ndtiff/test/data_loading_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 21:29:19.118307 ndtiff-1.9.1/ndtiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-06 21:29:19.000000 ndtiff-1.9.1/ndtiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-02-06 21:29:19.000000 ndtiff-1.9.1/ndtiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 21:29:19.000000 ndtiff-1.9.1/ndtiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-06 21:29:19.000000 ndtiff-1.9.1/ndtiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-06 21:29:19.000000 ndtiff-1.9.1/ndtiff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-06 21:29:08.000000 ndtiff-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 21:29:19.118307 ndtiff-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-06 21:29:08.000000 ndtiff-1.9.1/setup.py
```

### Comparing `ndtiff-1.9.0/PKG-INFO` & `ndtiff-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndtiff
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python libraries for NDTiff datasets
 Home-page: https://github.com/micro-manager/NDTiffStorage
 Author: Henry Pinkard
 Author-email: henry.pinkard@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ndtiff-1.9.0/ndtiff/_superclass.py` & `ndtiff-1.9.1/ndtiff/_superclass.py`

 * *Files identical despite different names*

### Comparing `ndtiff-1.9.0/ndtiff/nd_tiff_current.py` & `ndtiff-1.9.1/ndtiff/nd_tiff_current.py`

 * *Files identical despite different names*

### Comparing `ndtiff-1.9.0/ndtiff/nd_tiff_v2.py` & `ndtiff-1.9.1/ndtiff/nd_tiff_v2.py`

 * *Files identical despite different names*

```diff
@@ -720,15 +720,15 @@
             )
 
             res_level = self.res_levels[resolution_level]
             return res_level.read_metadata(axes)
 
     def close(self):
         with self._lock:
-            for res_level in self.res_levels:
+            for res_level in self.res_levels.values():
                 res_level.close()
 
     def get_channel_names(self):
         with self._lock:
             return self._channel_names.keys()
 
     def _consolidate_axes(self, channel, channel_name, z, position, time, row, col, kwargs):
```

### Comparing `ndtiff-1.9.0/ndtiff/ndtiff_v1.py` & `ndtiff-1.9.1/ndtiff/ndtiff_v1.py`

 * *Files identical despite different names*

### Comparing `ndtiff-1.9.0/ndtiff/test/data_loading_test.py` & `ndtiff-1.9.1/ndtiff/test/data_loading_test.py`

 * *Files identical despite different names*

### Comparing `ndtiff-1.9.0/ndtiff.egg-info/PKG-INFO` & `ndtiff-1.9.1/ndtiff.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndtiff
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python libraries for NDTiff datasets
 Home-page: https://github.com/micro-manager/NDTiffStorage
 Author: Henry Pinkard
 Author-email: henry.pinkard@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ndtiff-1.9.0/setup.py` & `ndtiff-1.9.1/setup.py`

 * *Files identical despite different names*

