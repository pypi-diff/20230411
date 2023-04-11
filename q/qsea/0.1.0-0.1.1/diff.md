# Comparing `tmp/qsea-0.1.0.tar.gz` & `tmp/qsea-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\qsea-0.1.0.tar", last modified: Tue Apr 11 20:40:17 2023, max compression
+gzip compressed data, was "dist\qsea-0.1.1.tar", last modified: Tue Apr 11 21:09:47 2023, max compression
```

## Comparing `qsea-0.1.0.tar` & `qsea-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 20:40:17.693055 qsea-0.1.0/
--rw-rw-rw-   0        0        0     1061 2023-01-13 17:31:55.000000 qsea-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      606 2023-04-11 20:40:17.692055 qsea-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-01-13 17:37:30.000000 qsea-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 20:40:17.664073 qsea-0.1.0/qsea/
--rw-rw-rw-   0        0        0       48 2023-01-13 17:39:45.000000 qsea-0.1.0/qsea/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:40:17.690058 qsea-0.1.0/qsea.egg-info/
--rw-rw-rw-   0        0        0      606 2023-04-11 20:40:17.000000 qsea-0.1.0/qsea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-04-11 20:40:17.000000 qsea-0.1.0/qsea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 20:40:17.000000 qsea-0.1.0/qsea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-11 20:40:17.000000 qsea-0.1.0/qsea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-11 20:40:17.000000 qsea-0.1.0/qsea.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 20:40:17.693055 qsea-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      876 2023-04-11 20:25:00.000000 qsea-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:09:47.042957 qsea-0.1.1/
+-rw-rw-rw-   0        0        0     1061 2023-01-13 17:31:55.000000 qsea-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      606 2023-04-11 21:09:47.040878 qsea-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-01-13 17:37:30.000000 qsea-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 21:09:47.030884 qsea-0.1.1/qsea/
+-rw-rw-rw-   0        0        0       48 2023-01-13 17:39:45.000000 qsea-0.1.1/qsea/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:09:47.038878 qsea-0.1.1/qsea.egg-info/
+-rw-rw-rw-   0        0        0      606 2023-04-11 21:09:46.000000 qsea-0.1.1/qsea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-04-11 21:09:46.000000 qsea-0.1.1/qsea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:09:46.000000 qsea-0.1.1/qsea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-11 21:09:46.000000 qsea-0.1.1/qsea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-11 21:09:46.000000 qsea-0.1.1/qsea.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 21:09:47.042957 qsea-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      840 2023-04-11 21:08:47.000000 qsea-0.1.1/setup.py
```

### Comparing `qsea-0.1.0/LICENSE.txt` & `qsea-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qsea-0.1.0/PKG-INFO` & `qsea-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsea
-Version: 0.1.0
+Version: 0.1.1
 Summary: Convenient way to work with Qlik Sense Engine API from Python
 Home-page: https://github.com/ncthuc/qsea
 Download-URL: https://pypi.org/project/qsea/
 Author: Lev Biriukov
 Author-email: lbiryukov@gmail.com
 License: MIT
 Keywords: QlikSense,Qlik
```

### Comparing `qsea-0.1.0/qsea.egg-info/PKG-INFO` & `qsea-0.1.1/qsea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsea
-Version: 0.1.0
+Version: 0.1.1
 Summary: Convenient way to work with Qlik Sense Engine API from Python
 Home-page: https://github.com/ncthuc/qsea
 Download-URL: https://pypi.org/project/qsea/
 Author: Lev Biriukov
 Author-email: lbiryukov@gmail.com
 License: MIT
 Keywords: QlikSense,Qlik
```

### Comparing `qsea-0.1.0/setup.py` & `qsea-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 from setuptools import setup, find_packages
-print(10)
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='qsea',
-    version='0.1.0',
+    version='0.1.1',
     description='Convenient way to work with Qlik Sense Engine API from Python',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Lev Biriukov',
     author_email='lbiryukov@gmail.com',
     keywords=['QlikSense', 'Qlik'],
     url='https://github.com/ncthuc/qsea',
     download_url='https://pypi.org/project/qsea/'
 )
 
-install_requires = [
-    'json',
-    'pandas',
-	'datetime',
-	'logging'
-]
+install_requires = ['pandas', 'datetime', 'logging']
 
 if __name__ == '__main__':
     setup(**setup_args, install_requires=install_requires)
```

