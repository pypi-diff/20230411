# Comparing `tmp/invenio-db-1.0.9.tar.gz` & `tmp/invenio-db-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-db-1.0.9.tar", last modified: Fri Mar 19 08:46:02 2021, max compression
+gzip compressed data, was "dist/invenio-db-1.1.0.tar", last modified: Tue Apr 11 08:04:00 2023, max compression
```

## Comparing `invenio-db-1.0.9.tar` & `invenio-db-1.1.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-19 08:46:02.000000 invenio-db-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-03-19 08:45:59.000000 invenio-db-1.0.9/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      804 2021-03-19 08:45:59.000000 invenio-db-1.0.9/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-19 08:46:02.000000 invenio-db-1.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-19 08:46:02.000000 invenio-db-1.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      661 2021-03-19 08:45:59.000000 invenio-db-1.0.9/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2205 2021-03-19 08:45:59.000000 invenio-db-1.0.9/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)      492 2021-03-19 08:45:59.000000 invenio-db-1.0.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1668 2021-03-19 08:45:59.000000 invenio-db-1.0.9/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3698 2021-03-19 08:45:59.000000 invenio-db-1.0.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      589 2021-03-19 08:45:59.000000 invenio-db-1.0.9/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-03-19 08:45:59.000000 invenio-db-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      662 2021-03-19 08:45:59.000000 invenio-db-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4439 2021-03-19 08:46:02.000000 invenio-db-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      948 2021-03-19 08:45:59.000000 invenio-db-1.0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-19 08:46:02.000000 invenio-db-1.0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7425 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-19 08:46:02.000000 invenio-db-1.0.9/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (121)     2093 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/_ext/ultramock.py
--rw-r--r--   0 runner    (1001) docker     (121)     6314 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/alembic.rst
--rw-r--r--   0 runner    (1001) docker     (121)      375 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9916 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1775 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      252 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      856 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6989 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4138 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/session_management.rst
--rw-r--r--   0 runner    (1001) docker     (121)      259 2021-03-19 08:45:59.000000 invenio-db-1.0.9/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-19 08:46:02.000000 invenio-db-1.0.9/invenio_db/
--rw-r--r--   0 runner    (1001) docker     (121)     2717 2021-03-19 08:45:59.000000 invenio-db-1.0.9/invenio_db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-19 08:46:02.000000 invenio-db-1.0.9/invenio_db/alembic/
--rw-r--r--   0 runner    (1001) docker     (121)     4007 2021-03-19 08:45:59.000000 invenio-db-1.0.9/invenio_db/alembic/35c1075e6360_force_naming_convention.py
--rw-r--r--   0 runner    (1001) docker     (121)      548 2021-03-19 08:45:59.000000 invenio-db-1.0.9/invenio_db/alembic/96e796392533_create_database_migrations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2021-03-19 08:45:59.000000 invenio-db-1.0.9/invenio_db/alembic/dbdbc1b19cf2_create_transaction_table.py
--rw-r--r--   0 runner    (1001) docker     (121)      693 2021-03-19 08:45:59.000000 invenio-db-1.0.9/invenio_db/alembic/script.py.mako
--rw-r--r--   0 runner    (1001) docker     (121)     3364 2021-03-19 08:45:59.000000 invenio-db-1.0.9/invenio_db/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     5098 2021-03-19 08:45:59.000000 invenio-db-1.0.9/invenio_db/ext.py
--rw-r--r--   0 runner    (1001) docker     (121)     4076 2021-03-19 08:45:59.000000 invenio-db-1.0.9/invenio_db/shared.py
--rw-r--r--   0 runner    (1001) docker     (121)     3456 2021-03-19 08:45:59.000000 invenio-db-1.0.9/invenio_db/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2021-03-19 08:45:59.000000 invenio-db-1.0.9/invenio_db/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-19 08:46:02.000000 invenio-db-1.0.9/invenio_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4439 2021-03-19 08:46:02.000000 invenio-db-1.0.9/invenio_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2021-03-19 08:46:02.000000 invenio-db-1.0.9/invenio_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-19 08:46:02.000000 invenio-db-1.0.9/invenio_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-03-19 08:46:02.000000 invenio-db-1.0.9/invenio_db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-19 08:46:02.000000 invenio-db-1.0.9/invenio_db.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      596 2021-03-19 08:46:02.000000 invenio-db-1.0.9/invenio_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-03-19 08:46:02.000000 invenio-db-1.0.9/invenio_db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      409 2021-03-19 08:45:59.000000 invenio-db-1.0.9/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      671 2021-03-19 08:45:59.000000 invenio-db-1.0.9/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      756 2021-03-19 08:45:59.000000 invenio-db-1.0.9/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-03-19 08:46:02.000000 invenio-db-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2747 2021-03-19 08:45:59.000000 invenio-db-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-19 08:46:02.000000 invenio-db-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2021-03-19 08:45:59.000000 invenio-db-1.0.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-19 08:46:02.000000 invenio-db-1.0.9/tests/demo/
--rw-r--r--   0 runner    (1001) docker     (121)      254 2021-03-19 08:45:59.000000 invenio-db-1.0.9/tests/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      537 2021-03-19 08:45:59.000000 invenio-db-1.0.9/tests/demo/child.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2021-03-19 08:45:59.000000 invenio-db-1.0.9/tests/demo/parent.py
--rw-r--r--   0 runner    (1001) docker     (121)      736 2021-03-19 08:45:59.000000 invenio-db-1.0.9/tests/demo/versioned_a.py
--rw-r--r--   0 runner    (1001) docker     (121)      736 2021-03-19 08:45:59.000000 invenio-db-1.0.9/tests/demo/versioned_b.py
--rw-r--r--   0 runner    (1001) docker     (121)    12727 2021-03-19 08:45:59.000000 invenio-db-1.0.9/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     2599 2021-03-19 08:45:59.000000 invenio-db-1.0.9/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2021-03-19 08:45:59.000000 invenio-db-1.0.9/tests/test_versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-04-11 08:03:57.000000 invenio-db-1.1.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-11 08:03:57.000000 invenio-db-1.1.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-11 08:03:57.000000 invenio-db-1.1.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      661 2023-04-11 08:03:57.000000 invenio-db-1.1.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2834 2023-04-11 08:03:57.000000 invenio-db-1.1.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-11 08:03:57.000000 invenio-db-1.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-04-11 08:03:57.000000 invenio-db-1.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-04-11 08:03:57.000000 invenio-db-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-04-11 08:03:57.000000 invenio-db-1.1.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-04-11 08:03:57.000000 invenio-db-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-04-11 08:03:57.000000 invenio-db-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-04-11 08:04:00.000000 invenio-db-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-04-11 08:03:57.000000 invenio-db-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-11 08:03:57.000000 invenio-db-1.1.0/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7425 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     6314 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/alembic.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     9968 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6989 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4138 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/session_management.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db/
+-rw-r--r--   0 runner    (1001) docker     (122)     2651 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)     4110 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/alembic/35c1075e6360_force_naming_convention.py
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/alembic/96e796392533_create_database_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/alembic/dbdbc1b19cf2_create_transaction_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/alembic/script.py.mako
+-rw-r--r--   0 runner    (1001) docker     (122)     3329 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5593 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/shared.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4315 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      329 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-04-11 08:03:57.000000 invenio-db-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      671 2023-04-11 08:03:57.000000 invenio-db-1.1.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      708 2023-04-11 08:03:57.000000 invenio-db-1.1.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-04-11 08:04:00.000000 invenio-db-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-04-11 08:03:57.000000 invenio-db-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/tests/demo/
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/demo/child.py
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/demo/parent.py
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/demo/versioned_a.py
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/demo/versioned_b.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12583 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3702 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/test_versioning.py
```

### Comparing `invenio-db-1.0.9/.editorconfig` & `invenio-db-1.1.0/.editorconfig`

 * *Files 9% similar despite different names*

```diff
@@ -11,23 +11,14 @@
 [*]
 indent_style = space
 end_of_line = lf
 insert_final_newline = true
 trim_trailing_whitespace = true
 charset = utf-8
 
-# Python files
-[*.py]
-indent_size = 4
-# isort plugin configuration
-known_first_party = invenio_db
-multi_line_output = 2
-default_section = THIRDPARTY
-skip = .eggs
-
 # RST files (used by sphinx)
 [*.rst]
 indent_size = 4
 
 # CSS, HTML, JS, JSON, YML
 [*.{css,html,js,json,yml}]
 indent_size = 2
```

### Comparing `invenio-db-1.0.9/.github/workflows/pypi-publish.yml` & `invenio-db-1.1.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-db-1.0.9/.github/workflows/tests.yml` & `invenio-db-1.1.0/.github/workflows/tests.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+# -*- coding: utf-8 -*-
+#
+# This file is part of Invenio.
+# Copyright (C) 2020 CERN.
+# Copyright (C) 2022 Graz University of Technology.
+#
+# Invenio is free software; you can redistribute it and/or modify it
+# under the terms of the MIT License; see LICENSE file for more details.
+
 name: CI
 
 on:
   push:
     branches: master
   pull_request:
     branches: master
@@ -16,63 +25,77 @@
         default: 'Manual trigger'
 
 jobs:
   Tests:
     runs-on: ubuntu-20.04
     strategy:
       matrix:
-          python-version: [3.6, 3.7, 3.8, 3.9]
-          requirements-level: [min, pypi]
-          db-service: [postgresql9, postgresql11, mysql5]
+          python-version: [3.7, 3.8, 3.9]
+          requirements-level: [pypi]
+          db-service: [postgresql10, postgresql14, mysql5, mysql8]
           exclude:
+          - python-version: 3.7
+            db-service: postgresql14
+            requirements-level: pypi
+
+          - python-version: 3.7
+            db-service: mysql8
+            requirements-level: pypi
+
           - python-version: 3.8
-            requirements-level: min
+            db-service: postgresql10
 
           - python-version: 3.9
-            requirements-level: min
+            db-service: postgresql10
 
-          - db-service: postgresql11
-            python-version: 3.6
+          - python-version: 3.8
+            db-service: mysql5
+
+          - python-version: 3.9
+            db-service: mysql5
 
           include:
-          - db-service: postgresql9
+          - db-service: postgresql10
             DB_EXTRAS: "postgresql"
 
-          - db-service: postgresql11
+          - db-service: postgresql14
             DB_EXTRAS: "postgresql"
 
           - db-service: mysql5
             DB_EXTRAS: "mysql"
 
+          - db-service: mysql8
+            DB_EXTRAS: "mysql"
+
     env:
       DB: ${{ matrix.db-service }}
-      EXTRAS: all,${{ matrix.DB_EXTRAS }}
+      EXTRAS: tests,${{ matrix.DB_EXTRAS }}
     steps:
       - name: Checkout
         uses: actions/checkout@v2
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Generate dependencies
         run: |
-          python -m pip install --upgrade pip setuptools py wheel requirements-builder
+          pip install wheel requirements-builder
           requirements-builder -e "$EXTRAS" --level=${{ matrix.requirements-level }} setup.py > .${{ matrix.requirements-level }}-${{ matrix.python-version }}-requirements.txt
 
       - name: Cache pip
         uses: actions/cache@v2
         with:
           path: ~/.cache/pip
           key: ${{ runner.os }}-pip-${{ hashFiles('.${{ matrix.requirements-level }}-${{ matrix.python-version }}-requirements.txt') }}
 
       - name: Install dependencies
         run: |
-          pip install -r .${{ matrix.requirements-level }}-${{ matrix.python-version }}-requirements.txt
+          pip install -r .${{ matrix.requirements-level }}-${{ matrix.python-version }}-requirements.txt -c constraints-${{ matrix.requirements-level }}.txt
           pip install ".[$EXTRAS]"
           pip freeze
           docker --version
           docker-compose --version
 
       - name: Run tests
         run: |
```

### Comparing `invenio-db-1.0.9/CHANGES.rst` & `invenio-db-1.1.0/CHANGES.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,48 @@
 ..
     This file is part of Invenio.
-    Copyright (C) 2015-2020 CERN.
+    Copyright (C) 2015-2023 CERN.
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 1.1.0 (released 2023-04-06)
+
+- Increase minimum version of Python to 3.7
+- Upgrades flask-sqlalchemy
+- Fixes deprecation warnings for flask-sqlalchemy, EncryptedType and WeakKeyDictionary
+
+Version 1.0.14 (released 2022-03-30)
+
+- Adds support for SQLAlchemy 1.4 and Flask v2.1.
+
+Version 1.0.13 (released 2022-02-21)
+
+- Changes alembic migrations to run a single migration in one transaction
+  instead of all migrations in a single transaction.
+
+Version 1.0.12 (released 2022-02-14)
+
+- Fixes a deprecation warning.
+
+Version 1.0.11 (released 2022-02-08)
+
+- Fixed issue with alembic version locations introduced in v1.0.10 due to the
+  importlib change.
+
+Version 1.0.10 (released 2022-02-08)
+
+- Adds a utility for creating an alembic test context to centrally manage
+  fixes for alembic migration tests in other modules.
+
+- Replaces pkg_resources with importlib
+
 Version 1.0.9 (released 2021-03-18)
 
 - Pins Flask-SQLAlchemy below 2.5 due to breaking changes. Perhaps to revisit when fixed.
 
 Version 1.0.8 (released 2020-11-16)
 
 - Pins SQLAlchemy to >=1.2.18 and <1.4 due to incompatibility between
```

### Comparing `invenio-db-1.0.9/CONTRIBUTING.rst` & `invenio-db-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-db-1.0.9/INSTALL.rst` & `invenio-db-1.1.0/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `invenio-db-1.0.9/LICENSE` & `invenio-db-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-db-1.0.9/MANIFEST.in` & `invenio-db-1.1.0/MANIFEST.in`

 * *Files 12% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs Makefile
 recursive-include invenio_db *.mako
 recursive-include invenio_db *.py
 recursive-include tests *.py
 recursive-include .github/workflows *.yml
+include .git-blame-ignore-revs
```

### Comparing `invenio-db-1.0.9/PKG-INFO` & `invenio-db-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: invenio-db
-Version: 1.0.9
+Version: 1.1.0
 Summary: Database management for Invenio.
 Home-page: https://github.com/inveniosoftware/invenio-db
-Author: Invenio Collaboration
+Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
             Copyright (C) 2015-2018 CERN.
         
             Invenio is free software; you can redistribute it and/or modify it
@@ -29,25 +29,55 @@
         .. image:: https://img.shields.io/pypi/v/invenio-db.svg
                 :target: https://pypi.org/pypi/invenio-db
         
         
         Database management for Invenio.
         Further documentation available on https://invenio-db.readthedocs.io/
         
-        
         ..
             This file is part of Invenio.
-            Copyright (C) 2015-2020 CERN.
+            Copyright (C) 2015-2023 CERN.
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.1.0 (released 2023-04-06)
+        
+        - Increase minimum version of Python to 3.7
+        - Upgrades flask-sqlalchemy
+        - Fixes deprecation warnings for flask-sqlalchemy, EncryptedType and WeakKeyDictionary
+        
+        Version 1.0.14 (released 2022-03-30)
+        
+        - Adds support for SQLAlchemy 1.4 and Flask v2.1.
+        
+        Version 1.0.13 (released 2022-02-21)
+        
+        - Changes alembic migrations to run a single migration in one transaction
+          instead of all migrations in a single transaction.
+        
+        Version 1.0.12 (released 2022-02-14)
+        
+        - Fixes a deprecation warning.
+        
+        Version 1.0.11 (released 2022-02-08)
+        
+        - Fixed issue with alembic version locations introduced in v1.0.10 due to the
+          importlib change.
+        
+        Version 1.0.10 (released 2022-02-08)
+        
+        - Adds a utility for creating an alembic test context to centrally manage
+          fixes for alembic migration tests in other modules.
+        
+        - Replaces pkg_resources with importlib
+        
         Version 1.0.9 (released 2021-03-18)
         
         - Pins Flask-SQLAlchemy below 2.5 due to breaking changes. Perhaps to revisit when fixed.
         
         Version 1.0.8 (released 2020-11-16)
         
         - Pins SQLAlchemy to >=1.2.18 and <1.4 due to incompatibility between
@@ -93,26 +123,13 @@
         
         Version 1.0.0 (released 2018-03-23)
         
         - Initial public release.
         
 Keywords: invenio database
 Platform: any
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 5 - Production/Stable
-Provides-Extra: docs
+Requires-Python: >=3.7
+Provides-Extra: tests
 Provides-Extra: mysql
 Provides-Extra: postgresql
 Provides-Extra: versioning
-Provides-Extra: tests
-Provides-Extra: all
```

### Comparing `invenio-db-1.0.9/README.rst` & `invenio-db-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-db-1.0.9/docs/Makefile` & `invenio-db-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-db-1.0.9/docs/alembic.rst` & `invenio-db-1.1.0/docs/alembic.rst`

 * *Files identical despite different names*

### Comparing `invenio-db-1.0.9/docs/conf.py` & `invenio-db-1.1.0/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,321 +1,318 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2018 CERN.
+# Copyright (C) 2022 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Sphinx configuration."""
 
-from __future__ import print_function
-
 import os
 import sys
 
 import sphinx.environment
 
+from invenio_db import __version__
+
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Do not warn on external images.
-suppress_warnings = ['image.nonlocal_uri']
+suppress_warnings = ["image.nonlocal_uri"]
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.coverage',
-    'sphinx.ext.doctest',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.viewcode',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.viewcode",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'Invenio-DB'
-copyright = u'2015, CERN'
-author = u'CERN'
+project = "Invenio-DB"
+copyright = "2015, CERN"
+author = "CERN"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 
 # Get the version string. Cannot be done with import!
-g = {}
-with open(os.path.join('..', 'invenio_db', 'version.py'), 'rt') as fp:
-    exec(fp.read(), g)
-    version = g['__version__']
+version = __version__
 
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = []
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
-#keep_warnings = False
+# keep_warnings = False
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output ----------------------------------------------
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 html_theme_options = {
-    'description': 'Database management for Invenio.',
-    'github_user': 'inveniosoftware',
-    'github_repo': 'invenio-db',
-    'github_button': False,
-    'github_banner': True,
-    'show_powered_by': False,
-    'extra_nav_links': {
-        'invenio-db@GitHub': 'https://github.com/inveniosoftware/invenio-db',
-        'invenio-db@PyPI': 'https://pypi.python.org/pypi/invenio-db/',
-    }
+    "description": "Database management for Invenio.",
+    "github_user": "inveniosoftware",
+    "github_repo": "invenio-db",
+    "github_button": False,
+    "github_banner": True,
+    "show_powered_by": False,
+    "extra_nav_links": {
+        "invenio-db@GitHub": "https://github.com/inveniosoftware/invenio-db",
+        "invenio-db@PyPI": "https://pypi.python.org/pypi/invenio-db/",
+    },
 }
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-#html_static_path = ['_static']
+# html_static_path = ['_static']
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
-#html_extra_path = []
+# html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
 html_sidebars = {
-    '**': [
-        'about.html',
-        'navigation.html',
-        'relations.html',
-        'searchbox.html',
-        'donate.html',
+    "**": [
+        "about.html",
+        "navigation.html",
+        "relations.html",
+        "searchbox.html",
+        "donate.html",
     ]
 }
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Language to be used for generating the HTML full-text search index.
 # Sphinx supports the following languages:
 #   'da', 'de', 'en', 'es', 'fi', 'fr', 'hu', 'it', 'ja'
 #   'nl', 'no', 'pt', 'ro', 'ru', 'sv', 'tr'
-#html_search_language = 'en'
+# html_search_language = 'en'
 
 # A dictionary with options for the search language support, empty by default.
 # Now only 'ja' uses this config value
-#html_search_options = {'type': 'default'}
+# html_search_options = {'type': 'default'}
 
 # The name of a javascript file (relative to the configuration directory) that
 # implements a search results scorer. If empty, the default will be used.
-#html_search_scorer = 'scorer.js'
+# html_search_scorer = 'scorer.js'
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'invenio-db_namedoc'
+htmlhelp_basename = "invenio-db_namedoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-#'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-#'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-#'preamble': '',
-
-# Latex figure (float) alignment
-#'figure_align': 'htbp',
+    # The paper size ('letterpaper' or 'a4paper').
+    #'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #'preamble': '',
+    # Latex figure (float) alignment
+    #'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-  (master_doc, 'invenio-db.tex', u'invenio-db Documentation',
-   u'CERN', 'manual'),
+    (master_doc, "invenio-db.tex", "invenio-db Documentation", "CERN", "manual"),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'invenio-db', u'invenio-db Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "invenio-db", "invenio-db Documentation", [author], 1)]
 
 # If true, show URL addresses after external links.
-#man_show_urls = False
+# man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-  (master_doc, 'invenio-db', u'Invenio-DB Documentation',
-   author, 'invenio-db', 'Database management for Invenio.',
-   'Miscellaneous'),
+    (
+        master_doc,
+        "invenio-db",
+        "Invenio-DB Documentation",
+        author,
+        "invenio-db",
+        "Database management for Invenio.",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
+# texinfo_appendices = []
 
 # If false, no module index is generated.
-#texinfo_domain_indices = True
+# texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
+# texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
-#texinfo_no_detailmenu = False
+# texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'https://docs.python.org/': None}
+intersphinx_mapping = {"https://docs.python.org/": None}
 
 # Autodoc configuraton.
-autoclass_content = 'both'
+autoclass_content = "both"
```

### Comparing `invenio-db-1.0.9/docs/configuration.rst` & `invenio-db-1.1.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `invenio-db-1.0.9/docs/index.rst` & `invenio-db-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-db-1.0.9/docs/make.bat` & `invenio-db-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-db-1.0.9/docs/session_management.rst` & `invenio-db-1.1.0/docs/session_management.rst`

 * *Files identical despite different names*

### Comparing `invenio-db-1.0.9/invenio_db/__init__.py` & `invenio-db-1.1.0/invenio_db/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,18 +84,17 @@
                'mymodule = mymodule.models',
            ],
        },
    )
 
 """
 
-from __future__ import absolute_import, print_function
-
 from .ext import InvenioDB
 from .shared import db
-from .version import __version__
+
+__version__ = "1.1.0"
 
 __all__ = (
-    '__version__',
-    'db',
-    'InvenioDB',
+    "__version__",
+    "db",
+    "InvenioDB",
 )
```

### Comparing `invenio-db-1.0.9/invenio_db/alembic/35c1075e6360_force_naming_convention.py` & `invenio-db-1.1.0/invenio_db/alembic/35c1075e6360_force_naming_convention.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,97 +6,105 @@
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Force naming convention."""
 
 import sqlalchemy as sa
 from alembic import op, util
-from sqlalchemy.engine.reflection import Inspector
+from sqlalchemy import inspect
 
 # revision identifiers, used by Alembic.
-revision = '35c1075e6360'
-down_revision = 'dbdbc1b19cf2'
+revision = "35c1075e6360"
+down_revision = "dbdbc1b19cf2"
 branch_labels = ()
 depends_on = None
 
-NAMING_CONVENTION = sa.util.immutabledict({
-    'ix': 'ix_%(column_0_label)s',
-    'uq': 'uq_%(table_name)s_%(column_0_name)s',
-    'ck': 'ck_%(table_name)s_%(constraint_name)s',
-    'fk': 'fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s',
-    'pk': 'pk_%(table_name)s',
-})
+NAMING_CONVENTION = sa.util.immutabledict(
+    {
+        "ix": "ix_%(column_0_label)s",
+        "uq": "uq_%(table_name)s_%(column_0_name)s",
+        "ck": "ck_%(table_name)s_%(constraint_name)s",
+        "fk": "fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s",
+        "pk": "pk_%(table_name)s",
+    }
+)
 """Configuration for constraint naming conventions (v1.0.0b5)."""
 
 
 def upgrade():
     """Upgrade database."""
-    op.execute('COMMIT')  # See https://bitbucket.org/zzzeek/alembic/issue/123
+    op.execute("COMMIT")  # See https://bitbucket.org/zzzeek/alembic/issue/123
     ctx = op.get_context()
-    metadata = ctx.opts['target_metadata']
+    metadata = ctx.opts["target_metadata"]
     metadata.naming_convention = NAMING_CONVENTION
     metadata.bind = ctx.connection.engine
-    insp = Inspector.from_engine(ctx.connection.engine)
+    insp = inspect(ctx.connection.engine)
 
     for table_name in insp.get_table_names():
         if table_name not in metadata.tables:
             continue
 
         table = metadata.tables[table_name]
 
         ixs = {}
         uqs = {}
         fks = {}
 
         for ix in insp.get_indexes(table_name):
-            ixs[tuple(ix['column_names'])] = ix
+            ixs[tuple(ix["column_names"])] = ix
         for uq in insp.get_unique_constraints(table_name):
-            uqs[tuple(uq['column_names'])] = uq
+            uqs[tuple(uq["column_names"])] = uq
         for fk in insp.get_foreign_keys(table_name):
-            fks[(tuple(fk['constrained_columns']), fk['referred_table'])] = fk
+            fks[(tuple(fk["constrained_columns"]), fk["referred_table"])] = fk
 
         with op.batch_alter_table(
-                table_name, naming_convention=NAMING_CONVENTION) as batch_op:
+            table_name, naming_convention=NAMING_CONVENTION
+        ) as batch_op:
             for c in list(table.constraints) + list(table.indexes):
                 key = None
                 if isinstance(c, sa.schema.ForeignKeyConstraint):
                     key = (tuple(c.column_keys), c.referred_table.name)
                     fk = fks.get(key)
-                    if fk and c.name != fk['name']:
-                        batch_op.drop_constraint(
-                            fk['name'], type_='foreignkey')
+                    if fk and c.name != fk["name"]:
+                        batch_op.drop_constraint(fk["name"], type_="foreignkey")
                         batch_op.create_foreign_key(
-                            op.f(c.name), fk['referred_table'],
-                            fk['constrained_columns'],
-                            fk['referred_columns'],
-                            **fk['options']
+                            op.f(c.name),
+                            fk["referred_table"],
+                            fk["constrained_columns"],
+                            fk["referred_columns"],
+                            **fk["options"]
                         )
                 elif isinstance(c, sa.schema.UniqueConstraint):
                     key = tuple(c.columns.keys())
                     uq = uqs.get(key)
-                    if uq and c.name != uq['name']:
-                        batch_op.drop_constraint(uq['name'], type_='unique')
+                    if uq and c.name != uq["name"]:
+                        batch_op.drop_constraint(uq["name"], type_="unique")
                         batch_op.create_unique_constraint(
-                            op.f(c.name), uq['column_names'])
+                            op.f(c.name), uq["column_names"]
+                        )
                 elif isinstance(c, sa.schema.CheckConstraint):
-                    util.warn('Update {0.table.name} CHECK {0.name} '
-                              'manually'.format(c))
+                    util.warn(
+                        "Update {0.table.name} CHECK {0.name} " "manually".format(c)
+                    )
                 elif isinstance(c, sa.schema.Index):
                     key = tuple(c.columns.keys())
                     ix = ixs.get(key)
-                    if ix and c.name != ix['name']:
-                        batch_op.drop_index(ix['name'])
+                    if ix and c.name != ix["name"]:
+                        batch_op.drop_index(ix["name"])
                         batch_op.create_index(
-                            op.f(c.name), ix['column_names'],
-                            unique=ix['unique'],
+                            op.f(c.name),
+                            ix["column_names"],
+                            unique=ix["unique"],
                         )
-                elif isinstance(c, sa.schema.PrimaryKeyConstraint) or \
-                        c.name == '_unnamed_':
+                elif (
+                    isinstance(c, sa.schema.PrimaryKeyConstraint)
+                    or c.name == "_unnamed_"
+                ):
                     # NOTE we don't care about primary keys since they have
                     # specific syntax.
                     pass
                 else:
-                    raise RuntimeError('Missing {0!r}'.format(c))
+                    raise RuntimeError("Missing {0!r}".format(c))
 
 
 def downgrade():
     """Downgrade database."""
```

### Comparing `invenio-db-1.0.9/invenio_db/alembic/96e796392533_create_database_migrations.py` & `invenio-db-1.1.0/invenio_db/alembic/96e796392533_create_database_migrations.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 """Create database migrations."""
 
 import sqlalchemy as sa
 from alembic import op
 
 # revision identifiers, used by Alembic.
-revision = '96e796392533'
+revision = "96e796392533"
 down_revision = None
-branch_labels = (u'default', )
+branch_labels = ("default",)
 depends_on = None
 
 
 def upgrade():
     """Update database."""
```

### Comparing `invenio-db-1.0.9/invenio_db/alembic/dbdbc1b19cf2_create_transaction_table.py` & `invenio-db-1.1.0/invenio_db/alembic/dbdbc1b19cf2_create_transaction_table.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 """Create transaction table."""
 
 import sqlalchemy as sa
 from alembic import op
 from sqlalchemy.schema import CreateSequence, DropSequence, Sequence
 
 # revision identifiers, used by Alembic.
-revision = 'dbdbc1b19cf2'
-down_revision = '96e796392533'
+revision = "dbdbc1b19cf2"
+down_revision = "96e796392533"
 branch_labels = ()
 depends_on = None
 
 
 def upgrade():
     """Update database."""
     op.create_table(
-        'transaction',
-        sa.Column('issued_at', sa.DateTime(), nullable=True),
-        sa.Column('id', sa.BigInteger(), nullable=False),
-        sa.Column('remote_addr', sa.String(length=50), nullable=True),
+        "transaction",
+        sa.Column("issued_at", sa.DateTime(), nullable=True),
+        sa.Column("id", sa.BigInteger(), nullable=False),
+        sa.Column("remote_addr", sa.String(length=50), nullable=True),
     )
-    op.create_primary_key('pk_transaction', 'transaction', ['id'])
+    op.create_primary_key("pk_transaction", "transaction", ["id"])
     if op._proxy.migration_context.dialect.supports_sequences:
-        op.execute(CreateSequence(Sequence('transaction_id_seq')))
+        op.execute(CreateSequence(Sequence("transaction_id_seq")))
 
 
 def downgrade():
     """Downgrade database."""
-    op.drop_table('transaction')
+    op.drop_table("transaction")
     if op._proxy.migration_context.dialect.supports_sequences:
-        op.execute(DropSequence(Sequence('transaction_id_seq')))
+        op.execute(DropSequence(Sequence("transaction_id_seq")))
```

### Comparing `invenio-db-1.0.9/invenio_db/alembic/script.py.mako` & `invenio-db-1.1.0/invenio_db/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `invenio-db-1.0.9/invenio_db/cli.py` & `invenio-db-1.1.0/invenio_db/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,104 +4,106 @@
 # Copyright (C) 2015-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Click command-line interface for database management."""
 
-from __future__ import absolute_import, print_function
-
-import sys
-
 import click
-from click import _termui_impl
-from flask import current_app
 from flask.cli import with_appcontext
-from sqlalchemy_utils.functions import create_database, database_exists, \
-    drop_database
-from werkzeug.local import LocalProxy
+from sqlalchemy_utils.functions import create_database, database_exists, drop_database
 
+from .proxies import current_sqlalchemy
 from .utils import create_alembic_version_table, drop_alembic_version_table
 
-_db = LocalProxy(lambda: current_app.extensions['sqlalchemy'].db)
-
-# Fix Python 3 compatibility issue in click
-if sys.version_info > (3,):
-    _termui_impl.long = int  # pragma: no cover
-
 
 def abort_if_false(ctx, param, value):
     """Abort command is value is False."""
     if not value:
         ctx.abort()
 
 
+def render_url(url):
+    """Render the URL for CLI output."""
+    try:
+        return url.render_as_string(hide_password=True)
+    except AttributeError:
+        # SQLAlchemy <1.4
+        return url.__to_string__(hide_password=True)
+
+
 #
 # Database commands
 #
 @click.group(chain=True)
 def db():
     """Database commands."""
 
 
 @db.command()
-@click.option('-v', '--verbose', is_flag=True, default=False)
+@click.option("-v", "--verbose", is_flag=True, default=False)
 @with_appcontext
 def create(verbose):
     """Create tables."""
-    click.secho('Creating all tables!', fg='yellow', bold=True)
-    with click.progressbar(_db.metadata.sorted_tables) as bar:
+    click.secho("Creating all tables!", fg="yellow", bold=True)
+    with click.progressbar(current_sqlalchemy.metadata.sorted_tables) as bar:
         for table in bar:
             if verbose:
-                click.echo(' Creating table {0}'.format(table))
-            table.create(bind=_db.engine, checkfirst=True)
+                click.echo(" Creating table {0}".format(table))
+            table.create(bind=current_sqlalchemy.engine, checkfirst=True)
     create_alembic_version_table()
-    click.secho('Created all tables!', fg='green')
+    click.secho("Created all tables!", fg="green")
 
 
 @db.command()
-@click.option('-v', '--verbose', is_flag=True, default=False)
-@click.option('--yes-i-know', is_flag=True, callback=abort_if_false,
-              expose_value=False,
-              prompt='Do you know that you are going to drop the db?')
+@click.option("-v", "--verbose", is_flag=True, default=False)
+@click.option(
+    "--yes-i-know",
+    is_flag=True,
+    callback=abort_if_false,
+    expose_value=False,
+    prompt="Do you know that you are going to drop the db?",
+)
 @with_appcontext
 def drop(verbose):
     """Drop tables."""
-    click.secho('Dropping all tables!', fg='red', bold=True)
-    with click.progressbar(reversed(_db.metadata.sorted_tables)) as bar:
+    click.secho("Dropping all tables!", fg="red", bold=True)
+    with click.progressbar(reversed(current_sqlalchemy.metadata.sorted_tables)) as bar:
         for table in bar:
             if verbose:
-                click.echo(' Dropping table {0}'.format(table))
-            table.drop(bind=_db.engine, checkfirst=True)
+                click.echo(" Dropping table {0}".format(table))
+            table.drop(bind=current_sqlalchemy.engine, checkfirst=True)
         drop_alembic_version_table()
-    click.secho('Dropped all tables!', fg='green')
+    click.secho("Dropped all tables!", fg="green")
 
 
 @db.command()
 @with_appcontext
 def init():
     """Create database."""
-    displayed_database = _db.engine.url.__to_string__(hide_password=True)
-    click.secho(f'Creating database {displayed_database}', fg='green')
-    database_url = str(_db.engine.url)
+    displayed_database = render_url(current_sqlalchemy.engine.url)
+    click.secho(f"Creating database {displayed_database}", fg="green")
+    database_url = str(current_sqlalchemy.engine.url)
     if not database_exists(database_url):
         create_database(database_url)
 
 
 @db.command()
-@click.option('--yes-i-know', is_flag=True, callback=abort_if_false,
-              expose_value=False,
-              prompt='Do you know that you are going to destroy the db?')
+@click.option(
+    "--yes-i-know",
+    is_flag=True,
+    callback=abort_if_false,
+    expose_value=False,
+    prompt="Do you know that you are going to destroy the db?",
+)
 @with_appcontext
 def destroy():
     """Drop database."""
-    displayed_database = _db.engine.url.__to_string__(hide_password=True)
-    click.secho(f'Destroying database {displayed_database}',
-                fg='red', bold=True)
-    if _db.engine.name == 'sqlite':
+    displayed_database = render_url(current_sqlalchemy.engine.url)
+    click.secho(f"Destroying database {displayed_database}", fg="red", bold=True)
+    if current_sqlalchemy.engine.name == "sqlite":
         try:
-            drop_database(_db.engine.url)
-        except FileNotFoundError as e:
-            click.secho('Sqlite database has not been initialised',
-                        fg='red', bold=True)
+            drop_database(current_sqlalchemy.engine.url)
+        except FileNotFoundError:
+            click.secho("Sqlite database has not been initialised", fg="red", bold=True)
     else:
-        drop_database(_db.engine.url)
+        drop_database(current_sqlalchemy.engine.url)
```

### Comparing `invenio-db-1.0.9/invenio_db/ext.py` & `invenio-db-1.1.0/invenio_db/ext.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,131 +1,147 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2018 CERN.
+# Copyright (C) 2022 RERO.
+# Copyright (C) 2022 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Database management for Invenio."""
 
-from __future__ import absolute_import, print_function
-
 import os
 
-import pkg_resources
+import importlib_metadata
+import importlib_resources
 import sqlalchemy as sa
 from flask_alembic import Alembic
 from sqlalchemy_utils.functions import get_class_by_table
 
 from .cli import db as db_cmd
 from .shared import db
 from .utils import versioning_models_registered
 
 
 class InvenioDB(object):
     """Invenio database extension."""
 
     def __init__(self, app=None, **kwargs):
         """Extension initialization."""
-        self.alembic = Alembic(run_mkdir=False, command_name='alembic')
+        self.alembic = Alembic(run_mkdir=False, command_name="alembic")
         if app:
             self.init_app(app, **kwargs)
 
     def init_app(self, app, **kwargs):
         """Initialize application object."""
         self.init_db(app, **kwargs)
 
-        app.config.setdefault('ALEMBIC', {
-            'script_location': pkg_resources.resource_filename(
-                'invenio_db', 'alembic'
-            ),
-            'version_locations': [
-                (base_entry.name, pkg_resources.resource_filename(
-                    base_entry.module_name, os.path.join(*base_entry.attrs)
-                )) for base_entry in pkg_resources.iter_entry_points(
-                    'invenio_db.alembic'
-                )
-            ],
-        })
+        script_location = str(importlib_resources.files("invenio_db") / "alembic")
+        version_locations = [
+            (
+                base_entry.name,
+                str(
+                    importlib_resources.files(base_entry.module)
+                    / os.path.join(base_entry.attr)
+                ),
+            )
+            for base_entry in importlib_metadata.entry_points(
+                group="invenio_db.alembic"
+            )
+        ]
+        app.config.setdefault(
+            "ALEMBIC",
+            {
+                "script_location": script_location,
+                "version_locations": version_locations,
+            },
+        )
+        app.config.setdefault(
+            "ALEMBIC_CONTEXT",
+            {
+                "transaction_per_migration": True,
+            },
+        )
 
         self.alembic.init_app(app)
-        app.extensions['invenio-db'] = self
+        app.extensions["invenio-db"] = self
         app.cli.add_command(db_cmd)
 
-    def init_db(self, app, entry_point_group='invenio_db.models', **kwargs):
+    def init_db(self, app, entry_point_group="invenio_db.models", **kwargs):
         """Initialize Flask-SQLAlchemy extension."""
         # Setup SQLAlchemy
         app.config.setdefault(
-            'SQLALCHEMY_DATABASE_URI',
-            'sqlite:///' + os.path.join(app.instance_path, app.name + '.db')
+            "SQLALCHEMY_DATABASE_URI",
+            "sqlite:///" + os.path.join(app.instance_path, app.name + ".db"),
         )
-        app.config.setdefault('SQLALCHEMY_ECHO', False)
+        app.config.setdefault("SQLALCHEMY_ECHO", False)
+        # Needed for before/after_flush/commit/rollback events
+        app.config.setdefault("SQLALCHEMY_TRACK_MODIFICATIONS", True)
 
         # Initialize Flask-SQLAlchemy extension.
-        database = kwargs.get('db', db)
+        database = kwargs.get("db", db)
         database.init_app(app)
 
         # Initialize versioning support.
-        self.init_versioning(app, database, kwargs.get('versioning_manager'))
+        self.init_versioning(app, database, kwargs.get("versioning_manager"))
 
         # Initialize model bases
         if entry_point_group:
-            for base_entry in pkg_resources.iter_entry_points(
-                    entry_point_group):
+            for base_entry in importlib_metadata.entry_points(group=entry_point_group):
                 base_entry.load()
 
         # All models should be loaded by now.
         sa.orm.configure_mappers()
         # Ensure that versioning classes have been built.
-        if app.config['DB_VERSIONING']:
+        if app.config["DB_VERSIONING"]:
             manager = self.versioning_manager
             if manager.pending_classes:
                 if not versioning_models_registered(manager, database.Model):
                     manager.builder.configure_versioned_classes()
-            elif 'transaction' not in database.metadata.tables:
+            elif "transaction" not in database.metadata.tables:
                 manager.declarative_base = database.Model
                 manager.create_transaction_model()
                 manager.plugins.after_build_tx_class(manager)
 
     def init_versioning(self, app, database, versioning_manager=None):
         """Initialize the versioning support using SQLAlchemy-Continuum."""
         try:
-            pkg_resources.get_distribution('sqlalchemy_continuum')
-        except pkg_resources.DistributionNotFound:  # pragma: no cover
+            importlib_metadata.version("sqlalchemy_continuum")
+        except importlib_metadata.PackageNotFoundError:  # pragma: no cover
             default_versioning = False
         else:
             default_versioning = True
 
-        app.config.setdefault('DB_VERSIONING', default_versioning)
+        app.config.setdefault("DB_VERSIONING", default_versioning)
 
-        if not app.config['DB_VERSIONING']:
+        if not app.config["DB_VERSIONING"]:
             return
 
         if not default_versioning:  # pragma: no cover
             raise RuntimeError(
-                'Please install extra versioning support first by running '
-                'pip install invenio-db[versioning].'
+                "Please install extra versioning support first by running "
+                "pip install invenio-db[versioning]."
             )
 
         # Now we can import SQLAlchemy-Continuum.
         from sqlalchemy_continuum import make_versioned
         from sqlalchemy_continuum import versioning_manager as default_vm
         from sqlalchemy_continuum.plugins import FlaskPlugin
 
         # Try to guess user model class:
-        if 'DB_VERSIONING_USER_MODEL' not in app.config:  # pragma: no cover
+        if "DB_VERSIONING_USER_MODEL" not in app.config:  # pragma: no cover
             try:
-                pkg_resources.get_distribution('invenio_accounts')
-            except pkg_resources.DistributionNotFound:
+                importlib_metadata.version("invenio_accounts")
+            except importlib_metadata.PackageNotFoundError:
                 user_cls = None
             else:
-                user_cls = 'User'
+                user_cls = "User"
         else:
-            user_cls = app.config.get('DB_VERSIONING_USER_MODEL')
+            user_cls = app.config.get("DB_VERSIONING_USER_MODEL")
 
         plugins = [FlaskPlugin()] if user_cls else []
 
         # Call make_versioned() before your models are defined.
         self.versioning_manager = versioning_manager or default_vm
         make_versioned(
             user_cls=user_cls,
```

### Comparing `invenio-db-1.0.9/invenio_db/shared.py` & `invenio-db-1.1.0/invenio_db/shared.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,100 +9,104 @@
 """Shared database object for Invenio."""
 
 from flask_sqlalchemy import SQLAlchemy as FlaskSQLAlchemy
 from sqlalchemy import MetaData, event, util
 from sqlalchemy.engine import Engine
 from werkzeug.local import LocalProxy
 
-NAMING_CONVENTION = util.immutabledict({
-    'ix': 'ix_%(column_0_label)s',
-    'uq': 'uq_%(table_name)s_%(column_0_name)s',
-    'ck': 'ck_%(table_name)s_%(constraint_name)s',
-    'fk': 'fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s',
-    'pk': 'pk_%(table_name)s',
-})
+NAMING_CONVENTION = util.immutabledict(
+    {
+        "ix": "ix_%(column_0_label)s",
+        "uq": "uq_%(table_name)s_%(column_0_name)s",
+        "ck": "ck_%(table_name)s_%(constraint_name)s",
+        "fk": "fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s",
+        "pk": "pk_%(table_name)s",
+    }
+)
 """Configuration for constraint naming conventions."""
 
 metadata = MetaData(naming_convention=NAMING_CONVENTION)
 """Default database metadata object holding associated schema constructs."""
 
 
 class SQLAlchemy(FlaskSQLAlchemy):
     """Implement or overide extension methods."""
 
-    def apply_driver_hacks(self, app, info, options):
+    def apply_driver_hacks(self, app, sa_url, options):
         """Call before engine creation."""
         # Don't forget to apply hacks defined on parent object.
-        super(SQLAlchemy, self).apply_driver_hacks(app, info, options)
+        super(SQLAlchemy, self).apply_driver_hacks(app, sa_url, options)
 
-        if info.drivername == 'sqlite':
-            connect_args = options.setdefault('connect_args', {})
+        if sa_url.drivername == "sqlite":
+            connect_args = options.setdefault("connect_args", {})
 
-            if 'isolation_level' not in connect_args:
+            if "isolation_level" not in connect_args:
                 # disable pysqlite's emitting of the BEGIN statement entirely.
                 # also stops it from emitting COMMIT before any DDL.
-                connect_args['isolation_level'] = None
+                connect_args["isolation_level"] = None
 
-            if not event.contains(Engine, 'connect', do_sqlite_connect):
-                event.listen(Engine, 'connect', do_sqlite_connect)
-            if not event.contains(Engine, 'begin', do_sqlite_begin):
-                event.listen(Engine, 'begin', do_sqlite_begin)
+            if not event.contains(Engine, "connect", do_sqlite_connect):
+                event.listen(Engine, "connect", do_sqlite_connect)
+            if not event.contains(Engine, "begin", do_sqlite_begin):
+                event.listen(Engine, "begin", do_sqlite_begin)
 
             from sqlite3 import register_adapter
 
             def adapt_proxy(proxy):
                 """Get current object and try to adapt it again."""
                 return proxy._get_current_object()
 
             register_adapter(LocalProxy, adapt_proxy)
 
-        elif info.drivername == 'postgresql+psycopg2':  # pragma: no cover
+        elif sa_url.drivername == "postgresql+psycopg2":  # pragma: no cover
             from psycopg2.extensions import adapt, register_adapter
 
             def adapt_proxy(proxy):
                 """Get current object and try to adapt it again."""
                 return adapt(proxy._get_current_object())
 
             register_adapter(LocalProxy, adapt_proxy)
 
-        elif info.drivername == 'mysql+pymysql':  # pragma: no cover
+        elif sa_url.drivername == "mysql+pymysql":  # pragma: no cover
             from pymysql import converters
 
             def escape_local_proxy(val, mapping):
                 """Get current object and try to adapt it again."""
                 return converters.escape_item(
                     val._get_current_object(),
                     self.engine.dialect.encoding,
                     mapping=mapping,
                 )
 
             converters.conversions[LocalProxy] = escape_local_proxy
             converters.encoders[LocalProxy] = escape_local_proxy
 
+        return sa_url, options
+
 
 def do_sqlite_connect(dbapi_connection, connection_record):
     """Ensure SQLite checks foreign key constraints.
 
     For further details see "Foreign key support" sections on
     https://docs.sqlalchemy.org/en/latest/dialects/sqlite.html#foreign-key-support
     """
     # Enable foreign key constraint checking
     cursor = dbapi_connection.cursor()
-    cursor.execute('PRAGMA foreign_keys=ON')
+    cursor.execute("PRAGMA foreign_keys=ON")
     cursor.close()
 
 
 def do_sqlite_begin(dbapi_connection):
     """Ensure SQLite transaction are started properly.
 
     For further details see "Foreign key support" sections on
     https://docs.sqlalchemy.org/en/rel_1_0/dialects/sqlite.html#pysqlite-serializable # noqa
     """
     # emit our own BEGIN
-    dbapi_connection.execute('BEGIN')
+    dbapi_connection.execute("BEGIN")
 
 
 db = SQLAlchemy(metadata=metadata)
 """Shared database instance using Flask-SQLAlchemy extension.
 
 This object is initialized during initialization of ``InvenioDB``
 extenstion that takes care about loading all entrypoints from key
```

### Comparing `invenio-db-1.0.9/invenio_db.egg-info/PKG-INFO` & `invenio-db-1.1.0/invenio_db.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: invenio-db
-Version: 1.0.9
+Version: 1.1.0
 Summary: Database management for Invenio.
 Home-page: https://github.com/inveniosoftware/invenio-db
-Author: Invenio Collaboration
+Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
             Copyright (C) 2015-2018 CERN.
         
             Invenio is free software; you can redistribute it and/or modify it
@@ -29,25 +29,55 @@
         .. image:: https://img.shields.io/pypi/v/invenio-db.svg
                 :target: https://pypi.org/pypi/invenio-db
         
         
         Database management for Invenio.
         Further documentation available on https://invenio-db.readthedocs.io/
         
-        
         ..
             This file is part of Invenio.
-            Copyright (C) 2015-2020 CERN.
+            Copyright (C) 2015-2023 CERN.
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.1.0 (released 2023-04-06)
+        
+        - Increase minimum version of Python to 3.7
+        - Upgrades flask-sqlalchemy
+        - Fixes deprecation warnings for flask-sqlalchemy, EncryptedType and WeakKeyDictionary
+        
+        Version 1.0.14 (released 2022-03-30)
+        
+        - Adds support for SQLAlchemy 1.4 and Flask v2.1.
+        
+        Version 1.0.13 (released 2022-02-21)
+        
+        - Changes alembic migrations to run a single migration in one transaction
+          instead of all migrations in a single transaction.
+        
+        Version 1.0.12 (released 2022-02-14)
+        
+        - Fixes a deprecation warning.
+        
+        Version 1.0.11 (released 2022-02-08)
+        
+        - Fixed issue with alembic version locations introduced in v1.0.10 due to the
+          importlib change.
+        
+        Version 1.0.10 (released 2022-02-08)
+        
+        - Adds a utility for creating an alembic test context to centrally manage
+          fixes for alembic migration tests in other modules.
+        
+        - Replaces pkg_resources with importlib
+        
         Version 1.0.9 (released 2021-03-18)
         
         - Pins Flask-SQLAlchemy below 2.5 due to breaking changes. Perhaps to revisit when fixed.
         
         Version 1.0.8 (released 2020-11-16)
         
         - Pins SQLAlchemy to >=1.2.18 and <1.4 due to incompatibility between
@@ -93,26 +123,13 @@
         
         Version 1.0.0 (released 2018-03-23)
         
         - Initial public release.
         
 Keywords: invenio database
 Platform: any
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 5 - Production/Stable
-Provides-Extra: docs
+Requires-Python: >=3.7
+Provides-Extra: tests
 Provides-Extra: mysql
 Provides-Extra: postgresql
 Provides-Extra: versioning
-Provides-Extra: tests
-Provides-Extra: all
```

### Comparing `invenio-db-1.0.9/invenio_db.egg-info/SOURCES.txt` & `invenio-db-1.1.0/invenio_db.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 .dockerignore
 .editorconfig
+.git-blame-ignore-revs
 AUTHORS.rst
 CHANGES.rst
 CONTRIBUTING.rst
 INSTALL.rst
 LICENSE
 MANIFEST.in
 README.rst
-pytest.ini
+constraints-pypi.txt
+pyproject.toml
 requirements-devel.txt
 run-tests.sh
 setup.cfg
 setup.py
 .github/workflows/pypi-publish.yml
 .github/workflows/tests.yml
 docs/Makefile
@@ -25,21 +27,20 @@
 docs/index.rst
 docs/installation.rst
 docs/license.rst
 docs/make.bat
 docs/requirements.txt
 docs/session_management.rst
 docs/usage.rst
-docs/_ext/ultramock.py
 invenio_db/__init__.py
 invenio_db/cli.py
 invenio_db/ext.py
+invenio_db/proxies.py
 invenio_db/shared.py
 invenio_db/utils.py
-invenio_db/version.py
 invenio_db.egg-info/PKG-INFO
 invenio_db.egg-info/SOURCES.txt
 invenio_db.egg-info/dependency_links.txt
 invenio_db.egg-info/entry_points.txt
 invenio_db.egg-info/not-zip-safe
 invenio_db.egg-info/requires.txt
 invenio_db.egg-info/top_level.txt
```

### Comparing `invenio-db-1.0.9/requirements-devel.txt` & `invenio-db-1.1.0/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-db-1.0.9/run-tests.sh` & `invenio-db-1.1.0/run-tests.sh`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env bash
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2020 CERN.
+# Copyright (C) 2022 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 # Quit on errors
 set -o errexit
 
@@ -16,14 +17,13 @@
 # Always bring down docker services
 function cleanup() {
     eval "$(docker-services-cli down --env)"
 }
 trap cleanup EXIT
 
 
-python -m check_manifest --ignore ".*-requirements.txt"
+python -m check_manifest
 python -m sphinx.cmd.build -qnNW docs docs/_build/html
 eval "$(docker-services-cli up --db ${DB:-postgresql} --env)"
 python -m pytest
 tests_exit_code=$?
-python -m sphinx.cmd.build -qnNW -b doctest docs docs/_build/doctest
 exit "$tests_exit_code"
```

### Comparing `invenio-db-1.0.9/tests/demo/versioned_a.py` & `invenio-db-1.1.0/tests/demo/versioned_b.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 
 from invenio_db import db
 
 
 class UnversionedArticle(db.Model):
     """Unversioned test model."""
 
-    __tablename__ = 'unversioned_article_a'
+    __tablename__ = "unversioned_article_b"
 
     id = db.Column(db.Integer, primary_key=True)
 
     name = db.Column(db.String(length=50))
 
 
 class VersionedArticle(db.Model):
     """Versioned test model."""
 
-    __tablename__ = 'versioned_article_a'
+    __tablename__ = "versioned_article_b"
     __versioned__ = {}
 
     id = db.Column(db.Integer, primary_key=True)
 
     name = db.Column(db.String(length=50))
```

### Comparing `invenio-db-1.0.9/tests/demo/versioned_b.py` & `invenio-db-1.1.0/tests/demo/versioned_a.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 
 from invenio_db import db
 
 
 class UnversionedArticle(db.Model):
     """Unversioned test model."""
 
-    __tablename__ = 'unversioned_article_b'
+    __tablename__ = "unversioned_article_a"
 
     id = db.Column(db.Integer, primary_key=True)
 
     name = db.Column(db.String(length=50))
 
 
 class VersionedArticle(db.Model):
     """Versioned test model."""
 
-    __tablename__ = 'versioned_article_b'
+    __tablename__ = "versioned_article_a"
     __versioned__ = {}
 
     id = db.Column(db.Integer, primary_key=True)
 
     name = db.Column(db.String(length=50))
```

### Comparing `invenio-db-1.0.9/tests/test_db.py` & `invenio-db-1.1.0/tests/test_db.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,86 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2018 CERN.
+# Copyright (C) 2022 RERO.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Test database integration layer."""
 
-from __future__ import absolute_import, print_function
+from unittest.mock import patch
 
 import pytest
 import sqlalchemy as sa
-from click.testing import CliRunner
-from conftest import ScriptInfo
 from flask import Flask
-from mock import patch
-from pkg_resources import EntryPoint
+from importlib_metadata import EntryPoint
+from sqlalchemy import inspect
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy_continuum import VersioningManager, remove_versioning
 from sqlalchemy_utils.functions import create_database, drop_database
 from werkzeug.utils import import_string
 
 from invenio_db import InvenioDB, shared
 from invenio_db.cli import db as db_cmd
-from invenio_db.utils import drop_alembic_version_table
+from invenio_db.utils import drop_alembic_version_table, has_table
 
 
 class MockEntryPoint(EntryPoint):
     """Mocking of entrypoint."""
 
     def load(self):
         """Mock load entry point."""
-        if self.name == 'importfail':
+        if self.name == "importfail":
             raise ImportError()
         else:
             return import_string(self.name)
 
 
 def _mock_entry_points(name):
-    data = {
-        'invenio_db.models': [MockEntryPoint('demo.child', 'demo.child'),
-                              MockEntryPoint('demo.parent', 'demo.parent')],
-        'invenio_db.models_a': [
-            MockEntryPoint('demo.versioned_a', 'demo.versioned_a'),
-        ],
-        'invenio_db.models_b': [
-            MockEntryPoint('demo.versioned_b', 'demo.versioned_b'),
-        ],
-    }
-    names = data.keys() if name is None else [name]
-    for key in names:
-        for entry_point in data.get(key, []):
-            yield entry_point
+    def fn(group):
+        data = {
+            "invenio_db.models": [
+                MockEntryPoint(name="demo.child", value="demo.child", group="test"),
+                MockEntryPoint(name="demo.parent", value="demo.parent", group="test"),
+            ],
+            "invenio_db.models_a": [
+                MockEntryPoint(
+                    name="demo.versioned_a", value="demo.versioned_a", group="test"
+                ),
+            ],
+            "invenio_db.models_b": [
+                MockEntryPoint(
+                    name="demo.versioned_b", value="demo.versioned_b", group="test"
+                ),
+            ],
+        }
+        if group:
+            return data.get(group, [])
+        if name:
+            return {name: data.get(name)}
+        return data
+
+    return fn
 
 
 def test_init(db, app):
     """Test extension initialization."""
+
     class Demo(db.Model):
-        __tablename__ = 'demo'
+        __tablename__ = "demo"
         pk = sa.Column(sa.Integer, primary_key=True)
 
     class Demo2(db.Model):
-        __tablename__ = 'demo2'
+        __tablename__ = "demo2"
         pk = sa.Column(sa.Integer, primary_key=True)
         fk = sa.Column(sa.Integer, sa.ForeignKey(Demo.pk))
 
-    app.config['DB_VERSIONING'] = False
+    app.config["DB_VERSIONING"] = False
     InvenioDB(app, entry_point_group=False, db=db)
     with app.app_context():
         db.create_all()
         assert len(db.metadata.tables) == 2
 
         # Test foreign key constraint checking
         d1 = Demo()
@@ -97,132 +107,145 @@
 
 
 def test_alembic(db, app):
     """Test alembic recipes."""
     ext = InvenioDB(app, entry_point_group=False, db=db)
 
     with app.app_context():
-        if db.engine.name == 'sqlite':
-            raise pytest.skip('Upgrades are not supported on SQLite.')
+        if db.engine.name == "sqlite":
+            raise pytest.skip("Upgrades are not supported on SQLite.")
 
         ext.alembic.upgrade()
-        ext.alembic.downgrade(target='96e796392533')
+        ext.alembic.downgrade(target="96e796392533")
 
 
 def test_naming_convention(db, app):
     """Test naming convention."""
     from sqlalchemy_continuum import remove_versioning
 
     ext = InvenioDB(app, entry_point_group=False, db=db)
     cfg = dict(
         DB_VERSIONING=True,
         DB_VERSIONING_USER_MODEL=None,
-        SQLALCHEMY_DATABASE_URI=app.config[
-            'SQLALCHEMY_DATABASE_URI'],
+        SQLALCHEMY_DATABASE_URI=app.config["SQLALCHEMY_DATABASE_URI"],
     )
 
     with app.app_context():
-        if db.engine.name == 'sqlite':
-            raise pytest.skip('Upgrades are not supported on SQLite.')
+        if db.engine.name == "sqlite":
+            raise pytest.skip("Upgrades are not supported on SQLite.")
 
     def model_factory(base):
         """Create test models."""
+
         class Master(base):
-            __tablename__ = 'master'
+            __tablename__ = "master"
             pk = sa.Column(sa.Integer, primary_key=True)
             name = sa.Column(sa.String(100), unique=True)
             city = sa.Column(sa.String(100), index=True)
-            active = sa.Column(sa.Boolean(name='active'), server_default='1')
+            active = sa.Column(sa.Boolean(name="active"), server_default="1")
 
         class Slave(base):
-            __tablename__ = 'slave'
+            __tablename__ = "slave"
             pk = sa.Column(sa.Integer, primary_key=True)
             fk = sa.Column(sa.Integer, sa.ForeignKey(Master.pk))
             code = sa.Column(sa.Integer, index=True, unique=True)
             source = sa.Column(sa.String(100))
 
             __table_args__ = (
                 sa.Index(None, source),
                 # do not add anything after
-                getattr(base, '__table_args__', {})
+                getattr(base, "__table_args__", {}),
             )
 
         return Master, Slave
 
     source_db = shared.SQLAlchemy(
-        metadata=shared.MetaData(naming_convention={
-            'ix': 'source_ix_%(table_name)s_%(column_0_label)s',
-            'uq': 'source_uq_%(table_name)s_%(column_0_name)s',
-            'ck': 'source_ck_%(table_name)s_%(constraint_name)s',
-            'fk': 'source_fk_%(table_name)s_%(column_0_name)s_'
-                  '%(referred_table_name)s',
-            'pk': 'source_pk_%(table_name)s',
-        }),
+        metadata=shared.MetaData(
+            naming_convention={
+                "ix": "source_ix_%(table_name)s_%(column_0_label)s",
+                "uq": "source_uq_%(table_name)s_%(column_0_name)s",
+                "ck": "source_ck_%(table_name)s_%(constraint_name)s",
+                "fk": "source_fk_%(table_name)s_%(column_0_name)s_"
+                "%(referred_table_name)s",
+                "pk": "source_pk_%(table_name)s",
+            }
+        ),
     )
-    source_app = Flask('source_app')
+    source_app = Flask("source_app")
     source_app.config.update(**cfg)
 
     source_models = model_factory(source_db.Model)
     source_ext = InvenioDB(
-        source_app, entry_point_group=False, db=source_db,
+        source_app,
+        entry_point_group=False,
+        db=source_db,
         versioning_manager=VersioningManager(),
     )
 
     with source_app.app_context():
         source_db.metadata.bind = source_db.engine
         source_db.create_all()
-        source_ext.alembic.stamp('dbdbc1b19cf2')
+        source_ext.alembic.stamp("dbdbc1b19cf2")
         assert not source_ext.alembic.compare_metadata()
-        source_constraints = set([
-            cns for model in source_models
-            for cns in list(model.__table__.constraints) + list(
-                model.__table__.indexes)
-        ])
+        source_constraints = set(
+            [
+                cns
+                for model in source_models
+                for cns in list(model.__table__.constraints)
+                + list(model.__table__.indexes)
+            ]
+        )
 
     remove_versioning(manager=source_ext.versioning_manager)
 
     target_db = shared.SQLAlchemy(
         metadata=shared.MetaData(naming_convention=shared.NAMING_CONVENTION)
     )
-    target_app = Flask('target_app')
+    target_app = Flask("target_app")
     target_app.config.update(**cfg)
 
     target_models = model_factory(target_db.Model)
     target_ext = InvenioDB(
-        target_app, entry_point_group=False, db=target_db,
+        target_app,
+        entry_point_group=False,
+        db=target_db,
         versioning_manager=VersioningManager(),
     )
 
     with target_app.app_context():
         target_db.metadata.bind = target_db.engine
         assert target_ext.alembic.compare_metadata()
-        target_ext.alembic.upgrade('35c1075e6360')
+        target_ext.alembic.upgrade("35c1075e6360")
         assert not target_ext.alembic.compare_metadata()
         target_db.drop_all()
-        target_constraints = set([
-            cns.name for model in source_models
-            for cns in list(model.__table__.constraints) + list(
-                model.__table__.indexes)
-        ])
+        target_constraints = set(
+            [
+                cns.name
+                for model in source_models
+                for cns in list(model.__table__.constraints)
+                + list(model.__table__.indexes)
+            ]
+        )
 
     remove_versioning(manager=target_ext.versioning_manager)
 
     assert source_constraints ^ target_constraints
 
 
 def test_transaction(db, app):
     """Test transcation commit and rollback.
 
     This is necessary to make sure that pysqlite hacks are properly working.
     """
+
     class Demo(db.Model):
-        __tablename__ = 'demo'
+        __tablename__ = "demo"
         pk = sa.Column(sa.Integer, primary_key=True)
 
-    app.config['DB_VERSIONING'] = False
+    app.config["DB_VERSIONING"] = False
     InvenioDB(app, entry_point_group=False, db=db)
 
     with app.app_context():
         db.drop_all()
         db.create_all()
         assert len(db.metadata.tables) == 1
 
@@ -261,131 +284,123 @@
         assert res[0].pk == 1
         db.session.commit()
 
     with app.app_context():
         db.drop_all()
 
 
-@patch('pkg_resources.iter_entry_points', _mock_entry_points)
+@patch("importlib_metadata.entry_points", _mock_entry_points("invenio_db.models"))
 def test_entry_points(db, app):
     """Test entrypoints loading."""
     InvenioDB(app, db=db)
 
-    runner = CliRunner()
-    script_info = ScriptInfo(create_app=lambda info: app)
+    runner = app.test_cli_runner()
 
     assert len(db.metadata.tables) == 2
 
     # Test merging a base another file.
     with runner.isolated_filesystem():
-        result = runner.invoke(db_cmd, [], obj=script_info)
+        result = runner.invoke(db_cmd, [])
         assert result.exit_code == 0
 
-        result = runner.invoke(db_cmd, ['destroy', '--yes-i-know'],
-                               obj=script_info)
+        result = runner.invoke(db_cmd, ["destroy", "--yes-i-know"])
         assert result.exit_code == 0
 
-        result = runner.invoke(db_cmd, ['init'], obj=script_info)
+        result = runner.invoke(db_cmd, ["init"])
         assert result.exit_code == 0
 
-        result = runner.invoke(db_cmd, ['create', '-v'], obj=script_info)
+        result = runner.invoke(db_cmd, ["create", "-v"])
         assert result.exit_code == 0
 
-        result = runner.invoke(db_cmd, ['drop'],
-                               obj=script_info)
+        result = runner.invoke(db_cmd, ["drop"])
         assert result.exit_code == 1
 
-        result = runner.invoke(db_cmd, ['drop', '-v', '--yes-i-know'],
-                               obj=script_info)
+        result = runner.invoke(db_cmd, ["drop", "-v", "--yes-i-know"])
         assert result.exit_code == 0
 
-        result = runner.invoke(db_cmd, ['drop', 'create'],
-                               obj=script_info)
+        result = runner.invoke(db_cmd, ["drop", "create"])
         assert result.exit_code == 1
 
-        result = runner.invoke(db_cmd, ['drop', '--yes-i-know', 'create'],
-                               obj=script_info)
+        result = runner.invoke(db_cmd, ["drop", "--yes-i-know", "create"])
         assert result.exit_code == 0
 
-        result = runner.invoke(db_cmd, ['destroy'],
-                               obj=script_info)
+        result = runner.invoke(db_cmd, ["destroy"])
         assert result.exit_code == 1
 
-        result = runner.invoke(db_cmd, ['destroy', '--yes-i-know'],
-                               obj=script_info)
+        result = runner.invoke(db_cmd, ["destroy", "--yes-i-know"])
         assert result.exit_code == 0
 
-        result = runner.invoke(db_cmd, ['init'], obj=script_info)
+        result = runner.invoke(db_cmd, ["init"])
         assert result.exit_code == 0
 
 
 def test_local_proxy(app, db):
     """Test local proxy filter."""
-    from werkzeug.local import LocalProxy
-
     InvenioDB(app, db=db)
 
     with app.app_context():
-        query = db.select([
-            db.literal('hello') != db.bindparam('a'),
-            db.literal(0) <= db.bindparam('x'),
-            db.literal('2') == db.bindparam('y'),
-            db.literal(None).is_(db.bindparam('z')),
-        ])
+        query = db.select(
+            [
+                db.literal("hello") != db.bindparam("a"),
+                db.literal(0) <= db.bindparam("x"),
+                db.literal("2") == db.bindparam("y"),
+                db.literal(None).is_(db.bindparam("z")),
+            ]
+        )
         result = db.engine.execute(
             query,
-            a=LocalProxy(lambda: 'world'),
-            x=LocalProxy(lambda: 1),
-            y=LocalProxy(lambda: '2'),
-            z=LocalProxy(lambda: None),
+            a="world",
+            x=1,
+            y="2",
+            z=None,
         ).fetchone()
         assert result == (True, True, True, True)
 
 
 def test_db_create_alembic_upgrade(app, db):
     """Test that 'db create/drop' and 'alembic create' are compatible.
 
     It also checks that "alembic_version" table is processed properly
     as it is normally created by alembic and not by sqlalchemy.
     """
-    app.config['DB_VERSIONING'] = True
-    ext = InvenioDB(app, entry_point_group=None, db=db,
-                    versioning_manager=VersioningManager())
+    app.config["DB_VERSIONING"] = True
+    ext = InvenioDB(
+        app, entry_point_group=None, db=db, versioning_manager=VersioningManager()
+    )
     with app.app_context():
         try:
-            if db.engine.name == 'sqlite':
-                raise pytest.skip('Upgrades are not supported on SQLite.')
+            if db.engine.name == "sqlite":
+                raise pytest.skip("Upgrades are not supported on SQLite.")
             db.drop_all()
-            runner = CliRunner()
-            script_info = ScriptInfo(create_app=lambda info: app)
+            runner = app.test_cli_runner()
             # Check that 'db create' creates the same schema as
             # 'alembic upgrade'.
-            result = runner.invoke(db_cmd, ['create', '-v'], obj=script_info)
+            result = runner.invoke(db_cmd, ["create", "-v"])
             assert result.exit_code == 0
-            assert db.engine.has_table('transaction')
+            assert has_table(db.engine, "transaction")
             assert ext.alembic.migration_context._has_version_table()
             # Note that compare_metadata does not detect additional sequences
             # and constraints.
-            assert not ext.alembic.compare_metadata()
+            # Note: this compare_metadata leads on mysql8 to a not finishing test
+            # assert not ext.alembic.compare_metadata()
             ext.alembic.upgrade()
-            assert db.engine.has_table('transaction')
+            assert has_table(db.engine, "transaction")
 
-            ext.alembic.downgrade(target='96e796392533')
-            assert db.engine.table_names() == ['alembic_version']
+            ext.alembic.downgrade(target="96e796392533")
+            assert inspect(db.engine).get_table_names() == ["alembic_version"]
 
             # Check that 'db drop' removes all tables, including
             # 'alembic_version'.
             ext.alembic.upgrade()
-            result = runner.invoke(db_cmd, ['drop', '-v', '--yes-i-know'],
-                                   obj=script_info)
+            result = runner.invoke(db_cmd, ["drop", "-v", "--yes-i-know"])
             assert result.exit_code == 0
-            assert len(db.engine.table_names()) == 0
+            assert len(inspect(db.engine).get_table_names()) == 0
 
             ext.alembic.upgrade()
             db.drop_all()
             drop_alembic_version_table()
-            assert len(db.engine.table_names()) == 0
+            assert len(inspect(db.engine).get_table_names()) == 0
 
         finally:
             drop_database(str(db.engine.url))
             remove_versioning(manager=ext.versioning_manager)
             create_database(str(db.engine.url))
```

### Comparing `invenio-db-1.0.9/tests/test_utils.py` & `invenio-db-1.1.0/tests/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,37 +6,39 @@
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Test DB utilities."""
 
 import pytest
 import sqlalchemy as sa
-from mock import patch
 from sqlalchemy_continuum import remove_versioning
-from sqlalchemy_utils.types import EncryptedType
-from test_db import _mock_entry_points
+from sqlalchemy_utils.types import StringEncryptedType
 
 from invenio_db import InvenioDB
-from invenio_db.utils import rebuild_encrypted_properties, \
-    versioning_model_classname, versioning_models_registered
+from invenio_db.utils import (
+    rebuild_encrypted_properties,
+    versioning_model_classname,
+    versioning_models_registered,
+)
 
 
 def test_rebuild_encrypted_properties(db, app):
     old_secret_key = "SECRET_KEY_1"
     new_secret_key = "SECRET_KEY_2"
     app.secret_key = old_secret_key
 
     def _secret_key():
-        return app.config.get('SECRET_KEY').encode('utf-8')
+        return app.config.get("SECRET_KEY").encode("utf-8")
 
     class Demo(db.Model):
-        __tablename__ = 'demo'
+        __tablename__ = "demo"
         pk = db.Column(sa.Integer, primary_key=True)
         et = db.Column(
-            EncryptedType(type_in=db.Unicode, key=_secret_key), nullable=False
+            StringEncryptedType(length=255, type_in=db.Unicode, key=_secret_key),
+            nullable=False,
         )
 
     InvenioDB(app, entry_point_group=False, db=db)
 
     with app.app_context():
         db.create_all()
         d1 = Demo(et="something")
@@ -45,38 +47,37 @@
 
     app.secret_key = new_secret_key
 
     with app.app_context():
         with pytest.raises(ValueError):
             db.session.query(Demo).all()
         with pytest.raises(AttributeError):
-            rebuild_encrypted_properties(old_secret_key, Demo, ['nonexistent'])
+            rebuild_encrypted_properties(old_secret_key, Demo, ["nonexistent"], db)
         assert app.secret_key == new_secret_key
 
     with app.app_context():
         with pytest.raises(ValueError):
             db.session.query(Demo).all()
-        rebuild_encrypted_properties(old_secret_key, Demo, ['et'])
+        rebuild_encrypted_properties(old_secret_key, Demo, ["et"], db)
         d1_after = db.session.query(Demo).first()
         assert d1_after.et == "something"
 
     with app.app_context():
         db.drop_all()
 
 
 def test_versioning_model_classname(db, app):
     """Test the versioning model utilities."""
+
     class FooClass(db.Model):
         __versioned__ = {}
         pk = db.Column(db.Integer, primary_key=True)
 
-    app.config['DB_VERSIONING'] = True
+    app.config["DB_VERSIONING"] = True
     idb = InvenioDB(app)
     manager = idb.versioning_manager
-    manager.options['use_module_name'] = True
-    assert versioning_model_classname(manager, FooClass) == \
-        'Test_UtilsFooClassVersion'
-    manager.options['use_module_name'] = False
-    assert versioning_model_classname(
-        manager, FooClass) == 'FooClassVersion'
+    manager.options["use_module_name"] = True
+    assert versioning_model_classname(manager, FooClass) == "Test_UtilsFooClassVersion"
+    manager.options["use_module_name"] = False
+    assert versioning_model_classname(manager, FooClass) == "FooClassVersion"
     assert versioning_models_registered(manager, db.Model)
     remove_versioning(manager=manager)
```

### Comparing `invenio-db-1.0.9/tests/test_versioning.py` & `invenio-db-1.1.0/tests/test_versioning.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2018 CERN.
+# Copyright (C) 2022 RERO.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Versioning tests for Invenio-DB"""
 
+from unittest.mock import patch
+
 import pytest
-from mock import patch
-from sqlalchemy_continuum import VersioningManager, make_versioned, \
-    remove_versioning
+from sqlalchemy_continuum import VersioningManager, remove_versioning
 from test_db import _mock_entry_points
 
 from invenio_db import InvenioDB
 
 
-@patch('pkg_resources.iter_entry_points', _mock_entry_points)
+@patch("importlib_metadata.entry_points", _mock_entry_points("invenio_db.models_a"))
 def test_disabled_versioning(db, app):
     """Test SQLAlchemy-Continuum with disabled versioning."""
-    InvenioDB(app, entry_point_group='invenio_db.models_a')
+    InvenioDB(app, entry_point_group="invenio_db.models_a")
 
     with app.app_context():
         assert 2 == len(db.metadata.tables)
 
 
-@pytest.mark.parametrize("versioning,tables", [
-    (False, 1),  (True, 3)
-])
+@pytest.mark.parametrize("versioning,tables", [(False, 1), (True, 3)])
 def test_disabled_versioning_with_custom_table(db, app, versioning, tables):
     """Test SQLAlchemy-Continuum table loading."""
-    app.config['DB_VERSIONING'] = versioning
+    app.config["DB_VERSIONING"] = versioning
 
     class EarlyClass(db.Model):
-
         __versioned__ = {}
 
         pk = db.Column(db.Integer, primary_key=True)
 
-    idb = InvenioDB(app, entry_point_group=None, db=db,
-                    versioning_manager=VersioningManager())
+    idb = InvenioDB(
+        app, entry_point_group=None, db=db, versioning_manager=VersioningManager()
+    )
 
     with app.app_context():
         db.drop_all()
         db.create_all()
 
         before = len(db.metadata.tables)
         ec = EarlyClass()
@@ -56,43 +55,48 @@
 
         db.drop_all()
 
     if versioning:
         remove_versioning(manager=idb.versioning_manager)
 
 
-@patch('pkg_resources.iter_entry_points', _mock_entry_points)
+@patch("importlib_metadata.entry_points", _mock_entry_points("invenio_db.models_b"))
 def test_versioning(db, app):
     """Test SQLAlchemy-Continuum enabled versioning."""
-    app.config['DB_VERSIONING'] = True
+    app.config["DB_VERSIONING"] = True
 
-    idb = InvenioDB(app, entry_point_group='invenio_db.models_b', db=db,
-                    versioning_manager=VersioningManager())
+    idb = InvenioDB(
+        app,
+        entry_point_group="invenio_db.models_b",
+        db=db,
+        versioning_manager=VersioningManager(),
+    )
 
     with app.app_context():
         assert 4 == len(db.metadata.tables)
 
         db.create_all()
 
         from demo.versioned_b import UnversionedArticle, VersionedArticle
-        original_name = 'original_name'
+
+        original_name = "original_name"
 
         versioned = VersionedArticle()
         unversioned = UnversionedArticle()
 
         versioned.name = original_name
         unversioned.name = original_name
 
         db.session.add(versioned)
         db.session.add(unversioned)
         db.session.commit()
 
         assert unversioned.name == versioned.name
 
-        modified_name = 'modified_name'
+        modified_name = "modified_name"
 
         versioned.name = modified_name
         unversioned.name = modified_name
         db.session.commit()
 
         assert unversioned.name == modified_name
         assert versioned.name == modified_name
@@ -113,16 +117,17 @@
         db.drop_all()
 
     remove_versioning(manager=idb.versioning_manager)
 
 
 def test_versioning_without_versioned_tables(db, app):
     """Test SQLAlchemy-Continuum without versioned tables."""
-    app.config['DB_VERSIONING'] = True
+    app.config["DB_VERSIONING"] = True
 
-    idb = InvenioDB(app, db=db, entry_point_group=None,
-                    versioning_manager=VersioningManager())
+    idb = InvenioDB(
+        app, db=db, entry_point_group=None, versioning_manager=VersioningManager()
+    )
 
     with app.app_context():
-        assert 'transaction' in db.metadata.tables
+        assert "transaction" in db.metadata.tables
 
     remove_versioning(manager=idb.versioning_manager)
```

