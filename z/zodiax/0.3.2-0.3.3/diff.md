# Comparing `tmp/zodiax-0.3.2.tar.gz` & `tmp/zodiax-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodiax-0.3.2.tar", last modified: Tue Apr 11 08:02:37 2023, max compression
+gzip compressed data, was "zodiax-0.3.3.tar", last modified: Tue Apr 11 08:49:33 2023, max compression
```

## Comparing `zodiax-0.3.2.tar` & `zodiax-0.3.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:02:37.631184 zodiax-0.3.2/
--rw-r--r--   0 louis      (501) staff       (20)       70 2022-11-14 06:22:13.000000 zodiax-0.3.2/.gitignore
--rw-r--r--   0 louis      (501) staff       (20)     1523 2022-11-14 06:12:01.000000 zodiax-0.3.2/LICENSE
--rw-r--r--   0 louis      (501) staff       (20)       49 2022-11-14 11:44:43.000000 zodiax-0.3.2/MANIFEST.ini
--rw-r--r--   0 louis      (501) staff       (20)      488 2023-04-11 08:02:37.631045 zodiax-0.3.2/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)     4292 2023-03-28 01:43:37.000000 zodiax-0.3.2/README.md
--rw-r--r--   0 louis      (501) staff       (20)     2992 2023-03-20 01:49:16.000000 zodiax-0.3.2/mkdocs.yml
--rw-r--r--   0 louis      (501) staff       (20)       55 2023-03-09 09:55:10.000000 zodiax-0.3.2/requirements.txt
--rw-r--r--   0 louis      (501) staff       (20)       38 2023-04-11 08:02:37.631225 zodiax-0.3.2/setup.cfg
--rw-r--r--   0 louis      (501) staff       (20)     1508 2023-04-11 07:58:40.000000 zodiax-0.3.2/setup.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:02:37.628709 zodiax-0.3.2/tests/
--rw-r--r--   0 louis      (501) staff       (20)     6936 2023-03-22 06:53:45.000000 zodiax-0.3.2/tests/test_base.py
--rw-r--r--   0 louis      (501) staff       (20)      824 2023-03-20 01:40:07.000000 zodiax-0.3.2/tests/test_equinox.py
--rw-r--r--   0 louis      (501) staff       (20)      700 2023-03-20 01:40:07.000000 zodiax-0.3.2/tests/test_optimisation.py
--rw-r--r--   0 louis      (501) staff       (20)      668 2023-03-20 01:40:07.000000 zodiax-0.3.2/tests/test_serialisation.py
--rw-r--r--   0 louis      (501) staff       (20)      366 2023-03-20 01:40:07.000000 zodiax-0.3.2/tests/test_tree.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:02:37.629487 zodiax-0.3.2/zodiax/
--rw-r--r--   0 louis      (501) staff       (20)      428 2023-04-11 08:00:25.000000 zodiax-0.3.2/zodiax/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)    21739 2023-03-22 06:51:07.000000 zodiax-0.3.2/zodiax/base.py
--rw-r--r--   0 louis      (501) staff       (20)     5112 2023-03-20 01:40:07.000000 zodiax-0.3.2/zodiax/equinox.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:02:37.630834 zodiax-0.3.2/zodiax/experimental/
--rw-r--r--   0 louis      (501) staff       (20)      238 2023-03-22 01:43:50.000000 zodiax-0.3.2/zodiax/experimental/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)     1290 2023-03-22 01:46:09.000000 zodiax-0.3.2/zodiax/experimental/jit.py
--rw-r--r--   0 louis      (501) staff       (20)    17276 2023-03-22 02:19:04.000000 zodiax-0.3.2/zodiax/experimental/serialisation.py
--rw-r--r--   0 louis      (501) staff       (20)     2101 2023-03-23 00:20:31.000000 zodiax-0.3.2/zodiax/optimisation.py
--rw-r--r--   0 louis      (501) staff       (20)     2104 2023-03-20 01:40:07.000000 zodiax-0.3.2/zodiax/tree.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:02:37.630132 zodiax-0.3.2/zodiax.egg-info/
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:02:37.630447 zodiax-0.3.2/zodiax.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 louis      (501) staff       (20)      391 2022-11-14 11:49:15.000000 zodiax-0.3.2/zodiax.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-14 11:49:15.000000 zodiax-0.3.2/zodiax.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 louis      (501) staff       (20)      488 2023-04-11 08:02:37.000000 zodiax-0.3.2/zodiax.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      645 2023-04-11 08:02:37.000000 zodiax-0.3.2/zodiax.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2023-04-11 08:02:37.000000 zodiax-0.3.2/zodiax.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)       49 2023-04-11 08:02:37.000000 zodiax-0.3.2/zodiax.egg-info/requires.txt
--rw-r--r--   0 louis      (501) staff       (20)       27 2023-04-11 08:02:37.000000 zodiax-0.3.2/zodiax.egg-info/top_level.txt
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:49:33.563444 zodiax-0.3.3/
+-rw-r--r--   0 louis      (501) staff       (20)       70 2022-11-14 06:22:13.000000 zodiax-0.3.3/.gitignore
+-rw-r--r--   0 louis      (501) staff       (20)     1523 2022-11-14 06:12:01.000000 zodiax-0.3.3/LICENSE
+-rw-r--r--   0 louis      (501) staff       (20)       49 2022-11-14 11:44:43.000000 zodiax-0.3.3/MANIFEST.ini
+-rw-r--r--   0 louis      (501) staff       (20)      488 2023-04-11 08:49:33.563284 zodiax-0.3.3/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)     4291 2023-04-11 08:47:45.000000 zodiax-0.3.3/README.md
+-rw-r--r--   0 louis      (501) staff       (20)     2992 2023-03-20 01:49:16.000000 zodiax-0.3.3/mkdocs.yml
+-rw-r--r--   0 louis      (501) staff       (20)       55 2023-03-09 09:55:10.000000 zodiax-0.3.3/requirements.txt
+-rw-r--r--   0 louis      (501) staff       (20)       38 2023-04-11 08:49:33.563488 zodiax-0.3.3/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)     1508 2023-04-11 07:58:40.000000 zodiax-0.3.3/setup.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:49:33.560862 zodiax-0.3.3/tests/
+-rw-r--r--   0 louis      (501) staff       (20)     6936 2023-03-22 06:53:45.000000 zodiax-0.3.3/tests/test_base.py
+-rw-r--r--   0 louis      (501) staff       (20)      824 2023-03-20 01:40:07.000000 zodiax-0.3.3/tests/test_equinox.py
+-rw-r--r--   0 louis      (501) staff       (20)      700 2023-03-20 01:40:07.000000 zodiax-0.3.3/tests/test_optimisation.py
+-rw-r--r--   0 louis      (501) staff       (20)      668 2023-03-20 01:40:07.000000 zodiax-0.3.3/tests/test_serialisation.py
+-rw-r--r--   0 louis      (501) staff       (20)      366 2023-03-20 01:40:07.000000 zodiax-0.3.3/tests/test_tree.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:49:33.561758 zodiax-0.3.3/zodiax/
+-rw-r--r--   0 louis      (501) staff       (20)      428 2023-04-11 08:47:45.000000 zodiax-0.3.3/zodiax/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)    21745 2023-04-11 08:47:45.000000 zodiax-0.3.3/zodiax/base.py
+-rw-r--r--   0 louis      (501) staff       (20)     5112 2023-03-20 01:40:07.000000 zodiax-0.3.3/zodiax/equinox.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:49:33.563060 zodiax-0.3.3/zodiax/experimental/
+-rw-r--r--   0 louis      (501) staff       (20)      238 2023-03-22 01:43:50.000000 zodiax-0.3.3/zodiax/experimental/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)     1296 2023-04-11 08:47:45.000000 zodiax-0.3.3/zodiax/experimental/jit.py
+-rw-r--r--   0 louis      (501) staff       (20)    17318 2023-04-11 08:47:45.000000 zodiax-0.3.3/zodiax/experimental/serialisation.py
+-rw-r--r--   0 louis      (501) staff       (20)     2101 2023-03-23 00:20:31.000000 zodiax-0.3.3/zodiax/optimisation.py
+-rw-r--r--   0 louis      (501) staff       (20)     2104 2023-03-20 01:40:07.000000 zodiax-0.3.3/zodiax/tree.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:49:33.562423 zodiax-0.3.3/zodiax.egg-info/
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:49:33.562689 zodiax-0.3.3/zodiax.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 louis      (501) staff       (20)      391 2022-11-14 11:49:15.000000 zodiax-0.3.3/zodiax.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-14 11:49:15.000000 zodiax-0.3.3/zodiax.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 louis      (501) staff       (20)      488 2023-04-11 08:49:33.000000 zodiax-0.3.3/zodiax.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      645 2023-04-11 08:49:33.000000 zodiax-0.3.3/zodiax.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2023-04-11 08:49:33.000000 zodiax-0.3.3/zodiax.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)       49 2023-04-11 08:49:33.000000 zodiax-0.3.3/zodiax.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       27 2023-04-11 08:49:33.000000 zodiax-0.3.3/zodiax.egg-info/top_level.txt
```

### Comparing `zodiax-0.3.2/LICENSE` & `zodiax-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.2/README.md` & `zodiax-0.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 Doccumentataion: [louisdesdoigts.github.io/zodiax/](https://louisdesdoigts.github.io/zodiax/)
 
 Installation: ```pip install zodiax```
 
 Contributors: [Louis Desdoigts](https://github.com/LouisDesdoigts)
 
-Requires: Python 3.10+, Jax 0.4.3+
+Requires: Python 3.8+, Jax 0.4.3+
 
 ---
 
 ### Quickstart
 
 Create a regular class that inherits from `zodiax.Base`
```

### Comparing `zodiax-0.3.2/mkdocs.yml` & `zodiax-0.3.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.2/setup.py` & `zodiax-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.2/tests/test_base.py` & `zodiax-0.3.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.2/tests/test_equinox.py` & `zodiax-0.3.3/tests/test_equinox.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.2/tests/test_optimisation.py` & `zodiax-0.3.3/tests/test_optimisation.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.2/tests/test_serialisation.py` & `zodiax-0.3.3/tests/test_serialisation.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.2/zodiax/base.py` & `zodiax-0.3.3/zodiax/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 import zodiax
 import jax.numpy as np
 from equinox import tree_at, Module
-from typing import Union, Any, Callable
+from typing import Union, Any, Callable, List
 from jaxtyping import Array, PyTree
 
 
 __all__ = ["Base"]
 
-PathLike = Union[list[str], str]
+PathLike = Union[List[str], str]
 
 
 def _get_leaf(pytree : PyTree, path : PathLike) -> Any:
     """
     A hidden class desinged to recurse down a pytree following the path,
     returning the leaf at the end of the path.
 
@@ -212,23 +212,23 @@
         new_paths = _format(paths)
         values = _get_leaves(self, new_paths)
         return values[0] if len(new_paths) == 1 else values
 
 
     def set(self   : PyTree,
             paths  : PathLike,
-            values : Union[list[Any], Any]) -> PyTree:
+            values : Union[List[Any], Any]) -> PyTree:
         """
         Set the leaves specified by paths with values.
 
         Parameters
         ----------
         paths : PathLike
             A path or list of paths or list of nested paths.
-        values : Union[list[Any], Any]
+        values : Union[List[Any], Any]
             The list of values to set at the leaves specified by paths.
 
         Returns
         -------
         pytree : PyTree
             The pytree with leaves specified by paths updated with values.
         """
@@ -243,23 +243,23 @@
         leaves_fn = lambda pytree: _get_leaves(pytree, new_paths)
         return tree_at(leaves_fn, self, new_values,
                       is_leaf = lambda leaf: leaf is None)
 
 
     def add(self   : PyTree,
             paths  : PathLike,
-            values : Union[list[Any], Any]) -> PyTree:
+            values : Union[List[Any], Any]) -> PyTree:
         """
         Add to the the leaves specified by paths with values.
 
         Parameters
         ----------
         paths : PathLike
             A path or list of paths or list of nested paths.
-        values : Union[list[Any], Any]
+        values : Union[List[Any], Any]
             The list of values to add to the leaves specified by paths.
 
         Returns
         -------
         pytree : PyTree
             The pytree with values added to leaves specified by paths.
         """
@@ -271,23 +271,23 @@
         leaves_fn = lambda pytree: _get_leaves(pytree, new_paths)
         return tree_at(leaves_fn, self, new_values,
                       is_leaf = lambda leaf: leaf is None)
 
 
     def multiply(self   : PyTree,
                  paths  : PathLike,
-                 values : Union[list[Any], Any]) -> PyTree:
+                 values : Union[List[Any], Any]) -> PyTree:
         """
         Multiplies the the leaves specified by paths with values.
 
         Parameters
         ----------
         paths : PathLike
             A path or list of paths or list of nested paths.
-        values : Union[list[Any], Any]
+        values : Union[List[Any], Any]
             The list of values to multiply the leaves specified by paths.
 
         Returns
         -------
         pytree : PyTree
             The pytree with values multiplied by leaves specified by paths.
         """
@@ -299,23 +299,23 @@
         leaves_fn = lambda pytree: _get_leaves(pytree, new_paths)
         return tree_at(leaves_fn, self, new_values,
                       is_leaf = lambda leaf: leaf is None)
 
 
     def divide(self   : PyTree,
                paths  : PathLike,
-               values : Union[list[Any], Any]) -> PyTree:
+               values : Union[List[Any], Any]) -> PyTree:
         """
         Divides the the leaves specified by paths with values.
 
         Parameters
         ----------
         paths : PathLike
             A path or list of paths or list of nested paths.
-        values : Union[list[Any], Any]
+        values : Union[List[Any], Any]
             The list of values to divide the leaves specified by paths.
 
         Returns
         -------
         pytree : PyTree
             The pytree with values divided by leaves specified by paths.
         """
@@ -327,23 +327,23 @@
         leaves_fn = lambda pytree: _get_leaves(pytree, new_paths)
         return tree_at(leaves_fn, self, new_values,
                       is_leaf = lambda leaf: leaf is None)
 
 
     def power(self   : PyTree,
               paths  : PathLike,
-              values : Union[list[Any], Any]) -> PyTree:
+              values : Union[List[Any], Any]) -> PyTree:
         """
         Raises th leaves specified by paths to the power of values.
 
         Parameters
         ----------
         paths : PathLike
             A path or list of paths or list of nested paths.
-        values : Union[list[Any], Any]
+        values : Union[List[Any], Any]
             The list of values to take the leaves specified by paths to the
             power of.
 
         Returns
         -------
         pytree : PyTree
             The pytree with the leaves specified by paths raised to the power
@@ -357,24 +357,24 @@
         leaves_fn = lambda pytree: _get_leaves(pytree, new_paths)
         return tree_at(leaves_fn, self, new_values,
                       is_leaf = lambda leaf: leaf is None)
 
 
     def min(self   : PyTree,
             paths  : PathLike,
-            values : Union[list[Any], Any]) -> PyTree:
+            values : Union[List[Any], Any]) -> PyTree:
         """
         Updates the leaves specified by paths with the minimum value of the
         leaves and values.
 
         Parameters
         ----------
         paths : PathLike
             A path or list of paths or list of nested paths.
-        values : Union[list[Any], Any]
+        values : Union[List[Any], Any]
             The list of values to take the minimum of and the leaf.
 
         Returns
         -------
         pytree : PyTree
             The pytree with the leaves specified by paths updated with the
             minimum value of the leaf and values.
@@ -387,24 +387,24 @@
         leaves_fn = lambda pytree: _get_leaves(pytree, new_paths)
         return tree_at(leaves_fn, self, new_values,
                       is_leaf = lambda leaf: leaf is None)
 
 
     def max(self   : PyTree,
             paths  : PathLike,
-            values : Union[list[Any], Any]) -> PyTree:
+            values : Union[List[Any], Any]) -> PyTree:
         """
         Updates the leaves specified by paths with the maximum value of the
         leaves and values.
 
         Parameters
         ----------
         paths : PathLike
             A path or list of paths or list of nested paths.
-        values : Union[list[Any], Any]
+        values : Union[List[Any], Any]
             The list of values to take the maximum of and the leaf.
 
         Returns
         -------
         pytree : PyTree
             The pytree with the leaves specified by paths updated with the
             maximum value of the leaf and values.
@@ -417,23 +417,23 @@
         leaves_fn = lambda pytree: _get_leaves(pytree, new_paths)
         return tree_at(leaves_fn, self, new_values,
                       is_leaf = lambda leaf: leaf is None)
 
 
     def apply(self  : PyTree,
               paths : PathLike,
-              fns   : Union[list[Callable], Callable]) -> PyTree:
+              fns   : Union[List[Callable], Callable]) -> PyTree:
         """
         Applies the functions within fns the leaves specified by paths.
 
         Parameters
         ----------
         paths : PathLike
             A path or list of paths or list of nested paths.
-        fns : Union[list[Callable], Callable]
+        fns : Union[List[Callable], Callable]
             The list of functions to apply to the leaves.
 
         Returns
         -------
         pytree : PyTree
             The pytree with fns applied to the leaves specified by paths.
         """
@@ -445,27 +445,27 @@
         leaves_fn = lambda pytree: _get_leaves(pytree, new_paths)
         return tree_at(leaves_fn, self, new_values,
                       is_leaf = lambda leaf: leaf is None)
 
 
     def apply_args(self  : PyTree,
                    paths : PathLike,
-                   fns   : Union[list[Callable], Callable],
-                   args  : Union[list[Any], Any]) -> PyTree:
+                   fns   : Union[List[Callable], Callable],
+                   args  : Union[List[Any], Any]) -> PyTree:
         """
         Applies the functions within fns the leaves specified by paths, while
         also passing in args to the function.
 
         Parameters
         ----------
         paths : PathLike
             A path or list of paths or list of nested paths.
-        fns : Union[list[Callable], Callable]
+        fns : Union[List[Callable], Callable]
             The list of functions to apply to the leaves.
-        args : Union[list[Any], Any]
+        args : Union[List[Any], Any]
             The tupe or list of tuples of extra arguments to pass into fns.
 
         Returns
         -------
         pytree : PyTree
             The pytree with fns applied to the leaves specified by paths with
             the extra args passed in.
@@ -479,15 +479,15 @@
         leaves_fn = lambda pytree: _get_leaves(pytree, new_paths)
         return tree_at(leaves_fn, self, new_values,
                       is_leaf = lambda leaf: leaf is None)
 
 
     def set_and_call(self    : PyTree,
                      paths   : PathLike,
-                     values  : Union[list[Any], Any],
+                     values  : Union[List[Any], Any],
                      call_fn : str,
                      **kwargs) -> Any:
         """
         Updates the leaves speficied by paths with values, and then calls the
         function specified by the string call_fn, returning whatever is
         returnd by the call_fn. Any extra positional arguments or key-word
         arguments are passed through to the modelling function.
@@ -496,30 +496,30 @@
         Please go through the 'PyTree interface' tutorial to see how this
         is used.
 
         Parameters
         ----------
         paths : PathLike
             A path or list of paths or list of nested paths.
-        values : Union[list[Any], Any]
+        values : Union[List[Any], Any]
             The list of values to set at the leaves specified by paths.
         call_fn : str
             A string specifying which model function to call.
 
         Returns
         -------
             : Any
             Whatever object is returned by call_fn.
         """
         return getattr(self.set(paths, values), call_fn)(**kwargs)
 
 
     def apply_and_call(self     : PyTree,
                        paths    : PathLike,
-                       fns      : Union[list[Callable], Callable],
+                       fns      : Union[List[Callable], Callable],
                        call_fn  : str,
                        **kwargs) -> object:
         """
         Applies the functions specified by fns to the leaves speficied by
         paths, and then calls the function specified by the string call_fn,
         returning whatever is returnd by the call_fn. Any extra positional
         arguments or keyword arguments are passed through to the modelling
@@ -527,15 +527,15 @@
 
         Parameters
         ----------
         call_fn : str
             A string specifying which model function to call.
         paths : PathLike
             A path or list of paths or list of nested paths.
-        fns : Union[list[Callable], Callable]
+        fns : Union[List[Callable], Callable]
             The list of functions to apply to the leaves.
 
         Returns
         -------
             : Any
             Whatever object is returned by call_fn.
         """
```

### Comparing `zodiax-0.3.2/zodiax/equinox.py` & `zodiax-0.3.3/zodiax/equinox.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.2/zodiax/experimental/jit.py` & `zodiax-0.3.3/zodiax/experimental/jit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import zodiax
 import jax.numpy as np
 from jax.tree_util import tree_map
 from equinox import partition, combine
-from typing import Union
+from typing import Union, List
 
 
 __all__ = ['get_jit_model']
 
 
 def _float_from_0d(leaf):
     """
@@ -14,26 +14,26 @@
     """
     if isinstance(leaf, np.ndarray):
         return float(leaf) if leaf.ndim == 0 else leaf
     else:
         return leaf
 
 
-def get_jit_model(model : zodiax.base.Base, params : Union[list[str], str]):
+def get_jit_model(model : zodiax.base.Base, params : Union[List[str], str]):
     """
     Replaces all scalar array leaves with python floats. This allows for those
     leaves to be marked as static under jit. The arguments in the params input
     are not cast to python types to prevent the model from being recompiled
     every time the arguments change under an optimisation loop.
 
     Parameters
     ----------
     model : zodiax.Base
         The model to be jitted.
-    params : Union[list[str], str]
+    params : Union[List[str], str]
         The arguments to be optimised under the jit compilation.
     
     Returns
     -------
     model : zodiax.Base
         The model with scalar arrays leaves replaced with python floats.
     """
```

### Comparing `zodiax-0.3.2/zodiax/experimental/serialisation.py` & `zodiax-0.3.3/zodiax/experimental/serialisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 import sys
 import pickle
 import zodiax
 from typing import Any
 from jax import Array
-from jax.typing import ArrayLike
+# from jax.typing import ArrayLike
 import numpy as onp
 import jax.numpy as jnp
 from equinox import tree_serialise_leaves, tree_deserialise_leaves
 from pathlib import Path
 
 
 __all__ = ['serialise', 'deserialise', 'load_structure', 'build_structure']
@@ -50,15 +50,16 @@
     Returns
     -------
     is_container : bool
         True if the object is a container, False if it is a leaf.
     """
     t = '  ' * depth
     conatiner_types = (list, tuple, dict, zodiax.Base)
-    leaf_types = (ArrayLike, bool, complex, float, int, str)
+    leaf_types = (Array, onp.ndarray, onp.bool_, onp.number, bool, int, float,
+        complex, str)
 
     # Contianer node
     if isinstance(obj, conatiner_types):
         if _print: print(f"{t}Node '{self_key}' of type: {type(obj)}")
         return True
 
     # NOTE: Checking None types in a tuple of types has some off behaviour.
```

### Comparing `zodiax-0.3.2/zodiax/optimisation.py` & `zodiax-0.3.3/zodiax/optimisation.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.2/zodiax/tree.py` & `zodiax-0.3.3/zodiax/tree.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.2/zodiax.egg-info/SOURCES.txt` & `zodiax-0.3.3/zodiax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

