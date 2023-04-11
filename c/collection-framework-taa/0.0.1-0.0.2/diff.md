# Comparing `tmp/collection_framework_taa-0.0.1.tar.gz` & `tmp/collection_framework_taa-0.0.2.tar.gz`

## Comparing `collection_framework_taa-0.0.1.tar` & `collection_framework_taa-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/.flake8
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/.pytest_cache/README.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/src/collect_framework.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/collection_framework_taa/__init__.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/collection_framework_taa/cli.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/collection_framework_taa/collect_framework.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/collection_framework_taa/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/tests/cli_test.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/tests/collect_framework_test.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/LICENSE
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/README.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/.flake8
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/src/collect_framework.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/collection_framework_taa/__init__.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/collection_framework_taa/cli.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/collection_framework_taa/collect_framework.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/collection_framework_taa/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/tests/cli_test.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/tests/collect_framework_test.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/LICENSE
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/README.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/PKG-INFO
```

### Comparing `collection_framework_taa-0.0.1/.pytest_cache/v/cache/nodeids` & `collection_framework_taa-0.0.2/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `collection_framework_taa-0.0.1/collection_framework_taa/cli.py` & `collection_framework_taa-0.0.2/collection_framework_taa/cli.py`

 * *Files identical despite different names*

### Comparing `collection_framework_taa-0.0.1/collection_framework_taa/collect_framework.py` & `collection_framework_taa-0.0.2/collection_framework_taa/collect_framework.py`

 * *Files identical despite different names*

### Comparing `collection_framework_taa-0.0.1/tests/cli_test.py` & `collection_framework_taa-0.0.2/tests/cli_test.py`

 * *Files identical despite different names*

### Comparing `collection_framework_taa-0.0.1/tests/collect_framework_test.py` & `collection_framework_taa-0.0.2/tests/collect_framework_test.py`

 * *Files identical despite different names*

### Comparing `collection_framework_taa-0.0.1/LICENSE` & `collection_framework_taa-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `collection_framework_taa-0.0.1/pyproject.toml` & `collection_framework_taa-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "collection_framework_taa"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "Unique symbols counter"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

