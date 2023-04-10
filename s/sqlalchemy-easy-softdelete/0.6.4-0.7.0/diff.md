# Comparing `tmp/sqlalchemy_easy_softdelete-0.6.4.tar.gz` & `tmp/sqlalchemy_easy_softdelete-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_easy_softdelete-0.6.4.tar", max compression
+gzip compressed data, was "sqlalchemy_easy_softdelete-0.7.0.tar", max compression
```

## Comparing `sqlalchemy_easy_softdelete-0.6.4.tar` & `sqlalchemy_easy_softdelete-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1497 2023-04-10 21:45:30.250003 sqlalchemy_easy_softdelete-0.6.4/LICENSE
--rw-r--r--   0        0        0     2877 2023-04-10 21:45:30.250003 sqlalchemy_easy_softdelete-0.6.4/README.md
--rw-r--r--   0        0        0     2309 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      140 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/__init__.py
--rw-r--r--   0        0        0       65 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/handler/__init__.py
--rw-r--r--   0        0        0     6089 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py
--rw-r--r--   0        0        0      850 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py
--rw-r--r--   0        0        0     1623 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/mixin.py
--rw-r--r--   0        0        0       56 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/__init__.py
--rw-r--r--   0        0        0     1971 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/conftest.py
--rw-r--r--   0        0        0     2489 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/model.py
--rw-r--r--   0        0        0      360 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/seed_data/__init__.py
--rw-r--r--   0        0        0     2025 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/seed_data/parent_child_childchild.py
--rw-r--r--   0        0        0        0 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/snapshots/__init__.py
--rw-r--r--   0        0        0     6518 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/snapshots/snap_test_queries.py
--rw-r--r--   0        0        0     9931 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/snapshots/snap_test_seed_data.py
--rw-r--r--   0        0        0     6340 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/test_queries.py
--rw-r--r--   0        0        0      595 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/test_seed_data.py
--rw-r--r--   0        0        0     4508 1970-01-01 00:00:00.000000 sqlalchemy_easy_softdelete-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-04-10 22:22:14.901077 sqlalchemy_easy_softdelete-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2877 2023-04-10 22:22:14.901077 sqlalchemy_easy_softdelete-0.7.0/README.md
+-rw-r--r--   0        0        0     2314 2023-04-10 22:22:14.901077 sqlalchemy_easy_softdelete-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      140 2023-04-10 22:22:14.901077 sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/__init__.py
+-rw-r--r--   0        0        0       65 2023-04-10 22:22:14.901077 sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/handler/__init__.py
+-rw-r--r--   0        0        0     6089 2023-04-10 22:22:14.901077 sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py
+-rw-r--r--   0        0        0      850 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py
+-rw-r--r--   0        0        0     1623 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/mixin.py
+-rw-r--r--   0        0        0       56 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     1971 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     2580 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/model.py
+-rw-r--r--   0        0        0      360 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/seed_data/__init__.py
+-rw-r--r--   0        0        0     2025 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/seed_data/parent_child_childchild.py
+-rw-r--r--   0        0        0        0 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0     6518 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/snapshots/snap_test_queries.py
+-rw-r--r--   0        0        0     9931 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/snapshots/snap_test_seed_data.py
+-rw-r--r--   0        0        0     6340 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/test_queries.py
+-rw-r--r--   0        0        0      595 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/test_seed_data.py
+-rw-r--r--   0        0        0     4557 1970-01-01 00:00:00.000000 sqlalchemy_easy_softdelete-0.7.0/PKG-INFO
```

### Comparing `sqlalchemy_easy_softdelete-0.6.4/LICENSE` & `sqlalchemy_easy_softdelete-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.4/README.md` & `sqlalchemy_easy_softdelete-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.4/pyproject.toml` & `sqlalchemy_easy_softdelete-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "sqlalchemy-easy-softdelete"
-version = "0.6.4"
+version = "0.7.0"
 homepage = "https://github.com/flipbit03/sqlalchemy-easy-softdelete"
 description = "Easily add soft-deletion to your SQLAlchemy Models."
 authors = ["Cadu <cadu.coelho@gmail.com>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
@@ -16,16 +16,16 @@
 ]
 packages = [
     { include = "sqlalchemy_easy_softdelete" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<4.0"
-SQLAlchemy = "^1.4"
+python = ">=3.9,<4.0"
+SQLAlchemy = ">=1.4,<2.1"
 certifi = ">=2022.12.07"
 cryptography = ">=38.0.3"
 
 black  = { version = "^21.5b2", optional = true}
 isort  = { version = "^5.8.0", optional = true}
 flake8  = { version = "^3.9.2", optional = true}
 flake8-docstrings = { version = "^1.6.0", optional = true }
```

### Comparing `sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py` & `sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py` & `sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/mixin.py` & `sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/mixin.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.4/tests/conftest.py` & `sqlalchemy_easy_softdelete-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.4/tests/model.py` & `sqlalchemy_easy_softdelete-0.7.0/tests/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,33 +28,37 @@
     int_field = Column(Integer)
 
     def __repr__(self):
         return f"<{self.__class__.__name__} id={self.id} deleted={bool(self.deleted_at)}>"
 
 
 class SDParent(TestModelBase, SoftDeleteMixin):
+    __allow_unmapped__ = True
     children: 'List[SDChild]' = relationship('SDChild')
 
     def __repr__(self):
         return f"<{self.__class__.__name__} id={self.id} deleted={bool(self.deleted_at)}>"
 
 
 class SDChild(TestModelBase, SoftDeleteMixin):
+    __allow_unmapped__ = True
     parent_id = Column(Integer, ForeignKey(f'{SDParent.__tablename__}.id'), nullable=False)
     parent: SDParent = relationship('SDParent', back_populates="children")
 
     child_children: 'List[SDChildChild]' = relationship('SDChildChild')
 
     def __repr__(self):
         pid = f"(parent_id={self.parent_id})"
         left = f"{self.__class__.__name__} id={self.id} deleted={bool(self.deleted_at)}"
         return f"<{left:30} {pid:>15}>"
 
 
 class SDChildChild(TestModelBase, SoftDeleteMixin):
+    __allow_unmapped__ = True
+
     child_id = Column(Integer, ForeignKey(f'{SDChild.__tablename__}.id'), nullable=False)
     child: SDChild = relationship('SDChild', back_populates="child_children")
 
     def __repr__(self):
         pid = f"(child_id={self.child_id})"
         left = f"{self.__class__.__name__} id={self.id} deleted={bool(self.deleted_at)}"
         return f"<{left:30} {pid:>15}>"
```

### Comparing `sqlalchemy_easy_softdelete-0.6.4/tests/seed_data/parent_child_childchild.py` & `sqlalchemy_easy_softdelete-0.7.0/tests/seed_data/parent_child_childchild.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.4/tests/snapshots/snap_test_queries.py` & `sqlalchemy_easy_softdelete-0.7.0/tests/snapshots/snap_test_queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 
 snapshots['test_ensure_aggregate_from_multiple_table_deletion_works_active_object_count 1'] = '''SELECT count(*) AS count_1 
 FROM sdchild JOIN sdparent ON sdparent.id = sdchild.parent_id 
 WHERE sdchild.deleted_at IS NULL AND sdparent.deleted_at IS NULL'''
 
 snapshots['test_ensure_aggregate_from_multiple_table_deletion_works_active_object_count 2'] = 1
 
-snapshots['test_ensure_table_with_inheritance_works 1'] = '''SELECT sdderivedrequest.id, sdbaserequest.id AS id_1, sdbaserequest.deleted_at, sdbaserequest.request_type, sdbaserequest.base_field, sdderivedrequest.derived_field 
+snapshots['test_ensure_table_with_inheritance_works 1'] = '''SELECT sdbaserequest.request_type, sdbaserequest.base_field, sdderivedrequest.id, sdbaserequest.id AS id_1, sdbaserequest.deleted_at, sdderivedrequest.derived_field 
 FROM sdbaserequest JOIN sdderivedrequest ON sdbaserequest.id = sdderivedrequest.id 
 WHERE sdbaserequest.deleted_at IS NULL'''
 
 snapshots['test_ensure_table_with_inheritance_works 2'] = [
     GenericRepr('<SDDerivedRequest id=1000>'),
     GenericRepr('<SDDerivedRequest id=1001>')
 ]
 
 snapshots['test_ensure_table_with_inheritance_works 3'] = [
     GenericRepr('<SDDerivedRequest id=1000>'),
     GenericRepr('<SDDerivedRequest id=1001>'),
     GenericRepr('<SDDerivedRequest id=1002>')
 ]
 
-snapshots['test_query_single_table 1'] = '''SELECT sdchild.id, sdchild.deleted_at, sdchild.parent_id 
+snapshots['test_query_single_table 1'] = '''SELECT sdchild.parent_id, sdchild.id, sdchild.deleted_at 
 FROM sdchild 
 WHERE sdchild.deleted_at IS NULL'''
 
 snapshots['test_query_single_table 2'] = [
     GenericRepr('<SDChild id=100000 deleted=False (parent_id=1000)>'),
     GenericRepr('<SDChild id=100001 deleted=False (parent_id=1000)>'),
     GenericRepr('<SDChild id=100002 deleted=False (parent_id=1000)>'),
@@ -41,18 +41,18 @@
     GenericRepr('<SDChild id=100200 deleted=False (parent_id=1002)>'),
     GenericRepr('<SDChild id=100201 deleted=False (parent_id=1002)>'),
     GenericRepr('<SDChild id=100202 deleted=False (parent_id=1002)>'),
     GenericRepr('<SDChild id=100203 deleted=False (parent_id=1002)>'),
     GenericRepr('<SDChild id=100204 deleted=False (parent_id=1002)>')
 ]
 
-snapshots['test_query_union_sdchild 1'] = '''SELECT anon_1.sdchild_id, anon_1.sdchild_deleted_at, anon_1.sdchild_parent_id 
-FROM (SELECT sdchild.id AS sdchild_id, sdchild.deleted_at AS sdchild_deleted_at, sdchild.parent_id AS sdchild_parent_id 
+snapshots['test_query_union_sdchild 1'] = '''SELECT anon_1.sdchild_parent_id, anon_1.sdchild_id, anon_1.sdchild_deleted_at 
+FROM (SELECT sdchild.parent_id AS sdchild_parent_id, sdchild.id AS sdchild_id, sdchild.deleted_at AS sdchild_deleted_at 
 FROM sdchild 
-WHERE sdchild.deleted_at IS NULL UNION SELECT sdchild.id AS sdchild_id, sdchild.deleted_at AS sdchild_deleted_at, sdchild.parent_id AS sdchild_parent_id 
+WHERE sdchild.deleted_at IS NULL UNION SELECT sdchild.parent_id AS sdchild_parent_id, sdchild.id AS sdchild_id, sdchild.deleted_at AS sdchild_deleted_at 
 FROM sdchild 
 WHERE sdchild.deleted_at IS NULL) AS anon_1'''
 
 snapshots['test_query_union_sdchild 2'] = [
     GenericRepr('<SDChild id=100000 deleted=False (parent_id=1000)>'),
     GenericRepr('<SDChild id=100001 deleted=False (parent_id=1000)>'),
     GenericRepr('<SDChild id=100002 deleted=False (parent_id=1000)>'),
@@ -67,15 +67,15 @@
 
 snapshots['test_query_union_sdchild_core 1'] = '''SELECT sdchild.id, sdchild.parent_id 
 FROM sdchild 
 WHERE sdchild.deleted_at IS NULL UNION SELECT sdchild.id, sdchild.parent_id 
 FROM sdchild 
 WHERE sdchild.deleted_at IS NULL'''
 
-snapshots['test_query_with_join 1'] = '''SELECT sdchild.id, sdchild.deleted_at, sdchild.parent_id 
+snapshots['test_query_with_join 1'] = '''SELECT sdchild.parent_id, sdchild.id, sdchild.deleted_at 
 FROM sdchild JOIN sdparent ON sdparent.id = sdchild.parent_id 
 WHERE sdchild.deleted_at IS NULL AND sdparent.deleted_at IS NULL'''
 
 snapshots['test_query_with_join 2'] = [
     GenericRepr('<SDChild id=100000 deleted=False (parent_id=1000)>'),
     GenericRepr('<SDChild id=100001 deleted=False (parent_id=1000)>'),
     GenericRepr('<SDChild id=100002 deleted=False (parent_id=1000)>'),
@@ -89,18 +89,18 @@
 
 snapshots['test_query_with_table_clause_as_table 1'] = '''SELECT id 
 FROM sdderivedrequest'''
 
 snapshots['test_query_with_text_clause_as_table 1'] = '''SELECT id 
 FROM sdderivedrequest'''
 
-snapshots['test_query_with_union_but_union_softdelete_disabled 1'] = '''SELECT anon_1.sdchild_id, anon_1.sdchild_deleted_at, anon_1.sdchild_parent_id 
-FROM (SELECT sdchild.id AS sdchild_id, sdchild.deleted_at AS sdchild_deleted_at, sdchild.parent_id AS sdchild_parent_id 
+snapshots['test_query_with_union_but_union_softdelete_disabled 1'] = '''SELECT anon_1.sdchild_parent_id, anon_1.sdchild_id, anon_1.sdchild_deleted_at 
+FROM (SELECT sdchild.parent_id AS sdchild_parent_id, sdchild.id AS sdchild_id, sdchild.deleted_at AS sdchild_deleted_at 
 FROM sdchild 
-WHERE sdchild.deleted_at IS NULL UNION SELECT sdchild.id AS sdchild_id, sdchild.deleted_at AS sdchild_deleted_at, sdchild.parent_id AS sdchild_parent_id 
+WHERE sdchild.deleted_at IS NULL UNION SELECT sdchild.parent_id AS sdchild_parent_id, sdchild.id AS sdchild_id, sdchild.deleted_at AS sdchild_deleted_at 
 FROM sdchild) AS anon_1'''
 
 snapshots['test_query_with_union_but_union_softdelete_disabled 2'] = [
     GenericRepr('<SDChild id=100000 deleted=False (parent_id=1000)>'),
     GenericRepr('<SDChild id=100001 deleted=False (parent_id=1000)>'),
     GenericRepr('<SDChild id=100002 deleted=False (parent_id=1000)>'),
     GenericRepr('<SDChild id=100003 deleted=False (parent_id=1000)>'),
```

### Comparing `sqlalchemy_easy_softdelete-0.6.4/tests/snapshots/snap_test_seed_data.py` & `sqlalchemy_easy_softdelete-0.7.0/tests/snapshots/snap_test_seed_data.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.4/tests/test_queries.py` & `sqlalchemy_easy_softdelete-0.7.0/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.4/tests/test_seed_data.py` & `sqlalchemy_easy_softdelete-0.7.0/tests/test_seed_data.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.4/PKG-INFO` & `sqlalchemy_easy_softdelete-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-easy-softdelete
-Version: 0.6.4
+Version: 0.7.0
 Summary: Easily add soft-deletion to your SQLAlchemy Models.
 Home-page: https://github.com/flipbit03/sqlalchemy-easy-softdelete
 License: BSD-3-Clause
 Author: Cadu
 Author-email: cadu.coelho@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: dev
 Provides-Extra: test
-Requires-Dist: SQLAlchemy (>=1.4,<2.0)
+Requires-Dist: SQLAlchemy (>=1.4,<2.1)
 Requires-Dist: black (>=21.5b2,<22.0) ; extra == "test"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
 Requires-Dist: certifi (>=2022.12.07)
 Requires-Dist: cryptography (>=38.0.3)
 Requires-Dist: flake8 (>=3.9.2,<4.0.0) ; extra == "test"
 Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
 Requires-Dist: isort (>=5.8.0,<6.0.0) ; extra == "test"
```

