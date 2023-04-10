# Comparing `tmp/pysparkler-0.3.dev1681163476.tar.gz` & `tmp/pysparkler-0.3.dev1681170435.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.3.dev1681163476.tar", max compression
+gzip compressed data, was "pysparkler-0.3.dev1681170435.tar", max compression
```

## Comparing `pysparkler-0.3.dev1681163476.tar` & `pysparkler-0.3.dev1681170435.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4137 2023-04-10 21:51:10.408723 pysparkler-0.3.dev1681163476/README.md
--rw-r--r--   0        0        0     1188 2023-04-10 21:51:17.368817 pysparkler-0.3.dev1681163476/pyproject.toml
--rw-r--r--   0        0        0      807 2023-04-10 21:51:10.408723 pysparkler-0.3.dev1681163476/pysparkler/__init__.py
--rw-r--r--   0        0        0     4142 2023-04-10 21:51:10.408723 pysparkler-0.3.dev1681163476/pysparkler/api.py
--rw-r--r--   0        0        0     3940 2023-04-10 21:51:10.408723 pysparkler-0.3.dev1681163476/pysparkler/base.py
--rw-r--r--   0        0        0     5681 2023-04-10 21:51:10.408723 pysparkler-0.3.dev1681163476/pysparkler/cli.py
--rw-r--r--   0        0        0    12402 2023-04-10 21:51:10.408723 pysparkler-0.3.dev1681163476/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3967 2023-04-10 21:51:10.408723 pysparkler-0.3.dev1681163476/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     5001 1970-01-01 00:00:00.000000 pysparkler-0.3.dev1681163476/PKG-INFO
+-rw-r--r--   0        0        0     4137 2023-04-10 23:47:08.877658 pysparkler-0.3.dev1681170435/README.md
+-rw-r--r--   0        0        0     1188 2023-04-10 23:47:15.753835 pysparkler-0.3.dev1681170435/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-04-10 23:47:08.877658 pysparkler-0.3.dev1681170435/pysparkler/__init__.py
+-rw-r--r--   0        0        0     4142 2023-04-10 23:47:08.877658 pysparkler-0.3.dev1681170435/pysparkler/api.py
+-rw-r--r--   0        0        0     3940 2023-04-10 23:47:08.877658 pysparkler-0.3.dev1681170435/pysparkler/base.py
+-rw-r--r--   0        0        0     5681 2023-04-10 23:47:08.881658 pysparkler-0.3.dev1681170435/pysparkler/cli.py
+-rw-r--r--   0        0        0    12402 2023-04-10 23:47:08.881658 pysparkler-0.3.dev1681170435/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3967 2023-04-10 23:47:08.881658 pysparkler-0.3.dev1681170435/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     5001 1970-01-01 00:00:00.000000 pysparkler-0.3.dev1681170435/PKG-INFO
```

### Comparing `pysparkler-0.3.dev1681163476/README.md` & `pysparkler-0.3.dev1681170435/README.md`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1681163476/pyproject.toml` & `pysparkler-0.3.dev1681170435/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.3.dev1681163476"
+version = "0.3.dev1681170435"
 description = "A tool that upgrades your PySpark scripts to Spark 3.3 as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
```

### Comparing `pysparkler-0.3.dev1681163476/pysparkler/__init__.py` & `pysparkler-0.3.dev1681170435/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1681163476/pysparkler/api.py` & `pysparkler-0.3.dev1681170435/pysparkler/api.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1681163476/pysparkler/base.py` & `pysparkler-0.3.dev1681170435/pysparkler/base.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1681163476/pysparkler/cli.py` & `pysparkler-0.3.dev1681170435/pysparkler/cli.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1681163476/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.3.dev1681170435/pysparkler/pyspark_24_to_30.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1681163476/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.3.dev1681170435/pysparkler/pyspark_31_to_32.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1681163476/PKG-INFO` & `pysparkler-0.3.dev1681170435/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.3.dev1681163476
+Version: 0.3.dev1681170435
 Summary: A tool that upgrades your PySpark scripts to Spark 3.3 as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
```

