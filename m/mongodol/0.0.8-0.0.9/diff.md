# Comparing `tmp/mongodol-0.0.8.tar.gz` & `tmp/mongodol-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodol-0.0.8.tar", last modified: Wed Nov 10 17:53:16 2021, max compression
+gzip compressed data, was "mongodol-0.0.9.tar", last modified: Tue Nov 16 21:59:12 2021, max compression
```

## Comparing `mongodol-0.0.8.tar` & `mongodol-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 17:53:16.971653 mongodol-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-11-10 17:52:48.000000 mongodol-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7934 2021-11-10 17:53:16.971653 mongodol-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5328 2021-11-10 17:52:48.000000 mongodol-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 17:53:16.971653 mongodol-0.0.8/mongodol/
--rw-r--r--   0 runner    (1001) docker     (121)      611 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4057 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/add_ons.py
--rw-r--r--   0 runner    (1001) docker     (121)    19104 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      510 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3467 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 17:53:16.971653 mongodol-0.0.8/mongodol/scrap/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/scrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13811 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/scrap/old01.py
--rw-r--r--   0 runner    (1001) docker     (121)    18935 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/scrap/views_work.py
--rw-r--r--   0 runner    (1001) docker     (121)     7420 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/stores.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 17:53:16.971653 mongodol-0.0.8/mongodol/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      269 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/tests/add_ons_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9970 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/tests/base_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8274 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 17:53:16.971653 mongodol-0.0.8/mongodol/tests/int_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/tests/int_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2913 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/tests/int_tests/base_int_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/tests/int_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      745 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/tests/not_working.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/tests/stores_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    10428 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/tracking_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)    10476 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/trans.py
--rw-r--r--   0 runner    (1001) docker     (121)     7145 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 17:53:16.971653 mongodol-0.0.8/mongodol/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10840 2021-11-10 17:52:48.000000 mongodol-0.0.8/mongodol/utils/werk_local.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 17:53:16.971653 mongodol-0.0.8/mongodol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7934 2021-11-10 17:53:16.000000 mongodol-0.0.8/mongodol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      872 2021-11-10 17:53:16.000000 mongodol-0.0.8/mongodol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-10 17:53:16.000000 mongodol-0.0.8/mongodol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-10 17:53:16.000000 mongodol-0.0.8/mongodol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-11-10 17:53:16.000000 mongodol-0.0.8/mongodol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-11-10 17:53:16.000000 mongodol-0.0.8/mongodol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      520 2021-11-10 17:53:16.971653 mongodol-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-11-10 17:52:48.000000 mongodol-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 21:59:12.899600 mongodol-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-11-16 21:58:41.000000 mongodol-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     7934 2021-11-16 21:59:12.899600 mongodol-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5328 2021-11-16 21:58:41.000000 mongodol-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 21:59:12.895600 mongodol-0.0.9/mongodol/
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4057 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/add_ons.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19959 2021-11-16 21:59:11.000000 mongodol-0.0.9/mongodol/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3467 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 21:59:12.895600 mongodol-0.0.9/mongodol/scrap/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/scrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13811 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/scrap/old01.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18935 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/scrap/views_work.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7420 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/stores.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 21:59:12.895600 mongodol-0.0.9/mongodol/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/tests/add_ons_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9970 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/tests/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8274 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 21:59:12.895600 mongodol-0.0.9/mongodol/tests/int_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/tests/int_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6153 2021-11-16 21:59:12.000000 mongodol-0.0.9/mongodol/tests/int_tests/base_int_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/tests/int_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/tests/not_working.py
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/tests/stores_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1904 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10428 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/tracking_methods.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10626 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/trans.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7145 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 21:59:12.899600 mongodol-0.0.9/mongodol/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10840 2021-11-16 21:58:41.000000 mongodol-0.0.9/mongodol/utils/werk_local.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 21:59:12.895600 mongodol-0.0.9/mongodol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7934 2021-11-16 21:59:12.000000 mongodol-0.0.9/mongodol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      872 2021-11-16 21:59:12.000000 mongodol-0.0.9/mongodol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-16 21:59:12.000000 mongodol-0.0.9/mongodol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-16 21:59:12.000000 mongodol-0.0.9/mongodol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-11-16 21:59:12.000000 mongodol-0.0.9/mongodol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-11-16 21:59:12.000000 mongodol-0.0.9/mongodol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      520 2021-11-16 21:59:12.899600 mongodol-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2021-11-16 21:58:41.000000 mongodol-0.0.9/setup.py
```

### Comparing `mongodol-0.0.8/LICENSE` & `mongodol-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/PKG-INFO` & `mongodol-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodol
-Version: 0.0.8
+Version: 0.0.9
 Summary: MongoDB Data Object Layer
 Home-page: https://github.com/i2mint/mongodol
 Author: OtoSense
 License: apache-2.0
 Description: 
         # mongodol
         MongoDB Data Object Layer.
```

### Comparing `mongodol-0.0.8/README.md` & `mongodol-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/mongodol/__init__.py` & `mongodol-0.0.9/mongodol/__init__.py`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/mongodol/add_ons.py` & `mongodol-0.0.9/mongodol/add_ons.py`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/mongodol/base.py` & `mongodol-0.0.9/mongodol/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Base mongoDB data object layers"""
 
 from functools import wraps, cached_property
-from typing import Mapping, Optional, Union, Iterable
-from collections.abc import KeysView, ValuesView, ItemsView
+from typing import Mapping, Optional, Union
 from collections import ChainMap
+from dol.base import Store
 
 from pymongo import MongoClient
 
 from dol import KvReader, Collection as DolCollection, BaseValuesView, BaseItemsView
 
 from mongodol.constants import ID, PyMongoCollectionSpec, end_of_cursor, DFLT_TEST_DB
 from mongodol.util import (
@@ -157,52 +157,35 @@
 
     """
 
     _projections_are_flattened = False
 
     class ValuesView(BaseValuesView):
         def __contains__(self, v):
-            m = self._mapping
-            cursor = m.mgc.find(filter=m._merge_with_filt(v), projection=())
-            return next(cursor, end_of_cursor) is not end_of_cursor
+            return self._mapping.contains_value(v)
 
         def __iter__(self):
-            m = self._mapping
-            return m.mgc.find(filter=m.filter, projection=m._getitem_projection)
-
-        # def distinct(self, key, filter=None, **kwargs):
-        #     m = self._mapping
-        #     # TODO: Check if this is correct (what about $ cases?): filter=m._merge_with_filt(filter)
-        #     return m.mgc.distinct(key, filter=m._merge_with_filt(filter), **kwargs)
-        #
-        # unique = distinct
+            return self._mapping.iter_values()
 
     class ItemsView(BaseItemsView):
         def __contains__(self, item):
-            m = self._mapping
-            k, v = item
-            # TODO: How do we have cursor return no data (here still has _id)
-            cursor = m.mgc.find(filter=dict(v, **m._merge_with_filt(k)), projection=())
-            # return cursor
-            return next(cursor, end_of_cursor) is not end_of_cursor
+            return self._mapping.contains_item(item)
 
         def __iter__(self):
-            m = self._mapping
-            for doc in m.mgc.find(filter=m.filter, projection=m._items_projection):
-                key = {k: doc.pop(k) for k in m.key_fields}
-                yield key, doc
+            return self._mapping.iter_items()
 
     def __init__(
         self,
         mgc: Union[PyMongoCollectionSpec, KvReader] = None,
         filter: Optional[dict] = None,
-        iter_projection: ProjectionSpec = (ID,),
+        iter_projection: ProjectionSpec = None,
         getitem_projection: ProjectionSpec = None,
         **mgc_find_kwargs,
     ):
+        iter_projection = iter_projection or (ID,)
         if not isinstance(iter_projection, dict):
             iter_projection = {k: True for k in iter_projection}
         assert iter_projection is not None, 'iter_projection cannot be None'
         super().__init__(
             mgc=mgc, filter=filter, iter_projection=iter_projection, **mgc_find_kwargs,
         )
         self._getitem_projection = getitem_projection
@@ -211,14 +194,47 @@
         assert isinstance(
             k, Mapping
         ), f'k (key) must be a mapping (typically a dictionary). Was:\n\tk={k}'
         return self.mgc.find(
             filter=self._merge_with_filt(k), projection=self._getitem_projection,
         )
 
+    def contains_value(self, v):
+        cursor = self.mgc.find(
+            filter=self._merge_with_filt(v), projection=(), **self._mgc_find_kwargs
+        )
+        return next(cursor, end_of_cursor) is not end_of_cursor
+
+    def iter_values(self):
+        return self.mgc.find(
+            filter=self.filter,
+            projection=self._getitem_projection,
+            **self._mgc_find_kwargs,
+        )
+
+    def contains_item(self, item):
+        k, v = item
+        # TODO: How do we have cursor return no data (here still has _id)
+        cursor = self.mgc.find(
+            filter=dict(v, **self._merge_with_filt(k)),
+            projection=(),
+            **self._mgc_find_kwargs,
+        )
+        return next(cursor, end_of_cursor) is not end_of_cursor
+
+    def iter_items(self):
+        cursor = self.mgc.find(
+            filter=self.filter,
+            projection=self._items_projection,
+            **self._mgc_find_kwargs,
+        )
+        for doc in cursor:
+            key = {k: doc.pop(k) for k in self.key_fields}
+            yield (key, doc)
+
     @cached_property
     def _items_projection(self):
         iter_projection = self._iter_projection
         getitem_projection = self._getitem_projection
         if iter_projection is None or getitem_projection is None:
             return None
         if not isinstance(self._iter_projection, Mapping):
@@ -513,7 +529,31 @@
         self.collection_store_cls = mk_collection_store
 
     def __iter__(self):
         yield from self.db.list_collection_names()
 
     def __getitem__(self, k):
         return self.collection_store_cls(self.db[k])
+
+
+class MongoBaseStore(Store):
+    def contains_value(self, v):
+        return self.store.contains_value(self._data_of_obj(v))
+
+    def iter_values(self):
+        return map(self._obj_of_data, self.store.iter_values())
+
+    def contains_item(self, item):
+        k, v = item
+        return self.store.contains_item((self._id_of_key(k), self._data_of_obj(v)))
+
+    def iter_items(self):
+        yield from (
+            (self._key_of_id(key), self._obj_of_data(doc))
+            for key, doc in self.store.iter_items()
+        )
+
+    def append(self, v):
+        return self.store.append(self._data_of_obj(v))
+
+    def extend(self, values):
+        return self.store.extend(list(map(self._data_of_obj, values)))
```

### Comparing `mongodol-0.0.8/mongodol/recipes.py` & `mongodol-0.0.9/mongodol/recipes.py`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/mongodol/scrap/old01.py` & `mongodol-0.0.9/mongodol/scrap/old01.py`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/mongodol/scrap/views_work.py` & `mongodol-0.0.9/mongodol/scrap/views_work.py`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/mongodol/stores.py` & `mongodol-0.0.9/mongodol/stores.py`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/mongodol/tests/add_ons_test.py` & `mongodol-0.0.9/mongodol/tests/add_ons_test.py`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/mongodol/tests/base_test.py` & `mongodol-0.0.9/mongodol/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/mongodol/tests/data.py` & `mongodol-0.0.9/mongodol/tests/data.py`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/mongodol/tests/not_working.py` & `mongodol-0.0.9/mongodol/tests/not_working.py`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/mongodol/tests/stores_test.py` & `mongodol-0.0.9/mongodol/tests/stores_test.py`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/mongodol/tests/util.py` & `mongodol-0.0.9/mongodol/tests/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from functools import lru_cache
 
+from pymongo import MongoClient
+
+from mongodol.base import MongoCollectionPersister
+from mongodol.tests import (
+    data as test_data,
+    NUMBER_MGC_NAME,
+    FEATURE_CUBE_MGC_NAME,
+    BDFL_MGC_NAME,
+)
 from mongodol.constants import (
     DFLT_MONGO_CLIENT_ARGS,
     DFLT_TEST_DB,
     DFLT_TEST_COLLECTION,
 )
-from pymongo import MongoClient
-
-from mongodol.base import MongoCollectionPersister
-
-# from mongodol.util import mk_dflt_mgc
-from mongodol.tests import data as test_data
 
 
 @lru_cache(maxsize=1)
 def get_test_database(mongo_client_args=DFLT_MONGO_CLIENT_ARGS, db_name=DFLT_TEST_DB):
     return MongoClient(*mongo_client_args)[db_name]
 
 
@@ -47,17 +50,17 @@
 
 def init_db():
     client = MongoClient(*DFLT_MONGO_CLIENT_ARGS)
     db = client[DFLT_TEST_DB]
     for collection in db.list_collection_names():
         db[collection].delete_many({})
 
-    db.number.insert_many(test_data.nums_and_lans)
-    db.feature_cube.insert_many(test_data.feature_cube)
-    db.bdfl.insert_many(test_data.bdfl)
+    db[NUMBER_MGC_NAME].insert_many(test_data.nums_and_lans)
+    db[FEATURE_CUBE_MGC_NAME].insert_many(test_data.feature_cube)
+    db[BDFL_MGC_NAME].insert_many(test_data.bdfl)
 
 
 def populated_pymongo_collection(docs=test_data.nums_and_lans):
     """Get a pymongo collection that has been populated with docs."""
     test_store = get_test_collection_persister()
     clear_all_and_populate(docs, test_store)
     return test_store.mgc
```

### Comparing `mongodol-0.0.8/mongodol/tracking_methods.py` & `mongodol-0.0.9/mongodol/tracking_methods.py`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/mongodol/trans.py` & `mongodol-0.0.9/mongodol/trans.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """Transformative functionality"""
 
 from copy import deepcopy
 from abc import ABC
 from typing import Mapping
-from functools import wraps
+from functools import partial, wraps
 from typing import Iterable, Optional, TypedDict
+from dol import wrap_kvs as dol_wrap_kvs
 
 from pymongo.results import (
     BulkWriteResult,
     DeleteResult,
     InsertManyResult,
     InsertOneResult,
     UpdateResult,
 )
 
 from dol.trans import (
     condition_function_call,
     double_up_as_factory,
     store_decorator,
 )
+from mongodol.base import MongoBaseStore
 from mongodol.util import KeyNotUniqueError
 
 
 #
 # def _key_does_not_exist(store, k, v):
 #     """Condition function for use in condition_function_call. Returns true iff the k is not in store"""
 #     return k in not store
@@ -300,7 +302,10 @@
                     method_name,
                     normalize_result(
                         getattr(cls, method_name),
                         method_names_to_normalize=method_names_to_normalize,
                     ),
                 )
         return cls
+
+
+wrap_kvs = partial(dol_wrap_kvs, wrapper=MongoBaseStore)
```

### Comparing `mongodol-0.0.8/mongodol/util.py` & `mongodol-0.0.9/mongodol/util.py`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/mongodol/utils/werk_local.py` & `mongodol-0.0.9/mongodol/utils/werk_local.py`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/mongodol.egg-info/PKG-INFO` & `mongodol-0.0.9/mongodol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodol
-Version: 0.0.8
+Version: 0.0.9
 Summary: MongoDB Data Object Layer
 Home-page: https://github.com/i2mint/mongodol
 Author: OtoSense
 License: apache-2.0
 Description: 
         # mongodol
         MongoDB Data Object Layer.
```

### Comparing `mongodol-0.0.8/mongodol.egg-info/SOURCES.txt` & `mongodol-0.0.9/mongodol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mongodol-0.0.8/setup.cfg` & `mongodol-0.0.9/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mongodol
-version = 0.0.8
+version = 0.0.9
 url = https://github.com/i2mint/mongodol
 platforms = any
 description_file = README.md
 root_url = https://github.com/i2mint/
 license = apache-2.0
 author = OtoSense
 description = MongoDB Data Object Layer
```

