# Comparing `tmp/magpy-nc-0.1.tar.gz` & `tmp/magpy-nc-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magpy-nc-0.1.tar", last modified: Tue Apr 11 05:34:07 2023, max compression
+gzip compressed data, was "magpy-nc-1.0.tar", last modified: Tue Apr 11 05:25:21 2023, max compression
```

## Comparing `magpy-nc-0.1.tar` & `magpy-nc-1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 05:34:07.436287 magpy-nc-0.1/
--rw-rw-rw-   0        0        0     1102 2023-04-11 00:10:27.000000 magpy-nc-0.1/LICENCE
--rw-rw-rw-   0        0        0      167 2023-04-11 05:34:07.435294 magpy-nc-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       38 2023-04-11 00:11:37.000000 magpy-nc-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 05:34:07.433298 magpy-nc-0.1/magpy_nc.egg-info/
--rw-rw-rw-   0        0        0      167 2023-04-11 05:34:07.000000 magpy-nc-0.1/magpy_nc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-04-11 05:34:07.000000 magpy-nc-0.1/magpy_nc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 05:34:07.000000 magpy-nc-0.1/magpy_nc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-11 05:34:07.000000 magpy-nc-0.1/magpy_nc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 05:34:07.000000 magpy-nc-0.1/magpy_nc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 05:34:07.436287 magpy-nc-0.1/setup.cfg
--rw-rw-rw-   0        0        0      332 2023-04-11 05:33:59.000000 magpy-nc-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:25:21.505180 magpy-nc-1.0/
+-rw-rw-rw-   0        0        0     1102 2023-04-11 00:10:27.000000 magpy-nc-1.0/LICENCE
+-rw-rw-rw-   0        0        0      163 2023-04-11 05:25:21.505180 magpy-nc-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2023-04-11 00:11:37.000000 magpy-nc-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 05:25:21.504036 magpy-nc-1.0/magpy_nc.egg-info/
+-rw-rw-rw-   0        0        0      163 2023-04-11 05:25:21.000000 magpy-nc-1.0/magpy_nc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-04-11 05:25:21.000000 magpy-nc-1.0/magpy_nc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 05:25:21.000000 magpy-nc-1.0/magpy_nc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-11 05:25:21.000000 magpy-nc-1.0/magpy_nc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 05:25:21.000000 magpy-nc-1.0/magpy_nc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 05:25:21.505180 magpy-nc-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      310 2023-04-11 05:25:05.000000 magpy-nc-1.0/setup.py
```

### Comparing `magpy-nc-0.1/LICENCE` & `magpy-nc-1.0/LICENCE`

 * *Files identical despite different names*

