# Comparing `tmp/MySQLPandas-0.0.8.tar.gz` & `tmp/MySQLPandas-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MySQLPandas-0.0.8.tar", last modified: Tue Apr 11 04:47:20 2023, max compression
+gzip compressed data, was "MySQLPandas-0.0.9.tar", last modified: Tue Apr 11 06:12:58 2023, max compression
```

## Comparing `MySQLPandas-0.0.8.tar` & `MySQLPandas-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-11 04:47:20.033980 MySQLPandas-0.0.8/
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     1071 2023-04-07 04:14:42.000000 MySQLPandas-0.0.8/LICENCE
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       16 2023-04-11 04:33:53.000000 MySQLPandas-0.0.8/MANIFEST.in
-drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-11 04:47:20.019980 MySQLPandas-0.0.8/MySQLPandas/
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)      291 2023-04-11 04:46:54.000000 MySQLPandas-0.0.8/MySQLPandas/__init__.py
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)    13341 2023-04-10 05:49:22.000000 MySQLPandas-0.0.8/MySQLPandas/core.py
-drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-11 04:47:20.029980 MySQLPandas-0.0.8/MySQLPandas/lib/
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     6471 2023-04-07 05:18:00.000000 MySQLPandas-0.0.8/MySQLPandas/lib/DataFrameClass.py
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       92 2023-03-27 05:45:36.000000 MySQLPandas-0.0.8/MySQLPandas/lib/ErrorClass.py
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)        0 2023-03-27 05:12:58.000000 MySQLPandas-0.0.8/MySQLPandas/lib/__init__.py
-drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-11 04:47:20.025980 MySQLPandas-0.0.8/MySQLPandas.egg-info/
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     2391 2023-04-11 04:47:19.000000 MySQLPandas-0.0.8/MySQLPandas.egg-info/PKG-INFO
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)      401 2023-04-11 04:47:19.000000 MySQLPandas-0.0.8/MySQLPandas.egg-info/SOURCES.txt
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)        1 2023-04-11 04:47:19.000000 MySQLPandas-0.0.8/MySQLPandas.egg-info/dependency_links.txt
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       45 2023-04-11 04:47:19.000000 MySQLPandas-0.0.8/MySQLPandas.egg-info/requires.txt
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       28 2023-04-11 04:47:19.000000 MySQLPandas-0.0.8/MySQLPandas.egg-info/top_level.txt
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     2391 2023-04-11 04:47:20.032980 MySQLPandas-0.0.8/PKG-INFO
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     1777 2023-04-11 04:43:41.000000 MySQLPandas-0.0.8/README.md
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       38 2023-04-11 04:47:20.033980 MySQLPandas-0.0.8/setup.cfg
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     1867 2023-04-11 03:08:38.000000 MySQLPandas-0.0.8/setup.py
-drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-11 04:47:20.031980 MySQLPandas-0.0.8/tests/
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     4526 2023-04-07 04:49:44.000000 MySQLPandas-0.0.8/tests/test_DataFrameClass.py
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     2132 2023-04-07 06:25:10.000000 MySQLPandas-0.0.8/tests/test_coreClass.py
+drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-11 06:12:58.785556 MySQLPandas-0.0.9/
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)    18092 2023-04-11 06:04:32.000000 MySQLPandas-0.0.9/LICENSE
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       16 2023-04-11 04:33:53.000000 MySQLPandas-0.0.9/MANIFEST.in
+drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-11 06:12:58.764557 MySQLPandas-0.0.9/MySQLPandas/
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)      293 2023-04-11 06:12:24.000000 MySQLPandas-0.0.9/MySQLPandas/__init__.py
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)    13341 2023-04-10 05:49:22.000000 MySQLPandas-0.0.9/MySQLPandas/core.py
+drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-11 06:12:58.779557 MySQLPandas-0.0.9/MySQLPandas/lib/
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     6471 2023-04-07 05:18:00.000000 MySQLPandas-0.0.9/MySQLPandas/lib/DataFrameClass.py
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       92 2023-03-27 05:45:36.000000 MySQLPandas-0.0.9/MySQLPandas/lib/ErrorClass.py
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)        0 2023-03-27 05:12:58.000000 MySQLPandas-0.0.9/MySQLPandas/lib/__init__.py
+drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-11 06:12:58.774556 MySQLPandas-0.0.9/MySQLPandas.egg-info/
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     2417 2023-04-11 06:12:58.000000 MySQLPandas-0.0.9/MySQLPandas.egg-info/PKG-INFO
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)      401 2023-04-11 06:12:58.000000 MySQLPandas-0.0.9/MySQLPandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)        1 2023-04-11 06:12:58.000000 MySQLPandas-0.0.9/MySQLPandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       57 2023-04-11 06:12:58.000000 MySQLPandas-0.0.9/MySQLPandas.egg-info/requires.txt
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       28 2023-04-11 06:12:58.000000 MySQLPandas-0.0.9/MySQLPandas.egg-info/top_level.txt
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     2417 2023-04-11 06:12:58.784556 MySQLPandas-0.0.9/PKG-INFO
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     1775 2023-04-11 06:08:32.000000 MySQLPandas-0.0.9/README.md
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       38 2023-04-11 06:12:58.785556 MySQLPandas-0.0.9/setup.cfg
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     1893 2023-04-11 06:10:37.000000 MySQLPandas-0.0.9/setup.py
+drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-11 06:12:58.782556 MySQLPandas-0.0.9/tests/
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     4526 2023-04-07 04:49:44.000000 MySQLPandas-0.0.9/tests/test_DataFrameClass.py
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     2132 2023-04-07 06:25:10.000000 MySQLPandas-0.0.9/tests/test_coreClass.py
```

### Comparing `MySQLPandas-0.0.8/MySQLPandas/core.py` & `MySQLPandas-0.0.9/MySQLPandas/core.py`

 * *Files identical despite different names*

### Comparing `MySQLPandas-0.0.8/MySQLPandas/lib/DataFrameClass.py` & `MySQLPandas-0.0.9/MySQLPandas/lib/DataFrameClass.py`

 * *Files identical despite different names*

### Comparing `MySQLPandas-0.0.8/MySQLPandas.egg-info/PKG-INFO` & `MySQLPandas-0.0.9/MySQLPandas.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: MySQLPandas
-Version: 0.0.8
+Version: 0.0.9
 Summary: MySQLPandas: simple connector between MySQL(MariaDB) and Pandas
 Home-page: https://github.com/Sota-Nakashima/MySQLPandas
 Author: Sota-Nakashima
 Author-email: souta.nakashima2001@gmail.com
-License: MIT
+License: GPLv2
 Keywords: Python,Pandas,Database
 Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
-License-File: LICENCE
+License-File: LICENSE
 
 MySQLPandas
 ============
 [![pages-build-deployment](https://github.com/Sota-Nakashima/MySQLPandas/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/Sota-Nakashima/MySQLPandas/actions/workflows/pages/pages-build-deployment)
 [![Version](https://img.shields.io/badge/stable-main-gree)](https://github.com/Sota-Nakashima/MySQLPandas)
-[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/Sota-Nakashima/MySQLPandas/blob/main/LICENCE)
+[![GNU GPLv2](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/Sota-Nakashima/MySQLPandas/blob/main/LICENCE)
 #  Overview
 Simple connector between MySQL(MariaDB) and Pandas
 
 ## Description
 This tool is primarily intended to help Python users easily handle databases.
 It uses Pandas as its base, so it should be easy to use even for those who are not familiar with databases.
 The tool supports MySQL or MariaDB as the database engine.
```

### Comparing `MySQLPandas-0.0.8/PKG-INFO` & `MySQLPandas-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: MySQLPandas
-Version: 0.0.8
+Version: 0.0.9
 Summary: MySQLPandas: simple connector between MySQL(MariaDB) and Pandas
 Home-page: https://github.com/Sota-Nakashima/MySQLPandas
 Author: Sota-Nakashima
 Author-email: souta.nakashima2001@gmail.com
-License: MIT
+License: GPLv2
 Keywords: Python,Pandas,Database
 Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
-License-File: LICENCE
+License-File: LICENSE
 
 MySQLPandas
 ============
 [![pages-build-deployment](https://github.com/Sota-Nakashima/MySQLPandas/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/Sota-Nakashima/MySQLPandas/actions/workflows/pages/pages-build-deployment)
 [![Version](https://img.shields.io/badge/stable-main-gree)](https://github.com/Sota-Nakashima/MySQLPandas)
-[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/Sota-Nakashima/MySQLPandas/blob/main/LICENCE)
+[![GNU GPLv2](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/Sota-Nakashima/MySQLPandas/blob/main/LICENCE)
 #  Overview
 Simple connector between MySQL(MariaDB) and Pandas
 
 ## Description
 This tool is primarily intended to help Python users easily handle databases.
 It uses Pandas as its base, so it should be easy to use even for those who are not familiar with databases.
 The tool supports MySQL or MariaDB as the database engine.
```

### Comparing `MySQLPandas-0.0.8/README.md` & `MySQLPandas-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 MySQLPandas
 ============
 [![pages-build-deployment](https://github.com/Sota-Nakashima/MySQLPandas/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/Sota-Nakashima/MySQLPandas/actions/workflows/pages/pages-build-deployment)
 [![Version](https://img.shields.io/badge/stable-main-gree)](https://github.com/Sota-Nakashima/MySQLPandas)
-[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/Sota-Nakashima/MySQLPandas/blob/main/LICENCE)
+[![GNU GPLv2](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/Sota-Nakashima/MySQLPandas/blob/main/LICENCE)
 #  Overview
 Simple connector between MySQL(MariaDB) and Pandas
 
 ## Description
 This tool is primarily intended to help Python users easily handle databases.
 It uses Pandas as its base, so it should be easy to use even for those who are not familiar with databases.
 The tool supports MySQL or MariaDB as the database engine.
```

### Comparing `MySQLPandas-0.0.8/setup.py` & `MySQLPandas-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,13 +53,13 @@
     description='MySQLPandas: simple connector between MySQL(MariaDB) and Pandas',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='Python, Pandas, Database',
 
     classifiers=[
         'Development Status :: 4 - Beta',
-        'License :: OSI Approved :: MIT License',
+        'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Database',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
 )
```

### Comparing `MySQLPandas-0.0.8/tests/test_DataFrameClass.py` & `MySQLPandas-0.0.9/tests/test_DataFrameClass.py`

 * *Files identical despite different names*

### Comparing `MySQLPandas-0.0.8/tests/test_coreClass.py` & `MySQLPandas-0.0.9/tests/test_coreClass.py`

 * *Files identical despite different names*

