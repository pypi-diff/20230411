# Comparing `tmp/noprint-3.0.0.tar.gz` & `tmp/noprint-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noprint-3.0.0.tar", last modified: Sat Apr  8 21:23:14 2023, max compression
+gzip compressed data, was "noprint-3.1.0.tar", last modified: Tue Apr 11 20:15:40 2023, max compression
```

## Comparing `noprint-3.0.0.tar` & `noprint-3.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:23:14.370231 noprint-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-08 21:23:02.000000 noprint-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-08 21:23:14.370231 noprint-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-04-08 21:23:02.000000 noprint-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-08 21:23:02.000000 noprint-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 21:23:14.370231 noprint-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:23:14.366231 noprint-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:23:14.370231 noprint-3.0.0/src/noprint/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-08 21:23:02.000000 noprint-3.0.0/src/noprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-08 21:23:02.000000 noprint-3.0.0/src/noprint/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-08 21:23:02.000000 noprint-3.0.0/src/noprint/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-08 21:23:02.000000 noprint-3.0.0/src/noprint/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-08 21:23:02.000000 noprint-3.0.0/src/noprint/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-04-08 21:23:02.000000 noprint-3.0.0/src/noprint/sprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:23:14.370231 noprint-3.0.0/src/noprint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-08 21:23:14.000000 noprint-3.0.0/src/noprint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-08 21:23:14.000000 noprint-3.0.0/src/noprint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:23:14.000000 noprint-3.0.0/src/noprint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-08 21:23:14.000000 noprint-3.0.0/src/noprint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-08 21:23:14.000000 noprint-3.0.0/src/noprint.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:23:14.370231 noprint-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-08 21:23:02.000000 noprint-3.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-08 21:23:02.000000 noprint-3.0.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-04-08 21:23:02.000000 noprint-3.0.0/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-08 21:23:02.000000 noprint-3.0.0/tests/test_sprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:15:40.868286 noprint-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-11 20:15:26.000000 noprint-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-11 20:15:40.868286 noprint-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-04-11 20:15:26.000000 noprint-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-11 20:15:26.000000 noprint-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 20:15:40.868286 noprint-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:15:40.864286 noprint-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:15:40.864286 noprint-3.1.0/src/noprint/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-11 20:15:26.000000 noprint-3.1.0/src/noprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-11 20:15:26.000000 noprint-3.1.0/src/noprint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-11 20:15:26.000000 noprint-3.1.0/src/noprint/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-11 20:15:26.000000 noprint-3.1.0/src/noprint/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-11 20:15:26.000000 noprint-3.1.0/src/noprint/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-04-11 20:15:26.000000 noprint-3.1.0/src/noprint/sprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:15:40.868286 noprint-3.1.0/src/noprint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-11 20:15:40.000000 noprint-3.1.0/src/noprint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-11 20:15:40.000000 noprint-3.1.0/src/noprint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:15:40.000000 noprint-3.1.0/src/noprint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 20:15:40.000000 noprint-3.1.0/src/noprint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 20:15:40.000000 noprint-3.1.0/src/noprint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:15:40.868286 noprint-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-11 20:15:26.000000 noprint-3.1.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-11 20:15:26.000000 noprint-3.1.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-04-11 20:15:26.000000 noprint-3.1.0/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-11 20:15:26.000000 noprint-3.1.0/tests/test_sprint.py
```

### Comparing `noprint-3.0.0/LICENSE` & `noprint-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `noprint-3.0.0/PKG-INFO` & `noprint-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noprint
-Version: 3.0.0
+Version: 3.1.0
 Summary: Do not allow prints in your code
 Author-email: Radoslaw Gryta <radek.gryta@gmail.com>
 Project-URL: Homepage, https://github.com/rgryta/NoPrint
 Project-URL: Bug Tracker, https://github.com/rgryta/NoPrint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: noprint Version: 3.0.0 Summary: Do not allow prints
+Metadata-Version: 2.1 Name: noprint Version: 3.1.0 Summary: Do not allow prints
 in your code Author-email: Radoslaw Gryta
 gryta@gmail.com> Project-URL: Homepage, https://github.com/rgryta/NoPrint
 Project-URL: Bug Tracker, https://github.com/rgryta/NoPrint/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
      [https://raw.githubusercontent.com/rgryta/NoPrint/main/docs/logo.png]
```

### Comparing `noprint-3.0.0/README.md` & `noprint-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `noprint-3.0.0/pyproject.toml` & `noprint-3.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "noprint"
-version = "3.0.0"
+version = "3.1.0"
 authors = [
   { name="Radoslaw Gryta", email="radek.gryta@gmail.com" },
 ]
 description = "Do not allow prints in your code"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `noprint-3.0.0/src/noprint/logger.py` & `noprint-3.1.0/src/noprint/logger.py`

 * *Files identical despite different names*

### Comparing `noprint-3.0.0/src/noprint/module.py` & `noprint-3.1.0/src/noprint/module.py`

 * *Files identical despite different names*

### Comparing `noprint-3.0.0/src/noprint/sprint.py` & `noprint-3.1.0/src/noprint/sprint.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,34 @@
 Module responsible for finding print statements in python modules
 """
 import os
 import re
 import ast
 import pkgutil
 import functools
-from typing import Tuple
+import contextvars
 from pathlib import Path
 from multiprocessing.pool import Pool
 
 import noprint.logger as logging
 
 from noprint import ENCODING_CAPTURE
 from noprint.module import Module
 from noprint.exceptions import ImportException, ParentModuleNotFoundException
 
 
-def _get_module(package, verbose):
+packages = contextvars.ContextVar("packages", default=[])
+mt_threads = contextvars.ContextVar("mt_threads", default=1)
+log_lvl = contextvars.ContextVar("log_lvl", default=logging.WARNING)
+first_only = contextvars.ContextVar("first_only", default=False)
+verbose = contextvars.ContextVar("verbose", default=False)
+very_verbose = contextvars.ContextVar("very_verbose", default=False)
+
+
+def _get_module(package):
     """Get Module of the package"""
     try:
         module = Module(package)
     except ParentModuleNotFoundException as exc:
         raise ImportException(exc) from exc
     if not module:
         raise ImportException(
@@ -30,30 +38,32 @@
 
     system_module = None
     try:
         system_module = Module(package, in_cwd=False)
     except ParentModuleNotFoundException:  # pragma: no cover
         pass
 
-    if not system_module and verbose:
-        logging.log(f"Module [{package}] is not installed", logging.WARNING)
+    if not system_module and verbose.get():
+        logging.log(
+            f"Module [{package}] is not installed", logging.WARNING
+        )  # pragma: no cover
     elif (
-        module != system_module
+        verbose.get()
         and system_module
+        and module != system_module
         and len(system_module.origin) > 0
-        and verbose
-    ):
+    ):  # pragma: no cover
         logging.log(
             f"Module [{package}] is overshadowing installed module", logging.WARNING
         )
 
     return module
 
 
-def _get_subpackages(package, verbose, module):
+def _get_subpackages(package, module):
     """Get all candidates for submodules"""
     # If module is a file or contains __init__ then yield it and set flag
     isinit = False
     if module.origin:
         candidates = [Path(orig).name for orig in module.origin]
         isinit = "__init__.py" in candidates
 
@@ -70,149 +80,146 @@
             ]
             sub_pkgs = [
                 ".".join([package, name])
                 for _, name, _ in pkgutil.iter_modules([pkg_path])
             ]
     # If submodule is a directory and doesn't contain __init__ raise Warning
     candidates_missing = set(candidates) - set(sub_pkgs)
-    if isinit and candidates_missing and verbose:
+    if isinit and candidates_missing and verbose.get():  # pragma: no cover
         for candidate in candidates_missing:
             logging.log(f"Module [{candidate}] has no __init__.py", logging.WARNING)
     # Patch missing submodules
     return list(set(candidates) | set(sub_pkgs))
 
 
-def _parse_module(package: str, verbose: bool = False):
+def _parse_module(package: str):
     """Grab all packages and subpackages"""
-    module = _get_module(package, verbose)
+    module = _get_module(package)
 
-    sub_pkgs = _get_subpackages(package, verbose, module)
+    sub_pkgs = _get_subpackages(package, module)
 
     funcs = []
     for pkg in sub_pkgs:
-        funcs = funcs + [functools.partial(_parse_module, package=pkg, verbose=verbose)]
+        funcs = funcs + [functools.partial(_parse_module, package=pkg)]
     return module if module.origin else None, funcs
 
 
-def _parse_pyfile(module, first_only):
+def _parse_pyfile(module):
     """Method for parsing python source code files to look for prints"""
     if isinstance(module, ImportException):
-        return ([], module)
+        logging.log(module.args[0], logging.CRITICAL)
+        return 2
 
-    prints = []
     encoding = "utf-8"
+    status = 0
     # First two lines of Python source code have to be ASCII compatible
     # PEP-8, PEP-263, PEP-3120
     for mod_file in module.origin:
         with open(mod_file, "r", encoding="utf-8") as file:
             for _ in range(2):  # Check 1st two lines
                 try:
                     found = re.search(ENCODING_CAPTURE, file.readline())
+                # pylint: disable=broad-exception-caught
                 except Exception as exc:  # pragma: no cover
-                    raise exc
+                    logging.log(exc.args[0], logging.CRITICAL)
+                    return 2
                 if found:
                     encoding = found.group(1)
                     break
 
         with open(mod_file, "r", encoding=encoding) as file:
             parsed = ast.parse(file.read())
             clear = True
             name = ""
             if mod_file.endswith("__init__.py") or mod_file.endswith("__main__.py"):
                 name = f".{mod_file[-11:-3]}"  # pragma: no cover
             for node in ast.walk(parsed):
                 if node.__dict__.get("id") == "print":
                     clear = False
-
-                    prints.append(
-                        (
-                            f"[{module.name}{name}] Line: {node.lineno}",
-                            True,
+                    status = 1
+                    if verbose.get():  # pragma: no cover
+                        logging.log(
+                            f"[{module.name}{name}] Line: {node.lineno}", log_lvl.get()
                         )
-                    )
-                    if first_only:
-                        return (prints, None)
-            if clear:
-                prints.append(
-                    (
-                        f"[CLEAR]:[{module.name}{name}]",
-                        False,
-                    )
-                )
-    return (prints, None)
+
+                    if first_only.get():  # pragma: no cover
+                        return status
+            if clear and very_verbose.get():
+                logging.log(
+                    f"[CLEAR]:[{module.name}{name}]", logging.INFO
+                )  # pragma: no cover
+    return status
 
 
 class PackageFinder:
     """Class responsible for finding all packages and handling multiprocessing"""
 
     processes = []
     results = []
 
-    def __init__(self, threads):  # pragma: no cover
-        self.pool = Pool(threads)
+    def __init__(self):  # pragma: no cover
+        self.pool = Pool(mt_threads.get())
 
     def err_callback(self, exc):  # pragma: no cover
         """Error callback from searching module"""
         self.results.append(exc)
 
     def callback(self, res):  # pragma: no cover
         """Callback from finding module"""
         self.results.append(res[0])
         for func in res[1]:
             proc = self.pool.apply_async(
                 func, callback=self.callback, error_callback=self.err_callback
             )
             self.processes.append(proc)
 
-    def packages_iter(self, packages: tuple, verbose: bool = False):
+    def packages_iter(self):
         """Iterate over all provided subpackages"""
-        for package in packages:
-            func = functools.partial(_parse_module, package=package, verbose=verbose)
+        for package in packages.get():
+            func = functools.partial(_parse_module, package=package)
             proc = self.pool.apply_async(
                 func, callback=self.callback, error_callback=self.err_callback
             )
             self.processes.append(proc)
 
         while len(self.processes) > 0:
             for job in list(self.processes):
                 if job.ready():
                     self.processes.remove(job)
                     res = self.results.pop()
                     if res:
                         yield res
 
-    def run(self, first_only, packages, verbose):
+    def run(self):
         """Find print statements and potential exceptions from selected packages"""
-        prints = []
-        exceptions = []
+        results = []
 
-        func = functools.partial(_parse_pyfile, first_only=first_only)
-        for module in self.packages_iter(packages, verbose):
-            found, exception = func(module)
-            if found:
-                prints = prints + found
-            elif exception:
-                exceptions.append(exception)
-            if any(printed for _, printed in found) and first_only:
+        for module in self.packages_iter():
+            res = _parse_pyfile(module)
+            results.append(res)
+            if res >= 1 and first_only.get():  # pragma: no cover
                 break
         self.pool.terminate()
         self.pool.join()
-        return (
-            prints,
-            exceptions,
-        )
+        return max(results)
 
 
-def detect_prints(
-    packages: tuple,
-    first_only: bool = False,
-    verbose: bool = False,
-    pool_threads: int = 1,
-) -> Tuple[list, list]:  # pragma: no cover
+def detect_prints() -> int:  # pragma: no cover
     """Detect print statements from packages found by _get_subpackages"""
+    # pylint: disable=unnecessary-lambda-assignment
+    get_var = lambda name, ctx: [var.get() for var in iter(ctx) if var.name == name][0]
+
+    ctx = contextvars.copy_context()
+
+    packages.set(get_var("packages", ctx))
+    mt_threads.set(get_var("mt_threads", ctx))
+    log_lvl.set(get_var("log_lvl", ctx))
+    first_only.set(get_var("first_only", ctx))
+    verbose.set(get_var("verbose", ctx))
+    very_verbose.set(get_var("very_verbose", ctx))
+
     logging.log(
         "Starting analysis, depending on package complexity, this may take a few seconds...",
         logging.INFO,
     )
-
-    pkg_finder = PackageFinder(pool_threads)
-    return pkg_finder.run(first_only, packages, verbose)
+    pkg_finder = PackageFinder()
+    return pkg_finder.run()
```

### Comparing `noprint-3.0.0/src/noprint.egg-info/PKG-INFO` & `noprint-3.1.0/src/noprint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noprint
-Version: 3.0.0
+Version: 3.1.0
 Summary: Do not allow prints in your code
 Author-email: Radoslaw Gryta <radek.gryta@gmail.com>
 Project-URL: Homepage, https://github.com/rgryta/NoPrint
 Project-URL: Bug Tracker, https://github.com/rgryta/NoPrint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: noprint Version: 3.0.0 Summary: Do not allow prints
+Metadata-Version: 2.1 Name: noprint Version: 3.1.0 Summary: Do not allow prints
 in your code Author-email: Radoslaw Gryta
 gryta@gmail.com> Project-URL: Homepage, https://github.com/rgryta/NoPrint
 Project-URL: Bug Tracker, https://github.com/rgryta/NoPrint/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
      [https://raw.githubusercontent.com/rgryta/NoPrint/main/docs/logo.png]
```

### Comparing `noprint-3.0.0/tests/test_logger.py` & `noprint-3.1.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `noprint-3.0.0/tests/test_module.py` & `noprint-3.1.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `noprint-3.0.0/tests/test_sprint.py` & `noprint-3.1.0/tests/test_sprint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module with tests for noprint.sprint
 """
+import contextvars
 from unittest import mock
 
 import pytest
 
 import noprint
 
 from noprint.sprint import (
@@ -32,15 +33,15 @@
     mod_mock_e.origin = ["origin"]
     mod_mock_e.name = "name"
     mod_mock_e.search_path = "loc"
     mod_mock_e.submodule_search_locations = ["loc"]
 
     mock_os.listdir.return_value = ["name"]
 
-    for package in _get_subpackages("noprint", verbose=True, module=mod_mock):
+    for package in _get_subpackages("noprint", module=mod_mock):
         assert package is not None
 
 
 @pytest.mark.parametrize("sub_pkgs", [[], [mock.Mock()], [mock.Mock(), mock.Mock()]])
 @pytest.mark.parametrize("origin", [None, "origin"])
 def test_parse_module(origin, sub_pkgs):
     """Testing function for _get_subpackages - mock several different module specs and finish with a proper one"""
@@ -53,27 +54,30 @@
         if module.origin:
             assert result[0] == module
         else:
             assert result[0] is None
         assert len(result[1]) == len(sub_pkgs)
 
 
-def _parse_mock(package, verbose):  # pylint:disable=unused-argument
+def _parse_mock(package):  # pylint:disable=unused-argument
     """Helper function for mocking _parse_module (Pool pickling)"""
     return (package, [])
 
 
 def test_pf_packages_iter():
     """Testing PackageFinder.packages_iter"""
-    pkg_finder = PackageFinder(1)
+    pkg_finder = PackageFinder()
 
     noprint.sprint._parse_module = _parse_mock  # pylint:disable=protected-access
 
     packages = ("source", "test")
-    assert set(pkg_finder.packages_iter(packages=packages)) == set(packages)
+    var = contextvars.ContextVar("packages")
+    var.set(packages)
+    noprint.sprint.packages = var
+    assert set(pkg_finder.packages_iter()) == set(packages)
 
 
 @pytest.mark.parametrize(
     "ret",
     [
         [mock.MagicMock(), mock.MagicMock()],
         [mock.MagicMock(), None],
@@ -83,15 +87,15 @@
 def test__get_module__mod(ret):
     """Testing function for _get_subpackages - mock several different module specs and finish with a proper one"""
 
     with mock.patch("noprint.sprint.Module") as mock_mod:
         if isinstance(ret[1], mock.MagicMock):
             ret[1].origin.__len__.return_value = 1
         mock_mod.side_effect = ret
-        _get_module("noprint", verbose=True)
+        _get_module("noprint")
 
 
 @pytest.mark.parametrize(
     "ret", [None, ParentModuleNotFoundException("Dummy exception")]
 )
 def test__get_module__import_exc(ret):
     """Testing function for _get_subpackages - mock several different module specs and finish with a proper one"""
@@ -99,45 +103,42 @@
     with mock.patch("noprint.sprint.Module") as mock_mod, pytest.raises(
         ImportException
     ):
         if ret is None:
             mock_mod.return_value = ret
         else:
             mock_mod.side_effect = ret
-        _get_module("noprint", verbose=True)
+        _get_module("noprint")
 
 
 @pytest.mark.parametrize("code", ["print('')", "", "i=1"])
-@pytest.mark.parametrize("first", [True, False])
 @pytest.mark.parametrize("mod", [None, ImportException("X")])
 @mock.patch("builtins.open")
-def test__parse_pyfile(mock_open, mod, first, code):
+def test__parse_pyfile(mock_open, mod, code):
     """Test method for _parse_python - finding print statements"""
     fin = mock.Mock()
     fin.return_value.readline.return_value = "# -*- coding: utf-8-sig -*-"
     fin.return_value.read.return_value = code
     mock_open.return_value.__enter__ = fin
 
     module = mock.Mock()
     module.origin = ["noprint"]
     module.name = "noprint"
 
     if mod is None:
         mod = module
 
-    res = _parse_pyfile(mod, first)
+    res = _parse_pyfile(mod)
 
     if isinstance(mod, ImportException):
-        assert not res[0]
-        assert isinstance(res[1], ImportException)
-        assert res[1].args[0] == mod.args[0]
+        assert res == 2
     elif "print" in code:
-        assert res == ([("[noprint] Line: 1", True)], None)
+        assert res == 1  # ([("[noprint] Line: 1", True)], None)
     else:
-        assert res == ([("[CLEAR]:[noprint]", False)], None)
+        assert res == 0  # ([("[CLEAR]:[noprint]", False)], None)
 
 
 @pytest.mark.parametrize("first", [True, False])
 @pytest.mark.parametrize(
     "mod",
     [
         (
@@ -150,28 +151,27 @@
         ),
         (
             [],
             ImportException("X"),
         ),
     ],
 )
-@mock.patch(
-    "noprint.sprint._parse_pyfile", side_effect=lambda module, first_only: module
-)
+@mock.patch("noprint.sprint._parse_pyfile", side_effect=lambda *args, **kwargs: 0)
 def test_pf_run(mock_parse, mod, first):  # pylint: disable=unused-argument
     """Testing function for _get_prints - verifying if code contains print statements"""
 
-    def _subpackages(package, _):  # pylint: disable=unused-argument
+    def _subpackages():  # pylint: disable=unused-argument
         i = 0
         yield mod
         i = i + 1
         if i == 10:
             return
 
     with mock.patch(
         "noprint.sprint.PackageFinder.packages_iter", side_effect=_subpackages
     ):
-        prints = PackageFinder(1).run(
-            packages=["noprint"], first_only=first, verbose=True
-        )
-        expected = (mod[0], [mod[1]] if mod[1] else [])
-        assert prints == expected
+        result = PackageFinder().run()
+        packages = ("source", "test")
+        var = contextvars.ContextVar("packages")
+        var.set(packages)
+        noprint.sprint.packages = var
+        assert result == 0
```

