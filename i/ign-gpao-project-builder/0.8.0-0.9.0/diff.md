# Comparing `tmp/ign-gpao-project-builder-0.8.0.tar.gz` & `tmp/ign-gpao-project-builder-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ign-gpao-project-builder-0.8.0.tar", last modified: Mon Dec 12 13:33:27 2022, max compression
+gzip compressed data, was "ign-gpao-project-builder-0.9.0.tar", last modified: Fri Jan  6 13:15:35 2023, max compression
```

## Comparing `ign-gpao-project-builder-0.8.0.tar` & `ign-gpao-project-builder-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:33:27.402914 ign-gpao-project-builder-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2022-12-12 13:33:27.402914 ign-gpao-project-builder-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2022-12-12 13:33:10.000000 ign-gpao-project-builder-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:33:27.402914 ign-gpao-project-builder-0.8.0/gpao/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-12 13:33:13.000000 ign-gpao-project-builder-0.8.0/gpao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2022-12-12 13:33:10.000000 ign-gpao-project-builder-0.8.0/gpao/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2022-12-12 13:33:10.000000 ign-gpao-project-builder-0.8.0/gpao/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2022-12-12 13:33:10.000000 ign-gpao-project-builder-0.8.0/gpao/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:33:27.402914 ign-gpao-project-builder-0.8.0/ign_gpao_project_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2022-12-12 13:33:27.000000 ign-gpao-project-builder-0.8.0/ign_gpao_project_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2022-12-12 13:33:27.000000 ign-gpao-project-builder-0.8.0/ign_gpao_project_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 13:33:27.000000 ign-gpao-project-builder-0.8.0/ign_gpao_project_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-12 13:33:27.000000 ign-gpao-project-builder-0.8.0/ign_gpao_project_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-12 13:33:27.000000 ign-gpao-project-builder-0.8.0/ign_gpao_project_builder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 13:33:27.402914 ign-gpao-project-builder-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      796 2022-12-12 13:33:10.000000 ign-gpao-project-builder-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 13:15:35.768620 ign-gpao-project-builder-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-01-06 13:15:35.768620 ign-gpao-project-builder-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-01-06 13:15:22.000000 ign-gpao-project-builder-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 13:15:35.768620 ign-gpao-project-builder-0.9.0/gpao/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-06 13:15:24.000000 ign-gpao-project-builder-0.9.0/gpao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-01-06 13:15:22.000000 ign-gpao-project-builder-0.9.0/gpao/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-01-06 13:15:22.000000 ign-gpao-project-builder-0.9.0/gpao/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-01-06 13:15:22.000000 ign-gpao-project-builder-0.9.0/gpao/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 13:15:35.768620 ign-gpao-project-builder-0.9.0/ign_gpao_project_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-01-06 13:15:35.000000 ign-gpao-project-builder-0.9.0/ign_gpao_project_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-01-06 13:15:35.000000 ign-gpao-project-builder-0.9.0/ign_gpao_project_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 13:15:35.000000 ign-gpao-project-builder-0.9.0/ign_gpao_project_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-06 13:15:35.000000 ign-gpao-project-builder-0.9.0/ign_gpao_project_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-06 13:15:35.000000 ign-gpao-project-builder-0.9.0/ign_gpao_project_builder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 13:15:35.768620 ign-gpao-project-builder-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-01-06 13:15:22.000000 ign-gpao-project-builder-0.9.0/setup.py
```

### Comparing `ign-gpao-project-builder-0.8.0/PKG-INFO` & `ign-gpao-project-builder-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ign-gpao-project-builder
-Version: 0.8.0
+Version: 0.9.0
 Summary: Write a json's GPAO file
 Home-page: https://github.com/ign-gpao/builder-python.git
 Author: Arnaud Birk
 Author-email: arnaud.birk@ign.fr
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ign-gpao-project-builder-0.8.0/README.md` & `ign-gpao-project-builder-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ign-gpao-project-builder-0.8.0/gpao/builder.py` & `ign-gpao-project-builder-0.9.0/gpao/builder.py`

 * *Files identical despite different names*

### Comparing `ign-gpao-project-builder-0.8.0/gpao/job.py` & `ign-gpao-project-builder-0.9.0/gpao/job.py`

 * *Files identical despite different names*

### Comparing `ign-gpao-project-builder-0.8.0/gpao/project.py` & `ign-gpao-project-builder-0.9.0/gpao/project.py`

 * *Files identical despite different names*

### Comparing `ign-gpao-project-builder-0.8.0/ign_gpao_project_builder.egg-info/PKG-INFO` & `ign-gpao-project-builder-0.9.0/ign_gpao_project_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ign-gpao-project-builder
-Version: 0.8.0
+Version: 0.9.0
 Summary: Write a json's GPAO file
 Home-page: https://github.com/ign-gpao/builder-python.git
 Author: Arnaud Birk
 Author-email: arnaud.birk@ign.fr
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ign-gpao-project-builder-0.8.0/setup.py` & `ign-gpao-project-builder-0.9.0/setup.py`

 * *Files identical despite different names*

