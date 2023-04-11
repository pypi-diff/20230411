# Comparing `tmp/anndata-0.9.0.tar.gz` & `tmp/anndata-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anndata-0.9.0.tar", last modified: Tue Apr 11 09:22:04 2023, max compression
+gzip compressed data, was "anndata-0.9.0rc1.tar", last modified: Tue Feb 21 16:28:58 2023, max compression
```

## Comparing `anndata-0.9.0.tar` & `anndata-0.9.0rc1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1544 2023-04-11 09:10:06.142630 anndata-0.9.0/LICENSE
--rw-r--r--   0        0        0     1901 2023-04-11 09:10:11.930300 anndata-0.9.0/README.md
--rw-r--r--   0        0        0      697 2023-04-11 09:10:06.142925 anndata-0.9.0/anndata/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 09:10:06.143030 anndata-0.9.0/anndata/_core/__init__.py
--rw-r--r--   0        0        0      818 2023-04-11 09:10:06.143156 anndata-0.9.0/anndata/_core/access.py
--rw-r--r--   0        0        0    11532 2023-04-11 09:10:06.143336 anndata-0.9.0/anndata/_core/aligned_mapping.py
--rw-r--r--   0        0        0    76595 2023-04-11 09:10:06.144196 anndata-0.9.0/anndata/_core/anndata.py
--rw-r--r--   0        0        0     3590 2023-04-11 09:10:06.144348 anndata-0.9.0/anndata/_core/file_backing.py
--rw-r--r--   0        0        0     7084 2023-04-11 09:10:06.144533 anndata-0.9.0/anndata/_core/index.py
--rw-r--r--   0        0        0    36304 2023-04-11 09:10:06.144873 anndata-0.9.0/anndata/_core/merge.py
--rw-r--r--   0        0        0     6836 2023-04-11 09:10:06.145065 anndata-0.9.0/anndata/_core/raw.py
--rw-r--r--   0        0        0    13269 2023-04-11 09:10:06.145253 anndata-0.9.0/anndata/_core/sparse_dataset.py
--rw-r--r--   0        0        0     9696 2023-04-11 09:10:06.145441 anndata-0.9.0/anndata/_core/views.py
--rw-r--r--   0        0        0      246 2023-04-11 09:10:06.145612 anndata-0.9.0/anndata/_io/__init__.py
--rw-r--r--   0        0        0    13086 2023-04-11 09:10:06.145854 anndata-0.9.0/anndata/_io/h5ad.py
--rw-r--r--   0        0        0    15794 2023-04-11 09:10:06.146055 anndata-0.9.0/anndata/_io/read.py
--rw-r--r--   0        0        0      111 2023-04-11 09:10:06.146232 anndata-0.9.0/anndata/_io/specs/__init__.py
--rw-r--r--   0        0        0    28569 2023-04-11 09:10:06.146471 anndata-0.9.0/anndata/_io/specs/methods.py
--rw-r--r--   0        0        0    11004 2023-04-11 09:10:11.930652 anndata-0.9.0/anndata/_io/specs/registry.py
--rw-r--r--   0        0        0     7780 2023-04-11 09:10:06.146830 anndata-0.9.0/anndata/_io/utils.py
--rw-r--r--   0        0        0     4602 2023-04-11 09:10:06.146973 anndata-0.9.0/anndata/_io/write.py
--rw-r--r--   0        0        0     4294 2023-04-11 09:10:06.147145 anndata-0.9.0/anndata/_io/zarr.py
--rw-r--r--   0        0        0     1312 2023-04-11 09:10:06.147287 anndata-0.9.0/anndata/_metadata.py
--rw-r--r--   0        0        0      436 2023-04-11 09:10:06.147393 anndata-0.9.0/anndata/_types.py
--rw-r--r--   0        0        0      695 2023-04-11 09:10:06.147508 anndata-0.9.0/anndata/_warnings.py
--rw-r--r--   0        0        0     9180 2023-04-11 09:10:06.147750 anndata-0.9.0/anndata/compat/__init__.py
--rw-r--r--   0        0        0      141 2023-04-11 09:10:06.147890 anndata-0.9.0/anndata/core.py
--rw-r--r--   0        0        0     3428 2023-04-11 09:10:06.148063 anndata-0.9.0/anndata/experimental/__init__.py
--rw-r--r--   0        0        0       42 2023-04-11 09:10:06.148221 anndata-0.9.0/anndata/experimental/multi_files/__init__.py
--rw-r--r--   0        0        0    34530 2023-04-11 09:10:06.148503 anndata-0.9.0/anndata/experimental/multi_files/_anncollection.py
--rw-r--r--   0        0        0       34 2023-04-11 09:10:06.148677 anndata-0.9.0/anndata/experimental/pytorch/__init__.py
--rw-r--r--   0        0        0     7097 2023-04-11 09:10:06.148822 anndata-0.9.0/anndata/experimental/pytorch/_annloader.py
--rw-r--r--   0        0        0     1429 2023-04-11 09:10:06.148954 anndata-0.9.0/anndata/logging.py
--rw-r--r--   0        0        0      144 2023-04-11 09:10:06.149047 anndata-0.9.0/anndata/readwrite.py
--rw-r--r--   0        0        0      101 2023-04-11 09:10:06.149197 anndata-0.9.0/anndata/tests/adata-comments.tsv
--rw-r--r--   0        0        0       39 2023-04-11 09:10:06.149294 anndata-0.9.0/anndata/tests/adata.csv
--rw-r--r--   0        0        0      309 2023-04-11 09:10:06.149392 anndata-0.9.0/anndata/tests/conftest.py
--rw-r--r--   0        0        0    17388 2023-04-11 09:10:06.153602 anndata-0.9.0/anndata/tests/helpers.py
--rw-r--r--   0        0        0    12139 2023-04-11 09:10:06.158385 anndata-0.9.0/anndata/utils.py
--rw-r--r--   0        0        0     4800 2023-04-11 09:10:06.163479 anndata-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4597 1970-01-01 00:00:00.000000 anndata-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1544 2023-02-21 15:51:40.691748 anndata-0.9.0rc1/LICENSE
+-rw-r--r--   0        0        0     2262 2023-02-21 15:51:40.691982 anndata-0.9.0rc1/README.rst
+-rw-r--r--   0        0        0      697 2023-02-21 15:51:40.692177 anndata-0.9.0rc1/anndata/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-21 15:51:40.692295 anndata-0.9.0rc1/anndata/_core/__init__.py
+-rw-r--r--   0        0        0      818 2023-02-21 15:51:40.692439 anndata-0.9.0rc1/anndata/_core/access.py
+-rw-r--r--   0        0        0    11532 2023-02-21 15:51:40.692599 anndata-0.9.0rc1/anndata/_core/aligned_mapping.py
+-rw-r--r--   0        0        0    76540 2023-02-21 15:51:40.693040 anndata-0.9.0rc1/anndata/_core/anndata.py
+-rw-r--r--   0        0        0     3574 2023-02-21 15:51:40.693190 anndata-0.9.0rc1/anndata/_core/file_backing.py
+-rw-r--r--   0        0        0     7084 2023-02-21 15:51:40.693351 anndata-0.9.0rc1/anndata/_core/index.py
+-rw-r--r--   0        0        0    36527 2023-02-21 15:51:40.693629 anndata-0.9.0rc1/anndata/_core/merge.py
+-rw-r--r--   0        0        0     6836 2023-02-21 15:51:40.693808 anndata-0.9.0rc1/anndata/_core/raw.py
+-rw-r--r--   0        0        0    13269 2023-02-21 15:51:40.694005 anndata-0.9.0rc1/anndata/_core/sparse_dataset.py
+-rw-r--r--   0        0        0     9696 2023-02-21 16:26:16.580730 anndata-0.9.0rc1/anndata/_core/views.py
+-rw-r--r--   0        0        0      246 2023-02-21 15:51:40.694338 anndata-0.9.0rc1/anndata/_io/__init__.py
+-rw-r--r--   0        0        0    13086 2023-02-21 15:51:40.694523 anndata-0.9.0rc1/anndata/_io/h5ad.py
+-rw-r--r--   0        0        0    15794 2023-02-21 15:51:40.694704 anndata-0.9.0rc1/anndata/_io/read.py
+-rw-r--r--   0        0        0      111 2023-02-21 15:51:40.694872 anndata-0.9.0rc1/anndata/_io/specs/__init__.py
+-rw-r--r--   0        0        0    28569 2023-02-21 15:51:40.695087 anndata-0.9.0rc1/anndata/_io/specs/methods.py
+-rw-r--r--   0        0        0    11004 2023-02-21 15:51:40.695269 anndata-0.9.0rc1/anndata/_io/specs/registry.py
+-rw-r--r--   0        0        0     7780 2023-02-21 15:51:40.695414 anndata-0.9.0rc1/anndata/_io/utils.py
+-rw-r--r--   0        0        0     4602 2023-02-21 15:51:40.695567 anndata-0.9.0rc1/anndata/_io/write.py
+-rw-r--r--   0        0        0     4294 2023-02-21 15:51:40.695714 anndata-0.9.0rc1/anndata/_io/zarr.py
+-rw-r--r--   0        0        0     1312 2023-02-21 15:51:40.695847 anndata-0.9.0rc1/anndata/_metadata.py
+-rw-r--r--   0        0        0      436 2023-02-21 15:51:40.695967 anndata-0.9.0rc1/anndata/_types.py
+-rw-r--r--   0        0        0      695 2023-02-21 15:51:40.696083 anndata-0.9.0rc1/anndata/_warnings.py
+-rw-r--r--   0        0        0     9180 2023-02-21 15:51:40.696304 anndata-0.9.0rc1/anndata/compat/__init__.py
+-rw-r--r--   0        0        0      141 2023-02-21 15:51:40.696436 anndata-0.9.0rc1/anndata/core.py
+-rw-r--r--   0        0        0     3428 2023-02-21 15:51:40.696624 anndata-0.9.0rc1/anndata/experimental/__init__.py
+-rw-r--r--   0        0        0       42 2023-02-21 15:51:40.696789 anndata-0.9.0rc1/anndata/experimental/multi_files/__init__.py
+-rw-r--r--   0        0        0    34530 2023-02-21 15:51:40.697054 anndata-0.9.0rc1/anndata/experimental/multi_files/_anncollection.py
+-rw-r--r--   0        0        0       34 2023-02-21 15:51:40.697255 anndata-0.9.0rc1/anndata/experimental/pytorch/__init__.py
+-rw-r--r--   0        0        0     7143 2023-02-21 15:51:40.697413 anndata-0.9.0rc1/anndata/experimental/pytorch/_annloader.py
+-rw-r--r--   0        0        0     1429 2023-02-21 15:51:40.697546 anndata-0.9.0rc1/anndata/logging.py
+-rw-r--r--   0        0        0      144 2023-02-21 15:51:40.697670 anndata-0.9.0rc1/anndata/readwrite.py
+-rw-r--r--   0        0        0      101 2023-02-21 15:51:40.697837 anndata-0.9.0rc1/anndata/tests/adata-comments.tsv
+-rw-r--r--   0        0        0       39 2023-02-21 15:51:40.697945 anndata-0.9.0rc1/anndata/tests/adata.csv
+-rw-r--r--   0        0        0      309 2023-02-21 15:51:40.698058 anndata-0.9.0rc1/anndata/tests/conftest.py
+-rw-r--r--   0        0        0    17361 2023-02-21 15:51:40.702336 anndata-0.9.0rc1/anndata/tests/helpers.py
+-rw-r--r--   0        0        0    12139 2023-02-21 15:51:40.709024 anndata-0.9.0rc1/anndata/utils.py
+-rw-r--r--   0        0        0     4771 2023-02-21 15:51:40.715595 anndata-0.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4906 1970-01-01 00:00:00.000000 anndata-0.9.0rc1/PKG-INFO
```

### Comparing `anndata-0.9.0/LICENSE` & `anndata-0.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/__init__.py` & `anndata-0.9.0rc1/anndata/__init__.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/_core/access.py` & `anndata-0.9.0rc1/anndata/_core/access.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/_core/aligned_mapping.py` & `anndata-0.9.0rc1/anndata/_core/aligned_mapping.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/_core/anndata.py` & `anndata-0.9.0rc1/anndata/_core/anndata.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             f"X needs to be 2-dimensional, not {len(X.shape)}-dimensional."
         )
 
 
 @singledispatch
 def _gen_dataframe(anno, length, index_names):
     if anno is None or len(anno) == 0:
-        return pd.DataFrame({}, index=pd.RangeIndex(0, length, name=None).astype(str))
+        return pd.DataFrame(index=pd.RangeIndex(0, length, name=None).astype(str))
     for index_name in index_names:
         if index_name in anno:
             return pd.DataFrame(
                 anno,
                 index=anno[index_name],
                 columns=[k for k in anno.keys() if k != index_name],
             )
@@ -754,15 +754,15 @@
         if value is None:
             del self.raw
         elif not isinstance(value, AnnData):
             raise ValueError("Can only init raw attribute with an AnnData object.")
         else:
             if self.is_view:
                 self._init_as_actual(self.copy())
-            self._raw = Raw(self, X=value.X, var=value.var, varm=value.varm)
+            self._raw = Raw(value)
 
     @raw.deleter
     def raw(self):
         if self.is_view:
             self._init_as_actual(self.copy())
         self._raw = None
 
@@ -840,15 +840,15 @@
 
     @obs.setter
     def obs(self, value: pd.DataFrame):
         self._set_dim_df(value, "obs")
 
     @obs.deleter
     def obs(self):
-        self.obs = pd.DataFrame({}, index=self.obs_names)
+        self.obs = pd.DataFrame(index=self.obs_names)
 
     @property
     def obs_names(self) -> pd.Index:
         """Names of observations (alias for `.obs.index`)."""
         return self.obs.index
 
     @obs_names.setter
@@ -863,15 +863,15 @@
 
     @var.setter
     def var(self, value: pd.DataFrame):
         self._set_dim_df(value, "var")
 
     @var.deleter
     def var(self):
-        self.var = pd.DataFrame({}, index=self.var_names)
+        self.var = pd.DataFrame(index=self.var_names)
 
     @property
     def var_names(self) -> pd.Index:
         """Names of variables (alias for `.var.index`)."""
         return self.var.index
 
     @var_names.setter
@@ -1453,15 +1453,15 @@
             new["uns"] = deepcopy(self._uns)
         if "raw" in kwargs:
             new["raw"] = kwargs["raw"]
         elif self.raw is not None:
             new["raw"] = self.raw.copy()
         return AnnData(**new)
 
-    def to_memory(self, copy=False) -> "AnnData":
+    def to_memory(self, copy=True) -> "AnnData":
         """Return a new AnnData object with all backed arrays loaded into memory.
 
         Params
         ------
             copy:
                 Whether the arrays that are already in-memory should be copied.
```

### Comparing `anndata-0.9.0/anndata/_core/file_backing.py` & `anndata-0.9.0rc1/anndata/_core/file_backing.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,47 +89,47 @@
         if self._file is None:
             return False
         # try accessing the id attribute to see if the file is open
         return bool(self._file.id)
 
 
 @singledispatch
-def to_memory(x, copy=False):
+def to_memory(x, copy=True):
     """Permissivley convert objects to in-memory representation.
 
     If they already are in-memory, (or are just unrecognized) pass a copy through.
     """
     if copy and hasattr(x, "copy"):
         return x.copy()
     else:
         return x
 
 
 @to_memory.register(ZarrArray)
 @to_memory.register(h5py.Dataset)
-def _(x, copy=False):
+def _(x, copy=True):
     return x[...]
 
 
 @to_memory.register(SparseDataset)
-def _(x: SparseDataset, copy=False):
+def _(x: SparseDataset, copy=True):
     return x.to_memory()
 
 
 @to_memory.register(DaskArray)
-def _(x, copy=False):
+def _(x, copy=True):
     return x.compute()
 
 
 @to_memory.register(Mapping)
-def _(x: Mapping, copy=False):
+def _(x: Mapping, copy=True):
     return {k: to_memory(v, copy=copy) for k, v in x.items()}
 
 
 @to_memory.register(AwkArray)
-def _(x, copy=False):
-    from copy import copy as _copy
+def _(x, copy=True):
+    from copy import copy
 
     if copy:
-        return _copy(x)
+        return copy(x)
     else:
         return x
```

### Comparing `anndata-0.9.0/anndata/_core/index.py` & `anndata-0.9.0rc1/anndata/_core/index.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/_core/merge.py` & `anndata-0.9.0rc1/anndata/_core/merge.py`

 * *Files 0% similar despite different names*

```diff
@@ -812,14 +812,20 @@
     fill_value: Optional[Any] = None,
     pairwise: bool = False,
 ) -> AnnData:
     """Concatenates AnnData objects along an axis.
 
     See the :doc:`concatenation <../concatenation>` section in the docs for a more in-depth description.
 
+    .. warning::
+
+        This function is marked as experimental for the `0.7` release series, and will
+        supercede the :meth:`AnnData.concatenate() <anndata.AnnData.concatenate>` method
+        in future releases.
+
     Params
     ------
     adatas
         The objects to be concatenated. If a Mapping is passed, keys are used for the `keys`
         argument and values are concatenated.
     axis
         Which axis to concatenate along.
```

### Comparing `anndata-0.9.0/anndata/_core/raw.py` & `anndata-0.9.0rc1/anndata/_core/raw.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/_core/sparse_dataset.py` & `anndata-0.9.0rc1/anndata/_core/sparse_dataset.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/_core/views.py` & `anndata-0.9.0rc1/anndata/_core/views.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/_io/h5ad.py` & `anndata-0.9.0rc1/anndata/_io/h5ad.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/_io/read.py` & `anndata-0.9.0rc1/anndata/_io/read.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/_io/specs/methods.py` & `anndata-0.9.0rc1/anndata/_io/specs/methods.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/_io/specs/registry.py` & `anndata-0.9.0rc1/anndata/_io/specs/registry.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/_io/utils.py` & `anndata-0.9.0rc1/anndata/_io/utils.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/_io/write.py` & `anndata-0.9.0rc1/anndata/_io/write.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/_io/zarr.py` & `anndata-0.9.0rc1/anndata/_io/zarr.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/_metadata.py` & `anndata-0.9.0rc1/anndata/_metadata.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/_warnings.py` & `anndata-0.9.0rc1/anndata/_warnings.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/compat/__init__.py` & `anndata-0.9.0rc1/anndata/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/experimental/__init__.py` & `anndata-0.9.0rc1/anndata/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/experimental/multi_files/_anncollection.py` & `anndata-0.9.0rc1/anndata/experimental/multi_files/_anncollection.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/experimental/pytorch/_annloader.py` & `anndata-0.9.0rc1/anndata/experimental/pytorch/_annloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ..multi_files._anncollection import AnnCollection, _ConcatViewMixin
 
 
 try:
     import torch
     from torch.utils.data import Sampler, BatchSampler, Dataset, DataLoader
 except ImportError:
+    warnings.warn("Сould not load pytorch.")
     Sampler, BatchSampler, Dataset, DataLoader = object, object, object, object
 
 
 # Custom sampler to get proper batches instead of joined separate indices
 # maybe move to multi_files
 class BatchIndexSampler(Sampler):
     def __init__(self, n_obs, batch_size, shuffle=False, drop_last=False):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `anndata-0.9.0/anndata/logging.py` & `anndata-0.9.0rc1/anndata/logging.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/anndata/tests/helpers.py` & `anndata-0.9.0rc1/anndata/tests/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -441,15 +441,15 @@
 
 
 @assert_equal.register(AwkArray)
 def assert_equal_awkarray(a, b, exact=False, elem_name=None):
     from anndata.compat import awkward as ak
 
     if exact:
-        assert a.type == b.type, f"{a.type} != {b.type}, {format_msg(elem_name)}"
+        assert a.type == b.type, format_msg(elem_name)
     assert ak.to_list(a) == ak.to_list(b), format_msg(elem_name)
 
 
 @assert_equal.register(Mapping)
 def assert_equal_mapping(a, b, exact=False, elem_name=None):
     assert set(a.keys()) == set(b.keys()), format_msg(elem_name)
     for k in a.keys():
```

### Comparing `anndata-0.9.0/anndata/utils.py` & `anndata-0.9.0rc1/anndata/utils.py`

 * *Files identical despite different names*

### Comparing `anndata-0.9.0/pyproject.toml` & `anndata-0.9.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     {name = "Sergei Rybakov"},
 ]
 maintainers = [
     {name = "Isaac Virshup", email = "ivirshup@gmail.com"},
     {name = "Philipp Angerer", email = "philipp.angerer@helmholtz-muenchen.de"},
     {name = "Alex Wolf", email = "f.alex.wolf@gmx.de"},
 ]
-readme = {file = "README.md", content-type="text/markdown"}
+readme = {file = "README.rst", content-type="text/x-rst"}
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Environment :: Console",
     "Framework :: Jupyter",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
@@ -64,15 +64,14 @@
     "docutils",
 ]
 doc = [
     "sphinx>=4.4",
     "sphinx-rtd-theme>=1.1.1",
     "sphinx-autodoc-typehints>=1.11.0",
     "sphinx_issues",
-    "sphinxext.opengraph",
     "nbsphinx",
     "scanpydoc>=0.7.7",
     "zarr",
     "awkward>=2.0.7",
     "IPython", # For syntax highlighting in notebooks
     "myst_parser",
 ]
```

### Comparing `anndata-0.9.0/PKG-INFO` & `anndata-0.9.0rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: anndata
-Version: 0.9.0
+Version: 0.9.0rc1
 Summary: Annotated data.
 Author: Philipp Angerer, Alex Wolf, Isaac Virshup, Sergei Rybakov
 Maintainer-email: Isaac Virshup <ivirshup@gmail.com>, Philipp Angerer <philipp.angerer@helmholtz-muenchen.de>, Alex Wolf <f.alex.wolf@gmx.de>
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Environment :: Console
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
@@ -30,15 +30,14 @@
 Requires-Dist: setuptools_scm ; extra == "dev"
 Requires-Dist: black>=20.8b1 ; extra == "dev"
 Requires-Dist: docutils ; extra == "dev"
 Requires-Dist: sphinx>=4.4 ; extra == "doc"
 Requires-Dist: sphinx-rtd-theme>=1.1.1 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints>=1.11.0 ; extra == "doc"
 Requires-Dist: sphinx_issues ; extra == "doc"
-Requires-Dist: sphinxext.opengraph ; extra == "doc"
 Requires-Dist: nbsphinx ; extra == "doc"
 Requires-Dist: scanpydoc>=0.7.7 ; extra == "doc"
 Requires-Dist: zarr ; extra == "doc"
 Requires-Dist: awkward>=2.0.7 ; extra == "doc"
 Requires-Dist: IPython ; extra == "doc"
 Requires-Dist: myst_parser ; extra == "doc"
 Requires-Dist: loompy>=3.0.5 ; extra == "test"
@@ -57,33 +56,47 @@
 Project-URL: Documentation, https://anndata.readthedocs.io/
 Project-URL: Home-page, https://github.com/scverse/anndata
 Project-URL: Source, https://github.com/scverse/anndata
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 
-[![Build Status](https://dev.azure.com/scverse/anndata/_apis/build/status/scverse.anndata?branchName=main)](https://dev.azure.com/scverse/anndata/_build)
-[![Conda](https://img.shields.io/conda/vn/conda-forge/anndata.svg)](https://anaconda.org/conda-forge/anndata)
-[![Coverage](https://codecov.io/gh/scverse/anndata/branch/main/graph/badge.svg?token=IN1mJN1Wi8)](https://codecov.io/gh/scverse/anndata)
-[![Docs](https://readthedocs.com/projects/icb-anndata/badge/?version=latest)](https://anndata.readthedocs.io)
-[![PyPI](https://img.shields.io/pypi/v/anndata.svg)](https://pypi.org/project/anndata)
-[![PyPIDownloadsMonth](https://img.shields.io/pypi/dm/scanpy?logo=PyPI&color=blue)](https://pypi.org/project/anndata)
-[![PyPIDownloadsTotal](https://pepy.tech/badge/anndata)](https://pepy.tech/project/anndata)
-[![Stars](https://img.shields.io/github/stars/scverse/anndata?logo=GitHub&color=yellow)](https://github.com/scverse/anndata/stargazers)
-
-```{image} https://raw.githubusercontent.com/scverse/anndata/main/docs/_static/img/anndata_schema.svg
-:align: right
-:width: 350px
-```
+|Stars| |PyPI| |PyPIDownloadsTotal| |PyPIDownloadsMonth| |Conda| |Docs| |Build Status| |Coverage|
 
-# anndata - Annotated data
+.. |Stars| image:: https://img.shields.io/github/stars/scverse/anndata?logo=GitHub&color=yellow
+   :target: https://github.com/scverse/anndata/stargazers
+.. |PyPI| image:: https://img.shields.io/pypi/v/anndata.svg
+   :target: https://pypi.org/project/anndata
+.. |PyPIDownloadsTotal| image:: https://pepy.tech/badge/anndata
+   :target: https://pepy.tech/project/anndata
+.. |PyPIDownloadsMonth| image:: https://img.shields.io/pypi/dm/scanpy?logo=PyPI&color=blue
+   :target: https://pypi.org/project/anndata
+.. |Conda| image:: https://img.shields.io/conda/vn/conda-forge/anndata.svg
+   :target: https://anaconda.org/conda-forge/anndata
+.. |Docs| image:: https://readthedocs.com/projects/icb-anndata/badge/?version=latest
+   :target: https://anndata.readthedocs.io
+.. |Build Status| image:: https://dev.azure.com/scverse/anndata/_apis/build/status/scverse.anndata?branchName=master
+   :target: https://dev.azure.com/scverse/anndata/_build
+.. |Coverage| image:: https://codecov.io/gh/scverse/anndata/branch/master/graph/badge.svg?token=IN1mJN1Wi8
+   :target: https://codecov.io/gh/scverse/anndata
+
+.. use URL instead of path here so PyPI can render it
+
+.. image:: https://raw.githubusercontent.com/scverse/anndata/master/docs/_static/img/anndata_schema.svg
+   :align: right
+   :width: 350px
+
+.. after image
+
+anndata - Annotated data
+========================
 
 anndata is a Python package for handling annotated data matrices in memory and on disk, positioned between pandas and xarray. anndata offers a broad range of computationally efficient features including, among others, sparse data support, lazy operations, and a PyTorch interface.
 
-- Discuss development on [GitHub](https://github.com/scverse/anndata).
-- Read the [documentation](https://anndata.readthedocs.io).
-- Ask questions on the [scverse Discourse](https://discourse.scverse.org).
-- Install via `pip install anndata` or `conda install anndata -c conda-forge`.
-- Consider citing the [anndata paper](https://doi.org/10.1101/2021.12.16.473007).
-- See [Scanpy's documentation](https://scanpy.readthedocs.io/) for usage
+* Discuss development on `GitHub <https://github.com/scverse/anndata>`_.
+* Read the `documentation <https://anndata.readthedocs.io>`_.
+* Ask questions on the `scverse Discourse <https://discourse.scverse.org>`_.
+* Install via ``pip install anndata`` or ``conda install anndata -c conda-forge``.
+* Consider citing the `anndata paper <https://doi.org/10.1101/2021.12.16.473007>`__.
+* See `Scanpy's documentation <https://scanpy.readthedocs.io/>`__ for usage
   related to single cell data. anndata was initially built for Scanpy.
```

