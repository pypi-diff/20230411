# Comparing `tmp/simplerabbit-0.0.2.tar.gz` & `tmp/simplerabbit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplerabbit-0.0.2.tar", last modified: Tue Apr 11 12:04:30 2023, max compression
+gzip compressed data, was "simplerabbit-0.0.3.tar", last modified: Tue Apr 11 12:15:06 2023, max compression
```

## Comparing `simplerabbit-0.0.2.tar` & `simplerabbit-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,13 @@
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:04:30.112334 simplerabbit-0.0.2/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1798 2023-04-11 12:04:30.112334 simplerabbit-0.0.2/PKG-INFO
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1100 2023-04-11 11:23:43.000000 simplerabbit-0.0.2/README.md
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      638 2023-04-11 12:04:19.000000 simplerabbit-0.0.2/pyproject.toml
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       79 2023-04-11 12:04:30.112334 simplerabbit-0.0.2/setup.cfg
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1616 2023-04-11 11:37:26.000000 simplerabbit-0.0.2/setup.py
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:04:30.112334 simplerabbit-0.0.2/simplerabbit/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 11:39:32.000000 simplerabbit-0.0.2/simplerabbit/__init__.py
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     3297 2023-04-11 11:23:43.000000 simplerabbit-0.0.2/simplerabbit/receiver.py
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     2836 2023-04-11 11:23:43.000000 simplerabbit-0.0.2/simplerabbit/sender.py
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:04:30.112334 simplerabbit-0.0.2/simplerabbit.egg-info/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1798 2023-04-11 12:04:30.000000 simplerabbit-0.0.2/simplerabbit.egg-info/PKG-INFO
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      309 2023-04-11 12:04:30.000000 simplerabbit-0.0.2/simplerabbit.egg-info/SOURCES.txt
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 12:04:30.000000 simplerabbit-0.0.2/simplerabbit.egg-info/dependency_links.txt
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       12 2023-04-11 12:04:30.000000 simplerabbit-0.0.2/simplerabbit.egg-info/requires.txt
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       13 2023-04-11 12:04:30.000000 simplerabbit-0.0.2/simplerabbit.egg-info/top_level.txt
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:04:30.112334 simplerabbit-0.0.2/tests/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       86 2023-04-11 11:23:43.000000 simplerabbit-0.0.2/tests/test.py
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:15:06.718434 simplerabbit-0.0.3/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-11 12:15:06.718434 simplerabbit-0.0.3/PKG-INFO
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1100 2023-04-11 11:23:43.000000 simplerabbit-0.0.3/README.md
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      638 2023-04-11 12:14:19.000000 simplerabbit-0.0.3/pyproject.toml
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       38 2023-04-11 12:15:06.718434 simplerabbit-0.0.3/setup.cfg
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:15:06.714434 simplerabbit-0.0.3/src/
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:15:06.718434 simplerabbit-0.0.3/src/simplerabbit.egg-info/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-11 12:15:06.000000 simplerabbit-0.0.3/src/simplerabbit.egg-info/PKG-INFO
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      198 2023-04-11 12:15:06.000000 simplerabbit-0.0.3/src/simplerabbit.egg-info/SOURCES.txt
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 12:15:06.000000 simplerabbit-0.0.3/src/simplerabbit.egg-info/dependency_links.txt
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 12:15:06.000000 simplerabbit-0.0.3/src/simplerabbit.egg-info/top_level.txt
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:15:06.718434 simplerabbit-0.0.3/tests/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      101 2023-04-11 12:09:34.000000 simplerabbit-0.0.3/tests/test.py
```

### Comparing `simplerabbit-0.0.2/PKG-INFO` & `simplerabbit-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 Metadata-Version: 2.1
 Name: simplerabbit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple RabbitMQ library
-Home-page: https://github.com/Energidanmark/simplerabbit
-Download-URL: https://github.com/Energidanmark/simplerabbit/archive/refs/tags/v_01.tar.gz
-Author: Phuong Do
 Author-email: Phuong Do <phdo@energidanmark.dk>
-License: MIT
 Project-URL: Homepage, https://github.com/Energidanmark/simplerabbit
 Project-URL: Bug Tracker, https://github.com/Energidanmark/simplerabbit/issues
-Keywords: RABBIT-MQ,PIKA
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Atom Rabbit Lib
```

### Comparing `simplerabbit-0.0.2/README.md` & `simplerabbit-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `simplerabbit-0.0.2/pyproject.toml` & `simplerabbit-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simplerabbit"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Phuong Do", email="phdo@energidanmark.dk" },
 ]
 description = "Simple RabbitMQ library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplerabbit-0.0.2/simplerabbit.egg-info/PKG-INFO` & `simplerabbit-0.0.3/src/simplerabbit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 Metadata-Version: 2.1
 Name: simplerabbit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple RabbitMQ library
-Home-page: https://github.com/Energidanmark/simplerabbit
-Download-URL: https://github.com/Energidanmark/simplerabbit/archive/refs/tags/v_01.tar.gz
-Author: Phuong Do
 Author-email: Phuong Do <phdo@energidanmark.dk>
-License: MIT
 Project-URL: Homepage, https://github.com/Energidanmark/simplerabbit
 Project-URL: Bug Tracker, https://github.com/Energidanmark/simplerabbit/issues
-Keywords: RABBIT-MQ,PIKA
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Atom Rabbit Lib
```

