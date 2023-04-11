# Comparing `tmp/sneaksmc-0.0.3.tar.gz` & `tmp/sneaksmc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneaksmc-0.0.3.tar", last modified: Tue Apr 11 13:53:02 2023, max compression
+gzip compressed data, was "sneaksmc-0.0.4.tar", last modified: Tue Apr 11 13:55:18 2023, max compression
```

## Comparing `sneaksmc-0.0.3.tar` & `sneaksmc-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 13:53:02.884838 sneaksmc-0.0.3/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 13:53:02.884838 sneaksmc-0.0.3/PKG-INFO
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       36 2023-03-01 09:47:59.000000 sneaksmc-0.0.3/README.rst
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      107 2023-04-11 13:53:02.884838 sneaksmc-0.0.3/setup.cfg
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      407 2023-04-11 13:52:45.000000 sneaksmc-0.0.3/setup.py
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 13:53:02.884838 sneaksmc-0.0.3/sneaksmc/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       75 2023-04-11 09:09:09.000000 sneaksmc-0.0.3/sneaksmc/__init__.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)     3461 2023-04-11 13:50:50.000000 sneaksmc-0.0.3/sneaksmc/client.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)     6390 2023-04-11 13:50:17.000000 sneaksmc-0.0.3/sneaksmc/crypt.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)    25027 2023-04-11 13:52:14.000000 sneaksmc-0.0.3/sneaksmc/server.py
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 13:53:02.884838 sneaksmc-0.0.3/sneaksmc.egg-info/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 13:53:02.000000 sneaksmc-0.0.3/sneaksmc.egg-info/PKG-INFO
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      265 2023-04-11 13:53:02.000000 sneaksmc-0.0.3/sneaksmc.egg-info/SOURCES.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)        1 2023-04-11 13:53:02.000000 sneaksmc-0.0.3/sneaksmc.egg-info/dependency_links.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       13 2023-04-11 13:53:02.000000 sneaksmc-0.0.3/sneaksmc.egg-info/requires.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)        9 2023-04-11 13:53:02.000000 sneaksmc-0.0.3/sneaksmc.egg-info/top_level.txt
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 13:55:18.156509 sneaksmc-0.0.4/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 13:55:18.156509 sneaksmc-0.0.4/PKG-INFO
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       36 2023-03-01 09:47:59.000000 sneaksmc-0.0.4/README.rst
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      107 2023-04-11 13:55:18.156509 sneaksmc-0.0.4/setup.cfg
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      407 2023-04-11 13:55:08.000000 sneaksmc-0.0.4/setup.py
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 13:55:18.156509 sneaksmc-0.0.4/sneaksmc/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       73 2023-04-11 13:54:48.000000 sneaksmc-0.0.4/sneaksmc/__init__.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)     3461 2023-04-11 13:50:50.000000 sneaksmc-0.0.4/sneaksmc/client.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)     6390 2023-04-11 13:50:17.000000 sneaksmc-0.0.4/sneaksmc/crypt.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)    25027 2023-04-11 13:52:14.000000 sneaksmc-0.0.4/sneaksmc/server.py
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 13:55:18.156509 sneaksmc-0.0.4/sneaksmc.egg-info/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 13:55:17.000000 sneaksmc-0.0.4/sneaksmc.egg-info/PKG-INFO
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      265 2023-04-11 13:55:18.000000 sneaksmc-0.0.4/sneaksmc.egg-info/SOURCES.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)        1 2023-04-11 13:55:17.000000 sneaksmc-0.0.4/sneaksmc.egg-info/dependency_links.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       13 2023-04-11 13:55:18.000000 sneaksmc-0.0.4/sneaksmc.egg-info/requires.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)        9 2023-04-11 13:55:18.000000 sneaksmc-0.0.4/sneaksmc.egg-info/top_level.txt
```

### Comparing `sneaksmc-0.0.3/sneaksmc/client.py` & `sneaksmc-0.0.4/sneaksmc/client.py`

 * *Files identical despite different names*

### Comparing `sneaksmc-0.0.3/sneaksmc/crypt.py` & `sneaksmc-0.0.4/sneaksmc/crypt.py`

 * *Files identical despite different names*

### Comparing `sneaksmc-0.0.3/sneaksmc/server.py` & `sneaksmc-0.0.4/sneaksmc/server.py`

 * *Files identical despite different names*

