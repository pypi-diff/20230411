# Comparing `tmp/proxy-decorator-0.1.0.tar.gz` & `tmp/proxy-decorator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxy-decorator-0.1.0.tar", last modified: Tue Apr 11 07:54:49 2023, max compression
+gzip compressed data, was "proxy-decorator-0.1.1.tar", last modified: Tue Apr 11 08:08:30 2023, max compression
```

## Comparing `proxy-decorator-0.1.0.tar` & `proxy-decorator-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 07:54:49.822299 proxy-decorator-0.1.0/
--rw-rw-rw-   0        0        0      356 2023-04-11 07:54:49.820299 proxy-decorator-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 07:54:49.818303 proxy-decorator-0.1.0/proxy_decorator.egg-info/
--rw-rw-rw-   0        0        0      356 2023-04-11 07:54:49.000000 proxy-decorator-0.1.0/proxy_decorator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-11 07:54:49.000000 proxy-decorator-0.1.0/proxy_decorator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 07:54:49.000000 proxy-decorator-0.1.0/proxy_decorator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 07:54:49.000000 proxy-decorator-0.1.0/proxy_decorator.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 07:54:49.000000 proxy-decorator-0.1.0/proxy_decorator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 07:54:49.822299 proxy-decorator-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      542 2023-04-11 07:54:42.000000 proxy-decorator-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:08:30.939415 proxy-decorator-0.1.1/
+-rw-rw-rw-   0        0        0      352 2023-04-11 08:08:30.937420 proxy-decorator-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 08:08:30.935414 proxy-decorator-0.1.1/proxy_decorator.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-04-11 08:08:30.000000 proxy-decorator-0.1.1/proxy_decorator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-04-11 08:08:30.000000 proxy-decorator-0.1.1/proxy_decorator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 08:08:30.000000 proxy-decorator-0.1.1/proxy_decorator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 08:08:30.000000 proxy-decorator-0.1.1/proxy_decorator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 08:08:30.000000 proxy-decorator-0.1.1/proxy_decorator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 08:08:30.939415 proxy-decorator-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      538 2023-04-11 08:08:25.000000 proxy-decorator-0.1.1/setup.py
```

### Comparing `proxy-decorator-0.1.0/setup.py` & `proxy-decorator-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="proxy-decorator",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
         "configparser",
     ],
-    python_requires=">=3.6, <4",
+    python_requires=">=3.6",
     author="joe_zhouman",
     author_email="man.man.man.man.a@gmail.com",
     description="A simple proxy decorator for Python functions",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3"
```

