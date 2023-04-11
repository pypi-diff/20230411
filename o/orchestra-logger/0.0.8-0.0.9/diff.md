# Comparing `tmp/orchestra-logger-0.0.8.tar.gz` & `tmp/orchestra-logger-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestra-logger-0.0.8.tar", last modified: Sat Apr  8 22:42:47 2023, max compression
+gzip compressed data, was "dist\orchestra-logger-0.0.9.tar", last modified: Tue Apr 11 20:05:40 2023, max compression
```

## Comparing `orchestra-logger-0.0.8.tar` & `orchestra-logger-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 22:42:47.952741 orchestra-logger-0.0.8/
--rw-rw-rw-   0        0        0     1098 2023-04-08 22:02:33.000000 orchestra-logger-0.0.8/LICENSE.gitignore
--rw-rw-rw-   0        0        0      711 2023-04-08 22:42:47.952741 orchestra-logger-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-04-08 11:40:32.000000 orchestra-logger-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 22:42:47.921756 orchestra-logger-0.0.8/orchestra_logger/
--rw-rw-rw-   0        0        0       70 2023-04-08 22:38:50.000000 orchestra-logger-0.0.8/orchestra_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 22:42:47.951748 orchestra-logger-0.0.8/orchestra_logger/orclogger/
--rw-rw-rw-   0        0        0        0 2023-04-08 11:57:19.000000 orchestra-logger-0.0.8/orchestra_logger/orclogger/__init__.py
--rw-rw-rw-   0        0        0     1582 2023-04-08 21:40:40.000000 orchestra-logger-0.0.8/orchestra_logger/orclogger/orclogger.py
-drwxrwxrwx   0        0        0        0 2023-04-08 22:42:47.946487 orchestra-logger-0.0.8/orchestra_logger.egg-info/
--rw-rw-rw-   0        0        0      711 2023-04-08 22:42:47.000000 orchestra-logger-0.0.8/orchestra_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-04-08 22:42:47.000000 orchestra-logger-0.0.8/orchestra_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 22:42:47.000000 orchestra-logger-0.0.8/orchestra_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-08 22:42:47.000000 orchestra-logger-0.0.8/orchestra_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-08 22:42:47.956569 orchestra-logger-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1396 2023-04-08 22:42:22.000000 orchestra-logger-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:05:40.680895 orchestra-logger-0.0.9/
+-rw-rw-rw-   0        0        0     1098 2023-04-11 19:42:58.000000 orchestra-logger-0.0.9/LICENSE.gitignore
+-rw-rw-rw-   0        0        0     5870 2023-04-11 20:05:40.681921 orchestra-logger-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5121 2023-04-11 19:42:58.000000 orchestra-logger-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 20:05:40.622332 orchestra-logger-0.0.9/orchestra_logger/
+-rw-rw-rw-   0        0        0       70 2023-04-11 19:42:58.000000 orchestra-logger-0.0.9/orchestra_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:05:40.659693 orchestra-logger-0.0.9/orchestra_logger/example/
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:42:58.000000 orchestra-logger-0.0.9/orchestra_logger/example/__init__.py
+-rw-rw-rw-   0        0        0      629 2023-04-11 19:42:58.000000 orchestra-logger-0.0.9/orchestra_logger/example/example.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:05:40.676478 orchestra-logger-0.0.9/orchestra_logger/orclogger/
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:42:58.000000 orchestra-logger-0.0.9/orchestra_logger/orclogger/__init__.py
+-rw-rw-rw-   0        0        0     1590 2023-04-11 19:54:29.000000 orchestra-logger-0.0.9/orchestra_logger/orclogger/orclogger.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:05:40.678632 orchestra-logger-0.0.9/orchestra_logger/services/
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:42:58.000000 orchestra-logger-0.0.9/orchestra_logger/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:05:40.647390 orchestra-logger-0.0.9/orchestra_logger.egg-info/
+-rw-rw-rw-   0        0        0     5870 2023-04-11 20:05:40.000000 orchestra-logger-0.0.9/orchestra_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-04-11 20:05:40.000000 orchestra-logger-0.0.9/orchestra_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 20:05:40.000000 orchestra-logger-0.0.9/orchestra_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-11 20:05:40.000000 orchestra-logger-0.0.9/orchestra_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-11 20:05:40.684970 orchestra-logger-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1248 2023-04-11 20:02:09.000000 orchestra-logger-0.0.9/setup.py
```

### Comparing `orchestra-logger-0.0.8/LICENSE.gitignore` & `orchestra-logger-0.0.9/LICENSE.gitignore`

 * *Files identical despite different names*

### Comparing `orchestra-logger-0.0.8/orchestra_logger/orclogger/orclogger.py` & `orchestra-logger-0.0.9/orchestra_logger/orclogger/orclogger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import sys
 import logging
-import inspect
-from src.services.orcProcess import orcProcess
+from orchestra_logger.services.orcProcess.orcProcess import orcProcess
 
 class orcLogger():
     def __init__(self, name=""):
         self.name = name
 
 class httpClient():
     def __init__(self, baseUrl):
```

### Comparing `orchestra-logger-0.0.8/setup.py` & `orchestra-logger-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
+    long_description__ = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Logging module to enable orchestration on self-hosted applications'
-LONG_DESCRIPTION = 'A logging-like module to be implemented on self-hosted applications that allows Orchestra to coordinate tasks and gather metadata'
 
 # Setting up
 setup(
     name="orchestra-logger",
     version=VERSION,
     author="Orchestra (Hugo Lu)",
     author_email="<hugo@getorchestra.io>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
-    long_description=long_description,
+    long_description=long_description__,
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'logging', 'data', 'orchestration'],
     classifiers=[
         'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',      # Define that your audience are developers
         'Topic :: Software Development :: Build Tools',
```

