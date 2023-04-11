# Comparing `tmp/krutils-0.20230411.1615.tar.gz` & `tmp/krutils-0.20230411.1616.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230411.1615.tar", last modified: Tue Apr 11 07:15:17 2023, max compression
+gzip compressed data, was "krutils-0.20230411.1616.tar", last modified: Tue Apr 11 07:16:53 2023, max compression
```

## Comparing `krutils-0.20230411.1615.tar` & `krutils-0.20230411.1616.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 07:15:17.290398 krutils-0.20230411.1615/
--rw-rw-rw-   0        0        0      332 2023-04-11 07:15:17.284940 krutils-0.20230411.1615/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1615/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 07:15:17.051688 krutils-0.20230411.1615/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1615/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1615/krutils/CONST.py
--rw-rw-rw-   0        0        0       93 2023-04-11 07:09:16.000000 krutils-0.20230411.1615/krutils/__init__.py
--rw-rw-rw-   0        0        0     5524 2021-10-04 16:16:25.000000 krutils-0.20230411.1615/krutils/dbmgr.py
--rw-rw-rw-   0        0        0    33497 2023-04-11 05:51:26.000000 krutils-0.20230411.1615/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:15:17.282198 krutils-0.20230411.1615/krutils.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-11 07:15:16.000000 krutils-0.20230411.1615/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-11 07:15:16.000000 krutils-0.20230411.1615/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 07:15:16.000000 krutils-0.20230411.1615/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-11 07:15:16.000000 krutils-0.20230411.1615/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 07:15:16.000000 krutils-0.20230411.1615/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 07:15:17.291599 krutils-0.20230411.1615/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-04-11 07:15:15.000000 krutils-0.20230411.1615/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:16:53.722585 krutils-0.20230411.1616/
+-rw-rw-rw-   0        0        0      332 2023-04-11 07:16:53.720988 krutils-0.20230411.1616/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1616/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 07:16:53.564332 krutils-0.20230411.1616/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1616/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1616/krutils/CONST.py
+-rw-rw-rw-   0        0        0       93 2023-04-11 07:09:16.000000 krutils-0.20230411.1616/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5485 2023-04-11 07:16:33.000000 krutils-0.20230411.1616/krutils/dbmgr.py
+-rw-rw-rw-   0        0        0    33497 2023-04-11 05:51:26.000000 krutils-0.20230411.1616/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:16:53.718181 krutils-0.20230411.1616/krutils.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-11 07:16:53.000000 krutils-0.20230411.1616/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-04-11 07:16:53.000000 krutils-0.20230411.1616/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 07:16:53.000000 krutils-0.20230411.1616/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-11 07:16:53.000000 krutils-0.20230411.1616/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 07:16:53.000000 krutils-0.20230411.1616/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 07:16:53.722940 krutils-0.20230411.1616/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-04-11 07:16:52.000000 krutils-0.20230411.1616/setup.py
```

### Comparing `krutils-0.20230411.1615/krutils/CONST.py` & `krutils-0.20230411.1616/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1615/krutils/dbmgr.py` & `krutils-0.20230411.1616/krutils/dbmgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 import os
 import pymysql
 from pymysql import Connection
-from common import logger
-from common import utils
+import utils
 
 
 # SQL PARAM 형식
 SQL_PARAM_PATTERN = "#\\{\\D[\\w]*\\}";
 
 # SELECT 기본 MAX 건수 : 500 (DBIO 조회 기본값)
 MAX_CNT = 10000;
```

### Comparing `krutils-0.20230411.1615/krutils/utils.py` & `krutils-0.20230411.1616/krutils/utils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1615/setup.py` & `krutils-0.20230411.1616/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230411.1615",
+    version="0.20230411.1616",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

