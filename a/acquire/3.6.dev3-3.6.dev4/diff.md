# Comparing `tmp/acquire-3.6.dev3.tar.gz` & `tmp/acquire-3.6.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquire-3.6.dev3.tar", last modified: Tue Apr 11 10:55:30 2023, max compression
+gzip compressed data, was "acquire-3.6.dev4.tar", last modified: Tue Apr 11 15:03:24 2023, max compression
```

## Comparing `acquire-3.6.dev3.tar` & `acquire-3.6.dev4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:55:30.042977 acquire-3.6.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-11 10:55:10.000000 acquire-3.6.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-11 10:55:10.000000 acquire-3.6.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 10:55:10.000000 acquire-3.6.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-11 10:55:30.042977 acquire-3.6.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-11 10:55:10.000000 acquire-3.6.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:55:30.034977 acquire-3.6.dev3/acquire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69745 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/acquire.py
--rw-r--r--   0 runner    (1001) docker     (123)    20712 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:55:30.034977 acquire-3.6.dev3/acquire/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:55:30.038977 acquire-3.6.dev3/acquire/dynamic/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/dynamic/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/dynamic/windows/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/dynamic/windows/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/dynamic/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/dynamic/windows/named_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/dynamic/windows/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/dynamic/windows/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/esxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:55:30.038977 acquire-3.6.dev3/acquire/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/outputs/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/outputs/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:55:30.038977 acquire-3.6.dev3/acquire/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/tools/decrypter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:55:30.038977 acquire-3.6.dev3/acquire/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/uploaders/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/uploaders/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/uploaders/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-04-11 10:55:10.000000 acquire-3.6.dev3/acquire/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-11 10:55:29.000000 acquire-3.6.dev3/acquire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:55:30.034977 acquire-3.6.dev3/acquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-11 10:55:29.000000 acquire-3.6.dev3/acquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-11 10:55:30.000000 acquire-3.6.dev3/acquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:55:29.000000 acquire-3.6.dev3/acquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 10:55:29.000000 acquire-3.6.dev3/acquire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-11 10:55:29.000000 acquire-3.6.dev3/acquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 10:55:29.000000 acquire-3.6.dev3/acquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-11 10:55:18.000000 acquire-3.6.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:55:30.042977 acquire-3.6.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:55:30.042977 acquire-3.6.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:55:10.000000 acquire-3.6.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-11 10:55:10.000000 acquire-3.6.dev3/tests/test_acquire_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-11 10:55:10.000000 acquire-3.6.dev3/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-11 10:55:10.000000 acquire-3.6.dev3/tests/test_esxi_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-11 10:55:10.000000 acquire-3.6.dev3/tests/test_file_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-11 10:55:10.000000 acquire-3.6.dev3/tests/test_minio_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-11 10:55:10.000000 acquire-3.6.dev3/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-11 10:55:10.000000 acquire-3.6.dev3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-11 10:55:10.000000 acquire-3.6.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.828563 acquire-3.6.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-11 15:03:10.000000 acquire-3.6.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-11 15:03:10.000000 acquire-3.6.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 15:03:10.000000 acquire-3.6.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-11 15:03:24.828563 acquire-3.6.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-11 15:03:10.000000 acquire-3.6.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.812563 acquire-3.6.dev4/acquire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75148 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20712 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.816563 acquire-3.6.dev4/acquire/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.820563 acquire-3.6.dev4/acquire/dynamic/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/windows/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/windows/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/windows/named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/windows/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/dynamic/windows/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/esxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.820563 acquire-3.6.dev4/acquire/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/outputs/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/outputs/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.820563 acquire-3.6.dev4/acquire/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/tools/decrypter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.824563 acquire-3.6.dev4/acquire/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/uploaders/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/uploaders/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/uploaders/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-04-11 15:03:10.000000 acquire-3.6.dev4/acquire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-11 15:03:24.000000 acquire-3.6.dev4/acquire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.816563 acquire-3.6.dev4/acquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-11 15:03:24.000000 acquire-3.6.dev4/acquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-11 15:03:24.000000 acquire-3.6.dev4/acquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:03:24.000000 acquire-3.6.dev4/acquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 15:03:24.000000 acquire-3.6.dev4/acquire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-11 15:03:24.000000 acquire-3.6.dev4/acquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 15:03:24.000000 acquire-3.6.dev4/acquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-11 15:03:15.000000 acquire-3.6.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:03:24.828563 acquire-3.6.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:24.828563 acquire-3.6.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/test_acquire_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/test_esxi_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/test_file_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/test_minio_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-11 15:03:10.000000 acquire-3.6.dev4/tox.ini
```

### Comparing `acquire-3.6.dev3/LICENSE` & `acquire-3.6.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/PKG-INFO` & `acquire-3.6.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.6.dev3
+Version: 3.6.dev4
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Programming Language :: Python :: 3
```

### Comparing `acquire-3.6.dev3/README.md` & `acquire-3.6.dev4/README.md`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/acquire.py` & `acquire-3.6.dev4/acquire/acquire.py`

 * *Files 4% similar despite different names*

```diff
@@ -1096,14 +1096,59 @@
         ("glob", "/Users/*/Library/Application Support/Google/Chrome/*/Last Session"),
         ("glob", "/Users/*/Library/Application Support/Google/Chrome/*/Last Tabs"),
         ("glob", "/Users/*/Library/Application Support/Chromium/*/Current Session"),
         ("glob", "/Users/*/Library/Application Support/Chromium/*/Current Tabs"),
         ("glob", "/Users/*/Library/Application Support/Chromium/*/Archived History"),
         ("glob", "/Users/*/Library/Application Support/Chromium/*/Last Session"),
         ("glob", "/Users/*/Library/Application Support/Chromium/*/Last Tabs"),
+        # Chrome - RHEL/Ubuntu - DNF
+        ("glob", ".config/google-chrome/*/Bookmarks", from_user_home),
+        ("glob", ".config/google-chrome/*/Favicons", from_user_home),
+        ("glob", ".config/google-chrome/*/History", from_user_home),
+        ("glob", ".config/google-chrome/*/Login Data", from_user_home),
+        ("glob", ".config/google-chrome/*/Login Data For Account", from_user_home),
+        ("glob", ".config/google-chrome/*/Shortcuts", from_user_home),
+        ("glob", ".config/google-chrome/*/Top Sites", from_user_home),
+        ("glob", ".config/google-chrome/*/Web Data", from_user_home),
+        # Chrome - RHEL/Ubuntu - Flatpak
+        ("glob", ".var/app/com.google.Chrome/config/google-chrome/*/Bookmarks", from_user_home),
+        ("glob", ".var/app/com.google.Chrome/config/google-chrome/*/Favicons", from_user_home),
+        ("glob", ".var/app/com.google.Chrome/config/google-chrome/*/History", from_user_home),
+        ("glob", ".var/app/com.google.Chrome/config/google-chrome/*/Login Data", from_user_home),
+        ("glob", ".var/app/com.google.Chrome/config/google-chrome/*/Login Data For Account", from_user_home),
+        ("glob", ".var/app/com.google.Chrome/config/google-chrome/*/Shortcuts", from_user_home),
+        ("glob", ".var/app/com.google.Chrome/config/google-chrome/*/Top Sites", from_user_home),
+        ("glob", ".var/app/com.google.Chrome/config/google-chrome/*/Web Data", from_user_home),
+        # Chromium - RHEL/Ubuntu - DNF/apt
+        ("glob", ".config/chromium/*/Bookmarks", from_user_home),
+        ("glob", ".config/chromium/*/Favicons", from_user_home),
+        ("glob", ".config/chromium/*/History", from_user_home),
+        ("glob", ".config/chromium/*/Login Data", from_user_home),
+        ("glob", ".config/chromium/*/Login Data For Account", from_user_home),
+        ("glob", ".config/chromium/*/Shortcuts", from_user_home),
+        ("glob", ".config/chromium/*/Top Sites", from_user_home),
+        ("glob", ".config/chromium/*/Web Data", from_user_home),
+        # Chromium - RHEL/Ubuntu - Flatpak
+        ("glob", ".var/app/org.chromium.Chromium/config/chromium/*/Bookmarks", from_user_home),
+        ("glob", ".var/app/org.chromium.Chromium/config/chromium/*/Favicons", from_user_home),
+        ("glob", ".var/app/org.chromium.Chromium/config/chromium/*/History", from_user_home),
+        ("glob", ".var/app/org.chromium.Chromium/config/chromium/*/Login Data", from_user_home),
+        ("glob", ".var/app/org.chromium.Chromium/config/chromium/*/Login Data For Account", from_user_home),
+        ("glob", ".var/app/org.chromium.Chromium/config/chromium/*/Shortcuts", from_user_home),
+        ("glob", ".var/app/org.chromium.Chromium/config/chromium/*/Top Sites", from_user_home),
+        ("glob", ".var/app/org.chromium.Chromium/config/chromium/*/Web Data", from_user_home),
+        # Chromium - RHEL/Ubuntu - snap
+        ("glob", "snap/chromium/common/chromium/*/Bookmarks", from_user_home),
+        ("glob", "snap/chromium/common/chromium/*/Favicons", from_user_home),
+        ("glob", "snap/chromium/common/chromium/*/History", from_user_home),
+        ("glob", "snap/chromium/common/chromium/*/Login Data", from_user_home),
+        ("glob", "snap/chromium/common/chromium/*/Login Data For Account", from_user_home),
+        ("glob", "snap/chromium/common/chromium/*/Shortcuts", from_user_home),
+        ("glob", "snap/chromium/common/chromium/*/Top Sites", from_user_home),
+        ("glob", "snap/chromium/common/chromium/*/Web Data", from_user_home),
         # Edge
         ("glob", "AppData/Local/Microsoft/Edge/User Data/*/Bookmarks", from_user_home),
         ("glob", "AppData/Local/Microsoft/Edge/User Data/*/Extension Cookies", from_user_home),
         ("glob", "AppData/Local/Microsoft/Edge/User Data/*/Favicons", from_user_home),
         ("glob", "AppData/Local/Microsoft/Edge/User Data/*/History", from_user_home),
         ("glob", "AppData/Local/Microsoft/Edge/User Data/*/Login Data", from_user_home),
         ("glob", "AppData/Local/Microsoft/Edge/User Data/*/Media History", from_user_home),
@@ -1160,20 +1205,45 @@
         ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/Favicons"),
         ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/History"),
         ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/Login Data"),
         ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/Media History"),
         ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/Shortcuts"),
         ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/Top Sites"),
         ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/Web Data"),
-        # Firefox
+        # Edge - RHEL/Ubuntu - DNF/apt
+        ("glob", ".config/microsoft-edge/*/Bookmarks", from_user_home),
+        ("glob", ".config/microsoft-edge/*/Favicons", from_user_home),
+        ("glob", ".config/microsoft-edge/*/History", from_user_home),
+        ("glob", ".config/microsoft-edge/*/Login Data", from_user_home),
+        ("glob", ".config/microsoft-edge/*/Login Data For Account", from_user_home),
+        ("glob", ".config/microsoft-edge/*/Shortcuts", from_user_home),
+        ("glob", ".config/microsoft-edge/*/Top Sites", from_user_home),
+        ("glob", ".config/microsoft-edge/*/Web Data", from_user_home),
+        # Edge - RHEL/Ubuntu - Flatpak
+        ("glob", ".var/app/com.microsoft.Edge/config/microsoft-edge/*/Bookmarks", from_user_home),
+        ("glob", ".var/app/com.microsoft.Edge/config/microsoft-edge/*/Favicons", from_user_home),
+        ("glob", ".var/app/com.microsoft.Edge/config/microsoft-edge/*/History", from_user_home),
+        ("glob", ".var/app/com.microsoft.Edge/config/microsoft-edge/*/Login Data", from_user_home),
+        ("glob", ".var/app/com.microsoft.Edge/config/microsoft-edge/*/Login Data For Account", from_user_home),
+        ("glob", ".var/app/com.microsoft.Edge/config/microsoft-edge/*/Shortcuts", from_user_home),
+        ("glob", ".var/app/com.microsoft.Edge/config/microsoft-edge/*/Top Sites", from_user_home),
+        ("glob", ".var/app/com.microsoft.Edge/config/microsoft-edge/*/Web Data", from_user_home),
+        # Firefox - Windows
         ("glob", "AppData/Local/Mozilla/Firefox/Profiles/*/*.sqlite*", from_user_home),
         ("glob", "AppData/Roaming/Mozilla/Firefox/Profiles/*/*.sqlite*", from_user_home),
         ("glob", "Application Data/Mozilla/Firefox/Profiles/*/*.sqlite*", from_user_home),
+        # Firefox - macOS
         ("glob", "/Users/*/Library/Application Support/Firefox/Profiles/*/*.sqlite*"),
-        # Safari
+        # Firefox - RHEL/Ubuntu - Flatpak
+        ("glob", ".var/app/org.mozilla.firefox/.mozilla/firefox/*/*.sqlite", from_user_home),
+        # Firefox - RHEL/Ubuntu - DNF/apt
+        ("glob", ".mozilla/firefox/*/*.sqlite", from_user_home),
+        # Firefox - RHEL/Ubuntu - snap
+        ("glob", "snap/firefox/common/.mozilla/firefox/*/*.sqlite", from_user_home),
+        # Safari - macOS
         ("glob", "/Users/*/Library/Safari/Bookmarks.plist"),
         ("glob", "/Users/*/Library/Safari/Downloads.plist"),
         ("glob", "/Users/*/Library/Safari/Extensions/Extensions.plist"),
         ("glob", "/Users/*/Library/Safari/History.*"),
         ("glob", "/Users/*/Library/Safari/LastSession.plist"),
         ("glob", "/Users/*/Library/Caches/com.apple.Safari/Cache.db"),
     ]
```

### Comparing `acquire-3.6.dev3/acquire/collector.py` & `acquire-3.6.dev4/acquire/collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/crypt.py` & `acquire-3.6.dev4/acquire/crypt.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/dynamic/windows/collect.py` & `acquire-3.6.dev4/acquire/dynamic/windows/collect.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/dynamic/windows/handles.py` & `acquire-3.6.dev4/acquire/dynamic/windows/handles.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/dynamic/windows/named_objects.py` & `acquire-3.6.dev4/acquire/dynamic/windows/named_objects.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/dynamic/windows/ntdll.py` & `acquire-3.6.dev4/acquire/dynamic/windows/ntdll.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/dynamic/windows/types.py` & `acquire-3.6.dev4/acquire/dynamic/windows/types.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/esxi.py` & `acquire-3.6.dev4/acquire/esxi.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/hashes.py` & `acquire-3.6.dev4/acquire/hashes.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/log.py` & `acquire-3.6.dev4/acquire/log.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/outputs/base.py` & `acquire-3.6.dev4/acquire/outputs/base.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/outputs/dir.py` & `acquire-3.6.dev4/acquire/outputs/dir.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/outputs/tar.py` & `acquire-3.6.dev4/acquire/outputs/tar.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/tools/decrypter.py` & `acquire-3.6.dev4/acquire/tools/decrypter.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/uploaders/minio.py` & `acquire-3.6.dev4/acquire/uploaders/minio.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/uploaders/plugin.py` & `acquire-3.6.dev4/acquire/uploaders/plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/uploaders/plugin_registry.py` & `acquire-3.6.dev4/acquire/uploaders/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire/utils.py` & `acquire-3.6.dev4/acquire/utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/acquire.egg-info/PKG-INFO` & `acquire-3.6.dev4/acquire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.6.dev3
+Version: 3.6.dev4
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Programming Language :: Python :: 3
```

### Comparing `acquire-3.6.dev3/acquire.egg-info/SOURCES.txt` & `acquire-3.6.dev4/acquire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/pyproject.toml` & `acquire-3.6.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/tests/test_acquire_command.py` & `acquire-3.6.dev4/tests/test_acquire_command.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/tests/test_collector.py` & `acquire-3.6.dev4/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/tests/test_esxi_memory.py` & `acquire-3.6.dev4/tests/test_esxi_memory.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/tests/test_file_sorting.py` & `acquire-3.6.dev4/tests/test_file_sorting.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/tests/test_minio_uploader.py` & `acquire-3.6.dev4/tests/test_minio_uploader.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/tests/test_plugin.py` & `acquire-3.6.dev4/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/tests/test_utils.py` & `acquire-3.6.dev4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev3/tox.ini` & `acquire-3.6.dev4/tox.ini`

 * *Files identical despite different names*

