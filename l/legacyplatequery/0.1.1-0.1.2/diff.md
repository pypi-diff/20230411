# Comparing `tmp/legacyplatequery-0.1.1.tar.gz` & `tmp/legacyplatequery-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legacyplatequery-0.1.1.tar", last modified: Tue Apr 11 14:53:00 2023, max compression
+gzip compressed data, was "legacyplatequery-0.1.2.tar", last modified: Tue Apr 11 15:12:16 2023, max compression
```

## Comparing `legacyplatequery-0.1.1.tar` & `legacyplatequery-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 14:53:00.187433 legacyplatequery-0.1.1/
--rw-rw-rw-   0        0        0     3752 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1528 2023-04-11 13:46:39.000000 legacyplatequery-0.1.1/LICENSE.rst
--rw-rw-rw-   0        0        0      252 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1785 2023-04-11 14:53:00.187433 legacyplatequery-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1060 2023-04-11 14:28:25.000000 legacyplatequery-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-11 14:53:00.174412 legacyplatequery-0.1.1/docs/
--rw-rw-rw-   0        0        0      637 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/Makefile
--rw-rw-rw-   0        0        0     5058 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/history.rst
--rw-rw-rw-   0        0        0      322 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/index.rst
--rw-rw-rw-   0        0        0     1248 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/installation.rst
--rwxrwxrwx   0        0        0      814 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/readme.rst
--rw-rw-rw-   0        0        0       95 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-04-11 14:53:00.179457 legacyplatequery-0.1.1/legacyplatequery/
--rw-rw-rw-   0        0        0     1573 2023-04-11 09:21:40.000000 legacyplatequery-0.1.1/legacyplatequery/__init__.py
--rw-rw-rw-   0        0        0     3776 2023-04-11 12:34:26.000000 legacyplatequery-0.1.1/legacyplatequery/api.py
--rw-rw-rw-   0        0        0     7392 2023-04-11 12:31:56.000000 legacyplatequery-0.1.1/legacyplatequery/client.py
--rw-rw-rw-   0        0        0       20 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/legacyplatequery/legacyplatequery.py
--rw-rw-rw-   0        0        0     1342 2023-04-11 09:19:58.000000 legacyplatequery-0.1.1/legacyplatequery/utils.py
--rw-rw-rw-   0        0        0      642 2023-04-11 14:50:36.000000 legacyplatequery-0.1.1/legacyplatequery/version.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:53:00.185435 legacyplatequery-0.1.1/legacyplatequery.egg-info/
--rw-rw-rw-   0        0        0     1785 2023-04-11 14:53:00.000000 legacyplatequery-0.1.1/legacyplatequery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      706 2023-04-11 14:53:00.000000 legacyplatequery-0.1.1/legacyplatequery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 14:53:00.000000 legacyplatequery-0.1.1/legacyplatequery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 09:15:52.000000 legacyplatequery-0.1.1/legacyplatequery.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-04-11 14:53:00.000000 legacyplatequery-0.1.1/legacyplatequery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-11 14:53:00.000000 legacyplatequery-0.1.1/legacyplatequery.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      459 2023-04-11 14:53:00.188432 legacyplatequery-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1366 2023-04-11 14:50:05.000000 legacyplatequery-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:53:00.187433 legacyplatequery-0.1.1/tests/
--rw-rw-rw-   0        0        0       47 2023-04-11 08:01:55.000000 legacyplatequery-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0      167 2023-04-11 10:11:44.000000 legacyplatequery-0.1.1/tests/test_api.py
--rw-rw-rw-   0        0        0      433 2023-04-11 12:22:35.000000 legacyplatequery-0.1.1/tests/test_legacyplatequery.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:12:16.091778 legacyplatequery-0.1.2/
+-rw-rw-rw-   0        0        0     3752 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1528 2023-04-11 13:46:39.000000 legacyplatequery-0.1.2/LICENSE.rst
+-rw-rw-rw-   0        0        0      252 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1797 2023-04-11 15:12:16.091778 legacyplatequery-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1072 2023-04-11 14:59:37.000000 legacyplatequery-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 15:12:16.081812 legacyplatequery-0.1.2/docs/
+-rw-rw-rw-   0        0        0      637 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/Makefile
+-rw-rw-rw-   0        0        0     5058 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/history.rst
+-rw-rw-rw-   0        0        0      322 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/index.rst
+-rw-rw-rw-   0        0        0     1248 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/installation.rst
+-rwxrwxrwx   0        0        0      814 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/readme.rst
+-rw-rw-rw-   0        0        0       95 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 15:12:16.085802 legacyplatequery-0.1.2/legacyplatequery/
+-rw-rw-rw-   0        0        0     1573 2023-04-11 09:21:40.000000 legacyplatequery-0.1.2/legacyplatequery/__init__.py
+-rw-rw-rw-   0        0        0     3776 2023-04-11 12:34:26.000000 legacyplatequery-0.1.2/legacyplatequery/api.py
+-rw-rw-rw-   0        0        0     7392 2023-04-11 12:31:56.000000 legacyplatequery-0.1.2/legacyplatequery/client.py
+-rw-rw-rw-   0        0        0       20 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/legacyplatequery/legacyplatequery.py
+-rw-rw-rw-   0        0        0     1342 2023-04-11 09:19:58.000000 legacyplatequery-0.1.2/legacyplatequery/utils.py
+-rw-rw-rw-   0        0        0      642 2023-04-11 14:50:36.000000 legacyplatequery-0.1.2/legacyplatequery/version.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:12:16.089789 legacyplatequery-0.1.2/legacyplatequery.egg-info/
+-rw-rw-rw-   0        0        0     1797 2023-04-11 15:12:16.000000 legacyplatequery-0.1.2/legacyplatequery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      706 2023-04-11 15:12:16.000000 legacyplatequery-0.1.2/legacyplatequery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 15:12:16.000000 legacyplatequery-0.1.2/legacyplatequery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 09:15:52.000000 legacyplatequery-0.1.2/legacyplatequery.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-04-11 15:12:16.000000 legacyplatequery-0.1.2/legacyplatequery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-11 15:12:16.000000 legacyplatequery-0.1.2/legacyplatequery.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      459 2023-04-11 15:12:16.091778 legacyplatequery-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1338 2023-04-11 15:11:47.000000 legacyplatequery-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:12:16.090785 legacyplatequery-0.1.2/tests/
+-rw-rw-rw-   0        0        0       47 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      167 2023-04-11 10:11:44.000000 legacyplatequery-0.1.2/tests/test_api.py
+-rw-rw-rw-   0        0        0      433 2023-04-11 12:22:35.000000 legacyplatequery-0.1.2/tests/test_legacyplatequery.py
```

### Comparing `legacyplatequery-0.1.1/CONTRIBUTING.rst` & `legacyplatequery-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.1/LICENSE.rst` & `legacyplatequery-0.1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.1/PKG-INFO` & `legacyplatequery-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legacyplatequery
-Version: 0.1.1
+Version: 0.1.2
 Summary: Legacyplate Data Query
 Home-page: https://github.com/wangweihua/legacyplatequery
 Author: Wang Weihua
 Author-email: wangwh@czu.cn
 Keywords: legacyplatequery
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -34,45 +34,51 @@
 pip install legacyplatequery
 ```
 
 Usage
 -----
 
 1. import the package.
+
 ```python
 import  legacyplatequery as lpdata
 ```
 
 2. Login
+
 ```python
 user = 'wangweihua'
 password = 'xxx'
 lpdata.auth(user, password)
 ```
 
 3. Get the total number of legacy plate
+
 ```python
 lpdata.get_total_of_plates()
 ```
 
 4. Get the total number of the stars in the star catalog
+
 ```python
 lpdata.get_total_of_star_catalog()
 ```
 
 5. Search the legacy plates with `q3c_radial_query`
+
 ```python
 ra = 12.0
 dec = 12.0
 radius = 12
 plates = lpdata.get_plates_by_radial_query(ra, dec, radius)
 print(plates)
 ```
 
 6. Search the stars with `q3c_radial_query`
+
 ```python
 stars = lpdata.get_star_catalog_by_radial_query(ra, dec)
 print(stars)
 ```
```

### Comparing `legacyplatequery-0.1.1/README.rst` & `legacyplatequery-0.1.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -16,45 +16,51 @@
 pip install legacyplatequery
 ```
 
 Usage
 -----
 
 1. import the package.
+
 ```python
 import  legacyplatequery as lpdata
 ```
 
 2. Login
+
 ```python
 user = 'wangweihua'
 password = 'xxx'
 lpdata.auth(user, password)
 ```
 
 3. Get the total number of legacy plate
+
 ```python
 lpdata.get_total_of_plates()
 ```
 
 4. Get the total number of the stars in the star catalog
+
 ```python
 lpdata.get_total_of_star_catalog()
 ```
 
 5. Search the legacy plates with `q3c_radial_query`
+
 ```python
 ra = 12.0
 dec = 12.0
 radius = 12
 plates = lpdata.get_plates_by_radial_query(ra, dec, radius)
 print(plates)
 ```
 
 6. Search the stars with `q3c_radial_query`
+
 ```python
 stars = lpdata.get_star_catalog_by_radial_query(ra, dec)
 print(stars)
 ```
```

### Comparing `legacyplatequery-0.1.1/docs/Makefile` & `legacyplatequery-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.1/docs/conf.py` & `legacyplatequery-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.1/docs/installation.rst` & `legacyplatequery-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.1/docs/make.bat` & `legacyplatequery-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.1/legacyplatequery/__init__.py` & `legacyplatequery-0.1.2/legacyplatequery/__init__.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.1/legacyplatequery/api.py` & `legacyplatequery-0.1.2/legacyplatequery/api.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.1/legacyplatequery/client.py` & `legacyplatequery-0.1.2/legacyplatequery/client.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.1/legacyplatequery/utils.py` & `legacyplatequery-0.1.2/legacyplatequery/utils.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.1/legacyplatequery/version.py` & `legacyplatequery-0.1.2/legacyplatequery/version.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.1/legacyplatequery.egg-info/PKG-INFO` & `legacyplatequery-0.1.2/legacyplatequery.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legacyplatequery
-Version: 0.1.1
+Version: 0.1.2
 Summary: Legacyplate Data Query
 Home-page: https://github.com/wangweihua/legacyplatequery
 Author: Wang Weihua
 Author-email: wangwh@czu.cn
 Keywords: legacyplatequery
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -34,45 +34,51 @@
 pip install legacyplatequery
 ```
 
 Usage
 -----
 
 1. import the package.
+
 ```python
 import  legacyplatequery as lpdata
 ```
 
 2. Login
+
 ```python
 user = 'wangweihua'
 password = 'xxx'
 lpdata.auth(user, password)
 ```
 
 3. Get the total number of legacy plate
+
 ```python
 lpdata.get_total_of_plates()
 ```
 
 4. Get the total number of the stars in the star catalog
+
 ```python
 lpdata.get_total_of_star_catalog()
 ```
 
 5. Search the legacy plates with `q3c_radial_query`
+
 ```python
 ra = 12.0
 dec = 12.0
 radius = 12
 plates = lpdata.get_plates_by_radial_query(ra, dec, radius)
 print(plates)
 ```
 
 6. Search the stars with `q3c_radial_query`
+
 ```python
 stars = lpdata.get_star_catalog_by_radial_query(ra, dec)
 print(stars)
 ```
```

### Comparing `legacyplatequery-0.1.1/legacyplatequery.egg-info/SOURCES.txt` & `legacyplatequery-0.1.2/legacyplatequery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.1/setup.py` & `legacyplatequery-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = ['requests',
                 'numpy',
                 'pandas',
-                'matplotlib',
-                'astropy']
+                'matplotlib']
 
 test_requirements = ['pytest>=3']
 
 setup(
     author="Wang Weihua",
     author_email='wangwh@czu.cn',
     python_requires='>=3.8',
@@ -37,10 +36,10 @@
     include_package_data=True,
     keywords='legacyplatequery',
     name='legacyplatequery',
     packages=find_packages(include=['legacyplatequery', 'legacyplatequery.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/wangweihua/legacyplatequery',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

