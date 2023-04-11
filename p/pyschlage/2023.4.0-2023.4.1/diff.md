# Comparing `tmp/pyschlage-2023.4.0.tar.gz` & `tmp/pyschlage-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyschlage-2023.4.0.tar", last modified: Sat Apr  8 15:39:48 2023, max compression
+gzip compressed data, was "pyschlage-2023.4.1.tar", last modified: Tue Apr 11 01:06:10 2023, max compression
```

## Comparing `pyschlage-2023.4.0.tar` & `pyschlage-2023.4.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:39:48.665775 pyschlage-2023.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/.devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:39:48.653774 pyschlage-2023.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:39:48.653774 pyschlage-2023.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/.github/workflows/publish-python.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:39:48.653774 pyschlage-2023.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-08 15:39:48.665775 pyschlage-2023.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:39:48.657775 pyschlage-2023.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:39:48.661775 pyschlage-2023.4.0/pyschlage/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/pyschlage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-08 15:39:48.000000 pyschlage-2023.4.0/pyschlage/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/pyschlage/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/pyschlage/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/pyschlage/code.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/pyschlage/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/pyschlage/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/pyschlage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/pyschlage/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/pyschlage/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/pyschlage/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:39:48.661775 pyschlage-2023.4.0/pyschlage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-08 15:39:48.000000 pyschlage-2023.4.0/pyschlage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-08 15:39:48.000000 pyschlage-2023.4.0/pyschlage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 15:39:48.000000 pyschlage-2023.4.0/pyschlage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-08 15:39:48.000000 pyschlage-2023.4.0/pyschlage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-08 15:39:48.000000 pyschlage-2023.4.0/pyschlage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 15:39:48.000000 pyschlage-2023.4.0/pyschlage.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:39:48.661775 pyschlage-2023.4.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/scripts/setup
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 15:39:48.665775 pyschlage-2023.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:39:48.665775 pyschlage-2023.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-08 15:39:27.000000 pyschlage-2023.4.0/tests/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.969962 pyschlage-2023.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.965962 pyschlage-2023.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.965962 pyschlage-2023.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.github/workflows/publish-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.965962 pyschlage-2023.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-11 01:06:10.969962 pyschlage-2023.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.965962 pyschlage-2023.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.969962 pyschlage-2023.4.1/pyschlage/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 01:06:10.000000 pyschlage-2023.4.1/pyschlage/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/pyschlage/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.969962 pyschlage-2023.4.1/pyschlage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-11 01:06:10.000000 pyschlage-2023.4.1/pyschlage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-11 01:06:10.000000 pyschlage-2023.4.1/pyschlage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:06:10.000000 pyschlage-2023.4.1/pyschlage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 01:06:10.000000 pyschlage-2023.4.1/pyschlage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 01:06:10.000000 pyschlage-2023.4.1/pyschlage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:06:10.000000 pyschlage-2023.4.1/pyschlage.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.969962 pyschlage-2023.4.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/scripts/setup
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:06:10.969962 pyschlage-2023.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:06:10.969962 pyschlage-2023.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-11 01:05:54.000000 pyschlage-2023.4.1/tests/test_user.py
```

### Comparing `pyschlage-2023.4.0/.devcontainer.json` & `pyschlage-2023.4.1/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/.github/workflows/build-and-test.yml` & `pyschlage-2023.4.1/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/.github/workflows/publish-python.yml` & `pyschlage-2023.4.1/.github/workflows/publish-python.yml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/.gitignore` & `pyschlage-2023.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/.pre-commit-config.yaml` & `pyschlage-2023.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/LICENSE` & `pyschlage-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/PKG-INFO` & `pyschlage-2023.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyschlage
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Python API for interacting with Schlage WiFi locks.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pyschlage
 Project-URL: Source Code, https://github.com/dknowles2/pyschlage
 Project-URL: Bug Reports, https://github.com/dknowles2/pyschlage/issues
 Project-URL: Documentation, https://pyschlage.readthedocs.io
```

### Comparing `pyschlage-2023.4.0/README.md` & `pyschlage-2023.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/docs/Makefile` & `pyschlage-2023.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/docs/api.rst` & `pyschlage-2023.4.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/docs/index.rst` & `pyschlage-2023.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/docs/make.bat` & `pyschlage-2023.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/pyproject.toml` & `pyschlage-2023.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/pyschlage/api.py` & `pyschlage-2023.4.1/pyschlage/api.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/pyschlage/auth.py` & `pyschlage-2023.4.1/pyschlage/auth.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/pyschlage/code.py` & `pyschlage-2023.4.1/pyschlage/code.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/pyschlage/common.py` & `pyschlage-2023.4.1/pyschlage/common.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/pyschlage/device.py` & `pyschlage-2023.4.1/pyschlage/device.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/pyschlage/lock.py` & `pyschlage-2023.4.1/pyschlage/lock.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 
     Also see known device types in device.py.
     """
 
     battery_level: int | None = None
     """The remaining battery level of the lock.
 
-    This is an integer between 0 and 100.
+    This is an integer between 0 and 100 or None if lock is unavailable.
     """
 
-    is_locked: bool = False
-    """Whether the device is currently locked."""
+    is_locked: bool | None = False
+    """Whether the device is currently locked or None if lock is unavailable."""
 
-    is_jammed: bool = False
-    """Whether the lock has identified itself as jammed."""
+    is_jammed: bool | None = False
+    """Whether the lock has identified itself as jammed or None if lock is unavailable."""
 
     firmware_version: str | None = None
-    """The firmware version installed on the lock."""
+    """The firmware version installed on the lock or None if lock is unavailable."""
 
     _cat: str = ""
 
     @staticmethod
     def request_path(device_id: str | None = None) -> str:
         """Returns the request path for a Lock.
 
@@ -59,23 +59,28 @@
 
     @classmethod
     def from_json(cls, auth, json):
         """Creates a Lock from a JSON object.
 
         :meta private:
         """
+        is_locked = is_jammed = None
+        if "lockState" in json["attributes"]:
+            is_locked = json["attributes"]["lockState"] == 1
+            is_jammed = json["attributes"]["lockState"] == 2
+
         return cls(
             _auth=auth,
             device_id=json["deviceId"],
             name=json["name"],
             model_name=json["modelName"],
             device_type=json["devicetypeId"],
             battery_level=json["attributes"].get("batteryLevel"),
-            is_locked=json["attributes"]["lockState"] == 1,
-            is_jammed=json["attributes"]["lockState"] == 2,
+            is_locked=is_locked,
+            is_jammed=is_jammed,
             firmware_version=json["attributes"].get("mainFirmwareVersion"),
             _cat=json["CAT"],
         )
 
     def _is_wifi_lock(self) -> bool:
         return self.device_type.startswith("be489") or self.device_type.startswith(
             "be499"
```

### Comparing `pyschlage-2023.4.0/pyschlage/log.py` & `pyschlage-2023.4.1/pyschlage/log.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/pyschlage/user.py` & `pyschlage-2023.4.1/pyschlage/user.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/pyschlage.egg-info/PKG-INFO` & `pyschlage-2023.4.1/pyschlage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyschlage
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Python API for interacting with Schlage WiFi locks.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pyschlage
 Project-URL: Source Code, https://github.com/dknowles2/pyschlage
 Project-URL: Bug Reports, https://github.com/dknowles2/pyschlage/issues
 Project-URL: Documentation, https://pyschlage.readthedocs.io
```

### Comparing `pyschlage-2023.4.0/pyschlage.egg-info/SOURCES.txt` & `pyschlage-2023.4.1/pyschlage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/tests/conftest.py` & `pyschlage-2023.4.1/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,23 @@
         "serialNumber": "serial-number",
         "timezone": -20,
         "users": lock_users_json,
     }
 
 
 @fixture
+def wifi_lock_unavailable_json(wifi_lock_json):
+    keep = ("modelName", "serialNumber", "macAddress", "SAT", "CAT")
+    for k in list(wifi_lock_json["attributes"].keys()):
+        if k not in keep:
+            del wifi_lock_json["attributes"][k]
+    return wifi_lock_json
+
+
+@fixture
 def lock_json(wifi_lock_json):
     return wifi_lock_json
 
 
 @fixture
 def ble_lock_json(lock_users_json):
     return {
```

### Comparing `pyschlage-2023.4.0/tests/test_auth.py` & `pyschlage-2023.4.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/tests/test_code.py` & `pyschlage-2023.4.1/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.4.0/tests/test_lock.py` & `pyschlage-2023.4.1/tests/test_lock.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,32 +12,31 @@
         assert lock.device_id == "__wifi_uuid__"
         assert lock.name == "Door Lock"
         assert lock.model_name == "__model_name__"
         assert lock.device_type == "be489wifi"
         assert lock.battery_level == 95
         assert lock.is_locked
         assert lock._cat == "01234"
-        assert not lock.is_jammed
+        assert lock.is_jammed == False
         assert lock.firmware_version == "10.00.00264232"
 
     def test_from_json_is_jammed(self, mock_auth, lock_json):
         lock_json["attributes"]["lockState"] = 2
         lock = Lock.from_json(mock_auth, lock_json)
-        assert not lock.is_locked
+        assert lock.is_locked == False
         assert lock.is_jammed
 
-    def test_from_json_no_battery(self, mock_auth, lock_json):
-        del lock_json["attributes"]["batteryLevel"]
-        lock = Lock.from_json(mock_auth, lock_json)
+    def test_from_json_wifi_lock_unavailable(
+        self, mock_auth, wifi_lock_unavailable_json
+    ):
+        lock = Lock.from_json(mock_auth, wifi_lock_unavailable_json)
         assert lock.battery_level is None
-
-    def test_from_json_no_firmware_version(self, mock_auth, lock_json):
-        del lock_json["attributes"]["mainFirmwareVersion"]
-        lock = Lock.from_json(mock_auth, lock_json)
         assert lock.firmware_version is None
+        assert lock.is_locked is None
+        assert lock.is_jammed is None
 
     def test_refresh(self, mock_auth, lock_json):
         lock = Lock.from_json(mock_auth, lock_json)
         lock_json["name"] = "<NAME>"
 
         mock_auth.request.return_value = mock.Mock(
             json=mock.Mock(return_value=lock_json)
@@ -77,15 +76,15 @@
             json=mock.Mock(return_value=new_json)
         )
         lock.unlock()
 
         mock_auth.request.assert_called_once_with(
             "put", "devices/__wifi_uuid__", json={"attributes": {"lockState": 0}}
         )
-        assert not lock.is_locked
+        assert lock.is_locked == False
 
     def test_lock_ble(self, mock_auth, ble_lock_json):
         lock = Lock.from_json(mock_auth, ble_lock_json)
         lock.lock()
 
         command_json = {
             "data": {
@@ -113,15 +112,15 @@
                 "userId": "<user-id>",
             },
             "name": "changelockstate",
         }
         mock_auth.request.assert_called_once_with(
             "post", "devices/__ble_uuid__/commands", json=command_json
         )
-        assert not lock.is_locked
+        assert lock.is_locked == False
 
     def test_access_codes(self, mock_auth, lock_json, access_code_json):
         lock = Lock.from_json(mock_auth, lock_json)
 
         mock_auth.request.return_value = mock.Mock(
             json=mock.Mock(return_value=[access_code_json])
         )
```

### Comparing `pyschlage-2023.4.0/tests/test_log.py` & `pyschlage-2023.4.1/tests/test_log.py`

 * *Files identical despite different names*

