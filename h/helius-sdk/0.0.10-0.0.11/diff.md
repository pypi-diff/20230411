# Comparing `tmp/helius-sdk-0.0.10.tar.gz` & `tmp/helius-sdk-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helius-sdk-0.0.10.tar", last modified: Tue Apr 11 16:43:23 2023, max compression
+gzip compressed data, was "helius-sdk-0.0.11.tar", last modified: Tue Apr 11 16:53:26 2023, max compression
```

## Comparing `helius-sdk-0.0.10.tar` & `helius-sdk-0.0.11.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:43:23.123042 helius-sdk-0.0.10/
--rw-r--r--   0 mayurchougule   (501) staff       (20)      630 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/.bumpversion.cfg
--rw-r--r--   0 mayurchougule   (501) staff       (20)     2792 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/.cookiecutterrc
--rw-r--r--   0 mayurchougule   (501) staff       (20)      178 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/.coveragerc
--rw-r--r--   0 mayurchougule   (501) staff       (20)      353 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/.editorconfig
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:43:23.054703 helius-sdk-0.0.10/.github/
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:43:23.058525 helius-sdk-0.0.10/.github/workflows/
--rw-r--r--   0 mayurchougule   (501) staff       (20)     4082 2023-04-09 20:21:51.000000 helius-sdk-0.0.10/.github/workflows/github-actions.yml
--rw-r--r--   0 mayurchougule   (501) staff       (20)      636 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/.pre-commit-config.yaml
--rw-r--r--   0 mayurchougule   (501) staff       (20)      231 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/.readthedocs.yml
--rw-r--r--   0 mayurchougule   (501) staff       (20)       61 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/AUTHORS.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)       86 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/CHANGELOG.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)     2433 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/CONTRIBUTING.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1102 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/LICENSE
--rw-r--r--   0 mayurchougule   (501) staff       (20)      427 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/MANIFEST.in
--rw-r--r--   0 mayurchougule   (501) staff       (20)     2914 2023-04-11 16:43:23.123148 helius-sdk-0.0.10/PKG-INFO
--rw-r--r--   0 mayurchougule   (501) staff       (20)     2655 2023-04-11 16:17:53.000000 helius-sdk-0.0.10/README.rst
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:43:23.058889 helius-sdk-0.0.10/ci/
--rwxr-xr-x   0 mayurchougule   (501) staff       (20)     2930 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/ci/bootstrap.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)       96 2023-04-09 22:51:17.000000 helius-sdk-0.0.10/ci/requirements.txt
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:43:23.054888 helius-sdk-0.0.10/ci/templates/
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:43:23.054939 helius-sdk-0.0.10/ci/templates/.github/
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:43:23.059124 helius-sdk-0.0.10/ci/templates/.github/workflows/
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1977 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:43:23.060912 helius-sdk-0.0.10/docs/
--rw-r--r--   0 mayurchougule   (501) staff       (20)       28 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/docs/authors.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)       30 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/docs/changelog.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1201 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/docs/conf.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)       33 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/docs/contributing.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)      244 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/docs/index.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)       90 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/docs/installation.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)       27 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/docs/readme.rst
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:43:23.061211 helius-sdk-0.0.10/docs/reference/
--rw-r--r--   0 mayurchougule   (501) staff       (20)      110 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/docs/reference/helius_sdk.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)       62 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/docs/reference/index.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)       30 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/docs/requirements.txt
--rw-r--r--   0 mayurchougule   (501) staff       (20)      109 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/docs/spelling_wordlist.txt
--rw-r--r--   0 mayurchougule   (501) staff       (20)       72 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/docs/usage.rst
--rw-r--r--   0 mayurchougule   (501) staff       (20)      176 2023-04-11 16:33:10.000000 helius-sdk-0.0.10/pyproject.toml
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1715 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/pytest.ini
--rw-r--r--   0 mayurchougule   (501) staff       (20)      308 2023-04-11 16:43:23.123431 helius-sdk-0.0.10/setup.cfg
--rwxr-xr-x   0 mayurchougule   (501) staff       (20)     2847 2023-04-11 16:43:00.000000 helius-sdk-0.0.10/setup.py
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:43:23.055237 helius-sdk-0.0.10/src/
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:43:23.121201 helius-sdk-0.0.10/src/helius_sdk/
--rw-r--r--   0 mayurchougule   (501) staff       (20)       22 2023-04-09 20:32:10.000000 helius-sdk-0.0.10/src/helius_sdk/__init__.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1213 2023-04-10 03:30:41.000000 helius-sdk-0.0.10/src/helius_sdk/__main__.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)      741 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/src/helius_sdk/cli.py
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:43:23.122584 helius-sdk-0.0.10/src/helius_sdk/conf/
--rw-r--r--   0 mayurchougule   (501) staff       (20)       94 2023-04-10 03:42:48.000000 helius-sdk-0.0.10/src/helius_sdk/conf/base.yml
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1602 2023-04-10 03:43:00.000000 helius-sdk-0.0.10/src/helius_sdk/core.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)     4152 2023-04-10 03:14:07.000000 helius-sdk-0.0.10/src/helius_sdk/event.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1217 2023-04-10 03:20:40.000000 helius-sdk-0.0.10/src/helius_sdk/nft.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)      935 2023-04-10 03:27:09.000000 helius-sdk-0.0.10/src/helius_sdk/transaction.py
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:43:23.122460 helius-sdk-0.0.10/src/helius_sdk.egg-info/
--rw-r--r--   0 mayurchougule   (501) staff       (20)     2914 2023-04-11 16:43:23.000000 helius-sdk-0.0.10/src/helius_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1088 2023-04-11 16:43:23.000000 helius-sdk-0.0.10/src/helius_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mayurchougule   (501) staff       (20)        1 2023-04-11 16:43:23.000000 helius-sdk-0.0.10/src/helius_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mayurchougule   (501) staff       (20)       52 2023-04-11 16:43:23.000000 helius-sdk-0.0.10/src/helius_sdk.egg-info/entry_points.txt
--rw-r--r--   0 mayurchougule   (501) staff       (20)        1 2023-04-09 20:27:43.000000 helius-sdk-0.0.10/src/helius_sdk.egg-info/not-zip-safe
--rw-r--r--   0 mayurchougule   (501) staff       (20)        6 2023-04-11 16:43:23.000000 helius-sdk-0.0.10/src/helius_sdk.egg-info/requires.txt
--rw-r--r--   0 mayurchougule   (501) staff       (20)       11 2023-04-11 16:43:23.000000 helius-sdk-0.0.10/src/helius_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:43:23.122820 helius-sdk-0.0.10/tests/
--rw-r--r--   0 mayurchougule   (501) staff       (20)      219 2023-04-09 22:47:53.000000 helius-sdk-0.0.10/tests/test_helius_sdk.py
--rw-r--r--   0 mayurchougule   (501) staff       (20)     1727 2023-04-09 20:21:46.000000 helius-sdk-0.0.10/tox.ini
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:53:26.086264 helius-sdk-0.0.11/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      630 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/.bumpversion.cfg
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     2792 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/.cookiecutterrc
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      178 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/.coveragerc
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      353 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/.editorconfig
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:53:26.075942 helius-sdk-0.0.11/.github/
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:53:26.079857 helius-sdk-0.0.11/.github/workflows/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     4082 2023-04-09 20:21:51.000000 helius-sdk-0.0.11/.github/workflows/github-actions.yml
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      636 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/.pre-commit-config.yaml
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      231 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/.readthedocs.yml
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       61 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/AUTHORS.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       86 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/CHANGELOG.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     2433 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/CONTRIBUTING.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1102 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/LICENSE
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      427 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/MANIFEST.in
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     2914 2023-04-11 16:53:26.086573 helius-sdk-0.0.11/PKG-INFO
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     2655 2023-04-11 16:17:53.000000 helius-sdk-0.0.11/README.rst
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:53:26.080347 helius-sdk-0.0.11/ci/
+-rwxr-xr-x   0 mayurchougule   (501) staff       (20)     2930 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/ci/bootstrap.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       96 2023-04-09 22:51:17.000000 helius-sdk-0.0.11/ci/requirements.txt
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:53:26.076134 helius-sdk-0.0.11/ci/templates/
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:53:26.076179 helius-sdk-0.0.11/ci/templates/.github/
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:53:26.080586 helius-sdk-0.0.11/ci/templates/.github/workflows/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1977 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:53:26.082275 helius-sdk-0.0.11/docs/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       28 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/docs/authors.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       30 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/docs/changelog.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1201 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/docs/conf.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       33 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/docs/contributing.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      244 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/docs/index.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       90 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/docs/installation.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       27 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/docs/readme.rst
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:53:26.082557 helius-sdk-0.0.11/docs/reference/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      110 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/docs/reference/helius_sdk.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       62 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/docs/reference/index.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       30 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/docs/requirements.txt
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      109 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/docs/spelling_wordlist.txt
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       72 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/docs/usage.rst
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      176 2023-04-11 16:33:10.000000 helius-sdk-0.0.11/pyproject.toml
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1715 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/pytest.ini
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      308 2023-04-11 16:53:26.086937 helius-sdk-0.0.11/setup.cfg
+-rwxr-xr-x   0 mayurchougule   (501) staff       (20)     2957 2023-04-11 16:53:21.000000 helius-sdk-0.0.11/setup.py
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:53:26.076478 helius-sdk-0.0.11/src/
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:53:26.084047 helius-sdk-0.0.11/src/helius_sdk/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       22 2023-04-09 20:32:10.000000 helius-sdk-0.0.11/src/helius_sdk/__init__.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1213 2023-04-10 03:30:41.000000 helius-sdk-0.0.11/src/helius_sdk/__main__.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      741 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/src/helius_sdk/cli.py
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:53:26.085621 helius-sdk-0.0.11/src/helius_sdk/conf/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       94 2023-04-10 03:42:48.000000 helius-sdk-0.0.11/src/helius_sdk/conf/base.yml
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1602 2023-04-10 03:43:00.000000 helius-sdk-0.0.11/src/helius_sdk/core.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     4152 2023-04-10 03:14:07.000000 helius-sdk-0.0.11/src/helius_sdk/event.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1217 2023-04-10 03:20:40.000000 helius-sdk-0.0.11/src/helius_sdk/nft.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      935 2023-04-10 03:27:09.000000 helius-sdk-0.0.11/src/helius_sdk/transaction.py
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:53:26.085480 helius-sdk-0.0.11/src/helius_sdk.egg-info/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     2914 2023-04-11 16:53:26.000000 helius-sdk-0.0.11/src/helius_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1088 2023-04-11 16:53:26.000000 helius-sdk-0.0.11/src/helius_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 mayurchougule   (501) staff       (20)        1 2023-04-11 16:53:26.000000 helius-sdk-0.0.11/src/helius_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       52 2023-04-11 16:53:26.000000 helius-sdk-0.0.11/src/helius_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 mayurchougule   (501) staff       (20)        1 2023-04-09 20:27:43.000000 helius-sdk-0.0.11/src/helius_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       50 2023-04-11 16:53:26.000000 helius-sdk-0.0.11/src/helius_sdk.egg-info/requires.txt
+-rw-r--r--   0 mayurchougule   (501) staff       (20)       11 2023-04-11 16:53:26.000000 helius-sdk-0.0.11/src/helius_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 mayurchougule   (501) staff       (20)        0 2023-04-11 16:53:26.085958 helius-sdk-0.0.11/tests/
+-rw-r--r--   0 mayurchougule   (501) staff       (20)      219 2023-04-09 22:47:53.000000 helius-sdk-0.0.11/tests/test_helius_sdk.py
+-rw-r--r--   0 mayurchougule   (501) staff       (20)     1727 2023-04-09 20:21:46.000000 helius-sdk-0.0.11/tox.ini
```

### Comparing `helius-sdk-0.0.10/.bumpversion.cfg` & `helius-sdk-0.0.11/.bumpversion.cfg`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/.cookiecutterrc` & `helius-sdk-0.0.11/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/.github/workflows/github-actions.yml` & `helius-sdk-0.0.11/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/.pre-commit-config.yaml` & `helius-sdk-0.0.11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/CONTRIBUTING.rst` & `helius-sdk-0.0.11/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/LICENSE` & `helius-sdk-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/PKG-INFO` & `helius-sdk-0.0.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: helius-sdk
-Version: 0.0.10
+Version: 0.0.11
 Summary: Helius SDK
 Home-page: https://github.com/mmchougule/helius-sdk-python
 Author: Mayur Chougule
 Author-email: mayurchougule1@gmail.com
 License: MIT
 Project-URL: Documentation, https://helius-sdk-python.readthedocs.io/
 Project-URL: Changelog, https://helius-sdk-python.readthedocs.io/en/latest/changelog.html
```

### Comparing `helius-sdk-0.0.10/README.rst` & `helius-sdk-0.0.11/README.rst`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/ci/bootstrap.py` & `helius-sdk-0.0.11/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/ci/templates/.github/workflows/github-actions.yml` & `helius-sdk-0.0.11/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/docs/conf.py` & `helius-sdk-0.0.11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/pytest.ini` & `helius-sdk-0.0.11/pytest.ini`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/setup.py` & `helius-sdk-0.0.11/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def read(*names, **kwargs):
     with io.open(join(dirname(__file__), *names), encoding=kwargs.get('encoding', 'utf8')) as fh:
         return fh.read()
 
 
 setup(
     name='helius-sdk',
-    version='0.0.10',
+    version='0.0.11',
     license='MIT',
     description='Helius SDK',
     long_description='{}\n{}'.format(
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst')),
     ),
     author='Mayur Chougule',
@@ -62,14 +62,20 @@
     },
     keywords=[
         # eg: 'keyword1', 'keyword2', 'keyword3',
     ],
     python_requires='>=3.7',
     install_requires=[
         'click',
+        'requests',
+        'pyyaml',
+        'polars',
+        'pandas',
+        'numpy',
+        'pyarrow',
         # eg: 'aspectlib==1.1.1', 'six>=1.7',
     ],
     extras_require={
         # eg:
         #   'rst': ['docutils>=0.11'],
         #   ':python_version=="2.6"': ['argparse'],
     },
```

### Comparing `helius-sdk-0.0.10/src/helius_sdk/__main__.py` & `helius-sdk-0.0.11/src/helius_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/src/helius_sdk/cli.py` & `helius-sdk-0.0.11/src/helius_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/src/helius_sdk/core.py` & `helius-sdk-0.0.11/src/helius_sdk/core.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/src/helius_sdk/event.py` & `helius-sdk-0.0.11/src/helius_sdk/event.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/src/helius_sdk/nft.py` & `helius-sdk-0.0.11/src/helius_sdk/nft.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/src/helius_sdk/transaction.py` & `helius-sdk-0.0.11/src/helius_sdk/transaction.py`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/src/helius_sdk.egg-info/PKG-INFO` & `helius-sdk-0.0.11/src/helius_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: helius-sdk
-Version: 0.0.10
+Version: 0.0.11
 Summary: Helius SDK
 Home-page: https://github.com/mmchougule/helius-sdk-python
 Author: Mayur Chougule
 Author-email: mayurchougule1@gmail.com
 License: MIT
 Project-URL: Documentation, https://helius-sdk-python.readthedocs.io/
 Project-URL: Changelog, https://helius-sdk-python.readthedocs.io/en/latest/changelog.html
```

### Comparing `helius-sdk-0.0.10/src/helius_sdk.egg-info/SOURCES.txt` & `helius-sdk-0.0.11/src/helius_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helius-sdk-0.0.10/tox.ini` & `helius-sdk-0.0.11/tox.ini`

 * *Files identical despite different names*

