# Comparing `tmp/ufbt-0.2.1rc3.tar.gz` & `tmp/ufbt-0.2.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufbt-0.2.1rc3.tar", last modified: Sun Apr  9 14:57:43 2023, max compression
+gzip compressed data, was "ufbt-0.2.1rc4.tar", last modified: Sun Apr  9 23:26:44 2023, max compression
```

## Comparing `ufbt-0.2.1rc3.tar` & `ufbt-0.2.1rc4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:43.555873 ufbt-0.2.1rc3/
--rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-04-09 14:57:32.000000 ufbt-0.2.1rc3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-09 14:57:43.555873 ufbt-0.2.1rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-09 14:57:32.000000 ufbt-0.2.1rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-09 14:57:32.000000 ufbt-0.2.1rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:57:43.555873 ufbt-0.2.1rc3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:43.555873 ufbt-0.2.1rc3/ufbt/
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-09 14:57:32.000000 ufbt-0.2.1rc3/ufbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-09 14:57:32.000000 ufbt-0.2.1rc3/ufbt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26207 2023-04-09 14:57:32.000000 ufbt-0.2.1rc3/ufbt/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:43.555873 ufbt-0.2.1rc3/ufbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-09 14:57:43.000000 ufbt-0.2.1rc3/ufbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-09 14:57:43.000000 ufbt-0.2.1rc3/ufbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:57:43.000000 ufbt-0.2.1rc3/ufbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 14:57:43.000000 ufbt-0.2.1rc3/ufbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 14:57:43.000000 ufbt-0.2.1rc3/ufbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:26:44.071512 ufbt-0.2.1rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-04-09 23:26:34.000000 ufbt-0.2.1rc4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-09 23:26:44.071512 ufbt-0.2.1rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-09 23:26:34.000000 ufbt-0.2.1rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-09 23:26:34.000000 ufbt-0.2.1rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 23:26:44.071512 ufbt-0.2.1rc4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:26:44.071512 ufbt-0.2.1rc4/ufbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-09 23:26:34.000000 ufbt-0.2.1rc4/ufbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-09 23:26:34.000000 ufbt-0.2.1rc4/ufbt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26207 2023-04-09 23:26:34.000000 ufbt-0.2.1rc4/ufbt/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:26:44.071512 ufbt-0.2.1rc4/ufbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-09 23:26:44.000000 ufbt-0.2.1rc4/ufbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-09 23:26:44.000000 ufbt-0.2.1rc4/ufbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 23:26:44.000000 ufbt-0.2.1rc4/ufbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 23:26:44.000000 ufbt-0.2.1rc4/ufbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 23:26:44.000000 ufbt-0.2.1rc4/ufbt.egg-info/top_level.txt
```

### Comparing `ufbt-0.2.1rc3/LICENSE.md` & `ufbt-0.2.1rc4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc3/PKG-INFO` & `ufbt-0.2.1rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.1rc3
+Version: 0.2.1rc4
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

### Comparing `ufbt-0.2.1rc3/README.md` & `ufbt-0.2.1rc4/README.md`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc3/pyproject.toml` & `ufbt-0.2.1rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc3/ufbt/__init__.py` & `ufbt-0.2.1rc4/ufbt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,12 +70,13 @@
         commandline = (
             '. "$UFBT_STATE_DIR/current/scripts/toolchain/fbtenv.sh" && '
             f'python3 -m SCons -Q --warn=target-not-built -C "$UFBT_STATE_DIR/current/scripts/ufbt" "UFBT_APP_DIR={UFBT_APP_DIR}" '
             + " ".join(sys.argv[1:])
         )
 
     # print(commandline)
-    return os.system(commandline)
+    retcode = os.system(commandline)
+    return 1 if retcode != 0 else 0
 
 
 if __name__ == "__main__":
     sys.exit(ufbt_cli() or 0)
```

### Comparing `ufbt-0.2.1rc3/ufbt/__main__.py` & `ufbt-0.2.1rc4/ufbt/__main__.py`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc3/ufbt/bootstrap.py` & `ufbt-0.2.1rc4/ufbt/bootstrap.py`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc3/ufbt.egg-info/PKG-INFO` & `ufbt-0.2.1rc4/ufbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.1rc3
+Version: 0.2.1rc4
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

