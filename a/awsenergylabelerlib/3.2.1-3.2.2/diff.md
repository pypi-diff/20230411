# Comparing `tmp/awsenergylabelerlib-3.2.1.tar.gz` & `tmp/awsenergylabelerlib-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsenergylabelerlib-3.2.1.tar", last modified: Fri Mar 10 11:47:08 2023, max compression
+gzip compressed data, was "awsenergylabelerlib-3.2.2.tar", last modified: Tue Apr 11 14:35:51 2023, max compression
```

## Comparing `awsenergylabelerlib-3.2.1.tar` & `awsenergylabelerlib-3.2.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:47:08.755487 awsenergylabelerlib-3.2.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3418 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-03-10 11:47:08.755487 awsenergylabelerlib-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    72232 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     2383 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/USAGE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:47:08.751487 awsenergylabelerlib-3.2.1/awsenergylabelerlib/
--rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3418 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    72232 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     2383 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/USAGE.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7719 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/awsenergylabelerlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/awsenergylabelerlibexceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7304 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7446 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/datamodels.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/dev-requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    40764 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/entities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2393 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/schemas.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8929 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:47:08.755487 awsenergylabelerlib-3.2.1/awsenergylabelerlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/awsenergylabelerlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:47:08.755487 awsenergylabelerlib-3.2.1/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6814 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9048 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/docs/contributing.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/docs/history.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/docs/installation.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/docs/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-10 11:47:08.000000 awsenergylabelerlib-3.2.1/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-03-10 11:47:08.755487 awsenergylabelerlib-3.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2084 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 11:47:08.755487 awsenergylabelerlib-3.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/tests/test_awsenergylabelerlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-03-10 11:45:41.000000 awsenergylabelerlib-3.2.1/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:51.019179 awsenergylabelerlib-3.2.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3529 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-04-11 14:35:51.019179 awsenergylabelerlib-3.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    71531 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2383 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/USAGE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:51.015179 awsenergylabelerlib-3.2.2/awsenergylabelerlib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3529 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    71531 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2383 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/USAGE.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7719 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/awsenergylabelerlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/awsenergylabelerlibexceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7304 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7446 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/datamodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/dev-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40854 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2419 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/schemas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8929 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:51.015179 awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:51.019179 awsenergylabelerlib-3.2.2/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6814 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9048 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/contributing.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/history.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-11 14:35:50.000000 awsenergylabelerlib-3.2.2/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-11 14:35:51.019179 awsenergylabelerlib-3.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2084 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:35:51.019179 awsenergylabelerlib-3.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/tests/test_awsenergylabelerlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-11 14:34:23.000000 awsenergylabelerlib-3.2.2/tests/test_validations.py
```

### Comparing `awsenergylabelerlib-3.2.1/CONTRIBUTING.rst` & `awsenergylabelerlib-3.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/HISTORY.rst` & `awsenergylabelerlib-3.2.2/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -188,7 +188,13 @@
 * Bump dependencies.
 
 
 3.2.1 (10-03-2023)
 ------------------
 
 * Updated dependencies
+
+
+3.2.2 (11-04-2023)
+------------------
+
+* Convert Dataclasses to Frozen for compatibility with latest python.
```

### Comparing `awsenergylabelerlib-3.2.1/LICENSE` & `awsenergylabelerlib-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/PKG-INFO` & `awsenergylabelerlib-3.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsenergylabelerlib
-Version: 3.2.1
+Version: 3.2.2
 Summary: Project energy labeling accounts and landing zone based on findings of Security Hub in AWS cloud.
 Home-page: https://github.com/schubergphilis/awsenergylabelerlib.git
 Author: Costas Tyfoxylos
 Author-email: ctyfoxylos@schubergphilis.com
 License: MIT
 Keywords: awsenergylabelerlib energy labeling aws security hub landing zone
 Classifier: Development Status :: 4 - Beta
@@ -275,7 +275,13 @@
 * Bump dependencies.
 
 
 3.2.1 (10-03-2023)
 ------------------
 
 * Updated dependencies
+
+
+3.2.2 (11-04-2023)
+------------------
+
+* Convert Dataclasses to Frozen for compatibility with latest python.
```

### Comparing `awsenergylabelerlib-3.2.1/Pipfile` & `awsenergylabelerlib-3.2.2/Pipfile`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/Pipfile.lock` & `awsenergylabelerlib-3.2.2/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9860585016835017%*

 * *Differences: {"'default'": "{'boto3': {'hashes': "*

 * *              "['sha256:8972a5e0a04ea6f477c41e390765a46ec7bcffb62f99d4a0774ce70fb87bea59', "*

 * *              "'sha256:97d942d958cac28687187b89ee88ac760e0fa3007094cb1d6b16e241144306f3'], "*

 * *              "'version': '==1.26.110'}, 'botocore': {'hashes': "*

 * *              "['sha256:39879fcc3d263513f9ba92cc5060b5a4dbe54f758a917be29c7a71132e34f399', "*

 * *              "'sha256:9d5054159782b19f27bff3e5a65bc494dc323255e889ea3abec002711a1fb0c0'], "*

 * *              "'version': '==1.29.11 […]*

```diff
@@ -12,27 +12,27 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "boto3": {
             "hashes": [
-                "sha256:5374c409d0153e5da4ccde3a0f7e3efac81ce7c60e4e18ffc9acc87c67e0c0a3",
-                "sha256:f4839565feeaaca4ef775b74a8df996b79b61d988db62c90571bcc948a9f24c5"
+                "sha256:8972a5e0a04ea6f477c41e390765a46ec7bcffb62f99d4a0774ce70fb87bea59",
+                "sha256:97d942d958cac28687187b89ee88ac760e0fa3007094cb1d6b16e241144306f3"
             ],
             "index": "pypi",
-            "version": "==1.26.88"
+            "version": "==1.26.110"
         },
         "botocore": {
             "hashes": [
-                "sha256:48ed2af0a10e7c15a3445eda62f665b106a2aba4ffa1ce730d7083022fd9596f",
-                "sha256:c320275d18ee140005ace4d04e9e720d5b1e30625cfde5267b1fc5133fd4d44d"
+                "sha256:39879fcc3d263513f9ba92cc5060b5a4dbe54f758a917be29c7a71132e34f399",
+                "sha256:9d5054159782b19f27bff3e5a65bc494dc323255e889ea3abec002711a1fb0c0"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.88"
+            "version": "==1.29.110"
         },
         "cachetools": {
             "hashes": [
                 "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
                 "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "index": "pypi",
@@ -92,37 +92,37 @@
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
+                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "version": "==1.26.15"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
                 "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.13"
         },
         "astroid": {
             "hashes": [
-                "sha256:525f126d5dc1b8b0b6ee398b33159105615d92dc4a17f2cd064125d57f6186fa",
-                "sha256:e3e4d0ffc2d15d954065579689c36aac57a339a4679a679579af6401db4d3fdb"
+                "sha256:6e61b85c891ec53b07471aec5878f4ac6446a41e590ede0f2ce095f39f7d49dd",
+                "sha256:dea89d9f99f491c66ac9c04ebddf91e4acf8bd711722175fe6245c0725cc19bb"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.15.0"
+            "version": "==2.15.2"
         },
         "babel": {
             "hashes": [
                 "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
                 "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
             "markers": "python_version >= '3.7'",
@@ -340,97 +340,93 @@
                 "sha256:7c991aa71a4577af2f82600d8f8f3a89f936baeaf9b50a9c197da014e5bf16b0"
             ],
             "index": "pypi",
             "version": "==15.0.1"
         },
         "coverage": {
             "hashes": [
-                "sha256:0339dc3237c0d31c3b574f19c57985fcbe494280153bbcad33f2cdf469f4ac3e",
-                "sha256:09643fb0df8e29f7417adc3f40aaf379d071ee8f0350ab290517c7004f05360b",
-                "sha256:0bd7e628f6c3ec4e7d2d24ec0e50aae4e5ae95ea644e849d92ae4805650b4c4e",
-                "sha256:0cf557827be7eca1c38a2480484d706693e7bb1929e129785fe59ec155a59de6",
-                "sha256:0f8318ed0f3c376cfad8d3520f496946977abde080439d6689d7799791457454",
-                "sha256:1b7fb13850ecb29b62a447ac3516c777b0e7a09ecb0f4bb6718a8654c87dfc80",
-                "sha256:22c308bc508372576ffa3d2dbc4824bb70d28eeb4fcd79d4d1aed663a06630d0",
-                "sha256:3004765bca3acd9e015794e5c2f0c9a05587f5e698127ff95e9cfba0d3f29339",
-                "sha256:3a209d512d157379cc9ab697cbdbb4cfd18daa3e7eebaa84c3d20b6af0037384",
-                "sha256:436313d129db7cf5b4ac355dd2bd3f7c7e5294af077b090b85de75f8458b8616",
-                "sha256:49567ec91fc5e0b15356da07a2feabb421d62f52a9fff4b1ec40e9e19772f5f8",
-                "sha256:4dd34a935de268a133e4741827ae951283a28c0125ddcdbcbba41c4b98f2dfef",
-                "sha256:570c21a29493b350f591a4b04c158ce1601e8d18bdcd21db136fbb135d75efa6",
-                "sha256:5928b85416a388dd557ddc006425b0c37e8468bd1c3dc118c1a3de42f59e2a54",
-                "sha256:5d2b9b5e70a21474c105a133ba227c61bc95f2ac3b66861143ce39a5ea4b3f84",
-                "sha256:617a94ada56bbfe547aa8d1b1a2b8299e2ec1ba14aac1d4b26a9f7d6158e1273",
-                "sha256:6a034480e9ebd4e83d1aa0453fd78986414b5d237aea89a8fdc35d330aa13bae",
-                "sha256:6fce673f79a0e017a4dc35e18dc7bb90bf6d307c67a11ad5e61ca8d42b87cbff",
-                "sha256:78d2c3dde4c0b9be4b02067185136b7ee4681978228ad5ec1278fa74f5ca3e99",
-                "sha256:7f099da6958ddfa2ed84bddea7515cb248583292e16bb9231d151cd528eab657",
-                "sha256:80559eaf6c15ce3da10edb7977a1548b393db36cbc6cf417633eca05d84dd1ed",
-                "sha256:834c2172edff5a08d78e2f53cf5e7164aacabeb66b369f76e7bb367ca4e2d993",
-                "sha256:861cc85dfbf55a7a768443d90a07e0ac5207704a9f97a8eb753292a7fcbdfcfc",
-                "sha256:8649371570551d2fd7dee22cfbf0b61f1747cdfb2b7587bb551e4beaaa44cb97",
-                "sha256:87dc37f16fb5e3a28429e094145bf7c1753e32bb50f662722e378c5851f7fdc6",
-                "sha256:8a6450da4c7afc4534305b2b7d8650131e130610cea448ff240b6ab73d7eab63",
-                "sha256:8d3843ca645f62c426c3d272902b9de90558e9886f15ddf5efe757b12dd376f5",
-                "sha256:8dca3c1706670297851bca1acff9618455122246bdae623be31eca744ade05ec",
-                "sha256:97a3189e019d27e914ecf5c5247ea9f13261d22c3bb0cfcfd2a9b179bb36f8b1",
-                "sha256:99f4dd81b2bb8fc67c3da68b1f5ee1650aca06faa585cbc6818dbf67893c6d58",
-                "sha256:9e872b082b32065ac2834149dc0adc2a2e6d8203080501e1e3c3c77851b466f9",
-                "sha256:a81dbcf6c6c877986083d00b834ac1e84b375220207a059ad45d12f6e518a4e3",
-                "sha256:abacd0a738e71b20e224861bc87e819ef46fedba2fb01bc1af83dfd122e9c319",
-                "sha256:ae82c988954722fa07ec5045c57b6d55bc1a0890defb57cf4a712ced65b26ddd",
-                "sha256:b0c0d46de5dd97f6c2d1b560bf0fcf0215658097b604f1840365296302a9d1fb",
-                "sha256:b1991a6d64231a3e5bbe3099fb0dd7c9aeaa4275ad0e0aeff4cb9ef885c62ba2",
-                "sha256:b2167d116309f564af56f9aa5e75ef710ef871c5f9b313a83050035097b56820",
-                "sha256:bd5a12239c0006252244f94863f1c518ac256160cd316ea5c47fb1a11b25889a",
-                "sha256:bdd3f2f285ddcf2e75174248b2406189261a79e7fedee2ceeadc76219b6faa0e",
-                "sha256:c77f2a9093ccf329dd523a9b2b3c854c20d2a3d968b6def3b820272ca6732242",
-                "sha256:cb5f152fb14857cbe7f3e8c9a5d98979c4c66319a33cad6e617f0067c9accdc4",
-                "sha256:cca7c0b7f5881dfe0291ef09ba7bb1582cb92ab0aeffd8afb00c700bf692415a",
-                "sha256:d2ef6cae70168815ed91388948b5f4fcc69681480a0061114db737f957719f03",
-                "sha256:d9256d4c60c4bbfec92721b51579c50f9e5062c21c12bec56b55292464873508",
-                "sha256:e191a63a05851f8bce77bc875e75457f9b01d42843f8bd7feed2fc26bbe60833",
-                "sha256:e2b50ebc2b6121edf352336d503357321b9d8738bb7a72d06fc56153fd3f4cd8",
-                "sha256:e3ea04b23b114572b98a88c85379e9e9ae031272ba1fb9b532aa934c621626d4",
-                "sha256:e4d70c853f0546855f027890b77854508bdb4d6a81242a9d804482e667fff6e6",
-                "sha256:f29351393eb05e6326f044a7b45ed8e38cb4dcc38570d12791f271399dc41431",
-                "sha256:f3d07edb912a978915576a776756069dede66d012baa503022d3a0adba1b6afa",
-                "sha256:fac6343bae03b176e9b58104a9810df3cdccd5cfed19f99adfa807ffbf43cf9b"
+                "sha256:06ddd9c0249a0546997fdda5a30fbcb40f23926df0a874a60a8a185bc3a87d93",
+                "sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013",
+                "sha256:0f3736a5d34e091b0a611964c6262fd68ca4363df56185902528f0b75dbb9c1f",
+                "sha256:1127b16220f7bfb3f1049ed4a62d26d81970a723544e8252db0efde853268e21",
+                "sha256:172db976ae6327ed4728e2507daf8a4de73c7cc89796483e0a9198fd2e47b462",
+                "sha256:182eb9ac3f2b4874a1f41b78b87db20b66da6b9cdc32737fbbf4fea0c35b23fc",
+                "sha256:1bb1e77a9a311346294621be905ea8a2c30d3ad371fc15bb72e98bfcfae532df",
+                "sha256:1fd78b911aea9cec3b7e1e2622c8018d51c0d2bbcf8faaf53c2497eb114911c1",
+                "sha256:20d1a2a76bb4eb00e4d36b9699f9b7aba93271c9c29220ad4c6a9581a0320235",
+                "sha256:21b154aba06df42e4b96fc915512ab39595105f6c483991287021ed95776d934",
+                "sha256:2c2e58e45fe53fab81f85474e5d4d226eeab0f27b45aa062856c89389da2f0d9",
+                "sha256:2c3b2803e730dc2797a017335827e9da6da0e84c745ce0f552e66400abdfb9a1",
+                "sha256:3146b8e16fa60427e03884301bf8209221f5761ac754ee6b267642a2fd354c48",
+                "sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4",
+                "sha256:387065e420aed3c71b61af7e82c7b6bc1c592f7e3c7a66e9f78dd178699da4fe",
+                "sha256:3f04becd4fcda03c0160d0da9c8f0c246bc78f2f7af0feea1ec0930e7c93fa4a",
+                "sha256:4a42e1eff0ca9a7cb7dc9ecda41dfc7cbc17cb1d02117214be0561bd1134772b",
+                "sha256:4ea748802cc0de4de92ef8244dd84ffd793bd2e7be784cd8394d557a3c751e21",
+                "sha256:55416d7385774285b6e2a5feca0af9652f7f444a4fa3d29d8ab052fafef9d00d",
+                "sha256:5d0391fb4cfc171ce40437f67eb050a340fdbd0f9f49d6353a387f1b7f9dd4fa",
+                "sha256:63cdeaac4ae85a179a8d6bc09b77b564c096250d759eed343a89d91bce8b6367",
+                "sha256:72fcae5bcac3333a4cf3b8f34eec99cea1187acd55af723bcbd559adfdcb5535",
+                "sha256:7c4ed4e9f3b123aa403ab424430b426a1992e6f4c8fd3cb56ea520446e04d152",
+                "sha256:83957d349838a636e768251c7e9979e899a569794b44c3728eaebd11d848e58e",
+                "sha256:87ecc7c9a1a9f912e306997ffee020297ccb5ea388421fe62a2a02747e4d5539",
+                "sha256:8f69770f5ca1994cb32c38965e95f57504d3aea96b6c024624fdd5bb1aa494a1",
+                "sha256:8f6c930fd70d91ddee53194e93029e3ef2aabe26725aa3c2753df057e296b925",
+                "sha256:965ee3e782c7892befc25575fa171b521d33798132692df428a09efacaffe8d0",
+                "sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2",
+                "sha256:981b4df72c93e3bc04478153df516d385317628bd9c10be699c93c26ddcca8ab",
+                "sha256:aa784405f0c640940595fa0f14064d8e84aff0b0f762fa18393e2760a2cf5841",
+                "sha256:ae7863a1d8db6a014b6f2ff9c1582ab1aad55a6d25bac19710a8df68921b6e30",
+                "sha256:aeae2aa38395b18106e552833f2a50c27ea0000122bde421c31d11ed7e6f9c91",
+                "sha256:b2317d5ed777bf5a033e83d4f1389fd4ef045763141d8f10eb09a7035cee774c",
+                "sha256:be19931a8dcbe6ab464f3339966856996b12a00f9fe53f346ab3be872d03e257",
+                "sha256:be9824c1c874b73b96288c6d3de793bf7f3a597770205068c6163ea1f326e8b9",
+                "sha256:c0045f8f23a5fb30b2eb3b8a83664d8dc4fb58faddf8155d7109166adb9f2040",
+                "sha256:c86bd45d1659b1ae3d0ba1909326b03598affbc9ed71520e0ff8c31a993ad911",
+                "sha256:ca0f34363e2634deffd390a0fef1aa99168ae9ed2af01af4a1f5865e362f8623",
+                "sha256:d298c2815fa4891edd9abe5ad6e6cb4207104c7dd9fd13aea3fdebf6f9b91259",
+                "sha256:d2a3a6146fe9319926e1d477842ca2a63fe99af5ae690b1f5c11e6af074a6b5c",
+                "sha256:dfd393094cd82ceb9b40df4c77976015a314b267d498268a076e940fe7be6b79",
+                "sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5",
+                "sha256:ea3f5bc91d7d457da7d48c7a732beaf79d0c8131df3ab278e6bba6297e23c6c4",
+                "sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4",
+                "sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22",
+                "sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd",
+                "sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1",
+                "sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910",
+                "sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859",
+                "sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312"
             ],
             "index": "pypi",
-            "version": "==7.2.1"
+            "version": "==7.2.3"
         },
         "cryptography": {
             "hashes": [
-                "sha256:103e8f7155f3ce2ffa0049fe60169878d47a4364b277906386f8de21c9234aa1",
-                "sha256:23df8ca3f24699167daf3e23e51f7ba7334d504af63a94af468f468b975b7dd7",
-                "sha256:2725672bb53bb92dc7b4150d233cd4b8c59615cd8288d495eaa86db00d4e5c06",
-                "sha256:30b1d1bfd00f6fc80d11300a29f1d8ab2b8d9febb6ed4a38a76880ec564fae84",
-                "sha256:35d658536b0a4117c885728d1a7032bdc9a5974722ae298d6c533755a6ee3915",
-                "sha256:50cadb9b2f961757e712a9737ef33d89b8190c3ea34d0fb6675e00edbe35d074",
-                "sha256:5f8c682e736513db7d04349b4f6693690170f95aac449c56f97415c6980edef5",
-                "sha256:6236a9610c912b129610eb1a274bdc1350b5df834d124fa84729ebeaf7da42c3",
-                "sha256:788b3921d763ee35dfdb04248d0e3de11e3ca8eb22e2e48fef880c42e1f3c8f9",
-                "sha256:8bc0008ef798231fac03fe7d26e82d601d15bd16f3afaad1c6113771566570f3",
-                "sha256:8f35c17bd4faed2bc7797d2a66cbb4f986242ce2e30340ab832e5d99ae60e011",
-                "sha256:b49a88ff802e1993b7f749b1eeb31134f03c8d5c956e3c125c75558955cda536",
-                "sha256:bc0521cce2c1d541634b19f3ac661d7a64f9555135e9d8af3980965be717fd4a",
-                "sha256:bc5b871e977c8ee5a1bbc42fa8d19bcc08baf0c51cbf1586b0e87a2694dde42f",
-                "sha256:c43ac224aabcbf83a947eeb8b17eaf1547bce3767ee2d70093b461f31729a480",
-                "sha256:d15809e0dbdad486f4ad0979753518f47980020b7a34e9fc56e8be4f60702fac",
-                "sha256:d7d84a512a59f4412ca8549b01f94be4161c94efc598bf09d027d67826beddc0",
-                "sha256:e029b844c21116564b8b61216befabca4b500e6816fa9f0ba49527653cae2108",
-                "sha256:e8a0772016feeb106efd28d4a328e77dc2edae84dfbac06061319fdb669ff828",
-                "sha256:e944fe07b6f229f4c1a06a7ef906a19652bdd9fd54c761b0ff87e83ae7a30354",
-                "sha256:eb40fe69cfc6f5cdab9a5ebd022131ba21453cf7b8a7fd3631f45bbf52bed612",
-                "sha256:fa507318e427169ade4e9eccef39e9011cdc19534f55ca2f36ec3f388c1f70f3",
-                "sha256:ffd394c7896ed7821a6d13b24657c6a34b6e2650bd84ae063cf11ccffa4f1a97"
+                "sha256:0a4e3406cfed6b1f6d6e87ed243363652b2586b2d917b0609ca4f97072994405",
+                "sha256:1e0af458515d5e4028aad75f3bb3fe7a31e46ad920648cd59b64d3da842e4356",
+                "sha256:2803f2f8b1e95f614419926c7e6f55d828afc614ca5ed61543877ae668cc3472",
+                "sha256:28d63d75bf7ae4045b10de5413fb1d6338616e79015999ad9cf6fc538f772d41",
+                "sha256:32057d3d0ab7d4453778367ca43e99ddb711770477c4f072a51b3ca69602780a",
+                "sha256:3a4805a4ca729d65570a1b7cac84eac1e431085d40387b7d3bbaa47e39890b88",
+                "sha256:63dac2d25c47f12a7b8aa60e528bfb3c51c5a6c5a9f7c86987909c6c79765554",
+                "sha256:650883cc064297ef3676b1db1b7b1df6081794c4ada96fa457253c4cc40f97db",
+                "sha256:6f2bbd72f717ce33100e6467572abaedc61f1acb87b8d546001328d7f466b778",
+                "sha256:7c872413353c70e0263a9368c4993710070e70ab3e5318d85510cc91cce77e7c",
+                "sha256:918cb89086c7d98b1b86b9fdb70c712e5a9325ba6f7d7cfb509e784e0cfc6917",
+                "sha256:9618a87212cb5200500e304e43691111570e1f10ec3f35569fdfcd17e28fd797",
+                "sha256:a805a7bce4a77d51696410005b3e85ae2839bad9aa38894afc0aa99d8e0c3160",
+                "sha256:cc3a621076d824d75ab1e1e530e66e7e8564e357dd723f2533225d40fe35c60c",
+                "sha256:cd033d74067d8928ef00a6b1327c8ea0452523967ca4463666eeba65ca350d4c",
+                "sha256:cf91e428c51ef692b82ce786583e214f58392399cf65c341bc7301d096fa3ba2",
+                "sha256:d36bbeb99704aabefdca5aee4eba04455d7a27ceabd16f3b3ba9bdcc31da86c4",
+                "sha256:d8aa3609d337ad85e4eb9bb0f8bcf6e4409bfb86e706efa9a027912169e89122",
+                "sha256:f5d7b79fa56bc29580faafc2ff736ce05ba31feaa9d4735048b0de7d9ceb2b94"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==39.0.2"
+            "version": "==40.0.1"
         },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
@@ -463,19 +459,19 @@
                 "sha256:a2986c21e4aba6b9870df40ef487a17be863cb7778dcf1c01e25917b7cd210bb"
             ],
             "index": "pypi",
             "version": "==2.2.0"
         },
         "filelock": {
             "hashes": [
-                "sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de",
-                "sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d"
+                "sha256:3618c0da67adcc0506b015fd11ef7faf1b493f0b40d87728e19986b536890c37",
+                "sha256:f08a52314748335c6460fc8fe40cd5638b85001225db78c2aa01c8c0db83b318"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.9.0"
+            "version": "==3.11.0"
         },
         "flake8": {
             "hashes": [
                 "sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db",
                 "sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248"
             ],
             "markers": "python_full_version >= '3.6.1'",
@@ -534,19 +530,19 @@
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad",
-                "sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d"
+                "sha256:23c2bcae4762dfb0bbe072d358faec24957901d75b6c4ab11172c0c982532402",
+                "sha256:8f8bd2af397cf33bd344d35cfe7f489219b7d14fc79a3f854b75b8417e9226b0"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==6.0.0"
+            "version": "==6.3.0"
         },
         "isort": {
             "hashes": [
                 "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
                 "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
             ],
             "markers": "python_full_version >= '3.8.0'",
@@ -752,19 +748,19 @@
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:13b08a53ed71021350c9e300d4ea8668438fb0046ab3937ac9a29913a1a1350a",
-                "sha256:accc3665857288317f32c7bebb5a8e482ba717b474f3fc1d18ca7f9214be0cef"
+                "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08",
+                "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.0"
+            "version": "==3.2.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -815,27 +811,27 @@
                 "sha256:491feb020dca48ccc562a8c0cbe8df07ee13078df59813b83959cbdada312ea3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.5.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094",
+                "sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.0"
         },
         "pylint": {
             "hashes": [
-                "sha256:1460829b6397cb5eb0cdb0b4fc4b556348e515cdca32115f74a1eb7c20b896b4",
-                "sha256:e097d8325f8c88e14ad12844e3fe2d963d3de871ea9a8f8ad25ab1c109889ddc"
+                "sha256:001cc91366a7df2970941d7e6bbefcbf98694e00102c1f121c531a814ddc2ea8",
+                "sha256:1b647da5249e7c279118f657ca28b6aaebb299f86bf92affc632acf199f7adbb"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.17.0"
+            "version": "==2.17.2"
         },
         "pylint-celery": {
             "hashes": [
                 "sha256:41e32094e7408d15c044178ea828dd524beedbdbe6f83f712c5e35bde1de4beb"
             ],
             "version": "==0.3"
         },
@@ -858,19 +854,19 @@
                 "sha256:ce48bc0516ae9415dd5c752c940dfe601b18fe0f48aa249f2386adfa95a004dd"
             ],
             "markers": "python_full_version >= '3.6.2'",
             "version": "==0.7"
         },
         "pyproject-api": {
             "hashes": [
-                "sha256:0962df21f3e633b8ddb9567c011e6c1b3dcdfc31b7860c0ede7e24c5a1200fbe",
-                "sha256:4c111277dfb96bcd562c6245428f27250b794bfe3e210b8714c4f893952f2c17"
+                "sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9",
+                "sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.5.0"
+            "version": "==1.5.1"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
@@ -952,19 +948,19 @@
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:91954fe80cfb7985727a467ca98a7618e5dd15178cc2da10f553b36a93859001",
-                "sha256:a104f37270bf677148d8acb07d33be1569eeee87e2d1beb286a4e9113caf6f2f"
+                "sha256:540c7d6d26a1178e8e8b37e9ba44573a3cd1464ff6348b99ee7061b95d1c6333",
+                "sha256:dc84400a9d842b3a9c5ff74addd8eb798d155f36c1c91303888e0a66850d2a15"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.2"
+            "version": "==13.3.3"
         },
         "secretstorage": {
             "hashes": [
                 "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
@@ -981,22 +977,14 @@
         "setoptconf-tmp": {
             "hashes": [
                 "sha256:76035d5cd1593d38b9056ae12d460eca3aaa34ad05c315b69145e138ba80a745",
                 "sha256:e0480addd11347ba52f762f3c4d8afa3e10ad0affbc53e3ffddc0ca5f27d5778"
             ],
             "version": "==0.3.1"
         },
-        "setuptools": {
-            "hashes": [
-                "sha256:2ee892cd5f29f3373097f5a814697e397cf3ce313616df0af11231e2ad118077",
-                "sha256:b78aaa36f6b90a074c1fa651168723acbf45d14cb1196b6f02c0fd07f17623b2"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==67.6.0"
-        },
         "sh": {
             "hashes": [
                 "sha256:ae3258c5249493cebe73cb4e18253a41ed69262484bad36fdb3efcb8ad8870bb",
                 "sha256:b52bf5833ed01c7b5c5fb73a7f71b3d98d48e9b9b8764236237bdc7ecae850fc"
             ],
             "markers": "sys_platform != 'win32'",
             "version": "==1.12.14"
@@ -1062,19 +1050,19 @@
                 "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==2.0.1"
         },
         "sphinxcontrib-jquery": {
             "hashes": [
-                "sha256:8fb65f6dba84bf7bcd1aea1f02ab3955ac34611d838bcc95d4983b805b234daa",
-                "sha256:ed47fa425c338ffebe3c37e1cdb56e30eb806116b85f01055b158c7057fdb995"
+                "sha256:1620739f04e36a2c779f1a131a2dfd49b2fd07351bf1968ced074365933abc7a",
+                "sha256:f936030d7d0147dd026a4f2b5a57343d233f1fc7b363f68b3d4f1cb0993878ae"
             ],
             "markers": "python_version >= '3.1'",
-            "version": "==2.0.0"
+            "version": "==4.1"
         },
         "sphinxcontrib-jsmath": {
             "hashes": [
                 "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178",
                 "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
             "markers": "python_version >= '3.5'",
@@ -1110,27 +1098,27 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:07de26b0d8cfc18f871aec595fda24d95b08fef89d147caa861939f37230bf4b",
-                "sha256:71b952e5721688937fb02cf9d354dbcf0785066149d2855e44531ebdd2b65d73"
+                "sha256:5325463a7da2ef0c6bbfefb62a3dc883aebe679984709aee32a317907d0a8d3c",
+                "sha256:f392ef70ad87a672f02519f99967d28a4d3047133e2d1df936511465fbb3791d"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.11.6"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.7"
         },
         "tox": {
             "hashes": [
-                "sha256:9786671d23b673ace7499c602c5746e2a225d1ecd9d9f624d0461303f40bd93b",
-                "sha256:e3d4a65852f029e5ba441a01824d2d839d30bb8fb071635ef9cb53952698e6bf"
+                "sha256:6fa4dbd933d0e335b5392c81e9cd467630119b3669705dbad47814a93b6c9586",
+                "sha256:cd88e41aef9c71f0ba02b6d7939f102760b192b63458fbe04dbbaed82f7bf5f5"
             ],
             "index": "pypi",
-            "version": "==4.4.6"
+            "version": "==4.4.11"
         },
         "twine": {
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
@@ -1142,27 +1130,27 @@
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version < '3.10'",
             "version": "==4.5.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
+                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "version": "==1.26.15"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:3c22fa5a7c7aa106ced59934d2c20a2ecb7f49b4130b8bf444178a16b880fa45",
-                "sha256:a8a4b8ca1e28f864b7514a253f98c1d62b64e31e77325ba279248c65fb4fcef4"
+                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
+                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.20.0"
+            "version": "==20.21.0"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
```

### Comparing `awsenergylabelerlib-3.2.1/README.rst` & `awsenergylabelerlib-3.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/USAGE.rst` & `awsenergylabelerlib-3.2.2/USAGE.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/CONTRIBUTING.rst` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/HISTORY.rst` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -188,7 +188,13 @@
 * Bump dependencies.
 
 
 3.2.1 (10-03-2023)
 ------------------
 
 * Updated dependencies
+
+
+3.2.2 (11-04-2023)
+------------------
+
+* Convert Dataclasses to Frozen for compatibility with latest python.
```

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/LICENSE` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/LICENSE`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/Pipfile` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/Pipfile`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/Pipfile.lock` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9860585016835017%*

 * *Differences: {"'default'": "{'boto3': {'hashes': "*

 * *              "['sha256:8972a5e0a04ea6f477c41e390765a46ec7bcffb62f99d4a0774ce70fb87bea59', "*

 * *              "'sha256:97d942d958cac28687187b89ee88ac760e0fa3007094cb1d6b16e241144306f3'], "*

 * *              "'version': '==1.26.110'}, 'botocore': {'hashes': "*

 * *              "['sha256:39879fcc3d263513f9ba92cc5060b5a4dbe54f758a917be29c7a71132e34f399', "*

 * *              "'sha256:9d5054159782b19f27bff3e5a65bc494dc323255e889ea3abec002711a1fb0c0'], "*

 * *              "'version': '==1.29.11 […]*

```diff
@@ -12,27 +12,27 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "boto3": {
             "hashes": [
-                "sha256:5374c409d0153e5da4ccde3a0f7e3efac81ce7c60e4e18ffc9acc87c67e0c0a3",
-                "sha256:f4839565feeaaca4ef775b74a8df996b79b61d988db62c90571bcc948a9f24c5"
+                "sha256:8972a5e0a04ea6f477c41e390765a46ec7bcffb62f99d4a0774ce70fb87bea59",
+                "sha256:97d942d958cac28687187b89ee88ac760e0fa3007094cb1d6b16e241144306f3"
             ],
             "index": "pypi",
-            "version": "==1.26.88"
+            "version": "==1.26.110"
         },
         "botocore": {
             "hashes": [
-                "sha256:48ed2af0a10e7c15a3445eda62f665b106a2aba4ffa1ce730d7083022fd9596f",
-                "sha256:c320275d18ee140005ace4d04e9e720d5b1e30625cfde5267b1fc5133fd4d44d"
+                "sha256:39879fcc3d263513f9ba92cc5060b5a4dbe54f758a917be29c7a71132e34f399",
+                "sha256:9d5054159782b19f27bff3e5a65bc494dc323255e889ea3abec002711a1fb0c0"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.88"
+            "version": "==1.29.110"
         },
         "cachetools": {
             "hashes": [
                 "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
                 "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "index": "pypi",
@@ -92,37 +92,37 @@
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
+                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "version": "==1.26.15"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
                 "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.13"
         },
         "astroid": {
             "hashes": [
-                "sha256:525f126d5dc1b8b0b6ee398b33159105615d92dc4a17f2cd064125d57f6186fa",
-                "sha256:e3e4d0ffc2d15d954065579689c36aac57a339a4679a679579af6401db4d3fdb"
+                "sha256:6e61b85c891ec53b07471aec5878f4ac6446a41e590ede0f2ce095f39f7d49dd",
+                "sha256:dea89d9f99f491c66ac9c04ebddf91e4acf8bd711722175fe6245c0725cc19bb"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.15.0"
+            "version": "==2.15.2"
         },
         "babel": {
             "hashes": [
                 "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
                 "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
             "markers": "python_version >= '3.7'",
@@ -340,97 +340,93 @@
                 "sha256:7c991aa71a4577af2f82600d8f8f3a89f936baeaf9b50a9c197da014e5bf16b0"
             ],
             "index": "pypi",
             "version": "==15.0.1"
         },
         "coverage": {
             "hashes": [
-                "sha256:0339dc3237c0d31c3b574f19c57985fcbe494280153bbcad33f2cdf469f4ac3e",
-                "sha256:09643fb0df8e29f7417adc3f40aaf379d071ee8f0350ab290517c7004f05360b",
-                "sha256:0bd7e628f6c3ec4e7d2d24ec0e50aae4e5ae95ea644e849d92ae4805650b4c4e",
-                "sha256:0cf557827be7eca1c38a2480484d706693e7bb1929e129785fe59ec155a59de6",
-                "sha256:0f8318ed0f3c376cfad8d3520f496946977abde080439d6689d7799791457454",
-                "sha256:1b7fb13850ecb29b62a447ac3516c777b0e7a09ecb0f4bb6718a8654c87dfc80",
-                "sha256:22c308bc508372576ffa3d2dbc4824bb70d28eeb4fcd79d4d1aed663a06630d0",
-                "sha256:3004765bca3acd9e015794e5c2f0c9a05587f5e698127ff95e9cfba0d3f29339",
-                "sha256:3a209d512d157379cc9ab697cbdbb4cfd18daa3e7eebaa84c3d20b6af0037384",
-                "sha256:436313d129db7cf5b4ac355dd2bd3f7c7e5294af077b090b85de75f8458b8616",
-                "sha256:49567ec91fc5e0b15356da07a2feabb421d62f52a9fff4b1ec40e9e19772f5f8",
-                "sha256:4dd34a935de268a133e4741827ae951283a28c0125ddcdbcbba41c4b98f2dfef",
-                "sha256:570c21a29493b350f591a4b04c158ce1601e8d18bdcd21db136fbb135d75efa6",
-                "sha256:5928b85416a388dd557ddc006425b0c37e8468bd1c3dc118c1a3de42f59e2a54",
-                "sha256:5d2b9b5e70a21474c105a133ba227c61bc95f2ac3b66861143ce39a5ea4b3f84",
-                "sha256:617a94ada56bbfe547aa8d1b1a2b8299e2ec1ba14aac1d4b26a9f7d6158e1273",
-                "sha256:6a034480e9ebd4e83d1aa0453fd78986414b5d237aea89a8fdc35d330aa13bae",
-                "sha256:6fce673f79a0e017a4dc35e18dc7bb90bf6d307c67a11ad5e61ca8d42b87cbff",
-                "sha256:78d2c3dde4c0b9be4b02067185136b7ee4681978228ad5ec1278fa74f5ca3e99",
-                "sha256:7f099da6958ddfa2ed84bddea7515cb248583292e16bb9231d151cd528eab657",
-                "sha256:80559eaf6c15ce3da10edb7977a1548b393db36cbc6cf417633eca05d84dd1ed",
-                "sha256:834c2172edff5a08d78e2f53cf5e7164aacabeb66b369f76e7bb367ca4e2d993",
-                "sha256:861cc85dfbf55a7a768443d90a07e0ac5207704a9f97a8eb753292a7fcbdfcfc",
-                "sha256:8649371570551d2fd7dee22cfbf0b61f1747cdfb2b7587bb551e4beaaa44cb97",
-                "sha256:87dc37f16fb5e3a28429e094145bf7c1753e32bb50f662722e378c5851f7fdc6",
-                "sha256:8a6450da4c7afc4534305b2b7d8650131e130610cea448ff240b6ab73d7eab63",
-                "sha256:8d3843ca645f62c426c3d272902b9de90558e9886f15ddf5efe757b12dd376f5",
-                "sha256:8dca3c1706670297851bca1acff9618455122246bdae623be31eca744ade05ec",
-                "sha256:97a3189e019d27e914ecf5c5247ea9f13261d22c3bb0cfcfd2a9b179bb36f8b1",
-                "sha256:99f4dd81b2bb8fc67c3da68b1f5ee1650aca06faa585cbc6818dbf67893c6d58",
-                "sha256:9e872b082b32065ac2834149dc0adc2a2e6d8203080501e1e3c3c77851b466f9",
-                "sha256:a81dbcf6c6c877986083d00b834ac1e84b375220207a059ad45d12f6e518a4e3",
-                "sha256:abacd0a738e71b20e224861bc87e819ef46fedba2fb01bc1af83dfd122e9c319",
-                "sha256:ae82c988954722fa07ec5045c57b6d55bc1a0890defb57cf4a712ced65b26ddd",
-                "sha256:b0c0d46de5dd97f6c2d1b560bf0fcf0215658097b604f1840365296302a9d1fb",
-                "sha256:b1991a6d64231a3e5bbe3099fb0dd7c9aeaa4275ad0e0aeff4cb9ef885c62ba2",
-                "sha256:b2167d116309f564af56f9aa5e75ef710ef871c5f9b313a83050035097b56820",
-                "sha256:bd5a12239c0006252244f94863f1c518ac256160cd316ea5c47fb1a11b25889a",
-                "sha256:bdd3f2f285ddcf2e75174248b2406189261a79e7fedee2ceeadc76219b6faa0e",
-                "sha256:c77f2a9093ccf329dd523a9b2b3c854c20d2a3d968b6def3b820272ca6732242",
-                "sha256:cb5f152fb14857cbe7f3e8c9a5d98979c4c66319a33cad6e617f0067c9accdc4",
-                "sha256:cca7c0b7f5881dfe0291ef09ba7bb1582cb92ab0aeffd8afb00c700bf692415a",
-                "sha256:d2ef6cae70168815ed91388948b5f4fcc69681480a0061114db737f957719f03",
-                "sha256:d9256d4c60c4bbfec92721b51579c50f9e5062c21c12bec56b55292464873508",
-                "sha256:e191a63a05851f8bce77bc875e75457f9b01d42843f8bd7feed2fc26bbe60833",
-                "sha256:e2b50ebc2b6121edf352336d503357321b9d8738bb7a72d06fc56153fd3f4cd8",
-                "sha256:e3ea04b23b114572b98a88c85379e9e9ae031272ba1fb9b532aa934c621626d4",
-                "sha256:e4d70c853f0546855f027890b77854508bdb4d6a81242a9d804482e667fff6e6",
-                "sha256:f29351393eb05e6326f044a7b45ed8e38cb4dcc38570d12791f271399dc41431",
-                "sha256:f3d07edb912a978915576a776756069dede66d012baa503022d3a0adba1b6afa",
-                "sha256:fac6343bae03b176e9b58104a9810df3cdccd5cfed19f99adfa807ffbf43cf9b"
+                "sha256:06ddd9c0249a0546997fdda5a30fbcb40f23926df0a874a60a8a185bc3a87d93",
+                "sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013",
+                "sha256:0f3736a5d34e091b0a611964c6262fd68ca4363df56185902528f0b75dbb9c1f",
+                "sha256:1127b16220f7bfb3f1049ed4a62d26d81970a723544e8252db0efde853268e21",
+                "sha256:172db976ae6327ed4728e2507daf8a4de73c7cc89796483e0a9198fd2e47b462",
+                "sha256:182eb9ac3f2b4874a1f41b78b87db20b66da6b9cdc32737fbbf4fea0c35b23fc",
+                "sha256:1bb1e77a9a311346294621be905ea8a2c30d3ad371fc15bb72e98bfcfae532df",
+                "sha256:1fd78b911aea9cec3b7e1e2622c8018d51c0d2bbcf8faaf53c2497eb114911c1",
+                "sha256:20d1a2a76bb4eb00e4d36b9699f9b7aba93271c9c29220ad4c6a9581a0320235",
+                "sha256:21b154aba06df42e4b96fc915512ab39595105f6c483991287021ed95776d934",
+                "sha256:2c2e58e45fe53fab81f85474e5d4d226eeab0f27b45aa062856c89389da2f0d9",
+                "sha256:2c3b2803e730dc2797a017335827e9da6da0e84c745ce0f552e66400abdfb9a1",
+                "sha256:3146b8e16fa60427e03884301bf8209221f5761ac754ee6b267642a2fd354c48",
+                "sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4",
+                "sha256:387065e420aed3c71b61af7e82c7b6bc1c592f7e3c7a66e9f78dd178699da4fe",
+                "sha256:3f04becd4fcda03c0160d0da9c8f0c246bc78f2f7af0feea1ec0930e7c93fa4a",
+                "sha256:4a42e1eff0ca9a7cb7dc9ecda41dfc7cbc17cb1d02117214be0561bd1134772b",
+                "sha256:4ea748802cc0de4de92ef8244dd84ffd793bd2e7be784cd8394d557a3c751e21",
+                "sha256:55416d7385774285b6e2a5feca0af9652f7f444a4fa3d29d8ab052fafef9d00d",
+                "sha256:5d0391fb4cfc171ce40437f67eb050a340fdbd0f9f49d6353a387f1b7f9dd4fa",
+                "sha256:63cdeaac4ae85a179a8d6bc09b77b564c096250d759eed343a89d91bce8b6367",
+                "sha256:72fcae5bcac3333a4cf3b8f34eec99cea1187acd55af723bcbd559adfdcb5535",
+                "sha256:7c4ed4e9f3b123aa403ab424430b426a1992e6f4c8fd3cb56ea520446e04d152",
+                "sha256:83957d349838a636e768251c7e9979e899a569794b44c3728eaebd11d848e58e",
+                "sha256:87ecc7c9a1a9f912e306997ffee020297ccb5ea388421fe62a2a02747e4d5539",
+                "sha256:8f69770f5ca1994cb32c38965e95f57504d3aea96b6c024624fdd5bb1aa494a1",
+                "sha256:8f6c930fd70d91ddee53194e93029e3ef2aabe26725aa3c2753df057e296b925",
+                "sha256:965ee3e782c7892befc25575fa171b521d33798132692df428a09efacaffe8d0",
+                "sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2",
+                "sha256:981b4df72c93e3bc04478153df516d385317628bd9c10be699c93c26ddcca8ab",
+                "sha256:aa784405f0c640940595fa0f14064d8e84aff0b0f762fa18393e2760a2cf5841",
+                "sha256:ae7863a1d8db6a014b6f2ff9c1582ab1aad55a6d25bac19710a8df68921b6e30",
+                "sha256:aeae2aa38395b18106e552833f2a50c27ea0000122bde421c31d11ed7e6f9c91",
+                "sha256:b2317d5ed777bf5a033e83d4f1389fd4ef045763141d8f10eb09a7035cee774c",
+                "sha256:be19931a8dcbe6ab464f3339966856996b12a00f9fe53f346ab3be872d03e257",
+                "sha256:be9824c1c874b73b96288c6d3de793bf7f3a597770205068c6163ea1f326e8b9",
+                "sha256:c0045f8f23a5fb30b2eb3b8a83664d8dc4fb58faddf8155d7109166adb9f2040",
+                "sha256:c86bd45d1659b1ae3d0ba1909326b03598affbc9ed71520e0ff8c31a993ad911",
+                "sha256:ca0f34363e2634deffd390a0fef1aa99168ae9ed2af01af4a1f5865e362f8623",
+                "sha256:d298c2815fa4891edd9abe5ad6e6cb4207104c7dd9fd13aea3fdebf6f9b91259",
+                "sha256:d2a3a6146fe9319926e1d477842ca2a63fe99af5ae690b1f5c11e6af074a6b5c",
+                "sha256:dfd393094cd82ceb9b40df4c77976015a314b267d498268a076e940fe7be6b79",
+                "sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5",
+                "sha256:ea3f5bc91d7d457da7d48c7a732beaf79d0c8131df3ab278e6bba6297e23c6c4",
+                "sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4",
+                "sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22",
+                "sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd",
+                "sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1",
+                "sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910",
+                "sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859",
+                "sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312"
             ],
             "index": "pypi",
-            "version": "==7.2.1"
+            "version": "==7.2.3"
         },
         "cryptography": {
             "hashes": [
-                "sha256:103e8f7155f3ce2ffa0049fe60169878d47a4364b277906386f8de21c9234aa1",
-                "sha256:23df8ca3f24699167daf3e23e51f7ba7334d504af63a94af468f468b975b7dd7",
-                "sha256:2725672bb53bb92dc7b4150d233cd4b8c59615cd8288d495eaa86db00d4e5c06",
-                "sha256:30b1d1bfd00f6fc80d11300a29f1d8ab2b8d9febb6ed4a38a76880ec564fae84",
-                "sha256:35d658536b0a4117c885728d1a7032bdc9a5974722ae298d6c533755a6ee3915",
-                "sha256:50cadb9b2f961757e712a9737ef33d89b8190c3ea34d0fb6675e00edbe35d074",
-                "sha256:5f8c682e736513db7d04349b4f6693690170f95aac449c56f97415c6980edef5",
-                "sha256:6236a9610c912b129610eb1a274bdc1350b5df834d124fa84729ebeaf7da42c3",
-                "sha256:788b3921d763ee35dfdb04248d0e3de11e3ca8eb22e2e48fef880c42e1f3c8f9",
-                "sha256:8bc0008ef798231fac03fe7d26e82d601d15bd16f3afaad1c6113771566570f3",
-                "sha256:8f35c17bd4faed2bc7797d2a66cbb4f986242ce2e30340ab832e5d99ae60e011",
-                "sha256:b49a88ff802e1993b7f749b1eeb31134f03c8d5c956e3c125c75558955cda536",
-                "sha256:bc0521cce2c1d541634b19f3ac661d7a64f9555135e9d8af3980965be717fd4a",
-                "sha256:bc5b871e977c8ee5a1bbc42fa8d19bcc08baf0c51cbf1586b0e87a2694dde42f",
-                "sha256:c43ac224aabcbf83a947eeb8b17eaf1547bce3767ee2d70093b461f31729a480",
-                "sha256:d15809e0dbdad486f4ad0979753518f47980020b7a34e9fc56e8be4f60702fac",
-                "sha256:d7d84a512a59f4412ca8549b01f94be4161c94efc598bf09d027d67826beddc0",
-                "sha256:e029b844c21116564b8b61216befabca4b500e6816fa9f0ba49527653cae2108",
-                "sha256:e8a0772016feeb106efd28d4a328e77dc2edae84dfbac06061319fdb669ff828",
-                "sha256:e944fe07b6f229f4c1a06a7ef906a19652bdd9fd54c761b0ff87e83ae7a30354",
-                "sha256:eb40fe69cfc6f5cdab9a5ebd022131ba21453cf7b8a7fd3631f45bbf52bed612",
-                "sha256:fa507318e427169ade4e9eccef39e9011cdc19534f55ca2f36ec3f388c1f70f3",
-                "sha256:ffd394c7896ed7821a6d13b24657c6a34b6e2650bd84ae063cf11ccffa4f1a97"
+                "sha256:0a4e3406cfed6b1f6d6e87ed243363652b2586b2d917b0609ca4f97072994405",
+                "sha256:1e0af458515d5e4028aad75f3bb3fe7a31e46ad920648cd59b64d3da842e4356",
+                "sha256:2803f2f8b1e95f614419926c7e6f55d828afc614ca5ed61543877ae668cc3472",
+                "sha256:28d63d75bf7ae4045b10de5413fb1d6338616e79015999ad9cf6fc538f772d41",
+                "sha256:32057d3d0ab7d4453778367ca43e99ddb711770477c4f072a51b3ca69602780a",
+                "sha256:3a4805a4ca729d65570a1b7cac84eac1e431085d40387b7d3bbaa47e39890b88",
+                "sha256:63dac2d25c47f12a7b8aa60e528bfb3c51c5a6c5a9f7c86987909c6c79765554",
+                "sha256:650883cc064297ef3676b1db1b7b1df6081794c4ada96fa457253c4cc40f97db",
+                "sha256:6f2bbd72f717ce33100e6467572abaedc61f1acb87b8d546001328d7f466b778",
+                "sha256:7c872413353c70e0263a9368c4993710070e70ab3e5318d85510cc91cce77e7c",
+                "sha256:918cb89086c7d98b1b86b9fdb70c712e5a9325ba6f7d7cfb509e784e0cfc6917",
+                "sha256:9618a87212cb5200500e304e43691111570e1f10ec3f35569fdfcd17e28fd797",
+                "sha256:a805a7bce4a77d51696410005b3e85ae2839bad9aa38894afc0aa99d8e0c3160",
+                "sha256:cc3a621076d824d75ab1e1e530e66e7e8564e357dd723f2533225d40fe35c60c",
+                "sha256:cd033d74067d8928ef00a6b1327c8ea0452523967ca4463666eeba65ca350d4c",
+                "sha256:cf91e428c51ef692b82ce786583e214f58392399cf65c341bc7301d096fa3ba2",
+                "sha256:d36bbeb99704aabefdca5aee4eba04455d7a27ceabd16f3b3ba9bdcc31da86c4",
+                "sha256:d8aa3609d337ad85e4eb9bb0f8bcf6e4409bfb86e706efa9a027912169e89122",
+                "sha256:f5d7b79fa56bc29580faafc2ff736ce05ba31feaa9d4735048b0de7d9ceb2b94"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==39.0.2"
+            "version": "==40.0.1"
         },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
@@ -463,19 +459,19 @@
                 "sha256:a2986c21e4aba6b9870df40ef487a17be863cb7778dcf1c01e25917b7cd210bb"
             ],
             "index": "pypi",
             "version": "==2.2.0"
         },
         "filelock": {
             "hashes": [
-                "sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de",
-                "sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d"
+                "sha256:3618c0da67adcc0506b015fd11ef7faf1b493f0b40d87728e19986b536890c37",
+                "sha256:f08a52314748335c6460fc8fe40cd5638b85001225db78c2aa01c8c0db83b318"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.9.0"
+            "version": "==3.11.0"
         },
         "flake8": {
             "hashes": [
                 "sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db",
                 "sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248"
             ],
             "markers": "python_full_version >= '3.6.1'",
@@ -534,19 +530,19 @@
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad",
-                "sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d"
+                "sha256:23c2bcae4762dfb0bbe072d358faec24957901d75b6c4ab11172c0c982532402",
+                "sha256:8f8bd2af397cf33bd344d35cfe7f489219b7d14fc79a3f854b75b8417e9226b0"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==6.0.0"
+            "version": "==6.3.0"
         },
         "isort": {
             "hashes": [
                 "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
                 "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
             ],
             "markers": "python_full_version >= '3.8.0'",
@@ -752,19 +748,19 @@
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:13b08a53ed71021350c9e300d4ea8668438fb0046ab3937ac9a29913a1a1350a",
-                "sha256:accc3665857288317f32c7bebb5a8e482ba717b474f3fc1d18ca7f9214be0cef"
+                "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08",
+                "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.0"
+            "version": "==3.2.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -815,27 +811,27 @@
                 "sha256:491feb020dca48ccc562a8c0cbe8df07ee13078df59813b83959cbdada312ea3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.5.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094",
+                "sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.0"
         },
         "pylint": {
             "hashes": [
-                "sha256:1460829b6397cb5eb0cdb0b4fc4b556348e515cdca32115f74a1eb7c20b896b4",
-                "sha256:e097d8325f8c88e14ad12844e3fe2d963d3de871ea9a8f8ad25ab1c109889ddc"
+                "sha256:001cc91366a7df2970941d7e6bbefcbf98694e00102c1f121c531a814ddc2ea8",
+                "sha256:1b647da5249e7c279118f657ca28b6aaebb299f86bf92affc632acf199f7adbb"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.17.0"
+            "version": "==2.17.2"
         },
         "pylint-celery": {
             "hashes": [
                 "sha256:41e32094e7408d15c044178ea828dd524beedbdbe6f83f712c5e35bde1de4beb"
             ],
             "version": "==0.3"
         },
@@ -858,19 +854,19 @@
                 "sha256:ce48bc0516ae9415dd5c752c940dfe601b18fe0f48aa249f2386adfa95a004dd"
             ],
             "markers": "python_full_version >= '3.6.2'",
             "version": "==0.7"
         },
         "pyproject-api": {
             "hashes": [
-                "sha256:0962df21f3e633b8ddb9567c011e6c1b3dcdfc31b7860c0ede7e24c5a1200fbe",
-                "sha256:4c111277dfb96bcd562c6245428f27250b794bfe3e210b8714c4f893952f2c17"
+                "sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9",
+                "sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.5.0"
+            "version": "==1.5.1"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
@@ -952,19 +948,19 @@
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:91954fe80cfb7985727a467ca98a7618e5dd15178cc2da10f553b36a93859001",
-                "sha256:a104f37270bf677148d8acb07d33be1569eeee87e2d1beb286a4e9113caf6f2f"
+                "sha256:540c7d6d26a1178e8e8b37e9ba44573a3cd1464ff6348b99ee7061b95d1c6333",
+                "sha256:dc84400a9d842b3a9c5ff74addd8eb798d155f36c1c91303888e0a66850d2a15"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.2"
+            "version": "==13.3.3"
         },
         "secretstorage": {
             "hashes": [
                 "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
@@ -981,22 +977,14 @@
         "setoptconf-tmp": {
             "hashes": [
                 "sha256:76035d5cd1593d38b9056ae12d460eca3aaa34ad05c315b69145e138ba80a745",
                 "sha256:e0480addd11347ba52f762f3c4d8afa3e10ad0affbc53e3ffddc0ca5f27d5778"
             ],
             "version": "==0.3.1"
         },
-        "setuptools": {
-            "hashes": [
-                "sha256:2ee892cd5f29f3373097f5a814697e397cf3ce313616df0af11231e2ad118077",
-                "sha256:b78aaa36f6b90a074c1fa651168723acbf45d14cb1196b6f02c0fd07f17623b2"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==67.6.0"
-        },
         "sh": {
             "hashes": [
                 "sha256:ae3258c5249493cebe73cb4e18253a41ed69262484bad36fdb3efcb8ad8870bb",
                 "sha256:b52bf5833ed01c7b5c5fb73a7f71b3d98d48e9b9b8764236237bdc7ecae850fc"
             ],
             "markers": "sys_platform != 'win32'",
             "version": "==1.12.14"
@@ -1062,19 +1050,19 @@
                 "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==2.0.1"
         },
         "sphinxcontrib-jquery": {
             "hashes": [
-                "sha256:8fb65f6dba84bf7bcd1aea1f02ab3955ac34611d838bcc95d4983b805b234daa",
-                "sha256:ed47fa425c338ffebe3c37e1cdb56e30eb806116b85f01055b158c7057fdb995"
+                "sha256:1620739f04e36a2c779f1a131a2dfd49b2fd07351bf1968ced074365933abc7a",
+                "sha256:f936030d7d0147dd026a4f2b5a57343d233f1fc7b363f68b3d4f1cb0993878ae"
             ],
             "markers": "python_version >= '3.1'",
-            "version": "==2.0.0"
+            "version": "==4.1"
         },
         "sphinxcontrib-jsmath": {
             "hashes": [
                 "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178",
                 "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
             "markers": "python_version >= '3.5'",
@@ -1110,27 +1098,27 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:07de26b0d8cfc18f871aec595fda24d95b08fef89d147caa861939f37230bf4b",
-                "sha256:71b952e5721688937fb02cf9d354dbcf0785066149d2855e44531ebdd2b65d73"
+                "sha256:5325463a7da2ef0c6bbfefb62a3dc883aebe679984709aee32a317907d0a8d3c",
+                "sha256:f392ef70ad87a672f02519f99967d28a4d3047133e2d1df936511465fbb3791d"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.11.6"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.7"
         },
         "tox": {
             "hashes": [
-                "sha256:9786671d23b673ace7499c602c5746e2a225d1ecd9d9f624d0461303f40bd93b",
-                "sha256:e3d4a65852f029e5ba441a01824d2d839d30bb8fb071635ef9cb53952698e6bf"
+                "sha256:6fa4dbd933d0e335b5392c81e9cd467630119b3669705dbad47814a93b6c9586",
+                "sha256:cd88e41aef9c71f0ba02b6d7939f102760b192b63458fbe04dbbaed82f7bf5f5"
             ],
             "index": "pypi",
-            "version": "==4.4.6"
+            "version": "==4.4.11"
         },
         "twine": {
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
@@ -1142,27 +1130,27 @@
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version < '3.10'",
             "version": "==4.5.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
+                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "version": "==1.26.15"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:3c22fa5a7c7aa106ced59934d2c20a2ecb7f49b4130b8bf444178a16b880fa45",
-                "sha256:a8a4b8ca1e28f864b7514a253f98c1d62b64e31e77325ba279248c65fb4fcef4"
+                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
+                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.20.0"
+            "version": "==20.21.0"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
```

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/README.rst` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/README.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/USAGE.rst` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/USAGE.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/__init__.py` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/__init__.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/_version.py` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/_version.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/awsenergylabelerlib.py` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/awsenergylabelerlib.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/awsenergylabelerlibexceptions.py` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/awsenergylabelerlibexceptions.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/configuration.py` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/configuration.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/datamodels.py` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/datamodels.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/entities.py` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 # pylint: disable=too-many-lines
 
 import logging
 import tempfile
 from abc import ABC, abstractmethod
 from collections import Counter
 from copy import copy, deepcopy
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import datetime
 from pathlib import Path
 from urllib.parse import urlparse, urljoin
 
 import boto3
 import botocore.errorfactory
 import botocore.exceptions
@@ -379,26 +379,26 @@
         accounts = []
         for page in paginator.paginate():
             accounts.extend([AwsAccount(account.get('AccountId'), self.account_thresholds)
                              for account in page['Members']])
         return accounts
 
 
-@dataclass
+@dataclass(frozen=True)
 class AwsAccount:
     """Models the aws account that can label itself."""
 
     id: str  # pylint: disable=invalid-name
-    account_thresholds: list
+    account_thresholds: field(default_factory=list)
     name: str = 'NOT_RETRIEVED'
     energy_label: AccountEnergyLabel = AccountEnergyLabel()
     _alias: str = None
 
     def __post_init__(self):
-        self._logger = logging.getLogger(f'{LOGGER_BASENAME}.{self.__class__.__name__}')
+        super().__setattr__('_logger', logging.getLogger(f'{LOGGER_BASENAME}.{self.__class__.__name__}'))
 
     @property
     def alias(self):
         """Alias."""
         if self._alias is None:
             self._alias = ''
             try:
@@ -470,22 +470,22 @@
                                                        number_of_low_findings,
                                                        max_days_open)
         except Exception:  # pylint: disable=broad-except
             self._logger.warning(f'Could not calculate energy label for account {self.id}, using the default "F"')
         return self.energy_label
 
 
-@dataclass
+@dataclass(frozen=True)
 class Finding:
     """Models a finding."""
 
     _data: dict
 
     def __post_init__(self):
-        self._logger = logging.getLogger(f'{LOGGER_BASENAME}.{self.__class__.__name__}')
+        super().__setattr__('_logger', logging.getLogger(f'{LOGGER_BASENAME}.{self.__class__.__name__}'))
 
     def __hash__(self):
         return hash(self.id)
 
     def __eq__(self, other):
         """Override the default equals behavior."""
         if not isinstance(other, Finding):
```

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/labels.py` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/labels.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,26 +45,26 @@
 __status__ = '''Development'''  # "Prototype", "Development", "Production".
 
 LOGGER_BASENAME = '''labels'''
 LOGGER = logging.getLogger(LOGGER_BASENAME)
 LOGGER.addHandler(logging.NullHandler())
 
 
-@dataclass
+@dataclass(frozen=True)
 class ZoneEnergyLabel:
     """Models the zone energy label."""
 
     label: str
     best_label: str
     worst_label: str
     accounts_measured: int
     coverage: float
 
 
-@dataclass
+@dataclass(frozen=True)
 class AccountEnergyLabel:
     """Models the account energy label."""
 
     label: str = "F"
     number_of_critical_findings: int = 9999
     number_of_high_findings: int = 9999
     number_of_medium_findings: int = 9999
```

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/schemas.py` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/schemas.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib/validations.py` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib/validations.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib.egg-info/PKG-INFO` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsenergylabelerlib
-Version: 3.2.1
+Version: 3.2.2
 Summary: Project energy labeling accounts and landing zone based on findings of Security Hub in AWS cloud.
 Home-page: https://github.com/schubergphilis/awsenergylabelerlib.git
 Author: Costas Tyfoxylos
 Author-email: ctyfoxylos@schubergphilis.com
 License: MIT
 Keywords: awsenergylabelerlib energy labeling aws security hub landing zone
 Classifier: Development Status :: 4 - Beta
@@ -275,7 +275,13 @@
 * Bump dependencies.
 
 
 3.2.1 (10-03-2023)
 ------------------
 
 * Updated dependencies
+
+
+3.2.2 (11-04-2023)
+------------------
+
+* Convert Dataclasses to Frozen for compatibility with latest python.
```

### Comparing `awsenergylabelerlib-3.2.1/awsenergylabelerlib.egg-info/SOURCES.txt` & `awsenergylabelerlib-3.2.2/awsenergylabelerlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/docs/Makefile` & `awsenergylabelerlib-3.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/docs/conf.py` & `awsenergylabelerlib-3.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/docs/index.rst` & `awsenergylabelerlib-3.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/setup.py` & `awsenergylabelerlib-3.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/tests/test_awsenergylabelerlib.py` & `awsenergylabelerlib-3.2.2/tests/test_awsenergylabelerlib.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/tests/test_entities.py` & `awsenergylabelerlib-3.2.2/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.1/tests/test_validations.py` & `awsenergylabelerlib-3.2.2/tests/test_validations.py`

 * *Files identical despite different names*

