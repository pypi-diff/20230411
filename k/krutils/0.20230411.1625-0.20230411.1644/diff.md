# Comparing `tmp/krutils-0.20230411.1625.tar.gz` & `tmp/krutils-0.20230411.1644.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230411.1625.tar", last modified: Tue Apr 11 07:26:00 2023, max compression
+gzip compressed data, was "krutils-0.20230411.1644.tar", last modified: Tue Apr 11 07:44:07 2023, max compression
```

## Comparing `krutils-0.20230411.1625.tar` & `krutils-0.20230411.1644.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 07:26:00.011513 krutils-0.20230411.1625/
--rw-rw-rw-   0        0        0      332 2023-04-11 07:25:59.976341 krutils-0.20230411.1625/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1625/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 07:25:59.923975 krutils-0.20230411.1625/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1625/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1625/krutils/CONST.py
--rw-rw-rw-   0        0        0       93 2023-04-11 07:24:11.000000 krutils-0.20230411.1625/krutils/__init__.py
--rw-rw-rw-   0        0        0     5481 2023-04-11 07:25:57.000000 krutils-0.20230411.1625/krutils/dbmgr.py
--rw-rw-rw-   0        0        0    33497 2023-04-11 05:51:26.000000 krutils-0.20230411.1625/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:25:59.972369 krutils-0.20230411.1625/krutils.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-11 07:25:59.000000 krutils-0.20230411.1625/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-11 07:25:59.000000 krutils-0.20230411.1625/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 07:25:59.000000 krutils-0.20230411.1625/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-11 07:25:59.000000 krutils-0.20230411.1625/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 07:25:59.000000 krutils-0.20230411.1625/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 07:26:00.012042 krutils-0.20230411.1625/setup.cfg
--rw-rw-rw-   0        0        0      664 2023-04-11 07:25:59.000000 krutils-0.20230411.1625/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:44:07.288281 krutils-0.20230411.1644/
+-rw-rw-rw-   0        0        0      332 2023-04-11 07:44:07.283490 krutils-0.20230411.1644/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1644/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 07:44:07.134510 krutils-0.20230411.1644/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1644/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230411.1644/krutils/CONST.py
+-rw-rw-rw-   0        0        0       71 2023-04-11 07:37:54.000000 krutils-0.20230411.1644/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5528 2023-04-11 07:31:01.000000 krutils-0.20230411.1644/krutils/_dbmgr.py
+-rw-rw-rw-   0        0        0    33519 2023-04-11 07:31:30.000000 krutils-0.20230411.1644/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:44:07.278313 krutils-0.20230411.1644/krutils.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-11 07:44:06.000000 krutils-0.20230411.1644/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-04-11 07:44:06.000000 krutils-0.20230411.1644/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 07:44:06.000000 krutils-0.20230411.1644/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-11 07:44:06.000000 krutils-0.20230411.1644/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 07:44:06.000000 krutils-0.20230411.1644/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 07:44:07.288281 krutils-0.20230411.1644/setup.cfg
+-rw-rw-rw-   0        0        0      664 2023-04-11 07:44:05.000000 krutils-0.20230411.1644/setup.py
```

### Comparing `krutils-0.20230411.1625/krutils/CONST.py` & `krutils-0.20230411.1644/krutils/CONST.py`

 * *Files 19% similar despite different names*

```diff
@@ -58,7 +58,30 @@
 # MAX TIMESTAMP : 9999년 12월 31일 23시 59분 59.999999초
 MAX_TIMESTAMP = "99991231235959999999"
 
 # MAX TIMESTAMP : 23시 59분 59.999999초
 MAX_TIMESTAMP_TM = "235959999999"
 
 
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+KATIS_CONFIG_FILE_NAME='katis.json'
+
+
+
```

### Comparing `krutils-0.20230411.1625/krutils/dbmgr.py` & `krutils-0.20230411.1644/krutils/_dbmgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import re
 import os
 import pymysql
 from pymysql import Connection
-from .krutils import utils
+import utils
+
+print (utils.__file__)
+logger = utils.logger(__file__)
+
 
 
 # SQL PARAM 형식
 SQL_PARAM_PATTERN = "#\\{\\D[\\w]*\\}";
 
 # SELECT 기본 MAX 건수 : 500 (DBIO 조회 기본값)
 MAX_CNT = 10000;
```

### Comparing `krutils-0.20230411.1625/krutils/utils.py` & `krutils-0.20230411.1644/krutils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -661,14 +661,15 @@
     curr_dir = os.path.dirname(__file__)
     # print("curr_dir[{0}]".format(curr_dir))
 
     katis_config_file_path = ""
     # while True:
     for ii in range(5):
         # print("[{0}] {1}".format(ii, curr_dir))
+        import CONST
 
         if (os.path.isfile(curr_dir + "/" + CONST.KATIS_CONFIG_FILE_NAME) == True):
             katis_config_file_path = os.path.join(curr_dir, CONST.KATIS_CONFIG_FILE_NAME)
             # print("찾았다!", katis_config_file_path)
             break
         else:
             # print("상위로 찾아 올라간다[{0}]->[{1}]".format(curr_dir, os.path.abspath(os.path.join(curr_dir, '..'))))
```

### Comparing `krutils-0.20230411.1625/setup.py` & `krutils-0.20230411.1644/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230411.1625",
+    version="0.20230411.1644",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

