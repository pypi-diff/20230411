# Comparing `tmp/eds-utils-0.2.4.tar.gz` & `tmp/eds-utils-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eds-utils-0.2.4.tar", last modified: Tue Apr 11 03:09:21 2023, max compression
+gzip compressed data, was "eds-utils-0.2.5.tar", last modified: Tue Apr 11 03:17:38 2023, max compression
```

## Comparing `eds-utils-0.2.4.tar` & `eds-utils-0.2.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.879304 eds-utils-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 03:09:12.000000 eds-utils-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-11 03:09:21.879304 eds-utils-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-11 03:09:12.000000 eds-utils-0.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.875304 eds-utils-0.2.4/eds_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.875304 eds-utils-0.2.4/eds_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/eds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.875304 eds-utils-0.2.4/eds_utils/core/file_io/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/file_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22994 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/file_io/read_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/file_io/write_canopennode.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/file_io/write_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/file_io/write_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/file_io/write_rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/core/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds2dcf.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds2md.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds2rst.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_autofix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.879304 eds-utils-0.2.4/eds_utils/eds_editor/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.879304 eds-utils-0.2.4/eds_utils/eds_editor/dialogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/dialogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/dialogs/add_object_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/dialogs/copy_object_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/dialogs/errors_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/dialogs/open_tmp_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/eds_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.879304 eds-utils-0.2.4/eds_utils/eds_editor/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/pages/_object_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/pages/device_commissioning_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/pages/general_info_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/pages/object_dictionary_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/pages/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/pages/pdo_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_editor/window.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 03:09:12.000000 eds-utils-0.2.4/eds_utils/eds_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.875304 eds-utils-0.2.4/eds_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-11 03:09:21.000000 eds-utils-0.2.4/eds_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-11 03:09:21.000000 eds-utils-0.2.4/eds_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:09:21.000000 eds-utils-0.2.4/eds_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-11 03:09:21.000000 eds-utils-0.2.4/eds_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 03:09:21.000000 eds-utils-0.2.4/eds_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 03:09:21.000000 eds-utils-0.2.4/eds_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 03:09:12.000000 eds-utils-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-11 03:09:21.879304 eds-utils-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:21.879304 eds-utils-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:09:12.000000 eds-utils-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-11 03:09:12.000000 eds-utils-0.2.4/tests/test_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-11 03:09:12.000000 eds-utils-0.2.4/tests/test_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.703668 eds-utils-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 03:17:28.000000 eds-utils-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-11 03:17:38.703668 eds-utils-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-11 03:17:28.000000 eds-utils-0.2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.691668 eds-utils-0.2.5/eds_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.695668 eds-utils-0.2.5/eds_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/eds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.695668 eds-utils-0.2.5/eds_utils/core/file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/file_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22994 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/file_io/read_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/file_io/write_canopennode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/file_io/write_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/file_io/write_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/file_io/write_rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/core/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds2dcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds2md.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds2rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_autofix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.699668 eds-utils-0.2.5/eds_utils/eds_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.699668 eds-utils-0.2.5/eds_utils/eds_editor/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/dialogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/dialogs/add_object_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/dialogs/copy_object_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/dialogs/errors_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/dialogs/open_tmp_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/eds_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.703668 eds-utils-0.2.5/eds_utils/eds_editor/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/pages/_object_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/pages/device_commissioning_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/pages/general_info_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/pages/object_dictionary_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/pages/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/pages/pdo_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_editor/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 03:17:28.000000 eds-utils-0.2.5/eds_utils/eds_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.695668 eds-utils-0.2.5/eds_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-11 03:17:38.000000 eds-utils-0.2.5/eds_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-11 03:17:38.000000 eds-utils-0.2.5/eds_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:17:38.000000 eds-utils-0.2.5/eds_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-11 03:17:38.000000 eds-utils-0.2.5/eds_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 03:17:38.000000 eds-utils-0.2.5/eds_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 03:17:38.000000 eds-utils-0.2.5/eds_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 03:17:28.000000 eds-utils-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-11 03:17:38.703668 eds-utils-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:38.703668 eds-utils-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:17:28.000000 eds-utils-0.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-11 03:17:28.000000 eds-utils-0.2.5/tests/test_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-11 03:17:28.000000 eds-utils-0.2.5/tests/test_objects.py
```

### Comparing `eds-utils-0.2.4/LICENSE` & `eds-utils-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/PKG-INFO` & `eds-utils-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eds-utils
-Version: 0.2.4
+Version: 0.2.5
 Summary: Utilities for editing CANopen EDS/DCF files
 Home-page: https://github.com/oresat/eds-utils
 Author: psas
 Author-email: oresat@pdx.edu
 Maintainer: psas
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `eds-utils-0.2.4/README.rst` & `eds-utils-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/__main__.py` & `eds-utils-0.2.5/eds_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/core/__init__.py` & `eds-utils-0.2.5/eds_utils/core/__init__.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/core/eds.py` & `eds-utils-0.2.5/eds_utils/core/eds.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/core/file_io/read_eds.py` & `eds-utils-0.2.5/eds_utils/core/file_io/read_eds.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/core/file_io/write_canopennode.py` & `eds-utils-0.2.5/eds_utils/core/file_io/write_canopennode.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/core/file_io/write_eds.py` & `eds-utils-0.2.5/eds_utils/core/file_io/write_eds.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/core/file_io/write_md.py` & `eds-utils-0.2.5/eds_utils/core/file_io/write_md.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/core/file_io/write_rst.py` & `eds-utils-0.2.5/eds_utils/core/file_io/write_rst.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/core/objects.py` & `eds-utils-0.2.5/eds_utils/core/objects.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds2c.py` & `eds-utils-0.2.5/eds_utils/eds2c.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds2dcf.py` & `eds-utils-0.2.5/eds_utils/eds2dcf.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds2md.py` & `eds-utils-0.2.5/eds_utils/eds2md.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds2rst.py` & `eds-utils-0.2.5/eds_utils/eds2rst.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds_autofix.py` & `eds-utils-0.2.5/eds_utils/eds_autofix.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds_editor/app.py` & `eds-utils-0.2.5/eds_utils/eds_editor/app.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py` & `eds-utils-0.2.5/eds_utils/eds_editor/dialogs/add_mapped_object_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds_editor/dialogs/add_object_dialog.py` & `eds-utils-0.2.5/eds_utils/eds_editor/dialogs/add_object_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds_editor/dialogs/copy_object_dialog.py` & `eds-utils-0.2.5/eds_utils/eds_editor/dialogs/copy_object_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds_editor/dialogs/errors_dialog.py` & `eds-utils-0.2.5/eds_utils/eds_editor/dialogs/errors_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds_editor/dialogs/open_tmp_dialog.py` & `eds-utils-0.2.5/eds_utils/eds_editor/dialogs/open_tmp_dialog.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds_editor/eds_notebook.py` & `eds-utils-0.2.5/eds_utils/eds_editor/eds_notebook.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds_editor/main.py` & `eds-utils-0.2.5/eds_utils/eds_editor/main.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds_editor/pages/_object_grid.py` & `eds-utils-0.2.5/eds_utils/eds_editor/pages/_object_grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.attach(self._obj_data_type, column=1, row=8, width=1, height=1)
 
         label = Gtk.Label.new('PDO Mapping:')
         label.set_halign(Gtk.Align.START)
         self._obj_pdo_mapping = Gtk.Switch()
         self._obj_pdo_mapping.set_halign(Gtk.Align.START)
         self._obj_pdo_mapping.set_valign(Gtk.Align.CENTER)
-        self._obj_pdo_mapping.connect('activate', self._on_obj_pdo_mapping_changed)
+        self._obj_pdo_mapping.connect('state-set', self._on_obj_pdo_mapping_changed)
         self.attach(label, column=2, row=8, width=1, height=1)
         self.attach(self._obj_pdo_mapping, column=3, row=8, width=1, height=1)
 
         label = Gtk.Label.new('Default Value:')
         label.set_halign(Gtk.Align.START)
         self._obj_default_value = Gtk.Entry()
         self._obj_default_value.connect('changed', self._on_obj_default_value_changed)
@@ -187,15 +187,15 @@
             self._obj_storage_loc.set_selected(self._eds.storage_locations.index(storage_loc))
         if self._selected_obj.object_type == ObjectType.VAR:
             data_type = self._selected_obj.data_type
             self._obj_data_type.set_selected(list(DataType).index(data_type))
             access_type = self._selected_obj.access_type
             self._obj_access_type.set_selected(list(AccessType).index(access_type))
             self._obj_default_value.set_text(self._selected_obj.default_value)
-            self._obj_pdo_mapping.set_state(self._selected_obj.pdo_mapping)
+            self._obj_pdo_mapping.set_active(self._selected_obj.pdo_mapping)
             self._obj_low_limit.set_text(self._selected_obj.low_limit)
             self._obj_high_limit.set_text(self._selected_obj.high_limit)
         elif self._selected_obj.object_type == ObjectType.ARRAY:
             if len(self._selected_obj) > 1:
                 data_type = self._selected_obj[1].data_type
                 self._obj_data_type.set_selected(list(DataType).index(data_type))
             else:  # array is empty, use dafault
@@ -220,38 +220,36 @@
     def _on_obj_comment_changed(self, buffer: Gtk.TextBuffer):
         text = buffer.get_text(buffer.get_start_iter(), buffer.get_end_iter(), False)
         if self._selected_obj:
             self._selected_obj.comments = text
 
     def _on_obj_data_type_changed(self, dropdown: Gtk.DropDown, flag: Gtk.StateFlags):
         data_type = list(DataType)[dropdown.get_selected()]
-        print('data change')
         if self._selected_obj:
             self._selected_obj.data_type = data_type
             if self._selected_obj.data_type in [DataType.VISIBLE_STRING, DataType.OCTET_STRING,
                                                 DataType.UNICODE_STRING]:
                 self._obj_default_value_len_label.show()
             else:
                 self._obj_default_value_len_label.hide()
 
-    def _on_obj_pdo_mapping_changed(self, switch: Gtk.Switch):
-        state = switch.get_state()
+    def _on_obj_pdo_mapping_changed(self, switch: Gtk.Switch, state: bool):
         if self._selected_obj:
             self._selected_obj.pdo_mapping = state
 
     def _on_obj_default_value_changed(self, entry: Gtk.Entry):
         text = entry.get_text()
         if self._selected_obj:
             self._selected_obj.default_value = text
+            length = 0
             if self._selected_obj.data_type in [DataType.VISIBLE_STRING, DataType.UNICODE_STRING]:
                 length = len(text)
-                self._obj_default_value_len_label.set_text(f'(Length: {length + 1})')
             elif self._selected_obj.data_type == DataType.OCTET_STRING:
                 length = m.ceil(len(text.replace(' ', '')) / 2)
-                self._obj_default_value_len_label.set_text(f'(Length: {length})')
+            self._obj_default_value_len_label.set_text(f'(Length: {length})')
 
     def _on_obj_low_limit_changed(self, entry: Gtk.Entry):
         text = entry.get_text()
         if self._selected_obj:
             self._selected_obj.low_limit = text
 
     def _on_obj_high_limit_changed(self, entry: Gtk.Entry):
```

### Comparing `eds-utils-0.2.4/eds_utils/eds_editor/pages/device_commissioning_page.py` & `eds-utils-0.2.5/eds_utils/eds_editor/pages/device_commissioning_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds_editor/pages/general_info_page.py` & `eds-utils-0.2.5/eds_utils/eds_editor/pages/general_info_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds_editor/pages/object_dictionary_page.py` & `eds-utils-0.2.5/eds_utils/eds_editor/pages/object_dictionary_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds_editor/pages/pdo_page.py` & `eds-utils-0.2.5/eds_utils/eds_editor/pages/pdo_page.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils/eds_editor/window.py` & `eds-utils-0.2.5/eds_utils/eds_editor/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,16 @@
             self.open_eds(file_path)
 
     def open_tmp_response(self, dialog: Gtk.Dialog, response: Gtk.ResponseType):
         '''Deal with the response to the open tmp dialog.'''
 
         response = dialog.get_response()
         if response == TmpResponse.USE_TMP:
-            self._open_eds(dialog.file_path + '.tmp')
+            os.rename(dialog.file_path + '.tmp', dialog.file_path)
+            self._open_eds(dialog.file_path)
         elif response == TmpResponse.DONT_USE_TMP:
             self._open_eds(dialog.file_path)
         else:
             os.remove(dialog.file_path + '.tmp')
             self._open_eds(dialog.file_path)
 
     def on_click_save(self, button: Gtk.Button):
```

### Comparing `eds-utils-0.2.4/eds_utils/eds_validate.py` & `eds-utils-0.2.5/eds_utils/eds_validate.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/eds_utils.egg-info/PKG-INFO` & `eds-utils-0.2.5/eds_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eds-utils
-Version: 0.2.4
+Version: 0.2.5
 Summary: Utilities for editing CANopen EDS/DCF files
 Home-page: https://github.com/oresat/eds-utils
 Author: psas
 Author-email: oresat@pdx.edu
 Maintainer: psas
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `eds-utils-0.2.4/eds_utils.egg-info/SOURCES.txt` & `eds-utils-0.2.5/eds_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/setup.cfg` & `eds-utils-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/tests/test_eds.py` & `eds-utils-0.2.5/tests/test_eds.py`

 * *Files identical despite different names*

### Comparing `eds-utils-0.2.4/tests/test_objects.py` & `eds-utils-0.2.5/tests/test_objects.py`

 * *Files identical despite different names*

