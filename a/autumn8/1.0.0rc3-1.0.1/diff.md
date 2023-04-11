# Comparing `tmp/autumn8-1.0.0rc3.tar.gz` & `tmp/autumn8-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.0rc3.tar", last modified: Wed Apr  5 00:11:47 2023, max compression
+gzip compressed data, was "autumn8-1.0.1.tar", last modified: Tue Apr 11 13:33:07 2023, max compression
```

## Comparing `autumn8-1.0.0rc3.tar` & `autumn8-1.0.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-05 00:11:47.066767 autumn8-1.0.0rc3/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2381 2023-04-05 00:11:47.066767 autumn8-1.0.0rc3/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2161 2023-03-10 14:58:37.000000 autumn8-1.0.0rc3/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-05 00:11:47.046767 autumn8-1.0.0rc3/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.0rc3/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-05 00:11:47.056767 autumn8-1.0.0rc3/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.0rc3/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.0rc3/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7857 2023-04-04 14:37:22.000000 autumn8-1.0.0rc3/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-04 14:37:22.000000 autumn8-1.0.0rc3/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-05 00:11:47.056767 autumn8-1.0.0rc3/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3190 2023-04-04 23:38:31.000000 autumn8-1.0.0rc3/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    14629 2023-04-05 00:05:16.000000 autumn8-1.0.0rc3/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.0rc3/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1453 2023-04-04 23:38:31.000000 autumn8-1.0.0rc3/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2992 2023-04-04 23:38:31.000000 autumn8-1.0.0rc3/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4953 2023-04-04 14:37:22.000000 autumn8-1.0.0rc3/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3126 2023-04-04 14:37:22.000000 autumn8-1.0.0rc3/autumn8/cli/pending_uploads.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-05 00:11:47.056767 autumn8-1.0.0rc3/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.0rc3/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-04-05 00:11:27.000000 autumn8-1.0.0rc3/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-05 00:11:47.056767 autumn8-1.0.0rc3/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.0rc3/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6503 2023-03-28 23:07:20.000000 autumn8-1.0.0rc3/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3200 2023-04-04 23:47:31.000000 autumn8-1.0.0rc3/autumn8/common/config/s3.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.0rc3/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    63841 2023-03-28 23:07:20.000000 autumn8-1.0.0rc3/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      366 2023-03-28 23:07:20.000000 autumn8-1.0.0rc3/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-05 00:11:47.056767 autumn8-1.0.0rc3/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.0rc3/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.0rc3/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.0rc3/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.0rc3/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.0rc3/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.0rc3/autumn8/examples/tensorflow_custom_layers.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-05 00:11:47.056767 autumn8-1.0.0rc3/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-04 14:37:22.000000 autumn8-1.0.0rc3/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-05 00:11:47.056767 autumn8-1.0.0rc3/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.0rc3/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2657 2023-03-28 23:07:20.000000 autumn8-1.0.0rc3/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    10168 2023-04-04 23:38:31.000000 autumn8-1.0.0rc3/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.0rc3/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1149 2023-04-04 14:37:22.000000 autumn8-1.0.0rc3/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-04 23:38:31.000000 autumn8-1.0.0rc3/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.0rc3/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4512 2023-04-04 23:38:31.000000 autumn8-1.0.0rc3/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-05 00:11:47.046767 autumn8-1.0.0rc3/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2381 2023-04-05 00:11:47.000000 autumn8-1.0.0rc3/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1262 2023-04-05 00:11:47.000000 autumn8-1.0.0rc3/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-04-05 00:11:47.000000 autumn8-1.0.0rc3/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-04-05 00:11:47.000000 autumn8-1.0.0rc3/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      126 2023-04-05 00:11:47.000000 autumn8-1.0.0rc3/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-04-05 00:11:47.000000 autumn8-1.0.0rc3/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1933 2023-03-31 14:44:39.000000 autumn8-1.0.0rc3/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-04-05 00:11:47.066767 autumn8-1.0.0rc3/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.0rc3/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-05 00:11:47.066767 autumn8-1.0.0rc3/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.0rc3/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.0rc3/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.492624 autumn8-1.0.1/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2378 2023-04-11 13:33:07.492624 autumn8-1.0.1/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2161 2023-03-10 14:58:37.000000 autumn8-1.0.1/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.442623 autumn8-1.0.1/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.462623 autumn8-1.0.1/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7857 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.462623 autumn8-1.0.1/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3190 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    14901 2023-04-11 13:30:43.000000 autumn8-1.0.1/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1453 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2992 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4953 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3126 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/cli/pending_uploads.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.462623 autumn8-1.0.1/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      103 2023-04-11 13:28:16.000000 autumn8-1.0.1/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.472623 autumn8-1.0.1/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6503 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3200 2023-04-11 12:40:47.000000 autumn8-1.0.1/autumn8/common/config/s3.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    63841 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      366 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.482623 autumn8-1.0.1/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/examples/tensorflow_custom_layers.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.482623 autumn8-1.0.1/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.492624 autumn8-1.0.1/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2657 2023-03-28 23:07:20.000000 autumn8-1.0.1/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    10168 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.1/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1149 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.1/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4512 2023-04-11 12:01:33.000000 autumn8-1.0.1/autumn8/lib/service.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.452623 autumn8-1.0.1/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2378 2023-04-11 13:33:07.000000 autumn8-1.0.1/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1262 2023-04-11 13:33:07.000000 autumn8-1.0.1/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-04-11 13:33:07.000000 autumn8-1.0.1/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-04-11 13:33:07.000000 autumn8-1.0.1/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      126 2023-04-11 13:33:07.000000 autumn8-1.0.1/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-04-11 13:33:07.000000 autumn8-1.0.1/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1933 2023-03-31 14:44:39.000000 autumn8-1.0.1/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-04-11 13:33:07.492624 autumn8-1.0.1/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.1/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 13:33:07.492624 autumn8-1.0.1/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.1/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.1/tests/test_settings.py
```

### Comparing `autumn8-1.0.0rc3/PKG-INFO` & `autumn8-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.0rc3
+Version: 1.0.1
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.0rc3/README.md` & `autumn8-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/cli/analyze.py` & `autumn8-1.0.1/autumn8/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/cli/cli_environment.py` & `autumn8-1.0.1/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/cli/commands/cloud.py` & `autumn8-1.0.1/autumn8/cli/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/cli/commands/models.py` & `autumn8-1.0.1/autumn8/cli/commands/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,54 +369,62 @@
         input_file_path=input_file,
         max_upload_workers=max_upload_workers,
     )
 
     announce_model_upload_response(model_upload_response)
 
 
-supported_model_types = {"GPT-J 6B": "gptj"}
+class SupportedModel(str, enum.Enum):
+    GPTJ = "gptj"
+
+
+supported_models_by_human_readable_label = {"GPT-J 6B": SupportedModel.GPTJ}
 
 
 @model_commands_group.command()
 @options.use_environment
 @click.argument("checkpoint_file_path")
 @common_upload_args
 @click.option(
-    "-t",
+    "-m",
     "--model_type",
+    "--model",
     type=click.Choice(
-        list(supported_model_types.values()), case_sensitive=False
+        list(SupportedModel),
+        case_sensitive=False,
     ),
     default=None,
-    help="Type of model",
+    help="One of the supported models for the checkpoint",
 )
 def submit_checkpoint(
-    organization_id,
-    checkpoint_file_path,
-    model_type,
-    model_name,
-    auto_confirm,
+    organization_id: int,
+    checkpoint_file_path: str,
+    model_type: Optional[SupportedModel],
+    model_name: str,
+    auto_confirm: bool,
     quantization,
     should_skip_inputs: bool,
     input_dims,
     input_file,
     group_id,
     max_upload_workers,
     **kwargs,
 ):
     """submit checkpoint to AutoDL"""
     environment = kwargs["environment"]
 
     if model_type is None:
         model_type_user_choice = questionary.select(
             "Choose one of the supported models for the checkpoint data",
-            choices=list(supported_model_types.keys()),
+            choices=list(supported_models_by_human_readable_label.keys()),
             use_shortcuts=True,
         ).unsafe_ask()
-        model_type = supported_model_types[model_type_user_choice]
+        model_type = supported_models_by_human_readable_label[
+            model_type_user_choice
+        ]
 
     framework = "PYTORCH"
     inferred_quantization = None  # nice to have TODO: detect quantization
     inferred_input_dims = None
     inferred_model_name = suggest_model_name(checkpoint_file_path)
     model_filepath = checkpoint_file_path
 
@@ -437,14 +445,15 @@
     )
     model_config = {
         "name": model_name,
         "framework": framework,
         "quantization": quantization,
         "inputs": input_dims,
         "group_id": group_id,
+        "model_type": model_type,
     }
 
     if not auto_confirm:
         logger.info("The details for your model are as follows:")
         click.echo(f"{json.dumps(model_config, indent=4)}")
         click.confirm(
             text="\n" + "Do you want to upload it to AutoDL?",
```

### Comparing `autumn8-1.0.0rc3/autumn8/cli/examples.py` & `autumn8-1.0.1/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/cli/interactive.py` & `autumn8-1.0.1/autumn8/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/cli/main.py` & `autumn8-1.0.1/autumn8/cli/main.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/cli/options.py` & `autumn8-1.0.1/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/cli/pending_uploads.py` & `autumn8-1.0.1/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/common/config/cloud_info.py` & `autumn8-1.0.1/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/common/config/s3.py` & `autumn8-1.0.1/autumn8/common/config/s3.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/common/config/settings.py` & `autumn8-1.0.1/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/common/config/supported_instances.py` & `autumn8-1.0.1/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/examples/mnist.py` & `autumn8-1.0.1/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/examples/model.py` & `autumn8-1.0.1/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/examples/sbert-alpha.py` & `autumn8-1.0.1/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.0.1/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/lib/__init__.py` & `autumn8-1.0.1/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/lib/api/cloud.py` & `autumn8-1.0.1/autumn8/lib/api/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/lib/api/lab.py` & `autumn8-1.0.1/autumn8/lib/api/lab.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/lib/api_creds.py` & `autumn8-1.0.1/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/lib/logging.py` & `autumn8-1.0.1/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/lib/logging.yaml` & `autumn8-1.0.1/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/lib/package_resolver.py` & `autumn8-1.0.1/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8/lib/service.py` & `autumn8-1.0.1/autumn8/lib/service.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/autumn8.egg-info/PKG-INFO` & `autumn8-1.0.1/autumn8.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.0rc3
+Version: 1.0.1
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.0rc3/autumn8.egg-info/SOURCES.txt` & `autumn8-1.0.1/autumn8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/pyproject.toml` & `autumn8-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/tests/test_io_bottleneck_detection.py` & `autumn8-1.0.1/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.0rc3/tests/test_settings.py` & `autumn8-1.0.1/tests/test_settings.py`

 * *Files identical despite different names*

