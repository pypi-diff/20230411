# Comparing `tmp/pyinflux3-0.6.2.tar.gz` & `tmp/pyinflux3-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-0.6.2.tar", last modified: Tue Apr 11 17:30:47 2023, max compression
+gzip compressed data, was "pyinflux3-0.6.3.tar", last modified: Tue Apr 11 17:49:49 2023, max compression
```

## Comparing `pyinflux3-0.6.2.tar` & `pyinflux3-0.6.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 17:30:47.426124 pyinflux3-0.6.2/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2523 2023-04-11 17:30:47.425773 pyinflux3-0.6.2/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)     1830 2023-04-11 16:44:30.000000 pyinflux3-0.6.2/README.md
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 17:30:47.422598 pyinflux3-0.6.2/influxdb_client_3/
--rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 15:27:56.000000 pyinflux3-0.6.2/influxdb_client_3/__init__.py
--rwxr-xr-x   0 jayclifford   (501) staff       (20)     6201 2023-04-11 16:54:23.000000 pyinflux3-0.6.2/influxdb_client_3/influx3.py
-drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 17:30:47.425087 pyinflux3-0.6.2/pyinflux3.egg-info/
--rw-r--r--   0 jayclifford   (501) staff       (20)     2523 2023-04-11 17:30:47.000000 pyinflux3-0.6.2/pyinflux3.egg-info/PKG-INFO
--rw-r--r--   0 jayclifford   (501) staff       (20)      277 2023-04-11 17:30:47.000000 pyinflux3-0.6.2/pyinflux3.egg-info/SOURCES.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-11 17:30:47.000000 pyinflux3-0.6.2/pyinflux3.egg-info/dependency_links.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       59 2023-04-11 17:30:47.000000 pyinflux3-0.6.2/pyinflux3.egg-info/entry_points.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       64 2023-04-11 17:30:47.000000 pyinflux3-0.6.2/pyinflux3.egg-info/requires.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-11 17:30:47.000000 pyinflux3-0.6.2/pyinflux3.egg-info/top_level.txt
--rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-11 17:30:47.426268 pyinflux3-0.6.2/setup.cfg
--rw-r--r--   0 jayclifford   (501) staff       (20)     1799 2023-04-11 17:30:25.000000 pyinflux3-0.6.2/setup.py
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 17:49:49.978182 pyinflux3-0.6.3/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     2515 2023-04-11 17:49:49.977816 pyinflux3-0.6.3/PKG-INFO
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1822 2023-04-11 17:34:27.000000 pyinflux3-0.6.3/README.md
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 17:49:49.973593 pyinflux3-0.6.3/influxdb_client_3/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1854 2023-04-11 15:27:56.000000 pyinflux3-0.6.3/influxdb_client_3/__init__.py
+-rwxr-xr-x   0 jayclifford   (501) staff       (20)     6201 2023-04-11 16:54:23.000000 pyinflux3-0.6.3/influxdb_client_3/influx3.py
+drwxr-xr-x   0 jayclifford   (501) staff       (20)        0 2023-04-11 17:49:49.977069 pyinflux3-0.6.3/pyinflux3.egg-info/
+-rw-r--r--   0 jayclifford   (501) staff       (20)     2515 2023-04-11 17:49:49.000000 pyinflux3-0.6.3/pyinflux3.egg-info/PKG-INFO
+-rw-r--r--   0 jayclifford   (501) staff       (20)      277 2023-04-11 17:49:49.000000 pyinflux3-0.6.3/pyinflux3.egg-info/SOURCES.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)        1 2023-04-11 17:49:49.000000 pyinflux3-0.6.3/pyinflux3.egg-info/dependency_links.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       59 2023-04-11 17:49:49.000000 pyinflux3-0.6.3/pyinflux3.egg-info/entry_points.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       71 2023-04-11 17:49:49.000000 pyinflux3-0.6.3/pyinflux3.egg-info/requires.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       18 2023-04-11 17:49:49.000000 pyinflux3-0.6.3/pyinflux3.egg-info/top_level.txt
+-rw-r--r--   0 jayclifford   (501) staff       (20)       38 2023-04-11 17:49:49.978307 pyinflux3-0.6.3/setup.cfg
+-rw-r--r--   0 jayclifford   (501) staff       (20)     1808 2023-04-11 17:49:24.000000 pyinflux3-0.6.3/setup.py
```

### Comparing `pyinflux3-0.6.2/PKG-INFO` & `pyinflux3-0.6.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.6.2
+Version: 0.6.3
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -38,33 +38,33 @@
     }
 }
 }
 ```
 
 Or you can use the config command to create or modify a config:
 ```
-% ./influx3 config --name="my-config" --namespace="boring-observability" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="bBBvtg5EBsa9iayvmP36UtN327gQti1D-1uReiptl_gEfODHmGFxU2IgFdoAWgJxltl8qanrSU4Q3a8nUIrHsQ==" --org="847e9dbb25976492"
+% influx3 config --name="my-config" --namespace="boring-observability" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="bBBvtg5EBsa9iayvmP36UtN327gQti1D-1uReiptl_gEfODHmGFxU2IgFdoAWgJxltl8qanrSU4Q3a8nUIrHsQ==" --org="847e9dbb25976492"
 ```
 
 If you are running against InfluxDB Cloud, then use the bucket name for the namespace in you configuration.
 
 # Run as a Command
 ```
-% ./influx3 sql "select * from anomalies"
+% influx3 sql "select * from anomalies"
 ```
 
 ```
-% ./influx3 write testmes f=7 
+% influx3 write testmes f=7 
 ```
 
 # Run and Query Interactively
 So far only the query command is supported.
 
 ```
-% ./influx3
+% influx3
 Welcome to my IOx CLI.
 
 (>) sql
 (sql >) select * from anomalies
     check    id  observed                          time     type user_id  value
 0       1  None       NaN 2023-02-03 20:56:57.513279776    error       1  400.0
 1       1  None       NaN 2023-02-03 17:52:54.328785835  latency       1  900.0
```

### Comparing `pyinflux3-0.6.2/README.md` & `pyinflux3-0.6.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,33 +20,33 @@
     }
 }
 }
 ```
 
 Or you can use the config command to create or modify a config:
 ```
-% ./influx3 config --name="my-config" --namespace="boring-observability" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="bBBvtg5EBsa9iayvmP36UtN327gQti1D-1uReiptl_gEfODHmGFxU2IgFdoAWgJxltl8qanrSU4Q3a8nUIrHsQ==" --org="847e9dbb25976492"
+% influx3 config --name="my-config" --namespace="boring-observability" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="bBBvtg5EBsa9iayvmP36UtN327gQti1D-1uReiptl_gEfODHmGFxU2IgFdoAWgJxltl8qanrSU4Q3a8nUIrHsQ==" --org="847e9dbb25976492"
 ```
 
 If you are running against InfluxDB Cloud, then use the bucket name for the namespace in you configuration.
 
 # Run as a Command
 ```
-% ./influx3 sql "select * from anomalies"
+% influx3 sql "select * from anomalies"
 ```
 
 ```
-% ./influx3 write testmes f=7 
+% influx3 write testmes f=7 
 ```
 
 # Run and Query Interactively
 So far only the query command is supported.
 
 ```
-% ./influx3
+% influx3
 Welcome to my IOx CLI.
 
 (>) sql
 (sql >) select * from anomalies
     check    id  observed                          time     type user_id  value
 0       1  None       NaN 2023-02-03 20:56:57.513279776    error       1  400.0
 1       1  None       NaN 2023-02-03 17:52:54.328785835  latency       1  900.0
```

### Comparing `pyinflux3-0.6.2/influxdb_client_3/__init__.py` & `pyinflux3-0.6.3/influxdb_client_3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.6.2/influxdb_client_3/influx3.py` & `pyinflux3-0.6.3/influxdb_client_3/influx3.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.6.2/pyinflux3.egg-info/PKG-INFO` & `pyinflux3-0.6.3/pyinflux3.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.6.2
+Version: 0.6.3
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -38,33 +38,33 @@
     }
 }
 }
 ```
 
 Or you can use the config command to create or modify a config:
 ```
-% ./influx3 config --name="my-config" --namespace="boring-observability" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="bBBvtg5EBsa9iayvmP36UtN327gQti1D-1uReiptl_gEfODHmGFxU2IgFdoAWgJxltl8qanrSU4Q3a8nUIrHsQ==" --org="847e9dbb25976492"
+% influx3 config --name="my-config" --namespace="boring-observability" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="bBBvtg5EBsa9iayvmP36UtN327gQti1D-1uReiptl_gEfODHmGFxU2IgFdoAWgJxltl8qanrSU4Q3a8nUIrHsQ==" --org="847e9dbb25976492"
 ```
 
 If you are running against InfluxDB Cloud, then use the bucket name for the namespace in you configuration.
 
 # Run as a Command
 ```
-% ./influx3 sql "select * from anomalies"
+% influx3 sql "select * from anomalies"
 ```
 
 ```
-% ./influx3 write testmes f=7 
+% influx3 write testmes f=7 
 ```
 
 # Run and Query Interactively
 So far only the query command is supported.
 
 ```
-% ./influx3
+% influx3
 Welcome to my IOx CLI.
 
 (>) sql
 (sql >) select * from anomalies
     check    id  observed                          time     type user_id  value
 0       1  None       NaN 2023-02-03 20:56:57.513279776    error       1  400.0
 1       1  None       NaN 2023-02-03 17:52:54.328785835  latency       1  900.0
```

### Comparing `pyinflux3-0.6.2/setup.py` & `pyinflux3-0.6.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 def get_version():
     # If running in GitHub Actions, get version from GITHUB_REF
     version = get_version_from_github_ref()
     if version:
         return version
 
     # Fallback to a default version if not in GitHub Actions
-    return "v0.6.2"
+    return "v0.6.3"
 
 setup(
     name='pyinflux3',
     version=get_version(),
     description='Community Python client for InfluxDB IOx',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='InfluxData',
     author_email='contact@influxdata.com',
     url='https://github.com/InfluxCommunity/pyinflux3',
     packages=['influxdb_client_3'],
-    install_requires=['pyarrow', 'flightsql-dbapi', 'influxdb-client', 'pygments', 'prompt_toolkit' ],
+    install_requires=['pyarrow', 'flightsql-dbapi', 'influxdb-client', 'pygments', 'prompt_toolkit', 'pandas'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

