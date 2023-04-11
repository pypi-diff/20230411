# Comparing `tmp/atlasofsmoothspaces-1.0.2.tar.gz` & `tmp/atlasofsmoothspaces-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlasofsmoothspaces-1.0.2.tar", last modified: Tue Apr 11 07:25:15 2023, max compression
+gzip compressed data, was "atlasofsmoothspaces-1.0.3.tar", last modified: Tue Apr 11 07:32:23 2023, max compression
```

## Comparing `atlasofsmoothspaces-1.0.2.tar` & `atlasofsmoothspaces-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:25:15.617735 atlasofsmoothspaces-1.0.2/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 07:25:15.617735 atlasofsmoothspaces-1.0.2/PKG-INFO
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:25:15.617735 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       23 2023-04-01 19:19:58.000000 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces/__init__.py
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)     7684 2023-04-11 07:21:08.000000 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces/main.py
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:25:15.617735 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces.egg-info/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 07:25:15.000000 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces.egg-info/PKG-INFO
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      240 2023-04-11 07:25:15.000000 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces.egg-info/SOURCES.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)        1 2023-04-11 07:25:15.000000 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces.egg-info/dependency_links.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       20 2023-04-11 07:25:15.000000 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces.egg-info/top_level.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       38 2023-04-11 07:25:15.617735 atlasofsmoothspaces-1.0.2/setup.cfg
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      888 2023-04-11 07:25:07.000000 atlasofsmoothspaces-1.0.2/setup.py
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:32:23.868679 atlasofsmoothspaces-1.0.3/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 07:32:23.868679 atlasofsmoothspaces-1.0.3/PKG-INFO
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:32:23.868679 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       19 2023-04-11 07:32:02.000000 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces/__init__.py
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)     7684 2023-04-11 07:21:08.000000 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces/main.py
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:32:23.868679 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces.egg-info/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 07:32:23.000000 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces.egg-info/PKG-INFO
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      240 2023-04-11 07:32:23.000000 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces.egg-info/SOURCES.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)        1 2023-04-11 07:32:23.000000 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces.egg-info/dependency_links.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       20 2023-04-11 07:32:23.000000 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces.egg-info/top_level.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       38 2023-04-11 07:32:23.868679 atlasofsmoothspaces-1.0.3/setup.cfg
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      888 2023-04-11 07:32:19.000000 atlasofsmoothspaces-1.0.3/setup.py
```

### Comparing `atlasofsmoothspaces-1.0.2/atlasofsmoothspaces/main.py` & `atlasofsmoothspaces-1.0.3/atlasofsmoothspaces/main.py`

 * *Files identical despite different names*

### Comparing `atlasofsmoothspaces-1.0.2/setup.py` & `atlasofsmoothspaces-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.2' 
+VERSION = '1.0.3' 
 DESCRIPTION = 'Calculating Smoothness from Input Stream'
 LONG_DESCRIPTION = 'Smoothness is calculated from an input stream. The input data format is midi.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="atlasofsmoothspaces",
```

