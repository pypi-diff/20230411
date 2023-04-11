# Comparing `tmp/chunked-uploads-attentive-0.0.2.tar.gz` & `tmp/chunked-uploads-attentive-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chunked-uploads-attentive-0.0.2.tar", last modified: Mon Apr 10 10:31:39 2023, max compression
+gzip compressed data, was "chunked-uploads-attentive-0.0.3.tar", last modified: Tue Apr 11 16:43:36 2023, max compression
```

## Comparing `chunked-uploads-attentive-0.0.2.tar` & `chunked-uploads-attentive-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 10:31:39.836020 chunked-uploads-attentive-0.0.2/
--rw-rw-rw-   0        0        0      583 2023-04-10 10:31:39.835019 chunked-uploads-attentive-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 10:31:39.834033 chunked-uploads-attentive-0.0.2/chunked_uploads_attentive.egg-info/
--rw-rw-rw-   0        0        0      583 2023-04-10 10:31:39.000000 chunked-uploads-attentive-0.0.2/chunked_uploads_attentive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-04-10 10:31:39.000000 chunked-uploads-attentive-0.0.2/chunked_uploads_attentive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 10:31:39.000000 chunked-uploads-attentive-0.0.2/chunked_uploads_attentive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-10 10:31:39.000000 chunked-uploads-attentive-0.0.2/chunked_uploads_attentive.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 10:31:39.000000 chunked-uploads-attentive-0.0.2/chunked_uploads_attentive.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 10:31:39.836020 chunked-uploads-attentive-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      940 2023-04-10 10:30:31.000000 chunked-uploads-attentive-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 16:43:36.987466 chunked-uploads-attentive-0.0.3/
+-rw-rw-rw-   0        0        0      478 2023-04-11 16:43:36.987466 chunked-uploads-attentive-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-11 16:43:36.988550 chunked-uploads-attentive-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      901 2023-04-11 16:43:33.000000 chunked-uploads-attentive-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 16:43:36.926297 chunked-uploads-attentive-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 16:43:36.957567 chunked-uploads-attentive-0.0.3/src/chunked_uploads/
+-rw-rw-rw-   0        0        0        0 2023-03-21 15:09:06.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads/__init__.py
+-rw-rw-rw-   0        0        0      325 2023-03-21 15:15:16.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads/admin.py
+-rw-rw-rw-   0        0        0      152 2023-03-21 15:09:06.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads/apps.py
+-rw-rw-rw-   0        0        0      301 2023-02-16 16:23:12.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads/constants.py
+-rw-rw-rw-   0        0        0      262 2023-02-13 12:36:18.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads/exceptions.py
+-rw-rw-rw-   0        0        0     3879 2023-03-31 07:05:44.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads/models.py
+-rw-rw-rw-   0        0        0      376 2023-02-13 12:36:18.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads/response.py
+-rw-rw-rw-   0        0        0      570 2023-03-21 15:17:55.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads/serializers.py
+-rw-rw-rw-   0        0        0     2334 2023-03-21 15:10:53.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads/settings.py
+-rw-rw-rw-   0        0        0       63 2023-03-21 15:09:06.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads/tests.py
+-rw-rw-rw-   0        0        0    18287 2023-03-31 07:10:24.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads/views.py
+drwxrwxrwx   0        0        0        0 2023-04-11 16:43:36.973144 chunked-uploads-attentive-0.0.3/src/chunked_uploads_attentive.egg-info/
+-rw-rw-rw-   0        0        0      478 2023-04-11 16:43:36.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads_attentive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2023-04-11 16:43:36.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads_attentive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 16:43:36.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads_attentive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-11 16:43:36.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads_attentive.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-11 16:43:36.000000 chunked-uploads-attentive-0.0.3/src/chunked_uploads_attentive.egg-info/top_level.txt
```

### Comparing `chunked-uploads-attentive-0.0.2/setup.py` & `chunked-uploads-attentive-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Chunked Upload of files on gcs using Django'
 LONG_DESCRIPTION = 'A package that allows to transfer files and resume in case of data failure'
 
 # Setting up
 setup(
     name="chunked-uploads-attentive",
     version=VERSION,
     author="Ayion",
     author_email="<ayan@attentive.ai>",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=LONG_DESCRIPTION,
-    packages=find_packages(),
+    package_dir={'':'src'},
+    packages=['chunked_uploads'],
     install_requires=['django', 'djangorestframework'],
     keywords=['python', 'file', 'transfer', 'chunk', 'chunks', 'upload'],
+    license='MIT',
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
```

