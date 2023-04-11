# Comparing `tmp/simplug-0.2.3.tar.gz` & `tmp/simplug-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplug-0.2.3.tar", max compression
+gzip compressed data, was "simplug-0.3.0.tar", max compression
```

## Comparing `simplug-0.2.3.tar` & `simplug-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2023-03-29 23:23:23.092213 simplug-0.2.3/LICENSE
--rw-r--r--   0        0        0     8015 2023-03-29 23:23:23.092213 simplug-0.2.3/README.md
--rw-r--r--   0        0        0      988 2023-03-29 23:23:23.092213 simplug-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    34066 2023-03-29 23:23:23.092213 simplug-0.2.3/simplug.py
--rw-r--r--   0        0        0     8855 1970-01-01 00:00:00.000000 simplug-0.2.3/setup.py
--rw-r--r--   0        0        0     8797 1970-01-01 00:00:00.000000 simplug-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-11 18:53:13.883838 simplug-0.3.0/LICENSE
+-rw-r--r--   0        0        0     8015 2023-04-11 18:53:13.883838 simplug-0.3.0/README.md
+-rw-r--r--   0        0        0      962 2023-04-11 18:53:13.883838 simplug-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    34179 2023-04-11 18:53:13.883838 simplug-0.3.0/simplug.py
+-rw-r--r--   0        0        0     8827 1970-01-01 00:00:00.000000 simplug-0.3.0/setup.py
+-rw-r--r--   0        0        0     8704 1970-01-01 00:00:00.000000 simplug-0.3.0/PKG-INFO
```

### Comparing `simplug-0.2.3/LICENSE` & `simplug-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simplug-0.2.3/README.md` & `simplug-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `simplug-0.2.3/pyproject.toml` & `simplug-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "simplug"
-version = "0.2.3"
+version = "0.3.0"
 description = "A simple plugin system for python with async hooks supported"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 homepage = "https://github.com/pwwang/simplug"
 repository  = "https://github.com/pwwang/simplug"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 diot = "^0.1"
-importlib-metadata = "^6"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-cov = "^4"
```

### Comparing `simplug-0.2.3/simplug.py` & `simplug-0.3.0/simplug.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """A simple entrypoint-free plugin system for python"""
 from __future__ import annotations
 
 import inspect
 import warnings
 from collections import namedtuple
 from enum import Enum
-from importlib import import_module
+from importlib import import_module, metadata
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     List,
     Optional,
     Tuple,
 )
 
-import importlib_metadata
 from diot import OrderedDiot
 
-__version__ = "0.2.3"
+__version__ = "0.3.0"
 
 SimplugImpl = namedtuple("SimplugImpl", ["impl", "has_self"])
 SimplugImpl.__doc__ = """A namedtuple wrapper for hook implementation.
 
 This is used to mark the method/function to be an implementation of a hook.
 
 Args:
@@ -814,15 +813,20 @@
     ) -> None:
         """Load plugins from setuptools entry_points"""
         group = group or self.project
 
         if isinstance(only, str):
             only = [only]
 
-        for ep in importlib_metadata.entry_points(group=group):
+        try:
+            eps = metadata.entry_points(group=group)
+        except TypeError:  # pragma: no cover
+            eps = metadata.entry_points().get(group, [])
+
+        for ep in eps:
             if only and ep.name not in only:
                 continue
 
             plugin = ep.load()
             self.register((plugin, ep.name))
 
     def register(self, *plugins: Any) -> None:
```

### Comparing `simplug-0.2.3/setup.py` & `simplug-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['simplug']
 install_requires = \
-['diot>=0.1,<0.2', 'importlib-metadata>=6,<7']
+['diot>=0.1,<0.2']
 
 setup_kwargs = {
     'name': 'simplug',
-    'version': '0.2.3',
+    'version': '0.3.0',
     'description': 'A simple plugin system for python with async hooks supported',
     'long_description': '# simplug\n\nA simple plugin system for python with async hooks supported\n\n## Installation\n\n```shell\npip install -U simplug\n```\n\n## Examples\n\n### A toy example\n\n```python\nfrom simplug import Simplug\n\nsimplug = Simplug(\'project\')\n\nclass MySpec:\n    """A hook specification namespace."""\n\n    @simplug.spec\n    def myhook(self, arg1, arg2):\n        """My special little hook that you can customize."""\n\nclass Plugin_1:\n    """A hook implementation namespace."""\n\n    @simplug.impl\n    def myhook(self, arg1, arg2):\n        print("inside Plugin_1.myhook()")\n        return arg1 + arg2\n\nclass Plugin_2:\n    """A 2nd hook implementation namespace."""\n\n    @simplug.impl\n    def myhook(self, arg1, arg2):\n        print("inside Plugin_2.myhook()")\n        return arg1 - arg2\n\nsimplug.register(Plugin_1, Plugin_2)\nresults = simplug.hooks.myhook(arg1=1, arg2=2)\nprint(results)\n```\n\n```shell\ninside Plugin_1.myhook()\ninside Plugin_2.myhook()\n[3, -1]\n```\n\nNote that the hooks are executed in the order the plugins are registered. This is different from `pluggy`.\n\n### A complete example\n\nSee `examples/complete/`.\n\nRunning `python -m examples.complete` gets us:\n\n```shell\nYour food. Enjoy some egg, egg, egg, salt, pepper, egg, egg\nSome condiments? We have pickled walnuts, steak sauce, mushy peas, mint sauce\n```\n\nAfter install the plugin:\n\n```shell\n> pip install --editable examples.complete.plugin\n> python -m examples.complete # run again\n```\n\n```shell\nYour food. Enjoy some egg, egg, egg, salt, pepper, egg, egg, lovely spam, wonderous spam\nSome condiments? We have pickled walnuts, mushy peas, mint sauce, spam sauce\nNow this is what I call a condiments tray!\n```\n\n## Usage\n\n### Definition of hooks\n\nHooks are specified and implemented by decorating the functions with `simplug.spec` and `simplug.impl` respectively.\n\n`simplug` is initialized by:\n\n```python\nsimplug = Simplug(\'project\')\n```\n\nThe `\'project\'` is a unique name to mark the project, which makes sure `Simplug(\'project\')` get the same instance each time.\n\nNote that if `simplug` is initialized without `project`, then a name is generated automatically as such `project-0`, `project-1`, etc.\n\nHook specification is marked by `simplug.spec`:\n\n```python\nsimplug = Simplug(\'project\')\n\n@simplug.spec\ndef setup(args):\n    ...\n```\n\n`simplug.spec` can take some arguments:\n\n- `required`: Whether this hook is required to be implemented in plugins\n- `result`: An enumerator to specify the way to collec the results.\n  - `SimplugResult.ALL`: Collect all results from all plugins\n  - `SimplugResult.ALL_AVAILS`: Get all the results from the hook, as a list, not including `None`s\n  - `SimplugResult.ALL_FIRST`: Executing all implementations and get the first result\n  - `SimplugResult.ALL_LAST`: Executing all implementations and get the last result\n  - `SimplugResult.TRY_ALL_FIRST`: Executing all implementations and get the first result, if no result is returned, return `None`\n  - `SimplugResult.TRY_ALL_LAST`: Executing all implementations and get the last result, if no result is returned, return `None`\n  - `SimplugResult.ALL_FIRST_AVAIL`: Executing all implementations and get the first non-`None` result\n  - `SimplugResult.ALL_LAST_AVAIL`: Executing all implementations and get the last non-`None` result\n  - `SimplugResult.TRY_ALL_FIRST_AVAIL`: Executing all implementations and get the first non-`None` result, if no result is returned, return `None`\n  - `SimplugResult.TRY_ALL_LAST_AVAIL`: Executing all implementations and get the last non-`None` result, if no result is returned, return `None`\n  - `SimplugResult.FIRST`: Get the first result, don\'t execute other implementations\n  - `SimplugResult.LAST`: Get the last result, don\'t execute other implementations\n  - `SimplugResult.TRY_FIRST`: Get the first result, don\'t execute other implementations, if no result is returned, return `None`\n  - `SimplugResult.TRY_LAST`: Get the last result, don\'t execute other implementations, if no result is returned, return `None`\n  - `SimplugResult.FIRST_AVAIL`: Get the first non-`None` result, don\'t execute other implementations\n  - `SimplugResult.LAST_AVAIL`: Get the last non-`None` result, don\'t execute other implementations\n  - `SimplugResult.TRY_FIRST_AVAIL`: Get the first non-`None` result, don\'t execute other implementations, if no result is returned, return `None`\n  - `SimplugResult.TRY_LAST_AVAIL`: Get the last non-`None` result, don\'t execute other implementations, if no result is returned, return `None`\n  - `SimplugResult.SINGLE`: Get the result from a single implementation\n  - `SimplugResult.TRY_SINGLE`: Get the result from a single implementation, if no result is returned, return `None`\n  - A callable to collect the result, take `calls` as the argument, a 3-element tuple with first element as the implementation, second element as the positional arguments, and third element as the keyword arguments.\n\nHook implementation is marked by `simplug.impl`, which takes no additional arguments.\n\nThe name of the function has to match the name of the function by `simplug.spec`. And the signatures of the specification function and the implementation function have to be the same in terms of names. This means you can specify default values in the specification function, but you don\'t have to write the default values in the implementation function.\n\nNote that default values in implementation functions will be ignored.\n\nAlso note if a hook specification is under a namespace, it can take `self` as argument. However, this argument will be ignored while the hook is being called (`self` will be `None`, and you still have to specify it in the function definition).\n\n### Loading plugins from setuptools entrypoint\n\nYou have to call `simplug.load_entrypoints(group)` after the hook specifications are defined to load the plugins registered by setuptools entrypoint. If `group` is not given, the project name will be used.\n\n### The plugin registry\n\nThe plugins are registered by `simplug.register(*plugins)`. Each plugin of `plugins` can be either a python object or a str denoting a module that can be imported by `importlib.import_module`.\n\nThe python object must have an attribute `name`, `__name__` or `__class.__name__` for `simplug` to determine the name of the plugin. If the plugin name is determined from `__name__` or `__class__.__name__`, it will be lowercased.\n\nIf a plugin is loaded from setuptools entrypoint, then the entrypoint name will be used (no matter what name is defined inside the plugin)\n\nYou can enable or disable a plugin temporarily after registration by:\n\n```python\nsimplug.disable(\'plugin_name\')\nsimplug.enable(\'plugin_name\')\n```\n\nYou can use following methods to inspect the plugin registry:\n\n- `simplug.get_plugin`: Get the plugin by name\n- `simplug.get_all_plugins`: Get a dictionary of name-plugin mappings of all plugins\n- `simplug.get_all_plugin_names`: Get the names of all plugins, in the order it will be executed.\n- `simplug.get_enabled_plugins`: Get a dictionary of name-plugin mappings of all enabled plugins\n- `simplug.get_enabled_plugin_names`: Get the names of all enabled plugins, in the order it will be executed.\n\n### Calling hooks\n\nHooks are call by `simplug.hooks.<hook_name>(<arguments>)` and results are collected based on the `result` argument passed in `simplug.spec` when defining hooks.\n\n### Async hooks\n\nIt makes no big difference to define an async hook:\n\n```python\n@simplug.spec\nasync def async_hook(arg):\n    ...\n\n# to supress warnings for sync implementation\n@simplug.spec(warn_sync_impl_on_async=False)\nasync def async_hook(arg):\n    ...\n```\n\nOne can implement this hook in either an async or a sync way. However, when implementing it in a sync way, a warning will be raised. To suppress the warning, one can pass a `False` value of argument `warn_sync_impl_on_async` to `simplug.spec`.\n\nTo call the async hooks (`simplug.hooks.async_hook(arg)`), you will just need to call it like any other async functions (using `asyncio.run`, for example)\n\n## API\n\nhttps://pwwang.github.io/simplug/\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/simplug',
     'py_modules': modules,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `simplug-0.2.3/PKG-INFO` & `simplug-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: simplug
-Version: 0.2.3
+Version: 0.3.0
 Summary: A simple plugin system for python with async hooks supported
 Home-page: https://github.com/pwwang/simplug
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: diot (>=0.1,<0.2)
-Requires-Dist: importlib-metadata (>=6,<7)
 Project-URL: Repository, https://github.com/pwwang/simplug
 Description-Content-Type: text/markdown
 
 # simplug
 
 A simple plugin system for python with async hooks supported
```

