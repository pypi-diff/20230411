# Comparing `tmp/Data_Save-1.0.0.tar.gz` & `tmp/Data_Save-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Data_Save-1.0.0.tar", last modified: Sun Jan  8 21:27:17 2023, max compression
+gzip compressed data, was "Data_Save-1.1.0.tar", last modified: Tue Apr 11 15:01:08 2023, max compression
```

## Comparing `Data_Save-1.0.0.tar` & `Data_Save-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-01-08 21:27:17.878269 Data_Save-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-01-08 21:27:17.872026 Data_Save-1.0.0/Data_Save/
--rw-rw-rw-   0        0        0       19 2023-01-08 20:46:21.000000 Data_Save-1.0.0/Data_Save/__init__.py
--rw-rw-rw-   0        0        0     1239 2023-01-08 20:48:42.000000 Data_Save-1.0.0/Data_Save/data.py
-drwxrwxrwx   0        0        0        0 2023-01-08 21:27:17.877266 Data_Save-1.0.0/Data_Save.egg-info/
--rw-rw-rw-   0        0        0      302 2023-01-08 21:27:17.000000 Data_Save-1.0.0/Data_Save.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-01-08 21:27:17.000000 Data_Save-1.0.0/Data_Save.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-08 21:27:17.000000 Data_Save-1.0.0/Data_Save.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-01-08 21:27:17.000000 Data_Save-1.0.0/Data_Save.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       19 2023-01-08 21:27:17.000000 Data_Save-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      302 2023-01-08 21:27:17.878269 Data_Save-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-01-08 21:27:17.879264 Data_Save-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      368 2023-01-08 21:27:17.000000 Data_Save-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:01:08.328239 Data_Save-1.1.0/
+drwxrwxrwx   0        0        0        0 2023-04-11 15:01:08.322245 Data_Save-1.1.0/Data_Save/
+-rw-rw-rw-   0        0        0     1043 2023-04-11 14:16:36.000000 Data_Save-1.1.0/Data_Save/README.md
+-rw-rw-rw-   0        0        0       19 2023-01-08 20:46:21.000000 Data_Save-1.1.0/Data_Save/__init__.py
+-rw-rw-rw-   0        0        0     4439 2023-04-11 14:06:53.000000 Data_Save-1.1.0/Data_Save/data.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:01:08.327239 Data_Save-1.1.0/Data_Save.egg-info/
+-rw-rw-rw-   0        0        0     1476 2023-04-11 15:01:08.000000 Data_Save-1.1.0/Data_Save.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-04-11 15:01:08.000000 Data_Save-1.1.0/Data_Save.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 15:01:08.000000 Data_Save-1.1.0/Data_Save.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-11 15:01:08.000000 Data_Save-1.1.0/Data_Save.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       19 2023-04-11 14:56:47.000000 Data_Save-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1476 2023-04-11 15:01:08.329238 Data_Save-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-11 15:01:08.330239 Data_Save-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      625 2023-04-11 14:56:47.000000 Data_Save-1.1.0/setup.py
```

