# Comparing `tmp/gator_core-2.0.0rc8.tar.gz` & `tmp/gator_core-2.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gator_core-2.0.0rc8.tar", max compression
+gzip compressed data, was "gator_core-2.0.0rc9.tar", max compression
```

## Comparing `gator_core-2.0.0rc8.tar` & `gator_core-2.0.0rc9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1061 2023-04-03 17:16:09.889841 gator_core-2.0.0rc8/LICENSE
--rw-r--r--   0        0        0      842 2023-04-03 17:16:09.889841 gator_core-2.0.0rc8/README.md
--rw-r--r--   0        0        0     1366 2023-04-03 17:16:33.073986 gator_core-2.0.0rc8/pyproject.toml
--rw-r--r--   0        0        0     5857 2023-04-03 17:16:09.889841 gator_core-2.0.0rc8/src/gator/core/data/dataset.py
--rw-r--r--   0        0        0       68 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/src/gator/core/data/utils/__init__.py
--rw-r--r--   0        0        0     1482 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/src/gator/core/data/utils/hash.py
--rw-r--r--   0        0        0     3458 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/src/gator/core/data/utils/io.py
--rw-r--r--   0        0        0     1226 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/src/gator/core/data/utils/serialization.py
--rw-r--r--   0        0        0       27 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/src/gator/core/models/__init__.py
--rw-r--r--   0        0        0      242 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/src/gator/core/models/common.py
--rw-r--r--   0        0        0    14640 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/src/gator/core/models/institution.py
--rw-r--r--   0        0        0      614 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/src/gator/core/models/mongoengine_typing.py
--rw-r--r--   0        0        0    28943 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/src/gator/core/models/timetable.py
--rw-r--r--   0        0        0       36 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/src/gator/core/schemas/__init__.py
--rw-r--r--   0        0        0      883 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/src/gator/core/schemas/institution.py
--rw-r--r--   0        0        0     2737 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/src/gator/core/schemas/timetable.py
--rw-r--r--   0        0        0       32 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/tests/__init__.py
--rw-r--r--   0        0        0     2770 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/tests/data/utils/test_hash.py
--rw-r--r--   0        0        0     9485 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/tests/data/utils/test_io.py
--rw-r--r--   0        0        0     1939 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/tests/data/utils/test_serialization.py
--rw-r--r--   0        0        0       28 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/tests/models/__init__.py
--rw-r--r--   0        0        0     6224 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/tests/models/test_timetable.py
--rw-r--r--   0        0        0     7304 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/tests/schemas/test_institution.py
--rw-r--r--   0        0        0    15757 2023-04-03 17:16:09.893841 gator_core-2.0.0rc8/tests/schemas/test_timetable.py
--rw-r--r--   0        0        0     1550 1970-01-01 00:00:00.000000 gator_core-2.0.0rc8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/LICENSE
+-rw-r--r--   0        0        0      842 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/README.md
+-rw-r--r--   0        0        0     1349 2023-04-04 16:53:03.320453 gator_core-2.0.0rc9/pyproject.toml
+-rw-r--r--   0        0        0     5857 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/src/gator/core/data/dataset.py
+-rw-r--r--   0        0        0       68 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/src/gator/core/data/utils/__init__.py
+-rw-r--r--   0        0        0     1482 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/src/gator/core/data/utils/hash.py
+-rw-r--r--   0        0        0     3458 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/src/gator/core/data/utils/io.py
+-rw-r--r--   0        0        0     1226 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/src/gator/core/data/utils/serialization.py
+-rw-r--r--   0        0        0       27 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/src/gator/core/models/__init__.py
+-rw-r--r--   0        0        0      242 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/src/gator/core/models/common.py
+-rw-r--r--   0        0        0    14976 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/src/gator/core/models/institution.py
+-rw-r--r--   0        0        0      614 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/src/gator/core/models/mongoengine_typing.py
+-rw-r--r--   0        0        0    28943 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/src/gator/core/models/timetable.py
+-rw-r--r--   0        0        0       36 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/src/gator/core/schemas/__init__.py
+-rw-r--r--   0        0        0      883 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/src/gator/core/schemas/institution.py
+-rw-r--r--   0        0        0     2737 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/src/gator/core/schemas/timetable.py
+-rw-r--r--   0        0        0       32 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/tests/__init__.py
+-rw-r--r--   0        0        0     2770 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/tests/data/utils/test_hash.py
+-rw-r--r--   0        0        0     9485 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/tests/data/utils/test_io.py
+-rw-r--r--   0        0        0     1939 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/tests/data/utils/test_serialization.py
+-rw-r--r--   0        0        0       28 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/tests/models/__init__.py
+-rw-r--r--   0        0        0     9405 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/tests/models/test_institution.py
+-rw-r--r--   0        0        0     6224 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/tests/models/test_timetable.py
+-rw-r--r--   0        0        0     7304 2023-04-04 16:52:40.080104 gator_core-2.0.0rc9/tests/schemas/test_institution.py
+-rw-r--r--   0        0        0    15757 2023-04-04 16:52:40.084104 gator_core-2.0.0rc9/tests/schemas/test_timetable.py
+-rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 gator_core-2.0.0rc9/PKG-INFO
```

### Comparing `gator_core-2.0.0rc8/LICENSE` & `gator_core-2.0.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/README.md` & `gator_core-2.0.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/pyproject.toml` & `gator_core-2.0.0rc9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gator-core"
-version = "v2.0.0-rc8"  # placeholder for the real version, which is retrieved from git tags
+version = "v2.0.0-rc9"  # placeholder for the real version, which is retrieved from git tags
 description = "A dataset aggregation framework for Sqrl Planner."
 authors = ["Shon Verch <verchshon@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "gator", from = "src" }
@@ -20,15 +20,14 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 mongoengine = ">=0.20"
 marshmallow = "^3.17.0"
 requests = "^2.28.2"
 bs4 = "^0.0.1"
 routes = "^2.5.1"
-hooky = "^0.5.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.20.0"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.7.0"
 pytest-httpserver = "^1.0.4"
```

### Comparing `gator_core-2.0.0rc8/src/gator/core/data/dataset.py` & `gator_core-2.0.0rc9/src/gator/core/data/dataset.py`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/src/gator/core/data/utils/hash.py` & `gator_core-2.0.0rc9/src/gator/core/data/utils/hash.py`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/src/gator/core/data/utils/io.py` & `gator_core-2.0.0rc9/src/gator/core/data/utils/io.py`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/src/gator/core/data/utils/serialization.py` & `gator_core-2.0.0rc9/src/gator/core/data/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/src/gator/core/models/institution.py` & `gator_core-2.0.0rc9/src/gator/core/models/institution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 """Model definitions for data about an academic institution."""
 from queue import Queue
-from typing import Any, Optional
+from typing import Any, List, Optional
 
-import hooky
+import gator._vendor.hooky as hooky
 import mongoengine
 from mongoengine import Document, EmbeddedDocument, fields
 
 
-class SubInstitutionList(hooky.List):
-    """A list of sub-institutions for an institution.
+class _SubInstitutionsList(hooky.List, List['Institution']):
+    """A list of sub-institutions for a wrapped institution.
 
     This list is used to ensure that the parent of each sub-institution is
     updated when the list is modified. This is done by intercepting calls to
     `append` and `remove`.
     """
 
     # Private Instance Attributes:
-    #   _institution: The institution whose sub-institutions this list
+    #   _institution: The wrapped institution whose sub-institutions this list
     #       represents.
     _institution: 'Institution'
 
     def __init__(self, institution: 'Institution', **kwargs: Any) -> None:
         """Initialize a list of sub-institutions.
 
         Args:
-            institution: The institution whose sub-institutions this list
-                represents.
+            institution: The wrapped institution whose sub-institutions this
+                list represents.
         """
         self._institution = institution
         super().__init__(self._institution._sub_institutions, **kwargs)
 
     def _after_add(self, key: Any, item: Any) -> None:
         """Call after an item is added to the list.
 
         This will set the parent of the added institution to the institution
         that this list was created for.
         """
+        super()._after_add(key, item)
         assert isinstance(key, int), 'Only integer keys are allowed'
         assert isinstance(item, Institution), 'Only institutions are allowed'
         item.parent = self._institution
 
-    def _after_remove(self, key: Any, item: Any) -> None:
+    def _after_del(self, key: Any, item: Any) -> None:
         """Call after an item is removed from the list.
 
         This will set the parent of the removed institution to None.
         """
+        super()._after_del(key, item)
         assert isinstance(key, int), 'Only integer keys are allowed'
         assert isinstance(item, Institution), 'Only institutions are allowed'
         item.parent = None
 
 
 class Institution(Document):
     """An academic institution.
@@ -139,41 +141,43 @@
 
         self._parent = new_parent
         if new_parent is not None:
             # Add this institution to the new parent's list of sub-institutions
             new_parent._sub_institutions.append(self)
 
     @property
-    def sub_institutions(self) -> SubInstitutionList:
+    def sub_institutions(self) -> _SubInstitutionsList:
         """Get the sub-institutions of this institution.
 
         >>> foo = Institution(code='foo', name='Foo', type='university')
         >>> bar = Institution(code='bar', name='Bar', type='campus')
         >>> baz = Institution(code='baz', name='Baz', type='department')
         >>> foo.sub_institutions.append(bar)
         >>> foo.sub_institutions.append(baz)
         >>> foo.sub_institutions  # doctest: +ELLIPSIS
         [Institution(code='bar', ...), Institution(code='baz', ...)]
         >>> bar.parent  # doctest: +ELLIPSIS
         Institution(code='foo', ...)
         >>> baz.parent  # doctest: +ELLIPSIS
         Institution(code='foo', ...)
         """
-        return SubInstitutionList(self, hook_when_init=False)
+        return _SubInstitutionsList(self, hook_when_init=False)
 
     @sub_institutions.setter
     def sub_institutions(self, new_sub_institutions: list['Institution']) \
             -> None:
         """Set the sub-institutions of this institution.
 
         Args:
             new_sub_institutions: The new sub-institutions of this
                 institution.
         """
-        self._sub_institutions = new_sub_institutions
+        self._sub_institutions.clear()
+        for sub_inst in new_sub_institutions:
+            self.sub_institutions.append(sub_inst)
 
     def find_children(self, institution_type: str) -> list['Institution']:
         """Find all sub-institutions of the given type.
 
         This function recursively searches through all sub-institutions of this
         institution, performing a queue-based breadth-first search, and returns
         a list of all institutions of the given type.
@@ -202,19 +206,20 @@
 
             for sub_inst in curr.sub_institutions:
                 q.put(sub_inst)
 
         return children
 
     def find_parent(self, institution_type: str) -> Optional['Institution']:
-        """Find the first parent institution of the given type.
+        """Find the first strictly parent institution of the given type.
 
         This function recursively searches through all parent institutions of
         this institution, performing a queue-based breadth-first search, and
-        returns the first institution of the given type.
+        returns the first institution of the given type. This function does not
+        include this institution in the search.
 
         Args:
             institution_type: The type of institution to search for. For
                 example, `university` or `campus`.
 
         Returns:
             The first (closest) parent institution of the given type, or None
@@ -227,15 +232,15 @@
 
         while not q.empty():
             curr = q.get()
             if curr.code in visited:
                 continue
             visited.add(curr.code)
 
-            if curr.type == institution_type:
+            if curr.type == institution_type and curr != self:
                 return curr
 
             if curr.parent is not None:
                 q.put(curr.parent)
 
         return None
```

### Comparing `gator_core-2.0.0rc8/src/gator/core/models/mongoengine_typing.py` & `gator_core-2.0.0rc9/src/gator/core/models/mongoengine_typing.py`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/src/gator/core/models/timetable.py` & `gator_core-2.0.0rc9/src/gator/core/models/timetable.py`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/src/gator/core/schemas/institution.py` & `gator_core-2.0.0rc9/src/gator/core/schemas/institution.py`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/src/gator/core/schemas/timetable.py` & `gator_core-2.0.0rc9/src/gator/core/schemas/timetable.py`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/tests/data/utils/test_hash.py` & `gator_core-2.0.0rc9/tests/data/utils/test_hash.py`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/tests/data/utils/test_io.py` & `gator_core-2.0.0rc9/tests/data/utils/test_io.py`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/tests/data/utils/test_serialization.py` & `gator_core-2.0.0rc9/tests/data/utils/test_serialization.py`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/tests/models/test_timetable.py` & `gator_core-2.0.0rc9/tests/models/test_timetable.py`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/tests/schemas/test_institution.py` & `gator_core-2.0.0rc9/tests/schemas/test_institution.py`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/tests/schemas/test_timetable.py` & `gator_core-2.0.0rc9/tests/schemas/test_timetable.py`

 * *Files identical despite different names*

### Comparing `gator_core-2.0.0rc8/PKG-INFO` & `gator_core-2.0.0rc9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: gator-core
-Version: 2.0.0rc8
+Version: 2.0.0rc9
 Summary: A dataset aggregation framework for Sqrl Planner.
 License: MIT
 Author: Shon Verch
 Author-email: verchshon@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
-Requires-Dist: hooky (>=0.5.0,<0.6.0)
 Requires-Dist: marshmallow (>=3.17.0,<4.0.0)
 Requires-Dist: mongoengine (>=0.20)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: routes (>=2.5.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sqrl-planner/gator-core/main.svg)](https://results.pre-commit.ci/latest/github/sqrl-planner/gator-core/main)
```

