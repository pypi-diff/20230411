# Comparing `tmp/quanturf_blankly-0.3.tar.gz` & `tmp/quanturf_blankly-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quanturf_blankly-0.3.tar", last modified: Tue Apr 11 13:04:01 2023, max compression
+gzip compressed data, was "quanturf_blankly-0.4.tar", last modified: Tue Apr 11 13:34:06 2023, max compression
```

## Comparing `quanturf_blankly-0.3.tar` & `quanturf_blankly-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 13:04:01.621995 quanturf_blankly-0.3/
--rw-rw-rw-   0        0        0      577 2023-04-11 13:04:01.621012 quanturf_blankly-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 13:04:01.572987 quanturf_blankly-0.3/quanturf_blankly/
--rw-rw-rw-   0        0        0        0 2023-03-21 18:01:57.000000 quanturf_blankly-0.3/quanturf_blankly/__init__.py
--rw-rw-rw-   0        0        0    14719 2023-04-10 19:46:29.000000 quanturf_blankly-0.3/quanturf_blankly/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:04:01.619986 quanturf_blankly-0.3/quanturf_blankly.egg-info/
--rw-rw-rw-   0        0        0      577 2023-04-11 13:04:01.000000 quanturf_blankly-0.3/quanturf_blankly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-04-11 13:04:01.000000 quanturf_blankly-0.3/quanturf_blankly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 13:04:01.000000 quanturf_blankly-0.3/quanturf_blankly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-11 13:04:01.000000 quanturf_blankly-0.3/quanturf_blankly.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       58 2023-04-11 13:04:01.000000 quanturf_blankly-0.3/quanturf_blankly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-11 13:04:01.000000 quanturf_blankly-0.3/quanturf_blankly.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 13:04:01.621995 quanturf_blankly-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-04-11 13:03:32.000000 quanturf_blankly-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:34:06.065414 quanturf_blankly-0.4/
+-rw-rw-rw-   0        0        0      509 2023-04-11 13:34:06.063426 quanturf_blankly-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 13:34:06.048442 quanturf_blankly-0.4/quanturf_blankly/
+-rw-rw-rw-   0        0        0        0 2023-03-21 18:01:57.000000 quanturf_blankly-0.4/quanturf_blankly/__init__.py
+-rw-rw-rw-   0        0        0    14719 2023-04-10 19:46:29.000000 quanturf_blankly-0.4/quanturf_blankly/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:34:06.058444 quanturf_blankly-0.4/quanturf_blankly.egg-info/
+-rw-rw-rw-   0        0        0      509 2023-04-11 13:34:05.000000 quanturf_blankly-0.4/quanturf_blankly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-04-11 13:34:05.000000 quanturf_blankly-0.4/quanturf_blankly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 13:34:05.000000 quanturf_blankly-0.4/quanturf_blankly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-11 13:34:05.000000 quanturf_blankly-0.4/quanturf_blankly.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       58 2023-04-11 13:34:05.000000 quanturf_blankly-0.4/quanturf_blankly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-11 13:34:05.000000 quanturf_blankly-0.4/quanturf_blankly.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 13:34:06.065414 quanturf_blankly-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2023-04-11 13:33:54.000000 quanturf_blankly-0.4/setup.py
```

### Comparing `quanturf_blankly-0.3/quanturf_blankly/__main__.py` & `quanturf_blankly-0.4/quanturf_blankly/__main__.py`

 * *Files identical despite different names*

### Comparing `quanturf_blankly-0.3/setup.py` & `quanturf_blankly-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import sys
 
 setup_args=dict(
     name="quanturf_blankly",
     packages=['quanturf_blankly'],
-    version='0.3',
+    version='0.4',
     description="",
     long_description="",
     author="Quanturf",
     url="https://github.com/Quanturf/quanturf_blankly_package",
     author_email="quanturf.finance@gmail.com",
     classifiers=[
         'Intended Audience :: Developers',
```

