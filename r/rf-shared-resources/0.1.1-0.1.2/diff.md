# Comparing `tmp/rf-shared-resources-0.1.1.tar.gz` & `tmp/rf-shared-resources-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rf-shared-resources/rf-shared-resources/dist/tmp8m9_kcec/rf-shared-resources-0.1.1.tar", last modified: Mon Jan 17 22:25:32 2022, max compression
+gzip compressed data, was "/home/runner/work/rf-shared-resources/rf-shared-resources/dist/.tmp-l0_19ivq/rf-shared-resources-0.1.2.tar", last modified: Tue Apr 11 17:02:05 2023, max compression
```

## Comparing `rf-shared-resources-0.1.1.tar` & `rf-shared-resources-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 22:25:32.000000 rf-shared-resources-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-01-17 22:25:23.000000 rf-shared-resources-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2848 2022-01-17 22:25:32.000000 rf-shared-resources-0.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     2360 2022-01-17 22:25:23.000000 rf-shared-resources-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 22:25:32.000000 rf-shared-resources-0.1.1/SharedResources/
--rwxr-xr-x   0 runner    (1001) docker     (121)      101 2022-01-17 22:25:23.000000 rf-shared-resources-0.1.1/SharedResources/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3318 2022-01-17 22:25:23.000000 rf-shared-resources-0.1.1/SharedResources/_shared_resources.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       22 2022-01-17 22:25:23.000000 rf-shared-resources-0.1.1/SharedResources/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 22:25:32.000000 rf-shared-resources-0.1.1/rf_shared_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2848 2022-01-17 22:25:32.000000 rf-shared-resources-0.1.1/rf_shared_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-01-17 22:25:32.000000 rf-shared-resources-0.1.1/rf_shared_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-17 22:25:32.000000 rf-shared-resources-0.1.1/rf_shared_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-01-17 22:25:32.000000 rf-shared-resources-0.1.1/rf_shared_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-01-17 22:25:32.000000 rf-shared-resources-0.1.1/rf_shared_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-17 22:25:32.000000 rf-shared-resources-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1046 2022-01-17 22:25:23.000000 rf-shared-resources-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:02:05.000000 rf-shared-resources-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 17:01:53.000000 rf-shared-resources-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-11 17:02:05.000000 rf-shared-resources-0.1.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2360 2023-04-11 17:01:53.000000 rf-shared-resources-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:02:05.000000 rf-shared-resources-0.1.2/SharedResources/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-04-11 17:01:53.000000 rf-shared-resources-0.1.2/SharedResources/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3337 2023-04-11 17:01:53.000000 rf-shared-resources-0.1.2/SharedResources/_shared_resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-04-11 17:01:53.000000 rf-shared-resources-0.1.2/SharedResources/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:02:05.000000 rf-shared-resources-0.1.2/rf_shared_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-11 17:02:05.000000 rf-shared-resources-0.1.2/rf_shared_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-11 17:02:05.000000 rf-shared-resources-0.1.2/rf_shared_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:02:05.000000 rf-shared-resources-0.1.2/rf_shared_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-11 17:02:05.000000 rf-shared-resources-0.1.2/rf_shared_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 17:02:05.000000 rf-shared-resources-0.1.2/rf_shared_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:02:05.000000 rf-shared-resources-0.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1046 2023-04-11 17:01:53.000000 rf-shared-resources-0.1.2/setup.py
```

### Comparing `rf-shared-resources-0.1.1/LICENSE` & `rf-shared-resources-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rf-shared-resources-0.1.1/PKG-INFO` & `rf-shared-resources-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: rf-shared-resources
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utility to share Robot Framework resource files in Python packages.
 Home-page: https://github.com/kangasta/rf-shared-resources
 Author: Toni Kangas
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -100,9 +98,7 @@
 ```
 
 Generate documentation with:
 
 ```bash
 python3 -m robot.libdoc SharedResources docs/index.html
 ```
-
-
```

### Comparing `rf-shared-resources-0.1.1/README.md` & `rf-shared-resources-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rf-shared-resources-0.1.1/SharedResources/_shared_resources.py` & `rf-shared-resources-0.1.2/SharedResources/_shared_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     resources_: Iterable[resources.Resource]
 ):
     built_in = BuiltIn()
 
     for resource in resources_:
         with resources.path(package, resource) as path:
             debug(f'Importing resource file from {path}')
-            built_in.import_resource(str(path))
+            built_in.import_resource(str(path).replace("\\", "/"))
 
 
 def _parse_args_and_load_resource_file(args):
     if len(args) < 2:
         raise ValueError(
             'Not enough arguments. Expected package name as first argument and resource names as following arguments.')
     load_resource_file(args[0], args[1:])
```

### Comparing `rf-shared-resources-0.1.1/rf_shared_resources.egg-info/PKG-INFO` & `rf-shared-resources-0.1.2/rf_shared_resources.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: rf-shared-resources
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utility to share Robot Framework resource files in Python packages.
 Home-page: https://github.com/kangasta/rf-shared-resources
 Author: Toni Kangas
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -100,9 +98,7 @@
 ```
 
 Generate documentation with:
 
 ```bash
 python3 -m robot.libdoc SharedResources docs/index.html
 ```
-
-
```

### Comparing `rf-shared-resources-0.1.1/setup.py` & `rf-shared-resources-0.1.2/setup.py`

 * *Files identical despite different names*

