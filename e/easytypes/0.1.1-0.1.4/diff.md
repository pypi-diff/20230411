# Comparing `tmp/easytypes-0.1.1.tar.gz` & `tmp/easytypes-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytypes-0.1.1.tar", max compression
+gzip compressed data, was "easytypes-0.1.4.tar", max compression
```

## Comparing `easytypes-0.1.1.tar` & `easytypes-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-04-11 17:37:20.003235 easytypes-0.1.1/LICENSE
--rw-r--r--   0        0        0     2627 2023-04-11 17:37:20.003235 easytypes-0.1.1/README.md
--rw-r--r--   0        0        0      318 2023-04-11 17:37:20.003235 easytypes-0.1.1/easytypes/__init__.py
--rw-r--r--   0        0        0     4508 2023-04-11 17:37:20.003235 easytypes-0.1.1/easytypes/easytypes_impl.py
--rw-r--r--   0        0        0     4639 2023-04-11 17:37:20.003235 easytypes-0.1.1/easytypes/easytypes_test.py
--rw-r--r--   0        0        0      810 2023-04-11 17:37:20.007235 easytypes-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3575 1970-01-01 00:00:00.000000 easytypes-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-11 17:45:42.817317 easytypes-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2627 2023-04-11 17:45:42.817317 easytypes-0.1.4/README.md
+-rw-r--r--   0        0        0      368 2023-04-11 17:45:42.817317 easytypes-0.1.4/easytypes/__init__.py
+-rw-r--r--   0        0        0     4508 2023-04-11 17:45:42.817317 easytypes-0.1.4/easytypes/easytypes_impl.py
+-rw-r--r--   0        0        0     4639 2023-04-11 17:45:42.817317 easytypes-0.1.4/easytypes/easytypes_test.py
+-rw-r--r--   0        0        0      814 2023-04-11 17:45:42.817317 easytypes-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3530 1970-01-01 00:00:00.000000 easytypes-0.1.4/PKG-INFO
```

### Comparing `easytypes-0.1.1/LICENSE` & `easytypes-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easytypes-0.1.1/README.md` & `easytypes-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `easytypes-0.1.1/easytypes/easytypes_impl.py` & `easytypes-0.1.4/easytypes/easytypes_impl.py`

 * *Files identical despite different names*

### Comparing `easytypes-0.1.1/easytypes/easytypes_test.py` & `easytypes-0.1.4/easytypes/easytypes_test.py`

 * *Files identical despite different names*

### Comparing `easytypes-0.1.1/pyproject.toml` & `easytypes-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "easytypes"
-version = "0.1.1"
+version = "0.1.4"
 description = "Easy declaration of data structures with runtime type checking"
 authors = ["Reim, Elijah <Elijah.Reim@wartsila.com>"]
-license = "Apache"
+license = "Apache-2.0"
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `easytypes-0.1.1/PKG-INFO` & `easytypes-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: easytypes
-Version: 0.1.1
+Version: 0.1.4
 Summary: Easy declaration of data structures with runtime type checking
-License: Apache
+License: Apache-2.0
 Author: Reim, Elijah
 Author-email: Elijah.Reim@wartsila.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

