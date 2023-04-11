# Comparing `tmp/medvedi-0.1.8.tar.gz` & `tmp/medvedi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medvedi-0.1.8.tar", last modified: Fri Mar 10 18:53:33 2023, max compression
+gzip compressed data, was "medvedi-0.1.9.tar", last modified: Fri Mar 10 18:57:23 2023, max compression
```

## Comparing `medvedi-0.1.8.tar` & `medvedi-0.1.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 18:53:33.583276 medvedi-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-10 18:53:10.000000 medvedi-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-10 18:53:33.583276 medvedi-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-10 18:53:10.000000 medvedi-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 18:53:33.579276 medvedi-0.1.8/medvedi/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/accelerators.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    31457 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    29799 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/io.pyx
--rwxr-xr-x   0 runner    (1001) docker     (123)   640792 2023-03-09 14:28:00.000000 medvedi-0.1.8/medvedi/libmimalloc.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   640792 2023-03-09 14:28:00.000000 medvedi-0.1.8/medvedi/libmimalloc.so.2
--rwxr-xr-x   0 runner    (1001) docker     (123)   640792 2023-03-09 14:28:00.000000 medvedi-0.1.8/medvedi/libmimalloc.so.2.0
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/merge_to_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    34811 2023-03-09 14:28:00.000000 medvedi-0.1.8/medvedi/mimalloc.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 18:53:33.583276 medvedi-0.1.8/medvedi/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/native/chunked_stream.h
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/native/chunked_stream.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/native/cpython.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/native/mi_heap_destroy_stl_allocator.h
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/native/mi_heap_destroy_stl_allocator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/native/mi_heap_destroy_stl_allocator.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/native/numpy.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/native/optional.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    50378 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/native/sorted_intersection.h
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/native/string_view.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/native/utf8.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/pure_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-10 18:53:10.000000 medvedi-0.1.8/medvedi/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 18:53:33.579276 medvedi-0.1.8/medvedi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-10 18:53:33.000000 medvedi-0.1.8/medvedi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-10 18:53:33.000000 medvedi-0.1.8/medvedi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 18:53:33.000000 medvedi-0.1.8/medvedi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-10 18:53:33.000000 medvedi-0.1.8/medvedi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-10 18:53:33.000000 medvedi-0.1.8/medvedi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-10 18:53:10.000000 medvedi-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-10 18:53:10.000000 medvedi-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 18:53:33.583276 medvedi-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-03-10 18:53:10.000000 medvedi-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 18:57:23.519535 medvedi-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-10 18:57:01.000000 medvedi-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-10 18:57:23.519535 medvedi-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-10 18:57:01.000000 medvedi-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 18:57:23.515535 medvedi-0.1.9/medvedi/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/accelerators.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    31992 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29799 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/io.pyx
+-rwxr-xr-x   0 runner    (1001) docker     (123)   640792 2023-03-09 14:28:00.000000 medvedi-0.1.9/medvedi/libmimalloc.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   640792 2023-03-09 14:28:00.000000 medvedi-0.1.9/medvedi/libmimalloc.so.2
+-rwxr-xr-x   0 runner    (1001) docker     (123)   640792 2023-03-09 14:28:00.000000 medvedi-0.1.9/medvedi/libmimalloc.so.2.0
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/merge_to_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34811 2023-03-09 14:28:00.000000 medvedi-0.1.9/medvedi/mimalloc.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 18:57:23.519535 medvedi-0.1.9/medvedi/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/native/chunked_stream.h
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/native/chunked_stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/native/cpython.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/native/mi_heap_destroy_stl_allocator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/native/mi_heap_destroy_stl_allocator.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/native/mi_heap_destroy_stl_allocator.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/native/numpy.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/native/optional.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    50378 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/native/sorted_intersection.h
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/native/string_view.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/native/utf8.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/pure_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-10 18:57:01.000000 medvedi-0.1.9/medvedi/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 18:57:23.515535 medvedi-0.1.9/medvedi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-10 18:57:23.000000 medvedi-0.1.9/medvedi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-10 18:57:23.000000 medvedi-0.1.9/medvedi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 18:57:23.000000 medvedi-0.1.9/medvedi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-10 18:57:23.000000 medvedi-0.1.9/medvedi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-10 18:57:23.000000 medvedi-0.1.9/medvedi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-10 18:57:01.000000 medvedi-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-10 18:57:01.000000 medvedi-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 18:57:23.519535 medvedi-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-03-10 18:57:01.000000 medvedi-0.1.9/setup.py
```

### Comparing `medvedi-0.1.8/LICENSE` & `medvedi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/PKG-INFO` & `medvedi-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medvedi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Memory Efficient Deconstructed Vectorized Dataframe Interface
 Home-page: https://github.com/athenianco/medvedi
 Download-URL: https://github.com/athenianco/medvedi
 Author: Athenian
 Author-email: vadim@athenian.co
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `medvedi-0.1.8/README.md` & `medvedi-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/accelerators.pyx` & `medvedi-0.1.9/medvedi/accelerators.pyx`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/dataframe.py` & `medvedi-0.1.9/medvedi/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,30 @@
         array([ 9, 13, 27])
         """
         indexes = np.empty(len(self.counts), dtype=int)
         indexes[0] = 0
         np.cumsum(self.counts[:-1], out=indexes[1:])
         return indexes
 
+    def group_indexes(self) -> npt.NDArray[np.int_]:
+        """
+        Calculate the group key indexes.
+
+        Usage:
+        >>> df = DataFrame({"a": [1, 1, 2, 2, 3, 3, 3], "b": [4, 5, 6, 7, 8, 9, 10]})
+        >>> df.groupby("a").group_indexes()
+        array([0, 2, 4])
+        >>> df["a"][df.groupby("a").group_indexes()]
+        array([1, 2, 3])
+        """
+        indexes = np.empty(len(self.counts), dtype=int)
+        indexes[0] = 0
+        np.cumsum(self.counts[:-1], out=indexes[1:])
+        return self.order[indexes]
+
     def __iter__(self):
         """
         Iterate over indexes of each group.
 
         This is lightweight and avoids materializing column chunks.
 
         Usage:
```

### Comparing `medvedi-0.1.8/medvedi/io.pyx` & `medvedi-0.1.9/medvedi/io.pyx`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/libmimalloc.so` & `medvedi-0.1.9/medvedi/libmimalloc.so`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/libmimalloc.so.2` & `medvedi-0.1.9/medvedi/libmimalloc.so.2`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/libmimalloc.so.2.0` & `medvedi-0.1.9/medvedi/libmimalloc.so.2.0`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/merge_to_str.py` & `medvedi-0.1.9/medvedi/merge_to_str.py`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/mimalloc.h` & `medvedi-0.1.9/medvedi/mimalloc.h`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/native/chunked_stream.h` & `medvedi-0.1.9/medvedi/native/chunked_stream.h`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/native/cpython.pxd` & `medvedi-0.1.9/medvedi/native/cpython.pxd`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/native/mi_heap_destroy_stl_allocator.h` & `medvedi-0.1.9/medvedi/native/mi_heap_destroy_stl_allocator.h`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/native/mi_heap_destroy_stl_allocator.pxd` & `medvedi-0.1.9/medvedi/native/mi_heap_destroy_stl_allocator.pxd`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/native/mi_heap_destroy_stl_allocator.pyx` & `medvedi-0.1.9/medvedi/native/mi_heap_destroy_stl_allocator.pyx`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/native/numpy.pxd` & `medvedi-0.1.9/medvedi/native/numpy.pxd`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/native/optional.pxd` & `medvedi-0.1.9/medvedi/native/optional.pxd`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/native/sorted_intersection.h` & `medvedi-0.1.9/medvedi/native/sorted_intersection.h`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/native/utf8.pxd` & `medvedi-0.1.9/medvedi/native/utf8.pxd`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/pure_static.py` & `medvedi-0.1.9/medvedi/pure_static.py`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi/testing.py` & `medvedi-0.1.9/medvedi/testing.py`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/medvedi.egg-info/PKG-INFO` & `medvedi-0.1.9/medvedi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medvedi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Memory Efficient Deconstructed Vectorized Dataframe Interface
 Home-page: https://github.com/athenianco/medvedi
 Download-URL: https://github.com/athenianco/medvedi
 Author: Athenian
 Author-email: vadim@athenian.co
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `medvedi-0.1.8/medvedi.egg-info/SOURCES.txt` & `medvedi-0.1.9/medvedi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/pyproject.toml` & `medvedi-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `medvedi-0.1.8/setup.py` & `medvedi-0.1.9/setup.py`

 * *Files identical despite different names*

