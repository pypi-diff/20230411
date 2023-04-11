# Comparing `tmp/pytpu-14.6.8.tar.gz` & `tmp/pytpu-14.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytpu-14.6.8.tar", last modified: Mon Apr 10 16:10:29 2023, max compression
+gzip compressed data, was "dist/pytpu-14.7.0.tar", last modified: Tue Apr 11 18:52:34 2023, max compression
```

## Comparing `pytpu-14.6.8.tar` & `pytpu-14.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-10 16:10:29.590434 pytpu-14.6.8/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       41 2023-04-10 16:09:07.000000 pytpu-14.6.8/MANIFEST.in
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4262 2023-04-10 16:10:29.590434 pytpu-14.6.8/PKG-INFO
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3131 2023-04-10 16:09:07.000000 pytpu-14.6.8/README.md
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-10 16:10:29.590434 pytpu-14.6.8/pytpu/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      600 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/__init__.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-10 16:10:29.590434 pytpu-14.6.8/pytpu/pytpu/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      695 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/pytpu/__init__.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)    12138 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/pytpu/libtpu_bindings.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-10 16:10:29.590434 pytpu-14.6.8/pytpu/scripts/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/scripts/__init__.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     2258 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/scripts/pyrun_tpu_cli.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      810 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/scripts/run_get_fps.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-10 16:10:29.590434 pytpu-14.6.8/pytpu/tools/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      119 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/tools/__init__.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     5134 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/tools/get_fps.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     6860 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/tools/helpers.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     7808 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/tools/tpu_runner.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-10 16:10:29.590434 pytpu-14.6.8/pytpu.egg-info/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4262 2023-04-10 16:10:29.000000 pytpu-14.6.8/pytpu.egg-info/PKG-INFO
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      489 2023-04-10 16:10:29.000000 pytpu-14.6.8/pytpu.egg-info/SOURCES.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-04-10 16:10:29.000000 pytpu-14.6.8/pytpu.egg-info/dependency_links.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      109 2023-04-10 16:10:29.000000 pytpu-14.6.8/pytpu.egg-info/entry_points.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-04-10 16:10:29.000000 pytpu-14.6.8/pytpu.egg-info/not-zip-safe
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      197 2023-04-10 16:10:29.000000 pytpu-14.6.8/pytpu.egg-info/requires.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        6 2023-04-10 16:10:29.000000 pytpu-14.6.8/pytpu.egg-info/top_level.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       38 2023-04-10 16:10:29.590434 pytpu-14.6.8/setup.cfg
--rwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)     1531 2023-04-10 16:10:29.000000 pytpu-14.6.8/setup.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-11 18:52:34.318198 pytpu-14.7.0/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       41 2023-04-11 18:51:16.000000 pytpu-14.7.0/MANIFEST.in
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4262 2023-04-11 18:52:34.318198 pytpu-14.7.0/PKG-INFO
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3131 2023-04-11 18:51:16.000000 pytpu-14.7.0/README.md
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-11 18:52:34.314198 pytpu-14.7.0/pytpu/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      600 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/__init__.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-11 18:52:34.318198 pytpu-14.7.0/pytpu/pytpu/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      695 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/pytpu/__init__.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)    12138 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/pytpu/libtpu_bindings.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-11 18:52:34.318198 pytpu-14.7.0/pytpu/scripts/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/scripts/__init__.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     2258 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/scripts/pyrun_tpu_cli.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      810 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/scripts/run_get_fps.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-11 18:52:34.318198 pytpu-14.7.0/pytpu/tools/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      119 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/tools/__init__.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     5134 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/tools/get_fps.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     6860 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/tools/helpers.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     7808 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/tools/tpu_runner.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-11 18:52:34.318198 pytpu-14.7.0/pytpu.egg-info/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4262 2023-04-11 18:52:34.000000 pytpu-14.7.0/pytpu.egg-info/PKG-INFO
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      489 2023-04-11 18:52:34.000000 pytpu-14.7.0/pytpu.egg-info/SOURCES.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-04-11 18:52:34.000000 pytpu-14.7.0/pytpu.egg-info/dependency_links.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      109 2023-04-11 18:52:34.000000 pytpu-14.7.0/pytpu.egg-info/entry_points.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-04-11 18:52:34.000000 pytpu-14.7.0/pytpu.egg-info/not-zip-safe
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      197 2023-04-11 18:52:34.000000 pytpu-14.7.0/pytpu.egg-info/requires.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        6 2023-04-11 18:52:34.000000 pytpu-14.7.0/pytpu.egg-info/top_level.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       38 2023-04-11 18:52:34.318198 pytpu-14.7.0/setup.cfg
+-rwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)     1531 2023-04-11 18:52:34.000000 pytpu-14.7.0/setup.py
```

### Comparing `pytpu-14.6.8/PKG-INFO` & `pytpu-14.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytpu
-Version: 14.6.8
+Version: 14.7.0
 Summary: TPU Python API
 Home-page: http://git.mmp.iva-tech.ru/tpu_sw/iva_tpu_sdk
 Author: Alexey Antipin
 Author-email: a.antipin@iva-tech.ru
 License: UNKNOWN
 Description: # IVA TPU Python API
         ## Main entities
```

### Comparing `pytpu-14.6.8/README.md` & `pytpu-14.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.8/pytpu/__init__.py` & `pytpu-14.7.0/pytpu/__init__.py`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.8/pytpu/pytpu/__init__.py` & `pytpu-14.7.0/pytpu/pytpu/__init__.py`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.8/pytpu/pytpu/libtpu_bindings.py` & `pytpu-14.7.0/pytpu/pytpu/libtpu_bindings.py`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.8/pytpu/scripts/pyrun_tpu_cli.py` & `pytpu-14.7.0/pytpu/scripts/pyrun_tpu_cli.py`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.8/pytpu/scripts/run_get_fps.py` & `pytpu-14.7.0/pytpu/scripts/run_get_fps.py`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.8/pytpu/tools/get_fps.py` & `pytpu-14.7.0/pytpu/tools/get_fps.py`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.8/pytpu/tools/helpers.py` & `pytpu-14.7.0/pytpu/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.8/pytpu/tools/tpu_runner.py` & `pytpu-14.7.0/pytpu/tools/tpu_runner.py`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.8/pytpu.egg-info/PKG-INFO` & `pytpu-14.7.0/pytpu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytpu
-Version: 14.6.8
+Version: 14.7.0
 Summary: TPU Python API
 Home-page: http://git.mmp.iva-tech.ru/tpu_sw/iva_tpu_sdk
 Author: Alexey Antipin
 Author-email: a.antipin@iva-tech.ru
 License: UNKNOWN
 Description: # IVA TPU Python API
         ## Main entities
```

### Comparing `pytpu-14.6.8/setup.py` & `pytpu-14.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #     print(f'Install version: {VERSION}')
 
 setup(
     name='pytpu',
     packages=['pytpu', 'pytpu.tools', 'pytpu.pytpu', 'pytpu.scripts'],
     # packages=find_packages(),
     # version=VERSION,
-    version="14.6.8",
+    version="14.7.0",
     author="Alexey Antipin",
     author_email="a.antipin@iva-tech.ru",
     description="TPU Python API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://git.mmp.iva-tech.ru/tpu_sw/iva_tpu_sdk",
     install_requires=[
```

