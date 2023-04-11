# Comparing `tmp/richvalues-3.0.0.tar.gz` & `tmp/richvalues-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richvalues-3.0.0.tar", last modified: Mon Apr 10 11:41:50 2023, max compression
+gzip compressed data, was "richvalues-3.0.1.tar", last modified: Tue Apr 11 10:43:55 2023, max compression
```

## Comparing `richvalues-3.0.0.tar` & `richvalues-3.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-10 11:41:50.361043 richvalues-3.0.0/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-10 11:41:50.361043 richvalues-3.0.0/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      809 2023-04-10 11:41:38.000000 richvalues-3.0.0/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)      515 2023-04-10 11:39:23.000000 richvalues-3.0.0/pyproject.toml
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-10 11:41:50.361043 richvalues-3.0.0/richvalues/
--rw-rw-r--   0 andres    (1000) andres    (1000)   143953 2023-04-10 11:34:25.000000 richvalues-3.0.0/richvalues/__init__.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-10 11:41:50.361043 richvalues-3.0.0/richvalues.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-10 11:41:50.000000 richvalues-3.0.0/richvalues.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-04-10 11:41:50.000000 richvalues-3.0.0/richvalues.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-04-10 11:41:50.000000 richvalues-3.0.0/richvalues.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-04-10 11:41:50.000000 richvalues-3.0.0/richvalues.egg-info/requires.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-04-10 11:41:50.000000 richvalues-3.0.0/richvalues.egg-info/top_level.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-04-10 11:41:50.361043 richvalues-3.0.0/setup.cfg
--rw-rw-r--   0 andres    (1000) andres    (1000)      753 2023-04-10 11:39:11.000000 richvalues-3.0.0/setup.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 10:43:55.868113 richvalues-3.0.1/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 10:43:55.868113 richvalues-3.0.1/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      809 2023-04-10 11:41:38.000000 richvalues-3.0.1/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)      515 2023-04-11 10:43:33.000000 richvalues-3.0.1/pyproject.toml
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 10:43:55.868113 richvalues-3.0.1/richvalues/
+-rw-rw-r--   0 andres    (1000) andres    (1000)   143953 2023-04-10 11:34:25.000000 richvalues-3.0.1/richvalues/__init__.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 10:43:55.868113 richvalues-3.0.1/richvalues.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 10:43:55.000000 richvalues-3.0.1/richvalues.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-04-11 10:43:55.000000 richvalues-3.0.1/richvalues.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-04-11 10:43:55.000000 richvalues-3.0.1/richvalues.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-04-11 10:43:55.000000 richvalues-3.0.1/richvalues.egg-info/requires.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-04-11 10:43:55.000000 richvalues-3.0.1/richvalues.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-04-11 10:43:55.868113 richvalues-3.0.1/setup.cfg
+-rw-rw-r--   0 andres    (1000) andres    (1000)      752 2023-04-11 10:43:24.000000 richvalues-3.0.1/setup.py
```

### Comparing `richvalues-3.0.0/PKG-INFO` & `richvalues-3.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Description: # RichValues
         
         Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
```

### Comparing `richvalues-3.0.0/README.md` & `richvalues-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `richvalues-3.0.0/pyproject.toml` & `richvalues-3.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "richvalues"
-version = "3.0.0"
+version = "3.0.1"
 description = "Python library for working with uncertainties and upper/lower limits"
 license = {file="LICENSE"}
 authors = [{name="Andrés Megías Toledano"}]
 readme = "README.md"
 dependencies = ["numpy", "pandas", "scipy", "matplotlib"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `richvalues-3.0.0/richvalues/__init__.py` & `richvalues-3.0.1/richvalues/__init__.py`

 * *Files identical despite different names*

### Comparing `richvalues-3.0.0/richvalues.egg-info/PKG-INFO` & `richvalues-3.0.1/richvalues.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Description: # RichValues
         
         Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
```

### Comparing `richvalues-3.0.0/setup.py` & `richvalues-3.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name = 'richvalues',
-    version = '3.0.0',
+    version = '3.0.1',
     license = 'BSD-3-Clause',
     author = 'Andrés Megías Toledano',
     description = 'Python library for working with uncertainties and upper/lower limits',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
-    packages = setuptools.find_packages('./'),
+    packages = setuptools.find_packages('.'),
     url = 'https://github.com/andresmegias/richvalues',
     install_requires = ['numpy', 'pandas', 'scipy', 'matplotlib'],
     classifiers = [
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent'
     ]
```

