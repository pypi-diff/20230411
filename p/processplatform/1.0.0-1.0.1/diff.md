# Comparing `tmp/processplatform-1.0.0.tar.gz` & `tmp/processplatform-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processplatform-1.0.0.tar", last modified: Mon Apr 10 23:01:04 2023, max compression
+gzip compressed data, was "processplatform-1.0.1.tar", last modified: Tue Apr 11 00:05:19 2023, max compression
```

## Comparing `processplatform-1.0.0.tar` & `processplatform-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 23:01:04.158756 processplatform-1.0.0/
--rw-rw-rw-   0        0        0      595 2023-04-10 23:01:04.156802 processplatform-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 23:01:04.155825 processplatform-1.0.0/processplatform.egg-info/
--rw-rw-rw-   0        0        0      595 2023-04-10 23:01:03.000000 processplatform-1.0.0/processplatform.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      164 2023-04-10 23:01:03.000000 processplatform-1.0.0/processplatform.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 23:01:03.000000 processplatform-1.0.0/processplatform.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 23:01:03.000000 processplatform-1.0.0/processplatform.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 23:01:04.159733 processplatform-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      716 2023-04-10 22:51:23.000000 processplatform-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:05:19.951251 processplatform-1.0.1/
+-rw-rw-rw-   0        0        0      595 2023-04-11 00:05:19.950274 processplatform-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 00:05:19.943434 processplatform-1.0.1/processplatform/
+-rw-rw-rw-   0        0        0     1096 2023-04-11 00:04:57.000000 processplatform-1.0.1/processplatform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:05:19.949297 processplatform-1.0.1/processplatform.egg-info/
+-rw-rw-rw-   0        0        0      595 2023-04-11 00:05:19.000000 processplatform-1.0.1/processplatform.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-11 00:05:19.000000 processplatform-1.0.1/processplatform.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 00:05:19.000000 processplatform-1.0.1/processplatform.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-11 00:05:19.000000 processplatform-1.0.1/processplatform.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 00:05:19.951251 processplatform-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      716 2023-04-11 00:05:05.000000 processplatform-1.0.1/setup.py
```

### Comparing `processplatform-1.0.0/PKG-INFO` & `processplatform-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: processplatform
-Version: 1.0.0
+Version: 1.0.1
 Summary: Computer process information
 Home-page: https://google.com
 Author: vesper
 Author-email: google@gmail.com
 License: MIT
 Description: Get any computer information or python plugins path with a simple get command.
 Keywords: process
```

### Comparing `processplatform-1.0.0/processplatform.egg-info/PKG-INFO` & `processplatform-1.0.1/processplatform.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: processplatform
-Version: 1.0.0
+Version: 1.0.1
 Summary: Computer process information
 Home-page: https://google.com
 Author: vesper
 Author-email: google@gmail.com
 License: MIT
 Description: Get any computer information or python plugins path with a simple get command.
 Keywords: process
```

### Comparing `processplatform-1.0.0/setup.py` & `processplatform-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='processplatform',
-  version='1.0.0',
+  version='1.0.1',
   description='Computer process information',
   long_description="Get any computer information or python plugins path with a simple get command.",
   url='https://google.com',
   author='vesper',
   author_email='google@gmail.com',
   license='MIT',
   classifiers=classifiers,
```

