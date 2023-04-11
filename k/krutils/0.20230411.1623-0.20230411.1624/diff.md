# Comparing `tmp/krutils-0.20230411.1623.tar.gz` & `tmp/krutils-0.20230411.1624.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230411.1623.tar", last modified: Tue Apr 11 07:23:19 2023, max compression
+gzip compressed data, was "krutils-0.20230411.1624.tar", last modified: Tue Apr 11 07:24:24 2023, max compression
```

## Comparing `krutils-0.20230411.1623.tar` & `krutils-0.20230411.1624.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 07:23:19.323120 krutils-0.20230411.1623/
--rw-rw-rw-   0        0        0      332 2023-04-11 07:23:19.271701 krutils-0.20230411.1623/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1623/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 07:23:19.024066 krutils-0.20230411.1623/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1623/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1623/krutils/CONST.py
--rw-rw-rw-   0        0        0       71 2023-04-11 07:23:09.000000 krutils-0.20230411.1623/krutils/__init__.py
--rw-rw-rw-   0        0        0     5485 2023-04-11 07:16:33.000000 krutils-0.20230411.1623/krutils/dbmgr.py
--rw-rw-rw-   0        0        0    33497 2023-04-11 05:51:26.000000 krutils-0.20230411.1623/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:23:19.239955 krutils-0.20230411.1623/krutils.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-11 07:23:18.000000 krutils-0.20230411.1623/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-11 07:23:18.000000 krutils-0.20230411.1623/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 07:23:18.000000 krutils-0.20230411.1623/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-11 07:23:18.000000 krutils-0.20230411.1623/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 07:23:18.000000 krutils-0.20230411.1623/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 07:23:19.324904 krutils-0.20230411.1623/setup.cfg
--rw-rw-rw-   0        0        0      664 2023-04-11 07:23:16.000000 krutils-0.20230411.1623/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:24:24.021708 krutils-0.20230411.1624/
+-rw-rw-rw-   0        0        0      332 2023-04-11 07:24:24.016898 krutils-0.20230411.1624/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1624/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 07:24:23.847590 krutils-0.20230411.1624/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1624/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1624/krutils/CONST.py
+-rw-rw-rw-   0        0        0       93 2023-04-11 07:24:11.000000 krutils-0.20230411.1624/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5485 2023-04-11 07:16:33.000000 krutils-0.20230411.1624/krutils/dbmgr.py
+-rw-rw-rw-   0        0        0    33497 2023-04-11 05:51:26.000000 krutils-0.20230411.1624/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:24:23.982991 krutils-0.20230411.1624/krutils.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-11 07:24:23.000000 krutils-0.20230411.1624/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-04-11 07:24:23.000000 krutils-0.20230411.1624/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 07:24:23.000000 krutils-0.20230411.1624/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-11 07:24:23.000000 krutils-0.20230411.1624/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 07:24:23.000000 krutils-0.20230411.1624/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 07:24:24.024096 krutils-0.20230411.1624/setup.cfg
+-rw-rw-rw-   0        0        0      664 2023-04-11 07:24:22.000000 krutils-0.20230411.1624/setup.py
```

### Comparing `krutils-0.20230411.1623/krutils/CONST.py` & `krutils-0.20230411.1624/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1623/krutils/dbmgr.py` & `krutils-0.20230411.1624/krutils/dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1623/krutils/utils.py` & `krutils-0.20230411.1624/krutils/utils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1623/setup.py` & `krutils-0.20230411.1624/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230411.1623",
+    version="0.20230411.1624",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

