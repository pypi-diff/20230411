# Comparing `tmp/np_zro-0.1.0.post1.tar.gz` & `tmp/np_zro-0.1.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_zro-0.1.0.post1.tar", last modified: Mon Apr 10 22:04:24 2023, max compression
+gzip compressed data, was "np_zro-0.1.0.post2.tar", last modified: Mon Apr 10 22:27:25 2023, max compression
```

## Comparing `np_zro-0.1.0.post1.tar` & `np_zro-0.1.0.post2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      664 2023-04-10 21:58:24.949622 np_zro-0.1.0.post1/README.md
--rw-r--r--   0        0        0     1492 2023-04-10 22:04:24.031085 np_zro-0.1.0.post1/pyproject.toml
--rw-r--r--   0        0        0       24 2023-04-10 21:41:03.103623 np_zro-0.1.0.post1/src/np_zro/__init__.py
--rw-r--r--   0        0        0    10397 2023-04-10 21:45:19.493620 np_zro-0.1.0.post1/src/np_zro/zro.py
--rw-r--r--   0        0        0       93 2023-04-10 21:57:56.464360 np_zro-0.1.0.post1/tests/test_readme.py
--rw-r--r--   0        0        0      360 2023-04-10 21:59:06.060121 np_zro-0.1.0.post1/tests/test_zro.py
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 np_zro-0.1.0.post1/PKG-INFO
+-rw-r--r--   0        0        0      664 2023-04-10 21:58:24.949622 np_zro-0.1.0.post2/README.md
+-rw-r--r--   0        0        0     1492 2023-04-10 22:27:25.320849 np_zro-0.1.0.post2/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-04-10 21:41:03.103623 np_zro-0.1.0.post2/src/np_zro/__init__.py
+-rw-r--r--   0        0        0    10397 2023-04-10 21:45:19.493620 np_zro-0.1.0.post2/src/np_zro/zro.py
+-rw-r--r--   0        0        0      812 2023-04-10 22:26:57.275597 np_zro-0.1.0.post2/tests/test_install.py
+-rw-r--r--   0        0        0       93 2023-04-10 21:57:56.464360 np_zro-0.1.0.post2/tests/test_readme.py
+-rw-r--r--   0        0        0      360 2023-04-10 21:59:06.060121 np_zro-0.1.0.post2/tests/test_zro.py
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 np_zro-0.1.0.post2/PKG-INFO
```

### Comparing `np_zro-0.1.0.post1/README.md` & `np_zro-0.1.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `np_zro-0.1.0.post1/pyproject.toml` & `np_zro-0.1.0.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np_zro"
-version = "0.1.0.post1"
+version = "0.1.0.post2"
 description = "Just the `zro.Proxy` class extracted from `mpeconfig`, with `zmq` as a dependency."
 authors = [
     { name = "derricw", email = "derricw@alleninstitute.org" },
     { name = "rossh", email = "rossh@alleninstitute.org" },
 ]
 maintainers = [
     { name = "bjhardcastle", email = "ben.hardcastle@alleninstitute.org" },
```

### Comparing `np_zro-0.1.0.post1/src/np_zro/zro.py` & `np_zro-0.1.0.post2/src/np_zro/zro.py`

 * *Files identical despite different names*

### Comparing `np_zro-0.1.0.post1/PKG-INFO` & `np_zro-0.1.0.post2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-zro
-Version: 0.1.0.post1
+Version: 0.1.0.post2
 Summary: Just the `zro.Proxy` class extracted from `mpeconfig`, with `zmq` as a dependency.
 Author-Email: derricw <derricw@alleninstitute.org>, rossh <rossh@alleninstitute.org>
 Maintainer-Email: bjhardcastle <ben.hardcastle@alleninstitute.org>
 Requires-Python: >=3.7
 Requires-Dist: zmq>=0.0.0
 Requires-Dist: typing-extensions>=4.5.0
 Description-Content-Type: text/markdown
```

