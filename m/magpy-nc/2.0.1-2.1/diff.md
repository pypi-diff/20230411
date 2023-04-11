# Comparing `tmp/magpy_nc-2.0.1.tar.gz` & `tmp/magpy_nc-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magpy_nc-2.0.1.tar", last modified: Tue Apr 11 08:57:47 2023, max compression
+gzip compressed data, was "magpy_nc-2.1.tar", last modified: Tue Apr 11 05:48:20 2023, max compression
```

## Comparing `magpy_nc-2.0.1.tar` & `magpy_nc-2.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 08:57:47.466683 magpy_nc-2.0.1/
--rw-rw-rw-   0        0        0     1102 2023-04-11 00:10:27.000000 magpy_nc-2.0.1/LICENCE
--rw-rw-rw-   0        0        0      169 2023-04-11 08:57:47.466683 magpy_nc-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2204 2023-04-11 08:55:05.000000 magpy_nc-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 08:57:47.465686 magpy_nc-2.0.1/magpy_nc.egg-info/
--rw-rw-rw-   0        0        0      169 2023-04-11 08:57:47.000000 magpy_nc-2.0.1/magpy_nc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-04-11 08:57:47.000000 magpy_nc-2.0.1/magpy_nc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 08:57:47.000000 magpy_nc-2.0.1/magpy_nc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-11 08:57:47.000000 magpy_nc-2.0.1/magpy_nc.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1935 2023-04-11 08:48:09.000000 magpy_nc-2.0.1/magpy_nc.egg-info/test_app.py
--rw-rw-rw-   0        0        0        1 2023-04-11 08:57:47.000000 magpy_nc-2.0.1/magpy_nc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 08:57:47.466683 magpy_nc-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      334 2023-04-11 08:57:41.000000 magpy_nc-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:48:20.272127 magpy_nc-2.1/
+-rw-rw-rw-   0        0        0     1102 2023-04-11 00:10:27.000000 magpy_nc-2.1/LICENCE
+-rw-rw-rw-   0        0        0      167 2023-04-11 05:48:20.272127 magpy_nc-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2023-04-11 05:36:11.000000 magpy_nc-2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 05:48:20.271131 magpy_nc-2.1/magpy_nc.egg-info/
+-rw-rw-rw-   0        0        0      167 2023-04-11 05:48:20.000000 magpy_nc-2.1/magpy_nc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-04-11 05:48:20.000000 magpy_nc-2.1/magpy_nc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 05:48:20.000000 magpy_nc-2.1/magpy_nc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-11 05:48:20.000000 magpy_nc-2.1/magpy_nc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 05:48:20.000000 magpy_nc-2.1/magpy_nc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 05:48:20.272127 magpy_nc-2.1/setup.cfg
+-rw-rw-rw-   0        0        0      332 2023-04-11 05:47:05.000000 magpy_nc-2.1/setup.py
```

### Comparing `magpy_nc-2.0.1/LICENCE` & `magpy_nc-2.1/LICENCE`

 * *Files identical despite different names*

