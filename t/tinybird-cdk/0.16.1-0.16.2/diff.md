# Comparing `tmp/tinybird-cdk-0.16.1.tar.gz` & `tmp/tinybird-cdk-0.16.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cdk-0.16.1.tar", last modified: Thu Apr  6 08:16:40 2023, max compression
+gzip compressed data, was "tinybird-cdk-0.16.2.tar", last modified: Tue Apr 11 13:50:33 2023, max compression
```

## Comparing `tinybird-cdk-0.16.1.tar` & `tinybird-cdk-0.16.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:16:40.043451 tinybird-cdk-0.16.1/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-06 08:16:40.043451 tinybird-cdk-0.16.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 08:16:40.043451 tinybird-cdk-0.16.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:16:40.039451 tinybird-cdk-0.16.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tests/test_gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:16:40.039451 tinybird-cdk-0.16.1/tinybird_cdk/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:16:40.043451 tinybird-cdk-0.16.1/tinybird_cdk/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/cloud/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/cloud/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/cloud/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/cloud/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:16:40.043451 tinybird-cdk-0.16.1/tinybird_cdk/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/connectors/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/connectors/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/connectors/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/connectors/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/connectors/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/connectors/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/connectors/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/connectors/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/tinybird.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-06 08:16:29.000000 tinybird-cdk-0.16.1/tinybird_cdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:16:40.043451 tinybird-cdk-0.16.1/tinybird_cdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-06 08:16:40.000000 tinybird-cdk-0.16.1/tinybird_cdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-06 08:16:40.000000 tinybird-cdk-0.16.1/tinybird_cdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:16:40.000000 tinybird-cdk-0.16.1/tinybird_cdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-06 08:16:40.000000 tinybird-cdk-0.16.1/tinybird_cdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-06 08:16:40.000000 tinybird-cdk-0.16.1/tinybird_cdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:50:33.197110 tinybird-cdk-0.16.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-11 13:50:33.197110 tinybird-cdk-0.16.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:50:33.197110 tinybird-cdk-0.16.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:50:33.193109 tinybird-cdk-0.16.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tests/test_gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:50:33.197110 tinybird-cdk-0.16.2/tinybird_cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:50:33.197110 tinybird-cdk-0.16.2/tinybird_cdk/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/cloud/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/cloud/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/cloud/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/cloud/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:50:33.197110 tinybird-cdk-0.16.2/tinybird_cdk/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/connectors/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/connectors/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/connectors/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/connectors/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/connectors/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/connectors/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/connectors/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/connectors/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/tinybird.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-11 13:50:21.000000 tinybird-cdk-0.16.2/tinybird_cdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:50:33.197110 tinybird-cdk-0.16.2/tinybird_cdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-11 13:50:33.000000 tinybird-cdk-0.16.2/tinybird_cdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-11 13:50:33.000000 tinybird-cdk-0.16.2/tinybird_cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:50:33.000000 tinybird-cdk-0.16.2/tinybird_cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 13:50:33.000000 tinybird-cdk-0.16.2/tinybird_cdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 13:50:33.000000 tinybird-cdk-0.16.2/tinybird_cdk.egg-info/top_level.txt
```

### Comparing `tinybird-cdk-0.16.1/README.md` & `tinybird-cdk-0.16.2/README.md`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/setup.py` & `tinybird-cdk-0.16.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tinybird-cdk',
-    version='0.16.1',
+    version='0.16.2',
     description="Tinybird's Connector Development Kit.",
     long_description='This package is under active development and currently meant for internal use only.',
     long_description_content_type='text/markdown',
     author='tinybird.co',
     author_email="support@tinybird.co",
     python_requires='>=3.8, <3.12',
     install_requires=[
```

### Comparing `tinybird-cdk-0.16.1/tests/test_gcp.py` & `tinybird-cdk-0.16.2/tests/test_gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/cloud/__init__.py` & `tinybird-cdk-0.16.2/tinybird_cdk/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/cloud/abstract_client.py` & `tinybird-cdk-0.16.2/tinybird_cdk/cloud/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/cloud/gcp.py` & `tinybird-cdk-0.16.2/tinybird_cdk/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/cloud/gcs.py` & `tinybird-cdk-0.16.2/tinybird_cdk/cloud/gcs.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/cloud/s3.py` & `tinybird-cdk-0.16.2/tinybird_cdk/cloud/s3.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/config.py` & `tinybird-cdk-0.16.2/tinybird_cdk/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/connector.py` & `tinybird-cdk-0.16.2/tinybird_cdk/connector.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/connectors/bigquery.py` & `tinybird-cdk-0.16.2/tinybird_cdk/connectors/bigquery.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/connectors/kinesis.py` & `tinybird-cdk-0.16.2/tinybird_cdk/connectors/kinesis.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/connectors/mysql.py` & `tinybird-cdk-0.16.2/tinybird_cdk/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/connectors/postgresql.py` & `tinybird-cdk-0.16.2/tinybird_cdk/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/connectors/snowflake.py` & `tinybird-cdk-0.16.2/tinybird_cdk/connectors/snowflake.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/connectors/sqlite.py` & `tinybird-cdk-0.16.2/tinybird_cdk/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/errors.py` & `tinybird-cdk-0.16.2/tinybird_cdk/errors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/export.py` & `tinybird-cdk-0.16.2/tinybird_cdk/export.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/formats.py` & `tinybird-cdk-0.16.2/tinybird_cdk/formats.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/logger.py` & `tinybird-cdk-0.16.2/tinybird_cdk/logger.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/schema.py` & `tinybird-cdk-0.16.2/tinybird_cdk/schema.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk/tinybird.py` & `tinybird-cdk-0.16.2/tinybird_cdk/tinybird.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import time
 import urllib.parse
 
 import httpx
 import humanize
+import random
 
 from . import config, errors, formats, logger
 from typing import Optional
 
 
 class Client:
     '''Tinybird client. All connectors have an instance of this class.'''
@@ -14,14 +15,15 @@
     DS_PATH     = '/v0/datasources'
     SQL_PATH    = '/v0/sql'
     EVENTS_PATH = '/v0/events'
 
     JOB_POLL_PERIOD_S     = 1.0
     MAX_RETRIES           = 5
     MAX_RATE_LIMIT_WAIT_S = 60*60
+    MIN_WAIT_S = 60
 
     # By default, HTTPX uses a timeout of 5s. David said in
     #
     #     https://3.basecamp.com/4360466/buckets/25800185/messages/4818119130#__recording_4827620424
     #
     # that this does not suffice for reading, because Tinybird starts responding
     # when the work has been completed and large payloads may need time. By now,
@@ -224,16 +226,20 @@
     # We discussed error handling in
     #
     #     https://3.basecamp.com/4360466/buckets/25800185/messages/4818119130
     #
     # In particular, retries on 500s were discarded except for 502s for GET.
     def _should_retry(self, method, status_code, headers, retries):
         # Rate limiting.
-        if status_code == 429:
-            return int(headers['Retry-After'])
+        if status_code == 429 and retries < self.MAX_RETRIES:
+            # Exponential backoff with some random jitter to avoid deadlocks
+            return max(
+                int(headers['Retry-After']) * 2 ** retries + random.randint(0, 9),
+                self.MIN_WAIT_S
+            )
 
         # Timeout: Retry safety considerations in the discussion linked above.
         if status_code == 408 and retries < self.MAX_RETRIES:
             return 2**(retries + 1)
 
         # Bad Gateway: Communication hiccup between NGINX and Analytics.
         if status_code == 502 and method in ('GET', 'HEAD'):
```

### Comparing `tinybird-cdk-0.16.1/tinybird_cdk.egg-info/SOURCES.txt` & `tinybird-cdk-0.16.2/tinybird_cdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

