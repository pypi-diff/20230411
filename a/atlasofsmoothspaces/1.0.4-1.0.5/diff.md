# Comparing `tmp/atlasofsmoothspaces-1.0.4.tar.gz` & `tmp/atlasofsmoothspaces-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlasofsmoothspaces-1.0.4.tar", last modified: Tue Apr 11 07:56:26 2023, max compression
+gzip compressed data, was "atlasofsmoothspaces-1.0.5.tar", last modified: Tue Apr 11 08:01:38 2023, max compression
```

## Comparing `atlasofsmoothspaces-1.0.4.tar` & `atlasofsmoothspaces-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:56:26.546502 atlasofsmoothspaces-1.0.4/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 07:56:26.546502 atlasofsmoothspaces-1.0.4/PKG-INFO
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:56:26.546502 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       19 2023-04-11 07:32:02.000000 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces/__init__.py
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)     7773 2023-04-11 07:55:48.000000 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces/main.py
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:56:26.546502 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces.egg-info/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 07:56:26.000000 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces.egg-info/PKG-INFO
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      240 2023-04-11 07:56:26.000000 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces.egg-info/SOURCES.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)        1 2023-04-11 07:56:26.000000 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces.egg-info/dependency_links.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       20 2023-04-11 07:56:26.000000 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces.egg-info/top_level.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       38 2023-04-11 07:56:26.546502 atlasofsmoothspaces-1.0.4/setup.cfg
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      888 2023-04-11 07:56:23.000000 atlasofsmoothspaces-1.0.4/setup.py
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 08:01:38.046491 atlasofsmoothspaces-1.0.5/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 08:01:38.046491 atlasofsmoothspaces-1.0.5/PKG-INFO
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 08:01:38.046491 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       19 2023-04-11 07:32:02.000000 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces/__init__.py
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)     7773 2023-04-11 08:01:20.000000 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces/main.py
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 08:01:38.046491 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces.egg-info/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 08:01:38.000000 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces.egg-info/PKG-INFO
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      240 2023-04-11 08:01:38.000000 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces.egg-info/SOURCES.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)        1 2023-04-11 08:01:38.000000 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces.egg-info/dependency_links.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       20 2023-04-11 08:01:38.000000 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces.egg-info/top_level.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       38 2023-04-11 08:01:38.046491 atlasofsmoothspaces-1.0.5/setup.cfg
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      888 2023-04-11 08:01:33.000000 atlasofsmoothspaces-1.0.5/setup.py
```

### Comparing `atlasofsmoothspaces-1.0.4/atlasofsmoothspaces/main.py` & `atlasofsmoothspaces-1.0.5/atlasofsmoothspaces/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
         self.lastUpdateTime = newTime
 
 
 
 class Smoothness():
 
-    MIDI_MAX : int = 137
+    MIDI_MAX : int = 127
 
     CHANNELS = {
         "CC16_1": "gyro x left",
         "CC16_2": "gyro x right",
         "CC17_1": "gyro y left",
         "CC17_2": "gyro y right",
         "CC18_1": "gyro z left",
```

### Comparing `atlasofsmoothspaces-1.0.4/setup.py` & `atlasofsmoothspaces-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.4' 
+VERSION = '1.0.5' 
 DESCRIPTION = 'Calculating Smoothness from Input Stream'
 LONG_DESCRIPTION = 'Smoothness is calculated from an input stream. The input data format is midi.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="atlasofsmoothspaces",
```

