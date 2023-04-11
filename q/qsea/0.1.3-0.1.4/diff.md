# Comparing `tmp/qsea-0.1.3.tar.gz` & `tmp/qsea-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\qsea-0.1.3.tar", last modified: Tue Apr 11 21:30:15 2023, max compression
+gzip compressed data, was "dist\qsea-0.1.4.tar", last modified: Tue Apr 11 21:45:48 2023, max compression
```

## Comparing `qsea-0.1.3.tar` & `qsea-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 21:30:15.820090 qsea-0.1.3/
--rw-rw-rw-   0        0        0     1061 2023-01-13 17:31:55.000000 qsea-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0      606 2023-04-11 21:30:15.818053 qsea-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-01-13 17:37:30.000000 qsea-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 21:30:15.803062 qsea-0.1.3/qsea/
--rw-rw-rw-   0        0        0       50 2023-04-11 21:27:17.000000 qsea-0.1.3/qsea/__init__.py
--rw-rw-rw-   0        0        0    59908 2023-04-11 21:29:44.000000 qsea-0.1.3/qsea/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-11 21:30:15.817056 qsea-0.1.3/qsea.egg-info/
--rw-rw-rw-   0        0        0      606 2023-04-11 21:30:15.000000 qsea-0.1.3/qsea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-04-11 21:30:15.000000 qsea-0.1.3/qsea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 21:30:15.000000 qsea-0.1.3/qsea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-11 21:30:15.000000 qsea-0.1.3/qsea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-11 21:30:15.000000 qsea-0.1.3/qsea.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 21:30:15.820090 qsea-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      829 2023-04-11 21:27:41.000000 qsea-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:45:48.614323 qsea-0.1.4/
+-rw-rw-rw-   0        0        0     1061 2023-01-13 17:31:55.000000 qsea-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      606 2023-04-11 21:45:48.612320 qsea-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-01-13 17:37:30.000000 qsea-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 21:45:48.606325 qsea-0.1.4/qsea/
+-rw-rw-rw-   0        0        0    59908 2023-04-11 21:29:44.000000 qsea-0.1.4/qsea/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:45:48.611321 qsea-0.1.4/qsea.egg-info/
+-rw-rw-rw-   0        0        0      606 2023-04-11 21:45:48.000000 qsea-0.1.4/qsea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-04-11 21:45:48.000000 qsea-0.1.4/qsea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:45:48.000000 qsea-0.1.4/qsea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-11 21:45:48.000000 qsea-0.1.4/qsea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-11 21:45:48.000000 qsea-0.1.4/qsea.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 21:45:48.614323 qsea-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      829 2023-04-11 21:45:39.000000 qsea-0.1.4/setup.py
```

### Comparing `qsea-0.1.3/LICENSE.txt` & `qsea-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qsea-0.1.3/PKG-INFO` & `qsea-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsea
-Version: 0.1.3
+Version: 0.1.4
 Summary: Convenient way to work with Qlik Sense Engine API from Python
 Home-page: https://github.com/ncthuc/qsea
 Download-URL: https://pypi.org/project/qsea/
 Author: Lev Biriukov
 Author-email: lbiryukov@gmail.com
 License: MIT
 Keywords: QlikSense,Qlik
```

### Comparing `qsea-0.1.3/qsea/tools.py` & `qsea-0.1.4/qsea/__init__.py`

 * *Files identical despite different names*

### Comparing `qsea-0.1.3/qsea.egg-info/PKG-INFO` & `qsea-0.1.4/qsea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsea
-Version: 0.1.3
+Version: 0.1.4
 Summary: Convenient way to work with Qlik Sense Engine API from Python
 Home-page: https://github.com/ncthuc/qsea
 Download-URL: https://pypi.org/project/qsea/
 Author: Lev Biriukov
 Author-email: lbiryukov@gmail.com
 License: MIT
 Keywords: QlikSense,Qlik
```

### Comparing `qsea-0.1.3/setup.py` & `qsea-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='qsea',
-    version='0.1.3',
+    version='0.1.4',
     description='Convenient way to work with Qlik Sense Engine API from Python',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Lev Biriukov',
     author_email='lbiryukov@gmail.com',
```

