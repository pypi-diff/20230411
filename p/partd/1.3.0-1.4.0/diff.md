# Comparing `tmp/partd-1.3.0.tar.gz` & `tmp/partd-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partd-1.3.0.tar", last modified: Thu Aug 11 23:22:05 2022, max compression
+gzip compressed data, was "partd-1.4.0.tar", last modified: Tue Apr 11 20:49:18 2023, max compression
```

## Comparing `partd-1.3.0.tar` & `partd-1.4.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2022-08-11 23:22:05.256542 partd-1.3.0/
--rw-r--r--   0 james      (501) staff       (20)     1505 2021-04-02 00:20:44.000000 partd-1.3.0/LICENSE.txt
--rw-r--r--   0 james      (501) staff       (20)      179 2021-04-02 00:20:51.000000 partd-1.3.0/MANIFEST.in
--rw-r--r--   0 james      (501) staff       (20)     4303 2022-08-11 23:22:05.256742 partd-1.3.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     3824 2021-04-02 00:20:51.000000 partd-1.3.0/README.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2022-08-11 23:22:05.258368 partd-1.3.0/partd/
--rw-r--r--   0 james      (501) staff       (20)      507 2021-10-21 20:59:21.000000 partd-1.3.0/partd/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      497 2022-08-11 23:22:05.258515 partd-1.3.0/partd/_version.py
--rw-r--r--   0 james      (501) staff       (20)     3628 2021-10-21 20:59:21.000000 partd-1.3.0/partd/buffer.py
--rw-r--r--   0 james      (501) staff       (20)     1174 2021-10-21 20:59:21.000000 partd-1.3.0/partd/compressed.py
--rw-r--r--   0 james      (501) staff       (20)     2259 2021-10-21 20:59:21.000000 partd-1.3.0/partd/core.py
--rw-r--r--   0 james      (501) staff       (20)     1701 2021-04-02 00:20:44.000000 partd-1.3.0/partd/dict.py
--rw-r--r--   0 james      (501) staff       (20)     1287 2021-04-02 00:20:44.000000 partd-1.3.0/partd/encode.py
--rw-r--r--   0 james      (501) staff       (20)     3954 2021-10-21 20:59:21.000000 partd-1.3.0/partd/file.py
--rw-r--r--   0 james      (501) staff       (20)     4181 2021-10-21 20:59:21.000000 partd-1.3.0/partd/numpy.py
--rw-r--r--   0 james      (501) staff       (20)     7031 2022-08-11 23:16:45.000000 partd-1.3.0/partd/pandas.py
--rw-r--r--   0 james      (501) staff       (20)      360 2021-10-21 20:59:21.000000 partd-1.3.0/partd/pickle.py
--rw-r--r--   0 james      (501) staff       (20)      902 2021-10-21 20:59:21.000000 partd-1.3.0/partd/python.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2022-08-11 23:22:05.256081 partd-1.3.0/partd/tests/
--rw-r--r--   0 james      (501) staff       (20)     1560 2021-04-02 00:20:44.000000 partd-1.3.0/partd/tests/test_buffer.py
--rw-r--r--   0 james      (501) staff       (20)      734 2021-04-02 00:20:44.000000 partd-1.3.0/partd/tests/test_compressed.py
--rw-r--r--   0 james      (501) staff       (20)      940 2021-04-02 00:20:44.000000 partd-1.3.0/partd/tests/test_dict.py
--rw-r--r--   0 james      (501) staff       (20)      700 2021-04-02 00:20:44.000000 partd-1.3.0/partd/tests/test_encode.py
--rw-r--r--   0 james      (501) staff       (20)     1800 2021-04-02 00:20:44.000000 partd-1.3.0/partd/tests/test_file.py
--rw-r--r--   0 james      (501) staff       (20)     2307 2021-10-21 20:59:21.000000 partd-1.3.0/partd/tests/test_numpy.py
--rw-r--r--   0 james      (501) staff       (20)     3934 2022-08-05 21:19:42.000000 partd-1.3.0/partd/tests/test_pandas.py
--rw-r--r--   0 james      (501) staff       (20)     1281 2021-04-02 00:20:44.000000 partd-1.3.0/partd/tests/test_partd.py
--rw-r--r--   0 james      (501) staff       (20)      762 2021-04-02 00:20:44.000000 partd-1.3.0/partd/tests/test_pickle.py
--rw-r--r--   0 james      (501) staff       (20)      248 2021-04-02 00:20:44.000000 partd-1.3.0/partd/tests/test_python.py
--rw-r--r--   0 james      (501) staff       (20)      258 2021-04-02 00:20:44.000000 partd-1.3.0/partd/tests/test_utils.py
--rw-r--r--   0 james      (501) staff       (20)     3335 2021-10-21 20:59:21.000000 partd-1.3.0/partd/tests/test_zmq.py
--rw-r--r--   0 james      (501) staff       (20)     3603 2021-10-21 20:59:21.000000 partd-1.3.0/partd/utils.py
--rw-r--r--   0 james      (501) staff       (20)     9578 2021-10-21 20:59:21.000000 partd-1.3.0/partd/zmq.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2022-08-11 23:22:05.249780 partd-1.3.0/partd.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     4303 2022-08-11 23:22:04.000000 partd-1.3.0/partd.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      795 2022-08-11 23:22:05.000000 partd-1.3.0/partd.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2022-08-11 23:22:04.000000 partd-1.3.0/partd.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2022-08-11 23:22:04.000000 partd-1.3.0/partd.egg-info/not-zip-safe
--rw-r--r--   0 james      (501) staff       (20)       65 2022-08-11 23:22:05.000000 partd-1.3.0/partd.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)        6 2022-08-11 23:22:05.000000 partd-1.3.0/partd.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       13 2021-04-02 00:20:44.000000 partd-1.3.0/requirements.txt
--rw-r--r--   0 james      (501) staff       (20)      194 2022-08-11 23:22:05.257659 partd-1.3.0/setup.cfg
--rwxr-xr-x   0 james      (501) staff       (20)     1055 2022-05-23 21:39:55.000000 partd-1.3.0/setup.py
--rw-r--r--   0 james      (501) staff       (20)    68607 2021-04-02 00:20:51.000000 partd-1.3.0/versioneer.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-11 20:49:18.793805 partd-1.4.0/
+-rw-r--r--   0 james      (501) staff       (20)     1505 2021-04-02 00:20:44.000000 partd-1.4.0/LICENSE.txt
+-rw-r--r--   0 james      (501) staff       (20)      179 2021-04-02 00:20:51.000000 partd-1.4.0/MANIFEST.in
+-rw-r--r--   0 james      (501) staff       (20)     4303 2023-04-11 20:49:18.794071 partd-1.4.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     3824 2021-04-02 00:20:51.000000 partd-1.4.0/README.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-11 20:49:18.795888 partd-1.4.0/partd/
+-rw-r--r--   0 james      (501) staff       (20)      507 2021-10-21 20:59:21.000000 partd-1.4.0/partd/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      497 2023-04-11 20:49:18.796062 partd-1.4.0/partd/_version.py
+-rw-r--r--   0 james      (501) staff       (20)     3628 2021-10-21 20:59:21.000000 partd-1.4.0/partd/buffer.py
+-rw-r--r--   0 james      (501) staff       (20)     1174 2021-10-21 20:59:21.000000 partd-1.4.0/partd/compressed.py
+-rw-r--r--   0 james      (501) staff       (20)     2259 2021-10-21 20:59:21.000000 partd-1.4.0/partd/core.py
+-rw-r--r--   0 james      (501) staff       (20)     1701 2021-04-02 00:20:44.000000 partd-1.4.0/partd/dict.py
+-rw-r--r--   0 james      (501) staff       (20)     1287 2021-04-02 00:20:44.000000 partd-1.4.0/partd/encode.py
+-rw-r--r--   0 james      (501) staff       (20)     3954 2021-10-21 20:59:21.000000 partd-1.4.0/partd/file.py
+-rw-r--r--   0 james      (501) staff       (20)     4181 2021-10-21 20:59:21.000000 partd-1.4.0/partd/numpy.py
+-rw-r--r--   0 james      (501) staff       (20)     7101 2023-04-11 19:53:52.000000 partd-1.4.0/partd/pandas.py
+-rw-r--r--   0 james      (501) staff       (20)      360 2021-10-21 20:59:21.000000 partd-1.4.0/partd/pickle.py
+-rw-r--r--   0 james      (501) staff       (20)      902 2021-10-21 20:59:21.000000 partd-1.4.0/partd/python.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-11 20:49:18.792831 partd-1.4.0/partd/tests/
+-rw-r--r--   0 james      (501) staff       (20)     1560 2021-04-02 00:20:44.000000 partd-1.4.0/partd/tests/test_buffer.py
+-rw-r--r--   0 james      (501) staff       (20)      734 2021-04-02 00:20:44.000000 partd-1.4.0/partd/tests/test_compressed.py
+-rw-r--r--   0 james      (501) staff       (20)      940 2021-04-02 00:20:44.000000 partd-1.4.0/partd/tests/test_dict.py
+-rw-r--r--   0 james      (501) staff       (20)      700 2021-04-02 00:20:44.000000 partd-1.4.0/partd/tests/test_encode.py
+-rw-r--r--   0 james      (501) staff       (20)     1800 2021-04-02 00:20:44.000000 partd-1.4.0/partd/tests/test_file.py
+-rw-r--r--   0 james      (501) staff       (20)     2307 2021-10-21 20:59:21.000000 partd-1.4.0/partd/tests/test_numpy.py
+-rw-r--r--   0 james      (501) staff       (20)     4849 2023-03-17 15:40:45.000000 partd-1.4.0/partd/tests/test_pandas.py
+-rw-r--r--   0 james      (501) staff       (20)     1281 2021-04-02 00:20:44.000000 partd-1.4.0/partd/tests/test_partd.py
+-rw-r--r--   0 james      (501) staff       (20)      762 2021-04-02 00:20:44.000000 partd-1.4.0/partd/tests/test_pickle.py
+-rw-r--r--   0 james      (501) staff       (20)      248 2021-04-02 00:20:44.000000 partd-1.4.0/partd/tests/test_python.py
+-rw-r--r--   0 james      (501) staff       (20)      258 2021-04-02 00:20:44.000000 partd-1.4.0/partd/tests/test_utils.py
+-rw-r--r--   0 james      (501) staff       (20)     3335 2021-10-21 20:59:21.000000 partd-1.4.0/partd/tests/test_zmq.py
+-rw-r--r--   0 james      (501) staff       (20)     3603 2021-10-21 20:59:21.000000 partd-1.4.0/partd/utils.py
+-rw-r--r--   0 james      (501) staff       (20)     9578 2021-10-21 20:59:21.000000 partd-1.4.0/partd/zmq.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-11 20:49:18.781684 partd-1.4.0/partd.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     4303 2023-04-11 20:49:18.000000 partd-1.4.0/partd.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      795 2023-04-11 20:49:18.000000 partd-1.4.0/partd.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-04-11 20:49:18.000000 partd-1.4.0/partd.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-04-11 20:49:18.000000 partd-1.4.0/partd.egg-info/not-zip-safe
+-rw-r--r--   0 james      (501) staff       (20)       65 2023-04-11 20:49:18.000000 partd-1.4.0/partd.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)        6 2023-04-11 20:49:18.000000 partd-1.4.0/partd.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       13 2021-04-02 00:20:44.000000 partd-1.4.0/requirements.txt
+-rw-r--r--   0 james      (501) staff       (20)      194 2023-04-11 20:49:18.795264 partd-1.4.0/setup.cfg
+-rwxr-xr-x   0 james      (501) staff       (20)     1055 2022-05-23 21:39:55.000000 partd-1.4.0/setup.py
+-rw-r--r--   0 james      (501) staff       (20)    68607 2021-04-02 00:20:51.000000 partd-1.4.0/versioneer.py
```

### Comparing `partd-1.3.0/LICENSE.txt` & `partd-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/PKG-INFO` & `partd-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partd
-Version: 1.3.0
+Version: 1.4.0
 Summary: Appendable key-value storage
 Home-page: http://github.com/dask/partd/
 Maintainer: Matthew Rocklin
 Maintainer-email: mrocklin@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `partd-1.3.0/README.rst` & `partd-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/buffer.py` & `partd-1.4.0/partd/buffer.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/compressed.py` & `partd-1.4.0/partd/compressed.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/core.py` & `partd-1.4.0/partd/core.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/dict.py` & `partd-1.4.0/partd/dict.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/encode.py` & `partd-1.4.0/partd/encode.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/file.py` & `partd-1.4.0/partd/file.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/numpy.py` & `partd-1.4.0/partd/numpy.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/pandas.py` & `partd-1.4.0/partd/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,17 @@
     if isinstance(ind, pd.CategoricalIndex):
         cat = (ind.ordered, ind.categories)
         values = ind.codes
     else:
         cat = None
         values = ind.values
 
+    if is_extension_array_dtype(ind):
+        return None, dumps(ind)
+
     header = (type(ind), {k: getattr(ind, k, None) for k in ind._attributes}, values.dtype, cat)
     bytes = pnp.compress(pnp.serialize(values), values.dtype)
     return header, bytes
 
 
 def index_from_header_bytes(header, bytes):
     if header is None:
@@ -176,15 +179,15 @@
     Uses Pandas blocks, snappy, and blosc to deconstruct an array into bytes
     """
     col_header, col_bytes = index_to_header_bytes(df.columns)
     ind_header, ind_bytes = index_to_header_bytes(df.index)
     headers = [col_header, ind_header]
     bytes = [col_bytes, ind_bytes]
 
-    for block in df._data.blocks:
+    for block in df._mgr.blocks:
         h, b = block_to_header_bytes(block)
         headers.append(h)
         bytes.append(b)
 
     frames = [dumps(headers)] + bytes
     return b''.join(map(frame, frames))
```

### Comparing `partd-1.3.0/partd/python.py` & `partd-1.4.0/partd/python.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/tests/test_buffer.py` & `partd-1.4.0/partd/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/tests/test_compressed.py` & `partd-1.4.0/partd/tests/test_compressed.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/tests/test_dict.py` & `partd-1.4.0/partd/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/tests/test_encode.py` & `partd-1.4.0/partd/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/tests/test_file.py` & `partd-1.4.0/partd/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/tests/test_numpy.py` & `partd-1.4.0/partd/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/tests/test_pandas.py` & `partd-1.4.0/partd/tests/test_pandas.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 pytest.importorskip('pandas')  # noqa
 
 import numpy as np
 import pandas as pd
 import pandas.testing as tm
 import os
 
+try:
+    import pyarrow as pa
+except ImportError:
+    pa = None
+
 from partd.pandas import PandasColumns, PandasBlocks, serialize, deserialize
 
 
 df1 = pd.DataFrame({'a': [1, 2, 3],
                     'b': [1., 2., 3.],
                     'c': ['x', 'y', 'x']}, columns=['a', 'b', 'c'],
                     index=pd.Index([1, 2, 3], name='myindex'))
@@ -111,7 +116,33 @@
 
 def test_other_extension_types():
     pytest.importorskip("pandas", minversion="0.25.0")
     a = pd.array([pd.Period("2000"), pd.Period("2001")])
     df = pd.DataFrame({"A": a})
     df2 = deserialize(serialize(df))
     tm.assert_frame_equal(df, df2)
+
+@pytest.mark.parametrize("dtype", ["Int64", "Int32", "Float64", "Float32"])
+def test_index_numeric_extension_types(dtype):
+    pytest.importorskip("pandas", minversion="1.4.0")
+
+    df = pd.DataFrame({"x": [1, 2, 3]}, index=[4, 5, 6])
+    df.index = df.index.astype(dtype)
+    df2 = deserialize(serialize(df))
+    tm.assert_frame_equal(df, df2)
+    
+@pytest.mark.parametrize(
+    "dtype",
+    [
+        "string[python]",
+        pytest.param(
+            "string[pyarrow]",
+            marks=pytest.mark.skipif(pa is None, reason="Requires pyarrow"),
+        ),
+    ],
+)
+def test_index_non_numeric_extension_types(dtype):
+    pytest.importorskip("pandas", minversion="1.4.0")
+    df = pd.DataFrame({"x": [1, 2, 3]}, index=["a", "b", "c"])
+    df.index = df.index.astype(dtype)
+    df2 = deserialize(serialize(df))
+    tm.assert_frame_equal(df, df2)
```

### Comparing `partd-1.3.0/partd/tests/test_partd.py` & `partd-1.4.0/partd/tests/test_partd.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/tests/test_pickle.py` & `partd-1.4.0/partd/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/tests/test_zmq.py` & `partd-1.4.0/partd/tests/test_zmq.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/utils.py` & `partd-1.4.0/partd/utils.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd/zmq.py` & `partd-1.4.0/partd/zmq.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/partd.egg-info/PKG-INFO` & `partd-1.4.0/partd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partd
-Version: 1.3.0
+Version: 1.4.0
 Summary: Appendable key-value storage
 Home-page: http://github.com/dask/partd/
 Maintainer: Matthew Rocklin
 Maintainer-email: mrocklin@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `partd-1.3.0/partd.egg-info/SOURCES.txt` & `partd-1.4.0/partd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/setup.py` & `partd-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `partd-1.3.0/versioneer.py` & `partd-1.4.0/versioneer.py`

 * *Files identical despite different names*

