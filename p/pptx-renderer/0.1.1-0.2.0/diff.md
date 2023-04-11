# Comparing `tmp/pptx_renderer-0.1.1.tar.gz` & `tmp/pptx_renderer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pptx_renderer-0.1.1.tar", last modified: Thu Mar 30 15:54:22 2023, max compression
+gzip compressed data, was "pptx_renderer-0.2.0.tar", last modified: Tue Apr 11 19:51:43 2023, max compression
```

## Comparing `pptx_renderer-0.1.1.tar` & `pptx_renderer-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:54:22.429634 pptx_renderer-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-30 15:54:05.000000 pptx_renderer-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-03-30 15:54:22.429634 pptx_renderer-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-03-30 15:54:05.000000 pptx_renderer-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:54:22.429634 pptx_renderer-0.1.1/pptx_renderer/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-30 15:54:05.000000 pptx_renderer-0.1.1/pptx_renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-30 15:54:05.000000 pptx_renderer-0.1.1/pptx_renderer/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-30 15:54:05.000000 pptx_renderer-0.1.1/pptx_renderer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-03-30 15:54:05.000000 pptx_renderer-0.1.1/pptx_renderer/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-03-30 15:54:05.000000 pptx_renderer-0.1.1/pptx_renderer/pptx_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-30 15:54:05.000000 pptx_renderer-0.1.1/pptx_renderer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:54:22.429634 pptx_renderer-0.1.1/pptx_renderer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-03-30 15:54:22.000000 pptx_renderer-0.1.1/pptx_renderer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-30 15:54:22.000000 pptx_renderer-0.1.1/pptx_renderer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 15:54:22.000000 pptx_renderer-0.1.1/pptx_renderer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-30 15:54:22.000000 pptx_renderer-0.1.1/pptx_renderer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-30 15:54:22.000000 pptx_renderer-0.1.1/pptx_renderer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-30 15:54:22.000000 pptx_renderer-0.1.1/pptx_renderer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-30 15:54:05.000000 pptx_renderer-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 15:54:22.429634 pptx_renderer-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 15:54:05.000000 pptx_renderer-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:54:22.429634 pptx_renderer-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-30 15:54:06.000000 pptx_renderer-0.1.1/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:51:43.048114 pptx_renderer-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 19:51:29.000000 pptx_renderer-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-04-11 19:51:43.048114 pptx_renderer-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-11 19:51:29.000000 pptx_renderer-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:51:43.044114 pptx_renderer-0.2.0/pptx_renderer/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 19:51:29.000000 pptx_renderer-0.2.0/pptx_renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-11 19:51:29.000000 pptx_renderer-0.2.0/pptx_renderer/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-11 19:51:29.000000 pptx_renderer-0.2.0/pptx_renderer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-11 19:51:29.000000 pptx_renderer-0.2.0/pptx_renderer/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-04-11 19:51:29.000000 pptx_renderer-0.2.0/pptx_renderer/pptx_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-11 19:51:29.000000 pptx_renderer-0.2.0/pptx_renderer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:51:43.044114 pptx_renderer-0.2.0/pptx_renderer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-04-11 19:51:43.000000 pptx_renderer-0.2.0/pptx_renderer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-11 19:51:43.000000 pptx_renderer-0.2.0/pptx_renderer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:51:43.000000 pptx_renderer-0.2.0/pptx_renderer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-11 19:51:43.000000 pptx_renderer-0.2.0/pptx_renderer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-11 19:51:43.000000 pptx_renderer-0.2.0/pptx_renderer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 19:51:43.000000 pptx_renderer-0.2.0/pptx_renderer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-11 19:51:29.000000 pptx_renderer-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:51:43.048114 pptx_renderer-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:51:29.000000 pptx_renderer-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:51:43.044114 pptx_renderer-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-11 19:51:29.000000 pptx_renderer-0.2.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-11 19:51:29.000000 pptx_renderer-0.2.0/tests/test_cli.py
```

### Comparing `pptx_renderer-0.1.1/LICENSE` & `pptx_renderer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pptx_renderer-0.1.1/PKG-INFO` & `pptx_renderer-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pptx_renderer
-Version: 0.1.1
+Version: 0.2.0
 Summary: Render ppt like a jupyter notebook
 Author-email: Najeem Muhammed <najeem@gmail.com>
 License: MIT License
         
         Copyright (c) 2023, Najeem Muhammed
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pptx_renderer-0.1.1/README.md` & `pptx_renderer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pptx_renderer-0.1.1/pptx_renderer/plugins.py` & `pptx_renderer-0.2.0/pptx_renderer/plugins.py`

 * *Files identical despite different names*

### Comparing `pptx_renderer-0.1.1/pptx_renderer/pptx_renderer.py` & `pptx_renderer-0.2.0/pptx_renderer/pptx_renderer.py`

 * *Files identical despite different names*

### Comparing `pptx_renderer-0.1.1/pptx_renderer/utils.py` & `pptx_renderer-0.2.0/pptx_renderer/utils.py`

 * *Files identical despite different names*

### Comparing `pptx_renderer-0.1.1/pptx_renderer.egg-info/PKG-INFO` & `pptx_renderer-0.2.0/pptx_renderer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pptx-renderer
-Version: 0.1.1
+Version: 0.2.0
 Summary: Render ppt like a jupyter notebook
 Author-email: Najeem Muhammed <najeem@gmail.com>
 License: MIT License
         
         Copyright (c) 2023, Najeem Muhammed
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pptx_renderer-0.1.1/pyproject.toml` & `pptx_renderer-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pptx_renderer-0.1.1/tests/test_basic.py` & `pptx_renderer-0.2.0/tests/test_basic.py`

 * *Files identical despite different names*

