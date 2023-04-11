# Comparing `tmp/wvpy-0.3.9.tar.gz` & `tmp/wvpy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wvpy-0.3.9.tar", last modified: Sun Jan 22 23:04:49 2023, max compression
+gzip compressed data, was "wvpy-0.4.0.tar", last modified: Tue Apr 11 19:43:16 2023, max compression
```

## Comparing `wvpy-0.3.9.tar` & `wvpy-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-01-22 23:04:49.854452 wvpy-0.3.9/
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-01-22 23:04:49.851079 wvpy-0.3.9/Doc/
--rw-r--r--   0 johnmount   (501) staff       (20)      108 2019-07-23 14:11:39.000000 wvpy-0.3.9/Doc/documentation.txt
--rw-r--r--   0 johnmount   (501) staff       (20)     1494 2019-07-23 14:35:20.000000 wvpy-0.3.9/LICENSE
--rw-r--r--   0 johnmount   (501) staff       (20)       82 2019-07-23 14:11:39.000000 wvpy-0.3.9/MANIFEST.in
--rw-r--r--   0 johnmount   (501) staff       (20)      995 2023-01-22 23:04:49.854207 wvpy-0.3.9/PKG-INFO
--rw-r--r--   0 johnmount   (501) staff       (20)      373 2022-12-29 19:46:58.000000 wvpy-0.3.9/README.txt
--rw-r--r--   0 johnmount   (501) staff       (20)       38 2023-01-22 23:04:49.854536 wvpy-0.3.9/setup.cfg
--rw-r--r--   0 johnmount   (501) staff       (20)     1367 2023-01-21 19:13:24.000000 wvpy-0.3.9/setup.py
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-01-22 23:04:49.852278 wvpy-0.3.9/wvpy/
--rw-r--r--   0 johnmount   (501) staff       (20)      173 2023-01-21 19:13:28.000000 wvpy-0.3.9/wvpy/__init__.py
--rw-r--r--   0 johnmount   (501) staff       (20)    17648 2023-01-22 18:12:56.000000 wvpy-0.3.9/wvpy/jtools.py
--rw-r--r--   0 johnmount   (501) staff       (20)     5898 2022-12-29 19:46:58.000000 wvpy-0.3.9/wvpy/pysheet.py
--rw-r--r--   0 johnmount   (501) staff       (20)     3234 2022-12-29 19:46:58.000000 wvpy-0.3.9/wvpy/render_workbook.py
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-01-22 23:04:49.853844 wvpy-0.3.9/wvpy.egg-info/
--rw-r--r--   0 johnmount   (501) staff       (20)      995 2023-01-22 23:04:49.000000 wvpy-0.3.9/wvpy.egg-info/PKG-INFO
--rw-r--r--   0 johnmount   (501) staff       (20)      272 2023-01-22 23:04:49.000000 wvpy-0.3.9/wvpy.egg-info/SOURCES.txt
--rw-r--r--   0 johnmount   (501) staff       (20)        1 2023-01-22 23:04:49.000000 wvpy-0.3.9/wvpy.egg-info/dependency_links.txt
--rw-r--r--   0 johnmount   (501) staff       (20)       69 2023-01-22 23:04:49.000000 wvpy-0.3.9/wvpy.egg-info/requires.txt
--rw-r--r--   0 johnmount   (501) staff       (20)        5 2023-01-22 23:04:49.000000 wvpy-0.3.9/wvpy.egg-info/top_level.txt
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-11 19:43:16.691479 wvpy-0.4.0/
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-11 19:43:16.687221 wvpy-0.4.0/Doc/
+-rw-r--r--   0 johnmount   (501) staff       (20)      108 2019-07-23 14:11:39.000000 wvpy-0.4.0/Doc/documentation.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)     1494 2019-07-23 14:35:20.000000 wvpy-0.4.0/LICENSE
+-rw-r--r--   0 johnmount   (501) staff       (20)       82 2019-07-23 14:11:39.000000 wvpy-0.4.0/MANIFEST.in
+-rw-r--r--   0 johnmount   (501) staff       (20)      995 2023-04-11 19:43:16.691229 wvpy-0.4.0/PKG-INFO
+-rw-r--r--   0 johnmount   (501) staff       (20)      373 2022-12-29 19:46:58.000000 wvpy-0.4.0/README.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)       38 2023-04-11 19:43:16.691553 wvpy-0.4.0/setup.cfg
+-rw-r--r--   0 johnmount   (501) staff       (20)     1367 2023-01-22 23:07:22.000000 wvpy-0.4.0/setup.py
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-11 19:43:16.689203 wvpy-0.4.0/wvpy/
+-rw-r--r--   0 johnmount   (501) staff       (20)      173 2023-01-22 23:07:08.000000 wvpy-0.4.0/wvpy/__init__.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    19223 2023-04-10 19:24:30.000000 wvpy-0.4.0/wvpy/jtools.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     5898 2022-12-29 19:46:58.000000 wvpy-0.4.0/wvpy/pysheet.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     3234 2022-12-29 19:46:58.000000 wvpy-0.4.0/wvpy/render_workbook.py
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-11 19:43:16.690815 wvpy-0.4.0/wvpy.egg-info/
+-rw-r--r--   0 johnmount   (501) staff       (20)      995 2023-04-11 19:43:16.000000 wvpy-0.4.0/wvpy.egg-info/PKG-INFO
+-rw-r--r--   0 johnmount   (501) staff       (20)      272 2023-04-11 19:43:16.000000 wvpy-0.4.0/wvpy.egg-info/SOURCES.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)        1 2023-04-11 19:43:16.000000 wvpy-0.4.0/wvpy.egg-info/dependency_links.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)       69 2023-04-11 19:43:16.000000 wvpy-0.4.0/wvpy.egg-info/requires.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)        5 2023-04-11 19:43:16.000000 wvpy-0.4.0/wvpy.egg-info/top_level.txt
```

### Comparing `wvpy-0.3.9/LICENSE` & `wvpy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wvpy-0.3.9/PKG-INFO` & `wvpy-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wvpy
-Version: 0.3.9
+Version: 0.4.0
 Summary: Convert Jupyter notebooks to and from Python files.
 Home-page: https://github.com/WinVector/wvpy
 Author: John Mount
 Author-email: jmount@win-vector.com
 License: License :: OSI Approved :: BSD 3-clause License
 Platform: any
 Classifier: Intended Audience :: Science/Research
```

### Comparing `wvpy-0.3.9/setup.py` & `wvpy-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 DESCRIPTION = "Convert Jupyter notebooks to and from Python files."
 LONG_DESCRIPTION = """
 Convert Jupyter notebooks to and from Python files.
 """
 
 setuptools.setup(
     name="wvpy",
-    version="0.3.9",
+    version="0.4.0",
     author="John Mount",
     author_email="jmount@win-vector.com",
     url="https://github.com/WinVector/wvpy",
     packages=setuptools.find_packages(exclude=['tests', 'Examples']),
     install_requires=[
         "IPython",
         "nbformat",
```

### Comparing `wvpy-0.3.9/wvpy/jtools.py` & `wvpy-0.4.0/wvpy/jtools.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 """Jupyter tools"""
 
 import re
 import datetime
 import os
 import nbformat
 import nbconvert.preprocessors
+from multiprocessing import Pool
+import sys
 
-from typing import Optional
+from typing import Iterable, Optional
 from functools import total_ordering
 
 have_pdf_kit = False
 try:
     import pdfkit
     have_pdf_kit = True
 except ModuleNotFoundError:
@@ -450,26 +452,73 @@
         ])
         return 'JTask(\n' + args_str + ",\n)"
 
     def __repr__(self) -> str:
         return self.__str__()
 
 
-def job_fn(arg: JTask):
+def job_fn(arg: JTask) -> None:
     """
     Function to run a JTask job
     """
     assert isinstance(arg, JTask)
     # render notebook
     arg.render_as_html()
 
 
-def job_fn_eat_exception(arg: JTask):
+def job_fn_eat_exception(arg: JTask) -> None:
     """
     Function to run a JTask job, eating any exception
     """
     assert isinstance(arg, JTask)
     # render notebook
     try:
         arg.render_as_html()
     except Exception as e:
         print(f"{arg} caught {e}")
+
+
+def run_pool(
+        tasks: Iterable, 
+        *, 
+        njobs: int = 4,
+        verbose: bool = True,
+        stop_on_error: bool = True,
+        ) -> None:
+    """
+    Run a pool of tasks.
+
+    :param tasks: iterable of tasks
+    :param njobs: degree of parallelism
+    :param verbose: if True, print on failure
+    :param stop_on_error: if True, stop pool on error
+    """
+    tasks = list(tasks)
+    assert isinstance(njobs, int)
+    assert njobs > 0
+    assert isinstance(verbose, bool)
+    assert isinstance(stop_on_error, bool)
+    if len(tasks) <= 0:
+        return
+    for task in tasks:
+        assert isinstance(task, JTask)
+    if stop_on_error:
+        # # complex way, allowing a stop on job failure
+        # https://stackoverflow.com/a/25791961/6901725
+        with Pool(njobs) as pool:
+            try:
+                list(pool.imap_unordered(job_fn, tasks))  # list is forcing iteration over tasks for side-effects
+            except Exception:
+                if verbose:
+                    sys.stdout.flush()
+                    print("!!! run_pool: a worker raised an Exception, aborting...")
+                    sys.stdout.flush()
+                pool.close()
+                pool.terminate()
+                raise  # re-raise Exception
+            else:
+                pool.close()
+                pool.join()
+    else:
+        # simple way, but doesn't exit until all jobs succeed or fail
+        with Pool(njobs) as pool:
+            pool.map(job_fn_eat_exception, tasks)
```

### Comparing `wvpy-0.3.9/wvpy/pysheet.py` & `wvpy-0.4.0/wvpy/pysheet.py`

 * *Files identical despite different names*

### Comparing `wvpy-0.3.9/wvpy/render_workbook.py` & `wvpy-0.4.0/wvpy/render_workbook.py`

 * *Files identical despite different names*

### Comparing `wvpy-0.3.9/wvpy.egg-info/PKG-INFO` & `wvpy-0.4.0/wvpy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wvpy
-Version: 0.3.9
+Version: 0.4.0
 Summary: Convert Jupyter notebooks to and from Python files.
 Home-page: https://github.com/WinVector/wvpy
 Author: John Mount
 Author-email: jmount@win-vector.com
 License: License :: OSI Approved :: BSD 3-clause License
 Platform: any
 Classifier: Intended Audience :: Science/Research
```

