# Comparing `tmp/caddo-tool-0.8.1.tar.gz` & `tmp/caddo-tool-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caddo-tool-0.8.1.tar", last modified: Mon Apr  3 14:58:44 2023, max compression
+gzip compressed data, was "caddo-tool-0.9.1.tar", last modified: Mon Apr  3 15:18:21 2023, max compression
```

## Comparing `caddo-tool-0.8.1.tar` & `caddo-tool-0.9.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:58:44.766104 caddo-tool-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-03 14:58:29.000000 caddo-tool-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-03 14:58:44.766104 caddo-tool-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-03 14:58:29.000000 caddo-tool-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:58:44.766104 caddo-tool-0.8.1/caddo_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-03 14:58:44.000000 caddo-tool-0.8.1/caddo_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-03 14:58:44.000000 caddo-tool-0.8.1/caddo_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 14:58:44.000000 caddo-tool-0.8.1/caddo_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-03 14:58:44.000000 caddo-tool-0.8.1/caddo_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-03 14:58:44.000000 caddo-tool-0.8.1/caddo_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-03 14:58:29.000000 caddo-tool-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 14:58:44.766104 caddo-tool-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:18:21.560541 caddo-tool-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-03 15:18:10.000000 caddo-tool-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-03 15:18:21.560541 caddo-tool-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-03 15:18:10.000000 caddo-tool-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:18:21.560541 caddo-tool-0.9.1/caddo_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-03 15:18:21.000000 caddo-tool-0.9.1/caddo_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-03 15:18:21.000000 caddo-tool-0.9.1/caddo_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 15:18:21.000000 caddo-tool-0.9.1/caddo_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-03 15:18:21.000000 caddo-tool-0.9.1/caddo_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-03 15:18:21.000000 caddo-tool-0.9.1/caddo_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-03 15:18:10.000000 caddo-tool-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 15:18:21.560541 caddo-tool-0.9.1/setup.cfg
```

### Comparing `caddo-tool-0.8.1/LICENSE` & `caddo-tool-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caddo-tool-0.8.1/PKG-INFO` & `caddo-tool-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caddo-tool
-Version: 0.8.1
+Version: 0.9.1
 Summary: Benchmark Tool for CaddoBenchmark Project
 Author-email: Piotr Tylczyński <piotr@ptl.cloud>, Katarzyna Kulesa <katarzyna.kulesa@kasiait.pl>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `caddo-tool-0.8.1/caddo_tool.egg-info/PKG-INFO` & `caddo-tool-0.9.1/caddo_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caddo-tool
-Version: 0.8.1
+Version: 0.9.1
 Summary: Benchmark Tool for CaddoBenchmark Project
 Author-email: Piotr Tylczyński <piotr@ptl.cloud>, Katarzyna Kulesa <katarzyna.kulesa@kasiait.pl>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `caddo-tool-0.8.1/pyproject.toml` & `caddo-tool-0.9.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caddo-tool"
-version = "0.8.1"
+version = "0.9.1"
 authors = [
     { name = "Piotr Tylczyński", email = "piotr@ptl.cloud" },
     { name = "Katarzyna Kulesa", email = "katarzyna.kulesa@kasiait.pl" },
 ]
 description = "Benchmark Tool for CaddoBenchmark Project"
 readme = "README.md"
 requires-python = ">=3.7"
```

