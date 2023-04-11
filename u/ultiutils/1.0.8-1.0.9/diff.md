# Comparing `tmp/ultiutils-1.0.8.tar.gz` & `tmp/ultiutils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultiutils-1.0.8.tar", last modified: Thu Mar 30 06:44:31 2023, max compression
+gzip compressed data, was "ultiutils-1.0.9.tar", last modified: Tue Apr 11 21:20:43 2023, max compression
```

## Comparing `ultiutils-1.0.8.tar` & `ultiutils-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-30 06:44:31.948583 ultiutils-1.0.8/
--rw-r--r--   0 runner    (1000) runner    (1000)      485 2023-03-30 06:44:31.948583 ultiutils-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2021-07-22 16:01:49.000000 ultiutils-1.0.8/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      306 2021-07-24 20:39:36.000000 ultiutils-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-03-30 06:44:31.948583 ultiutils-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1591 2021-07-24 20:08:38.000000 ultiutils-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-30 06:44:31.948583 ultiutils-1.0.8/ultiutils/
--rw-r--r--   0 runner    (1000) runner    (1000)      507 2021-07-24 20:39:17.000000 ultiutils-1.0.8/ultiutils/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3710 2021-07-23 01:39:59.000000 ultiutils-1.0.8/ultiutils/ultimain.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-30 06:44:31.948583 ultiutils-1.0.8/ultiutils.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      485 2023-03-30 06:44:31.000000 ultiutils-1.0.8/ultiutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      241 2023-03-30 06:44:31.000000 ultiutils-1.0.8/ultiutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-03-30 06:44:31.000000 ultiutils-1.0.8/ultiutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-03-30 06:44:31.000000 ultiutils-1.0.8/ultiutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-03-30 06:44:31.000000 ultiutils-1.0.8/ultiutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-11 21:20:43.734944 ultiutils-1.0.9/
+-rw-r--r--   0 runner    (1000) runner    (1000)      485 2023-04-11 21:20:43.734944 ultiutils-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2021-07-22 16:01:49.000000 ultiutils-1.0.9/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      306 2021-07-24 20:39:36.000000 ultiutils-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-11 21:20:43.734944 ultiutils-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1591 2021-07-24 20:08:38.000000 ultiutils-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-11 21:20:43.734944 ultiutils-1.0.9/ultiutils/
+-rw-r--r--   0 runner    (1000) runner    (1000)      507 2021-07-24 20:39:17.000000 ultiutils-1.0.9/ultiutils/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3710 2021-07-23 01:39:59.000000 ultiutils-1.0.9/ultiutils/ultimain.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-11 21:20:43.734944 ultiutils-1.0.9/ultiutils.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      485 2023-04-11 21:20:43.000000 ultiutils-1.0.9/ultiutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      241 2023-04-11 21:20:43.000000 ultiutils-1.0.9/ultiutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-11 21:20:43.000000 ultiutils-1.0.9/ultiutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-04-11 21:20:43.000000 ultiutils-1.0.9/ultiutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-04-11 21:20:43.000000 ultiutils-1.0.9/ultiutils.egg-info/top_level.txt
```

### Comparing `ultiutils-1.0.8/setup.py` & `ultiutils-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `ultiutils-1.0.8/ultiutils/ultimain.py` & `ultiutils-1.0.9/ultiutils/ultimain.py`

 * *Files identical despite different names*

