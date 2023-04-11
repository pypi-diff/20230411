# Comparing `tmp/IOTCommon-0.1.1.tar.gz` & `tmp/IOTCommon-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IOTCommon-0.1.1.tar", last modified: Tue Apr 11 21:02:10 2023, max compression
+gzip compressed data, was "IOTCommon-0.1.2.tar", last modified: Tue Apr 11 21:36:21 2023, max compression
```

## Comparing `IOTCommon-0.1.1.tar` & `IOTCommon-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 21:02:10.631425 IOTCommon-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-04-11 21:02:10.617423 IOTCommon-0.1.1/IOTCommon/
--rw-rw-rw-   0        0        0     1654 2023-04-11 17:33:40.000000 IOTCommon-0.1.1/IOTCommon/DatabaseLayer.py
--rw-rw-rw-   0        0        0     6794 2023-04-11 17:33:00.000000 IOTCommon-0.1.1/IOTCommon/Operations.py
--rw-rw-rw-   0        0        0        0 2023-04-11 17:33:44.000000 IOTCommon-0.1.1/IOTCommon/__init__.py
--rw-rw-rw-   0        0        0     1335 2023-04-11 17:33:24.000000 IOTCommon-0.1.1/IOTCommon/helperhttps.py
-drwxrwxrwx   0        0        0        0 2023-04-11 21:02:10.629427 IOTCommon-0.1.1/IOTCommon.egg-info/
--rw-rw-rw-   0        0        0      335 2023-04-11 21:02:10.000000 IOTCommon-0.1.1/IOTCommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-04-11 21:02:10.000000 IOTCommon-0.1.1/IOTCommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 21:02:10.000000 IOTCommon-0.1.1/IOTCommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-04-11 21:02:10.000000 IOTCommon-0.1.1/IOTCommon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-11 21:02:10.000000 IOTCommon-0.1.1/IOTCommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      335 2023-04-11 21:02:10.630423 IOTCommon-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 IOTCommon-0.1.1/README.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 21:02:10.632425 IOTCommon-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      598 2023-04-11 21:01:57.000000 IOTCommon-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:36:21.121574 IOTCommon-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:36:21.105572 IOTCommon-0.1.2/IOTCommon/
+-rw-rw-rw-   0        0        0     1654 2023-04-11 17:33:40.000000 IOTCommon-0.1.2/IOTCommon/DatabaseLayer.py
+-rw-rw-rw-   0        0        0     6794 2023-04-11 17:33:00.000000 IOTCommon-0.1.2/IOTCommon/Operations.py
+-rw-rw-rw-   0        0        0      424 2023-04-11 21:34:03.000000 IOTCommon-0.1.2/IOTCommon/__init__.py
+-rw-rw-rw-   0        0        0     1335 2023-04-11 17:33:24.000000 IOTCommon-0.1.2/IOTCommon/helperhttps.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:36:21.119574 IOTCommon-0.1.2/IOTCommon.egg-info/
+-rw-rw-rw-   0        0        0      335 2023-04-11 21:36:21.000000 IOTCommon-0.1.2/IOTCommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-04-11 21:36:21.000000 IOTCommon-0.1.2/IOTCommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:36:21.000000 IOTCommon-0.1.2/IOTCommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-04-11 21:36:21.000000 IOTCommon-0.1.2/IOTCommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-11 21:36:21.000000 IOTCommon-0.1.2/IOTCommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      335 2023-04-11 21:36:21.120572 IOTCommon-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 IOTCommon-0.1.2/README.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 21:36:21.121574 IOTCommon-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      598 2023-04-11 21:36:05.000000 IOTCommon-0.1.2/setup.py
```

### Comparing `IOTCommon-0.1.1/IOTCommon/DatabaseLayer.py` & `IOTCommon-0.1.2/IOTCommon/DatabaseLayer.py`

 * *Files identical despite different names*

### Comparing `IOTCommon-0.1.1/IOTCommon/Operations.py` & `IOTCommon-0.1.2/IOTCommon/Operations.py`

 * *Files identical despite different names*

### Comparing `IOTCommon-0.1.1/IOTCommon/helperhttps.py` & `IOTCommon-0.1.2/IOTCommon/helperhttps.py`

 * *Files identical despite different names*

### Comparing `IOTCommon-0.1.1/setup.py` & `IOTCommon-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='IOTCommon',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(exclude=['MyPackage']),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
```

