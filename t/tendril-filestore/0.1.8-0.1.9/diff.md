# Comparing `tmp/tendril-filestore-0.1.8.tar.gz` & `tmp/tendril-filestore-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-filestore-0.1.8.tar", last modified: Wed Dec 14 16:21:30 2022, max compression
+gzip compressed data, was "tendril-filestore-0.1.9.tar", last modified: Wed Dec 14 20:31:12 2022, max compression
```

## Comparing `tendril-filestore-0.1.8.tar` & `tendril-filestore-0.1.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.796031 tendril-filestore-0.1.8/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3983 2022-12-14 16:21:30.796031 tendril-filestore-0.1.8/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.792031 tendril-filestore-0.1.8/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.792031 tendril-filestore-0.1.8/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.792031 tendril-filestore-0.1.8/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-07 18:38:54.000000 tendril-filestore-0.1.8/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.792031 tendril-filestore-0.1.8/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      943 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.792031 tendril-filestore-0.1.8/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2022-12-14 16:21:30.800031 tendril-filestore-0.1.8/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3281 2022-12-11 14:50:39.000000 tendril-filestore-0.1.8/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.788031 tendril-filestore-0.1.8/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.792031 tendril-filestore-0.1.8/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.792031 tendril-filestore-0.1.8/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-25 03:24:33.000000 tendril-filestore-0.1.8/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.796031 tendril-filestore-0.1.8/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-07 14:54:45.000000 tendril-filestore-0.1.8/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5842 2022-12-14 15:34:06.000000 tendril-filestore-0.1.8/src/tendril/apiserver/routers/filestore.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.796031 tendril-filestore-0.1.8/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-10 07:41:07.000000 tendril-filestore-0.1.8/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.796031 tendril-filestore-0.1.8/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      212 2022-12-10 07:41:07.000000 tendril-filestore-0.1.8/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      157 2022-12-10 07:41:07.000000 tendril-filestore-0.1.8/src/tendril/authz/scopes/filestore.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.796031 tendril-filestore-0.1.8/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-03-20 07:52:05.000000 tendril-filestore-0.1.8/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3304 2022-12-11 09:56:27.000000 tendril-filestore-0.1.8/src/tendril/config/filestore.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2578 2022-12-11 09:56:27.000000 tendril-filestore-0.1.8/src/tendril/config/filestore_core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.796031 tendril-filestore-0.1.8/src/tendril/filestore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-09 07:18:42.000000 tendril-filestore-0.1.8/src/tendril/filestore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6081 2022-12-14 16:08:45.000000 tendril-filestore-0.1.8/src/tendril/filestore/actual.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1389 2022-12-14 14:41:06.000000 tendril-filestore-0.1.8/src/tendril/filestore/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2839 2022-12-11 09:56:27.000000 tendril-filestore-0.1.8/src/tendril/filestore/buckets.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.796031 tendril-filestore-0.1.8/src/tendril/filestore/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-09 14:37:31.000000 tendril-filestore-0.1.8/src/tendril/filestore/db/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4693 2022-12-14 15:29:12.000000 tendril-filestore-0.1.8/src/tendril/filestore/db/controller.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1290 2022-12-11 09:56:27.000000 tendril-filestore-0.1.8/src/tendril/filestore/db/model.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      101 2022-12-11 09:56:27.000000 tendril-filestore-0.1.8/src/tendril/filestore/remote.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.796031 tendril-filestore-0.1.8/src/tendril_filestore.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3983 2022-12-14 16:21:30.000000 tendril-filestore-0.1.8/src/tendril_filestore.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1250 2022-12-14 16:21:30.000000 tendril-filestore-0.1.8/src/tendril_filestore.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2022-12-14 16:21:30.000000 tendril-filestore-0.1.8/src/tendril_filestore.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      585 2022-12-14 16:21:30.000000 tendril-filestore-0.1.8/src/tendril_filestore.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2022-12-14 16:21:30.000000 tendril-filestore-0.1.8/src/tendril_filestore.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 16:21:30.796031 tendril-filestore-0.1.8/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-08 05:32:22.000000 tendril-filestore-0.1.8/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.217102 tendril-filestore-0.1.9/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3983 2022-12-14 20:31:12.217102 tendril-filestore-0.1.9/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.205102 tendril-filestore-0.1.9/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.209102 tendril-filestore-0.1.9/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.209102 tendril-filestore-0.1.9/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-07 18:38:54.000000 tendril-filestore-0.1.9/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.209102 tendril-filestore-0.1.9/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      943 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.213102 tendril-filestore-0.1.9/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2022-12-14 20:31:12.217102 tendril-filestore-0.1.9/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3281 2022-12-11 14:50:39.000000 tendril-filestore-0.1.9/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.201102 tendril-filestore-0.1.9/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.213102 tendril-filestore-0.1.9/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.213102 tendril-filestore-0.1.9/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-25 03:24:33.000000 tendril-filestore-0.1.9/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.213102 tendril-filestore-0.1.9/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-07 14:54:45.000000 tendril-filestore-0.1.9/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6908 2022-12-14 20:17:30.000000 tendril-filestore-0.1.9/src/tendril/apiserver/routers/filestore.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.213102 tendril-filestore-0.1.9/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-10 07:41:07.000000 tendril-filestore-0.1.9/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.213102 tendril-filestore-0.1.9/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      212 2022-12-10 07:41:07.000000 tendril-filestore-0.1.9/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      157 2022-12-10 07:41:07.000000 tendril-filestore-0.1.9/src/tendril/authz/scopes/filestore.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.213102 tendril-filestore-0.1.9/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-03-20 07:52:05.000000 tendril-filestore-0.1.9/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3304 2022-12-11 09:56:27.000000 tendril-filestore-0.1.9/src/tendril/config/filestore.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2578 2022-12-11 09:56:27.000000 tendril-filestore-0.1.9/src/tendril/config/filestore_core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.217102 tendril-filestore-0.1.9/src/tendril/filestore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-09 07:18:42.000000 tendril-filestore-0.1.9/src/tendril/filestore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5998 2022-12-14 18:06:40.000000 tendril-filestore-0.1.9/src/tendril/filestore/actual.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1389 2022-12-14 14:41:06.000000 tendril-filestore-0.1.9/src/tendril/filestore/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2839 2022-12-11 09:56:27.000000 tendril-filestore-0.1.9/src/tendril/filestore/buckets.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.217102 tendril-filestore-0.1.9/src/tendril/filestore/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-09 14:37:31.000000 tendril-filestore-0.1.9/src/tendril/filestore/db/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5289 2022-12-14 20:29:18.000000 tendril-filestore-0.1.9/src/tendril/filestore/db/controller.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1290 2022-12-11 09:56:27.000000 tendril-filestore-0.1.9/src/tendril/filestore/db/model.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      101 2022-12-11 09:56:27.000000 tendril-filestore-0.1.9/src/tendril/filestore/remote.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.217102 tendril-filestore-0.1.9/src/tendril_filestore.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3983 2022-12-14 20:31:12.000000 tendril-filestore-0.1.9/src/tendril_filestore.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1250 2022-12-14 20:31:12.000000 tendril-filestore-0.1.9/src/tendril_filestore.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2022-12-14 20:31:12.000000 tendril-filestore-0.1.9/src/tendril_filestore.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      585 2022-12-14 20:31:12.000000 tendril-filestore-0.1.9/src/tendril_filestore.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2022-12-14 20:31:12.000000 tendril-filestore-0.1.9/src/tendril_filestore.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:31:12.217102 tendril-filestore-0.1.9/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-08 05:32:22.000000 tendril-filestore-0.1.9/tox.ini
```

### Comparing `tendril-filestore-0.1.8/.gitignore` & `tendril-filestore-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/.readthedocs.yml` & `tendril-filestore-0.1.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/.travis.yml` & `tendril-filestore-0.1.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/LICENSE` & `tendril-filestore-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/PKG-INFO` & `tendril-filestore-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-filestore
-Version: 0.1.8
+Version: 0.1.9
 Summary: File Storage and Management Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-filestore
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 License: UNKNOWN
 Project-URL: Documentation, https://tendril-filestore.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-filestore/issues
```

### Comparing `tendril-filestore-0.1.8/README.rst` & `tendril-filestore-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/docs/Makefile` & `tendril-filestore-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/docs/_static/custom.css` & `tendril-filestore-0.1.9/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/docs/_static/favicon.ico` & `tendril-filestore-0.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/docs/_static/logo.png` & `tendril-filestore-0.1.9/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/docs/_static/logo_packed.png` & `tendril-filestore-0.1.9/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/docs/_templates/about.html` & `tendril-filestore-0.1.9/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/docs/conf.py` & `tendril-filestore-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/docs/index.rst` & `tendril-filestore-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/docs/installation.rst` & `tendril-filestore-0.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/setup.py` & `tendril-filestore-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/src/tendril/apiserver/routers/filestore.py` & `tendril-filestore-0.1.9/src/tendril/apiserver/routers/filestore.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 
 
 import json
+import datetime
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import Request
 from fastapi import File
 from fastapi import UploadFile
 from fastapi import HTTPException
 from fastapi import Body
+from fastapi_pagination import Page
+from fastapi_pagination import Params
+from fastapi_pagination import add_pagination
+
+from typing import Union
+from pydantic import Field
+from pydantic import validator
 
-from pydantic import BaseModel
-
-from tendril.authn.users import authn_dependency
-from tendril.authn.users import AuthUserModel
 from tendril.authn.users import auth_spec
+from tendril.authn.users import AuthUserModel
+from tendril.authn.users import authn_dependency
+from tendril.authn.users import UserStubTMixin
+
 from tendril.filestore.buckets import available_buckets
 from tendril.filestore.buckets import get_bucket
 from tendril.filestore.actual import FilestoreBucket
 
+from tendril.utils.pydantic import TendrilTBaseModel
+
 from tendril.config import FILESTORE_ENABLED
 
 
 filestore = APIRouter(prefix='/filestore',
                       tags=["File Management API"],
                       dependencies=[Depends(authn_dependency),
                                     auth_spec(scopes=['file_management:common'])])
@@ -56,15 +66,15 @@
     @classmethod
     def validate(cls, v):
         if v not in _available_buckets:
             raise ValueError(f"'{v}' is not in {_available_buckets}")
         return cls(v)
 
 
-class MoveRequest(BaseModel):
+class MoveRequest(TendrilTBaseModel):
     to_bucket: BucketName
     filename: str
     overwrite : bool = False
 
 
 @filestore.get("/buckets")
 async def get_available_buckets():
@@ -165,27 +175,50 @@
         raise HTTPException(
             status_code=403,
             detail=str(e)
         )
     return {'deleted': filename}
 
 
-@filestore_management.post("/{bucket}/ls")
+class StoredFilePropsTModel(TendrilTBaseModel):
+    size: int = Field(..., example=714794)
+    created: Union[datetime.datetime, None]
+    modified: Union[datetime.datetime, None]
+
+
+class StoredFileHashTModel(TendrilTBaseModel):
+    sha256: str = Field(..., example='e4dd9b81d05aec0ce7f3a66b9efd15a13da5dae6e6672b84c7a75b3504c22d43')
+
+
+class StoredFileInfoTModel(TendrilTBaseModel):
+    ext: str = Field(..., example='.jpg')
+    hash: StoredFileHashTModel
+    props: StoredFilePropsTModel
+
+
+class StoredFileTModel(UserStubTMixin(out='owner'), TendrilTBaseModel):
+    filename: str = Field(..., example="some_filename.jpg")
+    fileinfo: StoredFileInfoTModel
+
+
+@filestore_management.post("/{bucket}/ls",
+                           response_model=Page[StoredFileTModel])
 async def list_files_in_bucket(
         request: Request,
         bucket: BucketName,
+        params: Params = Depends(),
         user: AuthUserModel = auth_spec()):
     try:
         bucket: FilestoreBucket = get_bucket(bucket)
     except KeyError:
         raise HTTPException(
             status_code=404,
             detail=f'{bucket} is not a recognized filestore bucket'
         )
-    return bucket.list_info()
+    return bucket.list_info(params)
 
 
 @filestore_management.post("/{bucket}/purge")
 async def purge_all_files_in_bucket(
         request: Request,
         bucket: BucketName,
         user: AuthUserModel = auth_spec()):
```

### Comparing `tendril-filestore-0.1.8/src/tendril/config/__init__.py` & `tendril-filestore-0.1.9/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/src/tendril/config/filestore.py` & `tendril-filestore-0.1.9/src/tendril/config/filestore.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/src/tendril/config/filestore_core.py` & `tendril-filestore-0.1.9/src/tendril/config/filestore_core.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/src/tendril/filestore/actual.py` & `tendril-filestore-0.1.9/src/tendril/filestore/actual.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from tendril.authn.users import get_user_stub
 from tendril.filestore.base import FilestoreBucketBase
 from tendril.filestore.db.controller import register_bucket
 from tendril.filestore.db.controller import get_storedfile_owner
 from tendril.filestore.db.controller import register_stored_file
 from tendril.filestore.db.controller import change_file_bucket
 from tendril.filestore.db.controller import delete_stored_file
-from tendril.filestore.db.controller import get_stored_files
+from tendril.filestore.db.controller import get_paginated_stored_files
 
 from tendril.utils.db import with_db
 from tendril.utils.db import get_session
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEFAULT)
 
 
@@ -136,19 +136,18 @@
                                    exclude_dirs=self._exclude_directories):
             yield f.name
 
     def list(self, page=None):
         return list(self._list(page=page))
 
     @with_db
-    def list_info(self, page=None, session=None):
+    def list_info(self, params, page=None, session=None):
         items = self.list(page)
-        infos = get_stored_files(filenames=items, bucket=self.id, session=session)
-        return {x.filename: {'info': x.fileinfo,
-                             'owner': get_user_stub(x.user.puid)} for x in infos}
+        return get_paginated_stored_files(
+            params, filenames=items, bucket=self.id, session=session)
 
     def purge(self, user):
         if not self._allow_delete:
             raise PermissionError(f"Deletion of files from bucket {self.name} "
                                   f"is not permitted")
         logger.warning(f"Purging all files from bucket {self.name}")
         for filename in self.list():
```

### Comparing `tendril-filestore-0.1.8/src/tendril/filestore/base.py` & `tendril-filestore-0.1.9/src/tendril/filestore/base.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/src/tendril/filestore/buckets.py` & `tendril-filestore-0.1.9/src/tendril/filestore/buckets.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/src/tendril/filestore/db/controller.py` & `tendril-filestore-0.1.9/src/tendril/filestore/db/controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 
 
+from fastapi_pagination.ext.sqlalchemy import paginate
 from sqlalchemy.orm.exc import NoResultFound
+
 from tendril.utils.db import with_db
+from tendril.authn.db.model import User
 from tendril.authn.db.controller import preprocess_user
 from tendril.artefacts.db.controller import get_artefact_owner
 from tendril import config
 
 from .model import FilestoreBucketModel
 from .model import StoredFileModel
 
@@ -64,23 +67,39 @@
     if bucket:
         bucket_id = preprocess_bucket(bucket, session=session)
         q.filter_by(bucket_id=bucket_id)
     return q.one()
 
 
 @with_db
-def get_stored_files(filenames, bucket, session=None):
+def get_stored_files(bucket, filenames=None, session=None):
     bucket_id = preprocess_bucket(bucket, session=None)
-    q = session.query(StoredFileModel).\
-        filter_by(bucket_id=bucket_id).\
-        filter(StoredFileModel.filename.in_(filenames))
+    filters = [StoredFileModel.bucket_id == bucket_id]
+
+    if filenames:
+        filters.append(StoredFileModel.filename.in_(filenames))
+
+    q = session.query(StoredFileModel).filter(*filters)
     return q.all()
 
 
 @with_db
+def get_paginated_stored_files(params, bucket, filenames=None, session=None):
+    bucket_id = preprocess_bucket(bucket, session=None)
+    filters = [StoredFileModel.bucket_id == bucket_id]
+
+    if filenames:
+        filters.append(StoredFileModel.filename.in_(filenames))
+
+    q = session.query(StoredFileModel.filename, StoredFileModel.fileinfo, User.puid).\
+        join(User).filter(*filters)
+    return paginate(q, params)
+
+
+@with_db
 def register_stored_file(filename, bucket, user, fileinfo=None, overwrite=True, session=None):
     if not config.FILESTORE_ENABLED:
         raise EnvironmentError("Filestore not enabled on this component. "
                                "Use the filestore API on the filestore component instead.")
 
     if filename is None:
         raise AttributeError("name cannot be None")
```

### Comparing `tendril-filestore-0.1.8/src/tendril/filestore/db/model.py` & `tendril-filestore-0.1.9/src/tendril/filestore/db/model.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/src/tendril_filestore.egg-info/PKG-INFO` & `tendril-filestore-0.1.9/src/tendril_filestore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-filestore
-Version: 0.1.8
+Version: 0.1.9
 Summary: File Storage and Management Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-filestore
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 License: UNKNOWN
 Project-URL: Documentation, https://tendril-filestore.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-filestore/issues
```

### Comparing `tendril-filestore-0.1.8/src/tendril_filestore.egg-info/SOURCES.txt` & `tendril-filestore-0.1.9/src/tendril_filestore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/src/tendril_filestore.egg-info/requires.txt` & `tendril-filestore-0.1.9/src/tendril_filestore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/tests/coveralls.py` & `tendril-filestore-0.1.9/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.1.8/tox.ini` & `tendril-filestore-0.1.9/tox.ini`

 * *Files identical despite different names*

