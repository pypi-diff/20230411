# Comparing `tmp/add-testing-1.3.tar.gz` & `tmp/add-testing-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "add-testing-1.3.tar", last modified: Tue Apr 11 12:07:58 2023, max compression
+gzip compressed data, was "add-testing-1.3.1.tar", last modified: Tue Apr 11 11:20:52 2023, max compression
```

## Comparing `add-testing-1.3.tar` & `add-testing-1.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:07:58.165232 add-testing-1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-11 12:07:50.000000 add-testing-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-11 12:07:58.165232 add-testing-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 12:07:50.000000 add-testing-1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:07:58.165232 add-testing-1.3/add_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-11 12:07:58.000000 add-testing-1.3/add_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-11 12:07:58.000000 add-testing-1.3/add_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:07:58.000000 add-testing-1.3/add_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:07:58.000000 add-testing-1.3/add_testing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 12:07:58.000000 add-testing-1.3/add_testing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:07:58.000000 add-testing-1.3/add_testing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-11 12:07:50.000000 add-testing-1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-11 12:07:58.165232 add-testing-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 12:07:50.000000 add-testing-1.3/setup.py
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

### Comparing `add-testing-1.3/LICENSE` & `add-testing-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `add-testing-1.3/PKG-INFO` & `add-testing-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: add-testing
-Version: 1.3
+Version: 1.3.1
 Summary: A sample testing app
 Author: Shailesh Kumar
 Author-email: kumar.shailesh1597@gmail.com
 License: Apache-2.0
 Platform: unix
 Platform: linux
 Platform: osx
```

### Comparing `add-testing-1.3/add_testing.egg-info/PKG-INFO` & `add-testing-1.3.1/add_testing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: add-testing
-Version: 1.3
+Version: 1.3.1
 Summary: A sample testing app
 Author: Shailesh Kumar
 Author-email: kumar.shailesh1597@gmail.com
 License: Apache-2.0
 Platform: unix
 Platform: linux
 Platform: osx
```

### Comparing `add-testing-1.3/pyproject.toml` & `add-testing-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `add-testing-1.3/setup.cfg` & `add-testing-1.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = add-testing
-version = 1.3
+version = 1.3.1
 description = A sample testing app
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Shailesh Kumar
 author_email = kumar.shailesh1597@gmail.com
 license = Apache-2.0
 license_files = LICENSE
```

