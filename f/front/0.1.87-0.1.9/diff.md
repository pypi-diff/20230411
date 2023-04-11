# Comparing `tmp/front-0.1.87.tar.gz` & `tmp/front-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "front-0.1.87.tar", last modified: Tue Apr 11 00:30:08 2023, max compression
+gzip compressed data, was "front-0.1.9.tar", last modified: Fri Feb 18 02:01:54 2022, max compression
```

## Comparing `front-0.1.87.tar` & `front-0.1.9.tar`

### file list

```diff
@@ -1,59 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:30:08.582816 front-0.1.87/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 00:29:41.000000 front-0.1.87/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-04-11 00:30:08.582816 front-0.1.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-04-11 00:29:41.000000 front-0.1.87/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:30:08.578816 front-0.1.87/front/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-11 00:29:41.000000 front-0.1.87/front/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-11 00:29:41.000000 front-0.1.87/front/app_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-11 00:29:41.000000 front-0.1.87/front/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    36429 2023-04-11 00:29:41.000000 front-0.1.87/front/crude.py
--rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-04-11 00:29:41.000000 front-0.1.87/front/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-11 00:29:41.000000 front-0.1.87/front/data_binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:30:08.582816 front-0.1.87/front/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-11 00:29:41.000000 front-0.1.87/front/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-04-11 00:29:41.000000 front-0.1.87/front/elements/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-11 00:29:41.000000 front-0.1.87/front/elements/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-11 00:29:41.000000 front-0.1.87/front/elements/tree_maker_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:30:08.582816 front-0.1.87/front/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:29:41.000000 front-0.1.87/front/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-11 00:29:41.000000 front-0.1.87/front/examples/data_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-11 00:29:41.000000 front-0.1.87/front/examples/experimentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-11 00:29:41.000000 front-0.1.87/front/examples/issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-11 00:29:41.000000 front-0.1.87/front/examples/kaggle_front.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-11 00:29:41.000000 front-0.1.87/front/examples/pos_key_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-11 00:29:41.000000 front-0.1.87/front/examples/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-11 00:29:41.000000 front-0.1.87/front/examples/simple_ml_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-11 00:29:41.000000 front-0.1.87/front/examples/tw_data_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-11 00:29:41.000000 front-0.1.87/front/examples/wordle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-04-11 00:29:41.000000 front-0.1.87/front/py2pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:30:08.582816 front-0.1.87/front/scrap/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 00:29:41.000000 front-0.1.87/front/scrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-11 00:29:41.000000 front-0.1.87/front/scrap/binder_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-11 00:29:41.000000 front-0.1.87/front/scrap/binder_proposal_no_desc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-11 00:29:41.000000 front-0.1.87/front/scrap/state_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-11 00:29:41.000000 front-0.1.87/front/scrap/tw_simple_new_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-11 00:29:41.000000 front-0.1.87/front/spec_maker_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-04-11 00:29:41.000000 front-0.1.87/front/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:30:08.582816 front-0.1.87/front/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:29:41.000000 front-0.1.87/front/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-11 00:29:41.000000 front-0.1.87/front/tests/app_identity_pydantic_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-11 00:29:41.000000 front-0.1.87/front/tests/app_identity_write_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-11 00:29:41.000000 front-0.1.87/front/tests/test_combos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-11 00:29:41.000000 front-0.1.87/front/tests/test_crude.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-11 00:29:41.000000 front-0.1.87/front/tests/test_crudify_based_on_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-11 00:29:41.000000 front-0.1.87/front/tests/test_identity_write_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-11 00:29:41.000000 front-0.1.87/front/tests/test_py2pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-04-11 00:29:41.000000 front-0.1.87/front/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-11 00:29:41.000000 front-0.1.87/front/tests/test_use_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-11 00:29:41.000000 front-0.1.87/front/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-11 00:29:41.000000 front-0.1.87/front/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-04-11 00:29:41.000000 front-0.1.87/front/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:30:08.578816 front-0.1.87/front.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-04-11 00:30:08.000000 front-0.1.87/front.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 00:30:08.000000 front-0.1.87/front.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 00:30:08.000000 front-0.1.87/front.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 00:30:08.000000 front-0.1.87/front.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 00:30:08.000000 front-0.1.87/front.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 00:30:08.000000 front-0.1.87/front.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-11 00:30:08.582816 front-0.1.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 00:29:41.000000 front-0.1.87/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:54.493507 front-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-02-18 02:01:29.000000 front-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1157 2022-02-18 02:01:54.493507 front-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      766 2022-02-18 02:01:29.000000 front-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:54.493507 front-0.1.9/front/
+-rw-r--r--   0 runner    (1001) docker     (121)     1222 2022-02-18 02:01:53.000000 front-0.1.9/front/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-02-18 02:01:53.000000 front-0.1.9/front/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16485 2022-02-18 02:01:53.000000 front-0.1.9/front/crude.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:54.493507 front-0.1.9/front/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:29.000000 front-0.1.9/front/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-02-18 02:01:53.000000 front-0.1.9/front/examples/data_binding.py
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-02-18 02:01:53.000000 front-0.1.9/front/examples/experimentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-02-18 02:01:53.000000 front-0.1.9/front/examples/issues.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3762 2022-02-18 02:01:53.000000 front-0.1.9/front/examples/kaggle_front.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-02-18 02:01:53.000000 front-0.1.9/front/examples/pos_key_args.py
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-02-18 02:01:53.000000 front-0.1.9/front/examples/simple.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-02-18 02:01:53.000000 front-0.1.9/front/examples/tw_data_binding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-02-18 02:01:53.000000 front-0.1.9/front/py2pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:54.493507 front-0.1.9/front/scrap/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-02-18 02:01:29.000000 front-0.1.9/front/scrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:54.493507 front-0.1.9/front/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:29.000000 front-0.1.9/front/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-18 02:01:29.000000 front-0.1.9/front/tests/app_identity_pydantic_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2022-02-18 02:01:29.000000 front-0.1.9/front/tests/app_identity_write_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-02-18 02:01:53.000000 front-0.1.9/front/tests/test_combos.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-02-18 02:01:53.000000 front-0.1.9/front/tests/test_crude.py
+-rw-r--r--   0 runner    (1001) docker     (121)      390 2022-02-18 02:01:29.000000 front-0.1.9/front/tests/test_identity_write_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-02-18 02:01:29.000000 front-0.1.9/front/tests/test_py2pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4149 2022-02-18 02:01:53.000000 front-0.1.9/front/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 02:01:54.493507 front-0.1.9/front.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1157 2022-02-18 02:01:54.000000 front-0.1.9/front.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2022-02-18 02:01:54.000000 front-0.1.9/front.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-18 02:01:54.000000 front-0.1.9/front.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-18 02:01:54.000000 front-0.1.9/front.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-18 02:01:54.000000 front-0.1.9/front.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-02-18 02:01:54.000000 front-0.1.9/front.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2022-02-18 02:01:54.493507 front-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-02-18 02:01:29.000000 front-0.1.9/setup.py
```

### Comparing `front-0.1.87/LICENSE` & `front-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `front-0.1.87/front/__init__.py` & `front-0.1.9/front/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,26 +31,7 @@
     from streamlitfront import session_state
     from streamlitfront import base
     from streamlitfront import util
     from streamlitfront import *
     from warnings import warn
 
     warn('Moved to seperate streamlitfront package', DeprecationWarning)
-
-from .app_maker import AppMaker
-from .spec_maker_base import (
-    SpecMakerBase,
-    APP_KEY,
-    OBJ_KEY,
-    RENDERING_KEY,
-    NAME_KEY,
-)
-from .elements import (
-    ElementTreeMaker,
-    ELEMENT_KEY,
-    FrontComponentBase,
-    FrontContainerBase,
-    FrontElementBase,
-    DEFAULT_INPUT_KEY,
-)
-from .crude import Crudifier, prepare_for_crude_dispatch
-from .data_binding import BoundData, Binder
```

### Comparing `front-0.1.87/front/base.py` & `front-0.1.9/front/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     # for prepare_for_crude_dispatch
     param_to_mall_map=(),
     mall=None,
     output_store=None,
     save_name_param: str = 'save_name',
     include_stores_attribute: bool = False,
     # for setting defaults
-    defaults: Optional[Mapping] = None,
+    defaults: Optional[Mapping] = None
 ):
     param_to_mall_map = keys_to_values_if_non_mapping_iterable(param_to_mall_map)
 
     from i2 import Sig
 
     wrapped_func = func  # to seed the following sequence of wrapping
 
@@ -42,15 +42,15 @@
         include_stores_attribute=include_stores_attribute,
     )
 
     # enum wrap
     wrapped_func = inject_enum_annotations(
         wrapped_func,
         extract_enum_value=True,
-        **{param: mall[mall_key] for param, mall_key in param_to_mall_map.items()},
+        **{param: mall[mall_key] for param, mall_key in param_to_mall_map.items()}
     )
 
     # insert defaults
     if defaults:
         # get only keys that are in wrapped_func signature as well as defaults
         wrapped_sig = Sig(wrapped_func)
         _defaults = wrapped_sig.kwargs_from_args_and_kwargs(
```

### Comparing `front-0.1.87/front/examples/experimentation.py` & `front-0.1.9/front/examples/experimentation.py`

 * *Files identical despite different names*

### Comparing `front-0.1.87/front/examples/issues.py` & `front-0.1.9/front/examples/issues.py`

 * *Files identical despite different names*

### Comparing `front-0.1.87/front/examples/kaggle_front.py` & `front-0.1.9/front/examples/kaggle_front.py`

 * *Files identical despite different names*

### Comparing `front-0.1.87/front/examples/pos_key_args.py` & `front-0.1.9/front/examples/pos_key_args.py`

 * *Files identical despite different names*

### Comparing `front-0.1.87/front/examples/simple.py` & `front-0.1.9/front/examples/simple.py`

 * *Files identical despite different names*

### Comparing `front-0.1.87/front/examples/tw_data_binding.py` & `front-0.1.9/front/examples/tw_data_binding.py`

 * *Files identical despite different names*

### Comparing `front-0.1.87/front/tests/test_combos.py` & `front-0.1.9/front/tests/test_combos.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         foo,
         param_to_mall_map={'a': 'a_store'},
         mall=mall,
         output_store=mall['saves'],
         include_stores_attribute=True,
     )
 
-    assert str(Sig(bar)) == "(a: Literal['one', 'two'], b, save_name: str = '')"
+    assert str(Sig(bar)) == "(a: str, b, save_name: str = '')"
     assert bar('two', 'mice', save_name='save_here') == 'micemice'
 
     assert bar.store_for_param == {'a': {'one': 1, 'two': 2}}
     assert bar.output_store == {'save_here': 'micemice'}
 
     # ------------ With prepare_for_dispatch (prepare_for_crude_dispatch + enum) ----------
```

### Comparing `front-0.1.87/front/tests/test_crude.py` & `front-0.1.9/front/tests/test_crude.py`

 * *Files identical despite different names*

### Comparing `front-0.1.87/front/tests/test_py2pydantic.py` & `front-0.1.9/front/tests/test_py2pydantic.py`

 * *Files identical despite different names*

### Comparing `front-0.1.87/front.egg-info/SOURCES.txt` & `front-0.1.9/front.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,31 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 front/__init__.py
-front/app_maker.py
 front/base.py
 front/crude.py
-front/dag.py
-front/data_binding.py
 front/py2pydantic.py
-front/spec_maker_base.py
-front/state.py
-front/types.py
 front/util.py
 front.egg-info/PKG-INFO
 front.egg-info/SOURCES.txt
 front.egg-info/dependency_links.txt
 front.egg-info/not-zip-safe
 front.egg-info/requires.txt
 front.egg-info/top_level.txt
-front/elements/__init__.py
-front/elements/elements.py
-front/elements/implementation.py
-front/elements/tree_maker_base.py
 front/examples/__init__.py
 front/examples/data_binding.py
 front/examples/experimentation.py
 front/examples/issues.py
 front/examples/kaggle_front.py
 front/examples/pos_key_args.py
 front/examples/simple.py
-front/examples/simple_ml_1.py
 front/examples/tw_data_binding.py
-front/examples/wordle.py
 front/scrap/__init__.py
-front/scrap/binder_proposal.py
-front/scrap/binder_proposal_no_desc.py
-front/scrap/state_proposal.py
-front/scrap/tw_simple_new_arch.py
 front/tests/__init__.py
 front/tests/app_identity_pydantic_output.py
 front/tests/app_identity_write_output.py
 front/tests/test_combos.py
 front/tests/test_crude.py
-front/tests/test_crudify_based_on_names.py
 front/tests/test_identity_write_output.py
-front/tests/test_py2pydantic.py
-front/tests/test_state.py
-front/tests/test_use_case.py
-front/tests/util.py
+front/tests/test_py2pydantic.py
```

### Comparing `front-0.1.87/setup.cfg` & `front-0.1.9/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = front
-version = 0.1.87
+version = 0.1.9
 url = https://github.com/i2mint/front
 platforms = any
 description_file = README.md
 root_url = https://github.com/i2mint/
 license = apache-2.0
 author = OtoSense
 description = Getting from python objects to UIs exposing them
@@ -14,17 +14,15 @@
 display_name = front
 
 [options]
 packages = find:
 include_package_data = True
 zip_safe = False
 install_requires = 
-	dill
-	dol
 	i2
-	meshed
 	pydantic
+	dill
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

