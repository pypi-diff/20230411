# Comparing `tmp/cdk-skylight-1.1.93.tar.gz` & `tmp/cdk-skylight-1.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-skylight-1.1.93.tar", last modified: Mon Apr 10 00:13:43 2023, max compression
+gzip compressed data, was "cdk-skylight-1.1.94.tar", last modified: Tue Apr 11 00:14:23 2023, max compression
```

## Comparing `cdk-skylight-1.1.93.tar` & `cdk-skylight-1.1.94.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:13:43.153748 cdk-skylight-1.1.93/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-10 00:13:28.000000 cdk-skylight-1.1.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 00:13:28.000000 cdk-skylight-1.1.93/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-10 00:13:43.153748 cdk-skylight-1.1.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-10 00:13:28.000000 cdk-skylight-1.1.93/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-10 00:13:28.000000 cdk-skylight-1.1.93/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 00:13:43.153748 cdk-skylight-1.1.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-10 00:13:28.000000 cdk-skylight-1.1.93/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:13:43.153748 cdk-skylight-1.1.93/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:13:43.153748 cdk-skylight-1.1.93/src/cdk_skylight/
--rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-04-10 00:13:28.000000 cdk-skylight-1.1.93/src/cdk_skylight/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:13:43.153748 cdk-skylight-1.1.93/src/cdk_skylight/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-10 00:13:28.000000 cdk-skylight-1.1.93/src/cdk_skylight/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86448 2023-04-10 00:13:28.000000 cdk-skylight-1.1.93/src/cdk_skylight/_jsii/cdk-skylight@1.1.93.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:13:43.153748 cdk-skylight-1.1.93/src/cdk_skylight/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)    28299 2023-04-10 00:13:28.000000 cdk-skylight-1.1.93/src/cdk_skylight/authentication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:13:43.153748 cdk-skylight-1.1.93/src/cdk_skylight/compute/
--rw-r--r--   0 runner    (1001) docker     (123)    50139 2023-04-10 00:13:28.000000 cdk-skylight-1.1.93/src/cdk_skylight/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 00:13:28.000000 cdk-skylight-1.1.93/src/cdk_skylight/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:13:43.153748 cdk-skylight-1.1.93/src/cdk_skylight/storage/
--rw-r--r--   0 runner    (1001) docker     (123)    17481 2023-04-10 00:13:28.000000 cdk-skylight-1.1.93/src/cdk_skylight/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:13:43.153748 cdk-skylight-1.1.93/src/cdk_skylight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-10 00:13:43.000000 cdk-skylight-1.1.93/src/cdk_skylight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-10 00:13:43.000000 cdk-skylight-1.1.93/src/cdk_skylight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 00:13:43.000000 cdk-skylight-1.1.93/src/cdk_skylight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-10 00:13:43.000000 cdk-skylight-1.1.93/src/cdk_skylight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 00:13:43.000000 cdk-skylight-1.1.93/src/cdk_skylight.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:14:23.687357 cdk-skylight-1.1.94/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 00:14:08.000000 cdk-skylight-1.1.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 00:14:08.000000 cdk-skylight-1.1.94/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-11 00:14:23.687357 cdk-skylight-1.1.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-11 00:14:08.000000 cdk-skylight-1.1.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-11 00:14:08.000000 cdk-skylight-1.1.94/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 00:14:23.687357 cdk-skylight-1.1.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-11 00:14:08.000000 cdk-skylight-1.1.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:14:23.687357 cdk-skylight-1.1.94/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:14:23.687357 cdk-skylight-1.1.94/src/cdk_skylight/
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-04-11 00:14:08.000000 cdk-skylight-1.1.94/src/cdk_skylight/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:14:23.687357 cdk-skylight-1.1.94/src/cdk_skylight/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-11 00:14:08.000000 cdk-skylight-1.1.94/src/cdk_skylight/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86448 2023-04-11 00:14:08.000000 cdk-skylight-1.1.94/src/cdk_skylight/_jsii/cdk-skylight@1.1.94.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:14:23.687357 cdk-skylight-1.1.94/src/cdk_skylight/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)    28299 2023-04-11 00:14:08.000000 cdk-skylight-1.1.94/src/cdk_skylight/authentication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:14:23.687357 cdk-skylight-1.1.94/src/cdk_skylight/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)    50139 2023-04-11 00:14:08.000000 cdk-skylight-1.1.94/src/cdk_skylight/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 00:14:08.000000 cdk-skylight-1.1.94/src/cdk_skylight/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:14:23.687357 cdk-skylight-1.1.94/src/cdk_skylight/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)    17481 2023-04-11 00:14:08.000000 cdk-skylight-1.1.94/src/cdk_skylight/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:14:23.687357 cdk-skylight-1.1.94/src/cdk_skylight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-11 00:14:23.000000 cdk-skylight-1.1.94/src/cdk_skylight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-11 00:14:23.000000 cdk-skylight-1.1.94/src/cdk_skylight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 00:14:23.000000 cdk-skylight-1.1.94/src/cdk_skylight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-11 00:14:23.000000 cdk-skylight-1.1.94/src/cdk_skylight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 00:14:23.000000 cdk-skylight-1.1.94/src/cdk_skylight.egg-info/top_level.txt
```

### Comparing `cdk-skylight-1.1.93/LICENSE` & `cdk-skylight-1.1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-skylight-1.1.93/PKG-INFO` & `cdk-skylight-1.1.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-skylight
-Version: 1.1.93
+Version: 1.1.94
 Summary: cdk-skylight
 Home-page: https://github.com/cdklabs/cdk-skylight.git
 Author: Dudu (David) Twizer<dudut@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-skylight.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-skylight-1.1.93/README.md` & `cdk-skylight-1.1.94/README.md`

 * *Files identical despite different names*

### Comparing `cdk-skylight-1.1.93/setup.py` & `cdk-skylight-1.1.94/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-skylight",
-    "version": "1.1.93",
+    "version": "1.1.94",
     "description": "cdk-skylight",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-skylight.git",
     "long_description_content_type": "text/markdown",
     "author": "Dudu (David) Twizer<dudut@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -25,15 +25,15 @@
         "cdk_skylight._jsii",
         "cdk_skylight.authentication",
         "cdk_skylight.compute",
         "cdk_skylight.storage"
     ],
     "package_data": {
         "cdk_skylight._jsii": [
-            "cdk-skylight@1.1.93.jsii.tgz"
+            "cdk-skylight@1.1.94.jsii.tgz"
         ],
         "cdk_skylight": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-skylight-1.1.93/src/cdk_skylight/__init__.py` & `cdk-skylight-1.1.94/src/cdk_skylight/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-skylight-1.1.93/src/cdk_skylight/authentication/__init__.py` & `cdk-skylight-1.1.94/src/cdk_skylight/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-skylight-1.1.93/src/cdk_skylight/compute/__init__.py` & `cdk-skylight-1.1.94/src/cdk_skylight/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-skylight-1.1.93/src/cdk_skylight/storage/__init__.py` & `cdk-skylight-1.1.94/src/cdk_skylight/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-skylight-1.1.93/src/cdk_skylight.egg-info/PKG-INFO` & `cdk-skylight-1.1.94/src/cdk_skylight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-skylight
-Version: 1.1.93
+Version: 1.1.94
 Summary: cdk-skylight
 Home-page: https://github.com/cdklabs/cdk-skylight.git
 Author: Dudu (David) Twizer<dudut@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-skylight.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-skylight-1.1.93/src/cdk_skylight.egg-info/SOURCES.txt` & `cdk-skylight-1.1.94/src/cdk_skylight.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 src/cdk_skylight/py.typed
 src/cdk_skylight.egg-info/PKG-INFO
 src/cdk_skylight.egg-info/SOURCES.txt
 src/cdk_skylight.egg-info/dependency_links.txt
 src/cdk_skylight.egg-info/requires.txt
 src/cdk_skylight.egg-info/top_level.txt
 src/cdk_skylight/_jsii/__init__.py
-src/cdk_skylight/_jsii/cdk-skylight@1.1.93.jsii.tgz
+src/cdk_skylight/_jsii/cdk-skylight@1.1.94.jsii.tgz
 src/cdk_skylight/authentication/__init__.py
 src/cdk_skylight/compute/__init__.py
 src/cdk_skylight/storage/__init__.py
```

