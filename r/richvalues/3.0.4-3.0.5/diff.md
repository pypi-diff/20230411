# Comparing `tmp/richvalues-3.0.4.tar.gz` & `tmp/richvalues-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richvalues-3.0.4.tar", last modified: Tue Apr 11 14:03:36 2023, max compression
+gzip compressed data, was "richvalues-3.0.5.tar", last modified: Tue Apr 11 14:28:54 2023, max compression
```

## Comparing `richvalues-3.0.4.tar` & `richvalues-3.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:03:36.775993 richvalues-3.0.4/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 14:03:36.775993 richvalues-3.0.4/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      809 2023-04-10 11:41:38.000000 richvalues-3.0.4/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)      515 2023-04-11 13:59:18.000000 richvalues-3.0.4/pyproject.toml
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:03:36.775993 richvalues-3.0.4/richvalues/
--rw-rw-r--   0 andres    (1000) andres    (1000)   146009 2023-04-11 13:58:40.000000 richvalues-3.0.4/richvalues/__init__.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:03:36.775993 richvalues-3.0.4/richvalues.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 14:03:36.000000 richvalues-3.0.4/richvalues.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-04-11 14:03:36.000000 richvalues-3.0.4/richvalues.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-04-11 14:03:36.000000 richvalues-3.0.4/richvalues.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-04-11 14:03:36.000000 richvalues-3.0.4/richvalues.egg-info/requires.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-04-11 14:03:36.000000 richvalues-3.0.4/richvalues.egg-info/top_level.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-04-11 14:03:36.775993 richvalues-3.0.4/setup.cfg
--rw-rw-r--   0 andres    (1000) andres    (1000)      752 2023-04-11 13:59:10.000000 richvalues-3.0.4/setup.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:28:54.643054 richvalues-3.0.5/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 14:28:54.643054 richvalues-3.0.5/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      809 2023-04-10 11:41:38.000000 richvalues-3.0.5/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)      515 2023-04-11 14:27:49.000000 richvalues-3.0.5/pyproject.toml
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:28:54.639053 richvalues-3.0.5/richvalues/
+-rw-rw-r--   0 andres    (1000) andres    (1000)   146009 2023-04-11 13:58:40.000000 richvalues-3.0.5/richvalues/__init__.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:28:54.639053 richvalues-3.0.5/richvalues.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 14:28:54.000000 richvalues-3.0.5/richvalues.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-04-11 14:28:54.000000 richvalues-3.0.5/richvalues.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-04-11 14:28:54.000000 richvalues-3.0.5/richvalues.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-04-11 14:28:54.000000 richvalues-3.0.5/richvalues.egg-info/requires.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-04-11 14:28:54.000000 richvalues-3.0.5/richvalues.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-04-11 14:28:54.643054 richvalues-3.0.5/setup.cfg
+-rw-rw-r--   0 andres    (1000) andres    (1000)      752 2023-04-11 14:27:41.000000 richvalues-3.0.5/setup.py
```

### Comparing `richvalues-3.0.4/PKG-INFO` & `richvalues-3.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.0.4
+Version: 3.0.5
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Description: # RichValues
         
         Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
```

### Comparing `richvalues-3.0.4/README.md` & `richvalues-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `richvalues-3.0.4/pyproject.toml` & `richvalues-3.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "richvalues"
-version = "3.0.4"
+version = "3.0.5"
 description = "Python library for working with uncertainties and upper/lower limits"
 license = {file="LICENSE"}
 authors = [{name="Andrés Megías Toledano"}]
 readme = "README.md"
 dependencies = ["numpy", "pandas", "scipy", "matplotlib"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `richvalues-3.0.4/richvalues/__init__.py` & `richvalues-3.0.5/richvalues/__init__.py`

 * *Files identical despite different names*

### Comparing `richvalues-3.0.4/richvalues.egg-info/PKG-INFO` & `richvalues-3.0.5/richvalues.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.0.4
+Version: 3.0.5
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Description: # RichValues
         
         Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
```

### Comparing `richvalues-3.0.4/setup.py` & `richvalues-3.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name = 'richvalues',
-    version = '3.0.4',
+    version = '3.0.5',
     license = 'BSD-3-Clause',
     author = 'Andrés Megías Toledano',
     description = 'Python library for working with uncertainties and upper/lower limits',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages = setuptools.find_packages('.'),
     url = 'https://github.com/andresmegias/richvalues',
```

