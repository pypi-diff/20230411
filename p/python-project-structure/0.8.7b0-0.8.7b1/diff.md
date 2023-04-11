# Comparing `tmp/python-project-structure-0.8.7b0.tar.gz` & `tmp/python-project-structure-0.8.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-project-structure-0.8.7b0.tar", last modified: Tue Apr 11 20:28:28 2023, max compression
+gzip compressed data, was "python-project-structure-0.8.7b1.tar", last modified: Tue Apr 11 20:57:10 2023, max compression
```

## Comparing `python-project-structure-0.8.7b0.tar` & `python-project-structure-0.8.7b1.tar`

### file list

```diff
@@ -1,87 +1,91 @@
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.dir-locals.el.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.dockerignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.env.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.100737 python-project-structure-0.8.7b0/.github/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/.github/workflows/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.github/workflows/build-test.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4182 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.gitlab-ci.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.pre-commit-config.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/.prospector.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/CONTRIBUTING.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/Dockerfile.devel
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/LICENSE
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    57399 2023-04-11 12:31:39.000000 python-project-structure-0.8.7b0/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4550 2023-04-11 20:28:12.000000 python-project-structure-0.8.7b0/NEWS.rst
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/PKG-INFO
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/README.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/TODO.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/bin/cz-check-bump
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/bin/entrypoint
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/bin/get-base-version
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/bin/hadolint
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/build-host/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/build-host/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/build-host/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/build-host/README.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/build-host/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/build-host/bin/entrypoint
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/build-host/requirements-py310.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/build-host/requirements-py311.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/build-host/requirements-py37.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/build-host/requirements-py38.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/build-host/requirements-py39.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/build-host/requirements.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/dist/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/dist/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4627 2023-04-11 12:31:39.000000 python-project-structure-0.8.7b0/docker-compose.override.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/docker-compose.yml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/home/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/home/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/home/.pypirc.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2629 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/pyproject.toml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/requirements/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/requirements/build.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/requirements/py310/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/requirements/py310/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py310/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py310/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/requirements/py311/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/requirements/py311/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py311/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py311/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.104737 python-project-structure-0.8.7b0/requirements/py37/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/requirements/py37/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py37/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py37/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/requirements/py38/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/requirements/py38/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py38/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py38/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/requirements/py39/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/requirements/py39/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py39/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 20:28:14.000000 python-project-structure-0.8.7b0/requirements/py39/user.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/setup.cfg
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.100737 python-project-structure-0.8.7b0/src/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/src/python_project_structure.egg-info/
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-11 20:28:28.000000 python-project-structure-0.8.7b0/src/python_project_structure.egg-info/PKG-INFO
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1768 2023-04-11 20:28:28.000000 python-project-structure-0.8.7b0/src/python_project_structure.egg-info/SOURCES.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-11 20:28:28.000000 python-project-structure-0.8.7b0/src/python_project_structure.egg-info/dependency_links.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-11 20:28:28.000000 python-project-structure-0.8.7b0/src/python_project_structure.egg-info/entry_points.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-11 20:28:28.000000 python-project-structure-0.8.7b0/src/python_project_structure.egg-info/requires.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-11 20:28:28.000000 python-project-structure-0.8.7b0/src/python_project_structure.egg-info/top_level.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/src/pythonprojectstructure/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/src/pythonprojectstructure/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/src/pythonprojectstructure/__main__.py
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/src/pythonprojectstructure/newsfragments/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/src/pythonprojectstructure/newsfragments/.gitignore
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:28:28.108737 python-project-structure-0.8.7b0/src/pythonprojectstructure/tests/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/src/pythonprojectstructure/tests/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/src/pythonprojectstructure/tests/test_cli.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/src/pythonprojectstructure/utils.py
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-11 20:28:28.000000 python-project-structure-0.8.7b0/src/pythonprojectstructure/version.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b0/tox.ini
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.dir-locals.el.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.dockerignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.env.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.656696 python-project-structure-0.8.7b1/.github/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/.github/workflows/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.github/workflows/build-test.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4182 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.gitlab-ci.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.pre-commit-config.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.prospector.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/CONTRIBUTING.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/Dockerfile.devel
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/LICENSE
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    58038 2023-04-11 20:39:14.000000 python-project-structure-0.8.7b1/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4776 2023-04-11 20:56:55.000000 python-project-structure-0.8.7b1/NEWS.rst
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/PKG-INFO
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/README.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/TODO.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/bin/cz-check-bump
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/bin/entrypoint
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/bin/get-base-version
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/bin/hadolint
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/build-host/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/build-host/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/build-host/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/build-host/README.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/build-host/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/build-host/bin/entrypoint
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/build-host/requirements-py310.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/build-host/requirements-py311.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/build-host/requirements-py37.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/build-host/requirements-py38.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/build-host/requirements-py39.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/build-host/requirements.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/dist/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/dist/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5044 2023-04-11 20:39:14.000000 python-project-structure-0.8.7b1/docker-compose.override.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/docker-compose.yml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/gitlab-runner/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       46 2023-04-11 20:39:14.000000 python-project-structure-0.8.7b1/gitlab-runner/.gitignore
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/gitlab-runner/config/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1323 2023-04-11 20:39:14.000000 python-project-structure-0.8.7b1/gitlab-runner/config/config.toml.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/home/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/home/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/home/.pypirc.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2629 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/pyproject.toml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/requirements/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/requirements/build.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/requirements/py310/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/requirements/py310/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py310/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py310/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/requirements/py311/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/requirements/py311/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py311/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py311/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/requirements/py37/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/requirements/py37/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py37/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py37/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/requirements/py38/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/requirements/py38/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py38/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py38/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/requirements/py39/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/requirements/py39/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py39/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py39/user.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/setup.cfg
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.660696 python-project-structure-0.8.7b1/src/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/src/python_project_structure.egg-info/
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-11 20:57:10.000000 python-project-structure-0.8.7b1/src/python_project_structure.egg-info/PKG-INFO
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1829 2023-04-11 20:57:10.000000 python-project-structure-0.8.7b1/src/python_project_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-11 20:57:10.000000 python-project-structure-0.8.7b1/src/python_project_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-11 20:57:10.000000 python-project-structure-0.8.7b1/src/python_project_structure.egg-info/entry_points.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-11 20:57:10.000000 python-project-structure-0.8.7b1/src/python_project_structure.egg-info/requires.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-11 20:57:10.000000 python-project-structure-0.8.7b1/src/python_project_structure.egg-info/top_level.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/src/pythonprojectstructure/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/src/pythonprojectstructure/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/src/pythonprojectstructure/__main__.py
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/src/pythonprojectstructure/newsfragments/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/src/pythonprojectstructure/newsfragments/.gitignore
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/src/pythonprojectstructure/tests/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/src/pythonprojectstructure/tests/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/src/pythonprojectstructure/tests/test_cli.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/src/pythonprojectstructure/utils.py
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-11 20:57:10.000000 python-project-structure-0.8.7b1/src/pythonprojectstructure/version.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/tox.ini
```

### Comparing `python-project-structure-0.8.7b0/.dir-locals.el.in` & `python-project-structure-0.8.7b1/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/.dockerignore` & `python-project-structure-0.8.7b1/.dockerignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/.env.in` & `python-project-structure-0.8.7b1/.env.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/.github/workflows/build-test.yml` & `python-project-structure-0.8.7b1/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/.gitignore` & `python-project-structure-0.8.7b1/.gitignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/.gitlab-ci.yml` & `python-project-structure-0.8.7b1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/.pre-commit-config.yaml` & `python-project-structure-0.8.7b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/.prospector.yaml` & `python-project-structure-0.8.7b1/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/CONTRIBUTING.rst` & `python-project-structure-0.8.7b1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/Dockerfile` & `python-project-structure-0.8.7b1/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/Dockerfile.devel` & `python-project-structure-0.8.7b1/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/LICENSE` & `python-project-structure-0.8.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/Makefile` & `python-project-structure-0.8.7b1/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -541,15 +541,16 @@
 	false
 endif
 endif
 endif
 
 .PHONY: test-docker-lint
 ### Check the style and content of the `./Dockerfile*` files.
-test-docker-lint: ./.env build-docker-volumes-$(PYTHON_ENV)
+test-docker-lint: ./.env build-docker-volumes-$(PYTHON_ENV) \
+		./var/log/docker-login-DOCKER.log
 	docker compose pull hadolint
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
 	    hadolint "./Dockerfile.devel"
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
 	    hadolint "./build-host/Dockerfile"
 
@@ -707,14 +708,15 @@
 
 .PHONY: $(PYTHON_MINORS:%=release-docker-%)
 ### Publish the container images for one Python version to all container registry.
 $(PYTHON_MINORS:%=release-docker-%): $(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log)
 	export PYTHON_ENV="py$(subst .,,$(@:release-docker-%=%))"
 	$(MAKE) -e -j $(DOCKER_REGISTRIES:%=release-docker-registry-%)
 ifeq ($${PYTHON_ENV},$(PYTHON_LATEST_ENV))
+	$(MAKE) -e "./var/log/docker-login-DOCKER.log"
 	docker compose pull pandoc docker-pushrm
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) docker-pushrm
 endif
 
 .PHONY: $(DOCKER_REGISTRIES:%=release-docker-registry-%)
 ### Publish all container images to one container registry.
 $(DOCKER_REGISTRIES:%=release-docker-registry-%):
@@ -955,15 +957,16 @@
 		./Dockerfile.devel ./.dockerignore ./bin/entrypoint \
 		./pyproject.toml ./setup.cfg ./tox.ini \
 		./build-host/requirements.txt.in ./docker-compose.yml \
 		./docker-compose.override.yml ./.env \
 		./var/docker/$(PYTHON_ENV)/log/rebuild.log
 	true DEBUG Updated prereqs: $(?)
 	$(MAKE) -e "./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH)" \
-	    build-docker-volumes-$(PYTHON_ENV) "./var/log/tox/build/build.log"
+	    build-docker-volumes-$(PYTHON_ENV) "./var/log/tox/build/build.log" \
+	    "./var/log/docker-login-DOCKER.log"
 	mkdir -pv "$(dir $(@))"
 # Workaround issues with local images and the development image depending on the end
 # user image.  It seems that `depends_on` isn't sufficient.
 	$(MAKE) -e $(HOME)/.local/var/log/python-project-structure-host-install.log
 	export VERSION=$$(./.tox/build/bin/cz version --project)
 ifeq ($(DOCKER_BUILD_PULL),true)
 # Pull the development image and simulate as if it had been built here.
@@ -1012,15 +1015,15 @@
 	if $(MAKE) -e DOCKER_VARIANT="devel" pull-docker
 	then
 	    docker_build_caches+=" --cache-from \
 	$(DOCKER_IMAGE_GITHUB):devel-$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
 	fi
 endif
 endif
-	docker buildx build --pull $${docker_build_args} $${docker_build_devel_tags} \
+	docker buildx build $${docker_build_args} $${docker_build_devel_tags} \
 	    $${docker_build_caches} --file "./Dockerfile.devel" "./"
 # Ensure any subsequent builds have optimal caches
 ifeq ($(GITLAB_CI),true)
 	docker push \
 	    "$(DOCKER_IMAGE_GITLAB):devel-$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
 endif
 ifeq ($(GITHUB_ACTIONS),true)
@@ -1083,15 +1086,15 @@
 	if $(MAKE) -e pull-docker
 	then
 	    docker_build_caches+=" \
 	--cache-from $(DOCKER_IMAGE_GITHUB):$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
 	fi
 endif
 endif
-	docker buildx build --pull $${docker_build_args} $${docker_build_user_tags} \
+	docker buildx build $${docker_build_args} $${docker_build_user_tags} \
 	    --build-arg PYTHON_WHEEL="$${PYTHON_WHEEL}" $${docker_build_caches} "./"
 # Ensure any subsequent builds have optimal caches
 ifeq ($(GITLAB_CI),true)
 	docker push "$(DOCKER_IMAGE_GITLAB):$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
 endif
 ifeq ($(GITHUB_ACTIONS),true)
 ifneq ($(CI_IS_FORK),true)
@@ -1356,14 +1359,22 @@
 	echo "ERROR: GPG_SIGNING_PRIVATE_KEY or GPG_PASSPHRASE " \
 	    "missing from ./.env or CI secrets"
 	false
 endif
 	date | tee -a "$(@)"
 endif
 
+# TEMPLATE: Optionally, use the following command to generate a GitLab CI/CD runner
+# configuration, register it with your project, compare it with the template
+# prerequisite, apply the appropriate changes and then  run using `$ docker compose up
+# gitlab-runner`.  Particularly useful to conserve shared runner minutes:
+./gitlab-runner/config/config.toml: ./gitlab-runner/config/config.toml.in
+	docker compose run --rm gitlab-runner register \
+	    --url "https://gitlab.com/" --docker-image "docker" --executor "docker"
+
 
 ## Utility Targets:
 #
 # Recipes used to make similar changes across targets where using Make's basic syntax
 # can't be used.
 
 .PHONY: expand-template
```

### Comparing `python-project-structure-0.8.7b0/NEWS.rst` & `python-project-structure-0.8.7b1/NEWS.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+python-project-structure 0.8.7b1 (2023-04-11)
+=============================================
+
+Bugfixes
+--------
+
+- Upgrade all requirements to the latest versions as of Tue Apr 11 08:15:25 PM UTC 2023. (upgrade-requirements)
+
+
 python-project-structure 0.8.7b0 (2023-04-11)
 =============================================
 
 Bugfixes
 --------
 
 - Simulate a patch release. (simulate)
```

### Comparing `python-project-structure-0.8.7b0/PKG-INFO` & `python-project-structure-0.8.7b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.7b0
+Version: 0.8.7b1
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.7b0/README.rst` & `python-project-structure-0.8.7b1/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/TODO.rst` & `python-project-structure-0.8.7b1/TODO.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/bin/cz-check-bump` & `python-project-structure-0.8.7b1/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/bin/entrypoint` & `python-project-structure-0.8.7b1/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/bin/get-base-version` & `python-project-structure-0.8.7b1/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/build-host/Dockerfile` & `python-project-structure-0.8.7b1/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/build-host/Makefile` & `python-project-structure-0.8.7b1/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/build-host/README.rst` & `python-project-structure-0.8.7b1/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/build-host/bin/entrypoint` & `python-project-structure-0.8.7b1/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/build-host/requirements-py310.txt` & `python-project-structure-0.8.7b1/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/build-host/requirements-py311.txt` & `python-project-structure-0.8.7b1/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/build-host/requirements-py37.txt` & `python-project-structure-0.8.7b1/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/build-host/requirements-py38.txt` & `python-project-structure-0.8.7b1/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/build-host/requirements-py39.txt` & `python-project-structure-0.8.7b1/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/docker-compose.override.yml` & `python-project-structure-0.8.7b1/docker-compose.override.yml`

 * *Files 7% similar despite different names*

```diff
@@ -52,15 +52,15 @@
       # run-time.
       - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/:/usr/local/src/python-project-structure/var/"
       - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/.tox/:/usr/local/src/python-project-structure/.tox/"
       - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/python_project_structure.egg-info/:/usr/local/src/python-project-structure/src/python_project_structure.egg-info/"
 
   # https://github.com/hadolint/hadolint#how-to-use
   hadolint:
-    image: "hadolint/hadolint"
+    image: "ghcr.io/hadolint/hadolint"
     profiles:
       - "test"
     environment:
       TZ: "${TZ:-Etc/UTC}"
     volumes:
       - "${CHECKOUT_DIR}/:/usr/local/src/python-project-structure/"
     working_dir: "/usr/local/src/python-project-structure/"
@@ -102,16 +102,17 @@
       - "release"
     environment:
       CI_JOB_TOKEN: "${CI_JOB_TOKEN:-}"
     volumes:
       - "./:/usr/local/src/python-project-structure/"
     working_dir: "/usr/local/src/python-project-structure/"
 
-  ## Containers for simulating CI/CD:
+  ## Containers related to CI/CD:
 
+  # The container in which CI/CD is run:
   build-host:
     image: "merpatterson/python-project-structure:build-host"
     profiles:
       - "ci"
     build: "${CHECKOUT_DIR}/build-host/"
     privileged: true
     volumes:
@@ -125,7 +126,20 @@
       TZ: "${TZ:-Etc/UTC}"
       PUID: "${PUID:-1000}"
       PGID: "${DOCKER_GID:-${PGID:-${PUID:-1000}}}"
       # DEBUG: "true"
     working_dir: "${CHECKOUT_DIR}"
     command: >-
       make -e build-docker test-docker release
+
+  # Conserve shared runner minutes, run GitLab CI/CD jobs locally:
+  gitlab-runner:
+    image: "gitlab/gitlab-runner"
+    profiles:
+      - "ci"
+    volumes:
+      - "./gitlab-runner/config:/etc/gitlab-runner"
+      - "/var/run/docker.sock:/var/run/docker.sock"
+      - "./gitlab-runner/cache:/cache"
+      - "./gitlab-runner/certs:/certs"
+    ports:
+      - "8093:8093"
```

### Comparing `python-project-structure-0.8.7b0/docker-compose.yml` & `python-project-structure-0.8.7b1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/pyproject.toml` & `python-project-structure-0.8.7b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 # TEMPLATE: Update these versions to the latest version for your project and ensure the
 # tag exists both locally and on the project's remote:
 changelog_start_rev = "v0.0.0"
-version = "0.8.7b0"
+version = "0.8.7b1"
 tag_format = "v$version"
 annotated_tag = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
 """
```

### Comparing `python-project-structure-0.8.7b0/requirements/build.txt.in` & `python-project-structure-0.8.7b1/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/requirements/py310/build.txt` & `python-project-structure-0.8.7b1/requirements/py310/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/requirements/py310/devel.txt` & `python-project-structure-0.8.7b1/requirements/py310/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/requirements/py311/build.txt` & `python-project-structure-0.8.7b1/requirements/py311/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/requirements/py311/devel.txt` & `python-project-structure-0.8.7b1/requirements/py311/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/requirements/py37/build.txt` & `python-project-structure-0.8.7b1/requirements/py37/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/requirements/py37/devel.txt` & `python-project-structure-0.8.7b1/requirements/py37/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/requirements/py38/build.txt` & `python-project-structure-0.8.7b1/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/requirements/py38/devel.txt` & `python-project-structure-0.8.7b1/requirements/py38/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/requirements/py39/build.txt` & `python-project-structure-0.8.7b1/requirements/py39/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/requirements/py39/devel.txt` & `python-project-structure-0.8.7b1/requirements/py39/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/setup.cfg` & `python-project-structure-0.8.7b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/src/python_project_structure.egg-info/PKG-INFO` & `python-project-structure-0.8.7b1/src/python_project_structure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.7b0
+Version: 0.8.7b1
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.7b0/src/python_project_structure.egg-info/SOURCES.txt` & `python-project-structure-0.8.7b1/src/python_project_structure.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 build-host/requirements-py311.txt
 build-host/requirements-py37.txt
 build-host/requirements-py38.txt
 build-host/requirements-py39.txt
 build-host/requirements.txt.in
 build-host/bin/entrypoint
 dist/.gitignore
+gitlab-runner/.gitignore
+gitlab-runner/config/config.toml.in
 home/.gitignore
 home/.pypirc.in
 requirements/build.txt.in
 requirements/py310/build.txt
 requirements/py310/devel.txt
 requirements/py310/user.txt
 requirements/py311/build.txt
```

### Comparing `python-project-structure-0.8.7b0/src/pythonprojectstructure/__init__.py` & `python-project-structure-0.8.7b1/src/pythonprojectstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/src/pythonprojectstructure/tests/test_cli.py` & `python-project-structure-0.8.7b1/src/pythonprojectstructure/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b0/tox.ini` & `python-project-structure-0.8.7b1/tox.ini`

 * *Files identical despite different names*

