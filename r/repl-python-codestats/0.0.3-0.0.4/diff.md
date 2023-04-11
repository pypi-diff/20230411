# Comparing `tmp/repl-python-codestats-0.0.3.tar.gz` & `tmp/repl-python-codestats-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repl-python-codestats-0.0.3.tar", last modified: Wed Jan 18 13:44:49 2023, max compression
+gzip compressed data, was "repl-python-codestats-0.0.4.tar", last modified: Tue Apr 11 17:55:16 2023, max compression
```

## Comparing `repl-python-codestats-0.0.3.tar` & `repl-python-codestats-0.0.4.tar`

### file list

```diff
@@ -1,61 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:44:49.657778 repl-python-codestats-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:44:49.653778 repl-python-codestats-0.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:44:49.653778 repl-python-codestats-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/.github/workflows/mirror.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/.gitlint
--rwxr-xr-x   0 runner    (1001) docker     (123)     2609 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/.yamlint.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-01-18 13:44:49.653778 repl-python-codestats-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:44:49.653778 repl-python-codestats-0.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:44:49.653778 repl-python-codestats-0.0.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/docs/api/python_codestats.md
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:44:49.653778 repl-python-codestats-0.0.3/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/docs/resources/requirements.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2754 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:44:49.653778 repl-python-codestats-0.0.3/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)      129 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/requirements/ipython.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      111 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/requirements/keyring.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/requirements/ptipython.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/requirements/ptpython.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:44:49.653778 repl-python-codestats-0.0.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/scripts/generate-CITATION.cff.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/scripts/generate-api.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      474 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/scripts/generate-pyproject.toml.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      179 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/scripts/generate-requirements.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-18 13:44:49.657778 repl-python-codestats-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:44:49.649778 repl-python-codestats-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:44:49.653778 repl-python-codestats-0.0.3/src/repl_python_codestats/
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/src/repl_python_codestats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-18 13:44:49.000000 repl-python-codestats-0.0.3/src/repl_python_codestats/_metainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-18 13:44:49.000000 repl-python-codestats-0.0.3/src/repl_python_codestats/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/src/repl_python_codestats/ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/src/repl_python_codestats/ptpython.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/src/repl_python_codestats/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/src/repl_python_codestats/python.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/src/repl_python_codestats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:44:49.653778 repl-python-codestats-0.0.3/src/repl_python_codestats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-01-18 13:44:49.000000 repl-python-codestats-0.0.3/src/repl_python_codestats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-01-18 13:44:49.000000 repl-python-codestats-0.0.3/src/repl_python_codestats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 13:44:49.000000 repl-python-codestats-0.0.3/src/repl_python_codestats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-18 13:44:49.000000 repl-python-codestats-0.0.3/src/repl_python_codestats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-18 13:44:49.000000 repl-python-codestats-0.0.3/src/repl_python_codestats.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:44:49.653778 repl-python-codestats-0.0.3/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:44:49.653778 repl-python-codestats-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-01-18 13:44:19.000000 repl-python-codestats-0.0.3/tests/__init___test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:55:16.781569 repl-python-codestats-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:55:16.781569 repl-python-codestats-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:55:16.781569 repl-python-codestats-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/.github/workflows/mirror.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/.yamlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-04-11 17:55:16.781569 repl-python-codestats-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:55:16.781569 repl-python-codestats-0.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:55:16.781569 repl-python-codestats-0.0.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/docs/api/python_codestats.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:55:16.781569 repl-python-codestats-0.0.4/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:55:16.781569 repl-python-codestats-0.0.4/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      142 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/requirements/ipython.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      111 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/requirements/keyring.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/requirements/ptipython.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/requirements/ptpython.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:55:16.781569 repl-python-codestats-0.0.4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/scripts/generate-api.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      179 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/scripts/generate-requirements.md.pl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:55:16.781569 repl-python-codestats-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:55:16.777569 repl-python-codestats-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:55:16.781569 repl-python-codestats-0.0.4/src/repl_python_codestats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/src/repl_python_codestats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-11 17:55:16.000000 repl-python-codestats-0.0.4/src/repl_python_codestats/_metainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 17:55:16.000000 repl-python-codestats-0.0.4/src/repl_python_codestats/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/src/repl_python_codestats/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/src/repl_python_codestats/ptpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/src/repl_python_codestats/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/src/repl_python_codestats/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/src/repl_python_codestats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:55:16.781569 repl-python-codestats-0.0.4/src/repl_python_codestats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-04-11 17:55:16.000000 repl-python-codestats-0.0.4/src/repl_python_codestats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-11 17:55:16.000000 repl-python-codestats-0.0.4/src/repl_python_codestats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:55:16.000000 repl-python-codestats-0.0.4/src/repl_python_codestats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 17:55:16.000000 repl-python-codestats-0.0.4/src/repl_python_codestats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 17:55:16.000000 repl-python-codestats-0.0.4/src/repl_python_codestats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:55:16.781569 repl-python-codestats-0.0.4/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:55:16.781569 repl-python-codestats-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-11 17:55:04.000000 repl-python-codestats-0.0.4/tests/__init___test.py
```

### Comparing `repl-python-codestats-0.0.3/.github/workflows/main.yml` & `repl-python-codestats-0.0.4/.github/workflows/main.yml`

 * *Files 10% similar despite different names*

```diff
@@ -85,7 +85,15 @@
           files: |
             dist/*
             build/resources/*
       - uses: pypa/gh-action-pypi-publish@release/v1
         if: runner.os == 'Linux' && startsWith(github.ref, 'refs/tags/')
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
+      - uses: Freed-Wu/update-aur-package@v1.0.6
+        if: startsWith(github.ref, 'refs/tags/') && runner.os == 'Linux'
+        with:
+          tag_version_prefix: ""
+          package_name: python-repl-python-codestats
+          commit_username: github-action[bot]
+          commit_email: 41898282+github-actions[bot]@users.noreply.github.com
+          ssh_private_key: ${{ secrets.AUR_SSH_PRIVATE_KEY }}
```

### Comparing `repl-python-codestats-0.0.3/.gitignore` & `repl-python-codestats-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.3/.pre-commit-config.yaml` & `repl-python-codestats-0.0.4/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env -S pre-commit run -ac
 ---
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-added-large-files
       - id: fix-byte-order-marker
@@ -19,84 +18,92 @@
       - id: debug-statements
       - id: requirements-txt-fixer
       - id: check-xml
       - id: check-yaml
       - id: check-toml
       - id: check-json
   - repo: https://github.com/Lucas-C/pre-commit-hooks
-    rev: v1.3.1
+    rev: v1.4.2
     hooks:
       - id: remove-crlf
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
         additional_dependencies:
           - tomli
   - repo: https://github.com/jorisroovers/gitlint
-    rev: v0.18.0
+    rev: v0.19.1
     hooks:
       - id: gitlint
         args:
           - --msg-filename
   - repo: https://github.com/editorconfig-checker/editorconfig-checker.python
-    rev: 2.6.2
+    rev: 2.7.1
     hooks:
       - id: editorconfig-checker
   - repo: https://github.com/jumanjihouse/pre-commit-hooks
     rev: 3.0.0
     hooks:
       - id: check-mailmap
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.28.0
+    rev: v1.30.0
     hooks:
       - id: yamllint
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
-        args:
-          - --number
         additional_dependencies:
+          - mdformat-pyproject
           - mdformat-gfm
           - mdformat-myst
           - mdformat-toc
           - mdformat-deflist
           - mdformat-beautysh
           - mdformat-black
           - mdformat-config
   - repo: https://github.com/DavidAnson/markdownlint-cli2
     rev: v0.6.0
     hooks:
       - id: markdownlint-cli2
         additional_dependencies:
           - markdown-it-texmath@0.9.1
+  - repo: https://github.com/Freed-Wu/pre-commit-hooks
+    rev: 0.0.11
+    hooks:
+      - id: update-CITATION.cff
+      - id: update-pyproject.toml
+  - repo: https://github.com/perltidy/perltidy
+    rev: "20230309.02"
+    hooks:
+      - id: perltidy
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.1.0
     hooks:
       - id: black
   - repo: https://github.com/PyCQA/isort
-    rev: 5.11.4
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/pycqa/pydocstyle
-    rev: 6.1.1
+    rev: 6.3.0
     hooks:
       - id: pydocstyle
         additional_dependencies:
-          - toml
+          - tomli
   - repo: https://github.com/kumaraditya303/mirrors-pyright
-    rev: v1.1.286
+    rev: v1.1.300
     hooks:
       - id: pyright
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - -cpyproject.toml
         additional_dependencies:
-          - toml
+          - tomli
 
 ci:
   skip:
     - pyright
```

### Comparing `repl-python-codestats-0.0.3/LICENSE` & `repl-python-codestats-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.3/PKG-INFO` & `repl-python-codestats-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repl-python-codestats
-Version: 0.0.3
+Version: 0.0.4
 Summary: A codestats plugin for python REPLs
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://repl-python-codestats.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/repl-python-codestats/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/repl-python-codestats/issues
 Project-URL: Source, https://github.com/Freed-Wu/repl-python-codestats
```

### Comparing `repl-python-codestats-0.0.3/README.md` & `repl-python-codestats-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.3/docs/conf.py` & `repl-python-codestats-0.0.4/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,7 +47,8 @@
 # a list of builtin themes.
 #
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 # html_static_path = ["_static"]
+html_favicon = "https://codestats.net/assets/frontend/favicon.ico"
```

### Comparing `repl-python-codestats-0.0.3/pyproject.toml` & `repl-python-codestats-0.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-#!/usr/bin/env -S make -B
 [build-system]
 requires = ["setuptools >= 45", "setuptools_scm[toml] >= 6.2", "setuptools-generate"]
 build-backend = "setuptools.build_meta"
 
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [project]
 name = "repl-python-codestats"
 description = "A codestats plugin for python REPLs"
-authors = [{ name = "Wu Zhenyu", email = "wuzhenyu@ustc.edu" }]
 readme = "README.md"
 requires-python = ">= 3.9"
 keywords = ["codestats", "plugin", "python", "ptpython", "ipython"]
-license = { text = "GPL v3" }
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Topic :: Software Development :: Build Tools",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX",
@@ -27,14 +24,21 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = ["version", "dependencies", "optional-dependencies"]
 
+[[project.authors]]
+name = "Wu Zhenyu"
+email = "wuzhenyu@ustc.edu"
+
+[project.license]
+text = "GPL v3"
+
 [project.urls]
 Homepage = "https://repl-python-codestats.readthedocs.io"
 Download = "https://github.com/Freed-Wu/repl-python-codestats/releases"
 "Bug Report" = "https://github.com/Freed-Wu/repl-python-codestats/issues"
 Source = "https://github.com/Freed-Wu/repl-python-codestats"
 
 [tool.setuptools.package-data]
@@ -59,14 +63,17 @@
 
 [tool.setuptools_scm]
 write_to = "src/repl_python_codestats/_version.py"
 
 [tool.setuptools-generate]
 write-to = "src/repl_python_codestats/_metainfo.py"
 
+[tool.mdformat]
+number = true
+
 [tool.black]
 line-length = 79
 
 [tool.isort]
 line_length = 79
 profile = "black"
```

### Comparing `repl-python-codestats-0.0.3/src/repl_python_codestats/__init__.py` & `repl-python-codestats-0.0.4/src/repl_python_codestats/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from urllib.request import Request, urlopen
 
 from ._version import __version__, __version_tuple__  # type: ignore
 
 logger = logging.getLogger(__name__)
 INTERVAL = 10  # interval at which stats are sent
 SLEEP_INTERVAL = 0.1  # sleep interval for timeslicing
-VERSION = "1.2.0"  # versioning
 TIMEOUT = 2  # request timeout value (in seconds)
 
 codestats = None
 
 
 def codestats_hook(
     api_key: str = "",
@@ -112,15 +111,15 @@
         self.sem.acquire()
         xp_list = [dict(language=ft, xp=xp) for ft, xp in self.xp_dict.items()]
         self.xp_dict = {self.language_type: 0}
         self.sem.release()
 
         headers = {
             "Content-Type": "application/json",
-            "User-Agent": "code-stats-python/{0}".format(VERSION),
+            "User-Agent": "code-stats-python/{0}".format(__version__),
             "X-API-Token": self.api_key,
             "Accept": "*/*",
         }
 
         # after lock is released we can send the payload
         utc_now = datetime.now().astimezone().isoformat()
         pulse_json = json.dumps(
```

### Comparing `repl-python-codestats-0.0.3/src/repl_python_codestats/_metainfo.py` & `repl-python-codestats-0.0.4/src/repl_python_codestats/_metainfo.py`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.3/src/repl_python_codestats/ipython.py` & `repl-python-codestats-0.0.4/src/repl_python_codestats/ipython.py`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.3/src/repl_python_codestats/ptpython.py` & `repl-python-codestats-0.0.4/src/repl_python_codestats/ptpython.py`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.3/src/repl_python_codestats/utils.py` & `repl-python-codestats-0.0.4/src/repl_python_codestats/utils.py`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.3/src/repl_python_codestats.egg-info/PKG-INFO` & `repl-python-codestats-0.0.4/src/repl_python_codestats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repl-python-codestats
-Version: 0.0.3
+Version: 0.0.4
 Summary: A codestats plugin for python REPLs
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://repl-python-codestats.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/repl-python-codestats/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/repl-python-codestats/issues
 Project-URL: Source, https://github.com/Freed-Wu/repl-python-codestats
```

### Comparing `repl-python-codestats-0.0.3/src/repl_python_codestats.egg-info/SOURCES.txt` & `repl-python-codestats-0.0.4/src/repl_python_codestats.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .gitignore
 .gitlint
 .pre-commit-config.yaml
 .readthedocs.yaml
 .yamlint.yaml
 CITATION.cff
 LICENSE
-Makefile
 README.md
 pyproject.toml
 requirements.txt
 .github/FUNDING.yml
 .github/workflows/main.yml
 .github/workflows/mirror.yml
 docs/conf.py
@@ -19,17 +18,15 @@
 docs/resources/install.md
 docs/resources/requirements.md
 requirements/dev.txt
 requirements/ipython.txt
 requirements/keyring.txt
 requirements/ptipython.txt
 requirements/ptpython.txt
-scripts/generate-CITATION.cff.pl
 scripts/generate-api.md.pl
-scripts/generate-pyproject.toml.pl
 scripts/generate-requirements.md.pl
 src/repl_python_codestats/__init__.py
 src/repl_python_codestats/_metainfo.py
 src/repl_python_codestats/_version.py
 src/repl_python_codestats/ipython.py
 src/repl_python_codestats/ptpython.py
 src/repl_python_codestats/py.typed
```

### Comparing `repl-python-codestats-0.0.3/tests/__init___test.py` & `repl-python-codestats-0.0.4/tests/__init___test.py`

 * *Files identical despite different names*

