# Comparing `tmp/pyinflux3-0.6.1.tar.gz` & `tmp/pyinflux3-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-0.6.1.tar", last modified: Tue Apr 11 17:23:39 2023, max compression
+gzip compressed data, was "pyinflux3-0.6.2.tar", last modified: Tue Apr 11 17:30:47 2023, max compression
```

## Comparing `pyinflux3-0.6.1.tar` & `pyinflux3-0.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 17:23:39.349460 pyinflux3-0.6.1/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2523 2023-04-11 17:23:39.349047 pyinflux3-0.6.1/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)     1830 2023-04-11 16:44:30.000000 pyinflux3-0.6.1/README.md
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 17:23:39.345506 pyinflux3-0.6.1/influxdb_client_3/
--rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 15:27:56.000000 pyinflux3-0.6.1/influxdb_client_3/__init__.py
--rwxr-xr-x   0 jayclifford   (501) staff       (20)     6201 2023-04-11 16:54:23.000000 pyinflux3-0.6.1/influxdb_client_3/influx3
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 17:23:39.348395 pyinflux3-0.6.1/pyinflux3.egg-info/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2523 2023-04-11 17:23:39.000000 pyinflux3-0.6.1/pyinflux3.egg-info/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)      274 2023-04-11 17:23:39.000000 pyinflux3-0.6.1/pyinflux3.egg-info/SOURCES.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-11 17:23:39.000000 pyinflux3-0.6.1/pyinflux3.egg-info/dependency_links.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       59 2023-04-11 17:23:39.000000 pyinflux3-0.6.1/pyinflux3.egg-info/entry_points.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       64 2023-04-11 17:23:39.000000 pyinflux3-0.6.1/pyinflux3.egg-info/requires.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-11 17:23:39.000000 pyinflux3-0.6.1/pyinflux3.egg-info/top_level.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-11 17:23:39.349568 pyinflux3-0.6.1/setup.cfg
--rw-r--r--   0 jayclifford   (501) staff       (20)     1796 2023-04-11 17:23:29.000000 pyinflux3-0.6.1/setup.py
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 17:30:47.426124 pyinflux3-0.6.2/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     2523 2023-04-11 17:30:47.425773 pyinflux3-0.6.2/PKG-INFO
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1830 2023-04-11 16:44:30.000000 pyinflux3-0.6.2/README.md
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 17:30:47.422598 pyinflux3-0.6.2/influxdb_client_3/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 15:27:56.000000 pyinflux3-0.6.2/influxdb_client_3/__init__.py
+-rwxr-xr-x   0 jayclifford   (501) staff       (20)     6201 2023-04-11 16:54:23.000000 pyinflux3-0.6.2/influxdb_client_3/influx3.py
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 17:30:47.425087 pyinflux3-0.6.2/pyinflux3.egg-info/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     2523 2023-04-11 17:30:47.000000 pyinflux3-0.6.2/pyinflux3.egg-info/PKG-INFO
+-rw-r--r--   0 jayclifford   (501) staff       (20)      277 2023-04-11 17:30:47.000000 pyinflux3-0.6.2/pyinflux3.egg-info/SOURCES.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-11 17:30:47.000000 pyinflux3-0.6.2/pyinflux3.egg-info/dependency_links.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       59 2023-04-11 17:30:47.000000 pyinflux3-0.6.2/pyinflux3.egg-info/entry_points.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       64 2023-04-11 17:30:47.000000 pyinflux3-0.6.2/pyinflux3.egg-info/requires.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-11 17:30:47.000000 pyinflux3-0.6.2/pyinflux3.egg-info/top_level.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-11 17:30:47.426268 pyinflux3-0.6.2/setup.cfg
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1799 2023-04-11 17:30:25.000000 pyinflux3-0.6.2/setup.py
```

### Comparing `pyinflux3-0.6.1/PKG-INFO` & `pyinflux3-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.6.1
+Version: 0.6.2
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-0.6.1/README.md` & `pyinflux3-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.6.1/influxdb_client_3/__init__.py` & `pyinflux3-0.6.2/influxdb_client_3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.6.1/influxdb_client_3/influx3` & `pyinflux3-0.6.2/influxdb_client_3/influx3.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.6.1/pyinflux3.egg-info/PKG-INFO` & `pyinflux3-0.6.2/pyinflux3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.6.1
+Version: 0.6.2
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-0.6.1/setup.py` & `pyinflux3-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def get_version():
     # If running in GitHub Actions, get version from GITHUB_REF
     version = get_version_from_github_ref()
     if version:
         return version
 
     # Fallback to a default version if not in GitHub Actions
-    return "v0.6.1"
+    return "v0.6.2"
 
 setup(
     name='pyinflux3',
     version=get_version(),
     description='Community Python client for InfluxDB IOx',
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -46,11 +46,11 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
-    data_files=[('influx3', ['influxdb_client_3/influx3'])],
+    data_files=[('influx3', ['influxdb_client_3/influx3.py'])],
     entry_points={"console_scripts": [f"{binary_name} = influxdb_client_3.influx3:main"]},
 
 )
```

