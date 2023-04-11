# Comparing `tmp/quanturf_blankly-0.1.tar.gz` & `tmp/quanturf_blankly-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quanturf_blankly-0.1.tar", last modified: Tue Apr 11 12:46:17 2023, max compression
+gzip compressed data, was "quanturf_blankly-0.2.tar", last modified: Tue Apr 11 12:50:33 2023, max compression
```

## Comparing `quanturf_blankly-0.1.tar` & `quanturf_blankly-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 12:46:17.677520 quanturf_blankly-0.1/
--rw-rw-rw-   0        0        0      254 2023-04-11 12:46:17.676522 quanturf_blankly-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 12:46:17.460521 quanturf_blankly-0.1/quanturf_blankly/
--rw-rw-rw-   0        0        0        0 2023-03-21 18:01:57.000000 quanturf_blankly-0.1/quanturf_blankly/__init__.py
--rw-rw-rw-   0        0        0    14719 2023-04-10 19:46:29.000000 quanturf_blankly-0.1/quanturf_blankly/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:46:17.675524 quanturf_blankly-0.1/quanturf_blankly.egg-info/
--rw-rw-rw-   0        0        0      254 2023-04-11 12:46:14.000000 quanturf_blankly-0.1/quanturf_blankly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-04-11 12:46:15.000000 quanturf_blankly-0.1/quanturf_blankly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 12:46:14.000000 quanturf_blankly-0.1/quanturf_blankly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-11 12:46:14.000000 quanturf_blankly-0.1/quanturf_blankly.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2023-04-11 12:46:14.000000 quanturf_blankly-0.1/quanturf_blankly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-11 12:46:14.000000 quanturf_blankly-0.1/quanturf_blankly.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 12:46:17.677520 quanturf_blankly-0.1/setup.cfg
--rw-rw-rw-   0        0        0      726 2023-04-09 09:56:36.000000 quanturf_blankly-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:50:33.238899 quanturf_blankly-0.2/
+-rw-rw-rw-   0        0        0      254 2023-04-11 12:50:33.227883 quanturf_blankly-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 12:50:33.194883 quanturf_blankly-0.2/quanturf_blankly/
+-rw-rw-rw-   0        0        0        0 2023-03-21 18:01:57.000000 quanturf_blankly-0.2/quanturf_blankly/__init__.py
+-rw-rw-rw-   0        0        0    14719 2023-04-10 19:46:29.000000 quanturf_blankly-0.2/quanturf_blankly/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:50:33.205917 quanturf_blankly-0.2/quanturf_blankly.egg-info/
+-rw-rw-rw-   0        0        0      254 2023-04-11 12:50:33.000000 quanturf_blankly-0.2/quanturf_blankly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-04-11 12:50:33.000000 quanturf_blankly-0.2/quanturf_blankly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 12:50:33.000000 quanturf_blankly-0.2/quanturf_blankly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-11 12:50:33.000000 quanturf_blankly-0.2/quanturf_blankly.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2023-04-11 12:50:33.000000 quanturf_blankly-0.2/quanturf_blankly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-11 12:50:33.000000 quanturf_blankly-0.2/quanturf_blankly.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 12:50:33.239908 quanturf_blankly-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      714 2023-04-11 12:50:21.000000 quanturf_blankly-0.2/setup.py
```

### Comparing `quanturf_blankly-0.1/quanturf_blankly/__main__.py` & `quanturf_blankly-0.2/quanturf_blankly/__main__.py`

 * *Files identical despite different names*

### Comparing `quanturf_blankly-0.1/setup.py` & `quanturf_blankly-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup
 import sys
 
 setup_args=dict(
     name="quanturf_blankly",
     packages=['quanturf_blankly'],
-    version='0.1',
+    version='0.2',
     description="",
     long_description="",
     author="Quanturf",
     url="https://github.com/Quanturf/quanturf_blankly_package",
     author_email="quanturf.finance@gmail.com",
       entry_points={
         "console_scripts": [
             "myscript = quanturf_blankly.__main__:main",
         ]
     } 
 )
 
 if 'setuptools' in sys.modules:
     setup_args['install_requires'] = install_requires = [
-        "blankly","apscheduler","threading","alpaca_trade_api","pandas","numpy"
+        "blankly","apscheduler","alpaca_trade_api","pandas","numpy"
     ]
 
 def main():
     setup(**setup_args)
 
 if __name__ == '__main__':
     main()
```

