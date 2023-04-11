# Comparing `tmp/python-project-structure-0.8.6b0.tar.gz` & `tmp/python-project-structure-0.8.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-project-structure-0.8.6b0.tar", last modified: Tue Apr 11 11:47:35 2023, max compression
+gzip compressed data, was "python-project-structure-0.8.7b0.tar", last modified: Tue Apr 11 20:28:28 2023, max compression
```

## Comparing `python-project-structure-0.8.6b0.tar` & `python-project-structure-0.8.7b0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.dir-locals.el.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.dockerignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.env.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.279199 python-project-structure-0.8.6b0/.github/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.283199 python-project-structure-0.8.6b0/.github/workflows/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.github/workflows/build-test.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4182 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.gitlab-ci.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.pre-commit-config.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.prospector.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/CONTRIBUTING.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/Dockerfile.devel
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/LICENSE
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    57399 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4282 2023-04-11 11:47:19.000000 python-project-structure-0.8.6b0/NEWS.rst
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/PKG-INFO
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/README.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/TODO.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.283199 python-project-structure-0.8.6b0/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/bin/cz-check-bump
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/bin/entrypoint
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/bin/get-base-version
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/bin/hadolint
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.283199 python-project-structure-0.8.6b0/build-host/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/build-host/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/build-host/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/build-host/README.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.283199 python-project-structure-0.8.6b0/build-host/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/build-host/bin/entrypoint
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/build-host/requirements-py310.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/build-host/requirements-py311.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/build-host/requirements-py37.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/build-host/requirements-py38.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/build-host/requirements-py39.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/build-host/requirements.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.283199 python-project-structure-0.8.6b0/dist/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/dist/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4400 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/docker-compose.override.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/docker-compose.yml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/home/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/home/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/home/.pypirc.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2629 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/pyproject.toml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/requirements/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/requirements/build.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/requirements/py310/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/requirements/py310/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py310/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py310/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/requirements/py311/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/requirements/py311/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py311/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py311/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/requirements/py37/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/requirements/py37/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py37/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py37/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/requirements/py38/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/requirements/py38/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py38/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py38/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/requirements/py39/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/requirements/py39/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py39/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py39/user.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-11 11:47:35.291199 python-project-structure-0.8.6b0/setup.cfg
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.279199 python-project-structure-0.8.6b0/src/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/src/python_project_structure.egg-info/
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-11 11:47:35.000000 python-project-structure-0.8.6b0/src/python_project_structure.egg-info/PKG-INFO
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1768 2023-04-11 11:47:35.000000 python-project-structure-0.8.6b0/src/python_project_structure.egg-info/SOURCES.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-11 11:47:35.000000 python-project-structure-0.8.6b0/src/python_project_structure.egg-info/dependency_links.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-11 11:47:35.000000 python-project-structure-0.8.6b0/src/python_project_structure.egg-info/entry_points.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-11 11:47:35.000000 python-project-structure-0.8.6b0/src/python_project_structure.egg-info/requires.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-11 11:47:35.000000 python-project-structure-0.8.6b0/src/python_project_structure.egg-info/top_level.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/src/pythonprojectstructure/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/src/pythonprojectstructure/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/src/pythonprojectstructure/__main__.py
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/src/pythonprojectstructure/newsfragments/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/src/pythonprojectstructure/newsfragments/.gitignore
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/src/pythonprojectstructure/tests/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/src/pythonprojectstructure/tests/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/src/pythonprojectstructure/tests/test_cli.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/src/pythonprojectstructure/utils.py
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-11 11:47:35.000000 python-project-structure-0.8.6b0/src/pythonprojectstructure/version.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/tox.ini
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.dir-locals.el.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.dockerignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.env.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.100737 python-project-structure-0.8.7b0/.github/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/.github/workflows/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.github/workflows/build-test.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4182 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.gitlab-ci.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.pre-commit-config.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.prospector.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/CONTRIBUTING.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/Dockerfile.devel
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/LICENSE
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    57399 2023-04-11 12:31:39.000000 python-project-structure-0.8.7b0/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4550 2023-04-11 20:28:12.000000 python-project-structure-0.8.7b0/NEWS.rst
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/PKG-INFO
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/README.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/TODO.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/bin/cz-check-bump
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/bin/entrypoint
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/bin/get-base-version
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/bin/hadolint
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/build-host/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/build-host/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/build-host/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/build-host/README.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/build-host/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/build-host/bin/entrypoint
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/build-host/requirements-py310.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/build-host/requirements-py311.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/build-host/requirements-py37.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/build-host/requirements-py38.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/build-host/requirements-py39.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/build-host/requirements.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/dist/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/dist/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4627 2023-04-11 12:31:39.000000 python-project-structure-0.8.7b0/docker-compose.override.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/docker-compose.yml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/home/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/home/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/home/.pypirc.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2629 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/pyproject.toml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/requirements/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/requirements/build.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/requirements/py310/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/requirements/py310/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py310/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py310/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/requirements/py311/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/requirements/py311/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py311/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py311/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/requirements/py37/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/requirements/py37/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py37/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py37/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/requirements/py38/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/requirements/py38/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py38/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py38/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/requirements/py39/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/requirements/py39/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py39/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py39/user.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/setup.cfg
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.100737 python-project-structure-0.8.7b0/src/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/src/python_project_structure.egg-info/
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-11 20:28:28.000000 python-project-structure-0.8.7b0/src/python_project_structure.egg-info/PKG-INFO
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1768 2023-04-11 20:28:28.000000 python-project-structure-0.8.7b0/src/python_project_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-11 20:28:28.000000 python-project-structure-0.8.7b0/src/python_project_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-11 20:28:28.000000 python-project-structure-0.8.7b0/src/python_project_structure.egg-info/entry_points.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-11 20:28:28.000000 python-project-structure-0.8.7b0/src/python_project_structure.egg-info/requires.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-11 20:28:28.000000 python-project-structure-0.8.7b0/src/python_project_structure.egg-info/top_level.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/src/pythonprojectstructure/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/src/pythonprojectstructure/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/src/pythonprojectstructure/__main__.py
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/src/pythonprojectstructure/newsfragments/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/src/pythonprojectstructure/newsfragments/.gitignore
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/src/pythonprojectstructure/tests/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/src/pythonprojectstructure/tests/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/src/pythonprojectstructure/tests/test_cli.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/src/pythonprojectstructure/utils.py
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-11 20:28:28.000000 python-project-structure-0.8.7b0/src/pythonprojectstructure/version.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/tox.ini
```

### Comparing `python-project-structure-0.8.6b0/.dir-locals.el.in` & `python-project-structure-0.8.7b0/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/.dockerignore` & `python-project-structure-0.8.7b0/.dockerignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/.env.in` & `python-project-structure-0.8.7b0/.env.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/.github/workflows/build-test.yml` & `python-project-structure-0.8.7b0/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/.gitignore` & `python-project-structure-0.8.7b0/.gitignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/.gitlab-ci.yml` & `python-project-structure-0.8.7b0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/.pre-commit-config.yaml` & `python-project-structure-0.8.7b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/.prospector.yaml` & `python-project-structure-0.8.7b0/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/CONTRIBUTING.rst` & `python-project-structure-0.8.7b0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/Dockerfile` & `python-project-structure-0.8.7b0/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/Dockerfile.devel` & `python-project-structure-0.8.7b0/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/LICENSE` & `python-project-structure-0.8.7b0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/Makefile` & `python-project-structure-0.8.7b0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -543,16 +543,15 @@
 endif
 endif
 
 .PHONY: test-docker-lint
 ### Check the style and content of the `./Dockerfile*` files.
 test-docker-lint: ./.env build-docker-volumes-$(PYTHON_ENV)
 	docker compose pull hadolint
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
-	    hadolint "./Dockerfile"
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
 	    hadolint "./Dockerfile.devel"
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
 	    hadolint "./build-host/Dockerfile"
 
 .PHONY: test-push
 ### Perform any checks that should only be run before pushing.
@@ -650,15 +649,15 @@
 # that a published release is never *not* reflected in VCS.  Also ensure the tag is in
 # place on any mirrors, using multiple `pushurl` remotes, for those project hosts as
 # well:
 	$(MAKE) -e test-clean
 ifeq ($(VCS_BRANCH),master)
 # Merge the bumped version back into `develop`:
 	bump_rev="$$(git rev-parse HEAD)"
-	git checkout "develop" --
+	git checkout --track "$(VCS_UPSTREAM_REMOTE)/develop" --
 	git merge --ff --gpg-sign \
 	    -m "Merge branch 'master' release back into develop" "$${bump_rev}"
 	git push --no-verify --tags "$(VCS_REMOTE)" "HEAD:develop"
 	git checkout "$${bump_rev}" --
 endif
 ifneq ($(GITHUB_ACTIONS),true)
 ifneq ($(PROJECT_GITHUB_PAT),)
```

### Comparing `python-project-structure-0.8.6b0/NEWS.rst` & `python-project-structure-0.8.7b0/NEWS.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+python-project-structure 0.8.7b0 (2023-04-11)
+=============================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
+python-project-structure 0.8.6 (2023-04-11)
+===========================================
+
+No significant changes.
+
+
 python-project-structure 0.8.6b0 (2023-04-11)
 =============================================
 
 Bugfixes
 --------
 
 - Simulate a patch release. (simulate)
```

### Comparing `python-project-structure-0.8.6b0/PKG-INFO` & `python-project-structure-0.8.7b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.6b0
+Version: 0.8.7b0
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.6b0/README.rst` & `python-project-structure-0.8.7b0/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/TODO.rst` & `python-project-structure-0.8.7b0/TODO.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/bin/cz-check-bump` & `python-project-structure-0.8.7b0/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/bin/entrypoint` & `python-project-structure-0.8.7b0/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/bin/get-base-version` & `python-project-structure-0.8.7b0/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/build-host/Dockerfile` & `python-project-structure-0.8.7b0/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/build-host/Makefile` & `python-project-structure-0.8.7b0/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/build-host/README.rst` & `python-project-structure-0.8.7b0/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/build-host/bin/entrypoint` & `python-project-structure-0.8.7b0/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/build-host/requirements-py310.txt` & `python-project-structure-0.8.7b0/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/build-host/requirements-py311.txt` & `python-project-structure-0.8.7b0/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/build-host/requirements-py37.txt` & `python-project-structure-0.8.7b0/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/build-host/requirements-py38.txt` & `python-project-structure-0.8.7b0/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/build-host/requirements-py39.txt` & `python-project-structure-0.8.7b0/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/docker-compose.override.yml` & `python-project-structure-0.8.7b0/docker-compose.override.yml`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
   ## Contianers used for development and release:
 
   # Container for use by developers:
   python-project-structure-devel:
     image: "merpatterson/python-project-structure:devel-${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
     container_name: "python-project-structure-devel"
+    profiles:
+      - "test"
     build:
       context: "${CHECKOUT_DIR}/"
       dockerfile: "${CHECKOUT_DIR}/Dockerfile.devel"
       args:
         PYTHON_MINOR: "${PYTHON_MINOR:-3.10}"
         PYTHON_ENV: "${PYTHON_ENV:-py310}"
         VERSION: "${VERSION:-}"
@@ -51,57 +53,69 @@
       - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/:/usr/local/src/python-project-structure/var/"
       - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/.tox/:/usr/local/src/python-project-structure/.tox/"
       - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/python_project_structure.egg-info/:/usr/local/src/python-project-structure/src/python_project_structure.egg-info/"
 
   # https://github.com/hadolint/hadolint#how-to-use
   hadolint:
     image: "hadolint/hadolint"
+    profiles:
+      - "test"
     environment:
       TZ: "${TZ:-Etc/UTC}"
     volumes:
       - "${CHECKOUT_DIR}/:/usr/local/src/python-project-structure/"
     working_dir: "/usr/local/src/python-project-structure/"
+    command: >-
+      hadolint "./Dockerfile"
 
   pandoc:
     image: "pandoc/core"
+    profiles:
+      - "release"
     user: "${PUID:-1000}:${PGID:-${PUID:-1000}}"
     environment:
       TZ: "${TZ:-Etc/UTC}"
     volumes:
       - "${CHECKOUT_DIR}/:/data/"
     command: >-
       "./README.rst" -f "rst" -t "markdown" -o "./README.md"
 
   docker-pushrm:
     image: "chko/docker-pushrm"
     depends_on:
       pandoc:
         condition: "service_completed_successfully"
+    profiles:
+      - "release"
     environment:
       TZ: "${TZ:-Etc/UTC}"
       DOCKER_USER: "${DOCKER_USER:-merpatterson}"
       DOCKER_PASS: "${DOCKER_PASS}"
     volumes:
       - "${CHECKOUT_DIR}/:/data/"
     command: >-
       --file "/data/README.md" --short "Python project structure foundation or template"
       --debug "merpatterson/python-project-structure"
 
   gitlab-release-cli:
     image: "registry.gitlab.com/gitlab-org/release-cli:latest"
+    profiles:
+      - "release"
     environment:
       CI_JOB_TOKEN: "${CI_JOB_TOKEN:-}"
     volumes:
       - "./:/usr/local/src/python-project-structure/"
     working_dir: "/usr/local/src/python-project-structure/"
 
   ## Containers for simulating CI/CD:
 
   build-host:
     image: "merpatterson/python-project-structure:build-host"
+    profiles:
+      - "ci"
     build: "${CHECKOUT_DIR}/build-host/"
     privileged: true
     volumes:
       - "/var/run/docker.sock:/var/run/docker.sock"
       - "${CHECKOUT_DIR}/:${CHECKOUT_DIR}"
       - "${CHECKOUT_DIR}/build-host/bin/entrypoint:/usr/local/bin/entrypoint"
       # Share local SSH authentication to repository remotes
```

### Comparing `python-project-structure-0.8.6b0/docker-compose.yml` & `python-project-structure-0.8.7b0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/pyproject.toml` & `python-project-structure-0.8.7b0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 # TEMPLATE: Update these versions to the latest version for your project and ensure the
 # tag exists both locally and on the project's remote:
 changelog_start_rev = "v0.0.0"
-version = "0.8.6b0"
+version = "0.8.7b0"
 tag_format = "v$version"
 annotated_tag = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
 """
```

### Comparing `python-project-structure-0.8.6b0/requirements/build.txt.in` & `python-project-structure-0.8.7b0/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/requirements/py310/build.txt` & `python-project-structure-0.8.7b0/requirements/py310/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/requirements/py310/devel.txt` & `python-project-structure-0.8.7b0/requirements/py310/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/requirements/py311/build.txt` & `python-project-structure-0.8.7b0/requirements/py311/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/requirements/py311/devel.txt` & `python-project-structure-0.8.7b0/requirements/py311/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/requirements/py37/build.txt` & `python-project-structure-0.8.7b0/requirements/py37/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/requirements/py37/devel.txt` & `python-project-structure-0.8.7b0/requirements/py37/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/requirements/py38/build.txt` & `python-project-structure-0.8.7b0/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/requirements/py38/devel.txt` & `python-project-structure-0.8.7b0/requirements/py38/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/requirements/py39/build.txt` & `python-project-structure-0.8.7b0/requirements/py39/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/requirements/py39/devel.txt` & `python-project-structure-0.8.7b0/requirements/py39/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/setup.cfg` & `python-project-structure-0.8.7b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/src/python_project_structure.egg-info/PKG-INFO` & `python-project-structure-0.8.7b0/src/python_project_structure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.6b0
+Version: 0.8.7b0
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.6b0/src/python_project_structure.egg-info/SOURCES.txt` & `python-project-structure-0.8.7b0/src/python_project_structure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/src/pythonprojectstructure/__init__.py` & `python-project-structure-0.8.7b0/src/pythonprojectstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/src/pythonprojectstructure/tests/test_cli.py` & `python-project-structure-0.8.7b0/src/pythonprojectstructure/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.6b0/tox.ini` & `python-project-structure-0.8.7b0/tox.ini`

 * *Files identical despite different names*

