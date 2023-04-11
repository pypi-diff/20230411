# Comparing `tmp/legacyplatequery-0.1.2.tar.gz` & `tmp/legacyplatequery-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legacyplatequery-0.1.2.tar", last modified: Tue Apr 11 15:12:16 2023, max compression
+gzip compressed data, was "legacyplatequery-0.1.3.tar", last modified: Tue Apr 11 15:17:59 2023, max compression
```

## Comparing `legacyplatequery-0.1.2.tar` & `legacyplatequery-0.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 15:12:16.091778 legacyplatequery-0.1.2/
--rw-rw-rw-   0        0        0     3752 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/HISTORY.rst
--rw-rw-rw-   0        0        0     1528 2023-04-11 13:46:39.000000 legacyplatequery-0.1.2/LICENSE.rst
--rw-rw-rw-   0        0        0      252 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1797 2023-04-11 15:12:16.091778 legacyplatequery-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1072 2023-04-11 14:59:37.000000 legacyplatequery-0.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-11 15:12:16.081812 legacyplatequery-0.1.2/docs/
--rw-rw-rw-   0        0        0      637 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/Makefile
--rw-rw-rw-   0        0        0     5058 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/history.rst
--rw-rw-rw-   0        0        0      322 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/index.rst
--rw-rw-rw-   0        0        0     1248 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/installation.rst
--rwxrwxrwx   0        0        0      814 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/readme.rst
--rw-rw-rw-   0        0        0       95 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-04-11 15:12:16.085802 legacyplatequery-0.1.2/legacyplatequery/
--rw-rw-rw-   0        0        0     1573 2023-04-11 09:21:40.000000 legacyplatequery-0.1.2/legacyplatequery/__init__.py
--rw-rw-rw-   0        0        0     3776 2023-04-11 12:34:26.000000 legacyplatequery-0.1.2/legacyplatequery/api.py
--rw-rw-rw-   0        0        0     7392 2023-04-11 12:31:56.000000 legacyplatequery-0.1.2/legacyplatequery/client.py
--rw-rw-rw-   0        0        0       20 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/legacyplatequery/legacyplatequery.py
--rw-rw-rw-   0        0        0     1342 2023-04-11 09:19:58.000000 legacyplatequery-0.1.2/legacyplatequery/utils.py
--rw-rw-rw-   0        0        0      642 2023-04-11 14:50:36.000000 legacyplatequery-0.1.2/legacyplatequery/version.py
-drwxrwxrwx   0        0        0        0 2023-04-11 15:12:16.089789 legacyplatequery-0.1.2/legacyplatequery.egg-info/
--rw-rw-rw-   0        0        0     1797 2023-04-11 15:12:16.000000 legacyplatequery-0.1.2/legacyplatequery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      706 2023-04-11 15:12:16.000000 legacyplatequery-0.1.2/legacyplatequery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 15:12:16.000000 legacyplatequery-0.1.2/legacyplatequery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 09:15:52.000000 legacyplatequery-0.1.2/legacyplatequery.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2023-04-11 15:12:16.000000 legacyplatequery-0.1.2/legacyplatequery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-11 15:12:16.000000 legacyplatequery-0.1.2/legacyplatequery.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      459 2023-04-11 15:12:16.091778 legacyplatequery-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1338 2023-04-11 15:11:47.000000 legacyplatequery-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 15:12:16.090785 legacyplatequery-0.1.2/tests/
--rw-rw-rw-   0        0        0       47 2023-04-11 08:01:55.000000 legacyplatequery-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0      167 2023-04-11 10:11:44.000000 legacyplatequery-0.1.2/tests/test_api.py
--rw-rw-rw-   0        0        0      433 2023-04-11 12:22:35.000000 legacyplatequery-0.1.2/tests/test_legacyplatequery.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:17:59.198167 legacyplatequery-0.1.3/
+-rw-rw-rw-   0        0        0     3752 2023-04-11 08:01:55.000000 legacyplatequery-0.1.3/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-11 08:01:55.000000 legacyplatequery-0.1.3/HISTORY.rst
+-rw-rw-rw-   0        0        0     1528 2023-04-11 13:46:39.000000 legacyplatequery-0.1.3/LICENSE.rst
+-rw-rw-rw-   0        0        0      252 2023-04-11 08:01:55.000000 legacyplatequery-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1797 2023-04-11 15:17:59.198167 legacyplatequery-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1072 2023-04-11 14:59:37.000000 legacyplatequery-0.1.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 15:17:59.188198 legacyplatequery-0.1.3/docs/
+-rw-rw-rw-   0        0        0      637 2023-04-11 08:01:55.000000 legacyplatequery-0.1.3/docs/Makefile
+-rw-rw-rw-   0        0        0     5058 2023-04-11 08:01:55.000000 legacyplatequery-0.1.3/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-11 08:01:55.000000 legacyplatequery-0.1.3/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-11 08:01:55.000000 legacyplatequery-0.1.3/docs/history.rst
+-rw-rw-rw-   0        0        0      322 2023-04-11 08:01:55.000000 legacyplatequery-0.1.3/docs/index.rst
+-rw-rw-rw-   0        0        0     1248 2023-04-11 08:01:55.000000 legacyplatequery-0.1.3/docs/installation.rst
+-rwxrwxrwx   0        0        0      814 2023-04-11 08:01:55.000000 legacyplatequery-0.1.3/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-11 08:01:55.000000 legacyplatequery-0.1.3/docs/readme.rst
+-rw-rw-rw-   0        0        0       95 2023-04-11 08:01:55.000000 legacyplatequery-0.1.3/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 15:17:59.192187 legacyplatequery-0.1.3/legacyplatequery/
+-rw-rw-rw-   0        0        0     1573 2023-04-11 09:21:40.000000 legacyplatequery-0.1.3/legacyplatequery/__init__.py
+-rw-rw-rw-   0        0        0     3776 2023-04-11 12:34:26.000000 legacyplatequery-0.1.3/legacyplatequery/api.py
+-rw-rw-rw-   0        0        0     7392 2023-04-11 12:31:56.000000 legacyplatequery-0.1.3/legacyplatequery/client.py
+-rw-rw-rw-   0        0        0       20 2023-04-11 08:01:55.000000 legacyplatequery-0.1.3/legacyplatequery/legacyplatequery.py
+-rw-rw-rw-   0        0        0     1342 2023-04-11 09:19:58.000000 legacyplatequery-0.1.3/legacyplatequery/utils.py
+-rw-rw-rw-   0        0        0      642 2023-04-11 14:50:36.000000 legacyplatequery-0.1.3/legacyplatequery/version.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:17:59.196188 legacyplatequery-0.1.3/legacyplatequery.egg-info/
+-rw-rw-rw-   0        0        0     1797 2023-04-11 15:17:59.000000 legacyplatequery-0.1.3/legacyplatequery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      706 2023-04-11 15:17:59.000000 legacyplatequery-0.1.3/legacyplatequery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 15:17:59.000000 legacyplatequery-0.1.3/legacyplatequery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 09:15:52.000000 legacyplatequery-0.1.3/legacyplatequery.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-04-11 15:17:59.000000 legacyplatequery-0.1.3/legacyplatequery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-11 15:17:59.000000 legacyplatequery-0.1.3/legacyplatequery.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      459 2023-04-11 15:17:59.198167 legacyplatequery-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1338 2023-04-11 15:17:14.000000 legacyplatequery-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:17:59.197175 legacyplatequery-0.1.3/tests/
+-rw-rw-rw-   0        0        0       47 2023-04-11 08:01:55.000000 legacyplatequery-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      167 2023-04-11 10:11:44.000000 legacyplatequery-0.1.3/tests/test_api.py
+-rw-rw-rw-   0        0        0      433 2023-04-11 12:22:35.000000 legacyplatequery-0.1.3/tests/test_legacyplatequery.py
```

### Comparing `legacyplatequery-0.1.2/CONTRIBUTING.rst` & `legacyplatequery-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.2/LICENSE.rst` & `legacyplatequery-0.1.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.2/PKG-INFO` & `legacyplatequery-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legacyplatequery
-Version: 0.1.2
+Version: 0.1.3
 Summary: Legacyplate Data Query
 Home-page: https://github.com/wangweihua/legacyplatequery
 Author: Wang Weihua
 Author-email: wangwh@czu.cn
 Keywords: legacyplatequery
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `legacyplatequery-0.1.2/README.rst` & `legacyplatequery-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.2/docs/Makefile` & `legacyplatequery-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.2/docs/conf.py` & `legacyplatequery-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.2/docs/installation.rst` & `legacyplatequery-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.2/docs/make.bat` & `legacyplatequery-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.2/legacyplatequery/__init__.py` & `legacyplatequery-0.1.3/legacyplatequery/__init__.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.2/legacyplatequery/api.py` & `legacyplatequery-0.1.3/legacyplatequery/api.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.2/legacyplatequery/client.py` & `legacyplatequery-0.1.3/legacyplatequery/client.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.2/legacyplatequery/utils.py` & `legacyplatequery-0.1.3/legacyplatequery/utils.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.2/legacyplatequery/version.py` & `legacyplatequery-0.1.3/legacyplatequery/version.py`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.2/legacyplatequery.egg-info/PKG-INFO` & `legacyplatequery-0.1.3/legacyplatequery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legacyplatequery
-Version: 0.1.2
+Version: 0.1.3
 Summary: Legacyplate Data Query
 Home-page: https://github.com/wangweihua/legacyplatequery
 Author: Wang Weihua
 Author-email: wangwh@czu.cn
 Keywords: legacyplatequery
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `legacyplatequery-0.1.2/legacyplatequery.egg-info/SOURCES.txt` & `legacyplatequery-0.1.3/legacyplatequery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `legacyplatequery-0.1.2/setup.py` & `legacyplatequery-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,10 +36,10 @@
     include_package_data=True,
     keywords='legacyplatequery',
     name='legacyplatequery',
     packages=find_packages(include=['legacyplatequery', 'legacyplatequery.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/wangweihua/legacyplatequery',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

