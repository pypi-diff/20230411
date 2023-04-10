# Comparing `tmp/sqlalchemy_easy_softdelete-0.7.0.tar.gz` & `tmp/sqlalchemy_easy_softdelete-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_easy_softdelete-0.7.0.tar", max compression
+gzip compressed data, was "sqlalchemy_easy_softdelete-0.7.1.tar", max compression
```

## Comparing `sqlalchemy_easy_softdelete-0.7.0.tar` & `sqlalchemy_easy_softdelete-0.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1497 2023-04-10 22:22:14.901077 sqlalchemy_easy_softdelete-0.7.0/LICENSE
--rw-r--r--   0        0        0     2877 2023-04-10 22:22:14.901077 sqlalchemy_easy_softdelete-0.7.0/README.md
--rw-r--r--   0        0        0     2314 2023-04-10 22:22:14.901077 sqlalchemy_easy_softdelete-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      140 2023-04-10 22:22:14.901077 sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/__init__.py
--rw-r--r--   0        0        0       65 2023-04-10 22:22:14.901077 sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/handler/__init__.py
--rw-r--r--   0        0        0     6089 2023-04-10 22:22:14.901077 sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py
--rw-r--r--   0        0        0      850 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py
--rw-r--r--   0        0        0     1623 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/mixin.py
--rw-r--r--   0        0        0       56 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     1971 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0     2580 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/model.py
--rw-r--r--   0        0        0      360 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/seed_data/__init__.py
--rw-r--r--   0        0        0     2025 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/seed_data/parent_child_childchild.py
--rw-r--r--   0        0        0        0 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/snapshots/__init__.py
--rw-r--r--   0        0        0     6518 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/snapshots/snap_test_queries.py
--rw-r--r--   0        0        0     9931 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/snapshots/snap_test_seed_data.py
--rw-r--r--   0        0        0     6340 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/test_queries.py
--rw-r--r--   0        0        0      595 2023-04-10 22:22:14.905077 sqlalchemy_easy_softdelete-0.7.0/tests/test_seed_data.py
--rw-r--r--   0        0        0     4557 1970-01-01 00:00:00.000000 sqlalchemy_easy_softdelete-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2875 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/README.md
+-rw-r--r--   0        0        0     2314 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      140 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/__init__.py
+-rw-r--r--   0        0        0       65 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/handler/__init__.py
+-rw-r--r--   0        0        0     6089 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py
+-rw-r--r--   0        0        0      850 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py
+-rw-r--r--   0        0        0     1623 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/mixin.py
+-rw-r--r--   0        0        0       56 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0     1971 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0     2580 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/tests/model.py
+-rw-r--r--   0        0        0      360 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/tests/seed_data/__init__.py
+-rw-r--r--   0        0        0     2025 2023-04-10 22:33:17.766859 sqlalchemy_easy_softdelete-0.7.1/tests/seed_data/parent_child_childchild.py
+-rw-r--r--   0        0        0        0 2023-04-10 22:33:17.770859 sqlalchemy_easy_softdelete-0.7.1/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0     6518 2023-04-10 22:33:17.770859 sqlalchemy_easy_softdelete-0.7.1/tests/snapshots/snap_test_queries.py
+-rw-r--r--   0        0        0     9931 2023-04-10 22:33:17.770859 sqlalchemy_easy_softdelete-0.7.1/tests/snapshots/snap_test_seed_data.py
+-rw-r--r--   0        0        0     6340 2023-04-10 22:33:17.770859 sqlalchemy_easy_softdelete-0.7.1/tests/test_queries.py
+-rw-r--r--   0        0        0      595 2023-04-10 22:33:17.770859 sqlalchemy_easy_softdelete-0.7.1/tests/test_seed_data.py
+-rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 sqlalchemy_easy_softdelete-0.7.1/PKG-INFO
```

### Comparing `sqlalchemy_easy_softdelete-0.7.0/LICENSE` & `sqlalchemy_easy_softdelete-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.0/README.md` & `sqlalchemy_easy_softdelete-0.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SQLAlchemy Easy Soft-Delete
 
 [![pypi](https://img.shields.io/pypi/v/sqlalchemy-easy-softdelete.svg)](https://pypi.org/project/sqlalchemy-easy-softdelete/)
 [![python](https://img.shields.io/pypi/pyversions/sqlalchemy-easy-softdelete.svg)](https://pypi.org/project/sqlalchemy-easy-softdelete/)
-[![Build Status](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/build.yml/badge.svg)](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/build.yml)
+[![Build Status](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test.yml/badge.svg)](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test.yml)
 
 [//]: # ([![codecov]&#40;https://codecov.io/gh/flipbit03/sqlalchemy-easy-softdelete/branch/main/graphs/badge.svg&#41;]&#40;https://codecov.io/github/flipbit03/sqlalchemy-easy-softdelete&#41;)
 
 Easily add soft-deletion to your SQLAlchemy Models and automatically filter out soft-deleted objects from your queries and relationships.
 
 This package can generate a tailor-made SQLAlchemy Mixin that can be added to your SQLAlchemy Models, making them contain a field that, when set, will mark the entity as being soft-deleted.
```

### Comparing `sqlalchemy_easy_softdelete-0.7.0/pyproject.toml` & `sqlalchemy_easy_softdelete-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "sqlalchemy-easy-softdelete"
-version = "0.7.0"
+version = "0.7.1"
 homepage = "https://github.com/flipbit03/sqlalchemy-easy-softdelete"
 description = "Easily add soft-deletion to your SQLAlchemy Models."
 authors = ["Cadu <cadu.coelho@gmail.com>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
```

### Comparing `sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py` & `sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py` & `sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.0/sqlalchemy_easy_softdelete/mixin.py` & `sqlalchemy_easy_softdelete-0.7.1/sqlalchemy_easy_softdelete/mixin.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.0/tests/conftest.py` & `sqlalchemy_easy_softdelete-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.0/tests/model.py` & `sqlalchemy_easy_softdelete-0.7.1/tests/model.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.0/tests/seed_data/parent_child_childchild.py` & `sqlalchemy_easy_softdelete-0.7.1/tests/seed_data/parent_child_childchild.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.0/tests/snapshots/snap_test_queries.py` & `sqlalchemy_easy_softdelete-0.7.1/tests/snapshots/snap_test_queries.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.0/tests/snapshots/snap_test_seed_data.py` & `sqlalchemy_easy_softdelete-0.7.1/tests/snapshots/snap_test_seed_data.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.0/tests/test_queries.py` & `sqlalchemy_easy_softdelete-0.7.1/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.0/tests/test_seed_data.py` & `sqlalchemy_easy_softdelete-0.7.1/tests/test_seed_data.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.0/PKG-INFO` & `sqlalchemy_easy_softdelete-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-easy-softdelete
-Version: 0.7.0
+Version: 0.7.1
 Summary: Easily add soft-deletion to your SQLAlchemy Models.
 Home-page: https://github.com/flipbit03/sqlalchemy-easy-softdelete
 License: BSD-3-Clause
 Author: Cadu
 Author-email: cadu.coelho@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -36,15 +36,15 @@
 Requires-Dist: virtualenv (>=20.2.2,<21.0.0) ; extra == "dev"
 Description-Content-Type: text/markdown
 
 # SQLAlchemy Easy Soft-Delete
 
 [![pypi](https://img.shields.io/pypi/v/sqlalchemy-easy-softdelete.svg)](https://pypi.org/project/sqlalchemy-easy-softdelete/)
 [![python](https://img.shields.io/pypi/pyversions/sqlalchemy-easy-softdelete.svg)](https://pypi.org/project/sqlalchemy-easy-softdelete/)
-[![Build Status](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/build.yml/badge.svg)](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/build.yml)
+[![Build Status](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test.yml/badge.svg)](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test.yml)
 
 [//]: # ([![codecov]&#40;https://codecov.io/gh/flipbit03/sqlalchemy-easy-softdelete/branch/main/graphs/badge.svg&#41;]&#40;https://codecov.io/github/flipbit03/sqlalchemy-easy-softdelete&#41;)
 
 Easily add soft-deletion to your SQLAlchemy Models and automatically filter out soft-deleted objects from your queries and relationships.
 
 This package can generate a tailor-made SQLAlchemy Mixin that can be added to your SQLAlchemy Models, making them contain a field that, when set, will mark the entity as being soft-deleted.
```

