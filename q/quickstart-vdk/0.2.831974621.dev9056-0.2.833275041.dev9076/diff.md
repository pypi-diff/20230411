# Comparing `tmp/quickstart-vdk-0.2.831974621.dev9056.tar.gz` & `tmp/quickstart-vdk-0.2.833275041.dev9076.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.831974621.dev9056.tar", last modified: Sun Apr  9 04:28:52 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.833275041.dev9076.tar", last modified: Tue Apr 11 04:26:19 2023, max compression
```

## Comparing `quickstart-vdk-0.2.831974621.dev9056.tar` & `quickstart-vdk-0.2.833275041.dev9076.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 04:28:52.665968 quickstart-vdk-0.2.831974621.dev9056/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-09 04:28:52.665968 quickstart-vdk-0.2.831974621.dev9056/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-09 04:26:16.000000 quickstart-vdk-0.2.831974621.dev9056/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 04:28:52.665968 quickstart-vdk-0.2.831974621.dev9056/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-09 04:28:52.000000 quickstart-vdk-0.2.831974621.dev9056/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-09 04:28:52.000000 quickstart-vdk-0.2.831974621.dev9056/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 04:28:52.000000 quickstart-vdk-0.2.831974621.dev9056/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-09 04:28:52.000000 quickstart-vdk-0.2.831974621.dev9056/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-09 04:28:52.000000 quickstart-vdk-0.2.831974621.dev9056/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 04:28:52.665968 quickstart-vdk-0.2.831974621.dev9056/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-09 04:28:44.000000 quickstart-vdk-0.2.831974621.dev9056/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 04:28:52.665968 quickstart-vdk-0.2.831974621.dev9056/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-09 04:26:16.000000 quickstart-vdk-0.2.831974621.dev9056/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 04:26:19.690808 quickstart-vdk-0.2.833275041.dev9076/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-11 04:26:19.690808 quickstart-vdk-0.2.833275041.dev9076/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-11 04:23:24.000000 quickstart-vdk-0.2.833275041.dev9076/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 04:26:19.690808 quickstart-vdk-0.2.833275041.dev9076/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-11 04:26:19.000000 quickstart-vdk-0.2.833275041.dev9076/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-11 04:26:19.000000 quickstart-vdk-0.2.833275041.dev9076/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 04:26:19.000000 quickstart-vdk-0.2.833275041.dev9076/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-11 04:26:19.000000 quickstart-vdk-0.2.833275041.dev9076/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-11 04:26:19.000000 quickstart-vdk-0.2.833275041.dev9076/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 04:26:19.690808 quickstart-vdk-0.2.833275041.dev9076/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-11 04:26:06.000000 quickstart-vdk-0.2.833275041.dev9076/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 04:26:19.690808 quickstart-vdk-0.2.833275041.dev9076/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-11 04:23:24.000000 quickstart-vdk-0.2.833275041.dev9076/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.831974621.dev9056/PKG-INFO` & `quickstart-vdk-0.2.833275041.dev9076/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.831974621.dev9056
+Version: 0.2.833275041.dev9076
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.831974621.dev9056/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.833275041.dev9076/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.831974621.dev9056
+Version: 0.2.833275041.dev9076
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.831974621.dev9056/setup.py` & `quickstart-vdk-0.2.833275041.dev9076/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.831974621.dev9056"
+__version__ = "0.2.833275041.dev9076"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

