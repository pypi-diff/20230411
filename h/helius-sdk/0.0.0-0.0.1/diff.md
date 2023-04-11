# Comparing `tmp/helius-sdk-0.0.0.tar.gz` & `tmp/helius-sdk-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helius-sdk-0.0.0.tar", last modified: Tue Apr 11 16:24:12 2023, max compression
+gzip compressed data, was "helius-sdk-0.0.1.tar", last modified: Tue Apr 11 16:30:52 2023, max compression
```

## Comparing `helius-sdk-0.0.0.tar` & `helius-sdk-0.0.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:24:12.486444 helius-sdk-0.0.0/
--rw-r--r--   0 mayurchougule   (501) staff       (20)      630 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/.bumpversion.cfg
--rw-r--r--   0 mayurchougule   (501) staff       (20)     2792 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/.cookiecutterrc
--rw-r--r--   0 mayurchougule   (501) staff       (20)      178 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/.coveragerc
--rw-r--r--   0 mayurchougule   (501) staff       (20)      353 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/.editorconfig
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:24:12.476897 helius-sdk-0.0.0/.github/
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:24:12.480474 helius-sdk-0.0.0/.github/workflows/
--rw-r--r--   0 mayurchougule   (501) staff       (20)     4082 2023-04-09 20:21:51.000000 helius-sdk-0.0.0/.github/workflows/github-actions.yml
--rw-r--r--   0 mayurchougule   (501) staff       (20)      636 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0 mayurchougule   (501) staff       (20)      231 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/.readthedocs.yml
--rw-r--r--   0 mayurchougule   (501) staff       (20)       61 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/AUTHORS.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)       86 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/CHANGELOG.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)     2433 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/CONTRIBUTING.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1102 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/LICENSE
--rw-r--r--   0 mayurchougule   (501) staff       (20)      427 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/MANIFEST.in
--rw-r--r--   0 mayurchougule   (501) staff       (20)     2913 2023-04-11 16:24:12.486549 helius-sdk-0.0.0/PKG-INFO
--rw-r--r--   0 mayurchougule   (501) staff       (20)     2655 2023-04-11 16:17:53.000000 helius-sdk-0.0.0/README.rst
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:24:12.480861 helius-sdk-0.0.0/ci/
--rwxr-xr-x   0 mayurchougule   (501) staff       (20)     2930 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/ci/bootstrap.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)       96 2023-04-09 22:51:17.000000 helius-sdk-0.0.0/ci/requirements.txt
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:24:12.477070 helius-sdk-0.0.0/ci/templates/
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:24:12.477118 helius-sdk-0.0.0/ci/templates/.github/
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:24:12.481093 helius-sdk-0.0.0/ci/templates/.github/workflows/
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1977 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:24:12.482671 helius-sdk-0.0.0/docs/
--rw-r--r--   0 mayurchougule   (501) staff       (20)       28 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/docs/authors.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)       30 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/docs/changelog.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1201 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/docs/conf.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)       33 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/docs/contributing.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)      244 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/docs/index.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)       90 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/docs/installation.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)       27 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/docs/readme.rst
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:24:12.482994 helius-sdk-0.0.0/docs/reference/
--rw-r--r--   0 mayurchougule   (501) staff       (20)      110 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/docs/reference/helius_sdk.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)       62 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/docs/reference/index.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)       30 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/docs/requirements.txt
--rw-r--r--   0 mayurchougule   (501) staff       (20)      109 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/docs/spelling_wordlist.txt
--rw-r--r--   0 mayurchougule   (501) staff       (20)       72 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/docs/usage.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)      160 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/pyproject.toml
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1715 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/pytest.ini
--rw-r--r--   0 mayurchougule   (501) staff       (20)      308 2023-04-11 16:24:12.486911 helius-sdk-0.0.0/setup.cfg
--rwxr-xr-x   0 mayurchougule   (501) staff       (20)     2846 2023-04-10 03:33:18.000000 helius-sdk-0.0.0/setup.py
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:24:12.477404 helius-sdk-0.0.0/src/
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:24:12.484725 helius-sdk-0.0.0/src/helius_sdk/
--rw-r--r--   0 mayurchougule   (501) staff       (20)       22 2023-04-09 20:32:10.000000 helius-sdk-0.0.0/src/helius_sdk/__init__.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1213 2023-04-10 03:30:41.000000 helius-sdk-0.0.0/src/helius_sdk/__main__.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)      741 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/src/helius_sdk/cli.py
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:24:12.485908 helius-sdk-0.0.0/src/helius_sdk/conf/
--rw-r--r--   0 mayurchougule   (501) staff       (20)       94 2023-04-10 03:42:48.000000 helius-sdk-0.0.0/src/helius_sdk/conf/base.yml
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1602 2023-04-10 03:43:00.000000 helius-sdk-0.0.0/src/helius_sdk/core.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)     4152 2023-04-10 03:14:07.000000 helius-sdk-0.0.0/src/helius_sdk/event.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1217 2023-04-10 03:20:40.000000 helius-sdk-0.0.0/src/helius_sdk/nft.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)      935 2023-04-10 03:27:09.000000 helius-sdk-0.0.0/src/helius_sdk/transaction.py
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:24:12.485795 helius-sdk-0.0.0/src/helius_sdk.egg-info/
--rw-r--r--   0 mayurchougule   (501) staff       (20)     2913 2023-04-11 16:24:12.000000 helius-sdk-0.0.0/src/helius_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1088 2023-04-11 16:24:12.000000 helius-sdk-0.0.0/src/helius_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mayurchougule   (501) staff       (20)        1 2023-04-11 16:24:12.000000 helius-sdk-0.0.0/src/helius_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mayurchougule   (501) staff       (20)       52 2023-04-11 16:24:12.000000 helius-sdk-0.0.0/src/helius_sdk.egg-info/entry_points.txt
--rw-r--r--   0 mayurchougule   (501) staff       (20)        1 2023-04-09 20:27:43.000000 helius-sdk-0.0.0/src/helius_sdk.egg-info/not-zip-safe
--rw-r--r--   0 mayurchougule   (501) staff       (20)        6 2023-04-11 16:24:12.000000 helius-sdk-0.0.0/src/helius_sdk.egg-info/requires.txt
--rw-r--r--   0 mayurchougule   (501) staff       (20)       11 2023-04-11 16:24:12.000000 helius-sdk-0.0.0/src/helius_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:24:12.486128 helius-sdk-0.0.0/tests/
--rw-r--r--   0 mayurchougule   (501) staff       (20)      219 2023-04-09 22:47:53.000000 helius-sdk-0.0.0/tests/test_helius_sdk.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1727 2023-04-09 20:21:46.000000 helius-sdk-0.0.0/tox.ini
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:30:52.778386 helius-sdk-0.0.1/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      630 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/.bumpversion.cfg
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     2792 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/.cookiecutterrc
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      178 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/.coveragerc
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      353 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/.editorconfig
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:30:52.767767 helius-sdk-0.0.1/.github/
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:30:52.771432 helius-sdk-0.0.1/.github/workflows/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     4082 2023-04-09 20:21:51.000000 helius-sdk-0.0.1/.github/workflows/github-actions.yml
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      636 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      231 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/.readthedocs.yml
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       61 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/AUTHORS.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       86 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/CHANGELOG.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     2433 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1102 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/LICENSE
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      427 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/MANIFEST.in
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     2913 2023-04-11 16:30:52.778504 helius-sdk-0.0.1/PKG-INFO
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     2655 2023-04-11 16:17:53.000000 helius-sdk-0.0.1/README.rst
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:30:52.771837 helius-sdk-0.0.1/ci/
+-rwxr-xr-x   0 mayurchougule   (501) staff       (20)     2930 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/ci/bootstrap.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       96 2023-04-09 22:51:17.000000 helius-sdk-0.0.1/ci/requirements.txt
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:30:52.767950 helius-sdk-0.0.1/ci/templates/
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:30:52.767994 helius-sdk-0.0.1/ci/templates/.github/
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:30:52.772137 helius-sdk-0.0.1/ci/templates/.github/workflows/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1977 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:30:52.774129 helius-sdk-0.0.1/docs/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       28 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/docs/authors.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       30 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/docs/changelog.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1201 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/docs/conf.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       33 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/docs/contributing.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      244 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/docs/index.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       90 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/docs/installation.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       27 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/docs/readme.rst
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:30:52.774546 helius-sdk-0.0.1/docs/reference/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      110 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/docs/reference/helius_sdk.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       62 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/docs/reference/index.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       30 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/docs/requirements.txt
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      109 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/docs/spelling_wordlist.txt
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       72 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/docs/usage.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      160 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/pyproject.toml
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1715 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/pytest.ini
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      308 2023-04-11 16:30:52.778802 helius-sdk-0.0.1/setup.cfg
+-rwxr-xr-x   0 mayurchougule   (501) staff       (20)     2846 2023-04-11 16:30:28.000000 helius-sdk-0.0.1/setup.py
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:30:52.768290 helius-sdk-0.0.1/src/
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:30:52.776519 helius-sdk-0.0.1/src/helius_sdk/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       22 2023-04-09 20:32:10.000000 helius-sdk-0.0.1/src/helius_sdk/__init__.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1213 2023-04-10 03:30:41.000000 helius-sdk-0.0.1/src/helius_sdk/__main__.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      741 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/src/helius_sdk/cli.py
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:30:52.777930 helius-sdk-0.0.1/src/helius_sdk/conf/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       94 2023-04-10 03:42:48.000000 helius-sdk-0.0.1/src/helius_sdk/conf/base.yml
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1602 2023-04-10 03:43:00.000000 helius-sdk-0.0.1/src/helius_sdk/core.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     4152 2023-04-10 03:14:07.000000 helius-sdk-0.0.1/src/helius_sdk/event.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1217 2023-04-10 03:20:40.000000 helius-sdk-0.0.1/src/helius_sdk/nft.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      935 2023-04-10 03:27:09.000000 helius-sdk-0.0.1/src/helius_sdk/transaction.py
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:30:52.777799 helius-sdk-0.0.1/src/helius_sdk.egg-info/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     2913 2023-04-11 16:30:52.000000 helius-sdk-0.0.1/src/helius_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1088 2023-04-11 16:30:52.000000 helius-sdk-0.0.1/src/helius_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 mayurchougule   (501) staff       (20)        1 2023-04-11 16:30:52.000000 helius-sdk-0.0.1/src/helius_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       52 2023-04-11 16:30:52.000000 helius-sdk-0.0.1/src/helius_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 mayurchougule   (501) staff       (20)        1 2023-04-09 20:27:43.000000 helius-sdk-0.0.1/src/helius_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 mayurchougule   (501) staff       (20)        6 2023-04-11 16:30:52.000000 helius-sdk-0.0.1/src/helius_sdk.egg-info/requires.txt
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       11 2023-04-11 16:30:52.000000 helius-sdk-0.0.1/src/helius_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:30:52.778164 helius-sdk-0.0.1/tests/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      219 2023-04-09 22:47:53.000000 helius-sdk-0.0.1/tests/test_helius_sdk.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1727 2023-04-09 20:21:46.000000 helius-sdk-0.0.1/tox.ini
```

### Comparing `helius-sdk-0.0.0/.bumpversion.cfg` & `helius-sdk-0.0.1/.bumpversion.cfg`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/.cookiecutterrc` & `helius-sdk-0.0.1/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/.github/workflows/github-actions.yml` & `helius-sdk-0.0.1/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/.pre-commit-config.yaml` & `helius-sdk-0.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/CONTRIBUTING.rst` & `helius-sdk-0.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/LICENSE` & `helius-sdk-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/PKG-INFO` & `helius-sdk-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: helius-sdk
-Version: 0.0.0
+Version: 0.0.1
 Summary: Helius SDK
 Home-page: https://github.com/mmchougule/helius-sdk-python
 Author: Mayur Chougule
 Author-email: mayurchougule1@gmail.com
 License: MIT
 Project-URL: Documentation, https://helius-sdk-python.readthedocs.io/
 Project-URL: Changelog, https://helius-sdk-python.readthedocs.io/en/latest/changelog.html
```

### Comparing `helius-sdk-0.0.0/README.rst` & `helius-sdk-0.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/ci/bootstrap.py` & `helius-sdk-0.0.1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/ci/templates/.github/workflows/github-actions.yml` & `helius-sdk-0.0.1/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/docs/conf.py` & `helius-sdk-0.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/pytest.ini` & `helius-sdk-0.0.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/setup.py` & `helius-sdk-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def read(*names, **kwargs):
     with io.open(join(dirname(__file__), *names), encoding=kwargs.get('encoding', 'utf8')) as fh:
         return fh.read()
 
 
 setup(
     name='helius-sdk',
-    version='0.0.0',
+    version='0.0.1',
     license='MIT',
     description='Helius SDK',
     long_description='{}\n{}'.format(
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst')),
     ),
     author='Mayur Chougule',
```

### Comparing `helius-sdk-0.0.0/src/helius_sdk/__main__.py` & `helius-sdk-0.0.1/src/helius_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/src/helius_sdk/cli.py` & `helius-sdk-0.0.1/src/helius_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/src/helius_sdk/core.py` & `helius-sdk-0.0.1/src/helius_sdk/core.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/src/helius_sdk/event.py` & `helius-sdk-0.0.1/src/helius_sdk/event.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/src/helius_sdk/nft.py` & `helius-sdk-0.0.1/src/helius_sdk/nft.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/src/helius_sdk/transaction.py` & `helius-sdk-0.0.1/src/helius_sdk/transaction.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/src/helius_sdk.egg-info/PKG-INFO` & `helius-sdk-0.0.1/src/helius_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: helius-sdk
-Version: 0.0.0
+Version: 0.0.1
 Summary: Helius SDK
 Home-page: https://github.com/mmchougule/helius-sdk-python
 Author: Mayur Chougule
 Author-email: mayurchougule1@gmail.com
 License: MIT
 Project-URL: Documentation, https://helius-sdk-python.readthedocs.io/
 Project-URL: Changelog, https://helius-sdk-python.readthedocs.io/en/latest/changelog.html
```

### Comparing `helius-sdk-0.0.0/src/helius_sdk.egg-info/SOURCES.txt` & `helius-sdk-0.0.1/src/helius_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.0/tox.ini` & `helius-sdk-0.0.1/tox.ini`

 * *Files identical despite different names*

