# Comparing `tmp/pepotron-0.7.0.tar.gz` & `tmp/pepotron-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepotron-0.7.0.tar", last modified: Sat Jun 18 18:29:05 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pepotron-0.7.0.tar` & `pepotron-0.8.0.tar`

### file list

```diff
@@ -1,44 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 18:29:05.782787 pepotron-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-18 18:28:38.000000 pepotron-0.7.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-06-18 18:28:38.000000 pepotron-0.7.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 18:29:05.778787 pepotron-0.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-06-18 18:28:38.000000 pepotron-0.7.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-06-18 18:28:38.000000 pepotron-0.7.0/.github/labels.yml
--rw-r--r--   0 runner    (1001) docker     (121)      797 2022-06-18 18:28:38.000000 pepotron-0.7.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 18:29:05.778787 pepotron-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-06-18 18:28:38.000000 pepotron-0.7.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-06-18 18:28:38.000000 pepotron-0.7.0/.github/workflows/labels.yml
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-06-18 18:28:38.000000 pepotron-0.7.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-06-18 18:28:38.000000 pepotron-0.7.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-06-18 18:28:38.000000 pepotron-0.7.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-06-18 18:28:38.000000 pepotron-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-06-18 18:28:38.000000 pepotron-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-06-18 18:28:38.000000 pepotron-0.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5255 2022-06-18 18:29:05.782787 pepotron-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4084 2022-06-18 18:28:38.000000 pepotron-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-06-18 18:28:38.000000 pepotron-0.7.0/RELEASING.md
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-06-18 18:28:38.000000 pepotron-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-06-18 18:29:05.782787 pepotron-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-06-18 18:28:38.000000 pepotron-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 18:29:05.778787 pepotron-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 18:29:05.782787 pepotron-0.7.0/src/pepotron/
--rw-r--r--   0 runner    (1001) docker     (121)     3390 2022-06-18 18:28:38.000000 pepotron-0.7.0/src/pepotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-06-18 18:28:38.000000 pepotron-0.7.0/src/pepotron/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1633 2022-06-18 18:28:38.000000 pepotron-0.7.0/src/pepotron/_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-06-18 18:28:38.000000 pepotron-0.7.0/src/pepotron/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 18:29:05.782787 pepotron-0.7.0/src/pepotron/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-18 18:28:38.000000 pepotron-0.7.0/src/pepotron/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-06-18 18:28:38.000000 pepotron-0.7.0/src/pepotron/scripts/run_command.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 18:29:05.782787 pepotron-0.7.0/src/pepotron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5255 2022-06-18 18:29:05.000000 pepotron-0.7.0/src/pepotron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-06-18 18:29:05.000000 pepotron-0.7.0/src/pepotron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-18 18:29:05.000000 pepotron-0.7.0/src/pepotron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-06-18 18:29:05.000000 pepotron-0.7.0/src/pepotron.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-06-18 18:29:05.000000 pepotron-0.7.0/src/pepotron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-18 18:29:05.000000 pepotron-0.7.0/src/pepotron.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-18 18:29:05.000000 pepotron-0.7.0/src/pepotron.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 18:29:05.782787 pepotron-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-18 18:28:38.000000 pepotron-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-06-18 18:28:38.000000 pepotron-0.7.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2045 2022-06-18 18:28:38.000000 pepotron-0.7.0/tests/test_pepotron.py
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-06-18 18:28:38.000000 pepotron-0.7.0/tox.ini
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pepotron-0.8.0/.coveragerc
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pepotron-0.8.0/.editorconfig
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pepotron-0.8.0/.flake8
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 pepotron-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pepotron-0.8.0/RELEASING.md
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 pepotron-0.8.0/tox.ini
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/labels.yml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/renovate.json
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 pepotron-0.8.0/src/pepotron/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pepotron-0.8.0/src/pepotron/__main__.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pepotron-0.8.0/src/pepotron/_cache.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 pepotron-0.8.0/src/pepotron/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pepotron-0.8.0/src/pepotron/scripts/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pepotron-0.8.0/src/pepotron/scripts/run_command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pepotron-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 pepotron-0.8.0/tests/test_cache.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 pepotron-0.8.0/tests/test_pepotron.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pepotron-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pepotron-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 pepotron-0.8.0/README.md
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 pepotron-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 pepotron-0.8.0/PKG-INFO
```

### Comparing `pepotron-0.7.0/.github/labels.yml` & `pepotron-0.8.0/.github/labels.yml`

 * *Files 3% similar despite different names*

```diff
@@ -45,22 +45,25 @@
   description: "In case of vulnerabilities"
   name: "changelog: Security"
 - color: fbca04
   description: "Exclude PR from release draft"
   name: "changelog: skip"
 
 # Other labels
-- color: 28a745
-  description: "To automatically merge PRs that are ready"
-  name: automerge
 - color: 0366d6
-  description: "For dependencies and dependabot"
+  description: "For dependencies"
   name: dependencies
+- color: 0052cc
+  description: "Documentation"
+  name: docs
 - color: f4660e
   description: ""
   name: Hacktoberfest
 - color: f4660e
   description: "To credit accepted Hacktoberfest PRs"
   name: hacktoberfest-accepted
+- color: d65e88
+  description: "Deploy and release"
+  name: release
 - color: fbca04
   description: "Unit tests, linting, CI, etc."
   name: testing
```

### Comparing `pepotron-0.7.0/.github/release-drafter.yml` & `pepotron-0.8.0/.github/release-drafter.yml`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,19 @@
       - "bug"
   - title: "Security"
     label: "changelog: Security"
 
 exclude-labels:
   - "changelog: skip"
 
+autolabeler:
+  - label: "changelog: skip"
+    branch:
+      - "/pre-commit-ci-update-config/"
+
 template: |
   $CHANGES
 
 version-resolver:
   major:
     labels:
       - "changelog: Removed"
```

### Comparing `pepotron-0.7.0/.github/workflows/deploy.yml` & `pepotron-0.8.0/.github/workflows/deploy.yml`

 * *Files 23% similar despite different names*

```diff
@@ -10,43 +10,41 @@
   workflow_dispatch:
 
 jobs:
   deploy:
     if: github.repository_owner == 'hugovk'
     runs-on: ubuntu-latest
 
+    permissions:
+      # IMPORTANT: this permission is mandatory for trusted publishing
+      id-token: write
+
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Set up Python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.x"
           cache: pip
-          cache-dependency-path: setup.cfg
+          cache-dependency-path: pyproject.toml
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U build twine wheel
 
       - name: Build package
         run: |
-          python setup.py --version
           python -m build
           twine check --strict dist/*
 
       - name: Publish package to PyPI
         if: github.event.action == 'published'
-        uses: pypa/gh-action-pypi-publish@master
-        with:
-          user: __token__
-          password: ${{ secrets.PYPI_API_TOKEN }}
+        uses: pypa/gh-action-pypi-publish@release/v1
 
       - name: Publish package to TestPyPI
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          user: __token__
-          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-          repository_url: https://test.pypi.org/legacy/
+          repository-url: https://test.pypi.org/legacy/
```

### Comparing `pepotron-0.7.0/.github/workflows/test.yml` & `pepotron-0.8.0/.github/workflows/test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -7,53 +7,48 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["pypy-3.8", "3.7", "3.8", "3.9", "3.10", "3.11-dev"]
+        python-version: ["pypy3.9", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12-dev"]
         os: [windows-latest, macos-latest, ubuntu-latest]
-        include:
-          # Include new variables for Codecov
-          - { codecov-flag: GHA_macOS, os: macos-latest }
-          - { codecov-flag: GHA_Ubuntu, os: ubuntu-latest }
-          - { codecov-flag: GHA_Windows, os: windows-latest }
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: pip
-          cache-dependency-path: "setup.py"
+          cache-dependency-path: pyproject.toml
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U wheel
           python -m pip install -U tox
 
       - name: Tox tests
         run: |
           tox -e py
 
       - name: Cog
-        if: matrix.python-version == '3.10' && matrix.os == 'ubuntu-latest'
+        if: matrix.python-version == '3.11' && matrix.os == 'ubuntu-latest'
         run: |
           tox -e cog
 
       - name: Upload coverage
-        uses: codecov/codecov-action@v3.1.0
+        uses: codecov/codecov-action@v3
         with:
-          flags: ${{ matrix.codecov-flag }}
+          flags: ${{ matrix.os }}
           name: ${{ matrix.os }} Python ${{ matrix.python-version }}
 
   success:
     needs: test
     runs-on: ubuntu-latest
-    name: test successful
+    name: Test successful
     steps:
       - name: Success
         run: echo Test successful
```

### Comparing `pepotron-0.7.0/.pre-commit-config.yaml` & `pepotron-0.8.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,73 @@
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.34.0
+    rev: v3.3.1
     hooks:
       - id: pyupgrade
         args: [--py37-plus]
 
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
-        args: [--target-version=py37]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
+        args: [--add-import=from __future__ import annotations]
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
+    rev: 6.0.0
     hooks:
       - id: flake8
-        additional_dependencies: [flake8-2020, flake8-implicit-str-concat]
+        additional_dependencies:
+          [flake8-2020, flake8-errmsg, flake8-implicit-str-concat]
 
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
+      - id: python-no-log-warn
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
+      - id: check-case-conflict
       - id: check-merge-conflict
+      - id: check-json
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
-  - repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v1.20.1
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: v1.2.0
     hooks:
-      - id: setup-cfg-fmt
-        args: [--max-py-version=3.11]
+      - id: mypy
+        args: [--strict, --pretty, --show-error-codes]
+        additional_dependencies:
+          [httpx, platformdirs, pytest, types-freezegun, types-python-slugify]
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.3.3
+    rev: 0.9.2
     hooks:
       - id: pyproject-fmt
 
+  - repo: https://github.com/abravalheri/validate-pyproject
+    rev: v0.12.2
+    hooks:
+      - id: validate-pyproject
+
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: 0.5.2
+    rev: 1.3.0
     hooks:
       - id: tox-ini-fmt
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v2.7.1
+    rev: v3.0.0-alpha.6
     hooks:
       - id: prettier
         args: [--prose-wrap=always, --print-width=88]
 
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `pepotron-0.7.0/LICENSE.txt` & `pepotron-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pepotron-0.7.0/PKG-INFO` & `pepotron-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 Metadata-Version: 2.1
 Name: pepotron
-Version: 0.7.0
+Version: 0.8.0
 Summary: CLI to open PEPs in your browser
-Home-page: https://github.com/hugovk/pepotron
+Project-URL: Changelog, https://github.com/hugovk/pepotron/releases
+Project-URL: Homepage, https://github.com/hugovk/pepotron
+Project-URL: Source, https://github.com/hugovk/pepotron
 Author: Hugo van Kemenade
 License: MIT
-Project-URL: Source, https://github.com/hugovk/pepotron
-Project-URL: Changelog, https://github.com/hugovk/pepotron/releases
-Keywords: pep,bpo,cli
-Classifier: Development Status :: 3 - Alpha
+License-File: LICENSE.txt
+Keywords: bpo,cli,pep
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Requires-Dist: httpx>=0.22
+Requires-Dist: importlib-metadata; python_version < '3.8'
+Requires-Dist: platformdirs
+Requires-Dist: python-slugify
+Requires-Dist: thefuzz
 Provides-Extra: tests
-License-File: LICENSE.txt
+Requires-Dist: freezegun; extra == 'tests'
+Requires-Dist: pytest; extra == 'tests'
+Requires-Dist: pytest-cov; extra == 'tests'
+Description-Content-Type: text/markdown
 
 # pepotron
 
 [![PyPI version](https://img.shields.io/pypi/v/pepotron.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/pepotron/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/pepotron.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/pepotron/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/pepotron.svg)](https://pypistats.org/packages/pepotron)
 [![Test](https://github.com/hugovk/pepotron/actions/workflows/test.yml/badge.svg)](https://github.com/hugovk/pepotron/actions)
-[![codecov](https://codecov.io/gh/hugovk/pepotron/branch/main/graph/badge.svg)](https://codecov.io/gh/hugovk/pepotron)
-[![GitHub](https://img.shields.io/github/license/hugovk/pepotron.svg)](LICENSE.txt)
+[![Codecov](https://codecov.io/gh/hugovk/pepotron/branch/main/graph/badge.svg)](https://codecov.io/gh/hugovk/pepotron)
+[![Licence](https://img.shields.io/github/license/hugovk/pepotron.svg)](LICENSE.txt)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
 CLI to open PEPs in your browser.
 
 ## Installation
 
 ### From PyPI
@@ -104,14 +113,25 @@
 52	PEP 349: Allow str() to return unicode strings
 
 https://peps.python.org/pep-0594/
 ```
 
 <!-- [[[end]]] -->
 
+### Open a PEP topic
+
+<!-- [[[cog run("pep governance") ]]] -->
+
+```console
+$ pep governance
+https://peps.python.org/topic/governance/
+```
+
+<!-- [[[end]]] -->
+
 ### Open a build preview of a python/peps PR
 
 <!-- [[[cog run("pep 594 --pr 2440") ]]] -->
 
 ```console
 $ pep 594 --pr 2440
 https://pep-previews--2440.org.readthedocs.build/pep-0594/
@@ -163,16 +183,15 @@
 ```console
 $ pep --help
 usage: pep [-h] [-u URL] [-p PR] [--clear-cache] [-n] [-v] [-V] [search ...]
 
 pepotron: CLI to open PEPs in your browser
 
 positional arguments:
-  search             PEP number, or Python version for its schedule, or words
-                     from title
+  search             PEP number, or Python version for its schedule, or words from title
 
 options:
   -h, --help         show this help message and exit
   -u URL, --url URL  Base URL for PEPs (default: https://peps.python.org)
   -p PR, --pr PR     Open preview for python/peps PR
   --clear-cache      Clear cache before running
   -n, --dry-run      Don't open in browser
```

### Comparing `pepotron-0.7.0/README.md` & `pepotron-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pepotron
 
 [![PyPI version](https://img.shields.io/pypi/v/pepotron.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/pepotron/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/pepotron.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/pepotron/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/pepotron.svg)](https://pypistats.org/packages/pepotron)
 [![Test](https://github.com/hugovk/pepotron/actions/workflows/test.yml/badge.svg)](https://github.com/hugovk/pepotron/actions)
-[![codecov](https://codecov.io/gh/hugovk/pepotron/branch/main/graph/badge.svg)](https://codecov.io/gh/hugovk/pepotron)
-[![GitHub](https://img.shields.io/github/license/hugovk/pepotron.svg)](LICENSE.txt)
+[![Codecov](https://codecov.io/gh/hugovk/pepotron/branch/main/graph/badge.svg)](https://codecov.io/gh/hugovk/pepotron)
+[![Licence](https://img.shields.io/github/license/hugovk/pepotron.svg)](LICENSE.txt)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
 CLI to open PEPs in your browser.
 
 ## Installation
 
 ### From PyPI
@@ -75,14 +75,25 @@
 52	PEP 349: Allow str() to return unicode strings
 
 https://peps.python.org/pep-0594/
 ```
 
 <!-- [[[end]]] -->
 
+### Open a PEP topic
+
+<!-- [[[cog run("pep governance") ]]] -->
+
+```console
+$ pep governance
+https://peps.python.org/topic/governance/
+```
+
+<!-- [[[end]]] -->
+
 ### Open a build preview of a python/peps PR
 
 <!-- [[[cog run("pep 594 --pr 2440") ]]] -->
 
 ```console
 $ pep 594 --pr 2440
 https://pep-previews--2440.org.readthedocs.build/pep-0594/
@@ -134,16 +145,15 @@
 ```console
 $ pep --help
 usage: pep [-h] [-u URL] [-p PR] [--clear-cache] [-n] [-v] [-V] [search ...]
 
 pepotron: CLI to open PEPs in your browser
 
 positional arguments:
-  search             PEP number, or Python version for its schedule, or words
-                     from title
+  search             PEP number, or Python version for its schedule, or words from title
 
 options:
   -h, --help         show this help message and exit
   -u URL, --url URL  Base URL for PEPs (default: https://peps.python.org)
   -p PR, --pr PR     Open preview for python/peps PR
   --clear-cache      Clear cache before running
   -n, --dry-run      Don't open in browser
```

### Comparing `pepotron-0.7.0/RELEASING.md` & `pepotron-0.8.0/RELEASING.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 - [ ] Check the tagged
       [GitHub Actions build](https://github.com/hugovk/pepotron/actions/workflows/deploy.yml)
       has deployed to [PyPI](https://pypi.org/project/pepotron/#history)
 
 - [ ] Check installation:
 
 ```bash
-pip3 uninstall -y pepotron && pip3 install -U pepotron
+pip3 uninstall -y pepotron && pip3 install -U pepotron && pep --version
 ```
```

### Comparing `pepotron-0.7.0/src/pepotron/__init__.py` & `pepotron-0.8.0/src/pepotron/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 
 from pepotron import _cache
 
 try:
     # Python 3.8+
     import importlib.metadata as importlib_metadata
 except ImportError:
-    # Python 3.7 and lower
+    # Python 3.7
     import importlib_metadata  # type: ignore
 
 __version__ = importlib_metadata.version(__name__)
 
 BASE_URL = "https://peps.python.org"
 JSON_PATH = "/api/peps.json"
 USER_AGENT = f"pepotron/{__version__}"
 
+TOPICS = ("governance", "packaging", "release", "typing")
 VERSION_TO_PEP = {
     "1.6": 160,
     "2.0": 200,
     "2.1": 226,
     "2.2": 251,
     "2.3": 283,
     "2.4": 320,
@@ -76,15 +77,15 @@
 def word_search(search: str | None) -> int:
     import json
 
     peps_file = _download_peps_json()
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", category=UserWarning)
-        from thefuzz import process
+        from thefuzz import process  # type: ignore
 
     with open(peps_file) as f:
         peps = json.load(f)
 
     # We only want to search titles
     peps = ((number, details["title"]) for number, details in peps.items())
 
@@ -102,14 +103,18 @@
     """Get PEP URL"""
     if pr:
         base_url = f"https://pep-previews--{pr}.org.readthedocs.build"
 
     result = base_url.rstrip("/")
 
     if search:
+        if search.lower() in TOPICS:
+            result += f"/topic/{search}/"
+            return result
+
         try:
             # pep 8
             number = int(search)
         except ValueError:
             try:
                 # pep 3.11
                 number = VERSION_TO_PEP[search]
```

### Comparing `pepotron-0.7.0/src/pepotron/_cache.py` & `pepotron-0.8.0/src/pepotron/_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 if TYPE_CHECKING:
     if sys.version_info >= (3, 10):
         from typing import TypeAlias
     else:
         from typing_extensions import TypeAlias
 
-PepData: TypeAlias = "dict[str, dict[str, str | None]]"
+PepData: TypeAlias = "dict[str, dict[str, str]]"
 
 CACHE_DIR = Path(user_cache_dir("pepotron"))
 
 
 def filename(url: str) -> Path:
     """yyyy-mm-dd-url-slug.json"""
     from slugify import slugify
```

### Comparing `pepotron-0.7.0/src/pepotron/cli.py` & `pepotron-0.8.0/src/pepotron/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 pepotron: CLI to open PEPs in your browser
 """
+from __future__ import annotations
+
 import argparse
 import atexit
 import logging
 
 from pepotron import BASE_URL, __version__, _cache, open_bpo, open_pep
 
 atexit.register(_cache.clear)
 
 
-def add_common_arguments(parser):
+def add_common_arguments(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
     parser.add_argument(
         "-n", "--dry-run", action="store_true", help="Don't open in browser"
     )
     parser.add_argument(
         "-v",
         "--verbose",
         action="store_const",
```

### Comparing `pepotron-0.7.0/src/pepotron/scripts/run_command.py` & `pepotron-0.8.0/src/pepotron/scripts/run_command.py`

 * *Files identical despite different names*

### Comparing `pepotron-0.7.0/tests/test_cache.py` & `pepotron-0.8.0/tests/test_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Unit tests for _cache
 """
+from __future__ import annotations
+
 import tempfile
 from pathlib import Path
 
 from freezegun import freeze_time
 
 from pepotron import _cache
```

### Comparing `pepotron-0.7.0/tests/test_pepotron.py` & `pepotron-0.8.0/tests/test_pepotron.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """
 Unit tests
 """
+from __future__ import annotations
+
 import pytest
 
 import pepotron
 
 
 @pytest.mark.parametrize(
     "search, expected_url",
     [
         ("8", "https://peps.python.org/pep-0008/"),
         ("12", "https://peps.python.org/pep-0012/"),
         ("2.7", "https://peps.python.org/pep-0373/"),
         (None, "https://peps.python.org"),
         ("dead batteries", "https://peps.python.org/pep-0594/"),
+        ("release", "https://peps.python.org/topic/release/"),
+        ("typing", "https://peps.python.org/topic/typing/"),
     ],
 )
 def test_url(search: str, expected_url: str) -> None:
     # Act
     pep_url = pepotron.pep_url(search)
     # Assert
     assert pep_url == expected_url
@@ -58,15 +62,15 @@
 @pytest.mark.parametrize(
     "search, expected_url",
     [
         ("594", "https://pep-previews--2440.org.readthedocs.build/pep-0594/"),
         (None, "https://pep-previews--2440.org.readthedocs.build"),
     ],
 )
-def test_url_pr(search, expected_url) -> None:
+def test_url_pr(search: str | None, expected_url: str) -> None:
     # Arrange
     pr = 2440
     # Act
     pep_url = pepotron.pep_url(search, pr=pr)
     # Assert
     assert pep_url == expected_url
```

