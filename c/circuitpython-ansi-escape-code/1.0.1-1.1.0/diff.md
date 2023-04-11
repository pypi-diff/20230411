# Comparing `tmp/circuitpython-ansi-escape-code-1.0.1.tar.gz` & `tmp/circuitpython-ansi-escape-code-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-ansi-escape-code-1.0.1.tar", last modified: Thu Jan  6 07:30:59 2022, max compression
+gzip compressed data, was "circuitpython-ansi-escape-code-1.1.0.tar", last modified: Tue Apr 11 09:37:38 2023, max compression
```

## Comparing `circuitpython-ansi-escape-code-1.0.1.tar` & `circuitpython-ansi-escape-code-1.1.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 07:30:59.414582 circuitpython-ansi-escape-code-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 07:30:59.410582 circuitpython-ansi-escape-code-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 07:30:59.410582 circuitpython-ansi-escape-code-1.0.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 07:30:59.410582 circuitpython-ansi-escape-code-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2632 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2894 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16271 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6717 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 07:30:59.410582 circuitpython-ansi-escape-code-1.0.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4001 2022-01-06 07:30:59.410582 circuitpython-ansi-escape-code-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3247 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)    12017 2022-01-06 07:30:56.000000 circuitpython-ansi-escape-code-1.0.1/ansi_escape_code.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 07:30:59.410582 circuitpython-ansi-escape-code-1.0.1/circuitpython_ansi_escape_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4001 2022-01-06 07:30:59.000000 circuitpython-ansi-escape-code-1.0.1/circuitpython_ansi_escape_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-01-06 07:30:59.000000 circuitpython-ansi-escape-code-1.0.1/circuitpython_ansi_escape_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-06 07:30:59.000000 circuitpython-ansi-escape-code-1.0.1/circuitpython_ansi_escape_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-01-06 07:30:59.000000 circuitpython-ansi-escape-code-1.0.1/circuitpython_ansi_escape_code.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-01-06 07:30:59.000000 circuitpython-ansi-escape-code-1.0.1/circuitpython_ansi_escape_code.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 07:30:59.410582 circuitpython-ansi-escape-code-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 07:30:59.410582 circuitpython-ansi-escape-code-1.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5823 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-01-06 07:30:46.000000 circuitpython-ansi-escape-code-1.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 07:30:59.410582 circuitpython-ansi-escape-code-1.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2884 2022-01-06 07:30:56.000000 circuitpython-ansi-escape-code-1.0.1/examples/ansi_escape_code__cursor_position_dev.py
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-01-06 07:30:56.000000 circuitpython-ansi-escape-code-1.0.1/examples/ansi_escape_code_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-01-06 07:30:47.000000 circuitpython-ansi-escape-code-1.0.1/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-01-06 07:30:47.000000 circuitpython-ansi-escape-code-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-01-06 07:30:47.000000 circuitpython-ansi-escape-code-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-06 07:30:59.414582 circuitpython-ansi-escape-code-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-01-06 07:30:56.000000 circuitpython-ansi-escape-code-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:37:38.261866 circuitpython-ansi-escape-code-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:37:38.249866 circuitpython-ansi-escape-code-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:37:38.253866 circuitpython-ansi-escape-code-1.1.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:37:38.257866 circuitpython-ansi-escape-code-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:37:38.257866 circuitpython-ansi-escape-code-1.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-04-11 09:37:38.261866 circuitpython-ansi-escape-code-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-04-11 09:37:33.000000 circuitpython-ansi-escape-code-1.1.0/ansi_escape_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:37:38.257866 circuitpython-ansi-escape-code-1.1.0/circuitpython_ansi_escape_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-04-11 09:37:38.000000 circuitpython-ansi-escape-code-1.1.0/circuitpython_ansi_escape_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-11 09:37:38.000000 circuitpython-ansi-escape-code-1.1.0/circuitpython_ansi_escape_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:37:38.000000 circuitpython-ansi-escape-code-1.1.0/circuitpython_ansi_escape_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 09:37:38.000000 circuitpython-ansi-escape-code-1.1.0/circuitpython_ansi_escape_code.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 09:37:38.000000 circuitpython-ansi-escape-code-1.1.0/circuitpython_ansi_escape_code.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:37:38.261866 circuitpython-ansi-escape-code-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:37:38.261866 circuitpython-ansi-escape-code-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:37:38.261866 circuitpython-ansi-escape-code-1.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-11 09:37:33.000000 circuitpython-ansi-escape-code-1.1.0/examples/ansi_escape_code__cursor_position_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-11 09:37:33.000000 circuitpython-ansi-escape-code-1.1.0/examples/ansi_escape_code_background_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-11 09:37:33.000000 circuitpython-ansi-escape-code-1.1.0/examples/ansi_escape_code_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-11 09:37:20.000000 circuitpython-ansi-escape-code-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 09:37:38.261866 circuitpython-ansi-escape-code-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-11 09:37:33.000000 circuitpython-ansi-escape-code-1.1.0/setup.py
```

### Comparing `circuitpython-ansi-escape-code-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-ansi-escape-code-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-ansi-escape-code-1.0.1/.github/workflows/build.yml` & `circuitpython-ansi-escape-code-1.1.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-ansi-escape-code-1.0.1/.github/workflows/release.yml` & `circuitpython-ansi-escape-code-1.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-ansi-escape-code-1.0.1/.pre-commit-config.yaml` & `circuitpython-ansi-escape-code-1.1.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
--   repo: https://github.com/python/black
-    rev: 20.8b1
+  - repo: https://github.com/python/black
+    rev: 22.3.0
     hooks:
-    - id: black
--   repo: https://github.com/fsfe/reuse-tool
-    rev: v0.12.1
+      - id: black
+  - repo: https://github.com/fsfe/reuse-tool
+    rev: v0.14.0
     hooks:
-    - id: reuse
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
+      - id: reuse
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.2.0
     hooks:
-    -   id: check-yaml
-    -   id: end-of-file-fixer
-    -   id: trailing-whitespace
--   repo: https://github.com/pycqa/pylint
-    rev: pylint-2.7.1
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+  - repo: https://github.com/pycqa/pylint
+    rev: v2.15.5
     hooks:
-    -   id: pylint
+      - id: pylint
         name: pylint (library code)
         types: [python]
+        args:
+          - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
--   repo: local
-    hooks:
-    -   id: pylint_examples
-        name: pylint (examples code)
+      - id: pylint
+        name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
-        entry: /usr/bin/env bash -c
-        args: ['([[ ! -d "examples" ]] || for example in $(find . -path "./examples/*.py"); do pylint --disable=missing-docstring,invalid-name,consider-using-f-string $example; done)']
-        language: system
-    -   id: pylint_tests
-        name: pylint (tests code)
+        types: [python]
+        files: "^examples/"
+        args:
+          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+      - id: pylint
+        name: pylint (test code)
         description: Run pylint rules on "tests/*.py" files
-        entry: /usr/bin/env bash -c
-        args: ['([[ ! -d "tests" ]] || for test in $(find . -path "./tests/*.py"); do pylint --disable=missing-docstring $test; done)']
-        language: system
+        types: [python]
+        files: "^tests/"
+        args:
+          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `circuitpython-ansi-escape-code-1.0.1/.pylintrc` & `circuitpython-ansi-escape-code-1.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-ansi-escape-code-1.0.1/CODE_OF_CONDUCT.md` & `circuitpython-ansi-escape-code-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-ansi-escape-code-1.0.1/LICENSE` & `circuitpython-ansi-escape-code-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-ansi-escape-code-1.0.1/LICENSES/CC-BY-4.0.txt` & `circuitpython-ansi-escape-code-1.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ansi-escape-code-1.0.1/LICENSES/MIT.txt` & `circuitpython-ansi-escape-code-1.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ansi-escape-code-1.0.1/LICENSES/Unlicense.txt` & `circuitpython-ansi-escape-code-1.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ansi-escape-code-1.0.1/PKG-INFO` & `circuitpython-ansi-escape-code-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: circuitpython-ansi-escape-code
-Version: 1.0.1
+Version: 1.1.0
 Summary: simple helper library for common ANSI escape codes
 Home-page: https://github.com/s-light/CircuitPython_ansi_escape_code.git
 Author: Stefan Krüger
-Author-email: 
+Author-email: git@s-light.eu
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ansi_escape_code ansi escape code sequence terminal io cursor position color font
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
@@ -132,9 +131,7 @@
 before contributing to help this project stay welcoming.
 
 Documentation
 =============
 
 For information on building library documentation, please check out
 `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
-
```

### Comparing `circuitpython-ansi-escape-code-1.0.1/README.rst` & `circuitpython-ansi-escape-code-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-ansi-escape-code-1.0.1/ansi_escape_code.py` & `circuitpython-ansi-escape-code-1.1.0/ansi_escape_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 * Adafruit CircuitPython firmware
     `>= 7.0.0 for the supported boards. <https://github.com/adafruit/circuitpython/releases>`_
 * Python3
 * terminal with support for escape codes / sequences
     (tested with `GTKTerm <https://github.com/Jeija/gtkterm>`_)
 """
 
+__version__ = "0.0.0+auto.0"
+__repo__ = "https://github.com/s-light/CircuitPython_ansi_escape_code.git"
+
 # pylint: disable=invalid-name, too-few-public-methods
 
 # how to document on class attributes:
 # https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#directive-autoattribute
 
 import re
 import time
@@ -291,14 +294,15 @@
     ``n`` = row
     ``m`` = column
     """
 
     # device_status_report_regex = re.compile(r"XXX\[(?P<row>\d*);(?P<column>\d*)R")
     # device_status_report_regex = re.compile(r"\033\[" + r"(\d*);(\d*)R")
     device_status_report_regex = re.compile(r".\[(\d*);(\d*)R")
+    """Regex to match against the report returned by terminal."""
 
     @classmethod
     def device_status_report_parse(cls, input_string):
         """
         Parse Device Status Report. (Cursor Position Report / CPR)
 
         ``"ESC[n;mR"``
```

### Comparing `circuitpython-ansi-escape-code-1.0.1/circuitpython_ansi_escape_code.egg-info/PKG-INFO` & `circuitpython-ansi-escape-code-1.1.0/circuitpython_ansi_escape_code.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: circuitpython-ansi-escape-code
-Version: 1.0.1
+Version: 1.1.0
 Summary: simple helper library for common ANSI escape codes
 Home-page: https://github.com/s-light/CircuitPython_ansi_escape_code.git
 Author: Stefan Krüger
-Author-email: 
+Author-email: git@s-light.eu
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ansi_escape_code ansi escape code sequence terminal io cursor position color font
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
@@ -132,9 +131,7 @@
 before contributing to help this project stay welcoming.
 
 Documentation
 =============
 
 For information on building library documentation, please check out
 `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
-
```

### Comparing `circuitpython-ansi-escape-code-1.0.1/circuitpython_ansi_escape_code.egg-info/SOURCES.txt` & `circuitpython-ansi-escape-code-1.1.0/circuitpython_ansi_escape_code.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -30,8 +30,9 @@
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/ansi_escape_code__cursor_position_dev.py
+examples/ansi_escape_code_background_test.py
 examples/ansi_escape_code_simpletest.py
```

### Comparing `circuitpython-ansi-escape-code-1.0.1/docs/_static/favicon.ico` & `circuitpython-ansi-escape-code-1.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-ansi-escape-code-1.0.1/docs/conf.py` & `circuitpython-ansi-escape-code-1.1.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = [
     "_build",
     "Thumbs.db",
```

### Comparing `circuitpython-ansi-escape-code-1.0.1/docs/index.rst` & `circuitpython-ansi-escape-code-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-ansi-escape-code-1.0.1/examples/ansi_escape_code__cursor_position_dev.py` & `circuitpython-ansi-escape-code-1.1.0/examples/ansi_escape_code__cursor_position_dev.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ansi-escape-code-1.0.1/examples/ansi_escape_code_simpletest.py` & `circuitpython-ansi-escape-code-1.1.0/examples/ansi_escape_code_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ansi-escape-code-1.0.1/setup.py` & `circuitpython-ansi-escape-code-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     description="simple helper library for common ANSI escape codes",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     # The project's main homepage.
     url="https://github.com/s-light/CircuitPython_ansi_escape_code.git",
     # Author details
     author="Stefan Krüger",
-    author_email="",  # TODO: Add your email here
+    author_email="git@s-light.eu",
     install_requires=[
         "Adafruit-Blinka",
     ],
     # Choose your license
     license="MIT",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
@@ -54,11 +54,11 @@
         "Programming Language :: Python :: 3",
     ],
     # What does your project relate to?
     keywords="adafruit blinka circuitpython micropython ansi_escape_code ansi escape code "
     "sequence terminal io cursor position color font",
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
-    # TODO: IF LIBRARY FILES ARE A PACKAGE FOLDER,
+    # IF LIBRARY FILES ARE A PACKAGE FOLDER,
     #       CHANGE `py_modules=['...']` TO `packages=['...']`
     py_modules=["ansi_escape_code"],
 )
```

