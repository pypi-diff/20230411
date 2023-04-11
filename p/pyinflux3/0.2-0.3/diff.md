# Comparing `tmp/pyinflux3-0.2.tar.gz` & `tmp/pyinflux3-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-0.2.tar", last modified: Tue Apr 11 14:11:35 2023, max compression
+gzip compressed data, was "pyinflux3-0.3.tar", last modified: Tue Apr 11 15:17:47 2023, max compression
```

## Comparing `pyinflux3-0.2.tar` & `pyinflux3-0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 14:11:35.919340 pyinflux3-0.2/
--rw-r--r--   0 jayclifford   (501) staff       (20)      650 2023-04-11 14:11:35.918948 pyinflux3-0.2/PKG-INFO
--rwxr-xr-x   0 jayclifford   (501) staff       (20)     6201 2023-04-11 13:27:48.000000 pyinflux3-0.2/influx3
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 14:11:35.915714 pyinflux3-0.2/influxdb_client_3/
--rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 13:27:48.000000 pyinflux3-0.2/influxdb_client_3/__init__.py
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 14:11:35.918354 pyinflux3-0.2/pyinflux3.egg-info/
--rw-r--r--   0 jayclifford   (501) staff       (20)      650 2023-04-11 14:11:35.000000 pyinflux3-0.2/pyinflux3.egg-info/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)      210 2023-04-11 14:11:35.000000 pyinflux3-0.2/pyinflux3.egg-info/SOURCES.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-11 14:11:35.000000 pyinflux3-0.2/pyinflux3.egg-info/dependency_links.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       64 2023-04-11 14:11:35.000000 pyinflux3-0.2/pyinflux3.egg-info/requires.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-11 14:11:35.000000 pyinflux3-0.2/pyinflux3.egg-info/top_level.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-11 14:11:35.919450 pyinflux3-0.2/setup.cfg
--rw-r--r--   0 jayclifford   (501) staff       (20)      897 2023-04-11 14:11:10.000000 pyinflux3-0.2/setup.py
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 15:17:47.495337 pyinflux3-0.3/
+-rw-r--r--   0 jayclifford   (501) staff       (20)      650 2023-04-11 15:17:47.494988 pyinflux3-0.3/PKG-INFO
+-rwxr-xr-x   0 jayclifford   (501) staff       (20)     6201 2023-04-11 13:27:48.000000 pyinflux3-0.3/influx3
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 15:17:47.490739 pyinflux3-0.3/influxdb_client_3/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 13:27:48.000000 pyinflux3-0.3/influxdb_client_3/__init__.py
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 15:17:47.494482 pyinflux3-0.3/pyinflux3.egg-info/
+-rw-r--r--   0 jayclifford   (501) staff       (20)      650 2023-04-11 15:17:47.000000 pyinflux3-0.3/pyinflux3.egg-info/PKG-INFO
+-rw-r--r--   0 jayclifford   (501) staff       (20)      246 2023-04-11 15:17:47.000000 pyinflux3-0.3/pyinflux3.egg-info/SOURCES.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-11 15:17:47.000000 pyinflux3-0.3/pyinflux3.egg-info/dependency_links.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       59 2023-04-11 15:17:47.000000 pyinflux3-0.3/pyinflux3.egg-info/entry_points.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       64 2023-04-11 15:17:47.000000 pyinflux3-0.3/pyinflux3.egg-info/requires.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-11 15:17:47.000000 pyinflux3-0.3/pyinflux3.egg-info/top_level.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-11 15:17:47.495439 pyinflux3-0.3/setup.cfg
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1085 2023-04-11 15:17:06.000000 pyinflux3-0.3/setup.py
```

### Comparing `pyinflux3-0.2/PKG-INFO` & `pyinflux3-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.2
+Version: 0.3
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-0.2/influx3` & `pyinflux3-0.3/influx3`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.2/influxdb_client_3/__init__.py` & `pyinflux3-0.3/influxdb_client_3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.2/pyinflux3.egg-info/PKG-INFO` & `pyinflux3-0.3/pyinflux3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.2
+Version: 0.3
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

