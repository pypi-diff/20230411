# Comparing `tmp/ewoksdata-0.2.1.tar.gz` & `tmp/ewoksdata-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksdata-0.2.1.tar", last modified: Sun Apr  2 15:35:00 2023, max compression
+gzip compressed data, was "dist/ewoksdata-0.2.2.tar", last modified: Tue Apr 11 17:32:32 2023, max compression
```

## Comparing `ewoksdata-0.2.1.tar` & `ewoksdata-0.2.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 15:35:00.000000 ewoksdata-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-02 15:35:00.000000 ewoksdata-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-04-02 15:35:00.000000 ewoksdata-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 15:35:00.000000 ewoksdata-0.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 15:35:00.000000 ewoksdata-0.2.1/src/ewoksdata/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-02 15:33:17.000000 ewoksdata-0.2.1/src/ewoksdata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 15:35:00.000000 ewoksdata-0.2.1/src/ewoksdata/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-02 15:34:54.000000 ewoksdata-0.2.1/src/ewoksdata/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5265 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/src/ewoksdata/data/bliss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 15:35:00.000000 ewoksdata-0.2.1/src/ewoksdata/data/hdf5/
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/src/ewoksdata/data/hdf5/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6085 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/src/ewoksdata/data/hdf5/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/src/ewoksdata/data/hdf5/dataset_writer.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/src/ewoksdata/data/hdf5/types.py
--rw-rw-rw-   0 root         (0) root         (0)     1710 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/src/ewoksdata/data/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/src/ewoksdata/data/url.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/src/ewoksdata/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 15:35:00.000000 ewoksdata-0.2.1/src/ewoksdata/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-02 15:34:54.000000 ewoksdata-0.2.1/src/ewoksdata/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/src/ewoksdata/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 15:35:00.000000 ewoksdata-0.2.1/src/ewoksdata/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/src/ewoksdata/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3468 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/src/ewoksdata/tests/data/bliss_scans.py
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/src/ewoksdata/tests/test_data_bliss.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/src/ewoksdata/tests/test_data_hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)      570 2023-04-02 11:03:12.000000 ewoksdata-0.2.1/src/ewoksdata/tests/test_dataset_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 15:35:00.000000 ewoksdata-0.2.1/src/ewoksdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-02 15:35:00.000000 ewoksdata-0.2.1/src/ewoksdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      811 2023-04-02 15:35:00.000000 ewoksdata-0.2.1/src/ewoksdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 15:35:00.000000 ewoksdata-0.2.1/src/ewoksdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-04-02 15:35:00.000000 ewoksdata-0.2.1/src/ewoksdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-02 15:35:00.000000 ewoksdata-0.2.1/src/ewoksdata.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-11 17:31:40.000000 ewoksdata-0.2.2/src/ewoksdata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 17:32:26.000000 ewoksdata-0.2.2/src/ewoksdata/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5265 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/data/bliss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata/data/hdf5/
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-04-11 17:28:37.000000 ewoksdata-0.2.2/src/ewoksdata/data/hdf5/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6085 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/data/hdf5/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3373 2023-04-11 17:28:37.000000 ewoksdata-0.2.2/src/ewoksdata/data/hdf5/dataset_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/data/hdf5/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3057 2023-04-11 17:28:37.000000 ewoksdata-0.2.2/src/ewoksdata/data/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/data/url.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 17:32:26.000000 ewoksdata-0.2.2/src/ewoksdata/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3468 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/tests/data/bliss_scans.py
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/tests/test_data_bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/tests/test_data_hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-11 17:28:37.000000 ewoksdata-0.2.2/src/ewoksdata/tests/test_data_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)      570 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/tests/test_dataset_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata.egg-info/top_level.txt
```

### Comparing `ewoksdata-0.2.1/LICENSE.md` & `ewoksdata-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.1/PKG-INFO` & `ewoksdata-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdata
-Version: 0.2.1
+Version: 0.2.2
 Summary: Ewoks tasks for data access
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Project-URL: Documentation, https://ewoksdata.readthedocs.io
```

### Comparing `ewoksdata-0.2.1/setup.cfg` & `ewoksdata-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.1/src/ewoksdata/data/bliss.py` & `ewoksdata-0.2.2/src/ewoksdata/data/bliss.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.1/src/ewoksdata/data/hdf5/config.py` & `ewoksdata-0.2.2/src/ewoksdata/data/hdf5/config.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.1/src/ewoksdata/data/hdf5/dataset_writer.py` & `ewoksdata-0.2.2/src/ewoksdata/data/hdf5/dataset_writer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,91 +1,106 @@
 from typing import Optional
+
 import h5py
+import numpy
 from numpy.typing import ArrayLike
+
 from .types import StrictPositiveIntegral
 from .config import guess_dataset_config
 
 
 class DatasetWriter:
     def __init__(
         self,
         parent: h5py.Group,
         name: str,
         npoints: Optional[StrictPositiveIntegral] = None,
+        attrs: Optional[dict] = None,
     ) -> None:
         self._parent = parent
         self._name = name
+        self._attrs = attrs
         self._dataset_name = f"{parent.name}/{name}"
         self._dataset = None
         self._buffer = list()
+        self._npoints_added = 0
         self._npoints = npoints
         self._npoints_chunk = None
         self._dataset_idx = 0
 
     @property
-    def dataset_name(self):
+    def dataset_name(self) -> str:
         return self._dataset_name
 
-    def __enter__(self):
+    def __enter__(self) -> "DatasetWriter":
         return self
 
-    def __exit__(self, *args):
+    def __exit__(self, *args) -> None:
         self.flush_buffer()
 
     @property
     def dataset(self) -> Optional[h5py.Dataset]:
         return self._dataset
 
-    def _create_dataset(self, first_data_point):
+    def _create_dataset(self, first_data_point: numpy.ndarray) -> h5py.Dataset:
         scan_shape = (self._npoints,)
         detector_shape = first_data_point.shape
         dtype = first_data_point.dtype
         if self._npoints is None:
             max_shape = scan_shape + detector_shape
             shape = (1,) + first_data_point.shape
         else:
             max_shape = None
-            shape = scan_shape
+            shape = scan_shape + first_data_point.shape
 
         options = guess_dataset_config(
             scan_shape, detector_shape, dtype=dtype, max_shape=max_shape
         )
         options["shape"] = shape
         options["dtype"] = dtype
+        options["fillvalue"] = numpy.nan  # converts to 0 for integers
         if max_shape:
             options["maxshape"] = max_shape
-
         if options["chunks"]:
             self._npoints_chunk = options["chunks"][0]
         else:
             self._npoints_chunk = 0
-        return self._parent.create_dataset(self._name, **options)
+        dset = self._parent.create_dataset(self._name, **options)
+        if self._attrs:
+            dset.attrs.update(self._attrs)
+        return dset
+
+    @property
+    def npoints_added(self) -> int:
+        return self._npoints_added
 
     def add_point(self, data: ArrayLike) -> bool:
         if self._dataset is None:
             self._dataset = self._create_dataset(data)
         self._buffer.append(data)
+        self._npoints_added += 1
         return self.flush_buffer(align=True)
 
     def add_points(self, data: ArrayLike) -> bool:
         if self._dataset is None:
             self._dataset = self._create_dataset(data[0])
         self._buffer.extend(data)
+        self._npoints_added += len(data)
         return self.flush_buffer(align=True)
 
     def flush_buffer(self, align: bool = False) -> bool:
         nbuffer = len(self._buffer)
-        if align:
+        if align and self._npoints_chunk:
             nflush = nbuffer // self._npoints_chunk * self._npoints_chunk
         else:
             nflush = nbuffer
         if nflush == 0:
             return False
         npoints0 = self._dataset.shape[0]
         istart = self._dataset_idx
         npoints1 = istart + nflush
-        if npoints1 > npoints0:
+        if self._npoints_chunk and npoints1 > npoints0:
             self._dataset.resize(npoints1, axis=0)
         self._dataset[istart : istart + nflush] = self._buffer[:nflush]
         self._buffer = self._buffer[nflush:]
         self._dataset_idx += nflush
         return True
```

### Comparing `ewoksdata-0.2.1/src/ewoksdata/data/utils.py` & `ewoksdata-0.2.2/src/ewoksdata/data/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.1/src/ewoksdata/tests/data/bliss_scans.py` & `ewoksdata-0.2.2/src/ewoksdata/tests/data/bliss_scans.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.1/src/ewoksdata/tests/test_data_bliss.py` & `ewoksdata-0.2.2/src/ewoksdata/tests/test_data_bliss.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.1/src/ewoksdata/tests/test_dataset_writer.py` & `ewoksdata-0.2.2/src/ewoksdata/tests/test_dataset_writer.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.1/src/ewoksdata.egg-info/PKG-INFO` & `ewoksdata-0.2.2/src/ewoksdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdata
-Version: 0.2.1
+Version: 0.2.2
 Summary: Ewoks tasks for data access
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Project-URL: Documentation, https://ewoksdata.readthedocs.io
```

### Comparing `ewoksdata-0.2.1/src/ewoksdata.egg-info/SOURCES.txt` & `ewoksdata-0.2.2/src/ewoksdata.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,10 +18,11 @@
 src/ewoksdata/data/hdf5/config.py
 src/ewoksdata/data/hdf5/dataset_writer.py
 src/ewoksdata/data/hdf5/types.py
 src/ewoksdata/tests/__init__.py
 src/ewoksdata/tests/conftest.py
 src/ewoksdata/tests/test_data_bliss.py
 src/ewoksdata/tests/test_data_hdf5.py
+src/ewoksdata/tests/test_data_nexus.py
 src/ewoksdata/tests/test_dataset_writer.py
 src/ewoksdata/tests/data/__init__.py
 src/ewoksdata/tests/data/bliss_scans.py
```

