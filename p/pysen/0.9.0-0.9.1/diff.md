# Comparing `tmp/pysen-0.9.0.tar.gz` & `tmp/pysen-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysen-0.9.0.tar", last modified: Mon Mar 22 09:08:40 2021, max compression
+gzip compressed data, was "dist/pysen-0.9.1.tar", last modified: Sat Mar 27 12:05:20 2021, max compression
```

## Comparing `pysen-0.9.0.tar` & `pysen-0.9.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2021-03-22 09:08:40.000000 pysen-0.9.0/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1081 2021-03-22 09:08:32.000000 pysen-0.9.0/LICENSE
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       73 2021-03-22 09:08:32.000000 pysen-0.9.0/MANIFEST.in
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    10076 2021-03-22 09:08:40.000000 pysen-0.9.0/PKG-INFO
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     7445 2021-03-22 09:08:32.000000 pysen-0.9.0/README.md
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      830 2021-03-22 09:08:32.000000 pysen-0.9.0/pyproject.toml
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2021-03-22 09:08:40.000000 pysen-0.9.0/pysen/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2940 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/__init__.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       22 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/_version.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2970 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/black.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    10683 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/cli.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1620 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/cli_config.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1374 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/command.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1224 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/component.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2055 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/diagnostic.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      861 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/dist_version.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2408 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/dumper.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3156 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/error_lines.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      983 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/exceptions.py
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2021-03-22 09:08:40.000000 pysen-0.9.0/pysen/ext/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/ext/__init__.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3310 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/ext/black_wrapper.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3638 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/ext/flake8_wrapper.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4619 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/ext/isort_wrapper.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     7362 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/ext/mypy_wrapper.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4646 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/factory.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2595 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/flake8.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2789 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/git_utils.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3012 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/isort.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4326 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/lint_command.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     5678 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/logging_utils.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     6573 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/manifest.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1306 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/manifest_builder.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     6192 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/mypy.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1388 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/path.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      346 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/plugin.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1994 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/plugin_loader.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1497 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/process_utils.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/py.typed
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1585 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/py_module.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3026 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/py_version.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4630 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/pyproject.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    13848 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/pyproject_model.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4597 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/reporter.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4980 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/runner.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      272 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/runner_options.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     6556 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/setting.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     5650 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/setuptools.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     7332 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/source.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      137 2021-03-22 09:08:32.000000 pysen-0.9.0/pysen/types.py
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2021-03-22 09:08:40.000000 pysen-0.9.0/pysen.egg-info/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    10076 2021-03-22 09:08:39.000000 pysen-0.9.0/pysen.egg-info/PKG-INFO
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1058 2021-03-22 09:08:40.000000 pysen-0.9.0/pysen.egg-info/SOURCES.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        1 2021-03-22 09:08:39.000000 pysen-0.9.0/pysen.egg-info/dependency_links.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       41 2021-03-22 09:08:39.000000 pysen-0.9.0/pysen.egg-info/entry_points.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      259 2021-03-22 09:08:39.000000 pysen-0.9.0/pysen.egg-info/requires.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        6 2021-03-22 09:08:39.000000 pysen-0.9.0/pysen.egg-info/top_level.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      707 2021-03-22 09:08:40.000000 pysen-0.9.0/setup.cfg
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1833 2021-03-22 09:08:32.000000 pysen-0.9.0/setup.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2021-03-27 12:05:20.000000 pysen-0.9.1/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1081 2021-03-22 09:08:32.000000 pysen-0.9.1/LICENSE
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       73 2021-03-22 09:08:32.000000 pysen-0.9.1/MANIFEST.in
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    11146 2021-03-27 12:05:20.000000 pysen-0.9.1/PKG-INFO
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     8331 2021-03-27 12:04:11.000000 pysen-0.9.1/README.md
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      830 2021-03-22 09:08:32.000000 pysen-0.9.1/pyproject.toml
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2021-03-27 12:05:20.000000 pysen-0.9.1/pysen/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2940 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       22 2021-03-27 12:04:11.000000 pysen-0.9.1/pysen/_version.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2970 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/black.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    10683 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/cli.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1620 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/cli_config.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1374 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/command.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1224 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/component.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2055 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/diagnostic.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      861 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/dist_version.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2408 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/dumper.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3573 2021-03-27 12:04:11.000000 pysen-0.9.1/pysen/error_lines.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      983 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/exceptions.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2021-03-27 12:05:20.000000 pysen-0.9.1/pysen/ext/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/ext/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3310 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/ext/black_wrapper.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3638 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/ext/flake8_wrapper.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4619 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/ext/isort_wrapper.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     7362 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/ext/mypy_wrapper.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4646 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/factory.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2595 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/flake8.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2789 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/git_utils.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3012 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/isort.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4326 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/lint_command.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     5678 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/logging_utils.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     6573 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/manifest.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1306 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/manifest_builder.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     6192 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/mypy.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1388 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/path.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      346 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/plugin.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1994 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/plugin_loader.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1497 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/process_utils.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/py.typed
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1585 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/py_module.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3026 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/py_version.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4630 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/pyproject.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    13848 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/pyproject_model.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4597 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/reporter.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4980 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/runner.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      272 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/runner_options.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     6556 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/setting.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     5650 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/setuptools.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     7332 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/source.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      137 2021-03-22 09:08:32.000000 pysen-0.9.1/pysen/types.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2021-03-27 12:05:20.000000 pysen-0.9.1/pysen.egg-info/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    11146 2021-03-27 12:05:20.000000 pysen-0.9.1/pysen.egg-info/PKG-INFO
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1058 2021-03-27 12:05:20.000000 pysen-0.9.1/pysen.egg-info/SOURCES.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        1 2021-03-27 12:05:20.000000 pysen-0.9.1/pysen.egg-info/dependency_links.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       41 2021-03-27 12:05:20.000000 pysen-0.9.1/pysen.egg-info/entry_points.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      259 2021-03-27 12:05:20.000000 pysen-0.9.1/pysen.egg-info/requires.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        6 2021-03-27 12:05:20.000000 pysen-0.9.1/pysen.egg-info/top_level.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      707 2021-03-27 12:05:20.000000 pysen-0.9.1/setup.cfg
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1833 2021-03-22 09:08:32.000000 pysen-0.9.1/setup.py
```

### Comparing `pysen-0.9.0/LICENSE` & `pysen-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/PKG-INFO` & `pysen-0.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysen
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python linting made easy. Also a casual yet honorific way to address individuals who have entered an organization prior to you.
 Home-page: https://github.com/pfnet/pysen
 Author: Yuki Igarashi, Toru Ogawa, Ryo Miyajima
 Author-email: igarashi@preferred.jp, ogawa@preferred.jp, ryo@preferred.jp
 License: MIT License
 Description: # pysen
         
@@ -45,17 +45,17 @@
         ```
         
         
         ### Other installation examples
         
         ```sh
         # pipenv
-        pipenv install --dev "pysen[lint]==0.9.0"
+        pipenv install --dev "pysen[lint]==0.9.1"
         # poetry
-        poetry add -D pysen==0.9.0 -E lint
+        poetry add -D pysen==0.9.1 -E lint
         ```
         
         
         ## Quickstart: Set up linters using pysen
         
         Put the following pysen configuration to `pyproject.toml` of your python package:
         ```toml
@@ -141,14 +141,25 @@
         Then running `:make` will populate your quickfix window with errors.
         This also works with [`vim-dispatch`](https://github.com/tpope/vim-dispatch) as long as you invoke `:Make` instead of `:Dispatch` (for [this reason](https://github.com/tpope/vim-dispatch/issues/41#issuecomment-20555488))
         
         The result will look like the following:
         
         ![pysen-vim](https://github.com/pfnet/pysen/blob/main/assets/imgs/pysen_vim.gif?raw=true)
         
+        ### Emacs
+        
+        Refer to the [Compilation mode](https://www.gnu.org/software/emacs/manual/html_node/emacs/Compilation-Mode.html).
+        The following is an example hook for python.
+        ```el
+        (add-hook 'python-mode-hook
+            (lambda ()
+                (set (make-local-variable 'compile-command)
+                    (concat "pysen run_files lint --error-format gnu  " buffer-file-name))))
+        ```
+        
         ### VSCode
         
         Refer to the [example task setting](/assets/vscode/tasks.json).
         Running the task will populate your "PROBLEMS" window like so:
         
         ![pysen-vscode](https://github.com/pfnet/pysen/blob/main/assets/imgs/pysen_vscode.jpg?raw=true)
         
@@ -223,14 +234,26 @@
         $ pipenv lock --pre
         ```
         - Run all tests
         ```sh
         $ pipenv run tox
         ```
         
+        ## Contributing
+        
+        
+        This repository serves only as a mirror of our main repository on our private repository.
+        Therefore we do not plan to accept any pull requests.
+        We encourage aspiring developers to make patches on their forked repositories.
+        
+        Also, our resource limitations force us to prioritize development
+        to fulfill our corporate-specific demands.
+        As such we will keep Issues closed for the foreseeable future.
+        With a heavy heart we direct all questions, troubleshooting, feature requests and bug reports to `/dev/null`.
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pysen-0.9.0/README.md` & `pysen-0.9.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 ```
 
 
 ### Other installation examples
 
 ```sh
 # pipenv
-pipenv install --dev "pysen[lint]==0.9.0"
+pipenv install --dev "pysen[lint]==0.9.1"
 # poetry
-poetry add -D pysen==0.9.0 -E lint
+poetry add -D pysen==0.9.1 -E lint
 ```
 
 
 ## Quickstart: Set up linters using pysen
 
 Put the following pysen configuration to `pyproject.toml` of your python package:
 ```toml
@@ -133,14 +133,25 @@
 Then running `:make` will populate your quickfix window with errors.
 This also works with [`vim-dispatch`](https://github.com/tpope/vim-dispatch) as long as you invoke `:Make` instead of `:Dispatch` (for [this reason](https://github.com/tpope/vim-dispatch/issues/41#issuecomment-20555488))
 
 The result will look like the following:
 
 ![pysen-vim](https://github.com/pfnet/pysen/blob/main/assets/imgs/pysen_vim.gif?raw=true)
 
+### Emacs
+
+Refer to the [Compilation mode](https://www.gnu.org/software/emacs/manual/html_node/emacs/Compilation-Mode.html).
+The following is an example hook for python.
+```el
+(add-hook 'python-mode-hook
+    (lambda ()
+        (set (make-local-variable 'compile-command)
+            (concat "pysen run_files lint --error-format gnu  " buffer-file-name))))
+```
+
 ### VSCode
 
 Refer to the [example task setting](/assets/vscode/tasks.json).
 Running the task will populate your "PROBLEMS" window like so:
 
 ![pysen-vscode](https://github.com/pfnet/pysen/blob/main/assets/imgs/pysen_vscode.jpg?raw=true)
 
@@ -214,7 +225,19 @@
 ```sh
 $ pipenv lock --pre
 ```
 - Run all tests
 ```sh
 $ pipenv run tox
 ```
+
+## Contributing
+
+
+This repository serves only as a mirror of our main repository on our private repository.
+Therefore we do not plan to accept any pull requests.
+We encourage aspiring developers to make patches on their forked repositories.
+
+Also, our resource limitations force us to prioritize development
+to fulfill our corporate-specific demands.
+As such we will keep Issues closed for the foreseeable future.
+With a heavy heart we direct all questions, troubleshooting, feature requests and bug reports to `/dev/null`.
```

### Comparing `pysen-0.9.0/pyproject.toml` & `pysen-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/__init__.py` & `pysen-0.9.1/pysen/__init__.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/black.py` & `pysen-0.9.1/pysen/black.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/cli.py` & `pysen-0.9.1/pysen/cli.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/cli_config.py` & `pysen-0.9.1/pysen/cli_config.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/command.py` & `pysen-0.9.1/pysen/command.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/component.py` & `pysen-0.9.1/pysen/component.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/diagnostic.py` & `pysen-0.9.1/pysen/diagnostic.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/dist_version.py` & `pysen-0.9.1/pysen/dist_version.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/dumper.py` & `pysen-0.9.1/pysen/dumper.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/error_lines.py` & `pysen-0.9.1/pysen/error_lines.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import re
 from pathlib import Path
-from typing import Callable, Iterable, Optional
+from typing import Callable, Generator, Iterable, Optional
 
 import unidiff
 
 from pysen.diagnostic import Diagnostic
 from pysen.exceptions import UnexpectedErrorFormat
 
 FilePathParserType = Callable[[str], Path]
@@ -86,14 +86,24 @@
 
             try:
                 file_path = file_path_parser(patch.source_file)
             except UnexpectedErrorFormat:
                 _warn_parse_error(patch, logger)
                 continue
 
+            def filter_hunk(
+                hunk: unidiff.patch.Hunk,
+            ) -> Generator[unidiff.patch.Line, None, None]:
+                for line in hunk:
+                    if _is_changed(line):
+                        yield line
+                    elif line.source_line_no is not None:
+                        if start_line <= line.source_line_no <= end_line:
+                            yield line
+
             yield Diagnostic(
                 start_line=start_line,
                 end_line=end_line,
                 start_column=1,
                 file_path=file_path,
-                diff="".join(map(str, filter(_is_changed, hunk))),
+                diff="".join(map(str, filter_hunk(hunk))),
             )
```

### Comparing `pysen-0.9.0/pysen/exceptions.py` & `pysen-0.9.1/pysen/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/ext/black_wrapper.py` & `pysen-0.9.1/pysen/ext/black_wrapper.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/ext/flake8_wrapper.py` & `pysen-0.9.1/pysen/ext/flake8_wrapper.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/ext/isort_wrapper.py` & `pysen-0.9.1/pysen/ext/isort_wrapper.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/ext/mypy_wrapper.py` & `pysen-0.9.1/pysen/ext/mypy_wrapper.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/factory.py` & `pysen-0.9.1/pysen/factory.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/flake8.py` & `pysen-0.9.1/pysen/flake8.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/git_utils.py` & `pysen-0.9.1/pysen/git_utils.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/isort.py` & `pysen-0.9.1/pysen/isort.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/lint_command.py` & `pysen-0.9.1/pysen/lint_command.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/logging_utils.py` & `pysen-0.9.1/pysen/logging_utils.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/manifest.py` & `pysen-0.9.1/pysen/manifest.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/manifest_builder.py` & `pysen-0.9.1/pysen/manifest_builder.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/mypy.py` & `pysen-0.9.1/pysen/mypy.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/path.py` & `pysen-0.9.1/pysen/path.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/plugin_loader.py` & `pysen-0.9.1/pysen/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/process_utils.py` & `pysen-0.9.1/pysen/process_utils.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/py_module.py` & `pysen-0.9.1/pysen/py_module.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/py_version.py` & `pysen-0.9.1/pysen/py_version.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/pyproject.py` & `pysen-0.9.1/pysen/pyproject.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/pyproject_model.py` & `pysen-0.9.1/pysen/pyproject_model.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/reporter.py` & `pysen-0.9.1/pysen/reporter.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/runner.py` & `pysen-0.9.1/pysen/runner.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/setting.py` & `pysen-0.9.1/pysen/setting.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/setuptools.py` & `pysen-0.9.1/pysen/setuptools.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen/source.py` & `pysen-0.9.1/pysen/source.py`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/pysen.egg-info/PKG-INFO` & `pysen-0.9.1/pysen.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysen
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python linting made easy. Also a casual yet honorific way to address individuals who have entered an organization prior to you.
 Home-page: https://github.com/pfnet/pysen
 Author: Yuki Igarashi, Toru Ogawa, Ryo Miyajima
 Author-email: igarashi@preferred.jp, ogawa@preferred.jp, ryo@preferred.jp
 License: MIT License
 Description: # pysen
         
@@ -45,17 +45,17 @@
         ```
         
         
         ### Other installation examples
         
         ```sh
         # pipenv
-        pipenv install --dev "pysen[lint]==0.9.0"
+        pipenv install --dev "pysen[lint]==0.9.1"
         # poetry
-        poetry add -D pysen==0.9.0 -E lint
+        poetry add -D pysen==0.9.1 -E lint
         ```
         
         
         ## Quickstart: Set up linters using pysen
         
         Put the following pysen configuration to `pyproject.toml` of your python package:
         ```toml
@@ -141,14 +141,25 @@
         Then running `:make` will populate your quickfix window with errors.
         This also works with [`vim-dispatch`](https://github.com/tpope/vim-dispatch) as long as you invoke `:Make` instead of `:Dispatch` (for [this reason](https://github.com/tpope/vim-dispatch/issues/41#issuecomment-20555488))
         
         The result will look like the following:
         
         ![pysen-vim](https://github.com/pfnet/pysen/blob/main/assets/imgs/pysen_vim.gif?raw=true)
         
+        ### Emacs
+        
+        Refer to the [Compilation mode](https://www.gnu.org/software/emacs/manual/html_node/emacs/Compilation-Mode.html).
+        The following is an example hook for python.
+        ```el
+        (add-hook 'python-mode-hook
+            (lambda ()
+                (set (make-local-variable 'compile-command)
+                    (concat "pysen run_files lint --error-format gnu  " buffer-file-name))))
+        ```
+        
         ### VSCode
         
         Refer to the [example task setting](/assets/vscode/tasks.json).
         Running the task will populate your "PROBLEMS" window like so:
         
         ![pysen-vscode](https://github.com/pfnet/pysen/blob/main/assets/imgs/pysen_vscode.jpg?raw=true)
         
@@ -223,14 +234,26 @@
         $ pipenv lock --pre
         ```
         - Run all tests
         ```sh
         $ pipenv run tox
         ```
         
+        ## Contributing
+        
+        
+        This repository serves only as a mirror of our main repository on our private repository.
+        Therefore we do not plan to accept any pull requests.
+        We encourage aspiring developers to make patches on their forked repositories.
+        
+        Also, our resource limitations force us to prioritize development
+        to fulfill our corporate-specific demands.
+        As such we will keep Issues closed for the foreseeable future.
+        With a heavy heart we direct all questions, troubleshooting, feature requests and bug reports to `/dev/null`.
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pysen-0.9.0/pysen.egg-info/SOURCES.txt` & `pysen-0.9.1/pysen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/setup.cfg` & `pysen-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pysen-0.9.0/setup.py` & `pysen-0.9.1/setup.py`

 * *Files identical despite different names*

