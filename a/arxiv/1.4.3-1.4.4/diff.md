# Comparing `tmp/arxiv-1.4.3.tar.gz` & `tmp/arxiv-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arxiv-1.4.3.tar", last modified: Wed Feb  1 03:05:14 2023, max compression
+gzip compressed data, was "arxiv-1.4.4.tar", last modified: Tue Apr 11 01:17:31 2023, max compression
```

## Comparing `arxiv-1.4.3.tar` & `arxiv-1.4.4.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-02-01 03:05:14.000000 arxiv-1.4.3/
--rw-r--r--   0 lukas      (501) staff       (20)     1056 2018-08-22 17:46:13.000000 arxiv-1.4.3/LICENSE.txt
--rw-r--r--   0 lukas      (501) staff       (20)     7865 2023-02-01 03:05:14.000000 arxiv-1.4.3/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)     7363 2023-02-01 03:02:02.000000 arxiv-1.4.3/README.md
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-02-01 03:05:14.000000 arxiv-1.4.3/arxiv/
--rw-r--r--   0 lukas      (501) staff       (20)       35 2022-01-26 03:22:05.000000 arxiv-1.4.3/arxiv/__init__.py
--rw-r--r--   0 lukas      (501) staff       (20)    26566 2023-02-01 03:02:02.000000 arxiv-1.4.3/arxiv/arxiv.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-02-01 03:05:14.000000 arxiv-1.4.3/arxiv.egg-info/
--rw-r--r--   0 lukas      (501) staff       (20)     7865 2023-02-01 03:05:14.000000 arxiv-1.4.3/arxiv.egg-info/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)      217 2023-02-01 03:05:14.000000 arxiv-1.4.3/arxiv.egg-info/SOURCES.txt
--rw-r--r--   0 lukas      (501) staff       (20)        1 2023-02-01 03:05:14.000000 arxiv-1.4.3/arxiv.egg-info/dependency_links.txt
--rw-r--r--   0 lukas      (501) staff       (20)       11 2023-02-01 03:05:14.000000 arxiv-1.4.3/arxiv.egg-info/requires.txt
--rw-r--r--   0 lukas      (501) staff       (20)        6 2023-02-01 03:05:14.000000 arxiv-1.4.3/arxiv.egg-info/top_level.txt
--rw-r--r--   0 lukas      (501) staff       (20)      146 2023-02-01 03:05:14.000000 arxiv-1.4.3/setup.cfg
--rw-r--r--   0 lukas      (501) staff       (20)      890 2023-02-01 03:04:40.000000 arxiv-1.4.3/setup.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-11 01:17:31.047848 arxiv-1.4.4/
+-rw-r--r--   0 lukas      (501) staff       (20)     1056 2018-08-22 17:46:13.000000 arxiv-1.4.4/LICENSE.txt
+-rw-r--r--   0 lukas      (501) staff       (20)     7865 2023-04-11 01:17:31.047993 arxiv-1.4.4/PKG-INFO
+-rw-r--r--   0 lukas      (501) staff       (20)     7363 2023-03-12 19:09:15.000000 arxiv-1.4.4/README.md
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-11 01:17:31.040815 arxiv-1.4.4/arxiv/
+-rw-r--r--   0 lukas      (501) staff       (20)       35 2022-01-26 03:22:05.000000 arxiv-1.4.4/arxiv/__init__.py
+-rw-r--r--   0 lukas      (501) staff       (20)    26550 2023-04-11 01:15:41.000000 arxiv-1.4.4/arxiv/arxiv.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-11 01:17:31.044483 arxiv-1.4.4/arxiv.egg-info/
+-rw-r--r--   0 lukas      (501) staff       (20)     7865 2023-04-11 01:17:30.000000 arxiv-1.4.4/arxiv.egg-info/PKG-INFO
+-rw-r--r--   0 lukas      (501) staff       (20)      305 2023-04-11 01:17:30.000000 arxiv-1.4.4/arxiv.egg-info/SOURCES.txt
+-rw-r--r--   0 lukas      (501) staff       (20)        1 2023-04-11 01:17:30.000000 arxiv-1.4.4/arxiv.egg-info/dependency_links.txt
+-rw-r--r--   0 lukas      (501) staff       (20)       11 2023-04-11 01:17:30.000000 arxiv-1.4.4/arxiv.egg-info/requires.txt
+-rw-r--r--   0 lukas      (501) staff       (20)        6 2023-04-11 01:17:30.000000 arxiv-1.4.4/arxiv.egg-info/top_level.txt
+-rw-r--r--   0 lukas      (501) staff       (20)      146 2023-04-11 01:17:31.048848 arxiv-1.4.4/setup.cfg
+-rw-r--r--   0 lukas      (501) staff       (20)      890 2023-04-11 01:15:41.000000 arxiv-1.4.4/setup.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-11 01:17:31.047298 arxiv-1.4.4/tests/
+-rw-r--r--   0 lukas      (501) staff       (20)     1008 2021-08-18 02:16:12.000000 arxiv-1.4.4/tests/test_api_bugs.py
+-rw-r--r--   0 lukas      (501) staff       (20)     7417 2023-02-01 03:02:02.000000 arxiv-1.4.4/tests/test_client.py
+-rw-r--r--   0 lukas      (501) staff       (20)     1213 2022-01-26 03:22:05.000000 arxiv-1.4.4/tests/test_download.py
+-rw-r--r--   0 lukas      (501) staff       (20)     4098 2021-08-18 02:16:12.000000 arxiv-1.4.4/tests/test_result.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `arxiv-1.4.3/LICENSE.txt` & `arxiv-1.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arxiv-1.4.3/PKG-INFO` & `arxiv-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python wrapper for the arXiv API: http://arxiv.org/help/api/
 Home-page: https://github.com/lukasschwab/arxiv.py
 Author: Lukas Schwab
 Author-email: lukas.schwab@gmail.com
 License: MIT
 Keywords: arxiv api wrapper academic journals papers
 Classifier: Programming Language :: Python
```

### Comparing `arxiv-1.4.3/README.md` & `arxiv-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `arxiv-1.4.3/arxiv/arxiv.py` & `arxiv-1.4.4/arxiv/arxiv.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
     See [the arXiv API User's Manual: Details of Atom Results
     Returned](https://arxiv.org/help/api/user-manual#_details_of_atom_results_returned).
     """
 
     entry_id: str
     """A url of the form `http://arxiv.org/abs/{id}`."""
-    updated: time.struct_time
+    updated: datetime
     """When the result was last updated."""
-    published: time.struct_time
+    published: datetime
     """When the result was originally published."""
     title: str
     """The title of the result."""
     authors: list
     """The result's authors."""
     summary: str
     """The result abstract."""
```

### Comparing `arxiv-1.4.3/arxiv.egg-info/PKG-INFO` & `arxiv-1.4.4/arxiv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python wrapper for the arXiv API: http://arxiv.org/help/api/
 Home-page: https://github.com/lukasschwab/arxiv.py
 Author: Lukas Schwab
 Author-email: lukas.schwab@gmail.com
 License: MIT
 Keywords: arxiv api wrapper academic journals papers
 Classifier: Programming Language :: Python
```

### Comparing `arxiv-1.4.3/setup.py` & `arxiv-1.4.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '1.4.3'
+version = '1.4.4'
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='arxiv',
     version=version,
```

