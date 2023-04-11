# Comparing `tmp/pyinflux3-0.6.3.tar.gz` & `tmp/pyinflux3-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-0.6.3.tar", last modified: Tue Apr 11 17:49:49 2023, max compression
+gzip compressed data, was "pyinflux3-0.7.0.tar", last modified: Tue Apr 11 17:56:19 2023, max compression
```

## Comparing `pyinflux3-0.6.3.tar` & `pyinflux3-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 17:49:49.978182 pyinflux3-0.6.3/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2515 2023-04-11 17:49:49.977816 pyinflux3-0.6.3/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)     1822 2023-04-11 17:34:27.000000 pyinflux3-0.6.3/README.md
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 17:49:49.973593 pyinflux3-0.6.3/influxdb_client_3/
--rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 15:27:56.000000 pyinflux3-0.6.3/influxdb_client_3/__init__.py
--rwxr-xr-x   0 jayclifford   (501) staff       (20)     6201 2023-04-11 16:54:23.000000 pyinflux3-0.6.3/influxdb_client_3/influx3.py
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 17:49:49.977069 pyinflux3-0.6.3/pyinflux3.egg-info/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2515 2023-04-11 17:49:49.000000 pyinflux3-0.6.3/pyinflux3.egg-info/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)      277 2023-04-11 17:49:49.000000 pyinflux3-0.6.3/pyinflux3.egg-info/SOURCES.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-11 17:49:49.000000 pyinflux3-0.6.3/pyinflux3.egg-info/dependency_links.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       59 2023-04-11 17:49:49.000000 pyinflux3-0.6.3/pyinflux3.egg-info/entry_points.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       71 2023-04-11 17:49:49.000000 pyinflux3-0.6.3/pyinflux3.egg-info/requires.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-11 17:49:49.000000 pyinflux3-0.6.3/pyinflux3.egg-info/top_level.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-11 17:49:49.978307 pyinflux3-0.6.3/setup.cfg
--rw-r--r--   0 jayclifford   (501) staff       (20)     1808 2023-04-11 17:49:24.000000 pyinflux3-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:56:19.834894 pyinflux3-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-11 17:56:19.834894 pyinflux3-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-11 17:56:08.000000 pyinflux3-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:56:19.830894 pyinflux3-0.7.0/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-11 17:56:08.000000 pyinflux3-0.7.0/influxdb_client_3/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6201 2023-04-11 17:56:08.000000 pyinflux3-0.7.0/influxdb_client_3/influx3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:56:19.834894 pyinflux3-0.7.0/pyinflux3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-11 17:56:19.000000 pyinflux3-0.7.0/pyinflux3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-11 17:56:19.000000 pyinflux3-0.7.0/pyinflux3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:56:19.000000 pyinflux3-0.7.0/pyinflux3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-11 17:56:19.000000 pyinflux3-0.7.0/pyinflux3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-11 17:56:19.000000 pyinflux3-0.7.0/pyinflux3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 17:56:19.000000 pyinflux3-0.7.0/pyinflux3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:56:19.834894 pyinflux3-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-11 17:56:08.000000 pyinflux3-0.7.0/setup.py
```

### Comparing `pyinflux3-0.6.3/PKG-INFO` & `pyinflux3-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.6.3
+Version: 0.7.0
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-0.6.3/README.md` & `pyinflux3-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.6.3/influxdb_client_3/__init__.py` & `pyinflux3-0.7.0/influxdb_client_3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.6.3/influxdb_client_3/influx3.py` & `pyinflux3-0.7.0/influxdb_client_3/influx3.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.6.3/pyinflux3.egg-info/PKG-INFO` & `pyinflux3-0.7.0/pyinflux3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.6.3
+Version: 0.7.0
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyinflux3-0.6.3/setup.py` & `pyinflux3-0.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     description='Community Python client for InfluxDB IOx',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='InfluxData',
     author_email='contact@influxdata.com',
     url='https://github.com/InfluxCommunity/pyinflux3',
     packages=['influxdb_client_3'],
-    install_requires=['pyarrow', 'flightsql-dbapi', 'influxdb-client', 'pygments', 'prompt_toolkit', 'pandas'],
+    install_requires=['pyarrow', 'flightsql-dbapi', 'influxdb-client', 'pygments', 'prompt_toolkit', 'pandas', "tabulate"],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

