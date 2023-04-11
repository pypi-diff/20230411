# Comparing `tmp/my_python_package007-0.5.6.tar.gz` & `tmp/my_python_package007-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_python_package007-0.5.6.tar", last modified: Tue Apr 11 10:08:59 2023, max compression
+gzip compressed data, was "my_python_package007-0.5.7.tar", last modified: Tue Apr 11 10:19:23 2023, max compression
```

## Comparing `my_python_package007-0.5.6.tar` & `my_python_package007-0.5.7.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:08:59.898688 my_python_package007-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-11 10:08:59.898688 my_python_package007-0.5.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:08:59.894688 my_python_package007-0.5.6/my_python_package007.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-11 10:08:59.000000 my_python_package007-0.5.6/my_python_package007.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-11 10:08:59.000000 my_python_package007-0.5.6/my_python_package007.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:08:59.000000 my_python_package007-0.5.6/my_python_package007.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 10:08:59.000000 my_python_package007-0.5.6/my_python_package007.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:08:59.000000 my_python_package007-0.5.6/my_python_package007.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:08:59.898688 my_python_package007-0.5.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-04-11 10:08:45.000000 my_python_package007-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:08:59.894688 my_python_package007-0.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 10:08:45.000000 my_python_package007-0.5.6/tests/test_my_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:19:23.139619 my_python_package007-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-11 10:19:23.139619 my_python_package007-0.5.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:19:23.139619 my_python_package007-0.5.7/my_python_package007.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-11 10:19:23.000000 my_python_package007-0.5.7/my_python_package007.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-11 10:19:23.000000 my_python_package007-0.5.7/my_python_package007.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:19:23.000000 my_python_package007-0.5.7/my_python_package007.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 10:19:23.000000 my_python_package007-0.5.7/my_python_package007.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 10:19:23.000000 my_python_package007-0.5.7/my_python_package007.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:19:23.000000 my_python_package007-0.5.7/my_python_package007.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:19:23.139619 my_python_package007-0.5.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      659 2023-04-11 10:19:13.000000 my_python_package007-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:19:23.139619 my_python_package007-0.5.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-11 10:19:13.000000 my_python_package007-0.5.7/tests/test_my_module.py
```

### Comparing `my_python_package007-0.5.6/setup.py` & `my_python_package007-0.5.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='my_python_package007',
-    version='0.5.6',
+    version='0.5.7',
     description='My awesome Python package v2',
     author='DipakMehta',
     author_email='dipak@zvolv.com',
     url='https://github.com/DipakMehta/python',
     long_description='we are trying new version',
     packages=find_packages(),
     # entry_points={ 'console_scripts': [ 'my_python_package007=my_python_package:test_hello_world' ] }
     install_requires=[
         'numpy',
         'pandas',# list of dependencies
     ],
+    entry_points={
+        'console_scripts': [
+            'mycommand = my_package.my_module:my_function'
+        ]
+    }
 )
```

