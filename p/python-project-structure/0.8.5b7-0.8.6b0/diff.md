# Comparing `tmp/python-project-structure-0.8.5b7.tar.gz` & `tmp/python-project-structure-0.8.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-project-structure-0.8.5b7.tar", last modified: Mon Apr 10 21:17:18 2023, max compression
+gzip compressed data, was "python-project-structure-0.8.6b0.tar", last modified: Tue Apr 11 11:47:35 2023, max compression
```

## Comparing `python-project-structure-0.8.5b7.tar` & `python-project-structure-0.8.6b0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.009114 python-project-structure-0.8.5b7/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.dir-locals.el.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.dockerignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.env.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:17.992112 python-project-structure-0.8.5b7/.github/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:17.998113 python-project-structure-0.8.5b7/.github/workflows/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.github/workflows/build-test.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4182 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.gitlab-ci.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.pre-commit-config.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.prospector.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/CONTRIBUTING.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/Dockerfile.devel
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/LICENSE
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    56718 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4014 2023-04-10 21:17:06.000000 python-project-structure-0.8.5b7/NEWS.rst
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-10 21:17:18.009114 python-project-structure-0.8.5b7/PKG-INFO
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/README.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/TODO.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:17.999113 python-project-structure-0.8.5b7/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/bin/cz-check-bump
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/bin/entrypoint
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/bin/get-base-version
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/bin/hadolint
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.003113 python-project-structure-0.8.5b7/build-host/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/build-host/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/build-host/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/build-host/README.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.003113 python-project-structure-0.8.5b7/build-host/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/build-host/bin/entrypoint
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/build-host/requirements-py310.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/build-host/requirements-py311.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/build-host/requirements-py37.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/build-host/requirements-py38.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/build-host/requirements-py39.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/build-host/requirements.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.003113 python-project-structure-0.8.5b7/dist/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/dist/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4400 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/docker-compose.override.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/docker-compose.yml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.004113 python-project-structure-0.8.5b7/home/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/home/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/home/.pypirc.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2629 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/pyproject.toml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.004113 python-project-structure-0.8.5b7/requirements/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/requirements/build.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.004113 python-project-structure-0.8.5b7/requirements/py310/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/requirements/py310/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py310/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py310/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.005113 python-project-structure-0.8.5b7/requirements/py311/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/requirements/py311/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py311/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py311/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.005113 python-project-structure-0.8.5b7/requirements/py37/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/requirements/py37/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py37/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py37/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.006114 python-project-structure-0.8.5b7/requirements/py38/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/requirements/py38/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py38/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py38/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.007114 python-project-structure-0.8.5b7/requirements/py39/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/requirements/py39/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py39/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py39/user.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-10 21:17:18.010114 python-project-structure-0.8.5b7/setup.cfg
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:17.994112 python-project-structure-0.8.5b7/src/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.008114 python-project-structure-0.8.5b7/src/python_project_structure.egg-info/
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-10 21:17:17.000000 python-project-structure-0.8.5b7/src/python_project_structure.egg-info/PKG-INFO
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1768 2023-04-10 21:17:17.000000 python-project-structure-0.8.5b7/src/python_project_structure.egg-info/SOURCES.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-10 21:17:17.000000 python-project-structure-0.8.5b7/src/python_project_structure.egg-info/dependency_links.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-10 21:17:17.000000 python-project-structure-0.8.5b7/src/python_project_structure.egg-info/entry_points.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-10 21:17:17.000000 python-project-structure-0.8.5b7/src/python_project_structure.egg-info/requires.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-10 21:17:17.000000 python-project-structure-0.8.5b7/src/python_project_structure.egg-info/top_level.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.008114 python-project-structure-0.8.5b7/src/pythonprojectstructure/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/src/pythonprojectstructure/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/src/pythonprojectstructure/__main__.py
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.009114 python-project-structure-0.8.5b7/src/pythonprojectstructure/newsfragments/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/src/pythonprojectstructure/newsfragments/.gitignore
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.009114 python-project-structure-0.8.5b7/src/pythonprojectstructure/tests/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/src/pythonprojectstructure/tests/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/src/pythonprojectstructure/tests/test_cli.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/src/pythonprojectstructure/utils.py
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-10 21:17:17.000000 python-project-structure-0.8.5b7/src/pythonprojectstructure/version.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/tox.ini
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.dir-locals.el.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.dockerignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.env.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.279199 python-project-structure-0.8.6b0/.github/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.283199 python-project-structure-0.8.6b0/.github/workflows/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.github/workflows/build-test.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4182 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.gitlab-ci.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.pre-commit-config.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/.prospector.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/CONTRIBUTING.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/Dockerfile.devel
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/LICENSE
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    57399 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4282 2023-04-11 11:47:19.000000 python-project-structure-0.8.6b0/NEWS.rst
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/PKG-INFO
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/README.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/TODO.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.283199 python-project-structure-0.8.6b0/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/bin/cz-check-bump
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/bin/entrypoint
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/bin/get-base-version
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/bin/hadolint
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.283199 python-project-structure-0.8.6b0/build-host/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/build-host/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/build-host/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/build-host/README.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.283199 python-project-structure-0.8.6b0/build-host/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/build-host/bin/entrypoint
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/build-host/requirements-py310.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/build-host/requirements-py311.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/build-host/requirements-py37.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/build-host/requirements-py38.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/build-host/requirements-py39.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/build-host/requirements.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.283199 python-project-structure-0.8.6b0/dist/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/dist/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4400 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/docker-compose.override.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/docker-compose.yml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/home/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/home/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/home/.pypirc.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2629 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/pyproject.toml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/requirements/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/requirements/build.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/requirements/py310/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/requirements/py310/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py310/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py310/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/requirements/py311/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/requirements/py311/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py311/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py311/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/requirements/py37/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/requirements/py37/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py37/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py37/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/requirements/py38/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/requirements/py38/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py38/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py38/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/requirements/py39/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/requirements/py39/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py39/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 11:47:22.000000 python-project-structure-0.8.6b0/requirements/py39/user.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-11 11:47:35.291199 python-project-structure-0.8.6b0/setup.cfg
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.279199 python-project-structure-0.8.6b0/src/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/src/python_project_structure.egg-info/
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-11 11:47:35.000000 python-project-structure-0.8.6b0/src/python_project_structure.egg-info/PKG-INFO
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1768 2023-04-11 11:47:35.000000 python-project-structure-0.8.6b0/src/python_project_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-11 11:47:35.000000 python-project-structure-0.8.6b0/src/python_project_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-11 11:47:35.000000 python-project-structure-0.8.6b0/src/python_project_structure.egg-info/entry_points.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-11 11:47:35.000000 python-project-structure-0.8.6b0/src/python_project_structure.egg-info/requires.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-11 11:47:35.000000 python-project-structure-0.8.6b0/src/python_project_structure.egg-info/top_level.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/src/pythonprojectstructure/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/src/pythonprojectstructure/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/src/pythonprojectstructure/__main__.py
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/src/pythonprojectstructure/newsfragments/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/src/pythonprojectstructure/newsfragments/.gitignore
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 11:47:35.287199 python-project-structure-0.8.6b0/src/pythonprojectstructure/tests/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/src/pythonprojectstructure/tests/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/src/pythonprojectstructure/tests/test_cli.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/src/pythonprojectstructure/utils.py
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-11 11:47:35.000000 python-project-structure-0.8.6b0/src/pythonprojectstructure/version.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-11 11:32:46.000000 python-project-structure-0.8.6b0/tox.ini
```

### Comparing `python-project-structure-0.8.5b7/.dir-locals.el.in` & `python-project-structure-0.8.6b0/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/.dockerignore` & `python-project-structure-0.8.6b0/.dockerignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/.env.in` & `python-project-structure-0.8.6b0/.env.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/.github/workflows/build-test.yml` & `python-project-structure-0.8.6b0/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/.gitignore` & `python-project-structure-0.8.6b0/.gitignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/.gitlab-ci.yml` & `python-project-structure-0.8.6b0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/.pre-commit-config.yaml` & `python-project-structure-0.8.6b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/.prospector.yaml` & `python-project-structure-0.8.6b0/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/CONTRIBUTING.rst` & `python-project-structure-0.8.6b0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/Dockerfile` & `python-project-structure-0.8.6b0/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/Dockerfile.devel` & `python-project-structure-0.8.6b0/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/LICENSE` & `python-project-structure-0.8.6b0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/Makefile` & `python-project-structure-0.8.6b0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -148,16 +148,18 @@
 VCS_COMPARE_BRANCH=master
 endif
 # Assemble the targets used to avoid redundant fetches during release tasks:
 VCS_FETCH_TARGETS=./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH)
 ifneq ($(VCS_REMOTE)/$(VCS_BRANCH),$(VCS_COMPARE_REMOTE)/$(VCS_COMPARE_BRANCH))
 VCS_FETCH_TARGETS+=./var/git/refs/remotes/$(VCS_COMPARE_REMOTE)/$(VCS_COMPARE_BRANCH)
 endif
-ifeq ($(VCS_BRANCH),master)
 # Also fetch develop for merging back in the final release:
+VCS_RELEASE_FETCH_TARGETS=./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH)
+ifeq ($(VCS_BRANCH),master)
+VCS_RELEASE_FETCH_TARGETS+=./var/git/refs/remotes/$(VCS_COMPARE_REMOTE)/develop
 ifneq ($(VCS_REMOTE)/$(VCS_BRANCH),$(VCS_COMPARE_REMOTE)/develop)
 ifneq ($(VCS_COMPARE_REMOTE)/$(VCS_COMPARE_BRANCH),$(VCS_COMPARE_REMOTE)/develop)
 VCS_FETCH_TARGETS+=./var/git/refs/remotes/$(VCS_COMPARE_REMOTE)/develop
 endif
 endif
 endif
 # Determine the sequence of branches to find closes existing build artifacts, such as
@@ -609,16 +611,15 @@
 
 .PHONY: release
 ### Publish installable Python packages and container images as required by commits.
 release: release-python release-docker
 
 .PHONY: release-python
 ### Publish installable Python packages to PyPI.
-release-python: ./var/log/tox/build/build.log \
-		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
+release-python: ./var/log/tox/build/build.log $(VCS_RELEASE_FETCH_TARGETS) \
 		~/.pypirc ./.env build-docker-volumes-$(PYTHON_ENV)
 ifeq ($(VCS_BRANCH),master)
 	if ! ./.tox/build/bin/python ./bin/get-base-version $$(
 	    ./.tox/build/bin/cz version --project
 	)
 	then
 # There's no pre-release for which to publish a final release:
@@ -648,18 +649,20 @@
 # The VCS remote should reflect the release before the release is published to ensure
 # that a published release is never *not* reflected in VCS.  Also ensure the tag is in
 # place on any mirrors, using multiple `pushurl` remotes, for those project hosts as
 # well:
 	$(MAKE) -e test-clean
 ifeq ($(VCS_BRANCH),master)
 # Merge the bumped version back into `develop`:
-	git checkout "develop"
-	git merge --ff-only "master"
+	bump_rev="$$(git rev-parse HEAD)"
+	git checkout "develop" --
+	git merge --ff --gpg-sign \
+	    -m "Merge branch 'master' release back into develop" "$${bump_rev}"
 	git push --no-verify --tags "$(VCS_REMOTE)" "HEAD:develop"
-	git checkout "master"
+	git checkout "$${bump_rev}" --
 endif
 ifneq ($(GITHUB_ACTIONS),true)
 ifneq ($(PROJECT_GITHUB_PAT),)
 # Ensure the tag is available for creating the GitHub release below but push *before* to
 # GitLab to avoid a race with repository mirrorying:
 	git push --no-verify --tags "github" "HEAD:$(VCS_BRANCH)"
 endif
@@ -836,28 +839,35 @@
 # Commit the upgrade changes
 	echo "Upgrade all requirements to the latest versions as of $${now}." \
 	    >"./src/pythonprojectstructure/newsfragments/upgrade-requirements.bugfix.rst"
 	git add --update './build-host/requirements-*.txt' './requirements/*/*.txt' \
 	    "./.pre-commit-config.yaml"
 	git add \
 	    "./src/pythonprojectstructure/newsfragments/upgrade-requirements.bugfix.rst"
-	git commit --all --signoff -m \
+	git_commit_args="--all --gpg-sign"
+ifeq ($(CI),true)
+# Don't duplicate the CI run from the push below:
+	git_push_args+=" --no-verify"
+endif
+	git commit $${git_commit_args} -m \
 	    "fix(deps): Upgrade requirements latest versions"
 # Fail if upgrading left untracked files in VCS
 	$(MAKE) -e "test-clean"
+ifeq ($(CI),true)
 # Push any upgrades to the remote for review.  Specify both the ref and the expected ref
 # for `--force-with-lease=...` to support pushing to multiple mirrors/remotes via
 # multiple `pushUrl`:
 	git_push_args="--no-verify"
 	if [ "$${remote_branch_exists=true}" == "true" ]
 	then
 	    git_push_args+=" --force-with-lease=\
 	$(VCS_BRANCH)-upgrade:$(VCS_REMOTE)/$(VCS_BRANCH)-upgrade"
 	fi
 	git push $${git_push_args} "$(VCS_REMOTE)" "HEAD:$(VCS_BRANCH)-upgrade"
+endif
 
 
 ## Clean Targets:
 #
 # Recipes used to restore the checkout to initial conditions.
 
 .PHONY: clean
@@ -1210,30 +1220,41 @@
 	git config --global user.name "$(USER_FULL_NAME)"
 	git config --global user.email "$(USER_EMAIL)"
 
 ./var/log/git-remotes.log:
 ifeq ($(RELEASE_PUBLISH),true)
 	set +x
 ifneq ($(VCS_REMOTE_PUSH_URL),)
-	git remote set-url --push --add "origin" "$(VCS_REMOTE_PUSH_URL)"
+	if ! git remote get-url --push --all "origin" |
+	    grep -q -F "$(VCS_REMOTE_PUSH_URL)"
+	then
+	    git remote set-url --push --add "origin" "$(VCS_REMOTE_PUSH_URL)" |
+	        tee -a "$(@)"
+	fi
 endif
 ifneq ($(GITHUB_ACTIONS),true)
 ifneq ($(PROJECT_GITHUB_PAT),)
 # Also add a fetch remote for the `$ gh ...` CLI tool to detect:
-	git remote add "github" \
-	    "https://$(PROJECT_GITHUB_PAT)@github.com/$(CI_PROJECT_PATH).git"
+	if ! git remote get-url "github" >"/dev/null"
+	then
+	    git remote add "github" \
+	        "https://$(PROJECT_GITHUB_PAT)@github.com/$(CI_PROJECT_PATH).git" |
+	        tee -a "$(@)"
+	fi
 else ifneq ($(CI_IS_FORK),true)
 	set +x
 	echo "ERROR: PROJECT_GITHUB_PAT missing from ./.env or CI secrets"
 	false
 endif
 endif
 	set -x
 # Fail fast if there's still no push access
-	git push --no-verify --tags "origin"
+	git push --no-verify --tags "origin" | tee -a "$(@)"
+else
+	date | tee -a "$(@)"
 endif
 
 # Ensure release publishing authentication, mostly useful in automation such as CI.
 ~/.pypirc: ./home/.pypirc.in
 	$(MAKE) -e "template=$(<)" "target=$(@)" expand-template
 
 ./var/log/docker-login-DOCKER.log: ./.env
```

### Comparing `python-project-structure-0.8.5b7/NEWS.rst` & `python-project-structure-0.8.6b0/NEWS.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+python-project-structure 0.8.6b0 (2023-04-11)
+=============================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
+python-project-structure 0.8.5 (2023-04-11)
+===========================================
+
+No significant changes.
+
+
 python-project-structure 0.8.5b7 (2023-04-10)
 =============================================
 
 Bugfixes
 --------
 
 - Simulate a patch release. (simulate)
```

### Comparing `python-project-structure-0.8.5b7/PKG-INFO` & `python-project-structure-0.8.6b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.5b7
+Version: 0.8.6b0
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.5b7/README.rst` & `python-project-structure-0.8.6b0/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/TODO.rst` & `python-project-structure-0.8.6b0/TODO.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/bin/cz-check-bump` & `python-project-structure-0.8.6b0/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/bin/entrypoint` & `python-project-structure-0.8.6b0/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/bin/get-base-version` & `python-project-structure-0.8.6b0/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/build-host/Dockerfile` & `python-project-structure-0.8.6b0/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/build-host/Makefile` & `python-project-structure-0.8.6b0/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/build-host/README.rst` & `python-project-structure-0.8.6b0/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/build-host/bin/entrypoint` & `python-project-structure-0.8.6b0/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/build-host/requirements-py310.txt` & `python-project-structure-0.8.6b0/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/build-host/requirements-py311.txt` & `python-project-structure-0.8.6b0/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/build-host/requirements-py37.txt` & `python-project-structure-0.8.6b0/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/build-host/requirements-py38.txt` & `python-project-structure-0.8.6b0/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/build-host/requirements-py39.txt` & `python-project-structure-0.8.6b0/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/docker-compose.override.yml` & `python-project-structure-0.8.6b0/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/docker-compose.yml` & `python-project-structure-0.8.6b0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/pyproject.toml` & `python-project-structure-0.8.6b0/pyproject.toml`

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
-version = "0.8.5b7"
+version = "0.8.6b0"
 tag_format = "v$version"
 annotated_tag = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
 """
```

### Comparing `python-project-structure-0.8.5b7/requirements/build.txt.in` & `python-project-structure-0.8.6b0/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/requirements/py310/build.txt` & `python-project-structure-0.8.6b0/requirements/py310/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/requirements/py310/devel.txt` & `python-project-structure-0.8.6b0/requirements/py310/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/requirements/py311/build.txt` & `python-project-structure-0.8.6b0/requirements/py311/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/requirements/py311/devel.txt` & `python-project-structure-0.8.6b0/requirements/py311/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/requirements/py37/build.txt` & `python-project-structure-0.8.6b0/requirements/py37/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/requirements/py37/devel.txt` & `python-project-structure-0.8.6b0/requirements/py37/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/requirements/py38/build.txt` & `python-project-structure-0.8.6b0/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/requirements/py38/devel.txt` & `python-project-structure-0.8.6b0/requirements/py38/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/requirements/py39/build.txt` & `python-project-structure-0.8.6b0/requirements/py39/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/requirements/py39/devel.txt` & `python-project-structure-0.8.6b0/requirements/py39/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/setup.cfg` & `python-project-structure-0.8.6b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/src/python_project_structure.egg-info/PKG-INFO` & `python-project-structure-0.8.6b0/src/python_project_structure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.5b7
+Version: 0.8.6b0
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.5b7/src/python_project_structure.egg-info/SOURCES.txt` & `python-project-structure-0.8.6b0/src/python_project_structure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/src/pythonprojectstructure/__init__.py` & `python-project-structure-0.8.6b0/src/pythonprojectstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/src/pythonprojectstructure/tests/test_cli.py` & `python-project-structure-0.8.6b0/src/pythonprojectstructure/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b7/tox.ini` & `python-project-structure-0.8.6b0/tox.ini`

 * *Files identical despite different names*

