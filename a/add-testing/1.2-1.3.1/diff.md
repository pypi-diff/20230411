# Comparing `tmp/add-testing-1.2.tar.gz` & `tmp/add-testing-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "add-testing-1.2.tar", last modified: Tue Nov 22 12:08:46 2022, max compression
+gzip compressed data, was "add-testing-1.3.1.tar", last modified: Tue Apr 11 11:20:52 2023, max compression
```

## Comparing `add-testing-1.2.tar` & `add-testing-1.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 12:08:46.325874 add-testing-1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-11-22 12:08:38.000000 add-testing-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-11-22 12:08:46.325874 add-testing-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-22 12:08:38.000000 add-testing-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 12:08:46.325874 add-testing-1.2/add_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-11-22 12:08:46.000000 add-testing-1.2/add_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-11-22 12:08:46.000000 add-testing-1.2/add_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-22 12:08:46.000000 add-testing-1.2/add_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-22 12:08:46.000000 add-testing-1.2/add_testing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-11-22 12:08:46.000000 add-testing-1.2/add_testing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-22 12:08:46.000000 add-testing-1.2/add_testing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-11-22 12:08:38.000000 add-testing-1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-11-22 12:08:46.329874 add-testing-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-22 12:08:38.000000 add-testing-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:52.157169 add-testing-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-11 11:20:43.000000 add-testing-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-11 11:20:52.157169 add-testing-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 11:20:43.000000 add-testing-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:20:52.157169 add-testing-1.3.1/add_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-11 11:20:52.000000 add-testing-1.3.1/add_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-11 11:20:52.000000 add-testing-1.3.1/add_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:20:52.000000 add-testing-1.3.1/add_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:20:51.000000 add-testing-1.3.1/add_testing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 11:20:52.000000 add-testing-1.3.1/add_testing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:20:52.000000 add-testing-1.3.1/add_testing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-11 11:20:43.000000 add-testing-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-11 11:20:52.157169 add-testing-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 11:20:43.000000 add-testing-1.3.1/setup.py
```

### Comparing `add-testing-1.2/LICENSE` & `add-testing-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `add-testing-1.2/pyproject.toml` & `add-testing-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `add-testing-1.2/setup.cfg` & `add-testing-1.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = add-testing
-version = 1.2
+version = 1.3.1
 description = A sample testing app
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Shailesh Kumar
 author_email = kumar.shailesh1597@gmail.com
 license = Apache-2.0
 license_files = LICENSE
```

