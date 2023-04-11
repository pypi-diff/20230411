# Comparing `tmp/dapl-secure-bucket-0.0.2.tar.gz` & `tmp/dapl-secure-bucket-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapl-secure-bucket-0.0.2.tar", last modified: Thu Mar 30 09:16:55 2023, max compression
+gzip compressed data, was "dapl-secure-bucket-0.0.3.tar", last modified: Tue Apr 11 10:08:29 2023, max compression
```

## Comparing `dapl-secure-bucket-0.0.2.tar` & `dapl-secure-bucket-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:16:55.369641 dapl-secure-bucket-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-30 09:16:33.000000 dapl-secure-bucket-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-30 09:16:33.000000 dapl-secure-bucket-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-03-30 09:16:55.369641 dapl-secure-bucket-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-30 09:16:33.000000 dapl-secure-bucket-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-30 09:16:33.000000 dapl-secure-bucket-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 09:16:55.369641 dapl-secure-bucket-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-30 09:16:33.000000 dapl-secure-bucket-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:16:55.369641 dapl-secure-bucket-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:16:55.369641 dapl-secure-bucket-0.0.2/src/dapl_secure_bucket/
--rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-03-30 09:16:33.000000 dapl-secure-bucket-0.0.2/src/dapl_secure_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:16:55.369641 dapl-secure-bucket-0.0.2/src/dapl_secure_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-30 09:16:33.000000 dapl-secure-bucket-0.0.2/src/dapl_secure_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24016 2023-03-30 09:16:33.000000 dapl-secure-bucket-0.0.2/src/dapl_secure_bucket/_jsii/dapl_secure_bucket@0.0.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 09:16:33.000000 dapl-secure-bucket-0.0.2/src/dapl_secure_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:16:55.369641 dapl-secure-bucket-0.0.2/src/dapl_secure_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-03-30 09:16:55.000000 dapl-secure-bucket-0.0.2/src/dapl_secure_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-30 09:16:55.000000 dapl-secure-bucket-0.0.2/src/dapl_secure_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 09:16:55.000000 dapl-secure-bucket-0.0.2/src/dapl_secure_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-30 09:16:55.000000 dapl-secure-bucket-0.0.2/src/dapl_secure_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-30 09:16:55.000000 dapl-secure-bucket-0.0.2/src/dapl_secure_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:08:29.729430 dapl-secure-bucket-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 10:08:15.000000 dapl-secure-bucket-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 10:08:15.000000 dapl-secure-bucket-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-11 10:08:29.729430 dapl-secure-bucket-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-11 10:08:15.000000 dapl-secure-bucket-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-11 10:08:15.000000 dapl-secure-bucket-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:08:29.729430 dapl-secure-bucket-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-11 10:08:15.000000 dapl-secure-bucket-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:08:29.729430 dapl-secure-bucket-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:08:29.729430 dapl-secure-bucket-0.0.3/src/dapl_secure_bucket/
+-rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-04-11 10:08:15.000000 dapl-secure-bucket-0.0.3/src/dapl_secure_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:08:29.729430 dapl-secure-bucket-0.0.3/src/dapl_secure_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-11 10:08:15.000000 dapl-secure-bucket-0.0.3/src/dapl_secure_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24011 2023-04-11 10:08:15.000000 dapl-secure-bucket-0.0.3/src/dapl_secure_bucket/_jsii/dapl_secure_bucket@0.0.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:08:15.000000 dapl-secure-bucket-0.0.3/src/dapl_secure_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:08:29.729430 dapl-secure-bucket-0.0.3/src/dapl_secure_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-11 10:08:29.000000 dapl-secure-bucket-0.0.3/src/dapl_secure_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-11 10:08:29.000000 dapl-secure-bucket-0.0.3/src/dapl_secure_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:08:29.000000 dapl-secure-bucket-0.0.3/src/dapl_secure_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-11 10:08:29.000000 dapl-secure-bucket-0.0.3/src/dapl_secure_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 10:08:29.000000 dapl-secure-bucket-0.0.3/src/dapl_secure_bucket.egg-info/top_level.txt
```

### Comparing `dapl-secure-bucket-0.0.2/LICENSE` & `dapl-secure-bucket-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dapl-secure-bucket-0.0.2/PKG-INFO` & `dapl-secure-bucket-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapl-secure-bucket
-Version: 0.0.2
+Version: 0.0.3
 Summary: Secure S3 Bucket construct used in Enterprise DAPL
 Home-page: https://github.com/yvo.van.zee/dapl_secure_bucket.git
 Author: Yvo van Zee<yvo.vanzee@xebia.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yvo.van.zee/dapl_secure_bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `dapl-secure-bucket-0.0.2/README.md` & `dapl-secure-bucket-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dapl-secure-bucket-0.0.2/setup.py` & `dapl-secure-bucket-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "dapl-secure-bucket",
-    "version": "0.0.2",
+    "version": "0.0.3",
     "description": "Secure S3 Bucket construct used in Enterprise DAPL",
     "license": "Apache-2.0",
     "url": "https://github.com/yvo.van.zee/dapl_secure_bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "Yvo van Zee<yvo.vanzee@xebia.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "dapl_secure_bucket",
         "dapl_secure_bucket._jsii"
     ],
     "package_data": {
         "dapl_secure_bucket._jsii": [
-            "dapl_secure_bucket@0.0.2.jsii.tgz"
+            "dapl_secure_bucket@0.0.3.jsii.tgz"
         ],
         "dapl_secure_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.71.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.79.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `dapl-secure-bucket-0.0.2/src/dapl_secure_bucket/__init__.py` & `dapl-secure-bucket-0.0.3/src/dapl_secure_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `dapl-secure-bucket-0.0.2/src/dapl_secure_bucket.egg-info/PKG-INFO` & `dapl-secure-bucket-0.0.3/src/dapl_secure_bucket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapl-secure-bucket
-Version: 0.0.2
+Version: 0.0.3
 Summary: Secure S3 Bucket construct used in Enterprise DAPL
 Home-page: https://github.com/yvo.van.zee/dapl_secure_bucket.git
 Author: Yvo van Zee<yvo.vanzee@xebia.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yvo.van.zee/dapl_secure_bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

