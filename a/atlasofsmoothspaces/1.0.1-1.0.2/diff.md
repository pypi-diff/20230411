# Comparing `tmp/atlasofsmoothspaces-1.0.1.tar.gz` & `tmp/atlasofsmoothspaces-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlasofsmoothspaces-1.0.1.tar", last modified: Sat Apr  1 19:28:36 2023, max compression
+gzip compressed data, was "atlasofsmoothspaces-1.0.2.tar", last modified: Tue Apr 11 07:25:15 2023, max compression
```

## Comparing `atlasofsmoothspaces-1.0.1.tar` & `atlasofsmoothspaces-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-01 19:28:36.953212 atlasofsmoothspaces-1.0.1/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-01 19:28:36.953212 atlasofsmoothspaces-1.0.1/PKG-INFO
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-01 19:28:36.953212 atlasofsmoothspaces-1.0.1/atlasofsmoothspaces/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       23 2023-04-01 19:19:58.000000 atlasofsmoothspaces-1.0.1/atlasofsmoothspaces/__init__.py
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       65 2023-04-01 19:05:28.000000 atlasofsmoothspaces-1.0.1/atlasofsmoothspaces/main.py
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-01 19:28:36.953212 atlasofsmoothspaces-1.0.1/atlasofsmoothspaces.egg-info/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-01 19:28:36.000000 atlasofsmoothspaces-1.0.1/atlasofsmoothspaces.egg-info/PKG-INFO
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      240 2023-04-01 19:28:36.000000 atlasofsmoothspaces-1.0.1/atlasofsmoothspaces.egg-info/SOURCES.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)        1 2023-04-01 19:28:36.000000 atlasofsmoothspaces-1.0.1/atlasofsmoothspaces.egg-info/dependency_links.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       20 2023-04-01 19:28:36.000000 atlasofsmoothspaces-1.0.1/atlasofsmoothspaces.egg-info/top_level.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       38 2023-04-01 19:28:36.953212 atlasofsmoothspaces-1.0.1/setup.cfg
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      888 2023-04-01 19:28:21.000000 atlasofsmoothspaces-1.0.1/setup.py
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:25:15.617735 atlasofsmoothspaces-1.0.2/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 07:25:15.617735 atlasofsmoothspaces-1.0.2/PKG-INFO
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:25:15.617735 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       23 2023-04-01 19:19:58.000000 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces/__init__.py
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)     7684 2023-04-11 07:21:08.000000 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces/main.py
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:25:15.617735 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces.egg-info/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 07:25:15.000000 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces.egg-info/PKG-INFO
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      240 2023-04-11 07:25:15.000000 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces.egg-info/SOURCES.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)        1 2023-04-11 07:25:15.000000 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces.egg-info/dependency_links.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       20 2023-04-11 07:25:15.000000 atlasofsmoothspaces-1.0.2/atlasofsmoothspaces.egg-info/top_level.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       38 2023-04-11 07:25:15.617735 atlasofsmoothspaces-1.0.2/setup.cfg
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      888 2023-04-11 07:25:07.000000 atlasofsmoothspaces-1.0.2/setup.py
```

### Comparing `atlasofsmoothspaces-1.0.1/setup.py` & `atlasofsmoothspaces-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.1' 
+VERSION = '1.0.2' 
 DESCRIPTION = 'Calculating Smoothness from Input Stream'
 LONG_DESCRIPTION = 'Smoothness is calculated from an input stream. The input data format is midi.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="atlasofsmoothspaces",
```

