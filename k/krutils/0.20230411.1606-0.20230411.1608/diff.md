# Comparing `tmp/krutils-0.20230411.1606.tar.gz` & `tmp/krutils-0.20230411.1608.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230411.1606.tar", last modified: Tue Apr 11 07:06:21 2023, max compression
+gzip compressed data, was "krutils-0.20230411.1608.tar", last modified: Tue Apr 11 07:08:10 2023, max compression
```

## Comparing `krutils-0.20230411.1606.tar` & `krutils-0.20230411.1608.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 07:06:21.216911 krutils-0.20230411.1606/
--rw-rw-rw-   0        0        0      332 2023-04-11 07:06:21.120561 krutils-0.20230411.1606/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1606/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 07:06:20.845506 krutils-0.20230411.1606/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1606/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1606/krutils/CONST.py
--rw-rw-rw-   0        0        0      110 2023-04-11 07:06:02.000000 krutils-0.20230411.1606/krutils/__init__.py
--rw-rw-rw-   0        0        0     5524 2021-10-04 16:16:25.000000 krutils-0.20230411.1606/krutils/dbmgr.py
--rw-rw-rw-   0        0        0    33497 2023-04-11 05:51:26.000000 krutils-0.20230411.1606/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:06:21.067160 krutils-0.20230411.1606/krutils.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-11 07:06:20.000000 krutils-0.20230411.1606/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-04-11 07:06:20.000000 krutils-0.20230411.1606/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 07:06:20.000000 krutils-0.20230411.1606/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 07:06:20.000000 krutils-0.20230411.1606/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 07:06:21.221993 krutils-0.20230411.1606/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-04-11 07:06:18.000000 krutils-0.20230411.1606/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:06:21.111857 krutils-0.20230411.1606/test/
--rw-rw-rw-   0        0        0    11009 2023-04-11 02:27:48.000000 krutils-0.20230411.1606/test/KRLog.py
--rw-rw-rw-   0        0        0      176 2023-04-10 05:10:21.000000 krutils-0.20230411.1606/test/KRUtils.py
--rw-rw-rw-   0        0        0      320 2023-04-11 05:26:00.000000 krutils-0.20230411.1606/test/module_tester.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:08:10.268488 krutils-0.20230411.1608/
+-rw-rw-rw-   0        0        0      332 2023-04-11 07:08:10.257455 krutils-0.20230411.1608/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1608/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 07:08:10.108192 krutils-0.20230411.1608/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1608/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1608/krutils/CONST.py
+-rw-rw-rw-   0        0        0      106 2023-04-11 07:08:07.000000 krutils-0.20230411.1608/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5524 2021-10-04 16:16:25.000000 krutils-0.20230411.1608/krutils/dbmgr.py
+-rw-rw-rw-   0        0        0    33497 2023-04-11 05:51:26.000000 krutils-0.20230411.1608/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:08:10.185794 krutils-0.20230411.1608/krutils.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-11 07:08:09.000000 krutils-0.20230411.1608/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-04-11 07:08:09.000000 krutils-0.20230411.1608/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 07:08:09.000000 krutils-0.20230411.1608/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 07:08:09.000000 krutils-0.20230411.1608/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 07:08:10.273965 krutils-0.20230411.1608/setup.cfg
+-rw-rw-rw-   0        0        0      697 2023-04-11 07:08:09.000000 krutils-0.20230411.1608/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:08:10.213048 krutils-0.20230411.1608/test/
+-rw-rw-rw-   0        0        0    11009 2023-04-11 02:27:48.000000 krutils-0.20230411.1608/test/KRLog.py
+-rw-rw-rw-   0        0        0      176 2023-04-10 05:10:21.000000 krutils-0.20230411.1608/test/KRUtils.py
+-rw-rw-rw-   0        0        0      320 2023-04-11 05:26:00.000000 krutils-0.20230411.1608/test/module_tester.py
```

### Comparing `krutils-0.20230411.1606/krutils/CONST.py` & `krutils-0.20230411.1608/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1606/krutils/dbmgr.py` & `krutils-0.20230411.1608/krutils/dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1606/krutils/utils.py` & `krutils-0.20230411.1608/krutils/utils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1606/setup.py` & `krutils-0.20230411.1608/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230411.1606",
+    version="0.20230411.1608",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `krutils-0.20230411.1606/test/KRLog.py` & `krutils-0.20230411.1608/test/KRLog.py`

 * *Files identical despite different names*

