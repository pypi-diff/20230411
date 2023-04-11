# Comparing `tmp/pyproject-parser-0.7.0b1.tar.gz` & `tmp/pyproject-parser-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-parser-0.7.0b1.tar", last modified: Sat Jun  4 14:16:34 2022, max compression
+gzip compressed data, was "pyproject-parser-0.8.0.tar", last modified: Tue Apr 11 12:28:04 2023, max compression
```

## Comparing `pyproject-parser-0.7.0b1.tar` & `pyproject-parser-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 14:16:34.200972 pyproject-parser-0.7.0b1/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8477 2022-06-04 14:16:34.200972 pyproject-parser-0.7.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5607 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5652 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 14:16:34.196972 pyproject-parser-0.7.0b1/pyproject_parser/
--rw-r--r--   0 runner    (1001) docker     (121)    10886 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/pyproject_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9345 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/pyproject_parser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10138 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/pyproject_parser/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 14:16:34.196972 pyproject-parser-0.7.0b1/pyproject_parser/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     6297 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/pyproject_parser/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/pyproject_parser/cli/_json_encoders.py
--rw-r--r--   0 runner    (1001) docker     (121)    35618 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/pyproject_parser/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/pyproject_parser/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3778 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/pyproject_parser/type_hints.py
--rw-r--r--   0 runner    (1001) docker     (121)     4257 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/pyproject_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 14:16:34.196972 pyproject-parser-0.7.0b1/pyproject_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8477 2022-06-04 14:16:33.000000 pyproject-parser-0.7.0b1/pyproject_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-06-04 14:16:34.000000 pyproject-parser-0.7.0b1/pyproject_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-04 14:16:33.000000 pyproject-parser-0.7.0b1/pyproject_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-06-04 14:16:33.000000 pyproject-parser-0.7.0b1/pyproject_parser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-04 14:16:33.000000 pyproject-parser-0.7.0b1/pyproject_parser.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-06-04 14:16:34.000000 pyproject-parser-0.7.0b1/pyproject_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-04 14:16:34.000000 pyproject-parser-0.7.0b1/pyproject_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-06-04 14:16:34.200972 pyproject-parser-0.7.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-06-04 14:15:50.000000 pyproject-parser-0.7.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:28:04.395501 pyproject-parser-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8391 2023-04-11 12:28:04.395501 pyproject-parser-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5472 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5704 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:28:04.391500 pyproject-parser-0.8.0/pyproject_parser/
+-rw-r--r--   0 runner    (1001) docker     (122)    10900 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9377 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:28:04.391500 pyproject-parser-0.8.0/pyproject_parser/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     6437 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/cli/_json_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35674 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     3778 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/type_hints.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5126 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:28:04.391500 pyproject-parser-0.8.0/pyproject_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8391 2023-04-11 12:28:04.000000 pyproject-parser-0.8.0/pyproject_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-11 12:28:04.000000 pyproject-parser-0.8.0/pyproject_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 12:28:04.000000 pyproject-parser-0.8.0/pyproject_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-04-11 12:28:04.000000 pyproject-parser-0.8.0/pyproject_parser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 12:28:04.000000 pyproject-parser-0.8.0/pyproject_parser.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      362 2023-04-11 12:28:04.000000 pyproject-parser-0.8.0/pyproject_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-11 12:28:04.000000 pyproject-parser-0.8.0/pyproject_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-04-11 12:28:04.395501 pyproject-parser-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      648 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:28:04.395501 pyproject-parser-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    10428 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15102 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/tests/test_cli_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12980 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5900 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/tests/test_dumping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/tests/test_pyproject_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1859 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/tests/test_utils.py
```

### Comparing `pyproject-parser-0.7.0b1/LICENSE` & `pyproject-parser-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.7.0b1/PKG-INFO` & `pyproject-parser-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-parser
-Version: 0.7.0b1
+Version: 0.8.0
 Summary: Parser for 'pyproject.toml'
 Home-page: https://github.com/repo-helper/pyproject-parser
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,14 +40,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
@@ -112,16 +113,16 @@
 	:target: https://github.com/repo-helper/pyproject-parser/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/pyproject-parser/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/pyproject-parser/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/repo-helper/pyproject-parser/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/repo-helper/pyproject-parser/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/pyproject-parser/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/pyproject-parser/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/pyproject-parser/master?logo=coveralls
 	:target: https://coveralls.io/github/repo-helper/pyproject-parser?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/pyproject-parser?logo=codefactor
@@ -155,23 +156,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pyproject-parser
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.7.0b1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.8.0
 	:target: https://github.com/repo-helper/pyproject-parser/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/pyproject-parser
 	:target: https://pypi.org/project/pyproject-parser/
 	:alt: PyPI - Downloads
 
 .. end shields
@@ -187,25 +188,17 @@
 
 .. code-block:: bash
 
 	$ python -m pip install pyproject-parser
 
 To install with ``conda``:
 
-	* First add the required channels
-
-	.. code-block:: bash
-
-		$ conda config --add channels https://conda.anaconda.org/conda-forge
-
-	* Then install
-
-	.. code-block:: bash
+.. code-block:: bash
 
-		$ conda install pyproject-parser
+	$ conda install -c conda-forge pyproject-parser
 
 .. end installation
 
 ``pyproject-parser`` also has an optional README validation feature, which checks the README will render correctly on PyPI.
 This requires that the ``readme`` extra is installed:
 
 .. code-block:: bash
```

### Comparing `pyproject-parser-0.7.0b1/README.rst` & `pyproject-parser-0.8.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 	:target: https://github.com/repo-helper/pyproject-parser/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/pyproject-parser/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/pyproject-parser/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/repo-helper/pyproject-parser/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/repo-helper/pyproject-parser/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/pyproject-parser/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/pyproject-parser/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/pyproject-parser/master?logo=coveralls
 	:target: https://coveralls.io/github/repo-helper/pyproject-parser?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/pyproject-parser?logo=codefactor
@@ -97,23 +97,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pyproject-parser
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.7.0b1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.8.0
 	:target: https://github.com/repo-helper/pyproject-parser/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/pyproject-parser
 	:target: https://pypi.org/project/pyproject-parser/
 	:alt: PyPI - Downloads
 
 .. end shields
@@ -129,25 +129,17 @@
 
 .. code-block:: bash
 
 	$ python -m pip install pyproject-parser
 
 To install with ``conda``:
 
-	* First add the required channels
-
-	.. code-block:: bash
-
-		$ conda config --add channels https://conda.anaconda.org/conda-forge
-
-	* Then install
-
-	.. code-block:: bash
+.. code-block:: bash
 
-		$ conda install pyproject-parser
+	$ conda install -c conda-forge pyproject-parser
 
 .. end installation
 
 ``pyproject-parser`` also has an optional README validation feature, which checks the README will render correctly on PyPI.
 This requires that the ``readme`` extra is installed:
 
 .. code-block:: bash
```

### Comparing `pyproject-parser-0.7.0b1/pyproject.toml` & `pyproject-parser-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools!=61.*,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyproject-parser"
-version = "0.7.0b1"
+version = "0.8.0"
 description = "Parser for 'pyproject.toml'"
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "metadata", "packaging", "pep518", "pep621", "pyproject", "toml",]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -17,14 +17,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Archiving :: Packaging",
     "Typing :: Typed",
 ]
 dynamic = [ "dependencies",]
@@ -158,15 +159,15 @@
 base-classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Archiving :: Packaging",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 package = "pyproject_parser"
 
 [tool.mypy]
 python_version = "3.6"
```

### Comparing `pyproject-parser-0.7.0b1/pyproject_parser/__init__.py` & `pyproject-parser-0.8.0/pyproject_parser/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 		ProjectDict,
 		_PyProjectAsTomlDict
 		)
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.7.0b1"
+__version__: str = "0.8.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["PyProject", "PyProjectTomlEncoder", "_PP"]
 
 _PP = TypeVar("_PP", bound="PyProject")
 
 
@@ -71,15 +71,15 @@
 	Custom TOML encoder supporting types in :mod:`pyproject_parser.classes` and packaging_.
 
 	.. _packaging: https://packaging.pypa.io/en/latest/
 
 	.. autosummary-widths:: 23/64
 	"""
 
-	def __init__(self, _dict=dict, preserve: bool = False) -> None:
+	def __init__(self, _dict=dict, preserve: bool = False) -> None:  # noqa: MAN001
 		super().__init__(_dict=_dict, preserve=preserve)
 		self.dump_funcs[str] = _dump_str
 		self.dump_funcs[_NormalisedName] = _dump_str
 		self.dump_funcs[Version] = self.dump_packaging_types
 		self.dump_funcs[Requirement] = self.dump_packaging_types
 		self.dump_funcs[Marker] = self.dump_packaging_types
 		self.dump_funcs[SpecifierSet] = self.dump_packaging_types
```

### Comparing `pyproject-parser-0.7.0b1/pyproject_parser/__main__.py` & `pyproject-parser-0.8.0/pyproject_parser/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 	from consolekit.terminal_colours import ColourTrilean
 	from domdf_python_tools.typing import PathLike
 
 __all__ = ["main", "reformat", "check"]
 
 
 @click_group()
-def main():  # pragma: no cover  # noqa: D103
+def main() -> None:  # pragma: no cover  # noqa: D103
 	pass
 
 
 _C = TypeVar("_C", bound=click.Command)
 
 
 def options(c: _C) -> _C:
@@ -89,15 +89,15 @@
 
 @options
 @main.command(cls=MarkdownHelpCommand)
 def check(
 		pyproject_file: "PathLike" = "pyproject.toml",
 		parser_class: str = "pyproject_parser:PyProject",
 		show_traceback: bool = False,
-		):
+		) -> None:
 	"""
 	Validate the given ``pyproject.toml`` file.
 	"""
 
 	# 3rd party
 	import dom_toml
 	from dom_toml.parser import BadConfigError
@@ -184,15 +184,15 @@
 def info(
 		field: Optional[str] = None,
 		pyproject_file: "PathLike" = "pyproject.toml",
 		parser_class: str = "pyproject_parser:PyProject",
 		resolve: bool = False,
 		show_traceback: bool = False,
 		indent: Optional[int] = None,
-		):
+		) -> None:
 	"""
 	Extract information from the given ``pyproject.toml`` file and print the JSON representation.
 	"""
 
 	# stdlib
 	import os
 	import re
@@ -281,15 +281,15 @@
 def reformat(
 		pyproject_file: "PathLike" = "pyproject.toml",
 		encoder_class: str = "pyproject_parser:PyProjectTomlEncoder",
 		parser_class: str = "pyproject_parser:PyProject",
 		show_traceback: bool = False,
 		show_diff: bool = False,
 		colour: "ColourTrilean" = None,
-		):
+		) -> None:
 	"""
 	Reformat the given ``pyproject.toml`` file.
 	"""
 
 	# 3rd party
 	from consolekit.terminal_colours import resolve_color_default  # nodep
 	from consolekit.utils import coloured_diff  # nodep
```

### Comparing `pyproject-parser-0.7.0b1/pyproject_parser/classes.py` & `pyproject-parser-0.8.0/pyproject_parser/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,15 +340,15 @@
 	and allows the original name to be stored as an attribute.
 	"""  # noqa: D400
 
 	__slots__ = ("_unnormalized", )
 
 	_unnormalized: Optional[str]
 
-	def __new__(cls, o, **kwargs):
+	def __new__(cls, o, **kwargs):  # noqa: MAN001
 		self = super().__new__(cls, o, **kwargs)
 		self._unnormalized = None
 		return self
 
 	@property
 	def unnormalized(self) -> str:
 		if self._unnormalized is None:
```

### Comparing `pyproject-parser-0.7.0b1/pyproject_parser/cli/__init__.py` & `pyproject-parser-0.8.0/pyproject_parser/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 # stdlib
 import functools
 import importlib
 import re
 import sys
 import warnings
 from pathlib import Path
-from typing import TYPE_CHECKING, Pattern, Type
+from typing import TYPE_CHECKING, Optional, Pattern, TextIO, Type, Union
 
 # 3rd party
 import click  # nodep
 from consolekit.tracebacks import TracebackHandler  # nodep
 from consolekit.utils import abort  # nodep
 from dom_toml.parser import BadConfigError
 from packaging.specifiers import InvalidSpecifier
@@ -184,15 +184,22 @@
 
 	orig_showwarning = warnings.showwarning
 
 	if orig_showwarning is prettify_deprecation_warning:
 		return
 
 	@functools.wraps(warnings.showwarning)
-	def showwarning(message, category, filename, lineno, file=None, line=None):
+	def showwarning(
+			message: Union[Warning, str],
+			category: Type[Warning],
+			filename: str,
+			lineno: int,
+			file: Optional[TextIO] = None,
+			line: Optional[str] = None,
+			) -> None:
 		if isinstance(message, PyProjectDeprecationWarning):
 			if file is None:
 				file = sys.stderr
 
 			s = f"WARNING: {message.args[0]}\n"
 			file.write(s)
```

### Comparing `pyproject-parser-0.7.0b1/pyproject_parser/cli/_json_encoders.py` & `pyproject-parser-0.8.0/pyproject_parser/cli/_json_encoders.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.7.0b1/pyproject_parser/parsers.py` & `pyproject-parser-0.8.0/pyproject_parser/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,20 +58,20 @@
 		"PEP621Parser",
 		]
 
 name_re = re.compile("^([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])$", flags=re.IGNORECASE)
 extra_re = re.compile("^([a-z0-9]|[a-z0-9]([a-z0-9-](?!--))*[a-z0-9])$")
 
 
-def _documentation_url(__documentation_url: str):
+def _documentation_url(__documentation_url: str) -> Callable:
 
-	def deco(f):
+	def deco(f) -> Callable:  # noqa: MAN001
 
 		@functools.wraps(f)
-		def wrapper(*args, **kwds):
+		def wrapper(*args, **kwds):  # noqa: MAN002
 			try:
 				return f(*args, **kwds)
 			except Exception as e:
 				if getattr(e, "documentation", None) is None:
 					e.documentation = __documentation_url  # type: ignore[attr-defined]
 				raise
```

### Comparing `pyproject-parser-0.7.0b1/pyproject_parser/type_hints.py` & `pyproject-parser-0.8.0/pyproject_parser/type_hints.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.7.0b1/pyproject_parser/utils.py` & `pyproject-parser-0.8.0/pyproject_parser/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 #
 #  utils.py
 """
 Utility functions.
 """
 #
-#  Copyright © 2021 Dominic Davis-Foster <dominic@davis-foster.co.uk>
+#  Copyright © 2021-2023 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
 #  furnished to do so, subject to the following conditions:
@@ -24,14 +24,15 @@
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
 import functools
+import io
 import os
 import sys
 from typing import TYPE_CHECKING, Optional
 
 # 3rd party
 from dom_toml.parser import BadConfigError
 from domdf_python_tools.paths import PathPlus
@@ -64,34 +65,57 @@
 
 	rendering_result = readme_renderer.markdown.render(content, stream=sys.stderr)
 
 	if rendering_result is None:  # pragma: no cover
 		raise BadConfigError("Error rendering README.")
 
 
-def render_rst(content: str) -> None:
+def render_rst(content: str, filename: PathLike = "<string>") -> None:
 	"""
 	Attempt to render the given content as :wikipedia:`ReStructuredText`.
 
 	.. extras-require:: readme
 		:pyproject:
 		:scope: function
 
 	:param content:
+	:param filename: The original filename.
+
+	.. versionchanged:: 0.8.0  Added the ``filename`` argument.
 	"""
 
 	try:
 		# 3rd party
+		import docutils.core
 		import readme_renderer.rst  # type: ignore[import]
+		from docutils.utils import SystemMessage
+		from docutils.writers.html4css1 import Writer
+
 	except ImportError:  # pragma: no cover
 		return
 
-	rendering_result = readme_renderer.rst.render(content, stream=sys.stderr)
+	# Adapted from https://github.com/pypa/readme_renderer/blob/main/readme_renderer/rst.py#L106
+	settings = readme_renderer.rst.SETTINGS.copy()
+	settings["warning_stream"] = io.StringIO()
 
-	if rendering_result is None:
+	writer = Writer()
+	writer.translator_class = readme_renderer.rst.ReadMeHTMLTranslator
+
+	try:
+		parts = docutils.core.publish_parts(content, str(filename), writer=writer, settings_overrides=settings)
+		if parts.get("docinfo", '') + parts.get("fragment", ''):
+			# Success!
+			return
+	except SystemMessage:
+		pass
+
+	if not settings["warning_stream"].tell():
+		raise BadConfigError("Error rendering README: No content rendered from RST source.")
+	else:
+		sys.stderr.write(settings["warning_stream"].getvalue())
 		raise BadConfigError("Error rendering README.")
 
 
 @functools.lru_cache()
 def content_type_from_filename(filename: PathLike) -> "ContentTypes":
 	"""
 	Return the inferred content type for the given (readme) filename.
@@ -132,15 +156,15 @@
 
 	content = readme_file.read_text(encoding=encoding)
 
 	if int(os.environ.get("CHECK_README", 1)):
 		if content_type == "text/markdown":
 			render_markdown(content)
 		elif content_type == "text/x-rst":
-			render_rst(content)
+			render_rst(content, readme_file)
 
 
 class PyProjectDeprecationWarning(Warning):
 	"""
 	Warning for the use of deprecated features in `pyproject.toml`.
 
 	This is a user-facing warning which will be shown by default.
```

### Comparing `pyproject-parser-0.7.0b1/pyproject_parser.egg-info/PKG-INFO` & `pyproject-parser-0.8.0/pyproject_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-parser
-Version: 0.7.0b1
+Version: 0.8.0
 Summary: Parser for 'pyproject.toml'
 Home-page: https://github.com/repo-helper/pyproject-parser
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,14 +40,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
@@ -112,16 +113,16 @@
 	:target: https://github.com/repo-helper/pyproject-parser/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/pyproject-parser/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/pyproject-parser/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/repo-helper/pyproject-parser/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/repo-helper/pyproject-parser/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/pyproject-parser/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/pyproject-parser/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/pyproject-parser/master?logo=coveralls
 	:target: https://coveralls.io/github/repo-helper/pyproject-parser?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/pyproject-parser?logo=codefactor
@@ -155,23 +156,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pyproject-parser
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.7.0b1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.8.0
 	:target: https://github.com/repo-helper/pyproject-parser/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/pyproject-parser
 	:target: https://pypi.org/project/pyproject-parser/
 	:alt: PyPI - Downloads
 
 .. end shields
@@ -187,25 +188,17 @@
 
 .. code-block:: bash
 
 	$ python -m pip install pyproject-parser
 
 To install with ``conda``:
 
-	* First add the required channels
-
-	.. code-block:: bash
-
-		$ conda config --add channels https://conda.anaconda.org/conda-forge
-
-	* Then install
-
-	.. code-block:: bash
+.. code-block:: bash
 
-		$ conda install pyproject-parser
+	$ conda install -c conda-forge pyproject-parser
 
 .. end installation
 
 ``pyproject-parser`` also has an optional README validation feature, which checks the README will render correctly on PyPI.
 This requires that the ``readme`` extra is installed:
 
 .. code-block:: bash
```

### Comparing `pyproject-parser-0.7.0b1/pyproject_parser.egg-info/SOURCES.txt` & `pyproject-parser-0.8.0/pyproject_parser.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -17,8 +17,15 @@
 pyproject_parser.egg-info/SOURCES.txt
 pyproject_parser.egg-info/dependency_links.txt
 pyproject_parser.egg-info/entry_points.txt
 pyproject_parser.egg-info/not-zip-safe
 pyproject_parser.egg-info/requires.txt
 pyproject_parser.egg-info/top_level.txt
 pyproject_parser/cli/__init__.py
-pyproject_parser/cli/_json_encoders.py
+pyproject_parser/cli/_json_encoders.py
+tests/test_classes.py
+tests/test_cli.py
+tests/test_cli_module.py
+tests/test_config.py
+tests/test_dumping.py
+tests/test_pyproject_class.py
+tests/test_utils.py
```

### Comparing `pyproject-parser-0.7.0b1/setup.cfg` & `pyproject-parser-0.8.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyproject-parser
-version = 0.7.0b1
+version = 0.8.0
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = MIT License
 keywords = pep518, pep621, pyproject, toml, metadata, packaging
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
@@ -21,14 +21,15 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: System :: Archiving :: Packaging
 	Typing :: Typed
 
 [options]
```

### Comparing `pyproject-parser-0.7.0b1/setup.py` & `pyproject-parser-0.8.0/setup.py`

 * *Files identical despite different names*

