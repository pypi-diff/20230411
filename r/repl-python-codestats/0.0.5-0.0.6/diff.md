# Comparing `tmp/repl-python-codestats-0.0.5.tar.gz` & `tmp/repl-python-codestats-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repl-python-codestats-0.0.5.tar", last modified: Tue Apr 11 18:12:31 2023, max compression
+gzip compressed data, was "repl-python-codestats-0.0.6.tar", last modified: Tue Apr 11 18:49:49 2023, max compression
```

## Comparing `repl-python-codestats-0.0.5.tar` & `repl-python-codestats-0.0.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:12:31.915870 repl-python-codestats-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:12:31.911870 repl-python-codestats-0.0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:12:31.911870 repl-python-codestats-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/.github/workflows/mirror.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/.yamlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-04-11 18:12:31.915870 repl-python-codestats-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:12:31.911870 repl-python-codestats-0.0.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:12:31.911870 repl-python-codestats-0.0.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/docs/api/python_codestats.md
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:12:31.911870 repl-python-codestats-0.0.5/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:12:31.911870 repl-python-codestats-0.0.5/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)      142 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/requirements/ipython.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      111 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/requirements/keyring.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/requirements/ptipython.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/requirements/ptpython.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:12:31.911870 repl-python-codestats-0.0.5/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/scripts/generate-api.md.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      179 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/scripts/generate-requirements.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:12:31.915870 repl-python-codestats-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:12:31.911870 repl-python-codestats-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:12:31.915870 repl-python-codestats-0.0.5/src/repl_python_codestats/
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/src/repl_python_codestats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-11 18:12:31.000000 repl-python-codestats-0.0.5/src/repl_python_codestats/_metainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 18:12:31.000000 repl-python-codestats-0.0.5/src/repl_python_codestats/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/src/repl_python_codestats/ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/src/repl_python_codestats/ptpython.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/src/repl_python_codestats/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/src/repl_python_codestats/python.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/src/repl_python_codestats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:12:31.915870 repl-python-codestats-0.0.5/src/repl_python_codestats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-04-11 18:12:31.000000 repl-python-codestats-0.0.5/src/repl_python_codestats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-11 18:12:31.000000 repl-python-codestats-0.0.5/src/repl_python_codestats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:12:31.000000 repl-python-codestats-0.0.5/src/repl_python_codestats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 18:12:31.000000 repl-python-codestats-0.0.5/src/repl_python_codestats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 18:12:31.000000 repl-python-codestats-0.0.5/src/repl_python_codestats.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:12:31.915870 repl-python-codestats-0.0.5/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:12:31.915870 repl-python-codestats-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-11 18:12:19.000000 repl-python-codestats-0.0.5/tests/__init___test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:49.436258 repl-python-codestats-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:49.432258 repl-python-codestats-0.0.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:49.432258 repl-python-codestats-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/.github/workflows/mirror.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/.yamlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-04-11 18:49:49.436258 repl-python-codestats-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:49.432258 repl-python-codestats-0.0.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:49.432258 repl-python-codestats-0.0.6/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/docs/api/python_codestats.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:49.432258 repl-python-codestats-0.0.6/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:49.432258 repl-python-codestats-0.0.6/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      142 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/requirements/ipython.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      111 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/requirements/keyring.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/requirements/ptipython.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/requirements/ptpython.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:49.432258 repl-python-codestats-0.0.6/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/scripts/generate-api.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      179 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/scripts/generate-requirements.md.pl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:49:49.436258 repl-python-codestats-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:49.428258 repl-python-codestats-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:49.436258 repl-python-codestats-0.0.6/src/repl_python_codestats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/src/repl_python_codestats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-11 18:49:49.000000 repl-python-codestats-0.0.6/src/repl_python_codestats/_metainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 18:49:49.000000 repl-python-codestats-0.0.6/src/repl_python_codestats/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/src/repl_python_codestats/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/src/repl_python_codestats/ptpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/src/repl_python_codestats/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/src/repl_python_codestats/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/src/repl_python_codestats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:49.436258 repl-python-codestats-0.0.6/src/repl_python_codestats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-04-11 18:49:49.000000 repl-python-codestats-0.0.6/src/repl_python_codestats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-11 18:49:49.000000 repl-python-codestats-0.0.6/src/repl_python_codestats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:49:49.000000 repl-python-codestats-0.0.6/src/repl_python_codestats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 18:49:49.000000 repl-python-codestats-0.0.6/src/repl_python_codestats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 18:49:49.000000 repl-python-codestats-0.0.6/src/repl_python_codestats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:49.436258 repl-python-codestats-0.0.6/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:49.436258 repl-python-codestats-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-11 18:49:35.000000 repl-python-codestats-0.0.6/tests/__init___test.py
```

### Comparing `repl-python-codestats-0.0.5/.github/workflows/main.yml` & `repl-python-codestats-0.0.6/.github/workflows/main.yml`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
           files: |
             dist/*
             build/resources/*
       - uses: pypa/gh-action-pypi-publish@release/v1
         if: runner.os == 'Linux' && startsWith(github.ref, 'refs/tags/')
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
-      - uses: Freed-Wu/update-aur-package@v1.0.7
+      - uses: Freed-Wu/update-aur-package@v1.0.8
         if: startsWith(github.ref, 'refs/tags/') && runner.os == 'Linux'
         with:
           tag_version_prefix: ""
           package_name: python-repl-python-codestats
           commit_username: github-action[bot]
           commit_email: 41898282+github-actions[bot]@users.noreply.github.com
           ssh_private_key: ${{ secrets.AUR_SSH_PRIVATE_KEY }}
```

### Comparing `repl-python-codestats-0.0.5/.gitignore` & `repl-python-codestats-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.5/.pre-commit-config.yaml` & `repl-python-codestats-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.5/LICENSE` & `repl-python-codestats-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.5/PKG-INFO` & `repl-python-codestats-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repl-python-codestats
-Version: 0.0.5
+Version: 0.0.6
 Summary: A codestats plugin for python REPLs
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://repl-python-codestats.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/repl-python-codestats/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/repl-python-codestats/issues
 Project-URL: Source, https://github.com/Freed-Wu/repl-python-codestats
```

### Comparing `repl-python-codestats-0.0.5/README.md` & `repl-python-codestats-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.5/docs/conf.py` & `repl-python-codestats-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.5/pyproject.toml` & `repl-python-codestats-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.5/src/repl_python_codestats/__init__.py` & `repl-python-codestats-0.0.6/src/repl_python_codestats/__init__.py`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.5/src/repl_python_codestats/_metainfo.py` & `repl-python-codestats-0.0.6/src/repl_python_codestats/_metainfo.py`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.5/src/repl_python_codestats/ipython.py` & `repl-python-codestats-0.0.6/src/repl_python_codestats/ipython.py`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.5/src/repl_python_codestats/ptpython.py` & `repl-python-codestats-0.0.6/src/repl_python_codestats/ptpython.py`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.5/src/repl_python_codestats/utils.py` & `repl-python-codestats-0.0.6/src/repl_python_codestats/utils.py`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.5/src/repl_python_codestats.egg-info/PKG-INFO` & `repl-python-codestats-0.0.6/src/repl_python_codestats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repl-python-codestats
-Version: 0.0.5
+Version: 0.0.6
 Summary: A codestats plugin for python REPLs
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://repl-python-codestats.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/repl-python-codestats/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/repl-python-codestats/issues
 Project-URL: Source, https://github.com/Freed-Wu/repl-python-codestats
```

### Comparing `repl-python-codestats-0.0.5/src/repl_python_codestats.egg-info/SOURCES.txt` & `repl-python-codestats-0.0.6/src/repl_python_codestats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `repl-python-codestats-0.0.5/tests/__init___test.py` & `repl-python-codestats-0.0.6/tests/__init___test.py`

 * *Files identical despite different names*

