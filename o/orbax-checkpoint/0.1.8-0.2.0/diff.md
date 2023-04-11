# Comparing `tmp/orbax-checkpoint-0.1.8.tar.gz` & `tmp/orbax-checkpoint-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbax-checkpoint-0.1.8.tar", last modified: Fri Mar 31 20:52:17 2023, max compression
+gzip compressed data, was "orbax-checkpoint-0.2.0.tar", last modified: Tue Apr 11 01:58:27 2023, max compression
```

## Comparing `orbax-checkpoint-0.1.8.tar` & `orbax-checkpoint-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/LICENSE
--rw-r--r--   0        0        0      137 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/README.md
--rw-r--r--   0        0        0     2564 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/__init__.py
--rw-r--r--   0        0        0     2599 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/abstract_checkpointer.py
--rw-r--r--   0        0        0     2629 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/aggregate_handlers.py
--rw-r--r--   0        0        0     5348 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/array_checkpoint_handler.py
--rw-r--r--   0        0        0     1440 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/async_checkpoint_handler.py
--rw-r--r--   0        0        0     4742 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/async_checkpointer.py
--rw-r--r--   0        0        0     2119 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/checkpoint_handler.py
--rw-r--r--   0        0        0    33132 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/checkpoint_manager.py
--rw-r--r--   0        0        0     9920 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/checkpoint_utils.py
--rw-r--r--   0        0        0     7190 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/checkpoint_utils_test.py
--rw-r--r--   0        0        0     4022 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/checkpointer.py
--rw-r--r--   0        0        0      740 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/conftest.py
--rw-r--r--   0        0        0     1465 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/future.py
--rw-r--r--   0        0        0     2103 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/json_checkpoint_handler.py
--rw-r--r--   0        0        0     1821 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/json_checkpoint_handler_test.py
--rw-r--r--   0        0        0     1872 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/lazy_utils.py
--rw-r--r--   0        0        0     7146 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/msgpack_utils.py
--rw-r--r--   0        0        0    44930 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/orbax_checkpoint.ipynb
--rw-r--r--   0        0        0    18683 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/pytree_checkpoint_handler.py
--rw-r--r--   0        0        0     5234 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/test_utils.py
--rw-r--r--   0        0        0     8086 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/transform_utils.py
--rw-r--r--   0        0        0    13746 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/transform_utils_test.py
--rw-r--r--   0        0        0    19429 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/type_handlers.py
--rw-r--r--   0        0        0    19636 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/utils.py
--rw-r--r--   0        0        0     7071 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/orbax/checkpoint/utils_test.py
--rw-r--r--   0        0        0     1172 2023-03-31 20:51:40.284451 orbax-checkpoint-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 orbax-checkpoint-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/LICENSE
+-rw-r--r--   0        0        0      696 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/README.md
+-rw-r--r--   0        0        0     2564 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2599 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/abstract_checkpointer.py
+-rw-r--r--   0        0        0     2629 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/aggregate_handlers.py
+-rw-r--r--   0        0        0     5348 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/array_checkpoint_handler.py
+-rw-r--r--   0        0        0     1440 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/async_checkpoint_handler.py
+-rw-r--r--   0        0        0     4742 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/async_checkpointer.py
+-rw-r--r--   0        0        0     2119 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_handler.py
+-rw-r--r--   0        0        0    33132 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_manager.py
+-rw-r--r--   0        0        0     9920 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_utils.py
+-rw-r--r--   0        0        0     7190 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_utils_test.py
+-rw-r--r--   0        0        0     4022 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/checkpointer.py
+-rw-r--r--   0        0        0      740 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/conftest.py
+-rw-r--r--   0        0        0     1465 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/future.py
+-rw-r--r--   0        0        0     2103 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/json_checkpoint_handler.py
+-rw-r--r--   0        0        0     1821 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/json_checkpoint_handler_test.py
+-rw-r--r--   0        0        0     2002 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/lazy_utils.py
+-rw-r--r--   0        0        0     7146 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/msgpack_utils.py
+-rw-r--r--   0        0        0    44930 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/orbax_checkpoint.ipynb
+-rw-r--r--   0        0        0    21582 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/pytree_checkpoint_handler.py
+-rw-r--r--   0        0        0     5234 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/test_utils.py
+-rw-r--r--   0        0        0     9406 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/transform_utils.py
+-rw-r--r--   0        0        0    13488 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/transform_utils_test.py
+-rw-r--r--   0        0        0    21621 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/type_handlers.py
+-rw-r--r--   0        0        0    19878 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/utils.py
+-rw-r--r--   0        0        0     7444 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/orbax/checkpoint/utils_test.py
+-rw-r--r--   0        0        0     1172 2023-04-11 01:57:44.959889 orbax-checkpoint-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 orbax-checkpoint-0.2.0/PKG-INFO
```

### Comparing `orbax-checkpoint-0.1.8/LICENSE` & `orbax-checkpoint-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/__init__.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,8 +52,8 @@
 # Convenient shorthand where instead of the following:
 #   `checkpointer = Checkpointer(PyTreeCheckpointer())`
 # we can just use:
 #   `checkpointer = PyTreeCheckpointer()`
 PyTreeCheckpointer = functools.partial(Checkpointer, PyTreeCheckpointHandler())
 
 # A new PyPI release will be pushed everytime `__version__` is increased.
-__version__ = '0.1.8'
+__version__ = '0.2.0'
```

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/abstract_checkpointer.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/abstract_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/aggregate_handlers.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/aggregate_handlers.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/array_checkpoint_handler.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/array_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/async_checkpoint_handler.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/async_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/async_checkpointer.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/async_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/checkpoint_handler.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/checkpoint_manager.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/checkpoint_utils.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/checkpoint_utils_test.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/checkpoint_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/checkpointer.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/conftest.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/conftest.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/future.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/future.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/json_checkpoint_handler.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/json_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/json_checkpoint_handler_test.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/json_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/lazy_utils.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/lazy_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,41 +22,41 @@
 
 class LazyValue:
   """An interface allowing the real object to be fetched asynchronously."""
 
   def __init__(self, get_fn: Callable[[], Any]):
     self._get_fn = get_fn
 
-  async def get_async(self) -> Any:
-    return await self._get_fn()
+  async def get_async(self, *args, **kwargs) -> Any:
+    return await self._get_fn(*args, **kwargs)
 
-  def get(self) -> Any:
-    return asyncio.run(self.get_async())
+  def get(self, *args, **kwargs) -> Any:
+    return asyncio.run(self.get_async(*args, **kwargs))
 
 
 def identity(value):
   """Constructs an async function that returns the given value."""
 
   async def get_fn():
     return value
 
   return get_fn
 
 
-async def maybe_get_async(value):
+async def maybe_get_async(value, *args, **kwargs):
   """Gets the value asynchronously if it is a LazyValue."""
   if isinstance(value, LazyValue):
-    return await value.get_async()
+    return await value.get_async(*args, **kwargs)
   else:
     return await identity(value)()
 
 
-def maybe_get(value):
+def maybe_get(value, *args, **kwargs):
   """Gets the value if it is a LazyValue."""
-  return asyncio.run(maybe_get_async(value))
+  return asyncio.run(maybe_get_async(value, *args, **kwargs))
 
 
 async def maybe_get_tree_async(pytree):
   """Gets tree values asynchronously if they are LazyValue."""
   flat, structure = jax.tree_util.tree_flatten(
       jax.tree_util.tree_map(maybe_get_async, pytree))
   flat = await asyncio.gather(*flat)
```

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/msgpack_utils.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/msgpack_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/orbax_checkpoint.ipynb` & `orbax-checkpoint-0.2.0/orbax/checkpoint/orbax_checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/pytree_checkpoint_handler.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/pytree_checkpoint_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 Implementation of CheckpointHandler interface.
 """
 
 import asyncio
 import dataclasses
 import functools
 import re
-from typing import Any, Callable, List, Optional, Tuple
+from typing import Any, Callable, List, Optional, Tuple, Union
 
 from etils import epath
 import jax
 from jax.experimental.gda_serialization import serialization
 import numpy as np
 from orbax.checkpoint import aggregate_handlers
 from orbax.checkpoint import lazy_utils
@@ -42,14 +42,16 @@
 ArrayRestoreArgs = type_handlers.ArrayRestoreArgs
 SaveArgs = type_handlers.SaveArgs
 ParamInfo = type_handlers.ParamInfo
 TypeHandler = type_handlers.TypeHandler
 AggregateHandler = aggregate_handlers.AggregateHandler
 MsgpackHandler = aggregate_handlers.MsgpackHandler
 TransformFn = Callable[[PyTree, PyTree, PyTree], Tuple[PyTree, PyTree]]
+Transform = transform_utils.Transform
+LazyValue = lazy_utils.LazyValue
 
 _TYPE_METADATA_FILE = 'type_metadata'
 _CHECKPOINT_FILE = 'checkpoint'
 
 
 async def _create_param_save_dir(param_info: ParamInfo, args: SaveArgs):
   # Directory will be unused.
@@ -96,35 +98,41 @@
   )
 
 
 def _get_param_infos_from_structure(directory: epath.Path,
                                     structure: PyTree) -> PyTree:
   """Construct ParamInfos based on a PyTree."""
   names = _get_param_names(structure)
+  is_ocdbt_checkpoint = type_handlers.is_ocdbt_checkpoint(directory)
 
-  def _get_param_info(name, leaf):
+  def _get_param_info(name: str, leaf: Any) -> ParamInfo:
     if utils.leaf_is_placeholder(leaf):
       # Leaf is a param name.
       path = directory / utils.name_from_leaf_placeholder(leaf)
     # The following is kept for backwards compatibility.
     elif isinstance(leaf, ts.Spec):
       tspec = leaf.to_json()  # pytype: disable=attribute-error
       # Skip '.', since we need special regex handling for this char.
       pattern = r'\.' + utils.TMP_DIR_SUFFIX[1:] + r'\d+'
       path = re.sub(pattern, '', tspec['kvstore']['path'])
+    elif utils.is_supported_empty_aggregation_type(leaf):
+      return leaf  # Empty node, ParamInfo should not be returned.
     elif utils.is_supported_aggregation_type(leaf):
       # Value already restored, do not need ts.Spec.
       path = None
     else:
       raise ValueError(f'Unsupported type: {type(leaf)}')
-    return ParamInfo(name=name, path=path, aggregate=(path is None))
+    return ParamInfo(
+        name=name,
+        path=path,
+        aggregate=(path is None),
+        is_ocdbt_checkpoint=is_ocdbt_checkpoint,
+    )
 
-  return jax.tree_util.tree_map(
-      _get_param_info, names, structure, is_leaf=utils.is_empty_or_leaf
-  )
+  return jax.tree_util.tree_map(_get_param_info, names, structure)
 
 
 def _get_tree_for_aggregation(param_infos, save_args, item):
   """Get tree for aggregated checkpoint."""
 
   def _get_leaf_for_aggregation(param_info, arg, value):
     if arg.aggregate:  # Param was aggregated, return value after cast.
@@ -136,66 +144,127 @@
 
   return jax.tree_util.tree_map(
       _get_leaf_for_aggregation, param_infos, save_args, item
   )
 
 
 def _transform_structure(
-    item: PyTree, restored: PyTree, param_infos: PyTree, transforms: PyTree,
-    transforms_default_to_original: bool) -> Tuple[PyTree, PyTree]:
-  """Transforms `restored` and `param_infos` into the structure of `item`.
-
-  After restoring a checkpoint structure (represented by `restored`), we must
-  transform it to match the structure of `item` and fill in any missing values.
-
-  Note that `param_infos` must also be transformed since parameter names and
-  other information is computed based on the PyTree structure. We first create
-  `param_infos` based on the checkpoint structure, otherwise we would not find
-  some parameters after doing transformations and rearranging the tree
-  structure.
+    item: PyTree,
+    restored: PyTree,
+    transforms: Optional[PyTree],
+    transforms_default_to_original: bool,
+) -> PyTree:
+  """Optionally transforms the restored PyTree to the structure of `item`.
 
   Args:
     item: a PyTree representing the result structure ("new tree structure").
-    restored: a PyTree representing the original tree structure.
-    param_infos: A PyTree of ParamInfo having the same structure as `restored`.
+    restored: a PyTree representing the original tree structure. Note: this is a
+      tree of LazyValues.
     transforms: provides instructions on how to transform the input trees. See
       transform_utils.
     transforms_default_to_original: See transform_utils.
 
   Returns:
-    A pair of `item`, `param_infos` which have been transformed from the
-    original trees using `transforms`.
+    A transformed PyTree.
   """
   if item is None:
     if transforms is not None:
       msg = ('If providing `transforms`, must provide `item` matching structure'
              ' of expected result.')
       raise ValueError(msg)
     item = restored
   else:
     if transforms is None:
-      param_infos = utils.deserialize_tree(item, param_infos)
       item = utils.deserialize_tree(item, restored)
     else:
-      if transform_utils.has_value_functions(transforms):
-        raise ValueError(
-            'Found disallowed `value_fn` or `multi_value_fn` in `transforms`.')
+      transforms = _construct_lazy_transform_wrappers(transforms)
       item = transform_utils.apply_transformations(
           restored, transforms, item, transforms_default_to_original)
-      # param_infos must be transformed because the ts.Spec of saved params
-      # may correspond to the original structure rather than the new.
-      param_infos = transform_utils.apply_transformations(
-          param_infos, transforms, item, transforms_default_to_original)
-
-      def _create_param_info_if_already_restored(x):
-        return ParamInfo(aggregate=True) if not isinstance(x, ParamInfo) else x
-
-      param_infos = jax.tree_util.tree_map(
-          _create_param_info_if_already_restored, param_infos)
-  return item, param_infos
+  return item
+
+
+def _construct_lazy_transform_wrappers(transforms: PyTree) -> PyTree:
+  """Constructs wrapper functions for user-provided to handle `LazyValue`.
+
+  User-provided value-based transformation functions are written in terms of
+  real values, not `LazyValue`. However, we want to be able to load all
+  parameters as `LazyValue`, so as to avoid materializing unneeded parameters
+  until necessary. As such, we construct wrapper functions which accept
+  `LazyValue` and materialize the value before providing it to the user-defined
+  function.
+
+  Args:
+    transforms: User-provided tree of Transform objects.
+
+  Returns:
+    A tree of Transform objects which is roughly the same as the input, but
+    where all instances of `value_fn` or `multi_value_fn` are wrapped to accept
+    `LazyValue` as input and return `LazyValue` as output.
+  """
+
+  def _maybe_wrap_transform(transform: Transform):
+    async def _lazy_value_fn(lazy_value: LazyValue, args: RestoreArgs) -> Any:
+      # `lazy_value` is the value over which the function is performed.
+      # `args` is `RestoreArgs`, which is used to materialize the value.
+      value = await lazy_value.get_async(args=args)
+      return transform.value_fn(value)
+
+    async def _lazy_multi_value_fn(
+        transform_key: str, tree: PyTree, args: RestoreArgs
+    ) -> Any:
+      # `original_tree` consists of `LazyValue`s.
+      # `args` is unused, since relevant restoration args come from
+      # multi_value_fn_input_args.
+      del args
+      if not transform.multi_value_fn_input_args:
+        raise ValueError(
+            '`multi_value_fn` was specified, but `multi_value_fn_input_args`'
+            ' were not. The latter must be specified to identify inputs for the'
+            ' function.'
+        )
+
+      async def _materialize_lazy_tree_value(
+          keypath: Tuple[str], lazy_value: LazyValue
+      ) -> Union[Any, LazyValue]:
+        key = '/'.join([str(utils.get_key_name(k)) for k in keypath])
+        for (
+            input_key,
+            restore_args,
+        ) in transform.multi_value_fn_input_args.items():
+          if re.fullmatch(input_key, key):
+            return await lazy_value.get_async(args=restore_args)
+        return lazy_value  # Should not be used, so do not materialize.
+
+      futures, treedef = jax.tree_util.tree_flatten(
+          jax.tree_util.tree_map_with_path(_materialize_lazy_tree_value, tree)
+      )
+      flat_tree = await asyncio.gather(*futures)
+      return transform.multi_value_fn(
+          transform_key, jax.tree_util.tree_unflatten(treedef, flat_tree)
+      )
+
+    def _wrap_as_lazy_value(func, *args, **kwargs):
+      return LazyValue(functools.partial(func, *args, **kwargs))
+
+    # Only needed values are carried over to the wrapped Transform.
+    if transform.value_fn is not None:
+      return Transform(
+          original_key=transform.original_key,
+          value_fn=functools.partial(_wrap_as_lazy_value, _lazy_value_fn),
+      )
+    elif transform.multi_value_fn is not None:
+      return Transform(
+          multi_value_fn=functools.partial(
+              _wrap_as_lazy_value, _lazy_multi_value_fn
+          )
+      )
+    else:
+      return transform
+
+  return jax.tree_util.tree_map(_maybe_wrap_transform, transforms)
 
 
 class PyTreeCheckpointHandler(AsyncCheckpointHandler):
   """A CheckpointHandler implementation for any PyTree structure.
 
   The PyTree is assumed to be a nested dictionary with array values represented
   as array-like objects (see type_handlers for supported objects). If not
@@ -347,47 +416,46 @@
       if commit_futures:  # May be None.
         for future in commit_futures:
           future.result()  # Block on result.
 
     asyncio.run(async_save(directory, item, *args, **kwargs))
     utils.sync_global_devices('PyTreeCheckpointHandler:save')
 
-  async def _maybe_deserialize(self, info: ParamInfo, value: Any,
-                               args: RestoreArgs) -> Any:
+  def _maybe_deserialize(self, param_info: ParamInfo, value: Any) -> LazyValue:
     """Deserializes using handler or returns already restored value.
 
     If the ParamInfo indicates that the parameter was aggregated, then it must
     have already been restored. In this case, we simply perform a cast and
     convert to LazyArray if requested.
 
     Otherwise, we deserialize using an appropriate TypeHandler, converting to
     LazyArray and casting if requested.
 
     Args:
-      info: ParamInfo
+      param_info: ParamInfo
       value: a tree value which may have already been restored. Not relevant if
         info.aggregate is False.
-      args: RestoreArgs for TypeHandler restoration.
 
     Returns:
-      A deserialized parameter.
+      A LazyValue.
     """
-    if not isinstance(args, RestoreArgs):
-      return value
-    if info.aggregate:  # Already restored from AggregateHandler.
-      value = _try_array_cast(value, args.dtype)
-      if args.lazy:
-        value = lazy_utils.LazyValue(lazy_utils.identity(value))
-      return value
 
-    handler = type_handlers.get_type_handler(args.restore_type)
-    value = lazy_utils.LazyValue(lambda: handler.deserialize(info, args))
-    if not args.lazy:
-      value = await value.get_async()
-    return value
+    async def _maybe_cast(val: Any, args: RestoreArgs) -> Any:
+      return _try_array_cast(val, args.dtype)
+
+    async def _deserialize(info: ParamInfo, args: RestoreArgs) -> Any:
+      handler = type_handlers.get_type_handler(args.restore_type)
+      return await handler.deserialize(info, args)
+
+    if param_info.aggregate:  # Already restored from AggregateHandler.
+      get_fn = functools.partial(_maybe_cast, val=value)
+    else:
+      get_fn = functools.partial(_deserialize, info=param_info)
+
+    return LazyValue(get_fn)
 
   def restore(
       self,
       directory: epath.Path,
       item: Optional[PyTree] = None,
       restore_args: Optional[PyTree] = None,
       transforms: Optional[PyTree] = None,
@@ -421,62 +489,83 @@
     Returns:
       A PyTree matching the structure of `item`. If `lazy` restoration is
       enabled, leaves will be returned as `LazyValue`.
 
     Raises:
       FileNotFoundError: `directory` does not exist or is missing required files
       ValueError: `transforms` is provided without `item`.
-      ValueError: `transforms` contains elements with `value_fn` or
-        `multi_value_fn`.
+      ValueError: `transforms` contains elements with `multi_value_fn`.
     """
     if not directory.exists():
       raise FileNotFoundError(
           f'Requested directory for restore does not exist at {directory}')
 
-    restored_structure = self.structure(directory)
-    param_infos = _get_param_infos_from_structure(directory, restored_structure)
+    structure = self.structure(directory)
+    param_infos = _get_param_infos_from_structure(directory, structure)
+
     if transform_fn is not None and transforms is not None:
       raise ValueError('Cannot provide both `transforms` and `transform_fn`.')
-    if transform_fn is None:
-      item, param_infos = _transform_structure(
-          item,
-          restored_structure,
-          param_infos,
-          transforms,
-          transforms_default_to_original,
-      )
-    else:
-      item, param_infos = transform_fn(item, restored_structure, param_infos)
+    if transform_fn is not None:
+      structure, param_infos = transform_fn(item, structure, param_infos)
 
-    if restore_args is None:
-      restore_args = jax.tree_util.tree_map(lambda x: RestoreArgs(), item)
+    concurrent_bytes = self._concurrent_gb * 10**9
+    # Construction must take place here so that it is within the same async
+    # method, to prevent errors resulting from different event loops, and
+    # cannot be created below this level because there must be a single object
+    # for the entire restore call.
+    byte_limiter = serialization._LimitInFlightBytes(concurrent_bytes)  # pylint: disable=protected-access
+    param_infos = jax.tree_util.tree_map(
+        functools.partial(dataclasses.replace, byte_limiter=byte_limiter),
+        param_infos,
+    )
+    lazy_restored_item = jax.tree_util.tree_map(
+        self._maybe_deserialize,
+        param_infos,
+        structure,
+    )
 
-    async def _async_restore(param_infos, item, restore_args):
-      concurrent_bytes = self._concurrent_gb * 10**9
-      # Construction must take place here so that it is within the same async
-      # method, to prevent errors resulting from different event loops, and
-      # cannot be created below this level because there must be a single object
-      # for the entire restore call.
-      byte_limiter = serialization._LimitInFlightBytes(concurrent_bytes)  # pylint: disable=protected-access
-      param_infos = jax.tree_util.tree_map(
-          functools.partial(dataclasses.replace, byte_limiter=byte_limiter),
-          param_infos,
+    if not transform_fn:
+      lazy_restored_item = _transform_structure(
+          item, lazy_restored_item, transforms, transforms_default_to_original
       )
-      future_arrays = jax.tree_util.tree_map(
-          self._maybe_deserialize,
-          param_infos,
-          item,
-          restore_args,
+
+    if restore_args is None:
+      restore_args = jax.tree_util.tree_map(
+          lambda x: RestoreArgs(),
+          item or structure,
       )
-      future_arrays, tree_structure = jax.tree_util.tree_flatten(future_arrays)
-      result = await asyncio.gather(*future_arrays)
-      return jax.tree_util.tree_unflatten(tree_structure, result)
 
-    restored_item = asyncio.run(_async_restore(param_infos, item, restore_args))
+    def _maybe_get_materialization_function(
+        value: Union[LazyValue, Any], args: RestoreArgs
+    ) -> Any:
+      # Depending on the value of args.lazy, we either return a function that
+      # allows materializing the value, or return a function that returns
+      # another LazyValue, after passing in RestoreArgs.
+      if args.lazy:
+        if isinstance(value, LazyValue):
+          async_get_fn = functools.partial(value.get_async, args=args)
+        else:
+          async_get_fn = lazy_utils.identity(value)
+        return lazy_utils.identity(LazyValue(async_get_fn))()
+      else:
+        return lazy_utils.maybe_get_async(value, args=args)
+
+    async def _restore():
+      # Provide RestoreArgs now, since it was previously deferred.
+      flat, item_structure = jax.tree_util.tree_flatten(
+          jax.tree_util.tree_map(
+              _maybe_get_materialization_function,
+              lazy_restored_item,
+              restore_args,
+          )
+      )
+      flat = await asyncio.gather(*flat)
+      return jax.tree_util.tree_unflatten(item_structure, flat)
 
+    restored_item = asyncio.run(_restore())
     utils.sync_global_devices('PyTreeCheckpointHandler:restore')
     return restored_item
 
   def structure(self, directory: epath.Path) -> PyTree:
     """Restores the saved PyTree structure without regard for its leaf values.
 
     Args:
```

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/test_utils.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/test_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/transform_utils.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/transform_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Provides utils for transforming PyTrees from one version to another."""
 
 import dataclasses
 import re
-from typing import Any, Callable, Optional, Tuple, Union
+from typing import Any, Callable, Dict, Optional, Tuple, Union
 
 from absl import logging
-import jax
 from orbax.checkpoint import utils
 
 PyTree = Any
-ValueTransformFunction = Callable[[PyTree], Any]
+ValueFn = Callable[[Any], Any]
+MultiValueFn = Callable[[str, PyTree], Any]
 
 
 @dataclasses.dataclass
 class Transform:
   r"""A representation of a transformation applied to pytree keys/values.
 
   See `apply_transformations` for usage examples. Transform represents an
@@ -58,38 +58,58 @@
   use_fallback: if True, takes the value from the fallback tree. If
     `default_to_original=True` in `apply_transformations`, the fallback tree is
     `new_tree`. If `default_to_original=False` in `apply_transformations`, the
     fallback tree is `original_tree`.
   value_fn: A function accepting a single value and returning a single value.
     The value provided as an argument is the value of the transformation key in
     the original PyTree.
-  multi_value_fn: A function accepting a PyTree and returning any value. The
-    PyTree argument will be the original PyTree, and the function should return
-    the value of the key in the new PyTree.
+  multi_value_fn: A function accepting a string and PyTree and returning any
+    value. The string is the result key associated with the returned value, so
+    the function implementation can know for which key it is supposed to return
+    a value for. The PyTree argument will be the original PyTree, and the
+    function should return the value of the key in the new PyTree.
+  multi_value_fn_input_args: A dict of key name (in the original tree) to
+    required input arguments (typically `RestoreArgs` - see
+    `PyTreeCheckpointHandler`). These arguments are not used directly in
+    `apply_transformations`, but are necessary when applying transformations
+    when restoring from a checkpoint in `PyTreeCheckpointHandler`. These
+    arguments identify "dependencies" in the original tree (the checkpoint)
+    which are needed as inputs by the function, and provides additional
+    information needed for restoration. IMPORTANT: using multi_value_fn during
+    `PyTreeCheckpointHandler.restore` REQUIRES inputs to be identified.
   """
   original_key: Optional[Union[str, Tuple[str]]] = None
   use_fallback: bool = False
-  value_fn: Optional[Callable[[Any], Any]] = None
-  multi_value_fn: Optional[ValueTransformFunction] = None
-
-
-def has_value_functions(pytree: PyTree) -> bool:
-  """Returns True if a PyTree contains any Transform elements with value_fn or multi_value_fn."""
-  result = False
-
-  def elem_has_value_functions(transform: Transform):
-    nonlocal result
-    if transform.value_fn is not None or transform.multi_value_fn is not None:
-      result = True
-
-  jax.tree_util.tree_map(
-      elem_has_value_functions,
-      pytree,
-      is_leaf=lambda x: isinstance(x, Transform))
-  return result
+  value_fn: Optional[ValueFn] = None
+  multi_value_fn: Optional[MultiValueFn] = None
+  multi_value_fn_input_args: Optional[Dict[str, Any]] = None
+
+  def __post_init__(self):
+    if self.original_key is not None:
+      assert not self.use_fallback
+      assert self.multi_value_fn is None
+      assert self.multi_value_fn_input_args is None
+    if self.use_fallback:
+      assert self.original_key is None
+      assert self.value_fn is None
+      assert self.multi_value_fn is None
+      assert self.multi_value_fn_input_args is None
+    if self.value_fn is not None:
+      assert not self.use_fallback
+      assert self.multi_value_fn is None
+      assert self.multi_value_fn_input_args is None
+    if self.multi_value_fn is not None:
+      assert self.original_key is None
+      assert not self.use_fallback
+      assert self.value_fn is None
+    if self.multi_value_fn_input_args is not None:
+      assert self.original_key is None
+      assert not self.use_fallback
+      assert self.value_fn is None
+      assert self.multi_value_fn is not None
 
 
 # TODO(b/233407026) Add additional error checking.
 def apply_transformations(original_tree: PyTree,
                           transformations: PyTree,
                           new_tree: PyTree,
                           default_to_original: Optional[bool] = True) -> PyTree:
@@ -212,15 +232,15 @@
             )
           if transform.value_fn is None:
             value_fn = lambda x: x
           else:
             value_fn = transform.value_fn
           new[key] = value_fn(original[original_key])
         else:
-          new[key] = transform.multi_value_fn(original_tree)
+          new[key] = transform.multi_value_fn(key, original_tree)
     if not transform_found:
       if key in original:
         if default_to_original:
           # carry over directly from original, otherwise use value from new
           new[key] = original[key]
         # if default_to_new, do not carry over key from original
       else:
```

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/transform_utils_test.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/transform_utils_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,21 +71,14 @@
 
   def test_transform_missing_in_original(self):
     original = {'a': 1}
     transforms = {'b': Transform()}
     with self.assertRaises(ValueError):
       apply_transformations(original, transforms, {'b': ...})
 
-  def test_has_value_functions(self):
-    self.assertTrue(
-        transform_utils.has_value_functions(
-            {'a': Transform(original_key='a', value_fn=lambda x: x * 2)}))
-    self.assertFalse(
-        transform_utils.has_value_functions({'a': Transform(original_key='b')}))
-
   def test_rename(self):
     transforms = {
         'a1': Transform(original_key='a'),  # originally named "a"
         'c': {
             'a': Transform(),  # unchanged
         },
         # moved from being inside "c"
@@ -274,28 +267,28 @@
     self.assertDictEqual(
         expected,
         apply_transformations(self.original, transforms,
                               empty_pytree(expected)))
 
   def test_function(self):
     transforms = {
-        'a': Transform(multi_value_fn=lambda kv: kv['a'] * 2 + 20),
+        'a': Transform(multi_value_fn=lambda _, kv: kv['a'] * 2 + 20),
         # dropped b
         'c': {
             # added together two keys, leaving one remaining
-            'a':
-                Transform(multi_value_fn=lambda kv: kv['c']['a'] + kv['c']['e']
-                         ),
+            'a': Transform(
+                multi_value_fn=lambda _, kv: kv['c']['a'] + kv['c']['e']
+            ),
         },
         # many to many transformation: input two keys -> output two new keys
-        'w': Transform(multi_value_fn=lambda kv: kv['a'] + kv['b']),
-        'x': Transform(multi_value_fn=lambda kv: kv['a'] + kv['b'] * 2),
+        'w': Transform(multi_value_fn=lambda _, kv: kv['a'] + kv['b']),
+        'x': Transform(multi_value_fn=lambda _, kv: kv['a'] + kv['b'] * 2),
         # copied a single key into multiple
-        'y': Transform(multi_value_fn=lambda kv: kv['a']),
-        'z': Transform(multi_value_fn=lambda kv: kv['a']),
+        'y': Transform(multi_value_fn=lambda _, kv: kv['a']),
+        'z': Transform(multi_value_fn=lambda _, kv: kv['a']),
     }
     expected = {
         'a': 20,
         'c': {
             'a': 5,
         },
         'w': 1,
@@ -334,22 +327,23 @@
       c: SubTree  # same
       d: float  # new
       e: int  # from a.y
       f: List[int]  # from a.y
 
     transforms = NewTree(
         a1=Transform(original_key='a'),
-        b=Transform(multi_value_fn=lambda t: t.b * 2),
+        b=Transform(multi_value_fn=lambda _, t: t.b * 2),
         c=jax.tree_util.tree_map(lambda _: Transform(), tree.c),
         d=Transform(use_fallback=True),
-        e=Transform(multi_value_fn=lambda t: t.c.y[0]),
+        e=Transform(multi_value_fn=lambda _, t: t.c.y[0]),
         f=[
-            Transform(multi_value_fn=lambda t: t.c.y[1]),
-            Transform(multi_value_fn=lambda t: t.c.y[2])
-        ])
+            Transform(multi_value_fn=lambda _, t: t.c.y[1]),
+            Transform(multi_value_fn=lambda _, t: t.c.y[2]),
+        ],
+    )
     fallback_tree = NewTree(
         a1=utils.EmptyNode(),
         b=utils.EmptyNode(),
         c=SubTree(
             x={'i': utils.EmptyNode(), 'j': utils.EmptyNode()},
             y=[utils.EmptyNode(), utils.EmptyNode(), utils.EmptyNode()],
         ),
```

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/type_handlers.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/type_handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,19 @@
     jax_global_state.client.key_value_set(
         'ocdbt_coordinator', f'{ocdbt_address}:{coordinator_server.port}'
     )
 
   ocdbt_address = jax_global_state.client.blocking_key_value_get(
       'ocdbt_coordinator', _COORDINATOR_SETUP_TIMEOUT_SECS * 1000
   )
-  ts_context = {'ocdbt_coordinator': {'address': ocdbt_address}}
+  ts_context = {
+      'ocdbt_coordinator': {'address': ocdbt_address},
+      # Provide cache pool for B-tree nodes to avoid repeated reads.
+      'cache_pool#ocdbt': {'total_bytes_limit': 100000000},
+  }
   return (
       ts.Context(ts_context, parent=serialization.TS_CONTEXT),
       coordinator_server,
   )
 
 
 @dataclasses.dataclass
@@ -103,19 +107,24 @@
   represents information not provided by a user, and should be computed
   internally.
 
   name: name of the parameter.
   path: A path providing a location where file(s) should be saved. The path is
     assumed to be a directory.
   aggregate: whether the parameter should be / was aggregated.
+  byte_limiter: object to limit the number of bytes that can be read in
+    parallel.
+  is_ocdbt_checkpoint: indicates whether the checkpoint path uses OCDBT format
+    or not. Only used for restoration.
   """
   name: Optional[str] = None
   path: Optional[epath.Path] = None
   aggregate: Optional[bool] = None
   byte_limiter: Optional[serialization._LimitInFlightBytes] = None  # pylint: disable=protected-access
+  is_ocdbt_checkpoint: Optional[bool] = None
 
 
 @dataclasses.dataclass
 class SaveArgs:
   """Extra arguments that can be provided for saving.
 
   aggregate: if true, saves the given parameter in an aggregated tree format
@@ -222,14 +231,34 @@
         'base': tspec,
         'driver': 'cast',
         'dtype': jnp.dtype(args.dtype).name,
     }
   return tspec
 
 
+def _add_base_tspec_ocdbt_options(tspec: Dict[str, Any]) -> Dict[str, Any]:
+  tspec.update({'recheck_cached_data': False, 'recheck_cached_metadata': False})
+  tspec['kvstore'].update({  # Enable read coalescing.
+      'experimental_read_coalescing_threshold_bytes': 1000000,
+      # References the cache specified in ts.Context.
+      'cache_pool': 'cache_pool#ocdbt',
+  })
+  return tspec
+
+
+def _add_write_tspec_ocdbt_options(tspec: Dict[str, Any]) -> Dict[str, Any]:
+  tspec['kvstore']['config'] = {
+      # Store .zarray metadata inline but not large chunks.
+      'max_inline_value_bytes': 1024,
+      # Large value allows a single root node to support faster traversal.
+      'max_decoded_node_bytes': 100000000,
+  }
+  return tspec
+
+
 class NumpyHandler(TypeHandler):
   """Provides an implementation of TypeHandler for replicated numpy arrays."""
 
   def __init__(
       self,
       metadata_key: Optional[str] = None,
       use_ocdbt: bool = False,
@@ -252,41 +281,57 @@
     self._ts_context = ts_context or ts.Context(
         {'file_io_concurrency': {'limit': 128}}
     )
 
   def _get_json_tspec(
       self,
       info: ParamInfo,
-      value: Optional[np.ndarray] = None,
       use_ocdbt: bool = False,
   ) -> Dict[str, Any]:
     """Gets Tensorstore spec in JSON format."""
     if info.path is None:
       raise ValueError('Must construct serialization path.')
     path = os.fspath(info.path)
     tspec: Dict[str, Any] = get_tensorstore_spec(path, ocdbt=use_ocdbt)
     if self._metadata_key is not None:
       tspec['metadata_key'] = self._metadata_key
+    if use_ocdbt:
+      tspec = _add_base_tspec_ocdbt_options(tspec)
+    return tspec
+
+  def _get_json_tspec_write(
+      self, info: ParamInfo, value: Any, use_ocdbt: bool = False
+  ) -> Dict[str, Any]:
+    """Gets Tensorstore spec for writing."""
+    tspec = self._get_json_tspec(info, use_ocdbt=use_ocdbt)
     tspec['metadata'] = {
         'compressor': {
-            'id': 'gzip'
+            'id': 'zstd'
         },
     }
     if value is not None:
       tspec['metadata']['shape'] = value.shape
       tspec['metadata']['chunks'] = value.shape
+    if use_ocdbt:
+      tspec = _add_write_tspec_ocdbt_options(tspec)
     return tspec
 
+  def _get_json_tspec_read(
+      self, info: ParamInfo, use_ocdbt: bool = False
+  ) -> Dict[str, Any]:
+    """Gets Tensorstore spec for reading."""
+    return self._get_json_tspec(info, use_ocdbt=use_ocdbt)
+
   async def serialize(self,
                       value: np.ndarray,
                       info: ParamInfo,
                       args: Optional[SaveArgs] = None) -> List[Future]:
     """Uses Tensorstore to serialize a numpy array."""
     args = args or SaveArgs()
-    tspec = self._get_json_tspec(info, value, use_ocdbt=self._use_ocdbt)
+    tspec = self._get_json_tspec_write(info, value, use_ocdbt=self._use_ocdbt)
     tspec = _get_cast_tspec_serialize(tspec, value, args)
     t = await ts.open(
         ts.Spec(tspec), create=True, open=True, context=self._ts_context
     )
     write_future = t.write(value)
     await write_future.copy
     return [write_future.commit]
@@ -294,16 +339,16 @@
   async def deserialize(self,
                         info: ParamInfo,
                         args: Optional[RestoreArgs] = None) -> np.ndarray:
     """Deserializes the array using Tensorstore."""
     args = args or RestoreArgs()
 
     # Using OCDBT, but existing checkpoint may be stored in old format.
-    use_ocdbt = self._use_ocdbt and is_ocdbt_checkpoint(info.path.parent)
-    tspec = self._get_json_tspec(info, use_ocdbt=use_ocdbt)
+    use_ocdbt = self._use_ocdbt and info.is_ocdbt_checkpoint
+    tspec = self._get_json_tspec_read(info, use_ocdbt=use_ocdbt)
     tspec = _get_cast_tspec_deserialize(tspec, args)
     t = await ts.open(ts.Spec(tspec), open=True, context=self._ts_context)
     return await t.read()
 
 
 class ScalarHandler(NumpyHandler):
   """A wrapper around NumpyHandler to deal with scalar types (int, float, etc.).
@@ -377,35 +422,50 @@
     self._ts_context = ts_context or ts.Context(
         {'file_io_concurrency': {'limit': 128}}
     )
 
   def _get_json_tspec(
       self,
       info: ParamInfo,
-      value: Optional[Any] = None,
       use_ocdbt: bool = False,
   ) -> Dict[str, Any]:
     """Gets Tensorstore spec in JSON format."""
     if info.path is None:
       raise ValueError('Must construct serialization path.')
     path = os.fspath(info.path)
     tspec: Dict[str, Any] = get_tensorstore_spec(path, ocdbt=use_ocdbt)
     if self._metadata_key is not None:
       tspec['metadata_key'] = self._metadata_key
-    if value is not None:
-      tspec['metadata'] = serialization._get_metadata(value)  # pylint: disable=protected-access
-      del tspec['metadata']['dtype']
+    if use_ocdbt:
+      tspec = _add_base_tspec_ocdbt_options(tspec)
     return tspec
 
+  def _get_json_tspec_write(
+      self, info: ParamInfo, value: Any, use_ocdbt: bool = False
+  ) -> Dict[str, Any]:
+    """Gets Tensorstore spec for writing."""
+    tspec = self._get_json_tspec(info, use_ocdbt=use_ocdbt)
+    tspec['metadata'] = serialization._get_metadata(value)  # pylint: disable=protected-access
+    del tspec['metadata']['dtype']
+    if use_ocdbt:
+      tspec = _add_write_tspec_ocdbt_options(tspec)
+    return tspec
+
+  def _get_json_tspec_read(
+      self, info: ParamInfo, use_ocdbt: bool = False
+  ) -> Dict[str, Any]:
+    """Gets Tensorstore spec for reading."""
+    return self._get_json_tspec(info, use_ocdbt=use_ocdbt)
+
   async def serialize(
       self, value: jax.Array, info: ParamInfo, args: Optional[SaveArgs] = None
   ) -> List[Future]:
     """See superclass documentation."""
     args = args or SaveArgs()
-    tspec = self._get_json_tspec(info, value, use_ocdbt=self._use_ocdbt)
+    tspec = self._get_json_tspec_write(info, value, use_ocdbt=self._use_ocdbt)
     tspec = _get_cast_tspec_serialize(tspec, value, args)
     commit_futures = []
     await serialization.async_serialize(
         value, tspec, commit_future=commit_futures, context=self._ts_context
     )
     return commit_futures
 
@@ -434,16 +494,16 @@
           ' and `mesh_axes` OR `sharding`.'
       )
     if args.sharding is None:
       sharding = jax.sharding.NamedSharding(args.mesh, args.mesh_axes)
     else:
       sharding = args.sharding
     # Using OCDBT, but existing checkpoint may be stored in old format.
-    use_ocdbt = self._use_ocdbt and is_ocdbt_checkpoint(info.path.parent)
-    tspec = self._get_json_tspec(info, use_ocdbt=use_ocdbt)
+    use_ocdbt = self._use_ocdbt and info.is_ocdbt_checkpoint
+    tspec = self._get_json_tspec_read(info, use_ocdbt=use_ocdbt)
     tspec = _get_cast_tspec_deserialize(tspec, args)
     return await serialization.async_deserialize(
         sharding,
         tspec,
         global_shape=args.global_shape,
         byte_limiter=info.byte_limiter,
         context=self._ts_context,
```

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/utils.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,26 +238,28 @@
 
 
 def deserialize_tree(
     target: PyTree, serialized: PyTree, keep_empty_nodes: bool = False
 ) -> PyTree:
   """Deserializes a PyTree to the same structure as `target`."""
 
-  def fn(keypath, _):
+  def _reconstruct_from_keypath(keypath, _):
     result = serialized
     for key in keypath:
       key_name = get_key_name(key)
       # Special case to support Pax.
       if not isinstance(result, list) and key_name not in result:
         key_name = str(key_name)
       result = result[key_name]
     return result
 
   return jax.tree_util.tree_map_with_path(
-      fn, target, is_leaf=is_empty_or_leaf if keep_empty_nodes else None
+      _reconstruct_from_keypath,
+      target,
+      is_leaf=is_empty_or_leaf if keep_empty_nodes else None,
   )
 
 
 def from_flat_dict(
     tree: PyTree, flat_dict: PyTree, sep: Optional[str] = None
 ) -> PyTree:
   """Reconstructs the original tree object from a flattened dictionary.
@@ -301,20 +303,25 @@
     return placeholder.replace(_AGGREGATED_PREFIX, '', 1)
   elif placeholder.startswith(_PLACEHOLDER_PREFIX):
     return placeholder.replace(_PLACEHOLDER_PREFIX, '', 1)
   else:
     raise ValueError('Found placeholder beginning with unexpected prefix.')
 
 
+def is_supported_empty_aggregation_type(value: Any) -> bool:
+  """Determines if the *empty* value is supported for aggregation."""
+  return isinstance(value, (dict, list, type(None))) and not value
+
+
 def is_supported_aggregation_type(value: Any) -> bool:
   """Determines if the value is supported for aggregation."""
   return isinstance(
       value,
-      (str, int, float, np.number, np.ndarray, jnp.ndarray, bytes, type(None)),
-  ) or (isinstance(value, (dict, list)) and not value)
+      (str, int, float, np.number, np.ndarray, jnp.ndarray, bytes),
+  ) or is_supported_empty_aggregation_type(value)
 
 
 def pytree_structure(directory: epath.PathLike) -> PyTree:
   """Reconstruct state dict from saved model format in `directory`."""
   directory = epath.Path(directory)
 
   def add_nested_key(subtree, nested_key, key_name):
```

### Comparing `orbax-checkpoint-0.1.8/orbax/checkpoint/utils_test.py` & `orbax-checkpoint-0.2.0/orbax/checkpoint/utils_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,14 +172,30 @@
         'a': 1,
         'b': {'a': 'b', 'c': 'd'},
         'c': [optax.EmptyState(), optax.EmptyState()],
         'd': [{}, {'x': 'y'}, None],
     }
     self.assertDictEqual(expected, serialized)
 
+  def test_serialize_nested_class(self):
+    @flax.struct.dataclass
+    class Foo:
+      a: int
+
+    nested = {
+        'x': Foo(a=1),
+        'y': {'z': Foo(a=2)},
+    }
+    serialized = utils.serialize_tree(nested, keep_empty_nodes=True)
+    expected = {
+        'x': dict(a=1),
+        'y': {'z': dict(a=2)},
+    }
+    self.assertDictEqual(expected, serialized)
+
   def test_checkpoint_steps_paths_nonexistent_directory_fails(self):
     with self.assertRaisesRegex(ValueError, 'does not exist'):
       utils.checkpoint_steps_paths('/non/existent/dir')
 
   def test_checkpoint_steps_paths_returns_finalized_paths(self):
     digit_only_path = epath.Path(self.directory / '2')
     digit_only_path.mkdir()
@@ -195,15 +211,15 @@
 
   def test_checkpoint_steps_returns_steps_of_finalized_paths(self):
     epath.Path(self.directory / '2').mkdir()
     epath.Path(self.directory / 'checkpoint_01').mkdir()
     epath.Path(self.directory / 'checkpoint').mkdir()
     epath.Path(self.directory / '1000.orbax-checkpoint-tmp-1010101').mkdir()
 
-    self.assertEqual(
+    self.assertSameElements(
+        [1, 2],
         utils.checkpoint_steps(self.directory),
-        [2, 1],
     )
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `orbax-checkpoint-0.1.8/pyproject.toml` & `orbax-checkpoint-0.2.0/pyproject.toml`

 * *Files identical despite different names*

