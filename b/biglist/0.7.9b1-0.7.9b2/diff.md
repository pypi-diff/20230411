# Comparing `tmp/biglist-0.7.9b1.tar.gz` & `tmp/biglist-0.7.9b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biglist-0.7.9b1.tar", last modified: Mon Apr 10 09:32:11 2023, max compression
+gzip compressed data, was "biglist-0.7.9b2.tar", last modified: Mon Apr 10 23:43:11 2023, max compression
```

## Comparing `biglist-0.7.9b1.tar` & `biglist-0.7.9b2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.7.9b1/LICENSE
--rw-r--r--   0        0        0      931 2023-03-22 00:51:16.691348 biglist-0.7.9b1/README.rst
--rw-r--r--   0        0        0     1684 2023-04-10 09:18:54.169355 biglist-0.7.9b1/pyproject.toml
--rw-r--r--   0        0        0     2217 2023-04-10 09:19:33.793840 biglist-0.7.9b1/src/biglist/__init__.py
--rw-r--r--   0        0        0    18415 2023-04-10 09:27:34.589743 biglist-0.7.9b1/src/biglist/_base.py
--rw-r--r--   0        0        0    45513 2023-04-10 09:27:34.429899 biglist-0.7.9b1/src/biglist/_biglist.py
--rw-r--r--   0        0        0    33751 2023-03-30 06:44:24.186176 biglist-0.7.9b1/src/biglist/_parquet.py
--rw-r--r--   0        0        0    12025 2023-03-30 06:41:51.563305 biglist-0.7.9b1/src/biglist/_util.py
--rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.7.9b1/src/biglist/py.typed
--rw-r--r--   0        0        0     2273 1970-01-01 00:00:00.000000 biglist-0.7.9b1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.7.9b2/LICENSE
+-rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.7.9b2/README.rst
+-rw-r--r--   0        0        0     1628 2023-04-10 23:37:10.541736 biglist-0.7.9b2/pyproject.toml
+-rw-r--r--   0        0        0     2217 2023-04-10 23:37:43.212858 biglist-0.7.9b2/src/biglist/__init__.py
+-rw-r--r--   0        0        0    18415 2023-04-10 09:40:14.847560 biglist-0.7.9b2/src/biglist/_base.py
+-rw-r--r--   0        0        0    43804 2023-04-10 23:41:15.207783 biglist-0.7.9b2/src/biglist/_biglist.py
+-rw-r--r--   0        0        0    33751 2023-04-10 09:40:14.847560 biglist-0.7.9b2/src/biglist/_parquet.py
+-rw-r--r--   0        0        0    12025 2023-04-10 09:40:14.847560 biglist-0.7.9b2/src/biglist/_util.py
+-rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.7.9b2/src/biglist/py.typed
+-rw-r--r--   0        0        0     2209 1970-01-01 00:00:00.000000 biglist-0.7.9b2/PKG-INFO
```

### Comparing `biglist-0.7.9b1/LICENSE` & `biglist-0.7.9b2/LICENSE`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b1/README.rst` & `biglist-0.7.9b2/README.rst`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b1/src/biglist/__init__.py` & `biglist-0.7.9b2/src/biglist/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 )
 from ._util import (
     Chain,
     Seq,
     Slicer,
 )
 
-__version__ = "0.7.9b1"
+__version__ = "0.7.9b2"
```

### Comparing `biglist-0.7.9b1/src/biglist/_base.py` & `biglist-0.7.9b2/src/biglist/_base.py`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b1/src/biglist/_biglist.py` & `biglist-0.7.9b2/src/biglist/_biglist.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from typing import (
     Any,
     Callable,
     Optional,
 )
 from uuid import uuid4
 
-import orjson
 import pyarrow
 from typing_extensions import Self
 from upathlib import serializer
 
 from ._base import (
     BiglistBase,
     Element,
@@ -799,36 +798,14 @@
         return json.dumps(x, **kwargs).encode()
 
     @classmethod
     def deserialize(cls, y, **kwargs):
         return serializer._loads(json.loads, y.decode(), **kwargs)
 
 
-class OrjsonSerializer(serializer.ByteSerializer):
-    @classmethod
-    def serialize(cls, x, **kwargs):
-        return orjson.dumps(x, **kwargs)  # pylint: disable=no-member
-
-    @classmethod
-    def deserialize(cls, y):
-        return serializer._loads(orjson.loads, y)  # pylint: disable=no-member
-
-
-class ZOrjsonSerializer(OrjsonSerializer):
-    @classmethod
-    def serialize(cls, x, *, level=serializer.ZLIB_LEVEL, **kwargs):
-        y = super().serialize(x, **kwargs)
-        return serializer.z_compress(y, level=level)
-
-    @classmethod
-    def deserialize(cls, y):
-        y = serializer.z_decompress(y)
-        return super().deserialize(y)
-
-
 class ParquetSerializer(serializer.ByteSerializer):
     @classmethod
     def serialize(
         cls,
         x: list[dict],
         schema: pyarrow.Schema = None,
         schema_spec: Sequence = None,
@@ -890,51 +867,23 @@
         table = pyarrow.parquet.ParquetFile(y, **kwargs).read()
         return table.to_pylist()
 
 
 Biglist.register_storage_format("json", JsonByteSerializer)
 Biglist.register_storage_format("pickle", serializer.PickleSerializer)
 Biglist.register_storage_format("pickle-z", serializer.ZPickleSerializer)
-Biglist.register_storage_format("orjson", OrjsonSerializer)
-Biglist.register_storage_format("orjson-z", ZOrjsonSerializer)
 Biglist.register_storage_format("parquet", ParquetSerializer)
 
 
-if hasattr(serializer, 'zstd_compress'):
-
-    class ZstdOrjsonSerializer(OrjsonSerializer):
-        @classmethod
-        def serialize(cls, x, *, level=serializer.ZSTD_LEVEL, **kwargs):
-            y = super().serialize(x, **kwargs)
-            return serializer.zstd_compress(y, level=level)
-
-        @classmethod
-        def deserialize(cls, y):
-            y = serializer.zstd_decompress(y)
-            return super().deserialize(y)
-
+if hasattr(serializer, 'ZstdPickleSerializer'):
     Biglist.register_storage_format("pickle-zstd", serializer.ZstdPickleSerializer)
-    Biglist.register_storage_format("orjson-zstd", ZstdOrjsonSerializer)
-
-
-if hasattr(serializer, 'lz4_compress'):
-
-    class Lz4OrjsonSerializer(OrjsonSerializer):
-        @classmethod
-        def serialize(cls, x, *, level=serializer.LZ4_LEVEL, **kwargs):
-            y = super().serialize(x, **kwargs)
-            return serializer.lz4_compress(y, level=level)
 
-        @classmethod
-        def deserialize(cls, y):
-            y = serializer.lz4_decompress(y)
-            return super().deserialize(y)
 
+if hasattr(serializer, 'Lz4PickleSerializer'):
     Biglist.register_storage_format("pickle-lz4", serializer.Lz4PickleSerializer)
-    Biglist.register_storage_format("orjson-lz4", Lz4OrjsonSerializer)
 
 
 class Multiplexer:
     """
     Multiplexer is used to distribute data elements to multiple "workers" so that
     each element is obtained by exactly one worker.
```

### Comparing `biglist-0.7.9b1/src/biglist/_parquet.py` & `biglist-0.7.9b2/src/biglist/_parquet.py`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b1/src/biglist/_util.py` & `biglist-0.7.9b2/src/biglist/_util.py`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b1/PKG-INFO` & `biglist-0.7.9b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: biglist
-Version: 0.7.9b1
+Version: 0.7.9b2
 Summary: The package `biglist <https://github.com/zpz/biglist>`_ provides persisted, out-of-memory Python data structures
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: upathlib >= 0.7.7b1
 Requires-Dist: deprecation
 Requires-Dist: mpservice >= 0.11.9
-Requires-Dist: orjson
 Requires-Dist: pyarrow >= 10.0.0
 Requires-Dist: typing-extensions
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: numpydoc ; extra == "doc"
 Requires-Dist: pydata-sphinx-theme ; extra == "doc"
 Requires-Dist: upathlib[gcs] >= 0.7.3b1 ; extra == "gcs"
 Requires-Dist: google-auth ; extra == "gcs"
-Requires-Dist: upathlib[lz4] >= 0.7.7b1 ; extra == "lz4"
+Requires-Dist: lz4 ; extra == "lz4"
 Requires-Dist: boltons ; extra == "test"
 Requires-Dist: mypy ; extra == "test"
 Requires-Dist: ruff ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
-Requires-Dist: upathlib[zstandard] >= 0.7.7b1 ; extra == "zstandard"
+Requires-Dist: zstandard ; extra == "zstandard"
 Project-URL: Source, https://github.com/zpz/biglist
 Provides-Extra: doc
 Provides-Extra: gcs
 Provides-Extra: lz4
 Provides-Extra: parquet
 Provides-Extra: test
 Provides-Extra: zstandard
```

