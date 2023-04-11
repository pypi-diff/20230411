# Comparing `tmp/baselog-1.0.0.tar.gz` & `tmp/baselog-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baselog-1.0.0.tar", last modified: Tue Apr 11 09:57:23 2023, max compression
+gzip compressed data, was "baselog-2.0.0.tar", last modified: Tue Apr 11 20:19:24 2023, max compression
```

## Comparing `baselog-1.0.0.tar` & `baselog-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:57:23.853850 baselog-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-11 09:57:00.000000 baselog-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-11 09:57:23.853850 baselog-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-11 09:57:00.000000 baselog-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-11 09:57:00.000000 baselog-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 09:57:23.853850 baselog-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:57:23.849850 baselog-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:57:23.849850 baselog-1.0.0/src/baselog/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 09:57:00.000000 baselog-1.0.0/src/baselog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-11 09:57:00.000000 baselog-1.0.0/src/baselog/baselog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:57:23.853850 baselog-1.0.0/src/baselog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-11 09:57:23.000000 baselog-1.0.0/src/baselog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-11 09:57:23.000000 baselog-1.0.0/src/baselog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:57:23.000000 baselog-1.0.0/src/baselog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 09:57:23.000000 baselog-1.0.0/src/baselog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:19:24.427564 baselog-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-11 20:19:00.000000 baselog-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-11 20:19:24.427564 baselog-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-11 20:19:00.000000 baselog-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-11 20:19:00.000000 baselog-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 20:19:24.427564 baselog-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:19:24.423564 baselog-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:19:24.423564 baselog-2.0.0/src/baselog/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-11 20:19:00.000000 baselog-2.0.0/src/baselog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-04-11 20:19:00.000000 baselog-2.0.0/src/baselog/baselog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:19:24.423564 baselog-2.0.0/src/baselog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-11 20:19:24.000000 baselog-2.0.0/src/baselog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-11 20:19:24.000000 baselog-2.0.0/src/baselog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:19:24.000000 baselog-2.0.0/src/baselog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 20:19:24.000000 baselog-2.0.0/src/baselog.egg-info/top_level.txt
```

### Comparing `baselog-1.0.0/LICENSE` & `baselog-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `baselog-1.0.0/pyproject.toml` & `baselog-2.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "baselog"
-version = "1.0.0"
+version = "2.0.0"
 authors = [
   { name="Ben Burke", email="actualben@users.noreply.github.com" },
 ]
 description = "typed 12-factor app configuration helper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

