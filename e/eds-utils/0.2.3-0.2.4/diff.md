# Comparing `tmp/eds-utils-0.2.3.tar.gz` & `tmp/eds-utils-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eds-utils-0.2.3.tar", last modified: Wed Feb 22 04:49:24 2023, max compression
+gzip compressed data, was "eds-utils-0.2.4.tar", last modified: Tue Apr 11 03:09:21 2023, max compression
```

## Comparing `eds-utils-0.2.3.tar` & `eds-utils-0.2.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:49:24.602218 eds-utils-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-22 04:49:11.000000 eds-utils-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-02-22 04:49:24.602218 eds-utils-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-02-22 04:49:11.000000 eds-utils-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:49:24.594217 eds-utils-0.2.3/eds_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:49:24.598217 eds-utils-0.2.3/eds_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/core/eds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:49:24.598217 eds-utils-0.2.3/eds_utils/core/file_io/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/core/file_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/core/file_io/read_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/core/file_io/write_canopennode.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/core/file_io/write_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/core/file_io/write_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/core/file_io/write_rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/core/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds2dcf.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds2md.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds2rst.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_autofix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:49:24.598217 eds-utils-0.2.3/eds_utils/eds_editor/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:49:24.598217 eds-utils-0.2.3/eds_utils/eds_editor/dialogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/dialogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/dialogs/add_object_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/dialogs/copy_object_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/dialogs/errors_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/dialogs/open_tmp_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/eds_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:49:24.602218 eds-utils-0.2.3/eds_utils/eds_editor/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/pages/_object_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/pages/device_commissioning_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/pages/general_info_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/pages/object_dictionary_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/pages/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/pages/pdo_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_editor/window.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-22 04:49:11.000000 eds-utils-0.2.3/eds_utils/eds_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:49:24.598217 eds-utils-0.2.3/eds_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-02-22 04:49:24.000000 eds-utils-0.2.3/eds_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-02-22 04:49:24.000000 eds-utils-0.2.3/eds_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 04:49:24.000000 eds-utils-0.2.3/eds_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-22 04:49:24.000000 eds-utils-0.2.3/eds_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 04:49:24.000000 eds-utils-0.2.3/eds_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 04:49:24.000000 eds-utils-0.2.3/eds_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-22 04:49:11.000000 eds-utils-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-02-22 04:49:24.602218 eds-utils-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:49:24.602218 eds-utils-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 04:49:11.000000 eds-utils-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-02-22 04:49:11.000000 eds-utils-0.2.3/tests/test_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-02-22 04:49:11.000000 eds-utils-0.2.3/tests/test_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.879304 eds-utils-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 03:09:12.000000 eds-utils-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-11 03:09:21.879304 eds-utils-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-11 03:09:12.000000 eds-utils-0.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.875304 eds-utils-0.2.4/eds_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.875304 eds-utils-0.2.4/eds_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/eds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.875304 eds-utils-0.2.4/eds_utils/core/file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/file_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22994 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/file_io/read_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/file_io/write_canopennode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/file_io/write_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/file_io/write_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/file_io/write_rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds2dcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds2md.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds2rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_autofix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.879304 eds-utils-0.2.4/eds_utils/eds_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.879304 eds-utils-0.2.4/eds_utils/eds_editor/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/dialogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/dialogs/add_object_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/dialogs/copy_object_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/dialogs/errors_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/dialogs/open_tmp_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/eds_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.879304 eds-utils-0.2.4/eds_utils/eds_editor/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/pages/_object_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/pages/device_commissioning_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/pages/general_info_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/pages/object_dictionary_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/pages/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/pages/pdo_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.875304 eds-utils-0.2.4/eds_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-11 03:09:21.000000 eds-utils-0.2.4/eds_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-11 03:09:21.000000 eds-utils-0.2.4/eds_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:09:21.000000 eds-utils-0.2.4/eds_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-11 03:09:21.000000 eds-utils-0.2.4/eds_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 03:09:21.000000 eds-utils-0.2.4/eds_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 03:09:21.000000 eds-utils-0.2.4/eds_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 03:09:12.000000 eds-utils-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-11 03:09:21.879304 eds-utils-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.879304 eds-utils-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:12.000000 eds-utils-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-11 03:09:12.000000 eds-utils-0.2.4/tests/test_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-11 03:09:12.000000 eds-utils-0.2.4/tests/test_objects.py
```

### Comparing `eds-utils-0.2.3/LICENSE` & `eds-utils-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/PKG-INFO` & `eds-utils-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eds-utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: Utilities for editing CANopen EDS/DCF files
 Home-page: https://github.com/oresat/eds-utils
 Author: psas
 Author-email: oresat@pdx.edu
 Maintainer: psas
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: UI
 License-File: LICENSE
 
 =========
 eds-utils
 =========
 
 A collection of EDS / DCF utilities.
```

### Comparing `eds-utils-0.2.3/README.rst` & `eds-utils-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/__main__.py` & `eds-utils-0.2.4/eds_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/core/__init__.py` & `eds-utils-0.2.4/eds_utils/core/__init__.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/core/eds.py` & `eds-utils-0.2.4/eds_utils/core/eds.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,16 @@
         if subindex is None:
             if index in self._data:
                 raise EDSError(f'index 0x{index:X} already exist')
             self._data[index] = item
         elif index not in self._data:
             raise EDSError(f'cannot insert subindex 0x{subindex:X} for index 0x{index:X}, as that '
                            'index does not exist')
+        elif isinstance(self._data[index], Variable):
+            raise EDSError('cannot insert a subindex into a Variable')
         elif subindex in self._data[index].subindexes:
             raise EDSError(f'subindex 0x{subindex:X} already exist for index 0x{index:X}')
         elif not isinstance(item, Variable):
             raise EDSError('cannot insert non-Variable into subindex')
         else:
             self._data[index][subindex] = item
 
@@ -339,15 +341,15 @@
     def storage_locations(self) -> List[str]:
         '''The list of storage locations for CANopenNode support.'''
 
         return self._storage_locations
 
     def add_storage_location(self, storage_location: str):
 
-        if storage_location not in self._storage_locations:
+        if storage_location not in self._storage_locations and storage_location != '':
             self._storage_locations.append(storage_location)
 
     def copy_object(self, index: int, subindex: int, new_index: int, new_subindex: int,
                     move: bool = False):
         '''Move or copy an object in the OD'''
 
         if index not in self.indexes:
```

### Comparing `eds-utils-0.2.3/eds_utils/core/file_io/read_eds.py` & `eds-utils-0.2.4/eds_utils/core/file_io/read_eds.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
             elif object_type == ObjectType.ARRAY:
                 obj, err = _read_array(header, raw, comments)
             elif object_type == ObjectType.RECORD:
                 obj, err = _read_record(header, raw, comments)
 
             sl = obj.storage_location
-            if sl not in eds.storage_locations:
+            if sl not in eds.storage_locations and sl != '':
                 eds.add_storage_location(sl)
 
             errors += err
 
             index = int(header[1:5], 16)
 
             eds[index] = obj
@@ -125,15 +125,15 @@
                 var.data_type = DataType.UNSIGNED8
 
             # set subindex 0's storage_location
             sl = eds[index].storage_location
             if eds[index][0].storage_location == '':
                 eds[index][0].storage_location = sl
 
-            if sl not in eds.storage_locations:
+            if sl not in eds.storage_locations and sl != '':
                 eds.add_storage_location(sl)
 
             index = int(header[1:5], 16)
             subindex = int(header[8:-1], 16)
 
             if eds[index].storage_location != var.storage_location:
                 errors.append(f'{_LEVEL}: StorageLocation of [{index:X}] and {header} did not '
```

### Comparing `eds-utils-0.2.3/eds_utils/core/file_io/write_canopennode.py` & `eds-utils-0.2.4/eds_utils/core/file_io/write_canopennode.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/core/file_io/write_eds.py` & `eds-utils-0.2.4/eds_utils/core/file_io/write_eds.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/core/file_io/write_md.py` & `eds-utils-0.2.4/eds_utils/core/file_io/write_md.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/core/file_io/write_rst.py` & `eds-utils-0.2.4/eds_utils/core/file_io/write_rst.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/core/objects.py` & `eds-utils-0.2.4/eds_utils/core/objects.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds2c.py` & `eds-utils-0.2.4/eds_utils/eds2c.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds2dcf.py` & `eds-utils-0.2.4/eds_utils/eds2dcf.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds2md.py` & `eds-utils-0.2.4/eds_utils/eds2md.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds2rst.py` & `eds-utils-0.2.4/eds_utils/eds2rst.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds_autofix.py` & `eds-utils-0.2.4/eds_utils/eds_autofix.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds_editor/app.py` & `eds-utils-0.2.4/eds_utils/eds_editor/app.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py` & `eds-utils-0.2.4/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds_editor/dialogs/add_object_dialog.py` & `eds-utils-0.2.4/eds_utils/eds_editor/dialogs/add_object_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds_editor/dialogs/copy_object_dialog.py` & `eds-utils-0.2.4/eds_utils/eds_editor/dialogs/copy_object_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds_editor/dialogs/errors_dialog.py` & `eds-utils-0.2.4/eds_utils/eds_editor/dialogs/errors_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds_editor/dialogs/open_tmp_dialog.py` & `eds-utils-0.2.4/eds_utils/eds_editor/dialogs/open_tmp_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds_editor/eds_notebook.py` & `eds-utils-0.2.4/eds_utils/eds_editor/eds_notebook.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds_editor/main.py` & `eds-utils-0.2.4/eds_utils/eds_editor/main.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds_editor/pages/_object_grid.py` & `eds-utils-0.2.4/eds_utils/eds_editor/pages/_object_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         label = Gtk.Label.new('Access Type:')
         label.set_halign(Gtk.Align.START)
         self._obj_access_type = Gtk.DropDown()
         access_type_list = Gtk.StringList.new(strings=[i.name for i in AccessType])
         self._obj_access_type.set_model(access_type_list)
         self._obj_access_type.set_selected(0)
-        self._obj_access_type.connect('activate', self._on_obj_access_type_changed)
+        self._obj_access_type.connect('notify::selected-item', self._on_obj_access_type_changed)
         self.attach(label, column=2, row=2, width=1, height=1)
         self.attach(self._obj_access_type, column=3, row=2, width=1, height=1)
 
         label = Gtk.Label.new('Comment:')
         label.set_halign(Gtk.Align.START)
         scrolled_window = Gtk.ScrolledWindow()
         scrolled_window.set_vexpand(True)
@@ -70,15 +70,15 @@
 
         label = Gtk.Label.new('Data Type:')
         label.set_halign(Gtk.Align.START)
         self._obj_data_type = Gtk.DropDown()
         data_type_list = Gtk.StringList.new(strings=[i.name for i in DataType])
         self._obj_data_type.set_model(data_type_list)
         self._obj_data_type.set_selected(0)
-        self._obj_data_type.connect('activate', self._on_obj_data_type_changed)
+        self._obj_data_type.connect('notify::selected-item', self._on_obj_data_type_changed)
         self.attach(label, column=0, row=8, width=1, height=1)
         self.attach(self._obj_data_type, column=1, row=8, width=1, height=1)
 
         label = Gtk.Label.new('PDO Mapping:')
         label.set_halign(Gtk.Align.START)
         self._obj_pdo_mapping = Gtk.Switch()
         self._obj_pdo_mapping.set_halign(Gtk.Align.START)
@@ -116,15 +116,19 @@
         label = Gtk.Label.new('Storage Location (CANopenNode):')
         label.set_halign(Gtk.Align.START)
         self._obj_storage_loc = Gtk.DropDown()
         if self._eds.storage_locations:
             str_list = Gtk.StringList.new(strings=self._eds.storage_locations)
             self._obj_storage_loc.set_model(str_list)
             self._obj_storage_loc.set_selected(0)
-            self._obj_storage_loc.connect('activate', self._on_obj_storage_loc_changed)
+            self._obj_storage_loc.connect('notify::selected-item',
+                                          self._on_obj_storage_loc_changed)
+        else:
+            label.hide()
+            self._obj_storage_loc.hide()
         self.attach(label, column=0, row=11, width=1, height=1)
         self.attach(self._obj_storage_loc, column=1, row=11, width=1, height=1)
 
     def load_object(self, index: int, subindex: int = None):
         '''When value is selected in the treeview, changed the current selected object.'''
 
         self._index = index
@@ -137,14 +141,16 @@
         self._obj_default_value_len_label.hide()
 
         if subindex is None:
             self._obj_data_type.set_sensitive(False)
         elif self._eds[index].object_type == ObjectType.ARRAY:
             self._obj_storage_loc.set_sensitive(False)
             self._obj_data_type.set_sensitive(False)
+        else:
+            self._obj_storage_loc.set_sensitive(False)
 
         if self._selected_obj.object_type == ObjectType.ARRAY:
             self._obj_data_type.show()
             self._obj_access_type.hide()
             self._obj_pdo_mapping.hide()
             self._obj_default_value.hide()
             self._obj_low_limit.hide()
@@ -202,26 +208,27 @@
             if self._parameter_name_cb:
                 self._parameter_name_cb(name)
 
     def _on_obj_denotation_changed(self, entry: Gtk.Entry):
         if self._selected_obj:
             self._selected_obj.denotation = entry.get_text()
 
-    def _on_obj_access_type_changed(self, dropdown: Gtk.DropDown):
-        access_type = AccessType[dropdown.get_value()]
+    def _on_obj_access_type_changed(self, dropdown: Gtk.DropDown, flag: Gtk.StateFlags):
+        access_type = list(AccessType)[dropdown.get_selected()]
         if self._selected_obj:
             self._selected_obj.access_type = access_type
 
     def _on_obj_comment_changed(self, buffer: Gtk.TextBuffer):
         text = buffer.get_text(buffer.get_start_iter(), buffer.get_end_iter(), False)
         if self._selected_obj:
             self._selected_obj.comments = text
 
-    def _on_obj_data_type_changed(self, dropdown: Gtk.DropDown):
-        data_type = DataType[dropdown.get_value()]
+    def _on_obj_data_type_changed(self, dropdown: Gtk.DropDown, flag: Gtk.StateFlags):
+        data_type = list(DataType)[dropdown.get_selected()]
+        print('data change')
         if self._selected_obj:
             self._selected_obj.data_type = data_type
             if self._selected_obj.data_type in [DataType.VISIBLE_STRING, DataType.OCTET_STRING,
                                                 DataType.UNICODE_STRING]:
                 self._obj_default_value_len_label.show()
             else:
                 self._obj_default_value_len_label.hide()
@@ -248,12 +255,12 @@
             self._selected_obj.low_limit = text
 
     def _on_obj_high_limit_changed(self, entry: Gtk.Entry):
         text = entry.get_text()
         if self._selected_obj:
             self._selected_obj.high_limit = text
 
-    def _on_obj_storage_loc_changed(self, dropdown: Gtk.DropDown):
+    def _on_obj_storage_loc_changed(self, dropdown: Gtk.DropDown, flag: Gtk.StateFlags):
         if self._eds.storage_locations:
-            storage_location = self._eds.storage_locations[dropdown.get_value()]
+            storage_location = self._eds.storage_locations[dropdown.get_selected()]
             if self._selected_obj:
                 self._selected_obj.storage_location = storage_location
```

### Comparing `eds-utils-0.2.3/eds_utils/eds_editor/pages/device_commissioning_page.py` & `eds-utils-0.2.4/eds_utils/eds_editor/pages/device_commissioning_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds_editor/pages/general_info_page.py` & `eds-utils-0.2.4/eds_utils/eds_editor/pages/general_info_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds_editor/pages/object_dictionary_page.py` & `eds-utils-0.2.4/eds_utils/eds_editor/pages/object_dictionary_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds_editor/pages/pdo_page.py` & `eds-utils-0.2.4/eds_utils/eds_editor/pages/pdo_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds_editor/window.py` & `eds-utils-0.2.4/eds_utils/eds_editor/window.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils/eds_validate.py` & `eds-utils-0.2.4/eds_utils/eds_validate.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/eds_utils.egg-info/PKG-INFO` & `eds-utils-0.2.4/eds_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eds-utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: Utilities for editing CANopen EDS/DCF files
 Home-page: https://github.com/oresat/eds-utils
 Author: psas
 Author-email: oresat@pdx.edu
 Maintainer: psas
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: UI
 License-File: LICENSE
 
 =========
 eds-utils
 =========
 
 A collection of EDS / DCF utilities.
```

### Comparing `eds-utils-0.2.3/eds_utils.egg-info/SOURCES.txt` & `eds-utils-0.2.4/eds_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.3/setup.cfg` & `eds-utils-0.2.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -21,18 +21,20 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Software Development :: Embedded Systems
 
 [options]
 packages = find:
-install_requires = 
-	PyGObject
 python_requires = >=3.7
 
+[options.extras_require]
+UI = 
+	PyGObject
+
 [options.entry_points]
 console_scripts = 
 	eds-editor = eds_utils.eds_editor.main:eds_editor
 	eds-validate = eds_utils.eds_validate:eds_validate
 	eds2c = eds_utils.eds2c:eds2c
 	eds2dcf = eds_utils.eds2dcf:eds2dcf
 	eds2md = eds_utils.eds2md:eds2md
```

### Comparing `eds-utils-0.2.3/tests/test_eds.py` & `eds-utils-0.2.4/tests/test_eds.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import unittest
 
 from eds_utils.core.objects import Variable, Record
-from eds_utils.core.eds import EDS
+from eds_utils.core.eds import EDS, EDSError
 
 
 class TestEDS(unittest.TestCase):
 
     def test_insert(self):
         eds = EDS()
 
         # add a var to eds
         eds.insert(0x8000, None, Variable())
         self.assertEqual(len(eds.indexes), 1)
 
         # index already exist
-        with self.assertRaises(ValueError):
+        with self.assertRaises(EDSError):
             eds.insert(0x8000, None, Variable())
         self.assertEqual(len(eds.indexes), 1)
 
         # cannont insert an var as subindex to another var
-        with self.assertRaises(TypeError):
+        with self.assertRaises(EDSError):
             eds.insert(0x8000, 1, Variable())
         self.assertEqual(len(eds.indexes), 1)
 
         # add a rec to eds
         eds.insert(0x8100, None, Record())
         self.assertEqual(len(eds.indexes), 2)
 
         # add var to rec
         eds.insert(0x8100, 1, Variable())
         self.assertEqual(len(eds.indexes), 2)
 
         # try to re-insert var again
-        with self.assertRaises(ValueError):
+        with self.assertRaises(EDSError):
             eds.insert(0x8100, 1, Variable())
         self.assertEqual(len(eds.indexes), 2)
 
     def test_remove(self):
         eds = EDS()
 
         # try to remove something that doesn't exist
```

### Comparing `eds-utils-0.2.3/tests/test_objects.py` & `eds-utils-0.2.4/tests/test_objects.py`

 * *Files identical despite different names*

