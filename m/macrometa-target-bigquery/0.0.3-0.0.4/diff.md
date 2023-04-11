# Comparing `tmp/macrometa-target-bigquery-0.0.3.tar.gz` & `tmp/macrometa-target-bigquery-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-bigquery-0.0.3.tar", last modified: Sun Apr  2 13:09:26 2023, max compression
+gzip compressed data, was "macrometa-target-bigquery-0.0.4.tar", last modified: Tue Apr 11 12:01:50 2023, max compression
```

## Comparing `macrometa-target-bigquery-0.0.3.tar` & `macrometa-target-bigquery-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 13:09:26.633680 macrometa-target-bigquery-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-04-02 13:09:12.000000 macrometa-target-bigquery-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-02 13:09:26.633680 macrometa-target-bigquery-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20733 2023-04-02 13:09:12.000000 macrometa-target-bigquery-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 13:09:26.629680 macrometa-target-bigquery-0.0.3/macrometa_target_bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)    30013 2023-04-02 13:09:12.000000 macrometa-target-bigquery-0.0.3/macrometa_target_bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-04-02 13:09:12.000000 macrometa-target-bigquery-0.0.3/macrometa_target_bigquery/db_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-02 13:09:12.000000 macrometa-target-bigquery-0.0.3/macrometa_target_bigquery/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-02 13:09:12.000000 macrometa-target-bigquery-0.0.3/macrometa_target_bigquery/flattening.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-02 13:09:12.000000 macrometa-target-bigquery-0.0.3/macrometa_target_bigquery/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-02 13:09:12.000000 macrometa-target-bigquery-0.0.3/macrometa_target_bigquery/stream_ref_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-02 13:09:12.000000 macrometa-target-bigquery-0.0.3/macrometa_target_bigquery/stream_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 13:09:26.633680 macrometa-target-bigquery-0.0.3/macrometa_target_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-02 13:09:26.000000 macrometa-target-bigquery-0.0.3/macrometa_target_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-02 13:09:26.000000 macrometa-target-bigquery-0.0.3/macrometa_target_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 13:09:26.000000 macrometa-target-bigquery-0.0.3/macrometa_target_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-02 13:09:26.000000 macrometa-target-bigquery-0.0.3/macrometa_target_bigquery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-02 13:09:26.000000 macrometa-target-bigquery-0.0.3/macrometa_target_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-02 13:09:26.000000 macrometa-target-bigquery-0.0.3/macrometa_target_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 13:09:26.633680 macrometa-target-bigquery-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-02 13:09:12.000000 macrometa-target-bigquery-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:01:50.624559 macrometa-target-bigquery-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-04-11 12:01:31.000000 macrometa-target-bigquery-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-11 12:01:50.620559 macrometa-target-bigquery-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20733 2023-04-11 12:01:31.000000 macrometa-target-bigquery-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:01:50.620559 macrometa-target-bigquery-0.0.4/macrometa_target_bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)    29849 2023-04-11 12:01:31.000000 macrometa-target-bigquery-0.0.4/macrometa_target_bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-04-11 12:01:31.000000 macrometa-target-bigquery-0.0.4/macrometa_target_bigquery/db_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-11 12:01:31.000000 macrometa-target-bigquery-0.0.4/macrometa_target_bigquery/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-11 12:01:31.000000 macrometa-target-bigquery-0.0.4/macrometa_target_bigquery/flattening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-11 12:01:31.000000 macrometa-target-bigquery-0.0.4/macrometa_target_bigquery/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-11 12:01:31.000000 macrometa-target-bigquery-0.0.4/macrometa_target_bigquery/stream_ref_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-11 12:01:31.000000 macrometa-target-bigquery-0.0.4/macrometa_target_bigquery/stream_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:01:50.620559 macrometa-target-bigquery-0.0.4/macrometa_target_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-11 12:01:50.000000 macrometa-target-bigquery-0.0.4/macrometa_target_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-11 12:01:50.000000 macrometa-target-bigquery-0.0.4/macrometa_target_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:01:50.000000 macrometa-target-bigquery-0.0.4/macrometa_target_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 12:01:50.000000 macrometa-target-bigquery-0.0.4/macrometa_target_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-11 12:01:50.000000 macrometa-target-bigquery-0.0.4/macrometa_target_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 12:01:50.000000 macrometa-target-bigquery-0.0.4/macrometa_target_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 12:01:50.624559 macrometa-target-bigquery-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-11 12:01:31.000000 macrometa-target-bigquery-0.0.4/setup.py
```

### Comparing `macrometa-target-bigquery-0.0.3/LICENSE` & `macrometa-target-bigquery-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.3/PKG-INFO` & `macrometa-target-bigquery-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-bigquery
-Version: 0.0.3
+Version: 0.0.4
 Summary: Macrometa target bigquery connector for loading data to BigQuery
 Home-page: https://github.com/Macrometacorp/macrometa-target-bigquery
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `macrometa-target-bigquery-0.0.3/README.md` & `macrometa-target-bigquery-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.3/macrometa_target_bigquery/__init__.py` & `macrometa-target-bigquery-0.0.4/macrometa_target_bigquery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,34 +92,31 @@
             ConfigProperty('project_id', 'Project ID', ConfigAttributeType.STRING, True, False,
                            description='BigQuery project ID.',
                            placeholder_value='my_project_id'),
             ConfigProperty('credentials_file', 'Credentials JSON file', ConfigAttributeType.STRING, True, False,
                            description='Fully qualified path to client_secrets.json for your service account. See the '
                                        '"Activate the Google BigQuery API" section of the repository\'s README and '
                                        'https://cloud.google.com/docs/authentication/production.',
-                           placeholder_value='my_credentials'),
+                           placeholder_value='credentials.json contents'),
             ConfigProperty('target_schema', 'Target Schema/Dataset', ConfigAttributeType.STRING, True, False,
-                           description='Name of the schema/dataset where the tables will be created.',
-                           placeholder_value='my_schema'),
+                           description='Name of the schema/dataset where the tables will be created.'),
             ConfigProperty('target_table', 'Target Table', ConfigAttributeType.STRING, True, False,
-                           description='Name of the bigquery table. The table will be created if it does not exist',
-                           placeholder_value='my_table'),
+                           description='Name of the bigquery table. The table will be created if it does not exist'),
             ConfigProperty('location', 'Location', ConfigAttributeType.STRING, False, False,
-                           description='Region where BigQuery stores your dataset.',
-                           placeholder_value='my_location'),
+                           description='Region where BigQuery stores your dataset.'),
             ConfigProperty('default_target_schema_select_permission', 'Target Schema privileges',
                            ConfigAttributeType.STRING, False, False,
                            description='Grant USAGE privilege on newly created schemas and grant SELECT privilege on '
                                        'newly created table.',
                            placeholder_value='SELECT'),
             ConfigProperty('batch_size_rows', 'Batch Size', ConfigAttributeType.INT, False, False,
                            description='Maximum number of rows in each batch. At the end of each batch, '
                                        'the rows in the batch are loaded into BigQuery.',
                            default_value='10000'),
-            ConfigProperty('batch_wait_limit_seconds', 'Batch wait limit (seconds)',
+            ConfigProperty('batch_wait_limit_seconds', 'Batch Wait Limit (Seconds)',
                            ConfigAttributeType.INT, False, False,
                            description='Maximum time to wait for batch to reach batch_size_rows.',
                            placeholder_value='60'),
             ConfigProperty('flush_all_streams', 'Flush All Streams', ConfigAttributeType.BOOLEAN, False, False,
                            description='Flush and load every stream into BigQuery when one batch is full. Warning: '
                                        'This may trigger transfer of data with low number of records, '
                                        'and may cause performance problems.',
```

### Comparing `macrometa-target-bigquery-0.0.3/macrometa_target_bigquery/db_sync.py` & `macrometa-target-bigquery-0.0.4/macrometa_target_bigquery/db_sync.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.3/macrometa_target_bigquery/exceptions.py` & `macrometa-target-bigquery-0.0.4/macrometa_target_bigquery/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.3/macrometa_target_bigquery/flattening.py` & `macrometa-target-bigquery-0.0.4/macrometa_target_bigquery/flattening.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.3/macrometa_target_bigquery/sql_utils.py` & `macrometa-target-bigquery-0.0.4/macrometa_target_bigquery/sql_utils.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.3/macrometa_target_bigquery/stream_ref_helper.py` & `macrometa-target-bigquery-0.0.4/macrometa_target_bigquery/stream_ref_helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.3/macrometa_target_bigquery/stream_utils.py` & `macrometa-target-bigquery-0.0.4/macrometa_target_bigquery/stream_utils.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.3/macrometa_target_bigquery.egg-info/PKG-INFO` & `macrometa-target-bigquery-0.0.4/macrometa_target_bigquery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-bigquery
-Version: 0.0.3
+Version: 0.0.4
 Summary: Macrometa target bigquery connector for loading data to BigQuery
 Home-page: https://github.com/Macrometacorp/macrometa-target-bigquery
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `macrometa-target-bigquery-0.0.3/macrometa_target_bigquery.egg-info/SOURCES.txt` & `macrometa-target-bigquery-0.0.4/macrometa_target_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.3/setup.py` & `macrometa-target-bigquery-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name="macrometa-target-bigquery",
-      version='0.0.3',
+      version='0.0.4',
       description="Macrometa target bigquery connector for loading data to BigQuery",
       long_description=long_description,
       long_description_content_type='text/markdown',
       author="Macrometa",
       url='https://github.com/Macrometacorp/macrometa-target-bigquery',
       classifiers=[
           'License :: OSI Approved :: Apache Software License',
```

