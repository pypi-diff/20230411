# Comparing `tmp/pjy-0.12.0.tar.gz` & `tmp/pjy-0.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pjy-0.12.0.tar", last modified: Sun May  9 08:28:31 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pjy-0.12.0.tar` & `pjy-0.13.0.tar`

### file list

```diff
@@ -1,13 +1,6 @@
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2021-05-09 08:28:31.394602 pjy-0.12.0/
--rw-r--r--   0 ntome     (1000) ntome     (1000)    10272 2021-05-09 08:28:31.394602 pjy-0.12.0/PKG-INFO
--rw-r--r--   0 ntome     (1000) ntome     (1000)     6661 2021-05-09 08:23:51.000000 pjy-0.12.0/README.rst
--rwxr-xr-x   0 ntome     (1000) ntome     (1000)    11727 2021-05-09 08:27:34.000000 pjy-0.12.0/pjy
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2021-05-09 08:28:31.390602 pjy-0.12.0/pjy.egg-info/
--rw-r--r--   0 ntome     (1000) ntome     (1000)    10272 2021-05-09 08:28:30.000000 pjy-0.12.0/pjy.egg-info/PKG-INFO
--rw-r--r--   0 ntome     (1000) ntome     (1000)      189 2021-05-09 08:28:30.000000 pjy-0.12.0/pjy.egg-info/SOURCES.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)        1 2021-05-09 08:28:30.000000 pjy-0.12.0/pjy.egg-info/dependency_links.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)       21 2021-05-09 08:28:30.000000 pjy-0.12.0/pjy.egg-info/requires.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)        1 2021-05-09 08:28:30.000000 pjy-0.12.0/pjy.egg-info/top_level.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)        1 2020-09-20 16:27:16.000000 pjy-0.12.0/pjy.egg-info/zip-safe
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1120 2021-05-09 08:28:31.398602 pjy-0.12.0/setup.cfg
--rwxr-xr-x   0 ntome     (1000) ntome     (1000)      193 2021-05-09 08:23:51.000000 pjy-0.12.0/setup.py
+-rwxr-xr-x   0        0        0    11781 2020-02-02 00:00:00.000000 pjy-0.13.0/pjy.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pjy-0.13.0/.gitignore
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pjy-0.13.0/COPYING.WTFPL
+-rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 pjy-0.13.0/README.rst
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pjy-0.13.0/pyproject.toml
+-rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 pjy-0.13.0/PKG-INFO
```

### Comparing `pjy-0.12.0/PKG-INFO` & `pjy-0.13.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,348 +1,352 @@
 Metadata-Version: 2.1
 Name: pjy
-Version: 0.12.0
+Version: 0.13.0
 Summary: pjy - command-line JSON processor
-Home-page: https://gitlab.com/hydrargyrum/pjy
-Author: Hg
-Author-email: dev@indigo.re
-License: WTFPLv2
-Description: pjy - JSON Python processor
-        ===========================
-        
-        ``pjy`` is a command-line tool to process JSON data and execute queries on it.
-        It is a bit like `jq <https://stedolan.github.io/jq/>`_ but with a Python syntax for queries.
-        
-        Install
-        +++++++
-        
-        From `PyPI <https://pypi.org/project/pjy/>`_::
-        
-            pip install pjy
-        
-        Usage
-        +++++
-        
-            pjy [EXPR] [FILES]
-        
-        ``pjy`` will read JSON data from ``FILES`` and print the evaluation result of the Python expression ``EXPR``.
-        
-        If ``FILES`` is missing or is "``-``", pjy will use stdin.
-        
-        The simplest expression to use, which outputs the input unchanged is "``d``" (for data).
-        
-        It's possible to use multiple input files.
-        
-        Examples
-        ++++++++
-        
-        In ``pjy``, expressions are also called "filters", as in ``jq``.
-        
-        Just pretty-print
-        -----------------
-        
-        ``d`` (short for "data") is the most basic filter, it represents the whole input::
-        
-            pjy 'd'
-                {"foo":"bar","baz":[1,2,3]}
-        
-        Prints::
-        
-            {
-              "foo": "bar",
-              "baz": [
-                1,
-                2,
-                3
-              ]
-            }
-        
-        Select a dict key
-        -----------------
-        
-        The filters are Python expressions, hence we can select a dict key::
-        
-            pjy 'd["baz"]'
-                {"foo":"bar","baz":[1,2,3]}
-        
-        Alternatively, in ``pjy``, dicts keys are also attributes::
-        
-            pjy 'd.baz'
-                {"foo":"bar","baz":[1,2,3]}
-        
-        Both filters will print::
-        
-            [
-              1,
-              2,
-              3
-            ]
-        
-        In case a key has a reserved name, like ``import`` (keyword) or ``keys`` (dict method), simply use the bracket form.
-        
-        Non-existent keys
-        -----------------
-        
-        Non-existent keys::
-        
-            pjy 'd.baz'
-                {"foo":"bar"}
-        
-        will return ``None``::
-        
-            null
-        
-        Same for out-of-bounds indices::
-        
-            pjy 'd[3]'
-                [1, 2]
-        
-        Do a basic operation
-        --------------------
-        
-        It's possible to use everything that a Python expression can contain::
-        
-            pjy '[i + 1 for i in d["baz"]]'
-                {"foo":"bar","baz":[1,2,3]}
-        
-        Prints::
-        
-            [
-              2,
-              3,
-              4
-            ]
-        
-        Lambda-placeholder
-        ------------------
-        
-        A special identifier, ``_`` can be used to create lambdas. This identifier will absorb most operations done to it and return a lambda applying them.
-        Then, the returned lambda can be applied::
-        
-            pjy 'map(_ + 1, d.baz)'
-                {"foo":"bar","baz":[1,2,3]}
-        
-        Is equivalent to::
-        
-            pjy 'map((lambda x: x + 1), d.baz)'
-                {"foo":"bar","baz":[1,2,3]}
-        
-        Which will print::
-        
-            [
-              2,
-              3,
-              4
-            ]
-        
-        The lambda-placeholder will absorb chained operations::
-        
-            pjy 'map((_ + 1) * 2, d.baz)'
-                {"foo":"bar","baz":[1,2,3]}
-        
-        
-        Will result in::
-        
-            [
-              4,
-              6,
-              8
-            ]
-        
-        And::
-        
-            pjy 'map(_[1:3] * 2, d)'
-                {"foo":"bar","baz":[1,2,3]}
-        
-        Will return::
-        
-            {
-              "foo": "arar",
-              "baz": [
-                2,
-                3,
-                2,
-                3
-              ]
-            }
-        
-        Pipe-like iteration
-        -------------------
-        
-        The pipe (``|``) can be used to iterate on a list, it accepts a function as right operand::
-        
-            pjy 'd.baz | _ + 1'
-                {"foo":"bar","baz":[1,2,3]}
-        
-        Which prints::
-        
-            [
-              2,
-              3,
-              4
-            ]
-        
-        It also operates on a dict's values, and returns a dict::
-        
-            pjy 'd | (lambda x: repr(x))'
-                {"foo":"bar","baz":[1,2,3]}
-        
-        The values are replaced by the right operand value, the keys are unchanged::
-        
-            {
-              "foo": "'bar'",
-              "baz": "[1, 2, 3]"
-            }
-        
-        Ampersand for filtering
-        -----------------------
-        
-        Similar to the pipe, the ampersand (``&``) is used on a list and a function, but its purpose is to filter::
-        
-            pjy 'd & (_ % 2 == 0)'
-                [0, 1, 2, 3]
-        
-        outputs::
-        
-            [
-              0,
-              2
-            ]
-        
-        Which is equivalent to running::
-        
-            pjy 'filter(_ % 2 == 0, d)'
-                [0, 1, 2, 3]
-        
-        Like the pipe, it works on a dict, and the filter is applied on the dict values.
-        
-        Partial placeholder
-        -------------------
-        
-        It's not possible to call a function on a placeholder, for example, ``len(_)`` will not work.
-        However, it's possible to use the ``partial`` helper to prepare the function call::
-        
-            pjy 'd | partial(len, _)'
-                {"foo":"bar","baz":[1,2,3]}
-        
-        Prints::
-        
-            {
-              "foo": 3,
-              "baz": 3
-            }
-        
-        ``partial`` ressembles the ``functools.partial`` function: it returns a function wrapping the function passed as first argument.
-        The returned function will call the original function with the fixed arguments passed.
-        The difference is that lambda-placeholders can be passed, and they will be replaced by the wrapper's argument.
-        
-        ``p`` is a short alias for the ``partial`` function which can be used in pjy expressions.
-        
-        Imports
-        -------
-        
-        It's possible to import modules with the ``imp`` function::
-        
-           pjy 'filter(p(imp("fnmatch").fnmatch, _, "f*"), d.keys())'
-                {"foo":"bar","baz":[1,2,3]}
-        
-        Will print::
-        
-            [
-              "foo"
-            ]
-        
-        The ``math`` and ``re`` modules are already imported and available directly without having to call ``imp``.
-        
-        Multiple inputs
-        ---------------
-        
-        In ``pjy``, an ``inputs`` variable exists, which is a list containing the JSON data of each input file passed on the command line.
-        The ``d`` variable is simply an alias to ``inputs[0]``.
-        
-        For example::
-        
-            pjy 'filter(_[0] != _[1], zip(inputs[0], inputs[1]))' before.json after.json
-        
-        will read 2 files ``before.json`` and ``after.json``, which consist in a list of objects, and ``pjy`` will compare each zipped-pair of objects together.
-        Then it will print the list of differing pairs.
-        
-        Options
-        +++++++
-        
-        Input options
-        -------------
-        
-        	``--null-input``
-        
-        Don't read any input, act as if the input was only ``null``.
-        
-        	``--arg VAR VALUE``
-        
-        Inject a variable named VAR with a VALUE in the expression.
-        
-        Output options
-        --------------
-        
-        	``--monochrome-output``
-        
-        Force no colors even if output is a TTY.
-        
-        	``--ascii-output``
-        
-        When outputting non-ASCII strings, use ``\uXXXX`` notation instead of directly Unicode characters by default.
-        
-        	``--tab``
-        
-        Indent output with tabs instead of 2 spaces.
-        
-        	``--indent N``
-        
-        Indent output with N spaces instead of 2 spaces.
-        
-        	``--compact-output``
-        
-        Don't indent output and don't add extra whitespace between key/values and list elements.
-        
-        
-        Security
-        ++++++++
-        
-        ``pjy`` by itself does not write files (except stdout/stderr) or sockets, or run external commands.
-        However, ``pjy`` runs the given expressions passed as argument, in the Python interpreter, without a sandbox.
-        Hence, do NOT pass dangerous or untrusted Python expressions to ``pjy``.
-        
-        Dependencies
-        ++++++++++++
-        
-        ``pjy`` is written in Python 3. Its ``setup.py`` requires ``setuptools``.
-        
-        If ``pygments`` is installed, ``pjy``'s output will be colorized, but it's entirely optional.
-        
-        Version and license
-        +++++++++++++++++++
-        
-        .. $version
-        
-        ``pjy`` is at version 0.12.0, it uses `semantic versioning <http://semver.org/>`_.
-        It is licensed under the WTFPLv2, see COPYING.WTFPL for license text.
-        
-Keywords: json,processor,query,filter,jq
-Platform: UNKNOWN
+Project-URL: Project, https://gitlab.com/hydrargyrum/pjy
+Author-email: Hg <dev@indigo.re>
+License-Expression: WTFPL
+License-File: COPYING.WTFPL
+Keywords: filter,jq,json,processor,query
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: Public Domain
-Classifier: Topic :: Utilities
-Classifier: Topic :: Text Processing :: Filters
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Text Processing :: Filters
+Classifier: Topic :: Utilities
 Requires-Python: >=3
 Provides-Extra: pygments
+Requires-Dist: pygments; extra == 'pygments'
+Description-Content-Type: text/x-rst
+
+pjy - JSON Python processor
+===========================
+
+``pjy`` is a command-line tool to process JSON data and execute queries on it.
+It is a bit like `jq <https://stedolan.github.io/jq/>`_ but with a Python syntax for queries.
+
+Install
++++++++
+
+From `PyPI <https://pypi.org/project/pjy/>`_::
+
+    pip install pjy
+
+Usage
++++++
+
+    pjy [EXPR] [FILES]
+
+``pjy`` will read JSON data from ``FILES`` and print the evaluation result of the Python expression ``EXPR``.
+
+If ``FILES`` is missing or is "``-``", pjy will use stdin.
+
+The simplest expression to use, which outputs the input unchanged is "``d``" (for data).
+
+It's possible to use multiple input files.
+
+Examples
+++++++++
+
+In ``pjy``, expressions are also called "filters", as in ``jq``.
+
+Just pretty-print
+-----------------
+
+``d`` (short for "data") is the most basic filter, it represents the whole input::
+
+    pjy 'd'
+        {"foo":"bar","baz":[1,2,3]}
+
+Prints::
+
+    {
+      "foo": "bar",
+      "baz": [
+        1,
+        2,
+        3
+      ]
+    }
+
+Select a dict key
+-----------------
+
+The filters are Python expressions, hence we can select a dict key::
+
+    pjy 'd["baz"]'
+        {"foo":"bar","baz":[1,2,3]}
+
+Alternatively, in ``pjy``, dicts keys are also attributes::
+
+    pjy 'd.baz'
+        {"foo":"bar","baz":[1,2,3]}
+
+Both filters will print::
+
+    [
+      1,
+      2,
+      3
+    ]
+
+In case a key has a reserved name, like ``import`` (keyword) or ``keys`` (dict method), simply use the bracket form.
+
+Non-existent keys
+-----------------
+
+Non-existent keys::
+
+    pjy 'd.baz'
+        {"foo":"bar"}
+
+will return ``None``::
+
+    null
+
+Same for out-of-bounds indices::
+
+    pjy 'd[3]'
+        [1, 2]
+
+Do a basic operation
+--------------------
+
+It's possible to use everything that a Python expression can contain::
+
+    pjy '[i + 1 for i in d["baz"]]'
+        {"foo":"bar","baz":[1,2,3]}
+
+Prints::
+
+    [
+      2,
+      3,
+      4
+    ]
+
+Lambda-placeholder
+------------------
+
+A special identifier, ``_`` can be used to create lambdas. This identifier will absorb most operations done to it and return a lambda applying them.
+Then, the returned lambda can be applied::
+
+    pjy 'map(_ + 1, d.baz)'
+        {"foo":"bar","baz":[1,2,3]}
+
+Is equivalent to::
+
+    pjy 'map((lambda x: x + 1), d.baz)'
+        {"foo":"bar","baz":[1,2,3]}
+
+Which will print::
+
+    [
+      2,
+      3,
+      4
+    ]
+
+The lambda-placeholder will absorb chained operations::
+
+    pjy 'map((_ + 1) * 2, d.baz)'
+        {"foo":"bar","baz":[1,2,3]}
+
+
+Will result in::
+
+    [
+      4,
+      6,
+      8
+    ]
+
+And::
+
+    pjy 'map(_[1:3] * 2, d)'
+        {"foo":"bar","baz":[1,2,3]}
+
+Will return::
+
+    {
+      "foo": "arar",
+      "baz": [
+        2,
+        3,
+        2,
+        3
+      ]
+    }
+
+Pipe-like iteration
+-------------------
+
+The pipe (``|``) can be used to iterate on a list, it accepts a function as right operand::
+
+    pjy 'd.baz | _ + 1'
+        {"foo":"bar","baz":[1,2,3]}
+
+Which prints::
+
+    [
+      2,
+      3,
+      4
+    ]
+
+It also operates on a dict's values, and returns a dict::
+
+    pjy 'd | (lambda x: repr(x))'
+        {"foo":"bar","baz":[1,2,3]}
+
+The values are replaced by the right operand value, the keys are unchanged::
+
+    {
+      "foo": "'bar'",
+      "baz": "[1, 2, 3]"
+    }
+
+Ampersand for filtering
+-----------------------
+
+Similar to the pipe, the ampersand (``&``) is used on a list and a function, but its purpose is to filter::
+
+    pjy 'd & (_ % 2 == 0)'
+        [0, 1, 2, 3]
+
+outputs::
+
+    [
+      0,
+      2
+    ]
+
+Which is equivalent to running::
+
+    pjy 'filter(_ % 2 == 0, d)'
+        [0, 1, 2, 3]
+
+Like the pipe, it works on a dict, and the filter is applied on the dict values.
+
+Partial placeholder
+-------------------
+
+It's not possible to call a function on a placeholder, for example, ``len(_)`` will not work.
+However, it's possible to use the ``partial`` helper to prepare the function call::
+
+    pjy 'd | partial(len, _)'
+        {"foo":"bar","baz":[1,2,3]}
+
+Prints::
+
+    {
+      "foo": 3,
+      "baz": 3
+    }
+
+``partial`` ressembles the ``functools.partial`` function: it returns a function wrapping the function passed as first argument.
+The returned function will call the original function with the fixed arguments passed.
+The difference is that lambda-placeholders can be passed, and they will be replaced by the wrapper's argument.
+
+``p`` is a short alias for the ``partial`` function which can be used in pjy expressions.
+
+Imports
+-------
+
+It's possible to import modules with the ``imp`` function::
+
+   pjy 'filter(p(imp("fnmatch").fnmatch, _, "f*"), d.keys())'
+        {"foo":"bar","baz":[1,2,3]}
+
+Will print::
+
+    [
+      "foo"
+    ]
+
+The ``math`` and ``re`` modules are already imported and available directly without having to call ``imp``.
+
+Multiple inputs
+---------------
+
+In ``pjy``, an ``inputs`` variable exists, which is a list containing the JSON data of each input file passed on the command line.
+The ``d`` variable is simply an alias to ``inputs[0]``.
+
+For example::
+
+    pjy 'filter(_[0] != _[1], zip(inputs[0], inputs[1]))' before.json after.json
+
+will read 2 files ``before.json`` and ``after.json``, which consist in a list of objects, and ``pjy`` will compare each zipped-pair of objects together.
+Then it will print the list of differing pairs.
+
+Options
++++++++
+
+Input options
+-------------
+
+	``--null-input``
+
+Don't read any input, act as if the input was only ``null``.
+
+	``--arg VAR VALUE``
+
+Inject a variable named VAR with a VALUE in the expression.
+
+Output options
+--------------
+
+	``--monochrome-output``
+
+Force no colors even if output is a TTY.
+
+	``--ascii-output``
+
+When outputting non-ASCII strings, use ``\uXXXX`` notation instead of directly Unicode characters by default.
+
+	``--tab``
+
+Indent output with tabs instead of 2 spaces.
+
+	``--indent N``
+
+Indent output with N spaces instead of 2 spaces.
+
+	``--compact-output``
+
+Don't indent output and don't add extra whitespace between key/values and list elements.
+
+
+Security
+++++++++
+
+``pjy`` by itself does not write files (except stdout/stderr) or sockets, or run external commands.
+However, ``pjy`` runs the given expressions passed as argument, in the Python interpreter, without a sandbox.
+Hence, do NOT pass dangerous or untrusted Python expressions to ``pjy``.
+
+Dependencies
+++++++++++++
+
+``pjy`` is written in Python 3. Its ``setup.py`` requires ``setuptools``.
+
+If ``pygments`` is installed, ``pjy``'s output will be colorized, but it's entirely optional.
+
+Version and license
++++++++++++++++++++
+
+.. $version
+
+``pjy`` is at version 0.13.0, it uses `semantic versioning <http://semver.org/>`_.
+It is licensed under the WTFPLv2, see COPYING.WTFPL for license text.
```

### Comparing `pjy-0.12.0/README.rst` & `pjy-0.13.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -311,9 +311,9 @@
 If ``pygments`` is installed, ``pjy``'s output will be colorized, but it's entirely optional.
 
 Version and license
 +++++++++++++++++++
 
 .. $version
 
-``pjy`` is at version 0.12.0, it uses `semantic versioning <http://semver.org/>`_.
+``pjy`` is at version 0.13.0, it uses `semantic versioning <http://semver.org/>`_.
 It is licensed under the WTFPLv2, see COPYING.WTFPL for license text.
```

### Comparing `pjy-0.12.0/pjy` & `pjy-0.13.0/pjy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# This file is licensed under the WTFPLv2 [http://wtfpl.net]
+# SPDX-License-Identifier: WTFPL
 
 from argparse import ArgumentParser, FileType
 import ast
 from collections import OrderedDict
 from importlib import import_module
 import json
 import json.decoder
@@ -25,14 +25,17 @@
         formatter = pygments.formatters.TerminalFormatter()
         return pygments.highlight(s, lexer, formatter).rstrip()
 except ImportError:
     def colorize(s):
         return s
 
 
+__version__ = '0.13.0'  # $version
+
+
 def ph_call(obj, x):
     if isinstance(obj, Placeholder):
         return obj(x)
     return obj
 
 
 class Placeholder(object):
@@ -220,27 +223,35 @@
     return repr(obj)
 
 
 class Injector(ast.NodeTransformer):
     # convert list and dict literals to our Array and Dict
 
     def visit_List(self, node):
+        self.generic_visit(node)
+
         n = ast.Name(id='list', ctx=ast.Load())
         return ast.Call(func=n, args=[node], keywords=[])
 
     def visit_Dict(self, node):
+        self.generic_visit(node)
+
         n = ast.Name(id='dict', ctx=ast.Load())
         return ast.Call(func=n, args=[node], keywords=[])
 
     def visit_ListComp(self, node):
+        self.generic_visit(node)
+
         genex = ast.GeneratorExp(elt=node.elt, generators=node.generators)
         n = ast.Name(id='list', ctx=ast.Load())
         return ast.Call(func=n, args=[genex], keywords=[])
 
     def visit_DictComp(self, node):
+        self.generic_visit(node)
+
         n = ast.Name(id='dict', ctx=ast.Load())
         return ast.Call(func=n, args=[node], keywords=[])
 
 
 def parse_and_inject(src):
     node = ast.parse(src, '<eval>', 'eval')
     return Injector().visit(node)
@@ -265,19 +276,21 @@
                 }
                 exec(code, d)
                 return d
     return {}
 
 
 def main():
+    signal.signal(signal.SIGINT, signal.SIG_DFL)
+
     # arguments
     argparser = ArgumentParser()
     argparser.add_argument('expr', nargs='?', default='d')
     argparser.add_argument('files', nargs='*', default='-', type=FileType('r'))
-    argparser.add_argument('--version', action='version', version='0.12.0')  # $version
+    argparser.add_argument('--version', action='version', version=__version__)
     argparser.add_argument('--ascii', '--ascii-output', action='store_true')
     argparser.add_argument('--monochrome-output', action='store_true')
     grp = argparser.add_mutually_exclusive_group()
     grp.add_argument('--tab', help='Use tabs for indentation', action='store_true')
     grp.add_argument('--indent', type=int, help='Use the number of spaces for indentation')
     grp.add_argument(
         '--compact-output', dest='compact', action='store_true',
@@ -295,28 +308,20 @@
         '--arg', nargs=2,
         action='append', dest='user_vars',
         metavar='VAR',
         help='Inject a variable with a value in the expression',
     )
     args = argparser.parse_args()
 
-    try:
-        do_parse_indent(args)
-
-        code = do_parse_expression(args)
-
-        inputs = do_inputs(args)
-
-        vars = do_prepare_runtime(inputs, args)
-
-        res = do_eval(code, vars, args)
-
-        do_output(res, args)
-    except SystemExit as exc:
-        return exc.args[0]
+    do_parse_indent(args)
+    code = do_parse_expression(args)
+    inputs = do_inputs(args)
+    vars = do_prepare_runtime(inputs, args)
+    res = do_eval(code, vars, args)
+    do_output(res, args)
 
 
 def do_parse_indent(args):
     args.separators = None
     if args.compact:
         args.indent = None
         args.separators = (',', ':')
@@ -402,15 +407,15 @@
         sys.exit(os.EX_DATAERR)
 
     return res
 
 
 def do_output(res, args):
     # output
-    color = not args.monochrome_output
+    color = not (args.monochrome_output or os.getenv("NO_COLOR"))
     if args.raw_output and isinstance(res, str):
         color = False
         s = res
     else:
         s = json.dumps(
             res,
             default=convert_to_jsonable,
@@ -425,9 +430,8 @@
             print(s)
         sys.stdout.close()
     except IOError:
         pass
 
 
 if __name__ == '__main__':
-    signal.signal(signal.SIGINT, signal.SIG_DFL)
-    sys.exit(main() or 0)
+    main()
```

