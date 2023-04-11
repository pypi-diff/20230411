# Comparing `tmp/legacyplatequery-0.1.0.tar.gz` & `tmp/legacyplatequery-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legacyplatequery-0.1.0.tar", last modified: Tue Apr 11 13:56:48 2023, max compression
+gzip compressed data, was "legacyplatequery-0.1.1.tar", last modified: Tue Apr 11 14:53:00 2023, max compression
```

## Comparing `legacyplatequery-0.1.0.tar` & `legacyplatequery-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 13:56:48.896939 legacyplatequery-0.1.0/
--rw-rw-rw-   0        0        0     3752 2023-04-11 08:01:55.000000 legacyplatequery-0.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-11 08:01:55.000000 legacyplatequery-0.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1528 2023-04-11 13:46:39.000000 legacyplatequery-0.1.0/LICENSE.rst
--rw-rw-rw-   0        0        0      252 2023-04-11 08:01:55.000000 legacyplatequery-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1181 2023-04-11 13:56:48.896939 legacyplatequery-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-04-11 13:45:16.000000 legacyplatequery-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-11 13:56:48.887969 legacyplatequery-0.1.0/docs/
--rw-rw-rw-   0        0        0      637 2023-04-11 08:01:55.000000 legacyplatequery-0.1.0/docs/Makefile
--rw-rw-rw-   0        0        0     5058 2023-04-11 08:01:55.000000 legacyplatequery-0.1.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-11 08:01:55.000000 legacyplatequery-0.1.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-11 08:01:55.000000 legacyplatequery-0.1.0/docs/history.rst
--rw-rw-rw-   0        0        0      322 2023-04-11 08:01:55.000000 legacyplatequery-0.1.0/docs/index.rst
--rw-rw-rw-   0        0        0     1248 2023-04-11 08:01:55.000000 legacyplatequery-0.1.0/docs/installation.rst
--rwxrwxrwx   0        0        0      814 2023-04-11 08:01:55.000000 legacyplatequery-0.1.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-11 08:01:55.000000 legacyplatequery-0.1.0/docs/readme.rst
--rw-rw-rw-   0        0        0       95 2023-04-11 08:01:55.000000 legacyplatequery-0.1.0/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-04-11 13:56:48.890959 legacyplatequery-0.1.0/legacyplatequery/
--rw-rw-rw-   0        0        0     1573 2023-04-11 09:21:40.000000 legacyplatequery-0.1.0/legacyplatequery/__init__.py
--rw-rw-rw-   0        0        0     3776 2023-04-11 12:34:26.000000 legacyplatequery-0.1.0/legacyplatequery/api.py
--rw-rw-rw-   0        0        0     7392 2023-04-11 12:31:56.000000 legacyplatequery-0.1.0/legacyplatequery/client.py
--rw-rw-rw-   0        0        0       20 2023-04-11 08:01:55.000000 legacyplatequery-0.1.0/legacyplatequery/legacyplatequery.py
--rw-rw-rw-   0        0        0     1342 2023-04-11 09:19:58.000000 legacyplatequery-0.1.0/legacyplatequery/utils.py
--rw-rw-rw-   0        0        0      642 2023-04-11 08:10:11.000000 legacyplatequery-0.1.0/legacyplatequery/version.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:56:48.893949 legacyplatequery-0.1.0/legacyplatequery.egg-info/
--rw-rw-rw-   0        0        0     1181 2023-04-11 13:56:48.000000 legacyplatequery-0.1.0/legacyplatequery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      667 2023-04-11 13:56:48.000000 legacyplatequery-0.1.0/legacyplatequery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 13:56:48.000000 legacyplatequery-0.1.0/legacyplatequery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 09:15:52.000000 legacyplatequery-0.1.0/legacyplatequery.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2023-04-11 13:56:48.000000 legacyplatequery-0.1.0/legacyplatequery.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      459 2023-04-11 13:56:48.897936 legacyplatequery-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1246 2023-04-11 09:13:59.000000 legacyplatequery-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:56:48.896939 legacyplatequery-0.1.0/tests/
--rw-rw-rw-   0        0        0       47 2023-04-11 08:01:55.000000 legacyplatequery-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      167 2023-04-11 10:11:44.000000 legacyplatequery-0.1.0/tests/test_api.py
--rw-rw-rw-   0        0        0      433 2023-04-11 12:22:35.000000 legacyplatequery-0.1.0/tests/test_legacyplatequery.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:53:00.187433 legacyplatequery-0.1.1/
+-rw-rw-rw-   0        0        0     3752 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1528 2023-04-11 13:46:39.000000 legacyplatequery-0.1.1/LICENSE.rst
+-rw-rw-rw-   0        0        0      252 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1785 2023-04-11 14:53:00.187433 legacyplatequery-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1060 2023-04-11 14:28:25.000000 legacyplatequery-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 14:53:00.174412 legacyplatequery-0.1.1/docs/
+-rw-rw-rw-   0        0        0      637 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/Makefile
+-rw-rw-rw-   0        0        0     5058 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/history.rst
+-rw-rw-rw-   0        0        0      322 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/index.rst
+-rw-rw-rw-   0        0        0     1248 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      814 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/readme.rst
+-rw-rw-rw-   0        0        0       95 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 14:53:00.179457 legacyplatequery-0.1.1/legacyplatequery/
+-rw-rw-rw-   0        0        0     1573 2023-04-11 09:21:40.000000 legacyplatequery-0.1.1/legacyplatequery/__init__.py
+-rw-rw-rw-   0        0        0     3776 2023-04-11 12:34:26.000000 legacyplatequery-0.1.1/legacyplatequery/api.py
+-rw-rw-rw-   0        0        0     7392 2023-04-11 12:31:56.000000 legacyplatequery-0.1.1/legacyplatequery/client.py
+-rw-rw-rw-   0        0        0       20 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/legacyplatequery/legacyplatequery.py
+-rw-rw-rw-   0        0        0     1342 2023-04-11 09:19:58.000000 legacyplatequery-0.1.1/legacyplatequery/utils.py
+-rw-rw-rw-   0        0        0      642 2023-04-11 14:50:36.000000 legacyplatequery-0.1.1/legacyplatequery/version.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:53:00.185435 legacyplatequery-0.1.1/legacyplatequery.egg-info/
+-rw-rw-rw-   0        0        0     1785 2023-04-11 14:53:00.000000 legacyplatequery-0.1.1/legacyplatequery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      706 2023-04-11 14:53:00.000000 legacyplatequery-0.1.1/legacyplatequery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 14:53:00.000000 legacyplatequery-0.1.1/legacyplatequery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 09:15:52.000000 legacyplatequery-0.1.1/legacyplatequery.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-04-11 14:53:00.000000 legacyplatequery-0.1.1/legacyplatequery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-11 14:53:00.000000 legacyplatequery-0.1.1/legacyplatequery.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      459 2023-04-11 14:53:00.188432 legacyplatequery-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1366 2023-04-11 14:50:05.000000 legacyplatequery-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:53:00.187433 legacyplatequery-0.1.1/tests/
+-rw-rw-rw-   0        0        0       47 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      167 2023-04-11 10:11:44.000000 legacyplatequery-0.1.1/tests/test_api.py
+-rw-rw-rw-   0        0        0      433 2023-04-11 12:22:35.000000 legacyplatequery-0.1.1/tests/test_legacyplatequery.py
```

### Comparing `legacyplatequery-0.1.0/CONTRIBUTING.rst` & `legacyplatequery-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.0/LICENSE.rst` & `legacyplatequery-0.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.0/PKG-INFO` & `legacyplatequery-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,87 @@
 Metadata-Version: 2.1
 Name: legacyplatequery
-Version: 0.1.0
+Version: 0.1.1
 Summary: Legacyplate Data Query
 Home-page: https://github.com/wangweihua/legacyplatequery
 Author: Wang Weihua
 Author-email: wangwh@czu.cn
 Keywords: legacyplatequery
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 License-File: LICENSE.rst
 
 =================
 legacyplate query
 =================
 
-Legacyplate Data Query
+Description
+-----------
+legacyplatequery is a legacyplate query tool developed by Shanghai Astronomical Observatory. 
+It provide a python package like Astroquery.
 
 
-Features
---------
-
-* TODO
+Installation
+------------
+
+You can use pip command to install it:
+```shell
+pip install legacyplatequery
+```
 
-Credits
--------
+Usage
+-----
 
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+1. import the package.
+```python
+import  legacyplatequery as lpdata
+```
 
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+2. Login
+```python
+user = 'wangweihua'
+password = 'xxx'
+lpdata.auth(user, password)
+```
 
+3. Get the total number of legacy plate
+```python
+lpdata.get_total_of_plates()
+```
 
-## Installation
+4. Get the total number of the stars in the star catalog
+```python
+lpdata.get_total_of_star_catalog()
+```
 
+5. Search the legacy plates with `q3c_radial_query`
+```python
+ra = 12.0
+dec = 12.0
+radius = 12
+plates = lpdata.get_plates_by_radial_query(ra, dec, radius)
+print(plates)
 ```
-$ pip install legacyplatequery
+
+6. Search the stars with `q3c_radial_query`
+```python
+stars = lpdata.get_star_catalog_by_radial_query(ra, dec)
+print(stars)
 ```
 
+
+
+
+
 =======
 History
 =======
 
 0.1.0 (2023-04-11)
 ------------------
```

### Comparing `legacyplatequery-0.1.0/docs/Makefile` & `legacyplatequery-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.0/docs/conf.py` & `legacyplatequery-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.0/docs/installation.rst` & `legacyplatequery-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.0/docs/make.bat` & `legacyplatequery-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.0/legacyplatequery/__init__.py` & `legacyplatequery-0.1.1/legacyplatequery/__init__.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.0/legacyplatequery/api.py` & `legacyplatequery-0.1.1/legacyplatequery/api.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.0/legacyplatequery/client.py` & `legacyplatequery-0.1.1/legacyplatequery/client.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.0/legacyplatequery/utils.py` & `legacyplatequery-0.1.1/legacyplatequery/utils.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.0/legacyplatequery/version.py` & `legacyplatequery-0.1.1/legacyplatequery/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (c) 2023--2028, Wang Weihua.
 # All rights reserved.
 """Legacyplatequery 版本号"""
 __author__ = """Wang Weihua"""
 __email__ = 'wangwh@czu.cn'
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 
 _VersionInfo = __import__("collections").namedtuple(
     "version_info", ["major", "minor", "micro"]
 )
 version_info = ([int(v) for v in __version__.split('.')[:3]] + [0] * 3)[:3]
 version_info = _VersionInfo(*version_info)
```

### Comparing `legacyplatequery-0.1.0/legacyplatequery.egg-info/PKG-INFO` & `legacyplatequery-0.1.1/legacyplatequery.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,87 @@
 Metadata-Version: 2.1
 Name: legacyplatequery
-Version: 0.1.0
+Version: 0.1.1
 Summary: Legacyplate Data Query
 Home-page: https://github.com/wangweihua/legacyplatequery
 Author: Wang Weihua
 Author-email: wangwh@czu.cn
 Keywords: legacyplatequery
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 License-File: LICENSE.rst
 
 =================
 legacyplate query
 =================
 
-Legacyplate Data Query
+Description
+-----------
+legacyplatequery is a legacyplate query tool developed by Shanghai Astronomical Observatory. 
+It provide a python package like Astroquery.
 
 
-Features
---------
-
-* TODO
+Installation
+------------
+
+You can use pip command to install it:
+```shell
+pip install legacyplatequery
+```
 
-Credits
--------
+Usage
+-----
 
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+1. import the package.
+```python
+import  legacyplatequery as lpdata
+```
 
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+2. Login
+```python
+user = 'wangweihua'
+password = 'xxx'
+lpdata.auth(user, password)
+```
 
+3. Get the total number of legacy plate
+```python
+lpdata.get_total_of_plates()
+```
 
-## Installation
+4. Get the total number of the stars in the star catalog
+```python
+lpdata.get_total_of_star_catalog()
+```
 
+5. Search the legacy plates with `q3c_radial_query`
+```python
+ra = 12.0
+dec = 12.0
+radius = 12
+plates = lpdata.get_plates_by_radial_query(ra, dec, radius)
+print(plates)
 ```
-$ pip install legacyplatequery
+
+6. Search the stars with `q3c_radial_query`
+```python
+stars = lpdata.get_star_catalog_by_radial_query(ra, dec)
+print(stars)
 ```
 
+
+
+
+
 =======
 History
 =======
 
 0.1.0 (2023-04-11)
 ------------------
```

### Comparing `legacyplatequery-0.1.0/legacyplatequery.egg-info/SOURCES.txt` & `legacyplatequery-0.1.1/legacyplatequery.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,11 +20,12 @@
 legacyplatequery/legacyplatequery.py
 legacyplatequery/utils.py
 legacyplatequery/version.py
 legacyplatequery.egg-info/PKG-INFO
 legacyplatequery.egg-info/SOURCES.txt
 legacyplatequery.egg-info/dependency_links.txt
 legacyplatequery.egg-info/not-zip-safe
+legacyplatequery.egg-info/requires.txt
 legacyplatequery.egg-info/top_level.txt
 tests/__init__.py
 tests/test_api.py
 tests/test_legacyplatequery.py
```

### Comparing `legacyplatequery-0.1.0/setup.py` & `legacyplatequery-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,37 +6,41 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = [ ]
+requirements = ['requests',
+                'numpy',
+                'pandas',
+                'matplotlib',
+                'astropy']
 
-test_requirements = ['pytest>=3', ]
+test_requirements = ['pytest>=3']
 
 setup(
     author="Wang Weihua",
     author_email='wangwh@czu.cn',
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
     description="Legacyplate Data Query",
     install_requires=requirements,
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='legacyplatequery',
     name='legacyplatequery',
     packages=find_packages(include=['legacyplatequery', 'legacyplatequery.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/wangweihua/legacyplatequery',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

