# Comparing `tmp/azuredol-0.1.0.tar.gz` & `tmp/azuredol-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azuredol-0.1.0.tar", last modified: Tue Apr 11 17:11:25 2023, max compression
+gzip compressed data, was "azuredol-0.1.1.tar", last modified: Tue Apr 11 18:09:50 2023, max compression
```

## Comparing `azuredol-0.1.0.tar` & `azuredol-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:11:25.169612 azuredol-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 17:10:57.000000 azuredol-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-11 17:11:25.169612 azuredol-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 17:10:57.000000 azuredol-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:11:25.169612 azuredol-0.1.0/azuredol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:10:57.000000 azuredol-0.1.0/azuredol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-11 17:10:57.000000 azuredol-0.1.0/azuredol/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:11:25.169612 azuredol-0.1.0/azuredol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-11 17:11:25.000000 azuredol-0.1.0/azuredol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-11 17:11:25.000000 azuredol-0.1.0/azuredol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:11:25.000000 azuredol-0.1.0/azuredol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:11:25.000000 azuredol-0.1.0/azuredol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 17:11:25.000000 azuredol-0.1.0/azuredol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 17:11:25.000000 azuredol-0.1.0/azuredol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-11 17:11:25.169612 azuredol-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 17:10:57.000000 azuredol-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:09:50.496317 azuredol-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 18:09:24.000000 azuredol-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-11 18:09:50.496317 azuredol-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 18:09:24.000000 azuredol-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:09:50.496317 azuredol-0.1.1/azuredol/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 18:09:24.000000 azuredol-0.1.1/azuredol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-11 18:09:24.000000 azuredol-0.1.1/azuredol/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:09:50.496317 azuredol-0.1.1/azuredol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-11 18:09:50.000000 azuredol-0.1.1/azuredol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-11 18:09:50.000000 azuredol-0.1.1/azuredol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:09:50.000000 azuredol-0.1.1/azuredol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:09:50.000000 azuredol-0.1.1/azuredol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 18:09:50.000000 azuredol-0.1.1/azuredol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 18:09:50.000000 azuredol-0.1.1/azuredol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-11 18:09:50.496317 azuredol-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 18:09:24.000000 azuredol-0.1.1/setup.py
```

### Comparing `azuredol-0.1.0/LICENSE` & `azuredol-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `azuredol-0.1.0/setup.cfg` & `azuredol-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = azuredol
-version = 0.1.0
+version = 0.1.1
 url = https://github.com/i2mint/azuredol
 platforms = any
 description_file = README.md
 root_url = https://github.com/i2mint/
 license = apache-2.0
 author = OtoSense
 description = Azure Storage Data Object Layer
```

