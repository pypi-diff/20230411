# Comparing `tmp/easyaccess-1.4.8.dev0.tar.gz` & `tmp/easyaccess-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyaccess-1.4.8.dev0.tar", last modified: Thu Feb 24 20:52:41 2022, max compression
+gzip compressed data, was "easyaccess-1.4.9.tar", last modified: Thu Feb 24 20:57:36 2022, max compression
```

## Comparing `easyaccess-1.4.8.dev0.tar` & `easyaccess-1.4.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:52:41.517758 easyaccess-1.4.8.dev0/
--rw-r--r--   0 mjohns44   (502) staff       (20)      423 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/AUTHORS.md
--rw-r--r--   0 mjohns44   (502) staff       (20)     7257 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/CHANGES.md
--rw-r--r--   0 mjohns44   (502) staff       (20)     3349 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/CODE_OF_CONDUCT.md
--rw-r--r--   0 mjohns44   (502) staff       (20)     2418 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/CONTRIBUTING.md
--rw-r--r--   0 mjohns44   (502) staff       (20)     2431 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/FAQ.md
--rw-r--r--   0 mjohns44   (502) staff       (20)     1758 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/LICENSE.txt
--rw-r--r--   0 mjohns44   (502) staff       (20)      162 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/MANIFEST.in
--rw-r--r--   0 mjohns44   (502) staff       (20)     9801 2022-02-24 20:52:41.517192 easyaccess-1.4.8.dev0/PKG-INFO
--rw-r--r--   0 mjohns44   (502) staff       (20)     9405 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/README.md
--rw-r--r--   0 mjohns44   (502) staff       (20)      524 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/TODO.md
-drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:52:41.499646 easyaccess-1.4.8.dev0/bin/
--rwxr-xr-x   0 mjohns44   (502) staff       (20)       55 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/bin/easyaccess
-drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:52:41.494851 easyaccess-1.4.8.dev0/config/
-drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:52:41.500039 easyaccess-1.4.8.dev0/config/conda/
--rw-r--r--   0 mjohns44   (502) staff       (20)     1174 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/config/conda/meta.yaml
-drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:52:41.503627 easyaccess-1.4.8.dev0/data/
--rw-r--r--   0 mjohns44   (502) staff       (20)  1205787 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/data/help.gif
--rw-r--r--   0 mjohns44   (502) staff       (20)   122665 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/data/help_screenshot.png
-drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:52:41.506144 easyaccess-1.4.8.dev0/easyaccess/
--rw-r--r--   0 mjohns44   (502) staff       (20)      223 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/__init__.py
--rw-r--r--   0 mjohns44   (502) staff       (20)    11991 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/config_ea.py
--rw-r--r--   0 mjohns44   (502) staff       (20)     5365 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/eaparser.py
--rwxr-xr-x   0 mjohns44   (502) staff       (20)    55518 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/easyaccess.py
-drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:52:41.513959 easyaccess-1.4.8.dev0/easyaccess/eautils/
--rw-r--r--   0 mjohns44   (502) staff       (20)      180 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/eautils/__init__.py
--rw-r--r--   0 mjohns44   (502) staff       (20)     5740 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/eautils/cli_utils.py
--rw-r--r--   0 mjohns44   (502) staff       (20)    18873 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/eautils/db_api.py
--rw-r--r--   0 mjohns44   (502) staff       (20)    35002 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/eautils/db_utils.py
--rw-r--r--   0 mjohns44   (502) staff       (20)     1195 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/eautils/des_logo.py
--rw-r--r--   0 mjohns44   (502) staff       (20)     9498 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/eautils/des_utils.py
--rw-r--r--   0 mjohns44   (502) staff       (20)      878 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/eautils/dircache.py
--rw-r--r--   0 mjohns44   (502) staff       (20)     7269 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/eautils/dtypes.py
--rw-r--r--   0 mjohns44   (502) staff       (20)     3665 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/eautils/ea_utils.py
--rw-r--r--   0 mjohns44   (502) staff       (20)    14457 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/eautils/fileio.py
--rw-r--r--   0 mjohns44   (502) staff       (20)     3923 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/eautils/fun_utils.py
--rw-r--r--   0 mjohns44   (502) staff       (20)     3945 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/eautils/import_utils.py
--rw-r--r--   0 mjohns44   (502) staff       (20)    11642 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/eautils/python_api.py
--rw-r--r--   0 mjohns44   (502) staff       (20)      883 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/easyaccess/version.py
-drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:52:41.508311 easyaccess-1.4.8.dev0/easyaccess.egg-info/
--rw-r--r--   0 mjohns44   (502) staff       (20)     9801 2022-02-24 20:52:40.000000 easyaccess-1.4.8.dev0/easyaccess.egg-info/PKG-INFO
--rw-r--r--   0 mjohns44   (502) staff       (20)      994 2022-02-24 20:52:40.000000 easyaccess-1.4.8.dev0/easyaccess.egg-info/SOURCES.txt
--rw-r--r--   0 mjohns44   (502) staff       (20)        1 2022-02-24 20:52:40.000000 easyaccess-1.4.8.dev0/easyaccess.egg-info/dependency_links.txt
--rw-r--r--   0 mjohns44   (502) staff       (20)      103 2022-02-24 20:52:40.000000 easyaccess-1.4.8.dev0/easyaccess.egg-info/requires.txt
--rw-r--r--   0 mjohns44   (502) staff       (20)       11 2022-02-24 20:52:40.000000 easyaccess-1.4.8.dev0/easyaccess.egg-info/top_level.txt
--rw-r--r--   0 mjohns44   (502) staff       (20)       38 2022-02-24 20:52:41.517921 easyaccess-1.4.8.dev0/setup.cfg
--rw-r--r--   0 mjohns44   (502) staff       (20)     1443 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/setup.py
-drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:52:41.516562 easyaccess-1.4.8.dev0/tests/
--rw-r--r--   0 mjohns44   (502) staff       (20)    19982 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/tests/test_api.py
--rw-r--r--   0 mjohns44   (502) staff       (20)      934 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/tests/test_connection.py
--rw-r--r--   0 mjohns44   (502) staff       (20)    20883 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/tests/test_interpreter.py
--rwxr-xr-x   0 mjohns44   (502) staff       (20)     5277 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/tests/test_load_table.py
--rw-r--r--   0 mjohns44   (502) staff       (20)      669 2022-02-24 20:52:05.000000 easyaccess-1.4.8.dev0/tests/wrapped.py
+drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:57:36.246247 easyaccess-1.4.9/
+-rw-r--r--   0 mjohns44   (502) staff       (20)      423 2022-02-24 20:57:05.000000 easyaccess-1.4.9/AUTHORS.md
+-rw-r--r--   0 mjohns44   (502) staff       (20)     7257 2022-02-24 20:57:05.000000 easyaccess-1.4.9/CHANGES.md
+-rw-r--r--   0 mjohns44   (502) staff       (20)     3349 2022-02-24 20:57:05.000000 easyaccess-1.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 mjohns44   (502) staff       (20)     2418 2022-02-24 20:57:05.000000 easyaccess-1.4.9/CONTRIBUTING.md
+-rw-r--r--   0 mjohns44   (502) staff       (20)     2431 2022-02-24 20:57:05.000000 easyaccess-1.4.9/FAQ.md
+-rw-r--r--   0 mjohns44   (502) staff       (20)     1758 2022-02-24 20:57:05.000000 easyaccess-1.4.9/LICENSE.txt
+-rw-r--r--   0 mjohns44   (502) staff       (20)      162 2022-02-24 20:57:05.000000 easyaccess-1.4.9/MANIFEST.in
+-rw-r--r--   0 mjohns44   (502) staff       (20)     9796 2022-02-24 20:57:36.245796 easyaccess-1.4.9/PKG-INFO
+-rw-r--r--   0 mjohns44   (502) staff       (20)     9405 2022-02-24 20:57:05.000000 easyaccess-1.4.9/README.md
+-rw-r--r--   0 mjohns44   (502) staff       (20)      524 2022-02-24 20:57:05.000000 easyaccess-1.4.9/TODO.md
+drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:57:36.225091 easyaccess-1.4.9/bin/
+-rwxr-xr-x   0 mjohns44   (502) staff       (20)       55 2022-02-24 20:57:05.000000 easyaccess-1.4.9/bin/easyaccess
+drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:57:36.219846 easyaccess-1.4.9/config/
+drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:57:36.225608 easyaccess-1.4.9/config/conda/
+-rw-r--r--   0 mjohns44   (502) staff       (20)     1174 2022-02-24 20:57:05.000000 easyaccess-1.4.9/config/conda/meta.yaml
+drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:57:36.229302 easyaccess-1.4.9/data/
+-rw-r--r--   0 mjohns44   (502) staff       (20)  1205787 2022-02-24 20:57:05.000000 easyaccess-1.4.9/data/help.gif
+-rw-r--r--   0 mjohns44   (502) staff       (20)   122665 2022-02-24 20:57:05.000000 easyaccess-1.4.9/data/help_screenshot.png
+drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:57:36.232586 easyaccess-1.4.9/easyaccess/
+-rw-r--r--   0 mjohns44   (502) staff       (20)      223 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/__init__.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)    11991 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/config_ea.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)     5365 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/eaparser.py
+-rwxr-xr-x   0 mjohns44   (502) staff       (20)    55518 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/easyaccess.py
+drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:57:36.242258 easyaccess-1.4.9/easyaccess/eautils/
+-rw-r--r--   0 mjohns44   (502) staff       (20)      180 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/eautils/__init__.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)     5740 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/eautils/cli_utils.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)    18873 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/eautils/db_api.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)    35002 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/eautils/db_utils.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)     1195 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/eautils/des_logo.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)     9498 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/eautils/des_utils.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)      878 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/eautils/dircache.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)     7269 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/eautils/dtypes.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)     3665 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/eautils/ea_utils.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)    14457 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/eautils/fileio.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)     3923 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/eautils/fun_utils.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)     3945 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/eautils/import_utils.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)    11642 2022-02-24 20:57:05.000000 easyaccess-1.4.9/easyaccess/eautils/python_api.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)      892 2022-02-24 20:57:32.000000 easyaccess-1.4.9/easyaccess/version.py
+drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:57:36.235527 easyaccess-1.4.9/easyaccess.egg-info/
+-rw-r--r--   0 mjohns44   (502) staff       (20)     9796 2022-02-24 20:57:36.000000 easyaccess-1.4.9/easyaccess.egg-info/PKG-INFO
+-rw-r--r--   0 mjohns44   (502) staff       (20)      994 2022-02-24 20:57:36.000000 easyaccess-1.4.9/easyaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 mjohns44   (502) staff       (20)        1 2022-02-24 20:57:36.000000 easyaccess-1.4.9/easyaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 mjohns44   (502) staff       (20)      103 2022-02-24 20:57:36.000000 easyaccess-1.4.9/easyaccess.egg-info/requires.txt
+-rw-r--r--   0 mjohns44   (502) staff       (20)       11 2022-02-24 20:57:36.000000 easyaccess-1.4.9/easyaccess.egg-info/top_level.txt
+-rw-r--r--   0 mjohns44   (502) staff       (20)       38 2022-02-24 20:57:36.246382 easyaccess-1.4.9/setup.cfg
+-rw-r--r--   0 mjohns44   (502) staff       (20)     1443 2022-02-24 20:57:05.000000 easyaccess-1.4.9/setup.py
+drwxr-xr-x   0 mjohns44   (502) staff       (20)        0 2022-02-24 20:57:36.245212 easyaccess-1.4.9/tests/
+-rw-r--r--   0 mjohns44   (502) staff       (20)    19982 2022-02-24 20:57:05.000000 easyaccess-1.4.9/tests/test_api.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)      934 2022-02-24 20:57:05.000000 easyaccess-1.4.9/tests/test_connection.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)    20883 2022-02-24 20:57:05.000000 easyaccess-1.4.9/tests/test_interpreter.py
+-rwxr-xr-x   0 mjohns44   (502) staff       (20)     5277 2022-02-24 20:57:05.000000 easyaccess-1.4.9/tests/test_load_table.py
+-rw-r--r--   0 mjohns44   (502) staff       (20)      669 2022-02-24 20:57:05.000000 easyaccess-1.4.9/tests/wrapped.py
```

### Comparing `easyaccess-1.4.8.dev0/CHANGES.md` & `easyaccess-1.4.9/CHANGES.md`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/CODE_OF_CONDUCT.md` & `easyaccess-1.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/CONTRIBUTING.md` & `easyaccess-1.4.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/FAQ.md` & `easyaccess-1.4.9/FAQ.md`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/LICENSE.txt` & `easyaccess-1.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/PKG-INFO` & `easyaccess-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyaccess
-Version: 1.4.8.dev0
+Version: 1.4.9
 Summary: Easy access to the DES DB. Enhanced command line SQL interpreter client for DES
 Home-page: https://github.com/des-labs/easyaccess
 Author: Matias Carrasco Kind
 Author-email: mcarras2@illinois.edu
 License: LICENSE.txt
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `easyaccess-1.4.8.dev0/README.md` & `easyaccess-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/TODO.md` & `easyaccess-1.4.9/TODO.md`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/config/conda/meta.yaml` & `easyaccess-1.4.9/config/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/data/help.gif` & `easyaccess-1.4.9/data/help.gif`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/data/help_screenshot.png` & `easyaccess-1.4.9/data/help_screenshot.png`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/config_ea.py` & `easyaccess-1.4.9/easyaccess/config_ea.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/eaparser.py` & `easyaccess-1.4.9/easyaccess/eaparser.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/easyaccess.py` & `easyaccess-1.4.9/easyaccess/easyaccess.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/eautils/cli_utils.py` & `easyaccess-1.4.9/easyaccess/eautils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/eautils/db_api.py` & `easyaccess-1.4.9/easyaccess/eautils/db_api.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/eautils/db_utils.py` & `easyaccess-1.4.9/easyaccess/eautils/db_utils.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/eautils/des_logo.py` & `easyaccess-1.4.9/easyaccess/eautils/des_logo.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/eautils/des_utils.py` & `easyaccess-1.4.9/easyaccess/eautils/des_utils.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/eautils/dircache.py` & `easyaccess-1.4.9/easyaccess/eautils/dircache.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/eautils/dtypes.py` & `easyaccess-1.4.9/easyaccess/eautils/dtypes.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/eautils/ea_utils.py` & `easyaccess-1.4.9/easyaccess/eautils/ea_utils.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/eautils/fileio.py` & `easyaccess-1.4.9/easyaccess/eautils/fileio.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/eautils/fun_utils.py` & `easyaccess-1.4.9/easyaccess/eautils/fun_utils.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/eautils/import_utils.py` & `easyaccess-1.4.9/easyaccess/eautils/import_utils.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/eautils/python_api.py` & `easyaccess-1.4.9/easyaccess/eautils/python_api.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/easyaccess/version.py` & `easyaccess-1.4.9/easyaccess/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,12 +22,12 @@
             up_time = data["releases"][k][0]["upload_time"]
             uploads.append([k, datetime.strptime(up_time, "%Y-%m-%dT%H:%M:%S")])
         except:
             pass
     return sorted(uploads, key=lambda x: x[1])[-1][0]
 
 
-version_tag = (1, 4, 8, 'dev')
+version_tag = (1,4,9) #(1, 4, 8, 'dev')
 __version__ = ".".join(map(str, version_tag[:3]))
 
 if len(version_tag) > 3:
     __version__ = "%s-%s" % (__version__, version_tag[3])
```

### Comparing `easyaccess-1.4.8.dev0/easyaccess.egg-info/PKG-INFO` & `easyaccess-1.4.9/easyaccess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyaccess
-Version: 1.4.8.dev0
+Version: 1.4.9
 Summary: Easy access to the DES DB. Enhanced command line SQL interpreter client for DES
 Home-page: https://github.com/des-labs/easyaccess
 Author: Matias Carrasco Kind
 Author-email: mcarras2@illinois.edu
 License: LICENSE.txt
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `easyaccess-1.4.8.dev0/easyaccess.egg-info/SOURCES.txt` & `easyaccess-1.4.9/easyaccess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/setup.py` & `easyaccess-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/tests/test_api.py` & `easyaccess-1.4.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/tests/test_connection.py` & `easyaccess-1.4.9/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/tests/test_interpreter.py` & `easyaccess-1.4.9/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/tests/test_load_table.py` & `easyaccess-1.4.9/tests/test_load_table.py`

 * *Files identical despite different names*

### Comparing `easyaccess-1.4.8.dev0/tests/wrapped.py` & `easyaccess-1.4.9/tests/wrapped.py`

 * *Files identical despite different names*

