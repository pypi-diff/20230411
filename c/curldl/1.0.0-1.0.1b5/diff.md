# Comparing `tmp/curldl-1.0.0.tar.gz` & `tmp/curldl-1.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curldl-1.0.0.tar", last modified: Sun Apr  9 19:47:10 2023, max compression
+gzip compressed data, was "curldl-1.0.1b5.tar", last modified: Tue Apr 11 10:58:17 2023, max compression
```

## Comparing `curldl-1.0.0.tar` & `curldl-1.0.1b5.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.297367 curldl-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-09 19:45:54.000000 curldl-1.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-04-09 19:45:54.000000 curldl-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-04-09 19:47:10.297367 curldl-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-04-09 19:45:54.000000 curldl-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.289367 curldl-1.0.0/misc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.293367 curldl-1.0.0/misc/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-09 19:45:54.000000 curldl-1.0.0/misc/conda/test-environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.293367 curldl-1.0.0/misc/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-04-09 19:45:54.000000 curldl-1.0.0/misc/scripts/run-bandit.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      184 2023-04-09 19:45:54.000000 curldl-1.0.0/misc/scripts/run-mypy.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      186 2023-04-09 19:45:54.000000 curldl-1.0.0/misc/scripts/run-pylint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-09 19:45:54.000000 curldl-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:47:10.297367 curldl-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.293367 curldl-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.293367 curldl-1.0.0/src/curldl/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 19:47:10.000000 curldl-1.0.0/src/curldl/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    18853 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/curldl.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.293367 curldl-1.0.0/src/curldl/util/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/util/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/util/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/util/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-09 19:45:54.000000 curldl-1.0.0/src/curldl/util/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.293367 curldl-1.0.0/src/curldl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-04-09 19:47:10.000000 curldl-1.0.0/src/curldl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-09 19:47:10.000000 curldl-1.0.0/src/curldl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:47:10.000000 curldl-1.0.0/src/curldl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-09 19:47:10.000000 curldl-1.0.0/src/curldl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-09 19:47:10.000000 curldl-1.0.0/src/curldl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 19:47:10.000000 curldl-1.0.0/src/curldl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.293367 curldl-1.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.297367 curldl-1.0.0/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/functional/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/functional/test_curldl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:47:10.297367 curldl-1.0.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/unit/test_crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/unit/test_curldl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13398 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/unit/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/unit/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-09 19:45:54.000000 curldl-1.0.0/tests/unit/test_time.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3554 2023-04-09 19:45:54.000000 curldl-1.0.0/venv.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:58:17.350339 curldl-1.0.1b5/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-11 10:56:54.000000 curldl-1.0.1b5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:58:17.346339 curldl-1.0.1b5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:58:17.346339 curldl-1.0.1b5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-04-11 10:56:54.000000 curldl-1.0.1b5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-04-11 10:56:54.000000 curldl-1.0.1b5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-04-11 10:58:17.350339 curldl-1.0.1b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-04-11 10:56:54.000000 curldl-1.0.1b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:58:17.346339 curldl-1.0.1b5/misc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:58:17.346339 curldl-1.0.1b5/misc/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-11 10:56:54.000000 curldl-1.0.1b5/misc/conda/test-environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:58:17.346339 curldl-1.0.1b5/misc/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-04-11 10:56:54.000000 curldl-1.0.1b5/misc/scripts/run-bandit.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      184 2023-04-11 10:56:54.000000 curldl-1.0.1b5/misc/scripts/run-mypy.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      186 2023-04-11 10:56:54.000000 curldl-1.0.1b5/misc/scripts/run-pylint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-11 10:56:54.000000 curldl-1.0.1b5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:58:17.350339 curldl-1.0.1b5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:58:17.346339 curldl-1.0.1b5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:58:17.350339 curldl-1.0.1b5/src/curldl/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-11 10:56:54.000000 curldl-1.0.1b5/src/curldl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-11 10:56:54.000000 curldl-1.0.1b5/src/curldl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 10:58:17.000000 curldl-1.0.1b5/src/curldl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-11 10:56:54.000000 curldl-1.0.1b5/src/curldl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18853 2023-04-11 10:56:54.000000 curldl-1.0.1b5/src/curldl/curldl.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 10:56:54.000000 curldl-1.0.1b5/src/curldl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:58:17.350339 curldl-1.0.1b5/src/curldl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-11 10:56:54.000000 curldl-1.0.1b5/src/curldl/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-11 10:56:54.000000 curldl-1.0.1b5/src/curldl/util/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-04-11 10:56:54.000000 curldl-1.0.1b5/src/curldl/util/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-11 10:56:54.000000 curldl-1.0.1b5/src/curldl/util/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-11 10:56:54.000000 curldl-1.0.1b5/src/curldl/util/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:58:17.350339 curldl-1.0.1b5/src/curldl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-04-11 10:58:17.000000 curldl-1.0.1b5/src/curldl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-11 10:58:17.000000 curldl-1.0.1b5/src/curldl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:58:17.000000 curldl-1.0.1b5/src/curldl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 10:58:17.000000 curldl-1.0.1b5/src/curldl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-11 10:58:17.000000 curldl-1.0.1b5/src/curldl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 10:58:17.000000 curldl-1.0.1b5/src/curldl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:58:17.346339 curldl-1.0.1b5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:58:17.350339 curldl-1.0.1b5/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-11 10:56:54.000000 curldl-1.0.1b5/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-04-11 10:56:54.000000 curldl-1.0.1b5/tests/functional/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-11 10:56:54.000000 curldl-1.0.1b5/tests/functional/test_curldl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:58:17.350339 curldl-1.0.1b5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 10:56:54.000000 curldl-1.0.1b5/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-11 10:56:54.000000 curldl-1.0.1b5/tests/unit/test_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-04-11 10:56:54.000000 curldl-1.0.1b5/tests/unit/test_curldl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13398 2023-04-11 10:56:54.000000 curldl-1.0.1b5/tests/unit/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-11 10:56:54.000000 curldl-1.0.1b5/tests/unit/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-11 10:56:54.000000 curldl-1.0.1b5/tests/unit/test_time.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3554 2023-04-11 10:56:54.000000 curldl-1.0.1b5/venv.sh
```

### Comparing `curldl-1.0.0/LICENSE.md` & `curldl-1.0.1b5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/PKG-INFO` & `curldl-1.0.1b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curldl
-Version: 1.0.0
+Version: 1.0.1b5
 Summary: Safely and reliably download files with PycURL
 Author-email: Michael Orlov <orlovm@noexec.org>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://github.com/noexec/curldl
 Project-URL: Documentation, https://pypi.org/project/curldl/
 Project-URL: Bug Tracker, https://github.com/noexec/curldl/issues
 Keywords: cURL,PycURL,download
```

### Comparing `curldl-1.0.0/README.md` & `curldl-1.0.1b5/README.md`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/misc/conda/test-environment.yml` & `curldl-1.0.1b5/misc/conda/test-environment.yml`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/pyproject.toml` & `curldl-1.0.1b5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/src/curldl/cli.py` & `curldl-1.0.1b5/src/curldl/cli.py`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/src/curldl/curldl.py` & `curldl-1.0.1b5/src/curldl/curldl.py`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/src/curldl/util/crypt.py` & `curldl-1.0.1b5/src/curldl/util/crypt.py`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/src/curldl/util/fs.py` & `curldl-1.0.1b5/src/curldl/util/fs.py`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/src/curldl/util/log.py` & `curldl-1.0.1b5/src/curldl/util/log.py`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/src/curldl/util/time.py` & `curldl-1.0.1b5/src/curldl/util/time.py`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/src/curldl.egg-info/PKG-INFO` & `curldl-1.0.1b5/src/curldl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curldl
-Version: 1.0.0
+Version: 1.0.1b5
 Summary: Safely and reliably download files with PycURL
 Author-email: Michael Orlov <orlovm@noexec.org>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://github.com/noexec/curldl
 Project-URL: Documentation, https://pypi.org/project/curldl/
 Project-URL: Bug Tracker, https://github.com/noexec/curldl/issues
 Keywords: cURL,PycURL,download
```

### Comparing `curldl-1.0.0/src/curldl.egg-info/SOURCES.txt` & `curldl-1.0.1b5/src/curldl.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .editorconfig
 LICENSE.md
 README.md
 pyproject.toml
 venv.sh
+.github/workflows/tests.yml
+misc/github
 misc/conda/test-environment.yml
 misc/scripts/run-bandit.sh
 misc/scripts/run-mypy.sh
 misc/scripts/run-pylint.sh
 src/curldl/__init__.py
 src/curldl/__main__.py
 src/curldl/_version.py
```

### Comparing `curldl-1.0.0/tests/functional/test_cli.py` & `curldl-1.0.1b5/tests/functional/test_cli.py`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/tests/functional/test_curldl.py` & `curldl-1.0.1b5/tests/functional/test_curldl.py`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/tests/unit/test_crypt.py` & `curldl-1.0.1b5/tests/unit/test_crypt.py`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/tests/unit/test_curldl.py` & `curldl-1.0.1b5/tests/unit/test_curldl.py`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/tests/unit/test_fs.py` & `curldl-1.0.1b5/tests/unit/test_fs.py`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/tests/unit/test_log.py` & `curldl-1.0.1b5/tests/unit/test_log.py`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/tests/unit/test_time.py` & `curldl-1.0.1b5/tests/unit/test_time.py`

 * *Files identical despite different names*

### Comparing `curldl-1.0.0/venv.sh` & `curldl-1.0.1b5/venv.sh`

 * *Files identical despite different names*

