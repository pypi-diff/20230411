# Comparing `tmp/macrometa-source-collection-0.0.18.tar.gz` & `tmp/macrometa-source-collection-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.18.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.19.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.18.tar` & `macrometa-source-collection-0.0.19.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8418 2023-03-15 12:39:11.002224 macrometa-source-collection-0.0.18/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     4581 2023-03-15 12:39:11.002224 macrometa-source-collection-0.0.18/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1592 2023-03-15 12:39:11.246227 macrometa-source-collection-0.0.18/pyproject.toml
--rw-r--r--   0        0        0     1044 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.18/setup.py
--rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.18/PKG-INFO
+-rw-r--r--   0        0        0     8418 2023-04-11 05:53:24.786848 macrometa-source-collection-0.0.19/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     5895 2023-04-11 05:53:24.786848 macrometa-source-collection-0.0.19/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1621 2023-04-11 05:53:25.074850 macrometa-source-collection-0.0.19/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.19/setup.py
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.19/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.18/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.19/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.18/pyproject.toml` & `macrometa-source-collection-0.0.19/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.18'
+version='0.0.19'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -34,14 +34,15 @@
 idna = "2.10"
 numpy = "1.21.6"
 pandas = "1.3.5"
 pyC8 = "0.17.3"
 requests = "2.25.1"
 websocket-client = "0.57.0"
 pulsar-client = "2.10.1"
+prometheus-client = "0.16.0"
 
 [tool.poetry.scripts]
 # CLI declaration
 macrometa-source-collection = 'macrometa_source_collection:main'
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Macrometacorp/macrometa-source-collection/issues"
```

### Comparing `macrometa-source-collection-0.0.18/setup.py` & `macrometa-source-collection-0.0.19/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,27 @@
 install_requires = \
 ['c8connector==0.0.15',
  'chardet==4.0.0',
  'idna==2.10',
  'numpy==1.21.6',
  'pandas==1.3.5',
  'pipelinewise-singer-python==1.2.0',
+ 'prometheus-client==0.16.0',
  'pulsar-client==2.10.1',
  'pyC8==0.17.3',
  'requests==2.25.1',
  'websocket-client==0.57.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.18',
+    'version': '0.0.19',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.18/PKG-INFO` & `macrometa-source-collection-0.0.19/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.18
+Version: 0.0.19
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Tap
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,12 +16,13 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: c8connector (==0.0.15)
 Requires-Dist: chardet (==4.0.0)
 Requires-Dist: idna (==2.10)
 Requires-Dist: numpy (==1.21.6)
 Requires-Dist: pandas (==1.3.5)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
+Requires-Dist: prometheus-client (==0.16.0)
 Requires-Dist: pulsar-client (==2.10.1)
 Requires-Dist: pyC8 (==0.17.3)
 Requires-Dist: requests (==2.25.1)
 Requires-Dist: websocket-client (==0.57.0)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-source-collection/issues
```

