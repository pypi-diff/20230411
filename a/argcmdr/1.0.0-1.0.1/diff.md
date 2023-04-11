# Comparing `tmp/argcmdr-1.0.0.tar.gz` & `tmp/argcmdr-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/argcmdr-1.0.0.tar", last modified: Wed Feb 15 04:36:48 2023, max compression
+gzip compressed data, was "dist/argcmdr-1.0.1.tar", last modified: Tue Apr 11 19:35:04 2023, max compression
```

## Comparing `argcmdr-1.0.0.tar` & `argcmdr-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-02-15 04:36:48.000000 argcmdr-1.0.0/
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)      162 2023-02-15 04:36:48.000000 argcmdr-1.0.0/setup.cfg
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     1085 2022-06-08 18:44:16.000000 argcmdr-1.0.0/LICENSE
-drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-02-15 04:36:48.000000 argcmdr-1.0.0/test/
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    35406 2023-02-14 21:11:22.000000 argcmdr-1.0.0/test/test_argcmdr.py
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     1504 2023-02-08 19:44:26.000000 argcmdr-1.0.0/setup.py
-drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-02-15 04:36:48.000000 argcmdr-1.0.0/src/
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    30046 2023-02-15 04:36:48.000000 argcmdr-1.0.0/src/argcmdr.py
-drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-02-15 04:36:48.000000 argcmdr-1.0.0/src/argcmdr.egg-info/
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)        8 2023-02-15 04:36:48.000000 argcmdr-1.0.0/src/argcmdr.egg-info/top_level.txt
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)       52 2023-02-15 04:36:48.000000 argcmdr-1.0.0/src/argcmdr.egg-info/requires.txt
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)        1 2023-02-15 04:36:48.000000 argcmdr-1.0.0/src/argcmdr.egg-info/dependency_links.txt
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)      285 2023-02-15 04:36:48.000000 argcmdr-1.0.0/src/argcmdr.egg-info/SOURCES.txt
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)       44 2023-02-15 04:36:48.000000 argcmdr-1.0.0/src/argcmdr.egg-info/entry_points.txt
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    54317 2023-02-15 04:36:48.000000 argcmdr-1.0.0/src/argcmdr.egg-info/PKG-INFO
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    54317 2023-02-15 04:36:48.000000 argcmdr-1.0.0/PKG-INFO
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    45272 2023-02-15 04:28:28.000000 argcmdr-1.0.0/README.rst
+drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-11 19:35:04.000000 argcmdr-1.0.1/
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)      162 2023-04-11 19:35:04.000000 argcmdr-1.0.1/setup.cfg
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     1085 2022-06-08 18:44:16.000000 argcmdr-1.0.1/LICENSE
+drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-11 19:35:04.000000 argcmdr-1.0.1/test/
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    35406 2023-02-14 21:11:22.000000 argcmdr-1.0.1/test/test_argcmdr.py
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     1502 2023-04-11 19:34:12.000000 argcmdr-1.0.1/setup.py
+drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-11 19:35:04.000000 argcmdr-1.0.1/src/
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    30046 2023-04-11 19:33:32.000000 argcmdr-1.0.1/src/argcmdr.py
+drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-11 19:35:04.000000 argcmdr-1.0.1/src/argcmdr.egg-info/
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)        8 2023-04-11 19:35:04.000000 argcmdr-1.0.1/src/argcmdr.egg-info/top_level.txt
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)       50 2023-04-11 19:35:04.000000 argcmdr-1.0.1/src/argcmdr.egg-info/requires.txt
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)        1 2023-04-11 19:35:04.000000 argcmdr-1.0.1/src/argcmdr.egg-info/dependency_links.txt
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)      285 2023-04-11 19:35:04.000000 argcmdr-1.0.1/src/argcmdr.egg-info/SOURCES.txt
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)       44 2023-04-11 19:35:04.000000 argcmdr-1.0.1/src/argcmdr.egg-info/entry_points.txt
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    54317 2023-04-11 19:35:04.000000 argcmdr-1.0.1/src/argcmdr.egg-info/PKG-INFO
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    54317 2023-04-11 19:35:04.000000 argcmdr-1.0.1/PKG-INFO
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)    45272 2023-02-15 04:28:28.000000 argcmdr-1.0.1/README.rst
```

### Comparing `argcmdr-1.0.0/LICENSE` & `argcmdr-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argcmdr-1.0.0/test/test_argcmdr.py` & `argcmdr-1.0.1/test/test_argcmdr.py`

 * *Files identical despite different names*

### Comparing `argcmdr-1.0.0/setup.py` & `argcmdr-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     ],
     url="https://github.com/dssg/argcmdr",
     python_requires='>=3.6',
     package_dir={'': SRC_DIR},
     py_modules=[MODULE],
     install_requires=[
         'argcomplete>=1.9.4,<3',
-        'Dickens~=2.0.0',
+        'Dickens~=2.0',
         'plumbum~=1.8.1',
     ],
     entry_points={
         'console_scripts': [
             'manage = argcmdr:execute',
         ],
     },
```

### Comparing `argcmdr-1.0.0/src/argcmdr.py` & `argcmdr-1.0.1/src/argcmdr.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from descriptors import (
     cachedproperty as _cachedproperty,
     classproperty as _classproperty,
 )
 
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 __all__ = (
     'cmd',
     'cmdmethod',
     'local',
     'localmethod',
     'main',
```

### Comparing `argcmdr-1.0.0/src/argcmdr.egg-info/PKG-INFO` & `argcmdr-1.0.1/src/argcmdr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: argcmdr
-Version: 1.0.0
+Version: 1.0.1
 Summary: Thin argparse wrapper for quick, clear and easy declaration of hierarchical console command interfaces
 Home-page: https://github.com/dssg/argcmdr
 Author: Center for Data Science and Public Policy
 Author-email: datascifellows@gmail.com
 License: MIT
 Description: =======
         argcmdr
```

### Comparing `argcmdr-1.0.0/PKG-INFO` & `argcmdr-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: argcmdr
-Version: 1.0.0
+Version: 1.0.1
 Summary: Thin argparse wrapper for quick, clear and easy declaration of hierarchical console command interfaces
 Home-page: https://github.com/dssg/argcmdr
 Author: Center for Data Science and Public Policy
 Author-email: datascifellows@gmail.com
 License: MIT
 Description: =======
         argcmdr
```

### Comparing `argcmdr-1.0.0/README.rst` & `argcmdr-1.0.1/README.rst`

 * *Files identical despite different names*

