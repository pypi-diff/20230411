# Comparing `tmp/pyinflux3-0.1.tar.gz` & `tmp/pyinflux3-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-0.1.tar", last modified: Tue Apr 11 13:45:57 2023, max compression
+gzip compressed data, was "pyinflux3-0.2.tar", last modified: Tue Apr 11 14:11:35 2023, max compression
```

## Comparing `pyinflux3-0.1.tar` & `pyinflux3-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 13:45:57.176147 pyinflux3-0.1/
--rw-r--r--   0 jayclifford   (501) staff       (20)      650 2023-04-11 13:45:57.175788 pyinflux3-0.1/PKG-INFO
--rwxr-xr-x   0 jayclifford   (501) staff       (20)     6201 2023-04-11 13:27:48.000000 pyinflux3-0.1/influx3
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 13:45:57.172579 pyinflux3-0.1/influxdb_client_3/
--rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 13:27:48.000000 pyinflux3-0.1/influxdb_client_3/__init__.py
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 13:45:57.175202 pyinflux3-0.1/pyinflux3.egg-info/
--rw-r--r--   0 jayclifford   (501) staff       (20)      650 2023-04-11 13:45:57.000000 pyinflux3-0.1/pyinflux3.egg-info/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)      210 2023-04-11 13:45:57.000000 pyinflux3-0.1/pyinflux3.egg-info/SOURCES.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-11 13:45:57.000000 pyinflux3-0.1/pyinflux3.egg-info/dependency_links.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       40 2023-04-11 13:45:57.000000 pyinflux3-0.1/pyinflux3.egg-info/requires.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-11 13:45:57.000000 pyinflux3-0.1/pyinflux3.egg-info/top_level.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-11 13:45:57.176284 pyinflux3-0.1/setup.cfg
--rw-r--r--   0 jayclifford   (501) staff       (20)      866 2023-04-11 13:40:52.000000 pyinflux3-0.1/setup.py
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 14:11:35.919340 pyinflux3-0.2/
+-rw-r--r--   0 jayclifford   (501) staff       (20)      650 2023-04-11 14:11:35.918948 pyinflux3-0.2/PKG-INFO
+-rwxr-xr-x   0 jayclifford   (501) staff       (20)     6201 2023-04-11 13:27:48.000000 pyinflux3-0.2/influx3
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 14:11:35.915714 pyinflux3-0.2/influxdb_client_3/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 13:27:48.000000 pyinflux3-0.2/influxdb_client_3/__init__.py
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 14:11:35.918354 pyinflux3-0.2/pyinflux3.egg-info/
+-rw-r--r--   0 jayclifford   (501) staff       (20)      650 2023-04-11 14:11:35.000000 pyinflux3-0.2/pyinflux3.egg-info/PKG-INFO
+-rw-r--r--   0 jayclifford   (501) staff       (20)      210 2023-04-11 14:11:35.000000 pyinflux3-0.2/pyinflux3.egg-info/SOURCES.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-11 14:11:35.000000 pyinflux3-0.2/pyinflux3.egg-info/dependency_links.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       64 2023-04-11 14:11:35.000000 pyinflux3-0.2/pyinflux3.egg-info/requires.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-11 14:11:35.000000 pyinflux3-0.2/pyinflux3.egg-info/top_level.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-11 14:11:35.919450 pyinflux3-0.2/setup.cfg
+-rw-r--r--   0 jayclifford   (501) staff       (20)      897 2023-04-11 14:11:10.000000 pyinflux3-0.2/setup.py
```

### Comparing `pyinflux3-0.1/PKG-INFO` & `pyinflux3-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.1
+Version: 0.2
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-0.1/influx3` & `pyinflux3-0.2/influx3`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.1/influxdb_client_3/__init__.py` & `pyinflux3-0.2/influxdb_client_3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.1/pyinflux3.egg-info/PKG-INFO` & `pyinflux3-0.2/pyinflux3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.1
+Version: 0.2
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-0.1/setup.py` & `pyinflux3-0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 setup(
     name='pyinflux3',
-    version='0.1',
+    version='0.2',
     description='Community Python client for InfluxDB IOx',
     author='InfluxData',
     author_email='contact@influxdata.com',
     url='https://github.com/InfluxCommunity/pyinflux3',
     packages=['influxdb_client_3'],
-    install_requires=['pyarrow', 'flightsql-dbapi', 'influxdb-client'],
+    install_requires=['pyarrow', 'flightsql-dbapi', 'influxdb-client', 'pygments', 'prompt_toolkit' ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

