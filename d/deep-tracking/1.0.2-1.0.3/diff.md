# Comparing `tmp/deep_tracking-1.0.2.tar.gz` & `tmp/deep_tracking-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_tracking-1.0.2.tar", last modified: Tue Apr 11 19:58:12 2023, max compression
+gzip compressed data, was "deep_tracking-1.0.3.tar", last modified: Tue Apr 11 20:10:00 2023, max compression
```

## Comparing `deep_tracking-1.0.2.tar` & `deep_tracking-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 19:58:12.464451 deep_tracking-1.0.2/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     1085 2023-04-11 19:33:15.000000 deep_tracking-1.0.2/LICENCE.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-11 19:58:12.464451 deep_tracking-1.0.2/PKG-INFO
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      429 2023-04-04 11:20:37.000000 deep_tracking-1.0.2/README.md
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 19:58:12.460451 deep_tracking-1.0.2/deep_tracking/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       34 2023-04-11 19:57:41.000000 deep_tracking-1.0.2/deep_tracking/__init__.py
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     9923 2023-04-11 19:54:01.000000 deep_tracking-1.0.2/deep_tracking/deep_tracking.py
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 19:58:12.460451 deep_tracking-1.0.2/deep_tracking.egg-info/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-11 19:58:12.000000 deep_tracking-1.0.2/deep_tracking.egg-info/PKG-INFO
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      271 2023-04-11 19:58:12.000000 deep_tracking-1.0.2/deep_tracking.egg-info/SOURCES.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)        1 2023-04-11 19:58:12.000000 deep_tracking-1.0.2/deep_tracking.egg-info/dependency_links.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-11 19:58:12.000000 deep_tracking-1.0.2/deep_tracking.egg-info/requires.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-11 19:58:12.000000 deep_tracking-1.0.2/deep_tracking.egg-info/top_level.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       38 2023-04-11 19:58:12.464451 deep_tracking-1.0.2/setup.cfg
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      772 2023-04-11 19:57:54.000000 deep_tracking-1.0.2/setup.py
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 20:10:00.014168 deep_tracking-1.0.3/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     1085 2023-04-11 19:33:15.000000 deep_tracking-1.0.3/LICENCE.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-11 20:10:00.014168 deep_tracking-1.0.3/PKG-INFO
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      429 2023-04-04 11:20:37.000000 deep_tracking-1.0.3/README.md
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 20:10:00.010168 deep_tracking-1.0.3/deep_tracking/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       34 2023-04-11 20:09:29.000000 deep_tracking-1.0.3/deep_tracking/__init__.py
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     9923 2023-04-11 19:54:01.000000 deep_tracking-1.0.3/deep_tracking/deep_tracking.py
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 20:10:00.010168 deep_tracking-1.0.3/deep_tracking.egg-info/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-11 20:09:59.000000 deep_tracking-1.0.3/deep_tracking.egg-info/PKG-INFO
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      271 2023-04-11 20:09:59.000000 deep_tracking-1.0.3/deep_tracking.egg-info/SOURCES.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)        1 2023-04-11 20:09:59.000000 deep_tracking-1.0.3/deep_tracking.egg-info/dependency_links.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-11 20:09:59.000000 deep_tracking-1.0.3/deep_tracking.egg-info/requires.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-11 20:09:59.000000 deep_tracking-1.0.3/deep_tracking.egg-info/top_level.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       38 2023-04-11 20:10:00.014168 deep_tracking-1.0.3/setup.cfg
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      772 2023-04-11 20:09:50.000000 deep_tracking-1.0.3/setup.py
```

### Comparing `deep_tracking-1.0.2/LICENCE.txt` & `deep_tracking-1.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `deep_tracking-1.0.2/PKG-INFO` & `deep_tracking-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep_tracking
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to track the development of data science works using the DE&P method
 Home-page: https://github.com/biazotogabriel/deep_tracking
 Author: Gabriel Nuernberg Biazoto
 Author-email: biazotogabriel@gmail.com
 License: MIT
 Keywords: deep de&p data science
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deep_tracking-1.0.2/deep_tracking/deep_tracking.py` & `deep_tracking-1.0.3/deep_tracking/deep_tracking.py`

 * *Files identical despite different names*

### Comparing `deep_tracking-1.0.2/deep_tracking.egg-info/PKG-INFO` & `deep_tracking-1.0.3/deep_tracking.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-tracking
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to track the development of data science works using the DE&P method
 Home-page: https://github.com/biazotogabriel/deep_tracking
 Author: Gabriel Nuernberg Biazoto
 Author-email: biazotogabriel@gmail.com
 License: MIT
 Keywords: deep de&p data science
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deep_tracking-1.0.2/setup.py` & `deep_tracking-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='deep_tracking',
-    version='1.0.2',
+    version='1.0.3',
     description='Library to track the development of data science works using the DE&P method',
     long_description = 'Library to track the development of data science works using the DE&P method',
     author='Gabriel Nuernberg Biazoto',
     author_email='biazotogabriel@gmail.com',
     url='https://github.com/biazotogabriel/deep_tracking',
     packages=['deep_tracking'],
     license = 'MIT',
```

