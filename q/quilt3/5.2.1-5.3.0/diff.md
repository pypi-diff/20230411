# Comparing `tmp/quilt3-5.2.1.tar.gz` & `tmp/quilt3-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/quilt/quilt/api/python/dist/.tmp-7uu_r6jx/quilt3-5.2.1.tar", last modified: Wed Apr  5 11:03:20 2023, max compression
+gzip compressed data, was "/home/runner/work/quilt/quilt/api/python/dist/.tmp-tptj4r8t/quilt3-5.3.0.tar", last modified: Tue Apr 11 14:19:20 2023, max compression
```

## Comparing `quilt3-5.2.1.tar` & `quilt3-5.3.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:03:20.000000 quilt3-5.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-05 11:02:59.000000 quilt3-5.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-05 11:02:59.000000 quilt3-5.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-05 11:03:20.000000 quilt3-5.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:03:20.000000 quilt3-5.2.1/quilt3/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:03:20.000000 quilt3-5.2.1/quilt3/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/backends/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/backends/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    47152 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    40889 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    16032 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    62972 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/search_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19087 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:03:20.000000 quilt3-5.2.1/quilt3/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-05 11:02:59.000000 quilt3-5.2.1/quilt3/workflows/config-1.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:03:20.000000 quilt3-5.2.1/quilt3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-05 11:03:20.000000 quilt3-5.2.1/quilt3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-05 11:03:20.000000 quilt3-5.2.1/quilt3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 11:03:20.000000 quilt3-5.2.1/quilt3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-05 11:03:20.000000 quilt3-5.2.1/quilt3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-05 11:03:20.000000 quilt3-5.2.1/quilt3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-05 11:03:20.000000 quilt3-5.2.1/quilt3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 11:03:20.000000 quilt3-5.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-05 11:02:59.000000 quilt3-5.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 11:03:20.000000 quilt3-5.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-05 11:02:59.000000 quilt3-5.2.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-04-05 11:02:59.000000 quilt3-5.2.1/tests/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-04-05 11:02:59.000000 quilt3-5.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    24967 2023-04-05 11:02:59.000000 quilt3-5.2.1/tests/test_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-05 11:02:59.000000 quilt3-5.2.1/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-05 11:02:59.000000 quilt3-5.2.1/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-05 11:02:59.000000 quilt3-5.2.1/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-05 11:02:59.000000 quilt3-5.2.1/tests/test_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-05 11:02:59.000000 quilt3-5.2.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-04-05 11:02:59.000000 quilt3-5.2.1/tests/test_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:19:20.000000 quilt3-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 14:18:57.000000 quilt3-5.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 14:18:57.000000 quilt3-5.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-11 14:19:20.000000 quilt3-5.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/backends/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/backends/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47152 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42579 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62972 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/search_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19087 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/workflows/config-1.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 14:19:20.000000 quilt3-5.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-11 14:18:57.000000 quilt3-5.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:19:20.000000 quilt3-5.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24967 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_workflows.py
```

### Comparing `quilt3-5.2.1/LICENSE` & `quilt3-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/PKG-INFO` & `quilt3-5.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quilt3
-Version: 5.2.1
+Version: 5.3.0
 Summary: Quilt: where data comes together
 Home-page: https://github.com/quiltdata/quilt
 Author: quiltdata
 Author-email: contact@quiltdata.io
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Provides-Extra: pyarrow
+Provides-Extra: anndata
 Provides-Extra: tests
 Provides-Extra: catalog
 License-File: LICENSE
 
 Quilt manages data like code (with packages, repositories, browsing and
 revision history) so that teams can experiment faster in machine learning,
 biotech, and other data-driven domains.
```

### Comparing `quilt3-5.2.1/quilt3/__init__.py` & `quilt3-5.3.0/quilt3/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/admin.py` & `quilt3-5.3.0/quilt3/admin.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/api.py` & `quilt3-5.3.0/quilt3/api.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/backends/__init__.py` & `quilt3-5.3.0/quilt3/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/backends/base.py` & `quilt3-5.3.0/quilt3/backends/base.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/backends/local.py` & `quilt3-5.3.0/quilt3/backends/local.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/backends/s3.py` & `quilt3-5.3.0/quilt3/backends/s3.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/bucket.py` & `quilt3-5.3.0/quilt3/bucket.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/data_transfer.py` & `quilt3-5.3.0/quilt3/data_transfer.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/formats.py` & `quilt3-5.3.0/quilt3/formats.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,20 +65,23 @@
 
 """
 
 
 import copy
 import csv
 import gzip
+import importlib
 import io
 import json
 import sys
+import tempfile
 import warnings
 from abc import ABC, abstractmethod
 from collections import defaultdict
+from pathlib import Path
 
 try:
     from importlib import metadata as importlib_metadata
 except ImportError:
     import importlib_metadata
 
 from .util import QuiltException
@@ -319,37 +322,37 @@
     @classmethod
     def all_supported_formats(cls):
         """
         Returns a map of supported object types -> serialization formats, e.g.:
 
                             Python Object Type     Serialization Formats
          <class 'pandas.core.frame.DataFrame'>  [ssv, csv, tsv, parquet]
+                     <class 'anndata.AnnData'>                   [.h5ad]
                        <class 'numpy.ndarray'>                [npy, npz]
                                  <class 'str'>      [md, json, rst, txt]
                                 <class 'dict'>                    [json]
                             <class 'NoneType'>                    [json]
                                <class 'tuple'>                    [json]
                                  <class 'int'>                    [json]
                                 <class 'list'>                    [json]
                                <class 'float'>                    [json]
                                <class 'bytes'>                     [bin]
         """
-        try:
-            import numpy as np
-        except ImportError:
-            pass
-        else:
-            cls.search(np.ndarray)  # Force FormatHandlers to register np.ndarray as a supported object type
-
-        try:
-            import pandas as pd
-        except ImportError:
-            pass
-        else:
-            cls.search(pd.DataFrame)  # Force FormatHandlers to register pd.DataFrame as a supported object type
+        # Force FormatHandlers to register these classes as supported object types
+        for mod_name, cls_name in [
+            ('numpy', 'ndarray'),
+            ('pandas', 'DataFrame'),
+            ('anndata', 'AnnData'),
+        ]:
+            try:
+                mod = importlib.import_module(mod_name)
+            except ImportError:
+                pass
+            else:
+                cls.search(getattr(mod, cls_name))
 
         type_map = defaultdict(set)
         for handler in cls.registered_handlers:
             for t in handler.handled_types:
                 type_map[t].update(handler.handled_extensions)
         return dict(type_map)
 
@@ -1029,14 +1032,63 @@
 
 
 # compat -- also handle 'pyarrow' in meta['target'] and meta['format']['name'].
 ParquetFormatHandler('pyarrow').register()
 ParquetFormatHandler().register()  # latest is preferred
 
 
+class AnnDataFormatHandler(BaseFormatHandler):
+    """Format for AnnData <--> .h5ad
+
+    Format Opts:
+        The following options may be used anywhere format opts are accepted,
+        or directly in metadata under `{'format': {'opts': {...: ...}}}`.
+
+        compression('gzip', 'lzf', None):  applies during serialization only.
+    """
+    name = 'h5ad'
+    handled_extensions = ['h5ad']
+    opts = ('compression',)
+    defaults = dict(
+        compression='lzf',
+    )
+
+    def handles_type(self, typ: type) -> bool:
+        # don't load module unless we actually have to use it.
+        if 'anndata' not in sys.modules:
+            return False
+        import anndata as ad
+        self.handled_types.add(ad.AnnData)
+        return super().handles_type(typ)
+
+    def serialize(self, obj, meta=None, ext=None, **format_opts):
+        opts = self.get_opts(meta, format_opts)
+        opts_with_defaults = copy.deepcopy(self.defaults)
+        opts_with_defaults.update(opts)
+
+        with tempfile.TemporaryDirectory() as td:
+            path = Path(td) / 'data.h5ad'
+            obj.write(path, **opts_with_defaults)
+            data = path.read_bytes()
+
+        return data, self._update_meta(meta, additions=opts_with_defaults)
+
+    def deserialize(self, bytes_obj, meta=None, ext=None, **format_opts):
+        try:
+            import anndata as ad
+        except ImportError:
+            raise QuiltException("Please install quilt3[anndata]")
+
+        buf = io.BytesIO(bytes_obj)
+        return ad.read_h5ad(buf)
+
+
+AnnDataFormatHandler().register()
+
+
 class CompressionRegistry:
     """A collection for organizing `CompressionHandler` objects."""
     registered_handlers = []
 
     def __init__(self):
         raise TypeError("The {!r} class is organizational, and cannot be instantiated."
                         .format(type(self).__name__))
```

### Comparing `quilt3-5.2.1/quilt3/imports.py` & `quilt3-5.3.0/quilt3/imports.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/main.py` & `quilt3-5.3.0/quilt3/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sys
 import time
 
 import requests
 
 from . import Package
 from . import __version__ as quilt3_version
-from . import api, session
+from . import api, session, util
 from .backends import get_package_registry
 from .session import open_url
 from .util import (
     QuiltException,
     catalog_package_url,
     catalog_s3_url,
     get_from_config,
@@ -198,24 +198,33 @@
         print("Verification succeeded")
         return 0
     else:
         print("Verification failed")
         return 1
 
 
-def cmd_push(name, dir, registry, dest, message, meta, workflow, force, dedupe):
+# This is not a lambda to ease of testing.
+def _selector_fn_no_copy(*args):
+    return False
+
+
+def cmd_push(name, dir, registry, dest, message, meta, workflow, force, dedupe, no_copy):
+    if util.PhysicalKey.from_url(util.fix_url(dir)).is_local() and no_copy:
+        raise QuiltException("--no-copy flag can be specified only for remote data.")
+
     try:
         pkg = Package.browse(name, None)
     except FileNotFoundError:
         pkg = Package()
 
     pkg.set_dir('.', dir, meta=meta)
     pkg.push(
         name, registry=registry, dest=dest, message=message,
-        workflow=workflow, force=force, dedupe=dedupe
+        workflow=workflow, force=force, dedupe=dedupe,
+        **({"selector_fn": _selector_fn_no_copy} if no_copy else {}),
     )
 
 
 def create_parser():
     parser = argparse.ArgumentParser(allow_abbrev=False)
     parser.add_argument(
             "--version",
@@ -461,14 +470,19 @@
             """,
     )
     optional_args.add_argument(
         "--dedupe",
         action="store_true",
         help="Skip the push if the local package hash matches the remote hash.",
     )
+    optional_args.add_argument(
+        "--no-copy",
+        action="store_true",
+        help="Do not copy data. Package manifest entries will reference the data at the original location.",
+    )
     push_p.set_defaults(func=cmd_push)
 
     return parser
 
 
 def main(args=None):
     parser = create_parser()
```

### Comparing `quilt3-5.2.1/quilt3/packages.py` & `quilt3-5.3.0/quilt3/packages.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/search_util.py` & `quilt3-5.3.0/quilt3/search_util.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/session.py` & `quilt3-5.3.0/quilt3/session.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/telemetry.py` & `quilt3-5.3.0/quilt3/telemetry.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/util.py` & `quilt3-5.3.0/quilt3/util.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/workflows/__init__.py` & `quilt3-5.3.0/quilt3/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3/workflows/config-1.schema.json` & `quilt3-5.3.0/quilt3/workflows/config-1.schema.json`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/quilt3.egg-info/PKG-INFO` & `quilt3-5.3.0/quilt3.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quilt3
-Version: 5.2.1
+Version: 5.3.0
 Summary: Quilt: where data comes together
 Home-page: https://github.com/quiltdata/quilt
 Author: quiltdata
 Author-email: contact@quiltdata.io
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Provides-Extra: pyarrow
+Provides-Extra: anndata
 Provides-Extra: tests
 Provides-Extra: catalog
 License-File: LICENSE
 
 Quilt manages data like code (with packages, repositories, browsing and
 revision history) so that teams can experiment faster in machine learning,
 biotech, and other data-driven domains.
```

### Comparing `quilt3-5.2.1/quilt3.egg-info/SOURCES.txt` & `quilt3-5.3.0/quilt3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/setup.py` & `quilt3-5.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -71,18 +71,18 @@
     ],
     extras_require={
         'pyarrow': [
             'numpy>=1.14.0',                # required by pandas, but missing from its dependencies.
             'pandas>=0.19.2',
             'pyarrow>=0.14.1',              # as of 7/5/19: linux/circleci bugs on 0.14.0
         ],
+        'anndata': ['anndata>=0.8.0'],
         'tests': [
-            'numpy>=1.14.0',                # required by pandas, but missing from its dependencies.
-            'pandas>=0.19.2',
-            'pyarrow>=0.14.1',              # as of 7/5/19: linux/circleci bugs on 0.14.0
+            'anndata!=0.9.0',
+            'quilt3[pyarrow,anndata]',
             'pytest==6.*',
             'pytest-cov',
             'coverage==6.4',
             'pytest-env',
             'pytest-subtests',
             'responses',
             'git-pylint-commit-hook',
```

### Comparing `quilt3-5.2.1/tests/test_api.py` & `quilt3-5.3.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/tests/test_bucket.py` & `quilt3-5.3.0/tests/test_bucket.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/tests/test_cli.py` & `quilt3-5.3.0/tests/test_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -190,7 +190,33 @@
     with patch('quilt3.backends.s3.S3PackageRegistryV1.list_packages') as list_packages_mock:
         list_packages_mock.return_value = pkg_names
         main.main(('list-packages', registry))
 
         list_packages_mock.assert_called_once_with()
         captured = capsys.readouterr()
         assert captured.out.split() == pkg_names
+
+
+def test_push_no_copy():
+    name = 'test/name'
+    dir_path = 's3://test/dir/path'
+
+    with patch_package_class as mocked_package_class:
+        main.main(('push', '--dir', dir_path, '--no-copy', name))
+
+        mocked_package_class.browse.assert_called_once_with(name, None)
+        mocked_package_class.assert_not_called()
+        mocked_package = mocked_package_class.browse.return_value
+        mocked_package.set_dir.assert_called_once_with('.', dir_path, meta=None)
+        mocked_package.push.assert_called_once_with(
+            name, registry=None, dest=None, message=None, workflow=..., force=False, dedupe=False,
+            selector_fn=main._selector_fn_no_copy,
+        )
+
+
+def test_push_no_copy_local_dir(capsys):
+    name = 'test/name'
+    dir_path = 'test/dir/path'
+
+    assert main.main(('push', '--dir', dir_path, '--no-copy', name)) == 1
+    captured = capsys.readouterr()
+    assert "--no-copy flag can be specified only for remote data." in captured.err
```

### Comparing `quilt3-5.2.1/tests/test_data_transfer.py` & `quilt3-5.3.0/tests/test_data_transfer.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/tests/test_formats.py` & `quilt3-5.3.0/tests/test_formats.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import pathlib
 
 import numpy as np
 import pandas as pd
 import pytest
+from anndata import AnnData
 
 from quilt3.formats import FormatRegistry
 from quilt3.util import QuiltException
 
 # Constants
+data_dir = pathlib.Path(__file__).parent / 'data'
 
 
 # Code
 def test_buggy_parquet():
     """
     Test that Quilt avoids crashing on bad Pandas metadata from
     old pyarrow libaries.
@@ -142,14 +144,44 @@
     meta.update(format_meta)
     df2 = FormatRegistry.deserialize(bin, meta)
 
     assert test_data == bin
     assert df1.equals(df2)
 
 
+def test_formats_anndata_roundtrip():
+    meta = {'format': {'name': 'h5ad'}}
+    ad_file = data_dir / 'test.h5ad'
+    ad: AnnData = FormatRegistry.deserialize(ad_file.read_bytes(), meta)
+    assert isinstance(ad, AnnData)
+
+    bin, format_meta = FormatRegistry.serialize(ad, meta)
+    meta2 = {**meta, **format_meta}
+    ad2: AnnData = FormatRegistry.deserialize(bin, meta2)
+    np.allclose(ad.X, ad2.X)
+    ad.obs.equals(ad2.obs)
+    ad.var.equals(ad2.var)
+
+
+def test_all_supported_formats():
+    assert FormatRegistry.all_supported_formats() == {
+        AnnData: {'h5ad'},
+        pd.DataFrame: {'csv', 'parquet', 'ssv', 'tsv'},
+        np.ndarray: {'npy', 'npz'},
+        str: {'json', 'md', 'rst', 'txt'},
+        tuple: {'json'},
+        type(None): {'json'},
+        dict: {'json'},
+        int: {'json'},
+        list: {'json'},
+        float: {'json'},
+        bytes: {'bin'},
+    }
+
+
 def test_formats_search_fail_notfound():
     # a search that finds nothing should raise with an explanation.
     class Foo:
         pass
 
     bad_kwargs = [
         dict(obj_type=Foo, meta=None, ext=None),
```

### Comparing `quilt3-5.2.1/tests/test_search.py` & `quilt3-5.3.0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/tests/test_session.py` & `quilt3-5.3.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/tests/test_telemetry.py` & `quilt3-5.3.0/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/tests/test_util.py` & `quilt3-5.3.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.2.1/tests/test_workflows.py` & `quilt3-5.3.0/tests/test_workflows.py`

 * *Files identical despite different names*

