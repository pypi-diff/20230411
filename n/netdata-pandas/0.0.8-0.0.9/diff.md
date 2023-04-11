# Comparing `tmp/netdata_pandas-0.0.8.tar.gz` & `tmp/netdata_pandas-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/netdata_pandas-0.0.8.tar", last modified: Mon Jun 15 21:34:21 2020, max compression
+gzip compressed data, was "dist/netdata_pandas-0.0.9.tar", last modified: Mon Jun 15 21:50:19 2020, max compression
```

## Comparing `netdata_pandas-0.0.8.tar` & `netdata_pandas-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2020-06-15 21:34:21.503631 netdata_pandas-0.0.8/
--rw-r--r--   0 andre     (1000) andre     (1000)     2348 2020-06-15 19:20:38.000000 netdata_pandas-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 andre     (1000) andre     (1000)    11357 2020-06-15 19:20:38.000000 netdata_pandas-0.0.8/LICENSE
--rw-r--r--   0 andre     (1000) andre     (1000)      111 2020-06-15 19:20:38.000000 netdata_pandas-0.0.8/MANIFEST.in
--rw-r--r--   0 andre     (1000) andre     (1000)     1305 2020-06-15 21:34:21.501532 netdata_pandas-0.0.8/PKG-INFO
--rw-r--r--   0 andre     (1000) andre     (1000)      345 2020-06-15 21:33:46.000000 netdata_pandas-0.0.8/README.md
-drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2020-06-15 21:34:21.476580 netdata_pandas-0.0.8/netdata_pandas/
--rw-r--r--   0 andre     (1000) andre     (1000)       22 2020-06-15 21:33:36.000000 netdata_pandas-0.0.8/netdata_pandas/__init__.py
--rw-r--r--   0 andre     (1000) andre     (1000)      469 2020-06-15 21:33:36.000000 netdata_pandas-0.0.8/netdata_pandas/_nbdev.py
--rw-r--r--   0 andre     (1000) andre     (1000)     1580 2020-06-15 21:33:36.000000 netdata_pandas-0.0.8/netdata_pandas/data.py
--rw-r--r--   0 andre     (1000) andre     (1000)      176 2020-06-15 21:33:36.000000 netdata_pandas-0.0.8/netdata_pandas/utils.py
-drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2020-06-15 21:34:21.499315 netdata_pandas-0.0.8/netdata_pandas.egg-info/
--rw-r--r--   0 andre     (1000) andre     (1000)     1305 2020-06-15 21:34:21.000000 netdata_pandas-0.0.8/netdata_pandas.egg-info/PKG-INFO
--rw-r--r--   0 andre     (1000) andre     (1000)      433 2020-06-15 21:34:21.000000 netdata_pandas-0.0.8/netdata_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 andre     (1000) andre     (1000)        1 2020-06-15 21:34:21.000000 netdata_pandas-0.0.8/netdata_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 andre     (1000) andre     (1000)       20 2020-06-15 21:34:21.000000 netdata_pandas-0.0.8/netdata_pandas.egg-info/entry_points.txt
--rw-r--r--   0 andre     (1000) andre     (1000)        1 2020-06-15 19:54:45.000000 netdata_pandas-0.0.8/netdata_pandas.egg-info/not-zip-safe
--rw-r--r--   0 andre     (1000) andre     (1000)       39 2020-06-15 21:34:21.000000 netdata_pandas-0.0.8/netdata_pandas.egg-info/requires.txt
--rw-r--r--   0 andre     (1000) andre     (1000)       15 2020-06-15 21:34:21.000000 netdata_pandas-0.0.8/netdata_pandas.egg-info/top_level.txt
--rw-r--r--   0 andre     (1000) andre     (1000)      728 2020-06-15 21:31:30.000000 netdata_pandas-0.0.8/settings.ini
--rw-r--r--   0 andre     (1000) andre     (1000)       38 2020-06-15 21:34:21.503631 netdata_pandas-0.0.8/setup.cfg
--rw-r--r--   0 andre     (1000) andre     (1000)     1921 2020-06-15 19:20:38.000000 netdata_pandas-0.0.8/setup.py
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2020-06-15 21:50:19.858507 netdata_pandas-0.0.9/
+-rw-r--r--   0 andre     (1000) andre     (1000)     2348 2020-06-15 19:20:38.000000 netdata_pandas-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 andre     (1000) andre     (1000)    11357 2020-06-15 19:20:38.000000 netdata_pandas-0.0.9/LICENSE
+-rw-r--r--   0 andre     (1000) andre     (1000)      111 2020-06-15 19:20:38.000000 netdata_pandas-0.0.9/MANIFEST.in
+-rw-r--r--   0 andre     (1000) andre     (1000)     5112 2020-06-15 21:50:19.857014 netdata_pandas-0.0.9/PKG-INFO
+-rw-r--r--   0 andre     (1000) andre     (1000)     3088 2020-06-15 21:49:47.000000 netdata_pandas-0.0.9/README.md
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2020-06-15 21:50:19.829440 netdata_pandas-0.0.9/netdata_pandas/
+-rw-r--r--   0 andre     (1000) andre     (1000)       22 2020-06-15 21:49:40.000000 netdata_pandas-0.0.9/netdata_pandas/__init__.py
+-rw-r--r--   0 andre     (1000) andre     (1000)      469 2020-06-15 21:49:40.000000 netdata_pandas-0.0.9/netdata_pandas/_nbdev.py
+-rw-r--r--   0 andre     (1000) andre     (1000)     1580 2020-06-15 21:49:40.000000 netdata_pandas-0.0.9/netdata_pandas/data.py
+-rw-r--r--   0 andre     (1000) andre     (1000)      176 2020-06-15 21:49:40.000000 netdata_pandas-0.0.9/netdata_pandas/utils.py
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2020-06-15 21:50:19.852682 netdata_pandas-0.0.9/netdata_pandas.egg-info/
+-rw-r--r--   0 andre     (1000) andre     (1000)     5112 2020-06-15 21:50:19.000000 netdata_pandas-0.0.9/netdata_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 andre     (1000) andre     (1000)      433 2020-06-15 21:50:19.000000 netdata_pandas-0.0.9/netdata_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 andre     (1000) andre     (1000)        1 2020-06-15 21:50:19.000000 netdata_pandas-0.0.9/netdata_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 andre     (1000) andre     (1000)       20 2020-06-15 21:50:19.000000 netdata_pandas-0.0.9/netdata_pandas.egg-info/entry_points.txt
+-rw-r--r--   0 andre     (1000) andre     (1000)        1 2020-06-15 19:54:45.000000 netdata_pandas-0.0.9/netdata_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 andre     (1000) andre     (1000)       39 2020-06-15 21:50:19.000000 netdata_pandas-0.0.9/netdata_pandas.egg-info/requires.txt
+-rw-r--r--   0 andre     (1000) andre     (1000)       15 2020-06-15 21:50:19.000000 netdata_pandas-0.0.9/netdata_pandas.egg-info/top_level.txt
+-rw-r--r--   0 andre     (1000) andre     (1000)      728 2020-06-15 21:34:26.000000 netdata_pandas-0.0.9/settings.ini
+-rw-r--r--   0 andre     (1000) andre     (1000)       38 2020-06-15 21:50:19.858507 netdata_pandas-0.0.9/setup.cfg
+-rw-r--r--   0 andre     (1000) andre     (1000)     1921 2020-06-15 19:20:38.000000 netdata_pandas-0.0.9/setup.py
```

### Comparing `netdata_pandas-0.0.8/CONTRIBUTING.md` & `netdata_pandas-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `netdata_pandas-0.0.8/LICENSE` & `netdata_pandas-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netdata_pandas-0.0.8/netdata_pandas/data.py` & `netdata_pandas-0.0.9/netdata_pandas/data.py`

 * *Files identical despite different names*

### Comparing `netdata_pandas-0.0.8/settings.ini` & `netdata_pandas-0.0.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 user = netdata
 description = A helper library for pulling data from netdata into a pandas dataframe.
 keywords = netdata pandas
 author = Andrew Maguire
 author_email = andrewmaguire@netdata.cloud
 copyright = Netdata Cloud
 branch = master
-version = 0.0.8
+version = 0.0.9
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 2
 requirements = pandas==1.0.4 asks==2.3.7 trio==0.16.0
```

### Comparing `netdata_pandas-0.0.8/setup.py` & `netdata_pandas-0.0.9/setup.py`

 * *Files identical despite different names*

