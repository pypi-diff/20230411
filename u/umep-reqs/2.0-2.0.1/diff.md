# Comparing `tmp/umep-reqs-2.0.tar.gz` & `tmp/umep-reqs-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umep-reqs-2.0.tar", last modified: Wed Apr  5 12:48:24 2023, max compression
+gzip compressed data, was "umep-reqs-2.0.1.tar", last modified: Tue Apr 11 08:38:41 2023, max compression
```

## Comparing `umep-reqs-2.0.tar` & `umep-reqs-2.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:24.944478 umep-reqs-2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-05 12:48:24.944478 umep-reqs-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-05 12:48:10.000000 umep-reqs-2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 12:48:24.944478 umep-reqs-2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:24.944478 umep-reqs-2.0/umep-reqs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:10.000000 umep-reqs-2.0/umep-reqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-05 12:48:10.000000 umep-reqs-2.0/umep-reqs/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:48:24.944478 umep-reqs-2.0/umep_reqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-05 12:48:24.000000 umep-reqs-2.0/umep_reqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-05 12:48:24.000000 umep-reqs-2.0/umep_reqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 12:48:24.000000 umep-reqs-2.0/umep_reqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-05 12:48:24.000000 umep-reqs-2.0/umep_reqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-05 12:48:24.000000 umep-reqs-2.0/umep_reqs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:41.429685 umep-reqs-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-11 08:38:41.429685 umep-reqs-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-11 08:38:26.000000 umep-reqs-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:38:41.429685 umep-reqs-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:41.429685 umep-reqs-2.0.1/umep-reqs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:26.000000 umep-reqs-2.0.1/umep-reqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-11 08:38:26.000000 umep-reqs-2.0.1/umep-reqs/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:41.429685 umep-reqs-2.0.1/umep_reqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-11 08:38:41.000000 umep-reqs-2.0.1/umep_reqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-11 08:38:41.000000 umep-reqs-2.0.1/umep_reqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:38:41.000000 umep-reqs-2.0.1/umep_reqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-11 08:38:41.000000 umep-reqs-2.0.1/umep_reqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 08:38:41.000000 umep-reqs-2.0.1/umep_reqs.egg-info/top_level.txt
```

### Comparing `umep-reqs-2.0/umep-reqs/setup.py` & `umep-reqs-2.0.1/umep-reqs/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,14 @@
     name="umep-reqs",
     version=get_version(),  # Use setuptools_scm to get version from git tags.
     packages=find_packages(),
     install_requires=[
         "supy==2022.9.22",  # Replace with actual dependency and version number.
         "numba==0.56.4",
         "jaydebeapi==1.2.3",
-        "netCDF4==1.6.1", #   "dependency2==y.y.y" 
+        "netCDF4", #   "dependency2==y.y.y" 
     ],
     author="UMEP dev team",
     long_description=long_description,
     long_description_content_type="text/markdown",
     
 )
```

