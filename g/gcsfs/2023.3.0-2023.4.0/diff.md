# Comparing `tmp/gcsfs-2023.3.0.tar.gz` & `tmp/gcsfs-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcsfs-2023.3.0.tar", last modified: Sat Mar  4 20:33:50 2023, max compression
+gzip compressed data, was "gcsfs-2023.4.0.tar", last modified: Tue Apr 11 13:58:16 2023, max compression
```

## Comparing `gcsfs-2023.3.0.tar` & `gcsfs-2023.4.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 20:33:50.318164 gcsfs-2023.3.0/
--rw-r--r--   0 mdurant    (502) staff       (20)     1536 2023-01-02 14:01:40.000000 gcsfs-2023.3.0/LICENSE.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2023.3.0/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     1280 2023-03-04 20:33:50.318244 gcsfs-2023.3.0/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      526 2022-09-18 01:28:26.000000 gcsfs-2023.3.0/README.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 20:33:50.307621 gcsfs-2023.3.0/docs/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 20:33:50.311035 gcsfs-2023.3.0/docs/source/
--rw-r--r--   0 mdurant    (502) staff       (20)      800 2023-02-24 20:42:20.000000 gcsfs-2023.3.0/docs/source/api.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     4094 2023-03-04 20:33:19.000000 gcsfs-2023.3.0/docs/source/changelog.rst
--rw-r--r--   0 mdurant    (502) staff       (20)      906 2022-09-18 01:28:26.000000 gcsfs-2023.3.0/docs/source/developer.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     1776 2023-02-24 20:42:20.000000 gcsfs-2023.3.0/docs/source/fuse.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     6393 2023-02-24 20:42:20.000000 gcsfs-2023.3.0/docs/source/index.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 20:33:50.318883 gcsfs-2023.3.0/gcsfs/
--rw-r--r--   0 mdurant    (502) staff       (20)      192 2022-09-18 01:28:26.000000 gcsfs-2023.3.0/gcsfs/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-03-04 20:33:50.318940 gcsfs-2023.3.0/gcsfs/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3618 2023-01-02 14:01:40.000000 gcsfs-2023.3.0/gcsfs/checkers.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 20:33:50.315199 gcsfs-2023.3.0/gcsfs/cli/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2023.3.0/gcsfs/cli/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1942 2023-01-02 14:01:40.000000 gcsfs-2023.3.0/gcsfs/cli/gcsfuse.py
--rw-r--r--   0 mdurant    (502) staff       (20)    60406 2023-03-02 18:45:14.000000 gcsfs-2023.3.0/gcsfs/core.py
--rw-r--r--   0 mdurant    (502) staff       (20)     8947 2023-01-02 14:01:40.000000 gcsfs-2023.3.0/gcsfs/credentials.py
--rw-r--r--   0 mdurant    (502) staff       (20)       68 2022-09-18 01:28:26.000000 gcsfs-2023.3.0/gcsfs/dask_link.py
--rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2023.3.0/gcsfs/mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4691 2023-01-02 14:01:40.000000 gcsfs-2023.3.0/gcsfs/retry.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 20:33:50.317992 gcsfs-2023.3.0/gcsfs/tests/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2023.3.0/gcsfs/tests/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3885 2023-01-02 14:01:40.000000 gcsfs-2023.3.0/gcsfs/tests/conftest.py
--rw-r--r--   0 mdurant    (502) staff       (20)      178 2023-01-02 14:01:40.000000 gcsfs-2023.3.0/gcsfs/tests/settings.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4029 2023-01-02 14:01:40.000000 gcsfs-2023.3.0/gcsfs/tests/test_checkers.py
--rw-r--r--   0 mdurant    (502) staff       (20)    41351 2023-02-24 20:42:20.000000 gcsfs-2023.3.0/gcsfs/tests/test_core.py
--rw-r--r--   0 mdurant    (502) staff       (20)      222 2022-09-18 01:28:26.000000 gcsfs-2023.3.0/gcsfs/tests/test_credentials.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1822 2023-01-02 14:01:40.000000 gcsfs-2023.3.0/gcsfs/tests/test_fuse.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1040 2023-01-02 14:01:40.000000 gcsfs-2023.3.0/gcsfs/tests/test_manyopens.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3064 2023-01-02 14:01:40.000000 gcsfs-2023.3.0/gcsfs/tests/test_mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3429 2023-01-02 14:01:40.000000 gcsfs-2023.3.0/gcsfs/tests/test_retry.py
--rw-r--r--   0 mdurant    (502) staff       (20)      911 2023-01-02 14:01:40.000000 gcsfs-2023.3.0/gcsfs/tests/utils.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 20:33:50.314949 gcsfs-2023.3.0/gcsfs.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     1280 2023-03-04 20:33:50.000000 gcsfs-2023.3.0/gcsfs.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      842 2023-03-04 20:33:50.000000 gcsfs-2023.3.0/gcsfs.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-03-04 20:33:50.000000 gcsfs-2023.3.0/gcsfs.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-27 12:31:48.000000 gcsfs-2023.3.0/gcsfs.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)      160 2023-03-04 20:33:50.000000 gcsfs-2023.3.0/gcsfs.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        6 2023-03-04 20:33:50.000000 gcsfs-2023.3.0/gcsfs.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      129 2023-03-04 20:33:19.000000 gcsfs-2023.3.0/requirements.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      445 2023-03-04 20:33:50.318665 gcsfs-2023.3.0/setup.cfg
--rwxr-xr-x   0 mdurant    (502) staff       (20)     1184 2023-02-24 20:42:20.000000 gcsfs-2023.3.0/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    68739 2022-09-18 01:28:26.000000 gcsfs-2023.3.0/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-11 13:58:16.889359 gcsfs-2023.4.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1536 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/LICENSE.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     1280 2023-04-11 13:58:16.889424 gcsfs-2023.4.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      526 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/README.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-11 13:58:16.881876 gcsfs-2023.4.0/docs/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-11 13:58:16.884503 gcsfs-2023.4.0/docs/source/
+-rw-r--r--   0 mdurant    (502) staff       (20)      800 2023-02-24 20:42:20.000000 gcsfs-2023.4.0/docs/source/api.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     4125 2023-04-11 13:57:22.000000 gcsfs-2023.4.0/docs/source/changelog.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)      906 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/docs/source/developer.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     1776 2023-02-24 20:42:20.000000 gcsfs-2023.4.0/docs/source/fuse.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     6393 2023-02-24 20:42:20.000000 gcsfs-2023.4.0/docs/source/index.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-11 13:58:16.890161 gcsfs-2023.4.0/gcsfs/
+-rw-r--r--   0 mdurant    (502) staff       (20)      192 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/gcsfs/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-04-11 13:58:16.890202 gcsfs-2023.4.0/gcsfs/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3618 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/checkers.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-11 13:58:16.887541 gcsfs-2023.4.0/gcsfs/cli/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/gcsfs/cli/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1942 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/cli/gcsfuse.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    60406 2023-03-02 18:45:14.000000 gcsfs-2023.4.0/gcsfs/core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     8947 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/credentials.py
+-rw-r--r--   0 mdurant    (502) staff       (20)       68 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/gcsfs/dask_link.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/gcsfs/mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4691 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/retry.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-11 13:58:16.889231 gcsfs-2023.4.0/gcsfs/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/gcsfs/tests/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3885 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/conftest.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      178 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/settings.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4029 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/test_checkers.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    41351 2023-02-24 20:42:20.000000 gcsfs-2023.4.0/gcsfs/tests/test_core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      222 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/gcsfs/tests/test_credentials.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1822 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/test_fuse.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1040 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/test_manyopens.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3064 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/test_mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3429 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/test_retry.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      911 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/utils.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-11 13:58:16.887318 gcsfs-2023.4.0/gcsfs.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1280 2023-04-11 13:58:16.000000 gcsfs-2023.4.0/gcsfs.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      842 2023-04-11 13:58:16.000000 gcsfs-2023.4.0/gcsfs.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-04-11 13:58:16.000000 gcsfs-2023.4.0/gcsfs.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-27 12:31:48.000000 gcsfs-2023.4.0/gcsfs.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)      160 2023-04-11 13:58:16.000000 gcsfs-2023.4.0/gcsfs.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        6 2023-04-11 13:58:16.000000 gcsfs-2023.4.0/gcsfs.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      129 2023-04-11 13:57:22.000000 gcsfs-2023.4.0/requirements.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      445 2023-04-11 13:58:16.889693 gcsfs-2023.4.0/setup.cfg
+-rwxr-xr-x   0 mdurant    (502) staff       (20)     1184 2023-02-24 20:42:20.000000 gcsfs-2023.4.0/setup.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    68739 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/versioneer.py
```

### Comparing `gcsfs-2023.3.0/LICENSE.txt` & `gcsfs-2023.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/PKG-INFO` & `gcsfs-2023.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcsfs
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: Convenient Filesystem interface over GCS
 Home-page: https://github.com/fsspec/gcsfs
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Keywords: google-cloud-storage,gcloud,file-system
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gcsfs-2023.3.0/README.rst` & `gcsfs-2023.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/docs/source/api.rst` & `gcsfs-2023.4.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/docs/source/changelog.rst` & `gcsfs-2023.4.0/docs/source/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+2023.4.0
+--------
+
+No changes
+
 2023.3.0
 --------
 
 * Don't let find() mess up dircache (#531)
 * Drop py3.7 (#529)
 * Update docs (#528)
 * Make times UTC (#527)
```

### Comparing `gcsfs-2023.3.0/docs/source/developer.rst` & `gcsfs-2023.4.0/docs/source/developer.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/docs/source/fuse.rst` & `gcsfs-2023.4.0/docs/source/fuse.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/docs/source/index.rst` & `gcsfs-2023.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/gcsfs/checkers.py` & `gcsfs-2023.4.0/gcsfs/checkers.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/gcsfs/cli/gcsfuse.py` & `gcsfs-2023.4.0/gcsfs/cli/gcsfuse.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/gcsfs/core.py` & `gcsfs-2023.4.0/gcsfs/core.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/gcsfs/credentials.py` & `gcsfs-2023.4.0/gcsfs/credentials.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/gcsfs/retry.py` & `gcsfs-2023.4.0/gcsfs/retry.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/gcsfs/tests/conftest.py` & `gcsfs-2023.4.0/gcsfs/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/gcsfs/tests/test_checkers.py` & `gcsfs-2023.4.0/gcsfs/tests/test_checkers.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/gcsfs/tests/test_core.py` & `gcsfs-2023.4.0/gcsfs/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/gcsfs/tests/test_fuse.py` & `gcsfs-2023.4.0/gcsfs/tests/test_fuse.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/gcsfs/tests/test_manyopens.py` & `gcsfs-2023.4.0/gcsfs/tests/test_manyopens.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/gcsfs/tests/test_mapping.py` & `gcsfs-2023.4.0/gcsfs/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/gcsfs/tests/test_retry.py` & `gcsfs-2023.4.0/gcsfs/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/gcsfs/tests/utils.py` & `gcsfs-2023.4.0/gcsfs/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/gcsfs.egg-info/PKG-INFO` & `gcsfs-2023.4.0/gcsfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcsfs
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: Convenient Filesystem interface over GCS
 Home-page: https://github.com/fsspec/gcsfs
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Keywords: google-cloud-storage,gcloud,file-system
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gcsfs-2023.3.0/gcsfs.egg-info/SOURCES.txt` & `gcsfs-2023.4.0/gcsfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/setup.py` & `gcsfs-2023.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.3.0/versioneer.py` & `gcsfs-2023.4.0/versioneer.py`

 * *Files identical despite different names*

