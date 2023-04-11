# Comparing `tmp/pylibcrypto-1.0.0.tar.gz` & `tmp/pylibcrypto-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibcrypto-1.0.0.tar", last modified: Mon Apr 10 22:56:11 2023, max compression
+gzip compressed data, was "pylibcrypto-1.2.0.tar", last modified: Tue Apr 11 16:56:45 2023, max compression
```

## Comparing `pylibcrypto-1.0.0.tar` & `pylibcrypto-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 22:56:11.716916 pylibcrypto-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-10 22:56:11.716916 pylibcrypto-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 22:56:11.716916 pylibcrypto-1.0.0/pylibcrypto/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 22:56:11.000000 pylibcrypto-1.0.0/pylibcrypto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 22:56:11.716916 pylibcrypto-1.0.0/pylibcrypto.egg-info/
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-10 22:56:11.000000 pylibcrypto-1.0.0/pylibcrypto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-10 22:56:11.000000 pylibcrypto-1.0.0/pylibcrypto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 22:56:11.000000 pylibcrypto-1.0.0/pylibcrypto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-10 22:56:11.000000 pylibcrypto-1.0.0/pylibcrypto.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 22:56:11.716916 pylibcrypto-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      531 2023-04-10 22:56:10.000000 pylibcrypto-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:56:45.664989 pylibcrypto-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      395 2023-04-11 16:56:45.664989 pylibcrypto-1.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:56:45.664989 pylibcrypto-1.2.0/pylibcrypto/
+-rw-r--r--   0 root         (0) root         (0)    70957 2023-04-11 16:56:45.000000 pylibcrypto-1.2.0/pylibcrypto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:56:45.664989 pylibcrypto-1.2.0/pylibcrypto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      395 2023-04-11 16:56:45.000000 pylibcrypto-1.2.0/pylibcrypto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-11 16:56:45.000000 pylibcrypto-1.2.0/pylibcrypto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 16:56:45.000000 pylibcrypto-1.2.0/pylibcrypto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-11 16:56:45.000000 pylibcrypto-1.2.0/pylibcrypto.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 16:56:45.664989 pylibcrypto-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      608 2023-04-11 16:56:44.000000 pylibcrypto-1.2.0/setup.py
```

### Comparing `pylibcrypto-1.0.0/setup.py` & `pylibcrypto-1.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
-DESCRIPTION = "Hello World"
-LONG_DESCRIPTION = "Hello World"
+VERSION = '1.2.0'
+DESCRIPTION = "Libary used for various cryptographic algorythmus"
+LONG_DESCRIPTION = "Libary used for various cryptographic algorythmus"
 
 # Setting up
 setup(
     name="pylibcrypto",
     version=VERSION,
-    author="SuSB0t",
+    author="NHJonas",
     author_email="nick.faltermeier@gmx.de",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python'],
```

