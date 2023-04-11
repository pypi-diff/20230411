# Comparing `tmp/collection_framework_taa-0.0.2.tar.gz` & `tmp/collection_framework_taa-0.0.3.tar.gz`

## Comparing `collection_framework_taa-0.0.2.tar` & `collection_framework_taa-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/.flake8
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/.pytest_cache/README.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/src/collect_framework.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/collection_framework_taa/__init__.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/collection_framework_taa/cli.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/collection_framework_taa/collect_framework.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/collection_framework_taa/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/tests/cli_test.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/tests/collect_framework_test.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/LICENSE
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/README.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/.flake8
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/.pytest_cache/README.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/src/collect_framework.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/collection_framework_taa/__init__.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/collection_framework_taa/cli.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/collection_framework_taa/collect_framework.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/collection_framework_taa/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/tests/cli_test.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/tests/collect_framework_test.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/LICENSE
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/README.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 collection_framework_taa-0.0.3/PKG-INFO
```

### Comparing `collection_framework_taa-0.0.2/.pytest_cache/v/cache/nodeids` & `collection_framework_taa-0.0.3/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `collection_framework_taa-0.0.2/collection_framework_taa/cli.py` & `collection_framework_taa-0.0.3/collection_framework_taa/cli.py`

 * *Files identical despite different names*

### Comparing `collection_framework_taa-0.0.2/collection_framework_taa/collect_framework.py` & `collection_framework_taa-0.0.3/collection_framework_taa/collect_framework.py`

 * *Files identical despite different names*

### Comparing `collection_framework_taa-0.0.2/tests/cli_test.py` & `collection_framework_taa-0.0.3/tests/cli_test.py`

 * *Files identical despite different names*

### Comparing `collection_framework_taa-0.0.2/tests/collect_framework_test.py` & `collection_framework_taa-0.0.3/tests/collect_framework_test.py`

 * *Files identical despite different names*

### Comparing `collection_framework_taa-0.0.2/LICENSE` & `collection_framework_taa-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `collection_framework_taa-0.0.2/pyproject.toml` & `collection_framework_taa-0.0.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "collection_framework_taa"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "Unique symbols counter"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `collection_framework_taa-0.0.2/PKG-INFO` & `collection_framework_taa-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: collection_framework_taa
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unique symbols counter
 Author-email: Example Author <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Collection Framework
 
 
 Takes a string and returns the number of unique characters
 
-##Installations
+## Installations
 Install the package
 
-##Example of use
+## Example of use
 ``` 
 from collection_framework.cli import get_result
 
 if __name__ == "__main__":
     print(get_result())
 
 ```
-##Launch
+## Launch
 Рass a string as a parameter '--string'
 ```
 python3 {script_name} --string {string}
 ```
 or 
 pass the path to the file as a parameter '--file'
```

