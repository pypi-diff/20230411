# Comparing `tmp/np_zro-0.1.0.post2.tar.gz` & `tmp/np_zro-0.1.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_zro-0.1.0.post2.tar", last modified: Mon Apr 10 22:27:25 2023, max compression
+gzip compressed data, was "np_zro-0.1.0.post4.tar", last modified: Tue Apr 11 06:06:30 2023, max compression
```

## Comparing `np_zro-0.1.0.post2.tar` & `np_zro-0.1.0.post4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      664 2023-04-10 21:58:24.949622 np_zro-0.1.0.post2/README.md
--rw-r--r--   0        0        0     1492 2023-04-10 22:27:25.320849 np_zro-0.1.0.post2/pyproject.toml
--rw-r--r--   0        0        0       24 2023-04-10 21:41:03.103623 np_zro-0.1.0.post2/src/np_zro/__init__.py
--rw-r--r--   0        0        0    10397 2023-04-10 21:45:19.493620 np_zro-0.1.0.post2/src/np_zro/zro.py
--rw-r--r--   0        0        0      812 2023-04-10 22:26:57.275597 np_zro-0.1.0.post2/tests/test_install.py
--rw-r--r--   0        0        0       93 2023-04-10 21:57:56.464360 np_zro-0.1.0.post2/tests/test_readme.py
--rw-r--r--   0        0        0      360 2023-04-10 21:59:06.060121 np_zro-0.1.0.post2/tests/test_zro.py
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 np_zro-0.1.0.post2/PKG-INFO
+-rw-r--r--   0        0        0      664 2023-04-10 21:58:24.949622 np_zro-0.1.0.post4/README.md
+-rw-r--r--   0        0        0     1918 2023-04-11 06:06:30.108058 np_zro-0.1.0.post4/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-04-10 21:41:03.103623 np_zro-0.1.0.post4/src/np_zro/__init__.py
+-rw-r--r--   0        0        0    10397 2023-04-10 21:45:19.493620 np_zro-0.1.0.post4/src/np_zro/zro.py
+-rw-r--r--   0        0        0      812 2023-04-10 22:26:57.275597 np_zro-0.1.0.post4/tests/test_install.py
+-rw-r--r--   0        0        0       93 2023-04-10 21:57:56.464360 np_zro-0.1.0.post4/tests/test_readme.py
+-rw-r--r--   0        0        0      360 2023-04-10 21:59:06.060121 np_zro-0.1.0.post4/tests/test_zro.py
+-rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 np_zro-0.1.0.post4/PKG-INFO
```

### Comparing `np_zro-0.1.0.post2/README.md` & `np_zro-0.1.0.post4/README.md`

 * *Files identical despite different names*

### Comparing `np_zro-0.1.0.post2/pyproject.toml` & `np_zro-0.1.0.post4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 [project]
 name = "np_zro"
-version = "0.1.0.post2"
+version = "0.1.0.post4"
 description = "Just the `zro.Proxy` class extracted from `mpeconfig`, with `zmq` as a dependency."
 authors = [
     { name = "derricw", email = "derricw@alleninstitute.org" },
     { name = "rossh", email = "rossh@alleninstitute.org" },
 ]
 maintainers = [
     { name = "bjhardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "zmq>=0.0.0",
     "typing-extensions>=4.5.0",
 ]
 requires-python = ">=3.7"
 readme = "README.md"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
+
+[project.urls]
+Repository = "https://github.com/AllenInstitute/np_zro"
+"Bug Tracker" = "https://github.com/AllenInstitute/np_zro/issues"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `np_zro-0.1.0.post2/src/np_zro/zro.py` & `np_zro-0.1.0.post4/src/np_zro/zro.py`

 * *Files identical despite different names*

### Comparing `np_zro-0.1.0.post2/tests/test_install.py` & `np_zro-0.1.0.post4/tests/test_install.py`

 * *Files identical despite different names*

