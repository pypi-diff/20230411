# Comparing `tmp/python-project-structure-0.8.5b2.tar.gz` & `tmp/python-project-structure-0.8.5b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-project-structure-0.8.5b2.tar", last modified: Mon Apr 10 20:30:04 2023, max compression
+gzip compressed data, was "python-project-structure-0.8.5b7.tar", last modified: Mon Apr 10 21:17:18 2023, max compression
```

## Comparing `python-project-structure-0.8.5b2.tar` & `python-project-structure-0.8.5b7.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.207462 python-project-structure-0.8.5b2/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/.dir-locals.el.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/.dockerignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/.env.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.192461 python-project-structure-0.8.5b2/.github/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.199461 python-project-structure-0.8.5b2/.github/workflows/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/.github/workflows/build-test.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4164 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/.gitlab-ci.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/.pre-commit-config.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/.prospector.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/CONTRIBUTING.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/Dockerfile.devel
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/LICENSE
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    56729 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3351 2023-04-10 20:29:53.000000 python-project-structure-0.8.5b2/NEWS.rst
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-10 20:30:04.207462 python-project-structure-0.8.5b2/PKG-INFO
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/README.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/TODO.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.199461 python-project-structure-0.8.5b2/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/bin/cz-check-bump
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/bin/entrypoint
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/bin/get-base-version
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/bin/hadolint
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.201462 python-project-structure-0.8.5b2/build-host/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/build-host/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/build-host/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/build-host/README.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.201462 python-project-structure-0.8.5b2/build-host/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/build-host/bin/entrypoint
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/build-host/requirements-py310.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/build-host/requirements-py311.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/build-host/requirements-py37.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/build-host/requirements-py38.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/build-host/requirements-py39.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/build-host/requirements.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.201462 python-project-structure-0.8.5b2/dist/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/dist/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4400 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/docker-compose.override.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/docker-compose.yml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.202462 python-project-structure-0.8.5b2/home/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/home/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/home/.pypirc.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2624 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/pyproject.toml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.202462 python-project-structure-0.8.5b2/requirements/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/requirements/build.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.202462 python-project-structure-0.8.5b2/requirements/py310/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/requirements/py310/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/requirements/py310/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/requirements/py310/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.203462 python-project-structure-0.8.5b2/requirements/py311/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/requirements/py311/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/requirements/py311/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/requirements/py311/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.204462 python-project-structure-0.8.5b2/requirements/py37/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/requirements/py37/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/requirements/py37/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/requirements/py37/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.204462 python-project-structure-0.8.5b2/requirements/py38/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/requirements/py38/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/requirements/py38/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/requirements/py38/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.205462 python-project-structure-0.8.5b2/requirements/py39/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/requirements/py39/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/requirements/py39/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-10 20:29:55.000000 python-project-structure-0.8.5b2/requirements/py39/user.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-10 20:30:04.208462 python-project-structure-0.8.5b2/setup.cfg
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.194461 python-project-structure-0.8.5b2/src/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.206462 python-project-structure-0.8.5b2/src/python_project_structure.egg-info/
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-10 20:30:04.000000 python-project-structure-0.8.5b2/src/python_project_structure.egg-info/PKG-INFO
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1768 2023-04-10 20:30:04.000000 python-project-structure-0.8.5b2/src/python_project_structure.egg-info/SOURCES.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-10 20:30:04.000000 python-project-structure-0.8.5b2/src/python_project_structure.egg-info/dependency_links.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-10 20:30:04.000000 python-project-structure-0.8.5b2/src/python_project_structure.egg-info/entry_points.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-10 20:30:04.000000 python-project-structure-0.8.5b2/src/python_project_structure.egg-info/requires.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-10 20:30:04.000000 python-project-structure-0.8.5b2/src/python_project_structure.egg-info/top_level.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.207462 python-project-structure-0.8.5b2/src/pythonprojectstructure/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/src/pythonprojectstructure/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/src/pythonprojectstructure/__main__.py
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.207462 python-project-structure-0.8.5b2/src/pythonprojectstructure/newsfragments/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/src/pythonprojectstructure/newsfragments/.gitignore
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 20:30:04.207462 python-project-structure-0.8.5b2/src/pythonprojectstructure/tests/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/src/pythonprojectstructure/tests/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/src/pythonprojectstructure/tests/test_cli.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/src/pythonprojectstructure/utils.py
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-10 20:30:04.000000 python-project-structure-0.8.5b2/src/pythonprojectstructure/version.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-10 20:28:15.000000 python-project-structure-0.8.5b2/tox.ini
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.009114 python-project-structure-0.8.5b7/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.dir-locals.el.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.dockerignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.env.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:17.992112 python-project-structure-0.8.5b7/.github/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:17.998113 python-project-structure-0.8.5b7/.github/workflows/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.github/workflows/build-test.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4182 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.gitlab-ci.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.pre-commit-config.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/.prospector.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/CONTRIBUTING.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/Dockerfile.devel
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/LICENSE
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    56718 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4014 2023-04-10 21:17:06.000000 python-project-structure-0.8.5b7/NEWS.rst
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-10 21:17:18.009114 python-project-structure-0.8.5b7/PKG-INFO
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/README.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/TODO.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:17.999113 python-project-structure-0.8.5b7/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/bin/cz-check-bump
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/bin/entrypoint
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/bin/get-base-version
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/bin/hadolint
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.003113 python-project-structure-0.8.5b7/build-host/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/build-host/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/build-host/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/build-host/README.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.003113 python-project-structure-0.8.5b7/build-host/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/build-host/bin/entrypoint
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/build-host/requirements-py310.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/build-host/requirements-py311.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/build-host/requirements-py37.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/build-host/requirements-py38.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/build-host/requirements-py39.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/build-host/requirements.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.003113 python-project-structure-0.8.5b7/dist/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/dist/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4400 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/docker-compose.override.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/docker-compose.yml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.004113 python-project-structure-0.8.5b7/home/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/home/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/home/.pypirc.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2629 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/pyproject.toml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.004113 python-project-structure-0.8.5b7/requirements/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/requirements/build.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.004113 python-project-structure-0.8.5b7/requirements/py310/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/requirements/py310/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py310/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py310/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.005113 python-project-structure-0.8.5b7/requirements/py311/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/requirements/py311/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py311/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py311/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.005113 python-project-structure-0.8.5b7/requirements/py37/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/requirements/py37/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py37/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py37/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.006114 python-project-structure-0.8.5b7/requirements/py38/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/requirements/py38/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py38/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py38/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.007114 python-project-structure-0.8.5b7/requirements/py39/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/requirements/py39/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py39/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-10 21:17:08.000000 python-project-structure-0.8.5b7/requirements/py39/user.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-10 21:17:18.010114 python-project-structure-0.8.5b7/setup.cfg
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:17.994112 python-project-structure-0.8.5b7/src/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.008114 python-project-structure-0.8.5b7/src/python_project_structure.egg-info/
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-10 21:17:17.000000 python-project-structure-0.8.5b7/src/python_project_structure.egg-info/PKG-INFO
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1768 2023-04-10 21:17:17.000000 python-project-structure-0.8.5b7/src/python_project_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-10 21:17:17.000000 python-project-structure-0.8.5b7/src/python_project_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-10 21:17:17.000000 python-project-structure-0.8.5b7/src/python_project_structure.egg-info/entry_points.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-10 21:17:17.000000 python-project-structure-0.8.5b7/src/python_project_structure.egg-info/requires.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-10 21:17:17.000000 python-project-structure-0.8.5b7/src/python_project_structure.egg-info/top_level.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.008114 python-project-structure-0.8.5b7/src/pythonprojectstructure/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/src/pythonprojectstructure/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/src/pythonprojectstructure/__main__.py
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.009114 python-project-structure-0.8.5b7/src/pythonprojectstructure/newsfragments/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/src/pythonprojectstructure/newsfragments/.gitignore
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-10 21:17:18.009114 python-project-structure-0.8.5b7/src/pythonprojectstructure/tests/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/src/pythonprojectstructure/tests/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/src/pythonprojectstructure/tests/test_cli.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/src/pythonprojectstructure/utils.py
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-10 21:17:17.000000 python-project-structure-0.8.5b7/src/pythonprojectstructure/version.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-10 21:15:26.000000 python-project-structure-0.8.5b7/tox.ini
```

### Comparing `python-project-structure-0.8.5b2/.dir-locals.el.in` & `python-project-structure-0.8.5b7/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/.dockerignore` & `python-project-structure-0.8.5b7/.dockerignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/.env.in` & `python-project-structure-0.8.5b7/.env.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/.github/workflows/build-test.yml` & `python-project-structure-0.8.5b7/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/.gitignore` & `python-project-structure-0.8.5b7/.gitignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/.gitlab-ci.yml` & `python-project-structure-0.8.5b7/.gitlab-ci.yml`

 * *Files 11% similar despite different names*

```diff
@@ -49,19 +49,17 @@
   - "release"
   - "scheduled"
 
 build-test:
   stage: "build-test"
   rules:
     - if: >-
-        $CI_COMMIT_TAG ||
-        $CI_COMMIT_MESSAGE =~ "(?ims).*\[ci skip\].*"
-      when: "never"
-    - if: >-
-        $CI_PIPELINE_SOURCE != "schedule"
+        ($CI_COMMIT_TAG == null || $CI_COMMIT_TAG == "")
+        && $CI_PIPELINE_SOURCE != "schedule"
+        && $CI_COMMIT_MESSAGE !~ /(?ims).*\[actions skip\].*/
   interruptible: true
   parallel:
     matrix:
       - PYTHON_MINORS:
           - "3.11"
           - "3.10"
           - "3.9"
@@ -99,22 +97,20 @@
   # Avoid unnecessary artifact downloads:
   # https://docs.gitlab.com/ee/ci/yaml/#dependencies
   dependencies: []
   variables:
     DOCKER_BUILD_PULL: "true"
   rules:
     - if: >-
-        $CI_COMMIT_TAG ||
-        $CI_COMMIT_MESSAGE =~ "(?ims).*\[ci skip\].*"
-      when: "never"
-    - if: >-
-        $CI_PROJECT_NAMESPACE == "rpatterson"
+        ($CI_COMMIT_TAG == null || $CI_COMMIT_TAG == "")
+        && $CI_PROJECT_NAMESPACE == "rpatterson"
         && $CI_COMMIT_BRANCH != null
         && $CI_COMMIT_BRANCH =~ "^(develop|master)$"
         && $CI_PIPELINE_SOURCE != "schedule"
+        && $CI_COMMIT_MESSAGE !~ /(?ims).*\[actions skip\].*/
   script:
     - >-
       entrypoint make -e release-python test-clean
   artifacts:
     paths:
       - "./NEWS-release.rst"
       - "./dist/python?project?structure-*"
```

### Comparing `python-project-structure-0.8.5b2/.pre-commit-config.yaml` & `python-project-structure-0.8.5b7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/.prospector.yaml` & `python-project-structure-0.8.5b7/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/CONTRIBUTING.rst` & `python-project-structure-0.8.5b7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/Dockerfile` & `python-project-structure-0.8.5b7/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/Dockerfile.devel` & `python-project-structure-0.8.5b7/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/LICENSE` & `python-project-structure-0.8.5b7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/Makefile` & `python-project-structure-0.8.5b7/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -1225,15 +1225,15 @@
 	set +x
 	echo "ERROR: PROJECT_GITHUB_PAT missing from ./.env or CI secrets"
 	false
 endif
 endif
 	set -x
 # Fail fast if there's still no push access
-	git push -o ci.skip --no-verify --tags "origin"
+	git push --no-verify --tags "origin"
 endif
 
 # Ensure release publishing authentication, mostly useful in automation such as CI.
 ~/.pypirc: ./home/.pypirc.in
 	$(MAKE) -e "template=$(<)" "target=$(@)" expand-template
 
 ./var/log/docker-login-DOCKER.log: ./.env
```

### Comparing `python-project-structure-0.8.5b2/NEWS.rst` & `python-project-structure-0.8.5b7/NEWS.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,43 @@
+python-project-structure 0.8.5b7 (2023-04-10)
+=============================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
+python-project-structure 0.8.5b6 (2023-04-10)
+=============================================
+
+No significant changes.
+
+
+python-project-structure 0.8.5b5 (2023-04-10)
+=============================================
+
+No significant changes.
+
+
+python-project-structure 0.8.5b4 (2023-04-10)
+=============================================
+
+No significant changes.
+
+
+python-project-structure 0.8.5b3 (2023-04-10)
+=============================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
 python-project-structure 0.8.5b2 (2023-04-10)
 =============================================
 
 Bugfixes
 --------
 
 - Simulate a patch release. (simulate)
```

### Comparing `python-project-structure-0.8.5b2/PKG-INFO` & `python-project-structure-0.8.5b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.5b2
+Version: 0.8.5b7
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.5b2/README.rst` & `python-project-structure-0.8.5b7/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/TODO.rst` & `python-project-structure-0.8.5b7/TODO.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/bin/cz-check-bump` & `python-project-structure-0.8.5b7/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/bin/entrypoint` & `python-project-structure-0.8.5b7/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/bin/get-base-version` & `python-project-structure-0.8.5b7/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/build-host/Dockerfile` & `python-project-structure-0.8.5b7/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/build-host/Makefile` & `python-project-structure-0.8.5b7/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/build-host/README.rst` & `python-project-structure-0.8.5b7/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/build-host/bin/entrypoint` & `python-project-structure-0.8.5b7/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/build-host/requirements-py310.txt` & `python-project-structure-0.8.5b7/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/build-host/requirements-py311.txt` & `python-project-structure-0.8.5b7/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/build-host/requirements-py37.txt` & `python-project-structure-0.8.5b7/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/build-host/requirements-py38.txt` & `python-project-structure-0.8.5b7/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/build-host/requirements-py39.txt` & `python-project-structure-0.8.5b7/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/docker-compose.override.yml` & `python-project-structure-0.8.5b7/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/docker-compose.yml` & `python-project-structure-0.8.5b7/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/pyproject.toml` & `python-project-structure-0.8.5b7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 # TEMPLATE: Update these versions to the latest version for your project and ensure the
 # tag exists both locally and on the project's remote:
 changelog_start_rev = "v0.0.0"
-version = "0.8.5b2"
+version = "0.8.5b7"
 tag_format = "v$version"
 annotated_tag = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
-[ci skip]
+[actions skip]
 """
 [tool.towncrier]
 # https://towncrier.readthedocs.io/en/stable/#quick-start
 package = "pythonprojectstructure"
 package_dir = "src"
 name = "python-project-structure"
```

### Comparing `python-project-structure-0.8.5b2/requirements/build.txt.in` & `python-project-structure-0.8.5b7/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/requirements/py310/build.txt` & `python-project-structure-0.8.5b7/requirements/py310/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/requirements/py310/devel.txt` & `python-project-structure-0.8.5b7/requirements/py310/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/requirements/py311/build.txt` & `python-project-structure-0.8.5b7/requirements/py311/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/requirements/py311/devel.txt` & `python-project-structure-0.8.5b7/requirements/py311/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/requirements/py37/build.txt` & `python-project-structure-0.8.5b7/requirements/py37/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/requirements/py37/devel.txt` & `python-project-structure-0.8.5b7/requirements/py37/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/requirements/py38/build.txt` & `python-project-structure-0.8.5b7/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/requirements/py38/devel.txt` & `python-project-structure-0.8.5b7/requirements/py38/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/requirements/py39/build.txt` & `python-project-structure-0.8.5b7/requirements/py39/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/requirements/py39/devel.txt` & `python-project-structure-0.8.5b7/requirements/py39/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/setup.cfg` & `python-project-structure-0.8.5b7/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/src/python_project_structure.egg-info/PKG-INFO` & `python-project-structure-0.8.5b7/src/python_project_structure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.5b2
+Version: 0.8.5b7
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.5b2/src/python_project_structure.egg-info/SOURCES.txt` & `python-project-structure-0.8.5b7/src/python_project_structure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/src/pythonprojectstructure/__init__.py` & `python-project-structure-0.8.5b7/src/pythonprojectstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/src/pythonprojectstructure/tests/test_cli.py` & `python-project-structure-0.8.5b7/src/pythonprojectstructure/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.5b2/tox.ini` & `python-project-structure-0.8.5b7/tox.ini`

 * *Files identical despite different names*

