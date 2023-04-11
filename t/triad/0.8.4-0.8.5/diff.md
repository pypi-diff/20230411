# Comparing `tmp/triad-0.8.4.tar.gz` & `tmp/triad-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triad-0.8.4.tar", last modified: Sun Mar 19 07:22:26 2023, max compression
+gzip compressed data, was "triad-0.8.5.tar", last modified: Tue Apr 11 07:37:31 2023, max compression
```

## Comparing `triad-0.8.4.tar` & `triad-0.8.5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:22:26.778637 triad-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-19 07:21:44.000000 triad-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-03-19 07:22:26.778637 triad-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-03-19 07:21:44.000000 triad-0.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-19 07:22:26.778637 triad-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-19 07:21:44.000000 triad-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:22:26.770637 triad-0.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 07:21:44.000000 triad-0.8.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:22:26.770637 triad-0.8.4/tests/collections/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-19 07:21:44.000000 triad-0.8.4/tests/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-03-19 07:21:44.000000 triad-0.8.4/tests/collections/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-03-19 07:21:44.000000 triad-0.8.4/tests/collections/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-03-19 07:21:44.000000 triad-0.8.4/tests/collections/test_function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-03-19 07:21:44.000000 triad-0.8.4/tests/collections/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:22:26.774637 triad-0.8.4/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/convert_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:22:26.774637 triad-0.8.4/tests/utils/dispatcher_examples/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/dispatcher_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/dispatcher_examples/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/dispatcher_examples/invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/test_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/test_class_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/test_pandas_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/test_pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/test_pyarrow_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-19 07:21:44.000000 triad-0.8.4/tests/utils/test_threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:22:26.774637 triad-0.8.4/triad/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-19 07:21:44.000000 triad-0.8.4/triad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:22:26.778637 triad-0.8.4/triad/collections/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-19 07:21:44.000000 triad-0.8.4/triad/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-03-19 07:21:44.000000 triad-0.8.4/triad/collections/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-03-19 07:21:44.000000 triad-0.8.4/triad/collections/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-03-19 07:21:44.000000 triad-0.8.4/triad/collections/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-03-19 07:21:44.000000 triad-0.8.4/triad/collections/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-19 07:21:44.000000 triad-0.8.4/triad/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-19 07:21:44.000000 triad-0.8.4/triad/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:22:26.778637 triad-0.8.4/triad/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-19 07:21:44.000000 triad-0.8.4/triad/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-19 07:21:44.000000 triad-0.8.4/triad/utils/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-03-19 07:21:44.000000 triad-0.8.4/triad/utils/class_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-03-19 07:21:44.000000 triad-0.8.4/triad/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-03-19 07:21:44.000000 triad-0.8.4/triad/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-19 07:21:44.000000 triad-0.8.4/triad/utils/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-19 07:21:44.000000 triad-0.8.4/triad/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-03-19 07:21:44.000000 triad-0.8.4/triad/utils/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-19 07:21:44.000000 triad-0.8.4/triad/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-03-19 07:21:44.000000 triad-0.8.4/triad/utils/pandas_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    24206 2023-03-19 07:21:44.000000 triad-0.8.4/triad/utils/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-03-19 07:21:44.000000 triad-0.8.4/triad/utils/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-03-19 07:21:44.000000 triad-0.8.4/triad/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-19 07:21:44.000000 triad-0.8.4/triad/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-03-19 07:21:44.000000 triad-0.8.4/triad/utils/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:22:26.774637 triad-0.8.4/triad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-03-19 07:22:26.000000 triad-0.8.4/triad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-19 07:22:26.000000 triad-0.8.4/triad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 07:22:26.000000 triad-0.8.4/triad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-19 07:22:26.000000 triad-0.8.4/triad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-19 07:22:26.000000 triad-0.8.4/triad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:22:26.778637 triad-0.8.4/triad_version/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-19 07:21:44.000000 triad-0.8.4/triad_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.611298 triad-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 07:36:52.000000 triad-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-04-11 07:37:31.611298 triad-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-11 07:36:52.000000 triad-0.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-11 07:37:31.611298 triad-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-11 07:36:52.000000 triad-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.603298 triad-0.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:36:52.000000 triad-0.8.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.603298 triad-0.8.5/tests/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 07:36:52.000000 triad-0.8.5/tests/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-11 07:36:52.000000 triad-0.8.5/tests/collections/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-04-11 07:36:52.000000 triad-0.8.5/tests/collections/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-11 07:36:52.000000 triad-0.8.5/tests/collections/test_function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-04-11 07:36:52.000000 triad-0.8.5/tests/collections/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.607298 triad-0.8.5/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/convert_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.607298 triad-0.8.5/tests/utils/dispatcher_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/dispatcher_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/dispatcher_examples/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/dispatcher_examples/invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_class_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_pandas_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_pyarrow_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.607298 triad-0.8.5/triad/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-11 07:36:52.000000 triad-0.8.5/triad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.611298 triad-0.8.5/triad/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-11 07:36:52.000000 triad-0.8.5/triad/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-04-11 07:36:52.000000 triad-0.8.5/triad/collections/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-11 07:36:52.000000 triad-0.8.5/triad/collections/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-04-11 07:36:52.000000 triad-0.8.5/triad/collections/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-04-11 07:36:52.000000 triad-0.8.5/triad/collections/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 07:36:52.000000 triad-0.8.5/triad/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-11 07:36:52.000000 triad-0.8.5/triad/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.611298 triad-0.8.5/triad/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/class_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/pandas_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24206 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.611298 triad-0.8.5/triad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-04-11 07:37:31.000000 triad-0.8.5/triad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-11 07:37:31.000000 triad-0.8.5/triad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:37:31.000000 triad-0.8.5/triad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 07:37:31.000000 triad-0.8.5/triad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 07:37:31.000000 triad-0.8.5/triad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.611298 triad-0.8.5/triad_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 07:36:52.000000 triad-0.8.5/triad_version/__init__.py
```

### Comparing `triad-0.8.4/LICENSE` & `triad-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/PKG-INFO` & `triad-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triad
-Version: 0.8.4
+Version: 0.8.5
 Summary: A collection of python utils for Fugue projects
 Home-page: http://github.com/fugue-project/triad
 Author: Han Wang
 Author-email: goodwanghan@gmail.com
 License: Apache-2.0
 Description: # Triad
         
@@ -24,14 +24,19 @@
         ```bash
         pip install triad
         ```
         
         
         ## Release History
         
+        ### 0.8.5
+        
+        * Ensure pandas 2.0 compatibility
+        * Improve `to_schema` in `PandasUtils`
+        
         ### 0.8.4
         
         * Moved `FunctionWrapper` from Fugue into Triad
         * Improved groupby apply efficiency for pandas utils
         
         ### 0.8.3
```

### Comparing `triad-0.8.4/README.md` & `triad-0.8.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 ```bash
 pip install triad
 ```
 
 
 ## Release History
 
+### 0.8.5
+
+* Ensure pandas 2.0 compatibility
+* Improve `to_schema` in `PandasUtils`
+
 ### 0.8.4
 
 * Moved `FunctionWrapper` from Fugue into Triad
 * Improved groupby apply efficiency for pandas utils
 
 ### 0.8.3
```

### Comparing `triad-0.8.4/setup.py` & `triad-0.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/collections/test_dict.py` & `triad-0.8.5/tests/collections/test_dict.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/collections/test_fs.py` & `triad-0.8.5/tests/collections/test_fs.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/collections/test_function_wrapper.py` & `triad-0.8.5/tests/collections/test_function_wrapper.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/collections/test_schema.py` & `triad-0.8.5/tests/collections/test_schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/utils/test_assertion.py` & `triad-0.8.5/tests/utils/test_assertion.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/utils/test_class_extension.py` & `triad-0.8.5/tests/utils/test_class_extension.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/utils/test_convert.py` & `triad-0.8.5/tests/utils/test_convert.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/utils/test_dispatcher.py` & `triad-0.8.5/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/utils/test_hash.py` & `triad-0.8.5/tests/utils/test_hash.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/utils/test_iter.py` & `triad-0.8.5/tests/utils/test_iter.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/utils/test_pandas_like.py` & `triad-0.8.5/tests/utils/test_pandas_like.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,15 @@
     DF(
         [["a", dt, 1], ["b", dt, 2], ["b", dt, 2], ["b", None, 1]],
         "a:str,b:date,ct:int",
         True,
     ).assert_eq(res)
 
 
-def test_is_compatile_index():
+def test_is_compatible_index():
     df = DF([["a", 1], [None, 2]], "a:str,b:int", True)
     assert PD_UTILS.is_compatile_index(df.native)
     tdf = df.native.sort_values("a")
     assert PD_UTILS.is_compatile_index(tdf)
     tdf = tdf.set_index("a")
     assert not PD_UTILS.is_compatile_index(tdf)
```

### Comparing `triad-0.8.4/tests/utils/test_pyarrow.py` & `triad-0.8.5/tests/utils/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/utils/test_pyarrow_convert.py` & `triad-0.8.5/tests/utils/test_pyarrow_convert.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/utils/test_rename.py` & `triad-0.8.5/tests/utils/test_rename.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/utils/test_schema.py` & `triad-0.8.5/tests/utils/test_schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/utils/test_string.py` & `triad-0.8.5/tests/utils/test_string.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/tests/utils/test_threading.py` & `triad-0.8.5/tests/utils/test_threading.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/collections/dict.py` & `triad-0.8.5/triad/collections/dict.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/collections/fs.py` & `triad-0.8.5/triad/collections/fs.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/collections/function_wrapper.py` & `triad-0.8.5/triad/collections/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/collections/schema.py` & `triad-0.8.5/triad/collections/schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/utils/assertion.py` & `triad-0.8.5/triad/utils/assertion.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/utils/class_extension.py` & `triad-0.8.5/triad/utils/class_extension.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/utils/convert.py` & `triad-0.8.5/triad/utils/convert.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/utils/dispatcher.py` & `triad-0.8.5/triad/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/utils/entry_points.py` & `triad-0.8.5/triad/utils/entry_points.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/utils/hash.py` & `triad-0.8.5/triad/utils/hash.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/utils/iter.py` & `triad-0.8.5/triad/utils/iter.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/utils/json.py` & `triad-0.8.5/triad/utils/json.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/utils/pandas_like.py` & `triad-0.8.5/triad/utils/pandas_like.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from datetime import datetime
 from typing import Any, Callable, Dict, Generic, Iterable, List, Optional, TypeVar
 
 import numpy as np
 import pandas as pd
+import pyarrow as pa
+
 from triad.utils.assertion import assert_or_throw
 from triad.utils.pyarrow import (
     TRIAD_DEFAULT_TIMESTAMP_UNIT,
     apply_schema,
+    to_pa_datatype,
     to_pandas_dtype,
     to_single_pandas_dtype,
 )
 
-import pyarrow as pa
-
 T = TypeVar("T", bound=Any)
 _DEFAULT_JOIN_KEYS: List[str] = []
 _DEFAULT_DATETIME = datetime(2000, 1, 1)
 
 
 class PandasLikeUtils(Generic[T]):
     """A collection of utils for general pandas like dataframes"""
@@ -113,15 +114,15 @@
                 for i in range(df.shape[1]):
                     tp = df.dtypes[i]
                     if tp == np.dtype("object") or pd.api.types.is_string_dtype(tp):
                         t = pa.string()
                     elif isinstance(tp, pd.DatetimeTZDtype):
                         t = pa.timestamp(tp.unit, str(tp.tz))
                     else:
-                        t = pa.from_numpy_dtype(tp)
+                        t = to_pa_datatype(tp)
                     yield pa.field(df.columns[i], t)
 
         fields: List[pa.Field] = []
         for field in get_fields():
             if pa.types.is_timestamp(field.type):
                 fields.append(
                     pa.field(
@@ -254,16 +255,16 @@
         :param df: pandas like dataframe
         :raises ValueError: if not compatible
         """
         if df.index.name is not None:
             raise ValueError("pandas like datafame index can't have name")
         if self.is_compatile_index(df):
             return
-        if self.empty(df):
-            return
+        if self.empty(df):  # for pandas < 2
+            return  # pragma: no cover
         raise ValueError(
             f"pandas like datafame must have default index, but got {type(df.index)}"
         )
 
 
 class PandasUtils(PandasLikeUtils[pd.DataFrame]):
     """A collection of pandas utils"""
```

### Comparing `triad-0.8.4/triad/utils/pyarrow.py` & `triad-0.8.5/triad/utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/utils/rename.py` & `triad-0.8.5/triad/utils/rename.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/utils/schema.py` & `triad-0.8.5/triad/utils/schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/utils/string.py` & `triad-0.8.5/triad/utils/string.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad/utils/threading.py` & `triad-0.8.5/triad/utils/threading.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.4/triad.egg-info/PKG-INFO` & `triad-0.8.5/triad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triad
-Version: 0.8.4
+Version: 0.8.5
 Summary: A collection of python utils for Fugue projects
 Home-page: http://github.com/fugue-project/triad
 Author: Han Wang
 Author-email: goodwanghan@gmail.com
 License: Apache-2.0
 Description: # Triad
         
@@ -24,14 +24,19 @@
         ```bash
         pip install triad
         ```
         
         
         ## Release History
         
+        ### 0.8.5
+        
+        * Ensure pandas 2.0 compatibility
+        * Improve `to_schema` in `PandasUtils`
+        
         ### 0.8.4
         
         * Moved `FunctionWrapper` from Fugue into Triad
         * Improved groupby apply efficiency for pandas utils
         
         ### 0.8.3
```

### Comparing `triad-0.8.4/triad.egg-info/SOURCES.txt` & `triad-0.8.5/triad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

