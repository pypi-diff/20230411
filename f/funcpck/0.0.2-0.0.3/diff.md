# Comparing `tmp/funcpck-0.0.2.tar.gz` & `tmp/funcpck-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcpck-0.0.2.tar", last modified: Tue Apr 11 16:11:34 2023, max compression
+gzip compressed data, was "funcpck-0.0.3.tar", last modified: Tue Apr 11 21:45:47 2023, max compression
```

## Comparing `funcpck-0.0.2.tar` & `funcpck-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 16:11:34.321517 funcpck-0.0.2/
--rw-rw-rw-   0        0        0     1092 2023-04-11 10:44:32.000000 funcpck-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-11 10:44:32.000000 funcpck-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1367 2023-04-11 16:11:34.321517 funcpck-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-04-11 10:44:32.000000 funcpck-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 16:11:34.305499 funcpck-0.0.2/funcpck/
--rw-rw-rw-   0        0        0      233 2023-04-11 16:08:52.000000 funcpck-0.0.2/funcpck/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 16:11:34.313500 funcpck-0.0.2/funcpck.egg-info/
--rw-rw-rw-   0        0        0     1367 2023-04-11 16:11:34.000000 funcpck-0.0.2/funcpck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-04-11 16:11:34.000000 funcpck-0.0.2/funcpck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 16:11:34.000000 funcpck-0.0.2/funcpck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 16:11:34.000000 funcpck-0.0.2/funcpck.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-04-11 16:11:34.000000 funcpck-0.0.2/funcpck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-11 10:44:32.000000 funcpck-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0      415 2023-04-11 16:11:34.321517 funcpck-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1797 2023-04-11 15:56:12.000000 funcpck-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:45:47.743863 funcpck-0.0.3/
+-rw-rw-rw-   0        0        0     1092 2023-04-11 10:44:32.000000 funcpck-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-11 10:44:32.000000 funcpck-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1367 2023-04-11 21:45:47.743863 funcpck-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-04-11 10:44:32.000000 funcpck-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 21:45:47.735859 funcpck-0.0.3/funcpck/
+-rw-rw-rw-   0        0        0      227 2023-04-11 21:33:27.000000 funcpck-0.0.3/funcpck/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:45:47.743863 funcpck-0.0.3/funcpck.egg-info/
+-rw-rw-rw-   0        0        0     1367 2023-04-11 21:45:47.000000 funcpck-0.0.3/funcpck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-04-11 21:45:47.000000 funcpck-0.0.3/funcpck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:45:47.000000 funcpck-0.0.3/funcpck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 21:45:47.000000 funcpck-0.0.3/funcpck.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-04-11 21:45:47.000000 funcpck-0.0.3/funcpck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-11 10:44:32.000000 funcpck-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0      415 2023-04-11 21:45:47.743863 funcpck-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1797 2023-04-11 21:45:34.000000 funcpck-0.0.3/setup.py
```

### Comparing `funcpck-0.0.2/LICENSE` & `funcpck-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `funcpck-0.0.2/PKG-INFO` & `funcpck-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcpck
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for using a function
 Home-page: https://github.com/Youssefamroo/funcpck
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: funcpck
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `funcpck-0.0.2/README.md` & `funcpck-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `funcpck-0.0.2/funcpck.egg-info/PKG-INFO` & `funcpck-0.0.3/funcpck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcpck
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for using a function
 Home-page: https://github.com/Youssefamroo/funcpck
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: funcpck
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `funcpck-0.0.2/setup.py` & `funcpck-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='funcpck',
     name='funcpck',
     packages=find_packages(include=['funcpck', 'funcpck.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Youssefamroo/funcpck',
-    version='0.0.2',
+    version='0.0.3',
     zip_safe=False,
 )
```

