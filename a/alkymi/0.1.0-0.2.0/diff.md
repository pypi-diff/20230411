# Comparing `tmp/alkymi-0.1.0.tar.gz` & `tmp/alkymi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alkymi-0.1.0.tar", last modified: Tue Mar  7 21:00:15 2023, max compression
+gzip compressed data, was "alkymi-0.2.0.tar", last modified: Tue Apr 11 02:18:04 2023, max compression
```

## Comparing `alkymi-0.1.0.tar` & `alkymi-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-03-07 21:00:15.661082 alkymi-0.1.0/
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     1066 2022-06-02 18:56:50.000000 alkymi-0.1.0/LICENSE.md
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     6021 2023-03-07 21:00:15.661082 alkymi-0.1.0/PKG-INFO
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     3812 2023-03-07 20:55:52.000000 alkymi-0.1.0/README.md
-drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-03-07 21:00:15.661082 alkymi-0.1.0/alkymi/
--rw-rw-r--   0 mathias   (1000) mathias   (1000)      395 2023-03-07 20:55:52.000000 alkymi-0.1.0/alkymi/__init__.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     6808 2022-08-04 21:51:18.000000 alkymi-0.1.0/alkymi/checksums.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     3892 2022-08-04 21:51:18.000000 alkymi-0.1.0/alkymi/config.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)    18013 2023-03-07 20:55:52.000000 alkymi-0.1.0/alkymi/core.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     4855 2022-06-02 18:56:50.000000 alkymi-0.1.0/alkymi/decorators.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)    12241 2023-03-07 20:55:52.000000 alkymi-0.1.0/alkymi/foreach_recipe.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     7185 2023-03-07 20:55:52.000000 alkymi-0.1.0/alkymi/lab.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)      124 2022-02-10 21:09:03.000000 alkymi-0.1.0/alkymi/logging.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)        0 2022-06-02 18:56:50.000000 alkymi-0.1.0/alkymi/py.typed
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     9699 2023-03-07 20:55:52.000000 alkymi-0.1.0/alkymi/recipe.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     6757 2022-06-02 18:56:50.000000 alkymi-0.1.0/alkymi/recipes.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)    13148 2022-06-02 18:56:50.000000 alkymi-0.1.0/alkymi/serialization.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)      706 2023-03-07 20:55:52.000000 alkymi-0.1.0/alkymi/types.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     2146 2023-01-30 15:26:05.000000 alkymi-0.1.0/alkymi/utils.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)      120 2023-03-07 20:55:52.000000 alkymi-0.1.0/alkymi/version.py
-drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-03-07 21:00:15.661082 alkymi-0.1.0/alkymi.egg-info/
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     6021 2023-03-07 21:00:15.000000 alkymi-0.1.0/alkymi.egg-info/PKG-INFO
--rw-rw-r--   0 mathias   (1000) mathias   (1000)      452 2023-03-07 21:00:15.000000 alkymi-0.1.0/alkymi.egg-info/SOURCES.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)        1 2023-03-07 21:00:15.000000 alkymi-0.1.0/alkymi.egg-info/dependency_links.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)       38 2023-03-07 21:00:15.000000 alkymi-0.1.0/alkymi.egg-info/requires.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)        7 2023-03-07 21:00:15.000000 alkymi-0.1.0/alkymi.egg-info/top_level.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)       38 2023-03-07 21:00:15.661082 alkymi-0.1.0/setup.cfg
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     2054 2023-03-07 20:55:52.000000 alkymi-0.1.0/setup.py
+drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-04-11 02:18:04.619157 alkymi-0.2.0/
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     6028 2023-04-11 02:18:04.619157 alkymi-0.2.0/PKG-INFO
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     3818 2023-04-11 02:15:19.000000 alkymi-0.2.0/README.md
+drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-04-11 02:18:04.619157 alkymi-0.2.0/alkymi/
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)      395 2023-03-07 20:55:52.000000 alkymi-0.2.0/alkymi/__init__.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     6808 2023-03-26 09:01:00.000000 alkymi-0.2.0/alkymi/checksums.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     4464 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/config.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)    21794 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/core.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     4855 2023-03-26 08:25:39.000000 alkymi-0.2.0/alkymi/decorators.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)    12242 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/foreach_recipe.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     9063 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/lab.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)      124 2022-02-10 21:09:03.000000 alkymi-0.2.0/alkymi/logging.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     3781 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/progress.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)        0 2022-06-02 18:56:50.000000 alkymi-0.2.0/alkymi/py.typed
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     9966 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/recipe.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     6757 2022-06-02 18:56:50.000000 alkymi-0.2.0/alkymi/recipes.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)    13154 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/serialization.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     1397 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/types.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     2595 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/utils.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)      120 2023-04-11 02:15:19.000000 alkymi-0.2.0/alkymi/version.py
+drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-04-11 02:18:04.619157 alkymi-0.2.0/alkymi.egg-info/
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     6028 2023-04-11 02:18:04.000000 alkymi-0.2.0/alkymi.egg-info/PKG-INFO
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)      460 2023-04-11 02:18:04.000000 alkymi-0.2.0/alkymi.egg-info/SOURCES.txt
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)        1 2023-04-11 02:18:04.000000 alkymi-0.2.0/alkymi.egg-info/dependency_links.txt
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)       49 2023-04-11 02:18:04.000000 alkymi-0.2.0/alkymi.egg-info/requires.txt
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)        7 2023-04-11 02:18:04.000000 alkymi-0.2.0/alkymi.egg-info/top_level.txt
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)       38 2023-04-11 02:18:04.619157 alkymi-0.2.0/setup.cfg
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     2077 2023-04-11 02:15:19.000000 alkymi-0.2.0/setup.py
```

### Comparing `alkymi-0.1.0/PKG-INFO` & `alkymi-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alkymi
-Version: 0.1.0
+Version: 0.2.0
 Summary: alkymi - Pythonic task automation
 Home-page: https://github.com/MathiasStokholm/alkymi
 Author: Mathias Bøgh Stokholm
 Author-email: mathias.stokholm@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/MathiasStokholm/alkymi/
 Project-URL: Tracker, https://github.com/MathiasStokholm/alkymi/issues
@@ -13,20 +13,20 @@
         
         [![build](https://github.com/MathiasStokholm/alkymi/workflows/build/badge.svg?branch=master)](https://github.com/MathiasStokholm/alkymi/actions?query=workflow%3Abuild)
         [![docs](https://readthedocs.org/projects/alkymi/badge/?version=latest)](https://alkymi.readthedocs.io/en/latest/?badge=latest)
         [![coverage](https://codecov.io/gh/MathiasStokholm/alkymi/branch/develop/graph/badge.svg?token=L0DTW805NL)](https://codecov.io/gh/MathiasStokholm/alkymi)
         [![pypi](https://img.shields.io/pypi/v/alkymi.svg)](https://pypi.org/project/alkymi)
         [![versions](https://img.shields.io/pypi/pyversions/alkymi.svg)](https://pypi.org/project/alkymi)
         
-        Alkymi is a pure Python (3.6+) library for describing and executing tasks and pipelines with built-in caching and
+        Alkymi is a pure Python (3.7+) library for describing and executing tasks and pipelines with built-in caching and
         conditional evaluation based on checksums.
         
-        Alkymi is easy to install, simple to use, and has no dependencies outside of Python's standard library. The code is
-        cross-platform, and allows you to write your pipelines once and deploy to multiple operating systems (tested on Linux,
-        Windows and Mac).
+        Alkymi is easy to install, simple to use, and has very few dependencies outside of Python's standard library. The code
+        is cross-platform, and allows you to write your pipelines once and deploy to multiple operating systems (tested on
+        Linux, Windows and Mac).
         
         Documentation, including a quickstart guide, is provided [here](https://alkymi.readthedocs.io/en/latest/).
         
         ## Features
         * Easily define complex data pipelines as decorated Python functions
           * This allows you to run linting, type checking, etc. on your data pipelines
         * Return values are automatically cached to disk, regardless of type
@@ -95,23 +95,23 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: xxhash
```

### Comparing `alkymi-0.1.0/README.md` & `alkymi-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 [![build](https://github.com/MathiasStokholm/alkymi/workflows/build/badge.svg?branch=master)](https://github.com/MathiasStokholm/alkymi/actions?query=workflow%3Abuild)
 [![docs](https://readthedocs.org/projects/alkymi/badge/?version=latest)](https://alkymi.readthedocs.io/en/latest/?badge=latest)
 [![coverage](https://codecov.io/gh/MathiasStokholm/alkymi/branch/develop/graph/badge.svg?token=L0DTW805NL)](https://codecov.io/gh/MathiasStokholm/alkymi)
 [![pypi](https://img.shields.io/pypi/v/alkymi.svg)](https://pypi.org/project/alkymi)
 [![versions](https://img.shields.io/pypi/pyversions/alkymi.svg)](https://pypi.org/project/alkymi)
 
-Alkymi is a pure Python (3.6+) library for describing and executing tasks and pipelines with built-in caching and
+Alkymi is a pure Python (3.7+) library for describing and executing tasks and pipelines with built-in caching and
 conditional evaluation based on checksums.
 
-Alkymi is easy to install, simple to use, and has no dependencies outside of Python's standard library. The code is
-cross-platform, and allows you to write your pipelines once and deploy to multiple operating systems (tested on Linux,
-Windows and Mac).
+Alkymi is easy to install, simple to use, and has very few dependencies outside of Python's standard library. The code
+is cross-platform, and allows you to write your pipelines once and deploy to multiple operating systems (tested on
+Linux, Windows and Mac).
 
 Documentation, including a quickstart guide, is provided [here](https://alkymi.readthedocs.io/en/latest/).
 
 ## Features
 * Easily define complex data pipelines as decorated Python functions
   * This allows you to run linting, type checking, etc. on your data pipelines
 * Return values are automatically cached to disk, regardless of type
```

### Comparing `alkymi-0.1.0/alkymi/checksums.py` & `alkymi-0.2.0/alkymi/checksums.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.1.0/alkymi/config.py` & `alkymi-0.2.0/alkymi/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import enum
-from pathlib import Path
 import os
+from pathlib import Path
 from typing import Optional
 
+from .types import ProgressType
+
 
 @enum.unique
 class CacheType(enum.Enum):
     """
     Supported caching mechanisms
     """
     Cache = 0  # Enable caching
@@ -48,14 +50,15 @@
 
         # Set default values in config
         AlkymiConfig.__instance = self
         self._cache = True
         self._cache_path = None
         self._allow_pickling = True
         self._file_checksum_method = FileChecksumMethod.HashContents
+        self._progress_type = ProgressType.Fancy
 
     @property
     def cache(self) -> bool:
         """
         :return: Whether to enable alkymi caching globally (see CacheType.Auto)
         """
         return self._cache
@@ -117,10 +120,26 @@
         """
         Set the method to use for calculating file checksums (for Path objects)
 
         :param file_checksum_method: The method to use for calculating file checksums (for Path objects)
         """
         self._file_checksum_method = file_checksum_method
 
+    @property
+    def progress_type(self) -> ProgressType:
+        """
+        :return: The currently used type of progress indication
+        """
+        return self._progress_type
+
+    @progress_type.setter
+    def progress_type(self, progress_type: ProgressType) -> None:
+        """
+        Set the type of progress indication to use during recipe evaluation
+
+        :param progress_type: The type of progress indication to use
+        """
+        self._progress_type = progress_type
+
 
 # Force creation of singleton
 ALKYMI_CONFIG = AlkymiConfig.get()
```

### Comparing `alkymi-0.1.0/alkymi/core.py` & `alkymi-0.2.0/alkymi/core.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import asyncio
 import concurrent.futures
-from asyncio import Future, AbstractEventLoop
-from typing import Dict, Tuple, Optional, Awaitable, Any
+import typing
+from asyncio import Future, AbstractEventLoop, Task
+from typing import Dict, Tuple, Optional, Any, Coroutine, Union
+
+import networkx as nx
 
 from . import checksums
+from .config import ProgressType, AlkymiConfig
 from .foreach_recipe import ForeachRecipe, MappedOutputs, MappedInputs
-from .serialization import OutputWithValue
-from .types import Status
-from .recipe import Recipe, R
 from .logging import log
-
-import networkx as nx
+from .progress import FancyProgress
+from .recipe import Recipe, R
+from .serialization import OutputWithValue
+from .types import Status, ProgressCallback, EvaluateProgress
 
 OutputsAndChecksums = Tuple[R, Optional[str]]
 
 
 def create_graph(recipe: Recipe[R]) -> nx.DiGraph:
     """
     Create a Directed Acyclic Graph (DAG) based on the provided recipe
@@ -100,40 +103,65 @@
     """
     # Start recursion with an empty status dict
     statuses: Dict[Recipe, Status] = {}
     _compute_status(recipe, graph, statuses)
     return statuses
 
 
-def invoke(recipe: Recipe, inputs: Tuple[Any, ...], input_checksums: Tuple[Optional[str], ...]) -> OutputsAndChecksums:
+async def invoke(recipe: Recipe, inputs: Tuple[Any, ...], input_checksums: Tuple[Optional[str], ...],
+                 loop: AbstractEventLoop, executor: Optional[concurrent.futures.Executor],
+                 progress_callback: Optional[ProgressCallback] = None) -> OutputsAndChecksums:
     """
     Evaluate the Recipe using the provided inputs. This will call the bound function on the inputs.
 
     :param recipe: The recipe to evaluate given the provided inputs
     :param inputs: The inputs provided by the ingredients (dependencies) of the Recipe
     :param input_checksums: The (possibly new) input checksum
+    :param loop: The asyncio event loop to use for scheduling the recipe evaluation
+    :param executor: An optional executor to use for evaluating bound functions in parallel
+    :param progress_callback: An optional callback to invoke when evaluation progress occurs
+    :return: The output(s) and checksum(s) of the evaluated recipe
     """
     log.debug('Invoking recipe: {}'.format(recipe.name))
-    outputs = recipe(*inputs)
+
+    # Signal that work has started on 1 out of 1 unit of work
+    if progress_callback is not None:
+        progress_callback(EvaluateProgress.Started, recipe, 1, 1)
+
+    # Run code on executor if applicable, otherwise evaluate directly on this thread
+    if executor is not None:
+        outputs = await loop.run_in_executor(executor, recipe, *inputs)
+    else:
+        outputs = recipe(*inputs)
     recipe.set_result(outputs, input_checksums)
+
+    # Signal that work has completed on 1 out of 1 unit of work
+    if progress_callback is not None:
+        progress_callback(EvaluateProgress.Done, recipe, 1, 1)
+
     return recipe.outputs, recipe.output_checksum
 
 
-def invoke_foreach(recipe: ForeachRecipe, inputs: Tuple[Any, ...],
-                   input_checksums: Tuple[Optional[str], ...],
-                   executor: Optional[concurrent.futures.Executor]) -> OutputsAndChecksums:
+async def invoke_foreach(recipe: ForeachRecipe, inputs: Tuple[Any, ...],
+                         input_checksums: Tuple[Optional[str], ...],
+                         loop: AbstractEventLoop,
+                         executor: Optional[concurrent.futures.Executor],
+                         progress_callback: Optional[ProgressCallback] = None) -> OutputsAndChecksums:
     """
     Evaluate the ForeachRecipe using the provided inputs. This will apply the bound function to each item in the
     "mapped_inputs". If the result for any item is already cached, that result will be used instead (the checksum
     is used to check this). Only items from the immediately previous invoke call will be cached
 
     :param recipe: The ForeachRecipe to evaluate given the provided inputs
     :param inputs: The inputs provided by the ingredients (dependencies) of the ForeachRecipe
     :param input_checksums: The (possibly new) input checksum to use for checking cleanliness
-    :param executor: The executor to use for calling the bound function in parallel
+    :param loop: The asyncio event loop to use for scheduling the recipe evaluation
+    :param executor: An optional executor to use for evaluating bound functions in parallel
+    :param progress_callback: An optional callback to invoke when evaluation progress occurs
+    :return: The output(s) and checksum(s) of the evaluated recipe
     """
     log.debug("Invoking recipe: {}".format(recipe.name))
 
     # The first ingredient will provide the sequence to apply the bound function too
     mapped_inputs = inputs[0]
     mapped_inputs_checksum = input_checksums[0]
     other_inputs = inputs[1:]
@@ -199,125 +227,166 @@
                         found_output = recipe.mapped_outputs[key]
                         if found_output.valid:
                             outputs[key] = found_output
                             evaluated[key] = item
                             continue
                 not_evaluated[key] = item
 
+    # Signal that work has started on X out of Y units of work
+    if progress_callback is not None:
+        progress_callback(EvaluateProgress.Started, recipe, len(mapped_inputs), len(evaluated))
+
     log.debug("Num already cached results: {}/{}".format(len(evaluated), len(mapped_inputs)))
     if len(evaluated) == len(mapped_inputs):
         log.debug("Returning early since all items were already cached")
         recipe.set_current_result(evaluated, outputs, mapped_inputs_checksum, other_input_checksums, True)
         return recipe.outputs, recipe.output_checksum
 
     # Perform remaining work - store state every time an evaluation is successful
+    results: typing.Iterable[Any]
     if isinstance(not_evaluated, list) and isinstance(outputs, list) and isinstance(evaluated, list):
         if executor is not None:
-            results = executor.map(lambda _item: recipe(_item, *other_inputs), not_evaluated)
+            results = [loop.run_in_executor(executor, recipe.__call__, _item, *other_inputs) for _item in
+                       not_evaluated]
         else:
             results = map(lambda _item: recipe(_item, *other_inputs), not_evaluated)
-        for item, result in zip(not_evaluated, results):
+        for item, maybe_async_result in zip(not_evaluated, results):
+            result = await maybe_async_result if isinstance(maybe_async_result, Future) else maybe_async_result
             outputs.append(OutputWithValue(result, checksums.checksum(result)))
             evaluated.append(item)
             recipe.set_current_result(evaluated, outputs, mapped_inputs_checksum, other_input_checksums, False)
+
+            # Signal that work has completed on X out of Y units of work
+            if progress_callback is not None:
+                progress_callback(EvaluateProgress.InProgress, recipe, len(mapped_inputs), len(evaluated))
     elif isinstance(not_evaluated, dict):
         if executor is not None:
-            results = executor.map(lambda _item: recipe(_item, *other_inputs), not_evaluated.values())
+            results = [loop.run_in_executor(executor, recipe.__call__, _item, *other_inputs) for _item in
+                       not_evaluated.values()]
         else:
             results = map(lambda _item: recipe(_item, *other_inputs), not_evaluated.values())
-        for (key, item), result in zip(not_evaluated.items(), results):
+        for (key, item), maybe_async_result in zip(not_evaluated.items(), results):
+            result = await maybe_async_result if isinstance(maybe_async_result, Future) else maybe_async_result
             outputs[key] = OutputWithValue(result, checksums.checksum(result))
             evaluated[key] = item
             recipe.set_current_result(evaluated, outputs, mapped_inputs_checksum, other_input_checksums, False)
 
-    recipe.set_current_result(evaluated, outputs, mapped_inputs_checksum, other_input_checksums, True)
-    return recipe.outputs, recipe.output_checksum
+            # Signal that work has completed on X out of Y units of work
+            if progress_callback is not None:
+                progress_callback(EvaluateProgress.InProgress, recipe, len(mapped_inputs), len(evaluated))
 
+    recipe.set_current_result(evaluated, outputs, mapped_inputs_checksum, other_input_checksums, True)
 
-def retrieve_recipe_outputs(foreach_executor: Optional[concurrent.futures.Executor], recipe: Recipe, status: Status,
-                            inputs_and_checksums: Tuple[OutputsAndChecksums, ...] = ()) -> OutputsAndChecksums:
-    """
-    Helper function to delegate recipe invocation calls
+    # Signal that work has completed on N out of N units of work
+    if progress_callback is not None:
+        progress_callback(EvaluateProgress.Done, recipe, len(mapped_inputs), len(evaluated))
 
-    :param foreach_executor: The executor (if any) that should be used for evaluating ForeachRecipes in parallel
-    :param recipe: The recipe to evaluate using the executor
-    :param status: The status of the recipe - used to skip evaluation if unnecessary
-    :param inputs_and_checksums: The inputs and checksums of these to provide to the recipe for evaluation
-    :return: The output(s) and checksum(s) of the recipe
-    """
-    # If status is not Ok, call invoke to run recipe
-    if status != Status.Ok:
-        _inputs = tuple(inp[0] for inp in inputs_and_checksums)
-        _input_checksums = tuple(inp[1] for inp in inputs_and_checksums)
-        if isinstance(recipe, ForeachRecipe):
-            return invoke_foreach(recipe, _inputs, _input_checksums, foreach_executor)
-        else:
-            return invoke(recipe, _inputs, _input_checksums)
     return recipe.outputs, recipe.output_checksum
 
 
-async def schedule(loop: AbstractEventLoop, graph_executor: concurrent.futures.Executor,
-                   foreach_executor: Optional[concurrent.futures.Executor], recipe: Recipe,
-                   statuses: Dict[Recipe, Status],
-                   inputs_and_checksum_futures: Tuple[Awaitable[OutputsAndChecksums], ...]) -> Future:
+async def schedule(loop: AbstractEventLoop, executor: Optional[concurrent.futures.Executor], recipe: Recipe,
+                   status: Status, coros_or_tasks: Dict[Recipe, Union[Coroutine, Task]],
+                   progress_callback: Optional[ProgressCallback] = None) -> OutputsAndChecksums:
     """
-    Helper function used to asynchronously await inputs from dependant recipe futures, and then retrieve the output of
-    the provided recipe using the provided executor (evaluating it if necessary)
+    Helper function used to asynchronously await inputs from dependant recipes, and then retrieve the output of the
+    provided recipe (evaluating it if necessary). Note that inputs will only be awaited if needed (not if cached).
 
     :param loop: The asyncio event loop to use for scheduling the recipe evaluation
-    :param graph_executor: The executor that is being used to evaluate the graph
-    :param foreach_executor: The executor (if any) that should be used for evaluating ForeachRecipes in parallel
+    :param executor: An optional executor to use for evaluating bound functions in parallel
     :param recipe: The recipe to evaluate using the executor
-    :param statuses: The statuses of the recipes contained in the graph - used to skip evaluation if unnecessary
-    :param inputs_and_checksum_futures: A tuple of futures to await before providing them to the recipe evaluation
+    :param status: The status of the recipe being scheduled - used to skip evaluation if unnecessary
+    :param coros_or_tasks: Dictionary containing coroutines for recipes - used to await ingredient inputs
+    :param progress_callback: An optional callback to invoke when evaluation progress occurs
     :return: A future that will eventually return the output(s) and checksum(s) of the recipe
     """
-    inputs_and_checksums = tuple([await inp for inp in inputs_and_checksum_futures])
-    return loop.run_in_executor(graph_executor, retrieve_recipe_outputs, foreach_executor, recipe, statuses[recipe],
-                                inputs_and_checksums)
+
+    # If status is Ok, simply return the result and checksum
+    if status == Status.Ok:
+        return recipe.outputs, recipe.output_checksum
+
+    # Status is not Ok - evaluation needed
+    # Convert needed inputs from coroutines to tasks - this is done to ensure that multiple recipes can await the result
+    input_futures = []
+    for ingredient in recipe.ingredients:
+        coro_or_task = coros_or_tasks[ingredient]
+        if not isinstance(coro_or_task, asyncio.Task):
+            coro_or_task = loop.create_task(coro_or_task)
+            coros_or_tasks[ingredient] = coro_or_task
+        input_futures.append(coro_or_task)
+
+    # Block while waiting for inputs to become available
+    inputs_and_checksums = tuple(await asyncio.gather(*input_futures))
+    inputs = tuple(inp[0] for inp in inputs_and_checksums)
+    input_checksums = tuple(inp[1] for inp in inputs_and_checksums)
+    if isinstance(recipe, ForeachRecipe):
+        return await invoke_foreach(recipe, inputs, input_checksums, loop, executor, progress_callback)
+    else:
+        return await invoke(recipe, inputs, input_checksums, loop, executor, progress_callback)
 
 
-def evaluate_recipe(recipe: Recipe[R], graph: nx.DiGraph, statuses: Dict[Recipe, Status], jobs: int) -> \
-        OutputsAndChecksums[R]:
+def evaluate_recipe(recipe: Recipe[R], graph: nx.DiGraph, statuses: Dict[Recipe, Status], jobs: int,
+                    progress_type: Optional[ProgressType] = None) -> OutputsAndChecksums[R]:
     """
     Evaluate a Recipe, including any dependencies that are not up-to-date
 
     :param recipe: The recipe to evaluate
     :param graph: The graph to use for evaluation
     :param statuses: The statuses of the recipes contained in the graph - used to skip evaluation if unnecessary
     :param jobs: The number of jobs to use for evaluating the recipe in parallel, 1 job corresponds to no parallelism,
                  zero or negative values will cause alkymi to use the system's default number of jobs
+    :param progress_type: The method to use for showing progress, if None will default to setting in alkymi's config
     :return: The output(s) and checksum(s) of the evaluated recipe
     """
-    # Create the executor to use for evaluating recipes
-    executor = concurrent.futures.ThreadPoolExecutor(max_workers=jobs if jobs > 0 else None)
+    # Create the executor to use for evaluating bound functions
+    executor: Optional[concurrent.futures.Executor]
+    if jobs == 1:
+        executor = None
+    else:
+        executor = concurrent.futures.ThreadPoolExecutor(max_workers=jobs if jobs > 0 else None)
 
-    # If we have more than 1 job (threads) available, also use the executor for running ForeachRecipes in parallel
-    foreach_executor = executor if jobs > 1 else None
+    # Determine the progress type to use - if not provided by caller, use current setting in alkymi's global config
+    if progress_type is None:
+        progress_type = AlkymiConfig.get().progress_type
+    progress = FancyProgress(graph, statuses, recipe) if progress_type == ProgressType.Fancy else None
 
     # Create the asyncio event loop and set it on the calling thread
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
 
     async def _execute() -> OutputsAndChecksums[R]:
         # Sort the graph topographically, such that any recipe in the sorted list only depends on earlier recipes
         # This guarantees that futures only depend on already created futures
         recipes = list(nx.topological_sort(graph))
 
-        # Schedule all recipes to execute as soon as their inputs are available
-        tasks: Dict[Recipe, Future] = {}
+        # Create coroutines to evaluate each recipe - then from the top-down, the coroutines will request inputs that
+        # they need from other coroutines, which will be upgraded to tasks
+        # This approach is used to avoid loading outputs for recipes whose outputs are actually unused, because later
+        # recipes are already cached
+        coros_or_tasks: Dict[Recipe, Union[Coroutine, Task]] = {}
         for _recipe in recipes:
-            input_futures = tuple(tasks[ingredient] for ingredient in _recipe.ingredients)
-            tasks[_recipe] = await schedule(loop, executor, foreach_executor, _recipe, statuses, input_futures)
+            # Note that 'schedule()' might mutate 'tasks' once awaited
+            coros_or_tasks[_recipe] = schedule(loop, executor, _recipe, statuses[_recipe], coros_or_tasks,
+                                               progress)
 
         # Wait for future for target recipe to return
-        return await tasks[recipe]
+        result = await coros_or_tasks[recipe]
+
+        # Close coroutines that were not converted to tasks, since they were never needed for the execution
+        for coro_or_task in coros_or_tasks.values():
+            if not isinstance(coro_or_task, asyncio.Task):
+                coro_or_task.close()
+
+        return result
 
     # Return the output and checksum of the final recipe
+    if progress is not None:
+        progress.start()
     output, checksum = loop.run_until_complete(_execute())
+    if progress is not None:
+        progress.stop()
     return output, checksum
 
 
 def is_clean(recipe: Recipe[R], new_input_checksums: Tuple[Optional[str], ...]) -> Status:
     """
     Check whether a Recipe is clean (result is cached) based on a set of (potentially new) input checksums
 
@@ -348,21 +417,22 @@
     if not recipe.outputs_valid:
         return Status.OutputsInvalid
 
     # All checks passed
     return Status.Ok
 
 
-def brew(recipe: Recipe[R], *, jobs: int) -> R:
+def brew(recipe: Recipe[R], *, jobs: int, progress_type: Optional[ProgressType]) -> R:
     """
     Evaluate a Recipe and all dependent inputs - this will build the computational graph and execute any needed
     dependencies to produce the outputs of the input Recipe
 
     :param recipe: The Recipe to evaluate
     :param jobs: The number of jobs to use for evaluating the recipe in parallel, 1 job corresponds to no parallelism,
                  zero or negative values will cause alkymi to use the system's default number of jobs
+    :param progress_type: The method to use for showing progress, if None will default to setting in alkymi's config
     :return: The outputs of the Recipe (which correspond to the outputs of the bound function)
     """
     graph = create_graph(recipe)
     statuses = compute_recipe_status(recipe, graph)
-    result, _ = evaluate_recipe(recipe, graph, statuses, jobs)
+    result, _ = evaluate_recipe(recipe, graph, statuses, jobs, progress_type)
     return result
```

### Comparing `alkymi-0.1.0/alkymi/decorators.py` & `alkymi-0.2.0/alkymi/decorators.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.1.0/alkymi/foreach_recipe.py` & `alkymi-0.2.0/alkymi/foreach_recipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,14 +214,15 @@
             output_checksum=self.output_checksum,
             last_function_hash=self._last_function_hash,
             mapped_inputs_checksums=self.mapped_inputs_checksums,
             mapped_inputs_checksum=self.mapped_inputs_checksum,
             mapped_type="dict" if self.mapped_inputs_type == dict else "list"
         )
 
+
     def restore_from_dict(self, old_state: Dict) -> None:
         """
         Restores the state of this ForeachRecipe from a previously cached state
 
         :param old_state: The old cached state to restore
         """
         log.debug("Restoring {} from dict".format(self._name))
```

### Comparing `alkymi-0.1.0/alkymi/lab.py` & `alkymi-0.2.0/alkymi/lab.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import argparse
 import logging
 import sys
-from typing import Dict, Union, Any, List, Iterable, Optional, TextIO
+from typing import Dict, Union, Any, List, Optional
+from typing import Iterable, TextIO
+
+from rich import console
 
 from .core import Status, compute_recipe_status, create_graph
 from .logging import log
 from .recipe import Recipe
 from .recipes import Arg
+from .types import ProgressType
 
 
 class Lab:
     """
     Class used to define a collection of alkymi recipes and expose them as a command line interface (CLI)
 
     This can be used to create files that bear resemblance to Makefiles (see alkymi/labfile.py as an example)
@@ -21,14 +25,15 @@
         Creates a new Lab with the provided name
 
         :param name: The name of the Lab
         """
         self._name = name
         self._recipes: List[Recipe] = []
         self._args: Dict[str, Arg] = {}
+        self._console = console.Console(stderr=False)  # Default to using stdout for output
 
     def add_recipe(self, recipe: Recipe) -> Recipe:
         """
         Add a new recipe to the Lab (this will make the recipe available through the CLI)
 
         :param recipe: The recipe to add
         :return: The input recipe (to allow chaining calls)
@@ -50,33 +55,44 @@
         """
         Register an argument with the Lab (this will make the argument settable through the CLI)
 
         :param arg: The argument to register
         """
         self._args[arg.name] = arg
 
-    def brew(self, target_recipe: Union[Recipe, str], *, jobs=1) -> Any:
+    def brew(self, target_recipe: Union[Recipe, str], *, jobs=1,
+             progress_type: Optional[ProgressType] = ProgressType.Fancy) -> Any:
         """
         Brew (evaluate) a target recipe defined by its reference or name, and return the results
 
         :param target_recipe: The recipe to evaluate, as a reference ot by name
         :param jobs: The number of jobs to use for evaluating this recipe in parallel, defaults to 1 (no parallelism),
                      zero or negative values will cause alkymi to use the system's default number of jobs
+        :param progress_type: The method to use for showing progress, if None will default to setting in alkymi's config
         :return: The output of the evaluated recipe
         """
+
+        # Helper function to call brew on the matched recipe with CTRL-C handling
+        def _call_brew(_recipe: Recipe) -> Any:
+            try:
+                return _recipe.brew(jobs=jobs, progress_type=progress_type)
+            except KeyboardInterrupt:
+                self._console.print("[bold red]Interrupted by user")
+                sys.exit(1)
+
         if isinstance(target_recipe, str):
             # Try to match name
             for recipe in self._recipes:
                 if recipe.name == target_recipe:
-                    return recipe.brew(jobs=jobs)
+                    return _call_brew(recipe)
             raise ValueError("Unknown recipe: {}".format(target_recipe))
         else:
             # Match recipe directly
             if target_recipe in self._recipes:
-                return target_recipe.brew(jobs=jobs)
+                return _call_brew(target_recipe)
             raise ValueError("Unknown recipe: {}".format(target_recipe.name))
 
     @property
     def name(self) -> str:
         """
         :return: The name of this Lab
         """
@@ -128,15 +144,34 @@
         """
         status = self._build_full_status()
         state = ''
         for recipe in self._recipes:
             state += '\n\t{} - {}'.format(recipe.name, status[recipe])
         return '{} lab with recipes:{}'.format(self.name, state)
 
-    def open(self, args: Optional[List[str]] = None, stream: TextIO = sys.stderr) -> None:
+    def print_status(self) -> None:
+        colors = {
+            Status.Ok: "green",
+            Status.NotEvaluatedYet: "red",
+            Status.CustomDirty: "yellow",
+            Status.BoundFunctionChanged: "yellow",
+            Status.IngredientDirty: "yellow",
+            Status.InputsChanged: "yellow",
+            Status.OutputsInvalid: "yellow",
+        }
+
+        status = self._build_full_status()
+        state = ''
+        for recipe in self._recipes:
+            color = colors[status[recipe]]
+            status_string = status[recipe].name.replace("Status.", "")
+            state += '\n\t[cyan]{} - [{}]{}'.format(recipe.name, color, status_string)
+        self._console.print('[bold]{} lab with recipes:[/bold]{}'.format(self.name, state))
+
+    def open(self, args: Optional[List[str]] = None, stream: TextIO = sys.stdout) -> None:
         """
         Runs the command line interface for this Lab by parsing command line arguments and carrying out the designated
         command
 
         :param args: The input arguments to use - will default to system args
         :param stream: The stream to print output to
         """
@@ -159,30 +194,36 @@
 
         # Create the parser for the "brew" command
         brew_parser = subparsers.add_parser('brew', help='Brew the selected recipe')
         brew_parser.add_argument('recipe', choices=[recipe.name for recipe in self._recipes], nargs="+",
                                  help='Recipe(s) to brew')
         brew_parser.add_argument("-j", "--jobs", type=int, default=1,
                                  help="Use N jobs to evaluate the recipe, more than 1 job will parallelize evaluation")
+        brew_parser.add_argument("--progress", type=ProgressType, default=ProgressType.Fancy,
+                                 choices=list(ProgressType), help="The type of progress indication to use")
         self._add_user_args_(brew_parser)
 
         parsed_args = parser.parse_args(args)
         log.addHandler(logging.StreamHandler(stream))
         if parsed_args.verbose:
             log.setLevel(logging.DEBUG)
         else:
             log.setLevel(logging.INFO)
 
+        # Create a new console object if output needs to go elsewhere
+        if self._console.file != stream:
+            self._console = console.Console(file=stream)
+
         # Set arguments if supplied
         for arg_name, arg in self._args.items():
             provided_val = getattr(parsed_args, arg_name, None)
             if provided_val is not None:
                 arg.set(provided_val)
 
         if parsed_args.subparser_name == 'status':
-            print(self, file=stream)
+            self.print_status()
         elif parsed_args.subparser_name == 'brew':
             for recipe in parsed_args.recipe:
-                self.brew(recipe, jobs=parsed_args.jobs)
+                self.brew(recipe, jobs=parsed_args.jobs, progress_type=parsed_args.progress)
         else:
             # No recognized command provided - print help
             parser.print_help(file=stream)
```

### Comparing `alkymi-0.1.0/alkymi/recipe.py` & `alkymi-0.2.0/alkymi/recipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import Iterable, Callable, List, Optional, Tuple, TypeVar, Generic, cast
 
 from . import checksums, serialization
 from .config import CacheType, AlkymiConfig
 from .logging import log
 from .serialization import OutputWithValue, CachedOutput, Output
-from .types import Status
+from .types import Status, ProgressType
 
 R = TypeVar("R")  # The return type of the bound function
 
 CleanlinessFunc = Callable[[R], bool]
 
 
 class Recipe(Generic[R]):
@@ -88,26 +88,27 @@
         :param input_checksums: The checksums of the inputs that were used to calculate the outputs
         """
         self.outputs = outputs
         self._input_checksums = input_checksums
         self._last_function_hash = self.function_hash
         self._save_state()
 
-    def brew(self, *, jobs: int = 1) -> R:
+    def brew(self, *, jobs: int = 1, progress_type: Optional[ProgressType] = None) -> R:
         """
         Evaluate this Recipe and all dependent inputs - this will build the computational graph and execute any needed
         dependencies to produce the outputs of this Recipe
 
         :param jobs: The number of jobs to use for evaluating this recipe in parallel, defaults to 1 (no parallelism),
                      zero or negative values will cause alkymi to use the system's default number of jobs
+        :param progress_type: The method to use for showing progress, if None will default to setting in alkymi's config
         :return: The outputs of this Recipe (which correspond to the outputs of the bound function)
         """
         # Lazy import to avoid circular imports
         from .core import brew
-        return brew(self, jobs=jobs)
+        return brew(self, jobs=jobs, progress_type=progress_type)
 
     def status(self) -> Status:
         """
         :return: The status of this recipe (will evaluate all upstream dependencies)
         """
         # Lazy import to avoid circular imports
         from .core import compute_recipe_status, create_graph
@@ -246,7 +247,10 @@
         """
         log.debug("Restoring {} from dict".format(self._name))
         if old_state["input_checksums"] is not None:
             self._input_checksums = tuple(old_state["input_checksums"])
         if old_state["outputs"] is not None and old_state["output_checksum"] is not None:
             self._outputs = CachedOutput(None, old_state["output_checksum"], old_state["outputs"])
         self._last_function_hash = cast(str, old_state["last_function_hash"])
+
+    def __repr__(self) -> str:
+        return self.name
```

### Comparing `alkymi-0.1.0/alkymi/recipes.py` & `alkymi-0.2.0/alkymi/recipes.py`

 * *Files identical despite different names*

### Comparing `alkymi-0.1.0/alkymi/serialization.py` & `alkymi-0.2.0/alkymi/serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
     def value(self) -> T:
         """
         :return: The value associated with this Output
         """
         pass
 
 
-class OutputWithValue(Output):
+class OutputWithValue(Output[T]):
     """
     An Output that is guaranteed to have an in-memory value - all outputs start out as this before being cached
     """
 
     def __init__(self, value: T, checksum: str):
         """
         Create a new OutputWithValue
@@ -281,15 +281,15 @@
         # TODO(mathias): Find out if this is too expensive in general
         return checksums.checksum(self._value) == self.checksum
 
     def value(self) -> T:
         return self._value
 
 
-class CachedOutput(Output):
+class CachedOutput(Output[T]):
     """
     An Output that has been cached - may or may not have it's associated value in-memory
     """
 
     def __init__(self, value: Optional[T], checksum: str, serializable_representation: SerializableRepresentation):
         """
         Create a new CachedOutput
```

### Comparing `alkymi-0.1.0/alkymi/utils.py` & `alkymi-0.2.0/alkymi/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,18 @@
     log)
 
     :param args: The arguments representing the command to run, e.g. ["echo", "test"]
     :param echo_error_to_stream: A stream to which to echo the call's stderr on a non-zero exit code
     :param echo_output_to_stream: A stream to which to echo the call's stdout while the command is executing
     :return: The result of the execution as a subprocess.CompletedProcess instance
     """
+    # If running through a Lab CLI, sys.stdout may have been redirected
+    if echo_output_to_stream is not None and getattr(echo_output_to_stream, "name", None) == sys.stdout.name:
+        echo_output_to_stream = sys.stdout
+
     # Buffer one line at a time if echoing live, otherwise just use the default
     buffer_size = 1 if echo_output_to_stream is not None else -1
     proc = subprocess.Popen(args, universal_newlines=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                             bufsize=buffer_size)
 
     # Since we set these to PIPE, these should never be None
     assert proc.stdout is not None
@@ -28,14 +32,20 @@
     stdout: str = ""
     if echo_output_to_stream is not None:
         # Print each line to the stream as it arrives
         while proc.poll() is None:
             line = proc.stdout.readline()
             echo_output_to_stream.write(line)
             stdout += line
+
+        # Program has finished executing, check if any part of stdout still needs to be piped
+        line = proc.stdout.readline()
+        if line:
+            echo_output_to_stream.write(line)
+            stdout += line
     else:
         # Otherwise, simply wait for the command to finish and then grab stdout
         proc.wait()
         stdout = proc.stdout.read()
 
     stderr = proc.stderr.read()
```

### Comparing `alkymi-0.1.0/alkymi.egg-info/PKG-INFO` & `alkymi-0.2.0/alkymi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alkymi
-Version: 0.1.0
+Version: 0.2.0
 Summary: alkymi - Pythonic task automation
 Home-page: https://github.com/MathiasStokholm/alkymi
 Author: Mathias Bøgh Stokholm
 Author-email: mathias.stokholm@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/MathiasStokholm/alkymi/
 Project-URL: Tracker, https://github.com/MathiasStokholm/alkymi/issues
@@ -13,20 +13,20 @@
         
         [![build](https://github.com/MathiasStokholm/alkymi/workflows/build/badge.svg?branch=master)](https://github.com/MathiasStokholm/alkymi/actions?query=workflow%3Abuild)
         [![docs](https://readthedocs.org/projects/alkymi/badge/?version=latest)](https://alkymi.readthedocs.io/en/latest/?badge=latest)
         [![coverage](https://codecov.io/gh/MathiasStokholm/alkymi/branch/develop/graph/badge.svg?token=L0DTW805NL)](https://codecov.io/gh/MathiasStokholm/alkymi)
         [![pypi](https://img.shields.io/pypi/v/alkymi.svg)](https://pypi.org/project/alkymi)
         [![versions](https://img.shields.io/pypi/pyversions/alkymi.svg)](https://pypi.org/project/alkymi)
         
-        Alkymi is a pure Python (3.6+) library for describing and executing tasks and pipelines with built-in caching and
+        Alkymi is a pure Python (3.7+) library for describing and executing tasks and pipelines with built-in caching and
         conditional evaluation based on checksums.
         
-        Alkymi is easy to install, simple to use, and has no dependencies outside of Python's standard library. The code is
-        cross-platform, and allows you to write your pipelines once and deploy to multiple operating systems (tested on Linux,
-        Windows and Mac).
+        Alkymi is easy to install, simple to use, and has very few dependencies outside of Python's standard library. The code
+        is cross-platform, and allows you to write your pipelines once and deploy to multiple operating systems (tested on
+        Linux, Windows and Mac).
         
         Documentation, including a quickstart guide, is provided [here](https://alkymi.readthedocs.io/en/latest/).
         
         ## Features
         * Easily define complex data pipelines as decorated Python functions
           * This allows you to run linting, type checking, etc. on your data pipelines
         * Return values are automatically cached to disk, regardless of type
@@ -95,23 +95,23 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: xxhash
```

### Comparing `alkymi-0.1.0/setup.py` & `alkymi-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,19 @@
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Environment :: Console",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "Intended Audience :: System Administrators",
         "Topic :: Software Development :: Build Tools",
         "Topic :: Software Development :: Testing",
         "Topic :: Software Development :: Quality Assurance",
@@ -41,17 +41,18 @@
     ],
     keywords=["automation", "pipeline", "validation", "preprocessing", "make", "build", "task"],
     project_urls={
         "Source": "https://github.com/MathiasStokholm/alkymi/",
         "Tracker": "https://github.com/MathiasStokholm/alkymi/issues",
         "Documentation": "https://alkymi.readthedocs.io/en/latest/",
     },
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=[
-        "networkx>=2.0"
+        "networkx>=2.0",
+        "rich>=10.7"
     ],
     extras_require={
         "xxhash": ["xxhash>=2.0.0"]
     },
     package_data={
         "alkymi": ["py.typed"],
     },
```

