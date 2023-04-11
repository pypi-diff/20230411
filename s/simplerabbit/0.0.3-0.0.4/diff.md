# Comparing `tmp/simplerabbit-0.0.3.tar.gz` & `tmp/simplerabbit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplerabbit-0.0.3.tar", last modified: Tue Apr 11 12:15:06 2023, max compression
+gzip compressed data, was "simplerabbit-0.0.4.tar", last modified: Tue Apr 11 12:27:45 2023, max compression
```

## Comparing `simplerabbit-0.0.3.tar` & `simplerabbit-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:15:06.718434 simplerabbit-0.0.3/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-11 12:15:06.718434 simplerabbit-0.0.3/PKG-INFO
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1100 2023-04-11 11:23:43.000000 simplerabbit-0.0.3/README.md
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      638 2023-04-11 12:14:19.000000 simplerabbit-0.0.3/pyproject.toml
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       38 2023-04-11 12:15:06.718434 simplerabbit-0.0.3/setup.cfg
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:15:06.714434 simplerabbit-0.0.3/src/
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:15:06.718434 simplerabbit-0.0.3/src/simplerabbit.egg-info/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-11 12:15:06.000000 simplerabbit-0.0.3/src/simplerabbit.egg-info/PKG-INFO
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      198 2023-04-11 12:15:06.000000 simplerabbit-0.0.3/src/simplerabbit.egg-info/SOURCES.txt
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 12:15:06.000000 simplerabbit-0.0.3/src/simplerabbit.egg-info/dependency_links.txt
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 12:15:06.000000 simplerabbit-0.0.3/src/simplerabbit.egg-info/top_level.txt
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:15:06.718434 simplerabbit-0.0.3/tests/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      101 2023-04-11 12:09:34.000000 simplerabbit-0.0.3/tests/test.py
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:27:45.317679 simplerabbit-0.0.4/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-11 12:27:45.317679 simplerabbit-0.0.4/PKG-INFO
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1100 2023-04-11 11:23:43.000000 simplerabbit-0.0.4/README.md
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      638 2023-04-11 12:27:26.000000 simplerabbit-0.0.4/pyproject.toml
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       38 2023-04-11 12:27:45.317679 simplerabbit-0.0.4/setup.cfg
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:27:45.313679 simplerabbit-0.0.4/src/
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:27:45.313679 simplerabbit-0.0.4/src/simplerabbit/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 11:39:32.000000 simplerabbit-0.0.4/src/simplerabbit/__init__.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     3067 2023-04-11 12:11:18.000000 simplerabbit-0.0.4/src/simplerabbit/receiver.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     2768 2023-04-11 12:10:34.000000 simplerabbit-0.0.4/src/simplerabbit/sender.py
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:27:45.317679 simplerabbit-0.0.4/src/simplerabbit.egg-info/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-11 12:27:45.000000 simplerabbit-0.0.4/src/simplerabbit.egg-info/PKG-INFO
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      283 2023-04-11 12:27:45.000000 simplerabbit-0.0.4/src/simplerabbit.egg-info/SOURCES.txt
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 12:27:45.000000 simplerabbit-0.0.4/src/simplerabbit.egg-info/dependency_links.txt
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       13 2023-04-11 12:27:45.000000 simplerabbit-0.0.4/src/simplerabbit.egg-info/top_level.txt
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:27:45.317679 simplerabbit-0.0.4/tests/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      107 2023-04-11 12:24:50.000000 simplerabbit-0.0.4/tests/test.py
```

### Comparing `simplerabbit-0.0.3/PKG-INFO` & `simplerabbit-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplerabbit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple RabbitMQ library
 Author-email: Phuong Do <phdo@energidanmark.dk>
 Project-URL: Homepage, https://github.com/Energidanmark/simplerabbit
 Project-URL: Bug Tracker, https://github.com/Energidanmark/simplerabbit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simplerabbit-0.0.3/README.md` & `simplerabbit-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `simplerabbit-0.0.3/pyproject.toml` & `simplerabbit-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simplerabbit"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Phuong Do", email="phdo@energidanmark.dk" },
 ]
 description = "Simple RabbitMQ library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplerabbit-0.0.3/src/simplerabbit.egg-info/PKG-INFO` & `simplerabbit-0.0.4/src/simplerabbit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplerabbit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple RabbitMQ library
 Author-email: Phuong Do <phdo@energidanmark.dk>
 Project-URL: Homepage, https://github.com/Energidanmark/simplerabbit
 Project-URL: Bug Tracker, https://github.com/Energidanmark/simplerabbit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

