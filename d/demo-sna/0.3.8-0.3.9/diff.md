# Comparing `tmp/demo_sna-0.3.8.tar.gz` & `tmp/demo_sna-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demo_sna-0.3.8.tar", last modified: Tue Apr 11 20:07:11 2023, max compression
+gzip compressed data, was "demo_sna-0.3.9.tar", last modified: Tue Apr 11 20:18:17 2023, max compression
```

## Comparing `demo_sna-0.3.8.tar` & `demo_sna-0.3.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 20:07:11.759592 demo_sna-0.3.8/
--rw-rw-rw-   0        0        0      172 2023-03-28 19:17:05.000000 demo_sna-0.3.8/AUTHORS.rst
--rw-rw-rw-   0        0        0     1091 2023-03-28 19:17:05.000000 demo_sna-0.3.8/LICENSE
--rw-rw-rw-   0        0        0      820 2023-04-11 20:07:11.759592 demo_sna-0.3.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 20:07:11.750792 demo_sna-0.3.8/demo_sna.egg-info/
--rw-rw-rw-   0        0        0       19 2023-04-11 20:07:11.000000 demo_sna-0.3.8/demo_sna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 20:07:11.759592 demo_sna-0.3.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 20:18:17.837920 demo_sna-0.3.9/
+-rw-rw-rw-   0        0        0      172 2023-03-28 19:17:05.000000 demo_sna-0.3.9/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1091 2023-03-28 19:17:05.000000 demo_sna-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0      820 2023-04-11 20:18:17.837920 demo_sna-0.3.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 20:18:17.835417 demo_sna-0.3.9/demo_sna.egg-info/
+-rw-rw-rw-   0        0        0       19 2023-04-11 20:18:17.000000 demo_sna-0.3.9/demo_sna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 20:18:17.837920 demo_sna-0.3.9/setup.cfg
```

### Comparing `demo_sna-0.3.8/LICENSE` & `demo_sna-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `demo_sna-0.3.8/PKG-INFO` & `demo_sna-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demo_sna
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/demo
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: demo_sna
 Classifier: Development Status :: 2 - Pre-Alpha
```

