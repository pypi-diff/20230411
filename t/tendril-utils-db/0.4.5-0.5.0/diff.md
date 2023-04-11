# Comparing `tmp/tendril-utils-db-0.4.5.tar.gz` & `tmp/tendril-utils-db-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tendril-utils-db-0.4.5.tar", last modified: Tue Mar 28 18:12:00 2023, max compression
+gzip compressed data, was "tendril-utils-db-0.5.0.tar", last modified: Tue Apr 11 18:44:21 2023, max compression
```

## Comparing `tendril-utils-db-0.4.5.tar` & `tendril-utils-db-0.5.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.765604 tendril-utils-db-0.4.5/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3927 2023-03-28 18:12:00.765604 tendril-utils-db-0.4.5/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2205 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/README.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2109 2022-12-08 14:04:07.000000 tendril-utils-db-0.4.5/alembic.ini
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.757605 tendril-utils-db-0.4.5/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.761605 tendril-utils-db-0.4.5/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.761605 tendril-utils-db-0.4.5/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.761605 tendril-utils-db-0.4.5/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13493 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      869 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1643 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.761605 tendril-utils-db-0.4.5/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-03-28 18:12:00.765604 tendril-utils-db-0.4.5/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3310 2022-12-15 17:03:18.000000 tendril-utils-db-0.4.5/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.753606 tendril-utils-db-0.4.5/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.761605 tendril-utils-db-0.4.5/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:40.000000 tendril-utils-db-0.4.5/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.761605 tendril-utils-db-0.4.5/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2812 2023-03-28 18:11:09.000000 tendril-utils-db-0.4.5/src/tendril/config/db.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1599 2022-12-08 13:59:11.000000 tendril-utils-db-0.4.5/src/tendril/config/db_core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.761605 tendril-utils-db-0.4.5/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-08 13:59:11.000000 tendril-utils-db-0.4.5/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.761605 tendril-utils-db-0.4.5/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.4.5/src/tendril/db/controllers/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.761605 tendril-utils-db-0.4.5/src/tendril/db/migration/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2022-12-08 13:59:11.000000 tendril-utils-db-0.4.5/src/tendril/db/migration/README
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.4.5/src/tendril/db/migration/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2206 2022-12-08 13:59:11.000000 tendril-utils-db-0.4.5/src/tendril/db/migration/env.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      494 2022-12-08 13:59:11.000000 tendril-utils-db-0.4.5/src/tendril/db/migration/script.py.mako
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.761605 tendril-utils-db-0.4.5/src/tendril/db/migration/versions/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.4.5/src/tendril/db/migration/versions/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.761605 tendril-utils-db-0.4.5/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.4.5/src/tendril/db/models/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.765604 tendril-utils-db-0.4.5/src/tendril/utils/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:49.000000 tendril-utils-db-0.4.5/src/tendril/utils/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9142 2023-03-27 16:18:52.000000 tendril-utils-db-0.4.5/src/tendril/utils/db.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.765604 tendril-utils-db-0.4.5/src/tendril_utils_db.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3927 2023-03-28 18:12:00.000000 tendril-utils-db-0.4.5/src/tendril_utils_db.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1089 2023-03-28 18:12:00.000000 tendril-utils-db-0.4.5/src/tendril_utils_db.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-03-28 18:12:00.000000 tendril-utils-db-0.4.5/src/tendril_utils_db.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      763 2023-03-28 18:12:00.000000 tendril-utils-db-0.4.5/src/tendril_utils_db.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-03-28 18:12:00.000000 tendril-utils-db-0.4.5/src/tendril_utils_db.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 18:12:00.765604 tendril-utils-db-0.4.5/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      858 2020-08-18 06:57:07.000000 tendril-utils-db-0.4.5/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3495 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2205 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/README.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2109 2022-12-08 14:04:07.000000 tendril-utils-db-0.5.0/alembic.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.929615 tendril-utils-db-0.5.0/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13493 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      869 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1643 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3310 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.0/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.921615 tendril-utils-db-0.5.0/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:40.000000 tendril-utils-db-0.5.0/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2812 2023-03-28 18:11:09.000000 tendril-utils-db-0.5.0/src/tendril/config/db.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1599 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.0/src/tendril/config/db_core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.0/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.0/src/tendril/db/controllers/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/src/tendril/db/migration/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.0/src/tendril/db/migration/README
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.0/src/tendril/db/migration/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2206 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.0/src/tendril/db/migration/env.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      494 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.0/src/tendril/db/migration/script.py.mako
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/src/tendril/db/migration/versions/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.0/src/tendril/db/migration/versions/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.0/src/tendril/db/models/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/src/tendril/utils/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:49.000000 tendril-utils-db-0.5.0/src/tendril/utils/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9578 2023-04-11 18:42:19.000000 tendril-utils-db-0.5.0/src/tendril/utils/db.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3495 2023-04-11 18:44:21.000000 tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1089 2023-04-11 18:44:21.000000 tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-11 18:44:21.000000 tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      763 2023-04-11 18:44:21.000000 tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-11 18:44:21.000000 tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      858 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/tox.ini
```

### Comparing `tendril-utils-db-0.4.5/.gitignore` & `tendril-utils-db-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/.readthedocs.yml` & `tendril-utils-db-0.5.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/.travis.yml` & `tendril-utils-db-0.5.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/LICENSE` & `tendril-utils-db-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/PKG-INFO` & `tendril-utils-db-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-utils-db
-Version: 0.4.5
+Version: 0.5.0
 Summary: Database utilities for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-db
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
 Project-URL: Documentation, https://tendril-utils-db.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-db/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-db
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-utils-db.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-utils-db
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-utils-db.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-utils-db
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-utils-db.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-utils-db
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-utils-db.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-utils-db
-        
-        .. image:: https://img.shields.io/codacy/grade/694e07c41826407480e17a1b0dc6e1bd?logo=codacy
-            :target: https://www.codacy.com/app/chintal/tendril-utils-db
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-utils-db.svg
-            :target: https://requires.io/github/tendril-framework/tendril-utils-db/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-utils-db.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
-        
-        
-        
-        .. inclusion-marker-do-not-remove
-        
-        Introduction
-        ------------
-        
-        TODO Some brief introduction
-        
-        
-        Package Information
-        -------------------
-        
-        The latest version of the documentation, including installation, usage, and
-        API/developer notes can be found at
-        `ReadTheDocs <https://tendril-utils-db.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-utils-db>`_. Please use
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-utils-db`` is Chintalagiri Shashank. The
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-utils-db`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -80,7 +25,62 @@
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
 Provides-Extra: publish
 Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-utils-db.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-utils-db
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-utils-db.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-utils-db
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-utils-db.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-utils-db
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-utils-db.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-utils-db
+
+.. image:: https://img.shields.io/codacy/grade/694e07c41826407480e17a1b0dc6e1bd?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-utils-db
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-utils-db.svg
+    :target: https://requires.io/github/tendril-framework/tendril-utils-db/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-utils-db.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
+
+
+
+.. inclusion-marker-do-not-remove
+
+Introduction
+------------
+
+TODO Some brief introduction
+
+
+Package Information
+-------------------
+
+The latest version of the documentation, including installation, usage, and
+API/developer notes can be found at
+`ReadTheDocs <https://tendril-utils-db.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-utils-db>`_. Please use
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-utils-db`` is Chintalagiri Shashank. The
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-utils-db`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
```

### Comparing `tendril-utils-db-0.4.5/README.rst` & `tendril-utils-db-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/alembic.ini` & `tendril-utils-db-0.5.0/alembic.ini`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/docs/Makefile` & `tendril-utils-db-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/docs/_static/custom.css` & `tendril-utils-db-0.5.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/docs/_static/favicon.ico` & `tendril-utils-db-0.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/docs/_static/logo.png` & `tendril-utils-db-0.5.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/docs/_static/logo_packed.png` & `tendril-utils-db-0.5.0/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/docs/_templates/about.html` & `tendril-utils-db-0.5.0/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/docs/conf.py` & `tendril-utils-db-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/docs/index.rst` & `tendril-utils-db-0.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/docs/installation.rst` & `tendril-utils-db-0.5.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/setup.py` & `tendril-utils-db-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/src/tendril/config/__init__.py` & `tendril-utils-db-0.5.0/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/src/tendril/config/db.py` & `tendril-utils-db-0.5.0/src/tendril/config/db.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/src/tendril/config/db_core.py` & `tendril-utils-db-0.5.0/src/tendril/config/db_core.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/src/tendril/db/migration/env.py` & `tendril-utils-db-0.5.0/src/tendril/db/migration/env.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/src/tendril/utils/db.py` & `tendril-utils-db-0.5.0/src/tendril/utils/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 interaction with :mod:`sqlalchemy`
 
 .. rubric:: Module Contents
 
 """
 
 import importlib
+from sqlalchemy import MetaData
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.ext.declarative import declared_attr
 from sqlalchemy import Column, Integer
 from sqlalchemy_utils import ArrowType
 
@@ -41,15 +42,15 @@
 
 from tendril.utils.versions import get_namespace_package_names
 
 from tendril.config import DATABASE_URI
 from tendril.config import DATABASE_PACKAGE_PREFIXES
 
 from tendril.utils import log
-logger = log.get_logger(__name__, log.DEFAULT)
+logger = log.get_logger(__name__, log.DEBUG)
 log.logging.getLogger('sqlalchemy.engine').setLevel(log.WARNING)
 
 try:
     from tendril.devtooling import stack
 except ImportError:
     stack = None
 
@@ -141,16 +142,28 @@
                 kwargs['session'] = s
                 return func(*args, **kwargs)
         else:
             return func(*args, **kwargs)
     return inner
 
 
+#: Database metadata object initialization
+meta = MetaData(
+    naming_convention={
+        "ix": "%(column_0_label)s_idx",
+        "uq": "%(table_name)s_%(column_0_name)s_key",
+        "ck": "%(table_name)s_%(constraint_name)s_check",
+        "fk": "%(table_name)s_%(column_0_name)s_%(referred_table_name)s_fkey",
+        "pk": "%(table_name)s_pkey"
+    }
+)
+
+
 #: The :mod:`sqlalchemy` declarative base for all Models in Tendril
-DeclBase = declarative_base()
+DeclBase = declarative_base(metadata=meta)
 
 
 class BaseMixin(object):
     """
     This Mixin can / should be used (by inheriting from) by all Model classes
     defined by application code. It defines the :attr:`__tablename__`
     attribute of the Model class to the name of the class and creates a
@@ -216,25 +229,25 @@
             if p in _excluded_prefixes:
                 continue
             logger.debug(f"Trying to load models from '{p}.db.model'")
             try:
                 modname = '{0}.db.model'.format(p)
                 globals()[modname] = importlib.import_module(modname)
                 logger.info("Loaded DB Models from {0}".format(p))
-            except ImportError:
-                pass
+            except ImportError as e:
+                logger.debug(e)
     for prefix in _user_models_prefix:
         logger.info(f"Loading Instance DB Models from '{prefix}.*")
         for p in get_namespace_package_names(prefix):
             logger.debug(f"Trying to load models from '{p}'")
             try:
                 globals()[p] = importlib.import_module(p)
                 logger.info("Loaded DB Models from {0}".format(p))
-            except ImportError:
-                pass
+            except ImportError as e:
+                logger.debug(e)
     return DeclBase.metadata
 
 
 for_create = []
 
 
 def register_for_create(func):
```

### Comparing `tendril-utils-db-0.4.5/src/tendril_utils_db.egg-info/PKG-INFO` & `tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-utils-db
-Version: 0.4.5
+Version: 0.5.0
 Summary: Database utilities for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-db
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
 Project-URL: Documentation, https://tendril-utils-db.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-db/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-db
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-utils-db.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-utils-db
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-utils-db.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-utils-db
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-utils-db.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-utils-db
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-utils-db.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-utils-db
-        
-        .. image:: https://img.shields.io/codacy/grade/694e07c41826407480e17a1b0dc6e1bd?logo=codacy
-            :target: https://www.codacy.com/app/chintal/tendril-utils-db
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-utils-db.svg
-            :target: https://requires.io/github/tendril-framework/tendril-utils-db/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-utils-db.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
-        
-        
-        
-        .. inclusion-marker-do-not-remove
-        
-        Introduction
-        ------------
-        
-        TODO Some brief introduction
-        
-        
-        Package Information
-        -------------------
-        
-        The latest version of the documentation, including installation, usage, and
-        API/developer notes can be found at
-        `ReadTheDocs <https://tendril-utils-db.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-utils-db>`_. Please use
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-utils-db`` is Chintalagiri Shashank. The
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-utils-db`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -80,7 +25,62 @@
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
 Provides-Extra: publish
 Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-utils-db.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-utils-db
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-utils-db.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-utils-db
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-utils-db.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-utils-db
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-utils-db.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-utils-db
+
+.. image:: https://img.shields.io/codacy/grade/694e07c41826407480e17a1b0dc6e1bd?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-utils-db
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-utils-db.svg
+    :target: https://requires.io/github/tendril-framework/tendril-utils-db/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-utils-db.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
+
+
+
+.. inclusion-marker-do-not-remove
+
+Introduction
+------------
+
+TODO Some brief introduction
+
+
+Package Information
+-------------------
+
+The latest version of the documentation, including installation, usage, and
+API/developer notes can be found at
+`ReadTheDocs <https://tendril-utils-db.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-utils-db>`_. Please use
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-utils-db`` is Chintalagiri Shashank. The
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-utils-db`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
```

### Comparing `tendril-utils-db-0.4.5/src/tendril_utils_db.egg-info/SOURCES.txt` & `tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/src/tendril_utils_db.egg-info/requires.txt` & `tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/tests/coveralls.py` & `tendril-utils-db-0.5.0/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.4.5/tox.ini` & `tendril-utils-db-0.5.0/tox.ini`

 * *Files identical despite different names*

