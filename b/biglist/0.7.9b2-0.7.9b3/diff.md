# Comparing `tmp/biglist-0.7.9b2.tar.gz` & `tmp/biglist-0.7.9b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biglist-0.7.9b2.tar", last modified: Mon Apr 10 23:43:11 2023, max compression
+gzip compressed data, was "biglist-0.7.9b3.tar", last modified: Tue Apr 11 16:10:10 2023, max compression
```

## Comparing `biglist-0.7.9b2.tar` & `biglist-0.7.9b3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.7.9b2/LICENSE
--rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.7.9b2/README.rst
--rw-r--r--   0        0        0     1628 2023-04-10 23:37:10.541736 biglist-0.7.9b2/pyproject.toml
--rw-r--r--   0        0        0     2217 2023-04-10 23:37:43.212858 biglist-0.7.9b2/src/biglist/__init__.py
--rw-r--r--   0        0        0    18415 2023-04-10 09:40:14.847560 biglist-0.7.9b2/src/biglist/_base.py
--rw-r--r--   0        0        0    43804 2023-04-10 23:41:15.207783 biglist-0.7.9b2/src/biglist/_biglist.py
--rw-r--r--   0        0        0    33751 2023-04-10 09:40:14.847560 biglist-0.7.9b2/src/biglist/_parquet.py
--rw-r--r--   0        0        0    12025 2023-04-10 09:40:14.847560 biglist-0.7.9b2/src/biglist/_util.py
--rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.7.9b2/src/biglist/py.typed
--rw-r--r--   0        0        0     2209 1970-01-01 00:00:00.000000 biglist-0.7.9b2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.7.9b3/LICENSE
+-rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.7.9b3/README.rst
+-rw-r--r--   0        0        0     1628 2023-04-11 16:08:19.638866 biglist-0.7.9b3/pyproject.toml
+-rw-r--r--   0        0        0     2217 2023-04-11 15:56:45.207292 biglist-0.7.9b3/src/biglist/__init__.py
+-rw-r--r--   0        0        0    18415 2023-04-10 09:40:14.847560 biglist-0.7.9b3/src/biglist/_base.py
+-rw-r--r--   0        0        0    43822 2023-04-11 15:54:40.146432 biglist-0.7.9b3/src/biglist/_biglist.py
+-rw-r--r--   0        0        0    33751 2023-04-10 09:40:14.847560 biglist-0.7.9b3/src/biglist/_parquet.py
+-rw-r--r--   0        0        0    12025 2023-04-10 09:40:14.847560 biglist-0.7.9b3/src/biglist/_util.py
+-rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.7.9b3/src/biglist/py.typed
+-rw-r--r--   0        0        0     2209 1970-01-01 00:00:00.000000 biglist-0.7.9b3/PKG-INFO
```

### Comparing `biglist-0.7.9b2/LICENSE` & `biglist-0.7.9b3/LICENSE`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b2/README.rst` & `biglist-0.7.9b3/README.rst`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b2/pyproject.toml` & `biglist-0.7.9b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 lz4 = ["lz4"]
 doc = [
     "sphinx",
     "numpydoc",
     "pydata-sphinx-theme",
 ]
 gcs = [
-    "upathlib[gcs] >= 0.7.3b1",
+    "upathlib[gcs] >= 0.7.7b1",
     "google-auth",
 ]
 parquet = []
 test = [
     "boltons",
     "mypy",
     "ruff",
```

### Comparing `biglist-0.7.9b2/src/biglist/__init__.py` & `biglist-0.7.9b3/src/biglist/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 )
 from ._util import (
     Chain,
     Seq,
     Slicer,
 )
 
-__version__ = "0.7.9b2"
+__version__ = "0.7.9b3"
```

### Comparing `biglist-0.7.9b2/src/biglist/_base.py` & `biglist-0.7.9b3/src/biglist/_base.py`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b2/src/biglist/_biglist.py` & `biglist-0.7.9b3/src/biglist/_biglist.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,15 @@
                         with lock_to_use(self._info_file) as ff:
                             ff.write_json(self.info, overwrite=True)
 
     def __del__(self) -> None:
         if getattr(self, "keep_files", True) is False:
             self.destroy(concurrent=False)
         else:
-            if not self._flushed:
+            if not getattr(self, '_flushed', True):
                 warnings.warn(
                     f"did you forget to flush {self.__class__.__name__} at '{self.path}'?"
                 )
             self.flush()
 
     @property
     def batch_size(self) -> int:
```

### Comparing `biglist-0.7.9b2/src/biglist/_parquet.py` & `biglist-0.7.9b3/src/biglist/_parquet.py`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b2/src/biglist/_util.py` & `biglist-0.7.9b3/src/biglist/_util.py`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b2/PKG-INFO` & `biglist-0.7.9b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biglist
-Version: 0.7.9b2
+Version: 0.7.9b3
 Summary: The package `biglist <https://github.com/zpz/biglist>`_ provides persisted, out-of-memory Python data structures
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -12,15 +12,15 @@
 Requires-Dist: deprecation
 Requires-Dist: mpservice >= 0.11.9
 Requires-Dist: pyarrow >= 10.0.0
 Requires-Dist: typing-extensions
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: numpydoc ; extra == "doc"
 Requires-Dist: pydata-sphinx-theme ; extra == "doc"
-Requires-Dist: upathlib[gcs] >= 0.7.3b1 ; extra == "gcs"
+Requires-Dist: upathlib[gcs] >= 0.7.7b1 ; extra == "gcs"
 Requires-Dist: google-auth ; extra == "gcs"
 Requires-Dist: lz4 ; extra == "lz4"
 Requires-Dist: boltons ; extra == "test"
 Requires-Dist: mypy ; extra == "test"
 Requires-Dist: ruff ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: zstandard ; extra == "zstandard"
```

