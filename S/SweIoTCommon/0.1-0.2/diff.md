# Comparing `tmp/SweIoTCommon-0.1.tar.gz` & `tmp/SweIoTCommon-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SweIoTCommon-0.1.tar", last modified: Tue Apr 11 16:44:02 2023, max compression
+gzip compressed data, was "SweIoTCommon-0.2.tar", last modified: Tue Apr 11 19:55:16 2023, max compression
```

## Comparing `SweIoTCommon-0.1.tar` & `SweIoTCommon-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 16:44:02.185914 SweIoTCommon-0.1/
--rw-rw-rw-   0        0        0      336 2023-04-11 16:44:02.183913 SweIoTCommon-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 16:44:02.181913 SweIoTCommon-0.1/SweIoTCommon.egg-info/
--rw-rw-rw-   0        0        0      336 2023-04-11 16:44:02.000000 SweIoTCommon-0.1/SweIoTCommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-04-11 16:44:02.000000 SweIoTCommon-0.1/SweIoTCommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 16:44:02.000000 SweIoTCommon-0.1/SweIoTCommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1152 2023-04-11 16:44:02.000000 SweIoTCommon-0.1/SweIoTCommon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 16:44:02.000000 SweIoTCommon-0.1/SweIoTCommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 16:44:02.185914 SweIoTCommon-0.1/setup.cfg
--rw-rw-rw-   0        0        0      578 2023-04-11 16:37:26.000000 SweIoTCommon-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:55:16.643483 SweIoTCommon-0.2/
+-rw-rw-rw-   0        0        0      336 2023-04-11 19:55:16.642484 SweIoTCommon-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 19:55:16.640484 SweIoTCommon-0.2/SweIoTCommon.egg-info/
+-rw-rw-rw-   0        0        0      336 2023-04-11 19:55:16.000000 SweIoTCommon-0.2/SweIoTCommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-04-11 19:55:16.000000 SweIoTCommon-0.2/SweIoTCommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 19:55:16.000000 SweIoTCommon-0.2/SweIoTCommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-04-11 19:55:16.000000 SweIoTCommon-0.2/SweIoTCommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 19:55:16.000000 SweIoTCommon-0.2/SweIoTCommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 19:55:16.643483 SweIoTCommon-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      599 2023-04-11 19:47:55.000000 SweIoTCommon-0.2/setup.py
```

### Comparing `SweIoTCommon-0.1/setup.py` & `SweIoTCommon-0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='SweIoTCommon',
-    version='0.1',
-    packages=find_packages(),
+    version='0.2',
+    packages=find_packages(exclude=['MyPackage']),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
         'Programming Language :: Python :: 3',
```

