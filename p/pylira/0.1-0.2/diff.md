# Comparing `tmp/pylira-0.1.tar.gz` & `tmp/pylira-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylira-0.1.tar", last modified: Mon Mar 14 02:06:33 2022, max compression
+gzip compressed data, was "pylira-0.2.tar", last modified: Tue Apr 11 14:27:54 2023, max compression
```

## Comparing `pylira-0.1.tar` & `pylira-0.2.tar`

### file list

```diff
@@ -1,87 +1,93 @@
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.202641 pylira-0.1/
--rw-r--r--   0 adonath    (502) staff       (20)     2556 2021-11-10 13:53:11.000000 pylira-0.1/.clang-format
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.190465 pylira-0.1/.github/
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.193498 pylira-0.1/.github/workflows/
--rw-r--r--   0 adonath    (502) staff       (20)      723 2021-11-08 14:30:24.000000 pylira-0.1/.github/workflows/ci_cron_weekly.yml
--rw-r--r--   0 adonath    (502) staff       (20)     2926 2021-12-23 18:21:46.000000 pylira-0.1/.github/workflows/ci_tests.yml
--rw-r--r--   0 adonath    (502) staff       (20)      869 2021-12-17 15:33:10.000000 pylira-0.1/.gitignore
--rw-r--r--   0 adonath    (502) staff       (20)      232 2021-11-10 13:53:11.000000 pylira-0.1/.readthedocs.yml
--rw-r--r--   0 adonath    (502) staff       (20)      314 2021-12-23 18:21:46.000000 pylira-0.1/MANIFEST.in
--rw-r--r--   0 adonath    (502) staff       (20)     2895 2022-03-14 02:06:33.202743 pylira-0.1/PKG-INFO
--rw-r--r--   0 adonath    (502) staff       (20)     2481 2021-11-08 14:31:13.000000 pylira-0.1/README.rst
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.194504 pylira-0.1/docs/
--rw-r--r--   0 adonath    (502) staff       (20)     4581 2021-11-08 14:30:24.000000 pylira-0.1/docs/Makefile
--rw-r--r--   0 adonath    (502) staff       (20)     8389 2021-12-17 15:33:10.000000 pylira-0.1/docs/conf.py
--rw-r--r--   0 adonath    (502) staff       (20)      325 2021-12-17 15:33:10.000000 pylira-0.1/docs/index.rst
--rw-r--r--   0 adonath    (502) staff       (20)     4549 2021-11-08 14:30:24.000000 pylira-0.1/docs/make.bat
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.195857 pylira-0.1/docs/pylira/
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.196327 pylira-0.1/docs/pylira/api/
--rw-r--r--   0 adonath    (502) staff       (20)      172 2021-12-17 15:33:10.000000 pylira-0.1/docs/pylira/api/core.rst
--rw-r--r--   0 adonath    (502) staff       (20)      212 2021-12-17 15:33:10.000000 pylira-0.1/docs/pylira/api/data.rst
--rw-r--r--   0 adonath    (502) staff       (20)      253 2021-12-17 15:33:10.000000 pylira-0.1/docs/pylira/api/index.rst
--rw-r--r--   0 adonath    (502) staff       (20)      543 2021-12-17 15:33:10.000000 pylira-0.1/docs/pylira/api/utils.rst
--rw-r--r--   0 adonath    (502) staff       (20)       58 2021-12-17 15:33:10.000000 pylira-0.1/docs/pylira/changelog.rst
--rw-r--r--   0 adonath    (502) staff       (20)     1604 2021-12-17 15:33:10.000000 pylira-0.1/docs/pylira/developer.rst
--rw-r--r--   0 adonath    (502) staff       (20)      625 2022-03-14 01:55:12.000000 pylira-0.1/docs/pylira/index.rst
--rw-r--r--   0 adonath    (502) staff       (20)      999 2021-12-17 15:33:10.000000 pylira-0.1/docs/pylira/references.rst
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.196554 pylira-0.1/docs/pylira/user/
--rw-r--r--   0 adonath    (502) staff       (20)      922 2021-12-17 15:33:10.000000 pylira-0.1/docs/pylira/user/data.rst
--rw-r--r--   0 adonath    (502) staff       (20)     1367 2022-03-14 01:55:12.000000 pylira-0.1/docs/pylira/user/index.rst
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.196712 pylira-0.1/docs/pylira/user/tutorials/
--rw-r--r--   0 adonath    (502) staff       (20)      197 2021-12-17 15:33:10.000000 pylira-0.1/docs/pylira/user/tutorials/index.rst
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.196959 pylira-0.1/docs/pylira/user/tutorials/notebooks/
--rw-r--r--   0 adonath    (502) staff       (20)     5000 2022-03-14 01:55:12.000000 pylira-0.1/docs/pylira/user/tutorials/notebooks/mcmc-deconvolution-intro.md
--rw-r--r--   0 adonath    (502) staff       (20)     2810 2022-03-14 01:55:12.000000 pylira-0.1/docs/pylira/user/tutorials/notebooks/point_source.md
--rw-r--r--   0 adonath    (502) staff       (20)   241873 2021-11-08 14:30:24.000000 pylira-0.1/docs/pylira-logo.png
--rw-r--r--   0 adonath    (502) staff       (20)      503 2022-03-12 20:55:53.000000 pylira-0.1/environment.yaml
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.197602 pylira-0.1/licenses/
--rw-r--r--   0 adonath    (502) staff       (20)    37572 2021-11-08 14:30:24.000000 pylira-0.1/licenses/LICENSE.rst
--rw-r--r--   0 adonath    (502) staff       (20)      372 2021-11-08 14:30:24.000000 pylira-0.1/licenses/README.rst
--rw-r--r--   0 adonath    (502) staff       (20)     1659 2021-11-08 14:30:24.000000 pylira-0.1/licenses/TEMPLATE_LICENCE.rst
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.198377 pylira-0.1/pylira/
--rw-r--r--   0 adonath    (502) staff       (20)      518 2022-03-14 01:55:12.000000 pylira-0.1/pylira/__init__.py
--rw-r--r--   0 adonath    (502) staff       (20)      356 2022-03-14 01:55:12.000000 pylira-0.1/pylira/_astropy_init.py
--rw-r--r--   0 adonath    (502) staff       (20)     2095 2022-03-14 01:55:12.000000 pylira-0.1/pylira/conftest.py
--rw-r--r--   0 adonath    (502) staff       (20)    15301 2022-03-14 01:55:12.000000 pylira-0.1/pylira/core.py
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.199258 pylira-0.1/pylira/data/
--rw-r--r--   0 adonath    (502) staff       (20)      245 2021-11-08 14:30:24.000000 pylira-0.1/pylira/data/README.rst
--rw-r--r--   0 adonath    (502) staff       (20)       28 2022-03-14 01:55:12.000000 pylira-0.1/pylira/data/__init__.py
--rw-r--r--   0 adonath    (502) staff       (20)     6145 2022-03-14 01:55:12.000000 pylira-0.1/pylira/data/core.py
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.199815 pylira-0.1/pylira/data/files/
--rw-r--r--   0 adonath    (502) staff       (20)     1400 2022-02-11 22:29:29.000000 pylira-0.1/pylira/data/files/lincoln.png
--rw-r--r--   0 adonath    (502) staff       (20)    10646 2021-11-24 17:18:52.000000 pylira-0.1/pylira/data/files/output-par.txt
--rw-r--r--   0 adonath    (502) staff       (20)   102742 2021-11-24 17:18:52.000000 pylira-0.1/pylira/data/files/output.txt
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.200298 pylira-0.1/pylira/data/tests/
--rw-r--r--   0 adonath    (502) staff       (20)        0 2021-11-24 17:18:52.000000 pylira-0.1/pylira/data/tests/__init__.py
--rw-r--r--   0 adonath    (502) staff       (20)     1813 2022-03-14 01:55:12.000000 pylira-0.1/pylira/data/tests/test_core.py
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.200435 pylira-0.1/pylira/extern/
--rw-r--r--   0 adonath    (502) staff       (20)      220 2021-11-08 14:30:24.000000 pylira-0.1/pylira/extern/__init__.py
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.201057 pylira-0.1/pylira/src/
--rw-r--r--   0 adonath    (502) staff       (20)    74607 2021-12-28 20:47:23.000000 pylira-0.1/pylira/src/lira.h
--rw-r--r--   0 adonath    (502) staff       (20)     3395 2021-12-03 21:31:53.000000 pylira-0.1/pylira/src/lirabind.cpp
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.201377 pylira-0.1/pylira/tests/
--rw-r--r--   0 adonath    (502) staff       (20)      108 2021-11-08 14:30:24.000000 pylira-0.1/pylira/tests/__init__.py
--rw-r--r--   0 adonath    (502) staff       (20)     6941 2022-03-14 01:55:12.000000 pylira-0.1/pylira/tests/test_core.py
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.202027 pylira-0.1/pylira/utils/
--rw-r--r--   0 adonath    (502) staff       (20)      148 2021-11-08 14:30:24.000000 pylira-0.1/pylira/utils/__init__.py
--rw-r--r--   0 adonath    (502) staff       (20)     1114 2022-01-04 20:21:35.000000 pylira-0.1/pylira/utils/convolution.py
--rw-r--r--   0 adonath    (502) staff       (20)     3214 2022-03-14 01:55:12.000000 pylira-0.1/pylira/utils/io.py
--rw-r--r--   0 adonath    (502) staff       (20)    10345 2022-03-14 01:55:12.000000 pylira-0.1/pylira/utils/plot.py
--rw-r--r--   0 adonath    (502) staff       (20)     1379 2022-03-14 01:55:12.000000 pylira-0.1/pylira/utils/priors.py
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.202536 pylira-0.1/pylira/utils/tests/
--rw-r--r--   0 adonath    (502) staff       (20)        0 2021-11-08 14:30:24.000000 pylira-0.1/pylira/utils/tests/__init__.py
--rw-r--r--   0 adonath    (502) staff       (20)      725 2021-11-24 17:18:52.000000 pylira-0.1/pylira/utils/tests/test_io.py
--rw-r--r--   0 adonath    (502) staff       (20)     1356 2022-03-14 01:55:12.000000 pylira-0.1/pylira/utils/tests/test_plot.py
--rw-r--r--   0 adonath    (502) staff       (20)      486 2022-03-14 01:55:12.000000 pylira-0.1/pylira/utils/tests/test_priors.py
--rw-r--r--   0 adonath    (502) staff       (20)      335 2022-03-14 02:06:32.000000 pylira-0.1/pylira/version.py
-drwxr-xr-x   0 adonath    (502) staff       (20)        0 2022-03-14 02:06:33.198949 pylira-0.1/pylira.egg-info/
--rw-r--r--   0 adonath    (502) staff       (20)     2895 2022-03-14 02:06:33.000000 pylira-0.1/pylira.egg-info/PKG-INFO
--rw-r--r--   0 adonath    (502) staff       (20)     1605 2022-03-14 02:06:33.000000 pylira-0.1/pylira.egg-info/SOURCES.txt
--rw-r--r--   0 adonath    (502) staff       (20)        1 2022-03-14 02:06:33.000000 pylira-0.1/pylira.egg-info/dependency_links.txt
--rw-r--r--   0 adonath    (502) staff       (20)        1 2022-03-14 02:06:33.000000 pylira-0.1/pylira.egg-info/not-zip-safe
--rw-r--r--   0 adonath    (502) staff       (20)      176 2022-03-14 02:06:33.000000 pylira-0.1/pylira.egg-info/requires.txt
--rw-r--r--   0 adonath    (502) staff       (20)       13 2022-03-14 02:06:33.000000 pylira-0.1/pylira.egg-info/top_level.txt
--rw-r--r--   0 adonath    (502) staff       (20)      158 2021-11-08 14:31:13.000000 pylira-0.1/pyproject.toml
--rw-r--r--   0 adonath    (502) staff       (20)     1454 2022-03-14 02:06:33.203141 pylira-0.1/setup.cfg
--rwxr-xr-x   0 adonath    (502) staff       (20)     2857 2021-12-30 20:51:13.000000 pylira-0.1/setup.py
--rw-r--r--   0 adonath    (502) staff       (20)     2754 2021-11-10 02:26:47.000000 pylira-0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.120279 pylira-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-11 14:27:29.000000 pylira-0.2/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.104279 pylira-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.108279 pylira-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-11 14:27:29.000000 pylira-0.2/.github/workflows/ci_cron_weekly.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-11 14:27:29.000000 pylira-0.2/.github/workflows/ci_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-11 14:27:29.000000 pylira-0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-11 14:27:29.000000 pylira-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-11 14:27:29.000000 pylira-0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-11 14:27:29.000000 pylira-0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-11 14:27:29.000000 pylira-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-11 14:27:54.120279 pylira-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-11 14:27:29.000000 pylira-0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.108279 pylira-0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-11 14:27:29.000000 pylira-0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-04-11 14:27:29.000000 pylira-0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-11 14:27:29.000000 pylira-0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-11 14:27:29.000000 pylira-0.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.112279 pylira-0.2/docs/pylira/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.112279 pylira-0.2/docs/pylira/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-11 14:27:29.000000 pylira-0.2/docs/pylira/api/core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-11 14:27:29.000000 pylira-0.2/docs/pylira/api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-11 14:27:29.000000 pylira-0.2/docs/pylira/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-11 14:27:29.000000 pylira-0.2/docs/pylira/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-11 14:27:29.000000 pylira-0.2/docs/pylira/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-11 14:27:29.000000 pylira-0.2/docs/pylira/developer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-11 14:27:29.000000 pylira-0.2/docs/pylira/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-11 14:27:29.000000 pylira-0.2/docs/pylira/references.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.112279 pylira-0.2/docs/pylira/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-11 14:27:29.000000 pylira-0.2/docs/pylira/user/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-11 14:27:29.000000 pylira-0.2/docs/pylira/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.112279 pylira-0.2/docs/pylira/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-11 14:27:29.000000 pylira-0.2/docs/pylira/user/tutorials/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.112279 pylira-0.2/docs/pylira/user/tutorials/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-11 14:27:29.000000 pylira-0.2/docs/pylira/user/tutorials/notebooks/mcmc-deconvolution-intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-04-11 14:27:29.000000 pylira-0.2/docs/pylira/user/tutorials/notebooks/point_source.md
+-rw-r--r--   0 runner    (1001) docker     (123)   241873 2023-04-11 14:27:29.000000 pylira-0.2/docs/pylira-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-11 14:27:29.000000 pylira-0.2/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.112279 pylira-0.2/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)    37572 2023-04-11 14:27:29.000000 pylira-0.2/licenses/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-11 14:27:29.000000 pylira-0.2/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-11 14:27:29.000000 pylira-0.2/licenses/TEMPLATE_LICENCE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.112279 pylira-0.2/pylira/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-11 14:27:29.000000 pylira-0.2/pylira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-11 14:27:29.000000 pylira-0.2/pylira/_astropy_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-11 14:27:29.000000 pylira-0.2/pylira/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25438 2023-04-11 14:27:29.000000 pylira-0.2/pylira/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.116279 pylira-0.2/pylira/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-11 14:27:29.000000 pylira-0.2/pylira/data/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 14:27:29.000000 pylira-0.2/pylira/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 14:27:29.000000 pylira-0.2/pylira/data/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.116279 pylira-0.2/pylira/data/files/
+-rw-r--r--   0 runner    (1001) docker     (123)    24867 2023-04-11 14:27:29.000000 pylira-0.2/pylira/data/files/chandra-counts-obs-id-4683.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    24717 2023-04-11 14:27:29.000000 pylira-0.2/pylira/data/files/chandra-counts-obs-id-4684.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-04-11 14:27:29.000000 pylira-0.2/pylira/data/files/chandra-psf-obs-id-4683.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-04-11 14:27:29.000000 pylira-0.2/pylira/data/files/chandra-psf-obs-id-4684.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-11 14:27:29.000000 pylira-0.2/pylira/data/files/lincoln.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10646 2023-04-11 14:27:29.000000 pylira-0.2/pylira/data/files/output-par.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   102742 2023-04-11 14:27:29.000000 pylira-0.2/pylira/data/files/output.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.116279 pylira-0.2/pylira/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:29.000000 pylira-0.2/pylira/data/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-11 14:27:29.000000 pylira-0.2/pylira/data/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.116279 pylira-0.2/pylira/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-11 14:27:29.000000 pylira-0.2/pylira/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.116279 pylira-0.2/pylira/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    74580 2023-04-11 14:27:29.000000 pylira-0.2/pylira/src/lira.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-11 14:27:29.000000 pylira-0.2/pylira/src/lirabind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.116279 pylira-0.2/pylira/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 14:27:29.000000 pylira-0.2/pylira/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-11 14:27:29.000000 pylira-0.2/pylira/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.116279 pylira-0.2/pylira/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-11 14:27:29.000000 pylira-0.2/pylira/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-11 14:27:29.000000 pylira-0.2/pylira/utils/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-11 14:27:29.000000 pylira-0.2/pylira/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-04-11 14:27:29.000000 pylira-0.2/pylira/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-11 14:27:29.000000 pylira-0.2/pylira/utils/priors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.120279 pylira-0.2/pylira/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:29.000000 pylira-0.2/pylira/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-11 14:27:29.000000 pylira-0.2/pylira/utils/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-11 14:27:29.000000 pylira-0.2/pylira/utils/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-11 14:27:29.000000 pylira-0.2/pylira/utils/tests/test_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-11 14:27:54.000000 pylira-0.2/pylira/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:27:54.116279 pylira-0.2/pylira.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-11 14:27:54.000000 pylira-0.2/pylira.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-11 14:27:54.000000 pylira-0.2/pylira.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:27:54.000000 pylira-0.2/pylira.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:27:54.000000 pylira-0.2/pylira.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-11 14:27:54.000000 pylira-0.2/pylira.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 14:27:54.000000 pylira-0.2/pylira.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-11 14:27:29.000000 pylira-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-11 14:27:54.120279 pylira-0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2805 2023-04-11 14:27:29.000000 pylira-0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-11 14:27:29.000000 pylira-0.2/tox.ini
```

### Comparing `pylira-0.1/.clang-format` & `pylira-0.2/.clang-format`

 * *Files identical despite different names*

### Comparing `pylira-0.1/.github/workflows/ci_cron_weekly.yml` & `pylira-0.2/.github/workflows/ci_cron_weekly.yml`

 * *Files identical despite different names*

### Comparing `pylira-0.1/.github/workflows/ci_tests.yml` & `pylira-0.2/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `pylira-0.1/.gitignore` & `pylira-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pylira-0.1/PKG-INFO` & `pylira-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pylira
-Version: 0.1
+Version: 0.2
 Summary: A Python package for Bayesian low-counts image reconstruction and analysis
 Home-page: https://pylira.readthedocs.io/
 Author: pylira developers
 Author-email: 
 License: GNU GPL v3+
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
@@ -64,9 +63,7 @@
 the errors and assumptions that seasoned contributors have glossed over.
 
 Note: This disclaimer was originally written by
 `Adrienne Lowe <https://github.com/adriennefriend>`_ for a
 `PyCon talk <https://www.youtube.com/watch?v=6Uj746j9Heo>`_, and was adapted by
 pylira based on its use in the README file for the
 `MetPy project <https://github.com/Unidata/MetPy>`_.
-
-
```

### Comparing `pylira-0.1/README.rst` & `pylira-0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pylira-0.1/docs/Makefile` & `pylira-0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pylira-0.1/docs/conf.py` & `pylira-0.2/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,70 +21,72 @@
 # done. If the sys.path entry above is added, when the astropy.sphinx.conf
 # import occurs, it will import the *source* version of astropy instead of the
 # version installed (if invoked as "make html" or directly with sphinx), or the
 # version in the build directory (if "python setup.py build_sphinx" is used).
 # Thus, any C-extensions that are needed to build the documentation will *not*
 # be accessible, and the documentation will not build correctly.
 
+import datetime
 import os
 import sys
-import datetime
 from importlib import import_module
 
 try:
     from sphinx_astropy.conf.v1 import *  # noqa
 except ImportError:
-    print('ERROR: the documentation requires the sphinx-astropy package to be installed')
+    print(
+        "ERROR: the documentation requires the sphinx-astropy package to be installed"
+    )
     sys.exit(1)
 
 # Get configuration information from setup.cfg
 from configparser import ConfigParser
+
 conf = ConfigParser()
 
-conf.read([os.path.join(os.path.dirname(__file__), '..', 'setup.cfg')])
-setup_cfg = dict(conf.items('metadata'))
+conf.read([os.path.join(os.path.dirname(__file__), "..", "setup.cfg")])
+setup_cfg = dict(conf.items("metadata"))
 
 # -- General configuration ----------------------------------------------------
 
 # By default, highlight as Python 3.
-highlight_language = 'python3'
+highlight_language = "python3"
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.2'
+# needs_sphinx = '1.2'
 
 # To perform a Sphinx version check that needs to be more specific than
 # major.minor, call `check_sphinx_version("X.Y.Z")` here.
 # check_sphinx_version("1.2.1")
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns.append('_templates')
+exclude_patterns.append("_templates")
 
 # This is added to the end of RST files - a good place to put substitutions to
 # be used globally.
 rst_epilog += """
 """
 
 # -- Project information ------------------------------------------------------
 
 # This does not *have* to match the package name, but typically does
-project = setup_cfg['name']
-author = setup_cfg['author']
-copyright = '{0}, {1}'.format(
-    datetime.datetime.now().year, setup_cfg['author'])
+project = setup_cfg["name"]
+author = setup_cfg["author"]
+copyright = "{0}, {1}".format(datetime.datetime.now().year, setup_cfg["author"])
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 
-import_module(setup_cfg['name'])
-package = sys.modules[setup_cfg['name']]
+import_module(setup_cfg["name"])
+package = sys.modules[setup_cfg["name"]]
 
 # The short X.Y version.
-version = package.__version__.split('-', 1)[0]
+version = package.__version__.split("-", 1)[0]
 # The full version, including alpha/beta/rc tags.
 release = package.__version__
 
 
 # -- Options for HTML output --------------------------------------------------
 
 # A NOTE ON HTML THEMES
@@ -93,38 +95,38 @@
 # the options for this theme can be modified by overriding some of the
 # variables set in the global configuration. The variables set in the
 # global configuration are listed below, commented out.
 
 
 # Add any paths that contain custom themes here, relative to this directory.
 # To use a different custom theme, add the directory containing the theme.
-#html_theme_path = []
+# html_theme_path = []
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes. To override the custom theme, set this to the
 # name of a builtin theme or the name of a custom theme in html_theme_path.
-#html_theme = None
+# html_theme = None
 
 html_theme = "pydata_sphinx_theme"
 
 # Custom sidebar templates, maps document names to template names.
 html_sidebars = {}
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
 html_logo = "pylira-logo.png"
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-html_favicon = ''
+html_favicon = ""
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = ''
+# html_last_updated_fmt = ''
 
 html_context = {
     # "github_url": "https://github.com", # or your GitHub Enterprise interprise
     "github_user": "astrostat",
     "github_repo": "pylira",
     "github_version": "main",
     "doc_path": "docs",
@@ -139,43 +141,47 @@
         },
     ],
     "use_edit_page_button": True,
 }
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-html_title = '{0} v{1}'.format(project, release)
+html_title = "{0} v{1}".format(project, release)
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = project + 'doc'
+htmlhelp_basename = project + "doc"
 
 # Prefixes that are ignored for sorting the Python module index
 modindex_common_prefix = ["pylira."]
 
 
 # -- Options for LaTeX output -------------------------------------------------
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
-latex_documents = [('index', project + '.tex', project + u' Documentation',
-                    author, 'manual')]
+latex_documents = [
+    ("index", project + ".tex", project + " Documentation", author, "manual")
+]
 
 
 # -- Options for manual page output -------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [('index', project.lower(), project + u' Documentation',
-              [author], 1)]
+man_pages = [("index", project.lower(), project + " Documentation", [author], 1)]
 
-extensions += ["matplotlib.sphinxext.plot_directive", "nbsphinx", "sphinx_gallery.load_style"]
+extensions += [
+    "matplotlib.sphinxext.plot_directive",
+    "nbsphinx",
+    "sphinx_gallery.load_style",
+]
 
 
 nbsphinx_custom_formats = {
-    '.md': ['jupytext.reads', {'fmt': 'md'}],
+    ".md": ["jupytext.reads", {"fmt": "md"}],
 }
 
 nbsphinx_execute_arguments = [
     "--InlineBackend.figure_formats={'png'}",
     "--InlineBackend.rc=figure.dpi=96",
 ]
 
@@ -185,32 +191,32 @@
 .. raw:: html
 
     Notebook file for download: <a href="{{ docname|e }}">{{ docname|e }}</a>
 """
 
 # -- Options for the edit_on_github extension ---------------------------------
 
-if setup_cfg.get('edit_on_github').lower() == 'true':
+if setup_cfg.get("edit_on_github").lower() == "true":
 
-    extensions += ['sphinx_astropy.ext.edit_on_github']
+    extensions += ["sphinx_astropy.ext.edit_on_github"]
 
-    edit_on_github_project = setup_cfg['github_project']
+    edit_on_github_project = setup_cfg["github_project"]
     edit_on_github_branch = "main"
 
     edit_on_github_source_root = ""
     edit_on_github_doc_root = "docs"
 
 # -- Resolving issue number to links in changelog -----------------------------
-github_issues_url = 'https://github.com/{0}/issues/'.format(setup_cfg['github_project'])
+github_issues_url = "https://github.com/{0}/issues/".format(setup_cfg["github_project"])
 
 
 # -- Options for linkcheck output -------------------------------------------
 linkcheck_retry = 5
 linkcheck_ignore = [
-    r'https://github\.com/astrostat/pylira/(?:issues|pull)/\d+',
+    r"https://github\.com/astrostat/pylira/(?:issues|pull)/\d+",
 ]
 linkcheck_timeout = 180
 linkcheck_anchors = False
 
 # -- Turn on nitpicky mode for sphinx (to warn about references not found) ----
 #
 # nitpicky = True
```

### Comparing `pylira-0.1/docs/make.bat` & `pylira-0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pylira-0.1/docs/pylira/api/utils.rst` & `pylira-0.2/docs/pylira/api/utils.rst`

 * *Files identical despite different names*

### Comparing `pylira-0.1/docs/pylira/developer.rst` & `pylira-0.2/docs/pylira/developer.rst`

 * *Files identical despite different names*

### Comparing `pylira-0.1/docs/pylira/index.rst` & `pylira-0.2/docs/pylira/index.rst`

 * *Files identical despite different names*

### Comparing `pylira-0.1/docs/pylira/references.rst` & `pylira-0.2/docs/pylira/references.rst`

 * *Files identical despite different names*

### Comparing `pylira-0.1/docs/pylira/user/data.rst` & `pylira-0.2/docs/pylira/user/data.rst`

 * *Files 23% similar despite different names*

```diff
@@ -37,7 +37,20 @@
     :include-source:
 
     from pylira.data import gauss_and_point_sources_gauss_psf
     from pylira.utils.plot import plot_example_dataset
 
     data = gauss_and_point_sources_gauss_psf()
     plot_example_dataset(data)
+
+
+Chandra Galactic Center Example
+-------------------------------
+
+.. plot::
+    :include-source:
+
+    from pylira.data import chandra_gc
+    from pylira.utils.plot import plot_example_dataset
+
+    data = chandra_gc(obs_id=4683)
+    plot_example_dataset(data)
```

### Comparing `pylira-0.1/docs/pylira/user/index.rst` & `pylira-0.2/docs/pylira/user/index.rst`

 * *Files identical despite different names*

### Comparing `pylira-0.1/docs/pylira/user/tutorials/notebooks/mcmc-deconvolution-intro.md` & `pylira-0.2/docs/pylira/user/tutorials/notebooks/mcmc-deconvolution-intro.md`

 * *Files identical despite different names*

### Comparing `pylira-0.1/docs/pylira-logo.png` & `pylira-0.2/docs/pylira-logo.png`

 * *Files identical despite different names*

### Comparing `pylira-0.1/licenses/LICENSE.rst` & `pylira-0.2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pylira-0.1/licenses/TEMPLATE_LICENCE.rst` & `pylira-0.2/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `pylira-0.1/pylira/conftest.py` & `pylira-0.2/pylira/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 test infrastructure. It needs to live inside the package in order for it to
 get picked up when running the tests inside an interpreter using
 `pylira.test()`.
 
 """
 
 import os
-
 from astropy.version import version as astropy_version
 
 # For Astropy 3.0 and later, we can use the standalone pytest plugin
 if astropy_version < "3.0":
     from astropy.tests.pytest_plugins import *  # noqa
 
     del pytest_report_header
```

### Comparing `pylira-0.1/pylira/core.py` & `pylira-0.2/pylira/core.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+import os
+import tempfile
+from copy import deepcopy
 from pathlib import Path
 import numpy as np
+from scipy.ndimage import labeled_comprehension
 from astropy.table import Table
 from . import image_analysis
 from .utils.io import (
-    read_parameter_trace_file,
-    read_image_trace_file,
-    IO_FORMATS_WRITE,
     IO_FORMATS_READ,
+    IO_FORMATS_WRITE,
+    read_image_trace_file,
+    read_parameter_trace_file,
 )
 from .utils.plot import (
-    plot_parameter_traces,
     plot_parameter_distributions,
+    plot_parameter_traces,
     plot_pixel_trace,
     plot_pixel_trace_neighbours,
 )
 
-
 DTYPE_DEFAULT = np.float64
 
 __all__ = ["LIRADeconvolver", "LIRADeconvolverResult"]
 
 
 class LIRADeconvolver:
     """LIRA image deconvolution method
@@ -42,18 +45,14 @@
         Multiscale prior TODO: improve description
     ms_al_kap1: float
         Multiscale prior TODO: improve description
     ms_al_kap2: float
         Multiscale prior TODO: improve description
     ms_al_kap3: float
         Multiscale prior TODO: improve description
-    filename_out: str or `Path`
-        Output filename
-    filename_out_par: str or `Path`
-        Parameter output filename
     random_state : `~numpy.random.RandomState`
         Random state
 
     Examples
     --------
     This how to use the class:
 
@@ -79,33 +78,31 @@
         fit_background_scale=False,
         save_thin=True,
         ms_ttlcnt_pr=1,
         ms_ttlcnt_exp=0.05,
         ms_al_kap1=0.0,
         ms_al_kap2=1000.0,
         ms_al_kap3=3.0,
-        filename_out="output.txt",
-        filename_out_par="output-par.txt",
+        filename_out=None,
+        filename_out_par=None,
         random_state=None,
     ):
         self.alpha_init = np.array(alpha_init, dtype=DTYPE_DEFAULT)
         self.n_iter_max = n_iter_max
         self.n_burn_in = n_burn_in
         self.fit_background_scale = fit_background_scale
         self.save_thin = save_thin
         self.ms_ttlcnt_pr = ms_ttlcnt_pr
         self.ms_ttlcnt_exp = ms_ttlcnt_exp
         self.ms_al_kap1 = ms_al_kap1
         self.ms_al_kap2 = ms_al_kap2
         self.ms_al_kap3 = ms_al_kap3
-        self.filename_out = Path(filename_out)
-        self.filename_out_par = Path(filename_out_par)
 
         if random_state is None:
-            random_state = np.random.RandomState(None)
+            random_state = np.random.RandomState()
 
         self.random_state = random_state
 
     def __str__(self):
         """String representation"""
         cls_name = self.__class__.__name__
         info = cls_name + "\n"
@@ -113,16 +110,16 @@
         data = self.to_dict()
 
         for key, value in data.items():
             info += f"\t{key:21s}: {value}\n"
 
         return info.expandtabs(tabsize=4)
 
-    def _check_input_sizes(self, obs_arr):
-        obs_shape = obs_arr.shape[0]
+    def _check_input_sizes(self, shape):
+        obs_shape = shape[0]
         if obs_shape & (obs_shape - 1) != 0:
             raise ValueError(
                 f"Size of the input observation must be a power of 2. Size given: {obs_shape}"
             )
 
         if len(self.alpha_init) != np.log2(obs_shape):
             raise ValueError(
@@ -137,16 +134,14 @@
         -------
         data : dict
             Parameter dict.
         """
         data = {}
         data.update(self.__dict__)
         data["alpha_init"] = self.alpha_init.tolist()
-        data.pop("filename_out")
-        data.pop("filename_out_par")
         # TOOD: serialise random state for reproducibility?
         data.pop("random_state")
         return data
 
     def run(self, data):
         """Run the algorithm
 
@@ -156,47 +151,72 @@
             Data
 
         Returns
         -------
         result : `LIRADeconvolverResult`
             Result object.
         """
-        data = {name: arr.astype(DTYPE_DEFAULT) for name, arr in data.items()}
-        self._check_input_sizes(data["counts"])
+        data = {
+            name: arr.astype(DTYPE_DEFAULT)
+            for name, arr in data.items()
+            if name != "wcs"
+        }
+        shape_counts = data["counts"].shape
+        self._check_input_sizes(shape_counts)
+
+        for name in ["background", "exposure", "flux_init"]:
+            shape = data[name].shape
+            if shape != shape_counts:
+                raise ValueError(
+                    f"Quantity '{name}' has a shape of {shape}, however {shape_counts} is expected."
+                )
 
         random_seed = self.random_state.randint(1, np.iinfo(np.uint32).max)
 
-        posterior_mean = image_analysis(
-            observed_im=data["counts"],
-            start_im=data["flux_init"],
-            psf_im=data["psf"],
-            expmap_im=data["exposure"],
-            baseline_im=data["background"],
-            max_iter=self.n_iter_max,
-            burn_in=self.n_burn_in,
-            save_thin=self.save_thin,
-            fit_bkgscl=int(self.fit_background_scale),
-            out_img_file=str(self.filename_out),
-            out_param_file=str(self.filename_out_par),
-            alpha_init=self.alpha_init,
-            ms_ttlcnt_pr=self.ms_ttlcnt_pr,
-            ms_ttlcnt_exp=self.ms_ttlcnt_exp,
-            ms_al_kap1=self.ms_al_kap1,
-            ms_al_kap2=self.ms_al_kap2,
-            ms_al_kap3=self.ms_al_kap3,
-            random_seed=random_seed,
-        )
+        with tempfile.TemporaryDirectory() as tmpdir:
+            filename_image_trace = str(os.path.join(tmpdir, "image-trace.tx"))
+            filename_parameter_trace = str(os.path.join(tmpdir, "parameter-trace.txt"))
+
+            posterior_mean = image_analysis(
+                observed_im=data["counts"],
+                start_im=data["flux_init"],
+                psf_im=data["psf"],
+                expmap_im=data["exposure"],
+                baseline_im=data["background"],
+                out_img_file=filename_image_trace,
+                out_param_file=filename_parameter_trace,
+                max_iter=self.n_iter_max,
+                burn_in=self.n_burn_in,
+                save_thin=self.save_thin,
+                fit_bkgscl=int(self.fit_background_scale),
+                alpha_init=self.alpha_init,
+                ms_ttlcnt_pr=self.ms_ttlcnt_pr,
+                ms_ttlcnt_exp=self.ms_ttlcnt_exp,
+                ms_al_kap1=self.ms_al_kap1,
+                ms_al_kap2=self.ms_al_kap2,
+                ms_al_kap3=self.ms_al_kap3,
+                random_seed=random_seed,
+            )
+
+            parameter_trace = read_parameter_trace_file(
+                filename=filename_parameter_trace, format="ascii"
+            )
 
-        parameter_trace = {"filename": str(self.filename_out_par), "format": "ascii"}
-        image_trace = {"filename": str(self.filename_out), "format": "ascii"}
+            image_trace = read_image_trace_file(
+                filename=filename_image_trace, format="ascii"
+            )
 
         config = self.to_dict()
         config["random_seed"] = random_seed
+
+        posterior_std = np.nanstd(image_trace[self.n_burn_in :], axis=0)
+
         return LIRADeconvolverResult(
             posterior_mean=posterior_mean,
+            posterior_std=posterior_std,
             parameter_trace=parameter_trace,
             image_trace=image_trace,
             config=config,
         )
 
 
 class LIRADeconvolverResult:
@@ -204,34 +224,38 @@
 
     Parameters
     ----------
     config : `dict`
         Configuration from the `LIRADeconvolver`
     posterior_mean : `~numpy.ndarray`
         Posterior mean
+    posterior_std : `~numpy.ndarray`
+        Posterior standard deviation
     parameter_trace : `~astropy.table.Table` or dict
         Parameter trace. If a dict is provided it triggers the lazy loading.
         The dict must contain the argument to `read_parameter_trace_file`.
     image_trace : `~astropy.table.Table` or dict
         Image trace. If a dict is provided it triggers the lazy loading.
         The dict must contain the argument to `read_image_trace_file`.
     wcs : `~astropy.wcs.WCS`
         World coordinate transform object
     """
 
     def __init__(
         self,
         config,
         posterior_mean=None,
+        posterior_std=None,
         parameter_trace=None,
         image_trace=None,
         wcs=None,
     ):
         self._config = config
         self._posterior_mean = posterior_mean
+        self._posterior_std = posterior_std
         self._wcs = wcs
         self._image_trace = image_trace
         self._parameter_trace = parameter_trace
 
     @property
     def config(self):
         """Configuration data (`dict`)"""
@@ -256,24 +280,45 @@
 
     @property
     def n_burn_in(self):
         """Number of burn in iterations"""
         return self.config.get("n_burn_in", 0)
 
     @property
+    def n_iter_max(self):
+        """Number of max. iterations"""
+        return self.config["n_iter_max"]
+
+    @property
     def posterior_mean(self):
         """Posterior mean (`~numpy.ndarray`)"""
         return self._posterior_mean
 
     @property
+    def posterior_std(self):
+        """Posterior standard deviation (`~numpy.ndarray`)"""
+        return self._posterior_std
+
+    @property
     def posterior_mean_from_trace(self):
         """Posterior mean computed from trace(`~numpy.ndarray`)"""
+        if self.image_trace is None:
+            raise ValueError("No image trace available.")
+
         return np.nanmean(self.image_trace[self.n_burn_in :], axis=0)
 
     @property
+    def posterior_std_from_trace(self):
+        """Posterior std computed from trace(`~numpy.ndarray`)"""
+        if self.image_trace is None:
+            raise ValueError("No image trace available.")
+
+        return np.nanstd(self.image_trace[self.n_burn_in :], axis=0)
+
+    @property
     def image_trace(self):
         """Image trace (`~numpy.ndarray`)"""
         # TODO: this currently handles only in memory data, this might not scale for
         # many iterations and/or large images
         if isinstance(self._image_trace, dict):
             self._image_trace = read_image_trace_file(**self._image_trace)
 
@@ -285,15 +330,17 @@
         if isinstance(self._parameter_trace, dict):
             self._parameter_trace = read_parameter_trace_file(**self._parameter_trace)
             # TODO: add config to meta data of table, not sure whether it's the right place.
             self._parameter_trace.meta.update(self.config)
 
         return self._parameter_trace
 
-    def plot_pixel_traces_region(self, center_pix, radius_pix=0, figsize=(16, 6)):
+    def plot_pixel_traces_region(
+        self, center_pix, radius_pix=0, figsize=(16, 6), **kwargs
+    ):
         """Plot pixel traces in a given region.
 
         Parameters
         ----------
         center_pix : tuple of int
              Pixel indices, order is (x, y). By default the trace at the center is plotted.
         radius_pix : float
@@ -305,47 +352,54 @@
         from matplotlib.patches import Circle
 
         fig = plt.figure(figsize=figsize)
 
         data = self.posterior_mean_from_trace
 
         ax_image = plt.subplot(1, 2, 1, projection=self.wcs)
-        im = ax_image.imshow(data, origin="lower")
+        im = ax_image.imshow(data, origin="lower", **kwargs)
         fig.colorbar(im, ax=ax_image, label="Posterior Mean")
 
         radius = max(radius_pix, 1)
         artist = Circle(center_pix, radius=radius, color="w", fc="None")
         ax_image.add_artist(artist)
 
-        ax_trace = plt.subplot(1, 2, 2, projection=self.wcs)
+        ax_trace = plt.subplot(1, 2, 2)
 
         plot_pixel_trace(
             image_trace=self.image_trace,
             center_pix=center_pix,
             ax=ax_trace,
             config=self.config,
         )
 
         plot_pixel_trace_neighbours(
             image_trace=self.image_trace,
             center_pix=center_pix,
             radius_pix=radius_pix,
             ax=ax_trace,
         )
+        return {
+            "ax-image": ax_image,
+            "ax-trace": ax_trace,
+        }
 
     def plot_pixel_trace(self, center_pix=None, **kwargs):
         """Plot pixel trace at a given position.
 
         Parameters
         ----------
         center_pix : tuple of int
              Pixel indices, order is (x, y). By default the trace at the center is plotted.
         **kwargs : dict
             Keyword arguments forwarded to `plot_pixel_trace`
         """
+        if self.image_trace is None:
+            raise ValueError("No image trace available.")
+
         if center_pix is None:
             # choose center as default
             center_pix = tuple(np.array(self.posterior_mean.shape) // 2)
 
         plot_pixel_trace(
             image_trace=self.image_trace,
             config=self.config,
@@ -361,14 +415,17 @@
         center_pix : tuple of int
             Pixel indices, order is (x, y). By default the trace at the center is plotted.
         radius_pix : float
             Radius in which the traces are plotted.
         **kwargs : dict
             Keyword arguments forwarded to `~matplotlib.pyplot.plot`
         """
+        if self.image_trace is None:
+            raise ValueError("No image trace available.")
+
         if center_pix is None:
             # choose center as default
             center_pix = tuple(np.array(self.posterior_mean.shape) // 2)
 
         plot_pixel_trace_neighbours(
             image_trace=self.image_trace,
             center_pix=center_pix,
@@ -403,14 +460,17 @@
         """Plot image trace interactively
 
         Parameters
         ----------
         **kwargs : dict
             Keyword arguments forwarded to `~matplotlib.pyplot.imshow`
         """
+        if self.image_trace is None:
+            raise ValueError("No image trace available.")
+
         import matplotlib.pyplot as plt
         from ipywidgets import IntSlider
         from ipywidgets.widgets.interaction import interact
 
         kwargs.setdefault("interpolation", "nearest")
         kwargs.setdefault("origin", "lower")
 
@@ -426,14 +486,88 @@
 
         @interact(idx=slider)
         def _plot_interactive(idx):
             ax = plt.subplot(projection=self.wcs)
             im = ax.imshow(self.image_trace[idx], **kwargs)
             plt.colorbar(im, ax=ax, label="Flux")
 
+    def plot_image_trace_animation(
+        self,
+        ax=None,
+        interval=20,
+        repeat=True,
+        n_frames=None,
+        cumulative=False,
+        label_dxy=(20, 10),
+        **kwargs,
+    ):
+        """Plot image trace animation
+
+        Parameters
+        ----------
+        ax : `~matplotlib.pyplot.Axes`
+            Plot axes
+        interval : int
+            Interval im ms.
+        repeat : bool
+            Repeat animation
+        n_frames : int
+            Number of frames
+        cumulative : bool
+            Cumulated mean of the samples.
+        label_dxy : tuple of int
+            Shift of the frame label.
+
+
+        Returns
+        -------
+        anim : `~matplotlib.animation.FuncAnimation`
+            Func animation object.
+        """
+        if self.image_trace is None:
+            raise ValueError("No image trace available.")
+
+        import matplotlib.pyplot as plt
+        from matplotlib.animation import FuncAnimation
+
+        if ax is None:
+            ax = plt.subplot(projection=self.wcs)
+
+        if n_frames is None:
+            n_frames = self.n_iter_max
+
+        kwargs.setdefault("origin", "lower")
+
+        data = np.zeros(self.posterior_mean.shape)
+        image = ax.imshow(data, **kwargs)
+
+        y, x = self.posterior_mean.shape
+        dx, dy = label_dxy
+        text = ax.text(x - dx, y - dy, s="", color="w", va="center", ha="center")
+
+        def animate(idx, im, txt, result):
+            if cumulative:
+                data = np.mean(result.image_trace[:idx], axis=0)
+            else:
+                data = result.image_trace[idx]
+            im.set_data(data)
+            txt.set_text(f"$N_{{Iter}} = {idx}$")
+            return (image,)
+
+        anim = FuncAnimation(
+            fig=ax.figure,
+            func=animate,
+            fargs=[image, text, self],
+            frames=n_frames,
+            interval=interval,
+            blit=True,
+            repeat=repeat,
+        )
+        return anim
+
     def plot_parameter_traces(self, **kwargs):
         """Plot parameter traces
 
         Parameters
         ----------
         **kwargs : dict
             Keyword arguments forwarded to `plot_parameter_traces`
@@ -494,7 +628,202 @@
             raise ValueError(
                 f"Not a valid format '{format}', choose from {list(IO_FORMATS_READ)}"
             )
 
         reader = IO_FORMATS_READ[format]
         kwargs = reader(filename=filename)
         return cls(**kwargs)
+
+    def reduce_to_mean_std(self):
+        """Reduce to mean and std
+
+        Returns
+        -------
+        result : `~LIRADeconvolverResult`
+            Reduced result object
+        """
+        return self.__class__(
+            config=deepcopy(self.config),
+            posterior_mean=self.posterior_mean_from_trace,
+            posterior_std=self.posterior_std_from_trace,
+            wcs=deepcopy(self.wcs),
+            parameter_trace=deepcopy(self.parameter_trace),
+        )
+
+
+class LIRASignificanceEstimator:
+    """
+    Estimate the significance of emission from specified regions
+    using the method described in Stein et al. (2015)
+
+    Parameters
+    ----------
+    result_observed_im: `~LIRADeconvolverResult`
+        LIRA result for the observed image
+    result_replicates: list
+        LIRA result array for the baseline images
+    labels_im: `~numpy.ndarray`
+        Image with regions where each region is indicated with a unique integer
+    """
+
+    def __init__(
+        self,
+        result_observed_im,
+        result_replicates,
+        labels_im,
+    ):
+        self._result_observed_im = result_observed_im
+        self._result_replicates = result_replicates
+        self._labels_im = labels_im
+
+        self._labels = np.array([str(i) for i in np.unique(labels_im.flatten())])
+
+    def _estimate_xi(self, result, data):
+        xi_regions = []
+        burnin = result.config["n_burn_in"]
+        n_iter = result.config["n_iter_max"]
+        thin = result.config["save_thin"]
+        fit_bkgscl = result.config["fit_background_scale"]
+        bkg_scale_trace = (
+            result.parameter_trace["bkgScale"]
+            if "bkgScale" in result.parameter_trace.keys()
+            else np.ones(result.parameter_trace["iteration"].shape[0])
+        )
+        image_trace = result.image_trace
+
+        baseline_im = data["background"]
+
+        baseline_sum = labeled_comprehension(
+            baseline_im, self._labels_im, self._labels, np.sum, float, 0
+        )
+
+        # loop over each image from the trace and estimate xi
+        iter = 0
+        for i in range(burnin, n_iter, thin):
+            tau_1 = labeled_comprehension(
+                image_trace[iter, :, :], self._labels_im, self._labels, np.sum, float, 0
+            )
+
+            tau_0 = baseline_sum
+            if fit_bkgscl == 1:
+                tau_0 = baseline_sum * bkg_scale_trace[iter]
+
+            xi_regions.append(tau_1 / (tau_1 + tau_0))
+
+            iter = iter + 1
+
+        # each row is a distribution of xi for one region
+        xi_regions = np.array(xi_regions).T
+
+        return {self._labels[i]: xi_regions[i] for i in range(self._labels.shape[0])}
+
+    def _estimate_test_statistic(self, tail, observed_dist):
+        return (observed_dist >= tail).sum() / observed_dist.shape[0]
+
+    def _estimate_pval_ul(self, gamma, test_stat):
+        """
+        Stein et al. (2015) eq. 22
+        """
+        return gamma / test_stat
+
+    def estimate_p_values(self, data, gamma=0.005):
+        xi_dist_observed_im = self._estimate_xi(self._result_observed_im, data)
+        xi_dist_replicates = [
+            self._estimate_xi(result_replicate, data)
+            for result_replicate in self._result_replicates
+        ]
+
+        xi_dist_merged_replicates = {
+            self._labels[i]: [] for i in range(self._labels.shape[0])
+        }
+
+        for xi_replicate in xi_dist_replicates:
+            for k, v in xi_replicate.items():
+                xi_dist_merged_replicates[k] = np.concatenate(
+                    (xi_dist_merged_replicates[k], v)
+                )
+
+        xi_dist_merged_replicates = {
+            k: v.flatten() for k, v in xi_dist_merged_replicates.items()
+        }
+
+        # find the 1-gamma percentile
+        tail_1_gamma = {
+            k: np.percentile(v, (1 - gamma) * 100)
+            for k, v in xi_dist_merged_replicates.items()
+        }
+
+        # find the number of values in the xi_dist_observed beyond these percentiles
+        test_statistic = {
+            k: self._estimate_test_statistic(v, xi_dist_observed_im[k])
+            for k, v in tail_1_gamma.items()
+        }
+
+        # estimate upper limit on p-values
+        p_value_ul = {
+            k: self._estimate_pval_ul(gamma, v) for k, v in test_statistic.items()
+        }
+
+        return (
+            p_value_ul,
+            xi_dist_merged_replicates,
+            xi_dist_observed_im,
+            tail_1_gamma,
+            test_statistic,
+        )
+
+    def _plot_xi(self, xi_dist, ax, ls="--", c="gray", tol=1e-10, label=None):
+        from scipy import stats
+
+        xi_dist_c = deepcopy(xi_dist)
+        xi_dist_c[xi_dist_c <= tol] = tol
+
+        xi_dist_c = np.log10(xi_dist_c)
+
+        kernel = stats.gaussian_kde(xi_dist_c)
+        eval_points = np.linspace(np.min(xi_dist_c), 0, 100)
+        kde = kernel(eval_points)
+
+        ax.plot(eval_points, kde, ls=ls, c=c, label=label)
+
+    def plot_xi_dist(self, xi_obs, xi_repl, region_id, figsize=(8, 5)):
+        """
+        Plot the posterior distributions of xi for a region
+
+        Parameters
+        ----------
+        xi_obs : `~numpy.ndarray`
+            Posterior distribution of xi for the observation
+        xi_repl : `~numpy.ndarray`
+            Posterior distribution of xi for all the replicates
+        region_id : int
+            Integer representing the region
+        figsize : tuple
+            Figure size
+        """
+        import matplotlib.pyplot as plt
+
+        fig, ax = plt.subplots(1, 1, figsize=figsize)
+
+        n_replicates = int(xi_repl[region_id].shape[0] / xi_obs[region_id].shape[0])
+        n_iters = xi_obs[region_id].shape[0]
+
+        # plot the replicate distribution
+        for i in range(0, n_replicates * n_iters, n_iters):
+            self._plot_xi(xi_repl[region_id][i : i + n_iters], ax)
+
+        # plot the mean distribution
+        self._plot_xi(
+            xi_repl[region_id], ax, ls="-", c="black", label="Mean null distribution"
+        )
+
+        # plot the observed distribution
+        self._plot_xi(
+            xi_obs[region_id], ax, ls="-", c="blue", label="Best fit distribution"
+        )
+
+        ax.set_xlabel(r"Posterior distribution (log$_{10}\xi$)")
+        ax.set_ylabel("Density")
+
+        ax.set_title(f"Region: {region_id}")
+        plt.legend()
+        return ax
```

### Comparing `pylira-0.1/pylira/data/core.py` & `pylira-0.2/pylira/data/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import numpy as np
 from astropy.convolution import Gaussian2DKernel, Tophat2DKernel, convolve_fft
+from astropy.io import fits
 from astropy.utils.data import get_pkg_data_filename
-
+from astropy.wcs import WCS
 
 __all__ = [
     "point_source_gauss_psf",
     "disk_source_gauss_psf",
     "gauss_and_point_sources_gauss_psf",
     "lincoln",
+    "chandra_gc",
 ]
 
 
 def point_source_gauss_psf(
     shape=(32, 32),
     shape_psf=(17, 17),
     sigma_psf=3,
@@ -227,7 +229,55 @@
     return {
         "counts": counts,
         "psf": psf.array,
         "exposure": exposure,
         "background": background,
         "flux": flux,
     }
+
+
+def chandra_gc(obs_id=4683, cutout=True):
+    """Get Chandra Galactic Center example dataset.
+
+    The exposure is assumed unity and background is zero.
+
+    Parameters
+    ----------
+    obs_id : {4683, 4684}
+        Which observation id
+    cutout : bool
+        Use a smaller data cutout
+
+    Returns
+    -------
+    data : dict of `~numpy.ndarray`
+        Data dictionary
+    """
+    filename = get_pkg_data_filename(
+        f"files/chandra-counts-obs-id-{obs_id}.fits.gz", package="pylira.data"
+    )
+    counts = fits.getdata(filename)
+    wcs = WCS(fits.getheader(filename))
+
+    filename = get_pkg_data_filename(
+        f"files/chandra-psf-obs-id-{obs_id}.fits.gz", package="pylira.data"
+    )
+    psf = fits.getdata(filename)
+
+    if cutout:
+        psf_cutout = (slice(14, 31), slice(15, 32))
+        psf = psf[psf_cutout]
+
+        counts_cutout = (slice(65, 193), slice(64, 192))
+        counts = counts[counts_cutout]
+        wcs = wcs[counts_cutout]
+
+    background = np.zeros(counts.shape)
+    exposure = np.ones(counts.shape)
+
+    return {
+        "counts": counts,
+        "psf": psf,
+        "exposure": exposure,
+        "background": background,
+        "wcs": wcs,
+    }
```

### Comparing `pylira-0.1/pylira/data/files/lincoln.png` & `pylira-0.2/pylira/data/files/lincoln.png`

 * *Files identical despite different names*

### Comparing `pylira-0.1/pylira/data/files/output-par.txt` & `pylira-0.2/pylira/data/files/output-par.txt`

 * *Files identical despite different names*

### Comparing `pylira-0.1/pylira/data/files/output.txt` & `pylira-0.2/pylira/data/files/output.txt`

 * *Files identical despite different names*

### Comparing `pylira-0.1/pylira/data/tests/test_core.py` & `pylira-0.2/pylira/data/tests/test_core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,71 @@
+import pytest
 import numpy as np
 from numpy.testing import assert_allclose
-import pytest
 from pylira.data import (
-    point_source_gauss_psf,
+    chandra_gc,
     disk_source_gauss_psf,
     gauss_and_point_sources_gauss_psf,
     lincoln,
+    point_source_gauss_psf,
 )
 
 
 @pytest.fixture()
 def random_state():
     return np.random.RandomState(836)
 
 
 def test_data_point_source_gauss_psf(random_state):
     data = point_source_gauss_psf(random_state=random_state)
 
     assert_allclose(data["counts"][0][0], 2)
     assert_allclose(data["exposure"][0][0], 1)
     assert_allclose(data["background"][0][0], 2.0)
-    assert_allclose(data["psf"][0][0], 1.44298e-05, rtol=1e-5)
-    assert_allclose(data["flux"][16][16], 1000, rtol=1e-5)
+    assert_allclose(data["psf"][0][0], 1.44298e-05, rtol=1e-2)
+    assert_allclose(data["flux"][16][16], 1000, rtol=1e-2)
 
 
 def test_data_disk_source_gauss_psf(random_state):
     data = disk_source_gauss_psf(random_state=random_state)
 
     assert_allclose(data["counts"][0][0], 1)
     assert_allclose(data["exposure"][0][0], 0.5)
     assert_allclose(data["background"][0][0], 2.0)
-    assert_allclose(data["psf"][0][0], 1.44298e-05, rtol=1e-5)
-    assert_allclose(data["flux"][16][16], 35.367765, rtol=1e-5)
+    assert_allclose(data["psf"][0][0], 1.44298e-05, rtol=1e-2)
+    assert_allclose(data["flux"][16][16], 35.367765, rtol=1e-2)
 
 
 def test_data_gauss_and_point_sources_gauss_psf(random_state):
     data = gauss_and_point_sources_gauss_psf(random_state=random_state)
 
     assert_allclose(data["counts"][0][0], 1)
     assert_allclose(data["exposure"][0][0], 0.5)
     assert_allclose(data["background"][0][0], 2.0)
-    assert_allclose(data["psf"][0][0], 4.477632e-09, rtol=1e-5)
-    assert_allclose(data["flux"][16][16], 36.664897, rtol=1e-5)
+    assert_allclose(data["psf"][0][0], 4.477632e-09, rtol=1e-2)
+    assert_allclose(data["flux"][16][16], 36.664897, rtol=1e-2)
 
 
 def test_data_lincoln(random_state):
     data = lincoln(random_state=random_state)
 
     assert_allclose(data["counts"][0][0], 1)
     assert_allclose(data["exposure"][0][0], 1)
     assert_allclose(data["background"][0][0], 0)
-    assert_allclose(data["psf"][0][0], 1.990059e-09, rtol=1e-5)
-    assert_allclose(data["flux"][16][16], 3, rtol=1e-5)
+    assert_allclose(data["psf"][0][0], 1.990059e-09, rtol=1e-2)
+    assert_allclose(data["flux"][16][16], 3, rtol=1e-2)
+
+
+def test_data_chandra():
+    data = chandra_gc(obs_id=4683)
+
+    assert_allclose(data["counts"][64][64], 8)
+    assert_allclose(data["exposure"][0][0], 1)
+    assert_allclose(data["background"][0][0], 0)
+    assert_allclose(data["psf"][9][9], 0.034461, rtol=1e-2)
+
+    data = chandra_gc(obs_id=4684)
+
+    assert_allclose(data["counts"][64][64], 17)
+    assert_allclose(data["exposure"][0][0], 1)
+    assert_allclose(data["background"][0][0], 0)
+    assert_allclose(data["psf"][9][9], 0.122544, rtol=1e-2)
```

### Comparing `pylira-0.1/pylira/src/lira.h` & `pylira-0.2/pylira/src/lira.h`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
                       double* ms_al_kap1, double* ms_al_kap3, unsigned int random_seed);
 
 void bayes_image_analysis(double* outmap, double* post_mean, char* out_file_nm,
                           char* param_file_nm, controlType* cont, psfType* psf,
                           expmapType* expmap, cntType* obs, cntType* deblur,
                           cntType* src, cntType* bkg, mrfType* mrf, msType* ms,
                           llikeType* llike, scalemodelType* bkg_scale, unsigned int random_seed);
-                          
+
 int printf_d(const char*format,...){
 #ifdef DEBUG
   va_list vl;
   va_start(vl, format);
   auto ret = printf(format, vl);
   va_end(vl);
   return ret;
@@ -1632,19 +1632,19 @@
 
   FILE* param_file; /* the parameter output file */
   if (!(param_file = fopen(param_file_nm, "w")))
     c_error("Could not open the PARAMETER file");
   print_param_file_header(param_file, cont, expmap, ms);
 
   /********** Initialize the Random Seed ************/
-  if (random_seed = 0) random_seed = time(NULL);
+  if (random_seed == 0) random_seed = time(NULL);
+
+  std::srand(random_seed);
+  set_seed(rand(),rand());
 
-  srand(random_seed);
-  set_seed(rand(),rand());  
-     
   //GetRNGstate(); Throws a segfault outside the R environment
 
   /* Compute probability of counts spilling off detector */
   compute_expmap(psf, expmap, cont);
 
   update_deblur_image(expmap, deblur, src, bkg, bkg_scale);
```

### Comparing `pylira-0.1/pylira/src/lirabind.cpp` & `pylira-0.2/pylira/src/lirabind.cpp`

 * *Files identical despite different names*

### Comparing `pylira-0.1/pylira/tests/test_core.py` & `pylira-0.2/pylira/tests/test_core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from copy import deepcopy
 import pytest
 import numpy as np
 from numpy.testing import assert_allclose
 import pylira
+from pylira import LIRADeconvolver, LIRADeconvolverResult, LIRASignificanceEstimator
 from pylira.data import (
-    point_source_gauss_psf,
     disk_source_gauss_psf,
     gauss_and_point_sources_gauss_psf,
+    point_source_gauss_psf,
 )
-from pylira import LIRADeconvolver, LIRADeconvolverResult
 
 
 @pytest.fixture(scope="session")
 def lira_result(tmpdir_factory):
     random_state = np.random.RandomState(836)
     data = point_source_gauss_psf(random_state=random_state)
     data["flux_init"] = data["flux"]
@@ -57,21 +58,17 @@
 
     assert_allclose(config["alpha_init"], [1, 2, 3])
     assert not config["fit_background_scale"]
     assert "alpha_init" in str(deconvolve)
 
 
 def test_lira_deconvolver_run_point_source(lira_result):
-
     assert lira_result.config["random_seed"] == 1346985517
 
-    assert_allclose(lira_result.posterior_mean[16][16], 955.7, rtol=3e-2)
-    assert_allclose(
-        lira_result.posterior_mean, lira_result.posterior_mean_from_trace, atol=1e-2
-    )
+    assert_allclose(lira_result.posterior_mean_from_trace[16][16], 955.7, rtol=3e-2)
 
     assert lira_result.posterior_mean[16][16] > 700
     assert lira_result.parameter_trace["smoothingParam0"][-1] > 0
     assert "alpha_init" in lira_result.config
 
     # check total flux conservation
     assert_allclose(np.nansum(lira_result.posterior_mean), 985, atol=10)
@@ -83,14 +80,28 @@
     assert_allclose(np.mean(trace_par["smoothingParam0"][idx]), 0.056, rtol=0.1)
     assert_allclose(np.mean(trace_par["smoothingParam1"][idx]), 0.060, rtol=0.1)
     assert_allclose(np.mean(trace_par["smoothingParam2"][idx]), 0.060, rtol=0.1)
     assert_allclose(np.mean(trace_par["smoothingParam3"][idx]), 0.062, rtol=0.1)
     assert_allclose(np.mean(trace_par["smoothingParam4"][idx]), 0.070, rtol=0.1)
 
 
+def test_reduce_write_read(tmpdir, lira_result):
+    filename = tmpdir / "reduced.fits"
+    lira_result.reduce_to_mean_std().write(filename)
+
+    reduced = LIRADeconvolverResult.read(filename)
+
+    assert_allclose(
+        lira_result.posterior_mean_from_trace, reduced.posterior_mean, rtol=1e-5
+    )
+    assert_allclose(
+        lira_result.posterior_std_from_trace, reduced.posterior_std, rtol=1e-5
+    )
+
+
 @pytest.mark.xfail
 # TODO: make LIRA work for extended sources...
 def test_lira_deconvolver_run_disk_source(tmpdir):
     data = disk_source_gauss_psf()
     data["flux_init"] = data["flux"]
 
     alpha_init = 0.02 * np.ones(np.log2(data["counts"].shape[0]).astype(int))
@@ -194,7 +205,83 @@
 
     new_result = LIRADeconvolverResult.read(filename)
 
     assert_allclose(lira_result.config["alpha_init"], new_result.config["alpha_init"])
     assert_allclose(lira_result.posterior_mean, new_result.posterior_mean)
 
     assert lira_result.image_trace.shape == new_result.image_trace.shape
+
+
+def test_lira_significance_estimator(lira_result):
+    replica_res = [deepcopy(lira_result) for i in range(50)]
+    random_state = np.random.RandomState(836)
+    data = point_source_gauss_psf(random_state=random_state)
+
+    test_labels = np.zeros(data["background"].shape)
+    test_labels[15:18, 15:18] = 1
+
+    sig_est = LIRASignificanceEstimator(lira_result, replica_res, test_labels)
+    pvals, _, _, _, _ = sig_est.estimate_p_values(data)
+
+    assert pvals["0.0"] == 0.99
+    assert pvals["1.0"] == 0.99
+
+
+def test_random_seed_same():
+    random_state = np.random.RandomState(334)
+
+    data = point_source_gauss_psf(random_state=random_state)
+
+    data["flux_init"] = np.ones((32, 32))
+    alpha_init = np.ones(5)
+
+    deconvolve_1 = LIRADeconvolver(
+        alpha_init=alpha_init,
+        n_iter_max=10,
+        n_burn_in=0,
+        random_state=np.random.RandomState(334),
+    )
+    result_1 = deconvolve_1.run(data=data)
+
+    deconvolve_2 = LIRADeconvolver(
+        alpha_init=alpha_init,
+        n_iter_max=10,
+        n_burn_in=0,
+        random_state=np.random.RandomState(334),
+    )
+    result_2 = deconvolve_2.run(data=data)
+
+    assert result_1.config["random_seed"] == 1022788739
+    assert result_2.config["random_seed"] == 1022788739
+
+    assert_allclose(
+        result_1.posterior_mean[0, 0], result_2.posterior_mean[0, 0], rtol=1e-5
+    )
+
+
+def test_random_seed_different():
+    random_state = np.random.RandomState(334)
+
+    data = point_source_gauss_psf(random_state=random_state)
+    data["flux_init"] = np.ones((32, 32))
+    alpha_init = np.ones(5)
+
+    deconvolve_1 = LIRADeconvolver(
+        alpha_init=alpha_init,
+        n_iter_max=10,
+        n_burn_in=0,
+        random_state=np.random.RandomState(394),
+    )
+    result_1 = deconvolve_1.run(data=data)
+
+    deconvolve_2 = LIRADeconvolver(
+        alpha_init=alpha_init,
+        n_iter_max=10,
+        n_burn_in=0,
+        random_state=np.random.RandomState(434),
+    )
+    result_2 = deconvolve_2.run(data=data)
+
+    assert result_1.config["random_seed"] == 2187641588
+    assert result_2.config["random_seed"] == 1518241554
+
+    assert not np.allclose(result_1.posterior_mean[0, 0], result_2.posterior_mean[0, 0])
```

### Comparing `pylira-0.1/pylira/utils/convolution.py` & `pylira-0.2/pylira/utils/convolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 
-
 __all__ = ["fftconvolve"]
 
 
 def _centered(arr, newshape):
     # Return the center newshape portion of the array.
     newshape = np.asarray(newshape)
     currshape = np.array(arr.shape)
```

### Comparing `pylira-0.1/pylira/utils/io.py` & `pylira-0.2/pylira/utils/io.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
-from astropy.table import Table
 from astropy.io import fits
+from astropy.table import Table
 from astropy.wcs import WCS
 
 
 def read_parameter_trace_file(filename, format="ascii"):
     """Read LIRA parameter output file
 
     Parameters
@@ -68,30 +68,43 @@
         Overwrite file.
     """
     if result.wcs:
         header = result.wcs.to_header()
     else:
         header = None
 
+    hdulist = fits.HDUList()
+
+    # Primary HDU
     primary_hdu = fits.PrimaryHDU(
         header=header,
         data=result.posterior_mean,
     )
+    hdulist.append(primary_hdu)
+
+    posterior_std_hdu = fits.ImageHDU(
+        data=result.posterior_std,
+        name="POSTERIOR_STD",
+    )
+    hdulist.append(posterior_std_hdu)
 
+    # Parameter trace HDU
     table = result.parameter_trace.copy()
     table.meta = None
     parameter_trace_hdu = fits.BinTableHDU(table, name="PARAMETER_TRACE")
+    hdulist.append(parameter_trace_hdu)
 
-    image_trace_hdu = fits.ImageHDU(data=result.image_trace, name="IMAGE_TRACE")
+    # Image trace HDU
+    if result.image_trace is not None:
+        image_trace_hdu = fits.ImageHDU(data=result.image_trace, name="IMAGE_TRACE")
+        hdulist.append(image_trace_hdu)
 
+    # Config HDU
     config_hdu = fits.BinTableHDU(result.config_table, name="CONFIG")
-
-    hdulist = fits.HDUList(
-        [primary_hdu, parameter_trace_hdu, image_trace_hdu, config_hdu]
-    )
+    hdulist.append(config_hdu)
 
     hdulist.writeto(filename, overwrite=overwrite)
 
 
 def read_from_fits(filename):
     """Read LIRA result from FITS.
 
@@ -111,18 +124,21 @@
 
     config_table = Table.read(hdulist["CONFIG"])
     config = dict(config_table[0])
 
     paramter_trace = Table.read(hdulist["PARAMETER_TRACE"])
     posterior_mean = hdulist["PRIMARY"].data
 
+    posterior_std = hdulist["POSTERIOR_STD"].data
+
     # define location for lazy loading
     image_trace = {"filename": filename, "format": "fits"}
     return {
         "posterior_mean": posterior_mean,
+        "posterior_std": posterior_std,
         "config": config,
         "parameter_trace": paramter_trace,
         "image_trace": image_trace,
         "wcs": wcs,
     }
```

### Comparing `pylira-0.1/pylira/utils/plot.py` & `pylira-0.2/pylira/utils/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 from itertools import zip_longest
 import numpy as np
 from astropy.visualization import simple_norm
 from .priors import f_hyperprior_lira
 
-
 __all__ = [
     "plot_example_dataset",
     "plot_parameter_traces",
     "plot_parameter_distributions",
     "plot_pixel_trace",
     "plot_pixel_trace_neighbours",
 ]
 
 
+def get_grid_figsize(width, ncols, nrows):
+    height = width * (nrows / ncols)
+    return width, height
+
+
 def plot_example_dataset(data, figsize=(12, 7), **kwargs):
     """Plot example dataset
 
     Parameters
     ----------
     data : dict of `~numpy.ndarray`
         Data
     figsize : tuple
         Figure size
     **kwargs : dict
         Keyword arguments passed to `~matplotlib.pyplot.imshow`
     """
     import matplotlib.pyplot as plt
 
-    fig, axes = plt.subplots(nrows=2, ncols=3, figsize=figsize)
+    data = data.copy()
 
-    for name, ax in zip(data.keys(), axes.flat):
-        im = ax.imshow(data[name], origin="lower", **kwargs)
-        ax.set_title(name.title())
-        fig.colorbar(im, ax=ax)
+    wcs = data.pop("wcs", None)
 
-    axes.flat[-1].set_visible(False)
+    fig, axes = plt.subplots(
+        nrows=2,
+        ncols=3,
+        figsize=figsize,
+        subplot_kw={"projection": wcs},
+    )
 
+    for name, ax in zip_longest(data.keys(), axes.flat):
+        if name is None:
+            ax.set_visible(False)
+            continue
 
-def get_grid_figsize(width, ncols, nrows):
-    height = width * (nrows / ncols)
-    return width, height
+        im = ax.imshow(data[name], origin="lower", **kwargs)
+        ax.set_title(name.title())
+        fig.colorbar(im, ax=ax)
 
 
 def plot_trace(ax, idx, trace, n_burn_in, **kwargs):
     """Plot a single parameter trace
 
     Parameters
     ----------
@@ -338,15 +348,15 @@
 def plot_hyperpriors_lira(
     figsize=(12, 4),
     ncols=2,
     alphas=None,
     ms_al_kap1=0,
     ms_al_kap2=1000,
     ms_al_kap3=3,
-    **kwargs
+    **kwargs,
 ):
     """Plot hyperprior distributions
 
     Parameters
     ----------
     figsize: tuple of float
         Figure size
@@ -384,14 +394,14 @@
         axes = np.asanyarray([axes])
 
     for idx, ax in enumerate(axes.flat):
         values = f_hyperprior_lira(
             alpha=alphas,
             ms_al_kap1=ms_al_kap1[idx],
             ms_al_kap2=ms_al_kap2[idx],
-            ms_al_kap3=ms_al_kap3[idx]
+            ms_al_kap3=ms_al_kap3[idx],
         )
         ax.plot(alphas, values, **kwargs)
         ax.set_xlabel("Alpha")
         ax.set_ylabel("PDF / A.U.")
 
     return axes
```

### Comparing `pylira-0.1/pylira/utils/priors.py` & `pylira-0.2/pylira/utils/priors.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     Returns
     -------
     value : `~numpy.ndarray`
         Value
     """
     prefactor = (alpha * delta) ** index
-    exponential = np.exp(-delta * alpha ** index_alpha / index_alpha)
+    exponential = np.exp(-delta * alpha**index_alpha / index_alpha)
     return prefactor * exponential
 
 
 def f_hyperprior_lira(alpha, ms_al_kap1=0, ms_al_kap2=1000, ms_al_kap3=3):
     """Hyperprior distribution following LIRA implementation
 
     Parameters
@@ -44,8 +44,10 @@
     value : `~numpy.ndarray`
         Value
 
     """
     delta = ms_al_kap2 * ms_al_kap3
     index = ms_al_kap1
     index_alpha = ms_al_kap3
-    return f_hyperprior_esch(alpha=alpha, delta=delta, index=index, index_alpha=index_alpha)
+    return f_hyperprior_esch(
+        alpha=alpha, delta=delta, index=index, index_alpha=index_alpha
+    )
```

### Comparing `pylira-0.1/pylira/utils/tests/test_io.py` & `pylira-0.2/pylira/utils/tests/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from numpy.testing import assert_allclose
-from pylira.utils.io import read_parameter_trace_file, read_image_trace_file
 from astropy.utils.data import get_pkg_data_filename
+from pylira.utils.io import read_image_trace_file, read_parameter_trace_file
 
 
 def test_read_parameter_trace_file():
     filename = get_pkg_data_filename("files/output-par.txt", package="pylira.data")
 
     table = read_parameter_trace_file(filename)
```

### Comparing `pylira-0.1/pylira/utils/tests/test_plot.py` & `pylira-0.2/pylira/utils/tests/test_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from astropy.utils.data import get_pkg_data_filename
+from pylira.utils.io import read_image_trace_file, read_parameter_trace_file
 from pylira.utils.plot import (
-    plot_parameter_traces,
     plot_parameter_distributions,
+    plot_parameter_traces,
     plot_pixel_trace,
     plot_pixel_trace_neighbours,
 )
 
-from pylira.utils.io import read_parameter_trace_file, read_image_trace_file
-
 
 def test_plot_parameter_traces():
     filename = get_pkg_data_filename("files/output-par.txt", package="pylira.data")
     table = read_parameter_trace_file(filename)
 
     axes = plot_parameter_traces(table)
     assert axes.size == 9
```

### Comparing `pylira-0.1/pylira.egg-info/PKG-INFO` & `pylira-0.2/pylira.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pylira
-Version: 0.1
+Version: 0.2
 Summary: A Python package for Bayesian low-counts image reconstruction and analysis
 Home-page: https://pylira.readthedocs.io/
 Author: pylira developers
 Author-email: 
 License: GNU GPL v3+
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
@@ -64,9 +63,7 @@
 the errors and assumptions that seasoned contributors have glossed over.
 
 Note: This disclaimer was originally written by
 `Adrienne Lowe <https://github.com/adriennefriend>`_ for a
 `PyCon talk <https://www.youtube.com/watch?v=6Uj746j9Heo>`_, and was adapted by
 pylira based on its use in the README file for the
 `MetPy project <https://github.com/Unidata/MetPy>`_.
-
-
```

### Comparing `pylira-0.1/pylira.egg-info/SOURCES.txt` & `pylira-0.2/pylira.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 .clang-format
 .gitignore
+.pre-commit-config.yaml
 .readthedocs.yml
 MANIFEST.in
 README.rst
 environment.yaml
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/ci_cron_weekly.yml
 .github/workflows/ci_tests.yml
+.github/workflows/release.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/pylira-logo.png
 docs/pylira/changelog.rst
 docs/pylira/developer.rst
@@ -41,14 +43,18 @@
 pylira.egg-info/dependency_links.txt
 pylira.egg-info/not-zip-safe
 pylira.egg-info/requires.txt
 pylira.egg-info/top_level.txt
 pylira/data/README.rst
 pylira/data/__init__.py
 pylira/data/core.py
+pylira/data/files/chandra-counts-obs-id-4683.fits.gz
+pylira/data/files/chandra-counts-obs-id-4684.fits.gz
+pylira/data/files/chandra-psf-obs-id-4683.fits.gz
+pylira/data/files/chandra-psf-obs-id-4684.fits.gz
 pylira/data/files/lincoln.png
 pylira/data/files/output-par.txt
 pylira/data/files/output.txt
 pylira/data/tests/__init__.py
 pylira/data/tests/test_core.py
 pylira/extern/__init__.py
 pylira/src/lira.h
```

### Comparing `pylira-0.1/setup.py` & `pylira-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 # NOTE: The configuration for the package, including the name, version, and
 # other information are set in the setup.cfg file.
 
 import os
+import subprocess
 import sys
 from pathlib import Path
-import subprocess
-from setuptools import setup
-from setuptools.command.build_clib import build_clib
 from pybind11.setup_helpers import Pybind11Extension, build_ext
-
+from setuptools import setup
 
 # First provide helpful messages if contributors try and run legacy commands
 # for tests or docs.
 
 TEST_HELP = """
 Note: running tests is no longer done using 'python setup.py test'. Instead
 you will need to run:
@@ -33,15 +31,15 @@
     pytest
 
 For more information, see:
 
   http://docs.astropy.org/en/latest/development/testguide.html#running-tests
 """
 
-if 'test' in sys.argv:
+if "test" in sys.argv:
     print(TEST_HELP)
     sys.exit(1)
 
 DOCS_HELP = """
 Note: building the documentation is no longer done using
 'python setup.py build_docs'. Instead you will need to run:
 
@@ -58,15 +56,15 @@
     make html
 
 For more information, see:
 
   http://docs.astropy.org/en/latest/install.html#builddocs
 """
 
-if 'build_docs' in sys.argv or 'build_sphinx' in sys.argv:
+if "build_docs" in sys.argv or "build_sphinx" in sys.argv:
     print(DOCS_HELP)
     sys.exit(1)
 
 VERSION_TEMPLATE = """
 # Note that we need to fall back to the hard-coded version if either
 # setuptools_scm can't be imported or setuptools_scm can't determine the
 # version, so we catch the generic 'Exception'.
@@ -104,12 +102,14 @@
         include_dirs=include_dirs,
         libraries=["Rmath"],
         library_dirs=library_dirs,
     ),
 ]
 
 setup(
-    use_scm_version={'write_to': os.path.join('pylira', 'version.py'),
-                     'write_to_template': VERSION_TEMPLATE},
+    use_scm_version={
+        "write_to": os.path.join("pylira", "version.py"),
+        "write_to_template": VERSION_TEMPLATE,
+    },
     ext_modules=ext_modules,
-    cmdclass={'build_ext': build_ext},
+    cmdclass={"build_ext": build_ext},
 )
```

### Comparing `pylira-0.1/tox.ini` & `pylira-0.2/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,22 @@
     NIGHTLY = https://pypi.anaconda.org/scipy-wheels-nightly/simple
 
 [testenv]
 # Suppress display of matplotlib plots generated during docs build
 setenv = MPLBACKEND=agg
 
 # Pass through the following environment variables which may be needed for the CI
-passenv = HOME WINDIR LC_ALL LC_CTYPE CC CI TRAVIS
+passenv = 
+    HOME
+    WINDIR
+    LC_ALL
+    LC_CTYPE
+    CC
+    CI
+    TRAVIS
 
 # Run the tests in a temporary directory to make sure that we don't import
 # this package from the source tree
 changedir = .tmp/{envname}
 
 # tox environments are constructed with so-called 'factors' (or terms)
 # separated by hyphens, e.g. test-devdeps-cov. Lines below starting with factor:
```

