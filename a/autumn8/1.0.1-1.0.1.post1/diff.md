# Comparing `tmp/autumn8-1.0.1.tar.gz` & `tmp/autumn8-1.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.1.tar", last modified: Tue Apr 11 13:33:07 2023, max compression
+gzip compressed data, was "autumn8-1.0.1.post1.tar", last modified: Tue Apr 11 14:32:35 2023, max compression
```

## Comparing `autumn8-1.0.1.tar` & `autumn8-1.0.1.post1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.492624 autumn8-1.0.1/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2378 2023-04-11 13:33:07.492624 autumn8-1.0.1/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2161 2023-03-10 14:58:37.000000 autumn8-1.0.1/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.442623 autumn8-1.0.1/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.462623 autumn8-1.0.1/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7857 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.462623 autumn8-1.0.1/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3190 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    14901 2023-04-11 13:30:43.000000 autumn8-1.0.1/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1453 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2992 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4953 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3126 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/cli/pending_uploads.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.462623 autumn8-1.0.1/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      103 2023-04-11 13:28:16.000000 autumn8-1.0.1/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.472623 autumn8-1.0.1/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6503 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3200 2023-04-11 12:40:47.000000 autumn8-1.0.1/autumn8/common/config/s3.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    63841 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      366 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.482623 autumn8-1.0.1/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/examples/tensorflow_custom_layers.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.482623 autumn8-1.0.1/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.492624 autumn8-1.0.1/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2657 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    10168 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1149 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.1/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4512 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.452623 autumn8-1.0.1/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2378 2023-04-11 13:33:07.000000 autumn8-1.0.1/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1262 2023-04-11 13:33:07.000000 autumn8-1.0.1/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-04-11 13:33:07.000000 autumn8-1.0.1/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-04-11 13:33:07.000000 autumn8-1.0.1/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      126 2023-04-11 13:33:07.000000 autumn8-1.0.1/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-04-11 13:33:07.000000 autumn8-1.0.1/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1933 2023-03-31 14:44:39.000000 autumn8-1.0.1/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-04-11 13:33:07.492624 autumn8-1.0.1/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.1/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.492624 autumn8-1.0.1/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.1/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.1/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.354785 autumn8-1.0.1.post1/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2384 2023-04-11 14:32:35.354785 autumn8-1.0.1.post1/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2161 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.304785 autumn8-1.0.1.post1/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.314785 autumn8-1.0.1.post1/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7850 2023-04-11 13:47:09.000000 autumn8-1.0.1.post1/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.324785 autumn8-1.0.1.post1/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3190 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    15401 2023-04-11 13:56:38.000000 autumn8-1.0.1.post1/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1453 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3227 2023-04-11 14:28:57.000000 autumn8-1.0.1.post1/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4953 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3126 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/cli/pending_uploads.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.324785 autumn8-1.0.1.post1/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      109 2023-04-11 14:31:49.000000 autumn8-1.0.1.post1/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.324785 autumn8-1.0.1.post1/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6503 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3200 2023-04-11 12:40:47.000000 autumn8-1.0.1.post1/autumn8/common/config/s3.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    63841 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      366 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.334785 autumn8-1.0.1.post1/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/examples/tensorflow_custom_layers.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.344785 autumn8-1.0.1.post1/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.354785 autumn8-1.0.1.post1/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2657 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    10255 2023-04-11 14:30:25.000000 autumn8-1.0.1.post1/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1149 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.1.post1/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4578 2023-04-11 14:30:05.000000 autumn8-1.0.1.post1/autumn8/lib/service.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.304785 autumn8-1.0.1.post1/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2384 2023-04-11 14:32:35.000000 autumn8-1.0.1.post1/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1262 2023-04-11 14:32:35.000000 autumn8-1.0.1.post1/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-04-11 14:32:35.000000 autumn8-1.0.1.post1/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-04-11 14:32:35.000000 autumn8-1.0.1.post1/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      126 2023-04-11 14:32:35.000000 autumn8-1.0.1.post1/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-04-11 14:32:35.000000 autumn8-1.0.1.post1/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1933 2023-03-31 14:44:39.000000 autumn8-1.0.1.post1/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-04-11 14:32:35.354785 autumn8-1.0.1.post1/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.354785 autumn8-1.0.1.post1/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/tests/test_settings.py
```

### Comparing `autumn8-1.0.1/PKG-INFO` & `autumn8-1.0.1.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.1
+Version: 1.0.1.post1
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.1/README.md` & `autumn8-1.0.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/cli/analyze.py` & `autumn8-1.0.1.post1/autumn8/cli/analyze.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,41 +154,39 @@
     return Path(model_file_path).stem
 
 
 def filepath_is_a_link(filepath: str) -> bool:
     return filepath.startswith("http://") or filepath.startswith("https://")
 
 
-def analyze_model_file(model_file_path: str, model_script_args=[]):
-    extension = Path(model_file_path).suffixes[-1]
+def analyze_model_file(model_filepath_or_url: str, model_script_args=[]):
+    extension = Path(model_filepath_or_url).suffixes[-1]
     is_source_annotated_model = False
 
     (
-        model_file,
         inferred_model_name,
         framework,
         inferred_quantization,
-    ) = (None, None, None, None)
+    ) = (None, None, None)
     _inferred_batch_size = None
     inferred_input_dims = []
 
-    model_file = model_file_path
-    inferred_model_name = suggest_model_name(model_file_path)
+    inferred_model_name = suggest_model_name(model_filepath_or_url)
     inferred_quantization = "FP32"
 
     if extension in [".py"]:
-        if filepath_is_a_link(model_file_path):
+        if filepath_is_a_link(model_filepath_or_url):
             raise ClickException(
                 "Hosted .py files are not supported yet - please download the script and run the CLI on it"
             )
         is_source_annotated_model = True
         dummy_input, model_file_name, framework = pack_annotated_script_model(
-            model_file_path, model_script_args, inferred_model_name
+            model_filepath_or_url, model_script_args, inferred_model_name
         )
-        model_file = model_file_name
+        model_filepath_or_url = model_file_name
 
         if hasattr(dummy_input, "shape"):
             [
                 _inferred_batch_size,
                 *inferred_input_dims,
             ] = dummy_input.shape
         else:
@@ -218,14 +216,14 @@
 
     else:
         raise ClickException(
             f"Files with '{extension}' are not supported - please contact us at support@autumn8.ai to add the support."
         )
 
     return (
-        model_file,
+        model_filepath_or_url,
         inferred_model_name,
         framework,
         inferred_quantization,
         inferred_input_dims,
         is_source_annotated_model,
     )
```

### Comparing `autumn8-1.0.1/autumn8/cli/cli_environment.py` & `autumn8-1.0.1.post1/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/cli/commands/cloud.py` & `autumn8-1.0.1.post1/autumn8/cli/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/cli/commands/models.py` & `autumn8-1.0.1.post1/autumn8/cli/commands/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -284,28 +284,28 @@
 
     return func
 
 
 @model_commands_group.command()
 @options.use_environment
 @click.argument(
-    "model_file_path",
+    "model_filepath_or_url",
     type=str,
     # help="File path or HTTP URL to the model file or script",
 )
 @click.argument(
     "model_script_args",
     type=str,
     nargs=-1,
     # help="Arguments to pass to the model file during load",
 )
 @common_upload_args
 def submit_model(
-    organization_id,
-    model_file_path: str,
+    organization_id: int,
+    model_filepath_or_url: str,
     model_script_args: str,
     model_name: str,
     auto_confirm: bool,
     quiet: bool,
     should_skip_inputs: bool,
     quantization,
     input_dims: Optional[str],
@@ -316,21 +316,21 @@
 ):
     """Submit a model to AutoDL."""
 
     # Priority: flags, then configCache, then inference, then interactive user input
     environment = kwargs["environment"]
 
     (
-        model_file,
+        model_filepath_or_url,
         inferred_model_name,
         framework,
         inferred_quantization,
         inferred_input_dims,
         is_source_annotated_model,
-    ) = analyze_model_file(model_file_path, model_script_args)
+    ) = analyze_model_file(model_filepath_or_url, model_script_args)
 
     (
         model_name,
         quantization,
         input_dims,
         input_file,
     ) = prompt_for_missing_model_info(
@@ -361,15 +361,15 @@
             default=True,
         )
 
     model_upload_response = autodl.upload_model(
         environment,
         organization_id,
         model_config,
-        model_file,
+        model_filepath_or_url=model_filepath_or_url,
         input_file_path=input_file,
         max_upload_workers=max_upload_workers,
     )
 
     announce_model_upload_response(model_upload_response)
 
 
@@ -378,30 +378,30 @@
 
 
 supported_models_by_human_readable_label = {"GPT-J 6B": SupportedModel.GPTJ}
 
 
 @model_commands_group.command()
 @options.use_environment
-@click.argument("checkpoint_file_path")
+@click.argument("checkpoint_filepath_or_url")
 @common_upload_args
 @click.option(
     "-m",
     "--model_type",
     "--model",
     type=click.Choice(
         list(SupportedModel),
         case_sensitive=False,
     ),
     default=None,
     help="One of the supported models for the checkpoint",
 )
 def submit_checkpoint(
     organization_id: int,
-    checkpoint_file_path: str,
+    checkpoint_filepath_or_url: str,
     model_type: Optional[SupportedModel],
     model_name: str,
     auto_confirm: bool,
     quantization,
     should_skip_inputs: bool,
     input_dims,
     input_file,
@@ -421,16 +421,15 @@
         model_type = supported_models_by_human_readable_label[
             model_type_user_choice
         ]
 
     framework = "PYTORCH"
     inferred_quantization = None  # nice to have TODO: detect quantization
     inferred_input_dims = None
-    inferred_model_name = suggest_model_name(checkpoint_file_path)
-    model_filepath = checkpoint_file_path
+    inferred_model_name = suggest_model_name(checkpoint_filepath_or_url)
 
     (
         model_name,
         quantization,
         input_dims,
         input_file,
     ) = prompt_for_missing_model_info(
@@ -457,50 +456,63 @@
         click.echo(f"{json.dumps(model_config, indent=4)}")
         click.confirm(
             text="\n" + "Do you want to upload it to AutoDL?",
             abort=True,
             default=True,
         )
 
-    model_filepath = os.path.abspath(model_filepath)
-
-    if os.path.isdir(model_filepath):
+    if os.path.isdir(os.path.abspath(checkpoint_filepath_or_url)):
         # TODO: add zip progress bar
         time_start = time.time()
         logger.info("Zipping the model checkpoint folder, please wait...")
-        zipped_model_file = zipfile.ZipFile(
-            os.path.join(".", model_name + ".zip"),
-            "w",
-            compresslevel=0,
+        checkpoint_filepath_or_url = zip_checkpoint_dir(
+            os.path.abspath(checkpoint_filepath_or_url), model_name
         )
-        # write all files in the folder to the zip file
-        for root, _, files in os.walk(model_filepath):
-            for file in files:
-                zipped_model_file.write(
-                    os.path.join(root, file),
-                    arcname=os.path.join(file),
-                )
+        checkpoint_filepath_or_url = os.path.abspath(checkpoint_filepath_or_url)
 
-        model_filepath = zipped_model_file.filename
         logger.info("Zipping finished in %s seconds", time.time() - time_start)
-        logger.info("Zipped model file path: %s", model_filepath)
-        zipped_model_file.close()
+        logger.info("Zipped model file path: %s", checkpoint_filepath_or_url)
 
     logger.info("Starting the model upload")
     logger.warning(
         "If the upload isn't utilizing the whole network bandwidth, "
         + "please drop the upload and try again with "
         + "the --max_upload_workers flag set to a higher value "
         + "(currently =%s).",
         max_upload_workers,
     )
     model_upload_response = autodl.upload_model(
         environment,
         organization_id,
         model_config,
-        model_filepath,
+        model_filepath_or_url=checkpoint_filepath_or_url,
         input_file_path=input_file,
         model_type=model_type,
         max_upload_workers=max_upload_workers,
     )
 
     announce_model_upload_response(model_upload_response)
+
+
+def zip_checkpoint_dir(checkpoint_filepath_or_url: str, model_name: str) -> str:
+    zipped_model_file = zipfile.ZipFile(
+        os.path.join(".", model_name + ".zip"),
+        "w",
+        compresslevel=0,
+    )
+
+    # write all files in the folder to the zip file
+    for root, _, files in os.walk(checkpoint_filepath_or_url):
+        for file in files:
+            zipped_model_file.write(
+                os.path.join(root, file),
+                arcname=os.path.join(file),
+            )
+
+    zipped_model_file.close()
+
+    if zipped_model_file.filename is None:
+        raise RuntimeError(
+            "Failed to zip the checkpoint, please contact support@autumn8.ai if you encounter this error"
+        )
+
+    return zipped_model_file.filename
```

### Comparing `autumn8-1.0.1/autumn8/cli/examples.py` & `autumn8-1.0.1.post1/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/cli/interactive.py` & `autumn8-1.0.1.post1/autumn8/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/cli/main.py` & `autumn8-1.0.1.post1/autumn8/cli/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,15 +35,23 @@
     pending_uploads.forget_all_pending_uploads()
     current_pending_uploads = {}
 
 # TODO: save costs by configuring https://docs.aws.amazon.com/AmazonS3/latest/userguide/mpu-abort-incomplete-mpu-lifecycle-config.html
 # TODO: detect if the cached upload is still available on S3; forget it if it got cleaned up
 for key in current_pending_uploads:
     resume_args = current_pending_uploads[key]
-    print("You have pending upload of {}".format(resume_args["model_file"]))
+    click.echo(
+        "You have pending upload of {}".format(
+            resume_args["model_filepath_or_url"]
+            if "model_filepath_or_url" in resume_args
+            else resume_args[
+                "model_file"
+            ]  # backwards compat - TODO: remove this in May or later
+        )
+    )
     continue_upload = questionary.select(
         "Do you want to continue upload?",
         choices=[
             Choice(title="Yes", value="Y"),
             Choice(title="No", value="n"),
             Choice(title="Drop upload", value="drop"),
         ],
```

### Comparing `autumn8-1.0.1/autumn8/cli/options.py` & `autumn8-1.0.1.post1/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/cli/pending_uploads.py` & `autumn8-1.0.1.post1/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/common/config/cloud_info.py` & `autumn8-1.0.1.post1/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/common/config/s3.py` & `autumn8-1.0.1.post1/autumn8/common/config/s3.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/common/config/settings.py` & `autumn8-1.0.1.post1/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/common/config/supported_instances.py` & `autumn8-1.0.1.post1/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/examples/mnist.py` & `autumn8-1.0.1.post1/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/examples/model.py` & `autumn8-1.0.1.post1/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/examples/sbert-alpha.py` & `autumn8-1.0.1.post1/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.0.1.post1/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/lib/__init__.py` & `autumn8-1.0.1.post1/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/lib/api/cloud.py` & `autumn8-1.0.1.post1/autumn8/lib/api/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/lib/api/lab.py` & `autumn8-1.0.1.post1/autumn8/lib/api/lab.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 import json
 import os
 import urllib
 import urllib.parse
 from http import HTTPStatus
 from threading import Lock
-from typing import Dict, List
+from typing import Any, Dict, List, Optional
 
 import appdirs
 import requests
 from mypy_boto3_s3 import S3Client
 from mypy_boto3_s3.type_defs import PartTypeDef
 from requests.auth import HTTPBasicAuth
 from tqdm.contrib.concurrent import thread_map
@@ -68,15 +68,19 @@
         auth=HTTPBasicAuth(user_id, api_key),
     )
 
     require_ok_response(response)
     return json.loads(response.text)["user"]
 
 
-def post_model(environment: CliEnvironment, organization_id, model_config):
+def post_model(
+    environment: CliEnvironment,
+    organization_id: int,
+    model_config: Dict[str, Any],
+):
     autodl_host = environment.value.app_host
     api_route = f"{autodl_host}/api/lab/model"
     logger.info("Submitting model to %s", api_route)
     response = requests.post(
         url_with_params(api_route, {"organization_id": organization_id}),
         headers={"Content-Type": "application/json"},
         data=json.dumps(model_config),
@@ -123,15 +127,15 @@
             resume_args=resume_args,
             id_key=id_key,
             mpu_id=mpu_id,
             max_upload_workers=max_upload_workers,
         )
 
 
-def normal_upload(environment: CliEnvironment, s3_file_url, f):
+def normal_upload(environment: CliEnvironment, s3_file_url: str, f):
     S3 = init_s3(environment.value.s3_host)
 
     compatible_s3_file_url = get_hacked_legacy_backwards_compatible_s3_file_url(
         environment.value.s3_bucket_root_folder, s3_file_url
     )
 
     S3.Bucket(environment.value.s3_bucket_name).Object(
@@ -186,15 +190,15 @@
             UploadId=mpu_id,
             PartNumber=part_number,
         )
 
 
 def multipart_upload(
     environment: CliEnvironment,
-    s3_file_url,
+    s3_file_url: str,
     file,
     resume_args,
     id_key,
     mpu_id=None,
     max_upload_workers=DEFAULT_MAX_UPLOAD_WORKERS,
 ):
     file.seek(0, 2)  # seek to end of file
@@ -274,18 +278,18 @@
             ]
         },
     )
 
 
 # TODO: fix s3 file structure so that this is not needed
 def get_hacked_legacy_backwards_compatible_s3_file_url(
-    s3_root_folder_name,
-    s3_file_url,
+    s3_root_folder_name: Optional[str],
+    s3_file_url: str,
 ):
-    return s3path_join(s3_root_folder_name, s3_file_url)
+    return s3path_join(s3_root_folder_name or "", s3_file_url)
 
 
 def post_model_file(
     environment: CliEnvironment,
     bytes_or_filepath,
     s3_file_url,
     resume_args,
```

### Comparing `autumn8-1.0.1/autumn8/lib/api_creds.py` & `autumn8-1.0.1.post1/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/lib/logging.py` & `autumn8-1.0.1.post1/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/lib/logging.yaml` & `autumn8-1.0.1.post1/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/lib/package_resolver.py` & `autumn8-1.0.1.post1/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/autumn8/lib/service.py` & `autumn8-1.0.1.post1/autumn8/lib/service.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,39 +25,39 @@
         pending_uploads.abort_and_forget_upload(upload_task["run_id"])
 
 
 def upload_model(
     environment: CliEnvironment,
     organization_id,
     model_config: Dict[str, Any],
-    model_file: str,
+    model_filepath_or_url: str,
     input_file_path: Optional[str],
     max_upload_workers: int = DEFAULT_MAX_UPLOAD_WORKERS,
     model_file_upload_id: Optional[str] = None,
     input_file_upload_id: Optional[str] = None,
     run_id: Optional[str] = None,
     **kwargs,
 ):
     if run_id is None:  # used for resuming upload
         run_id = str(uuid.uuid4())
-    if type(model_file) == io.BytesIO:
-        model_file.seek(0)
+    if type(model_filepath_or_url) == io.BytesIO:
+        model_filepath_or_url.seek(0)
         model_file_name = model_config["name"]  # TODO add extension?
     else:
-        model_file_name = os.path.basename(model_file)
+        model_file_name = os.path.basename(model_filepath_or_url)
 
     s3_bucket_root_folder = environment.value.s3_bucket_root_folder
 
     model_type = None if "model_type" not in kwargs else kwargs["model_type"]
 
     s3_file_url = kwargs.get("s3_file_url") or generate_s3_file_url(
         organization_id=organization_id,
         run_id=run_id,
         model_file_name=model_file_name,
-        model_file=model_file,
+        model_file=model_filepath_or_url,
         s3_bucket_root_folder=s3_bucket_root_folder,
         model_type=model_type,
     )
 
     s3_input_file_url = None
     if input_file_path != None and len(input_file_path) > 0:
         filename = Path(input_file_path).name
@@ -72,15 +72,15 @@
 
     function_args = locals()
 
     time_start = time.time()
     logger.info("Uploading the model files...")
     api.lab.post_model_file(
         environment,
-        model_file,
+        model_filepath_or_url,
         s3_file_url,
         function_args,
         "model_file_upload_id",
         model_file_upload_id,
         max_upload_workers=max_upload_workers,
     )
     model_config["s3_file_url"] = s3_file_url
```

### Comparing `autumn8-1.0.1/autumn8.egg-info/PKG-INFO` & `autumn8-1.0.1.post1/autumn8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.1
+Version: 1.0.1.post1
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.1/autumn8.egg-info/SOURCES.txt` & `autumn8-1.0.1.post1/autumn8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/pyproject.toml` & `autumn8-1.0.1.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/tests/test_io_bottleneck_detection.py` & `autumn8-1.0.1.post1/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1/tests/test_settings.py` & `autumn8-1.0.1.post1/tests/test_settings.py`

 * *Files identical despite different names*

