# Comparing `tmp/krutils-0.20230411.1609.tar.gz` & `tmp/krutils-0.20230411.1615.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230411.1609.tar", last modified: Tue Apr 11 07:09:23 2023, max compression
+gzip compressed data, was "krutils-0.20230411.1615.tar", last modified: Tue Apr 11 07:15:17 2023, max compression
```

## Comparing `krutils-0.20230411.1609.tar` & `krutils-0.20230411.1615.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 07:09:23.213901 krutils-0.20230411.1609/
--rw-rw-rw-   0        0        0      332 2023-04-11 07:09:23.206954 krutils-0.20230411.1609/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1609/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 07:09:23.012756 krutils-0.20230411.1609/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1609/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1609/krutils/CONST.py
--rw-rw-rw-   0        0        0       93 2023-04-11 07:09:16.000000 krutils-0.20230411.1609/krutils/__init__.py
--rw-rw-rw-   0        0        0     5524 2021-10-04 16:16:25.000000 krutils-0.20230411.1609/krutils/dbmgr.py
--rw-rw-rw-   0        0        0    33497 2023-04-11 05:51:26.000000 krutils-0.20230411.1609/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:09:23.189708 krutils-0.20230411.1609/krutils.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-11 07:09:22.000000 krutils-0.20230411.1609/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-04-11 07:09:22.000000 krutils-0.20230411.1609/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 07:09:22.000000 krutils-0.20230411.1609/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 07:09:22.000000 krutils-0.20230411.1609/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 07:09:23.214859 krutils-0.20230411.1609/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-04-11 07:09:21.000000 krutils-0.20230411.1609/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:09:23.205688 krutils-0.20230411.1609/test/
--rw-rw-rw-   0        0        0    11009 2023-04-11 02:27:48.000000 krutils-0.20230411.1609/test/KRLog.py
--rw-rw-rw-   0        0        0      176 2023-04-10 05:10:21.000000 krutils-0.20230411.1609/test/KRUtils.py
--rw-rw-rw-   0        0        0      320 2023-04-11 05:26:00.000000 krutils-0.20230411.1609/test/module_tester.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:15:17.290398 krutils-0.20230411.1615/
+-rw-rw-rw-   0        0        0      332 2023-04-11 07:15:17.284940 krutils-0.20230411.1615/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1615/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 07:15:17.051688 krutils-0.20230411.1615/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1615/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1615/krutils/CONST.py
+-rw-rw-rw-   0        0        0       93 2023-04-11 07:09:16.000000 krutils-0.20230411.1615/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5524 2021-10-04 16:16:25.000000 krutils-0.20230411.1615/krutils/dbmgr.py
+-rw-rw-rw-   0        0        0    33497 2023-04-11 05:51:26.000000 krutils-0.20230411.1615/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:15:17.282198 krutils-0.20230411.1615/krutils.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-11 07:15:16.000000 krutils-0.20230411.1615/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-04-11 07:15:16.000000 krutils-0.20230411.1615/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 07:15:16.000000 krutils-0.20230411.1615/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-11 07:15:16.000000 krutils-0.20230411.1615/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 07:15:16.000000 krutils-0.20230411.1615/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 07:15:17.291599 krutils-0.20230411.1615/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-04-11 07:15:15.000000 krutils-0.20230411.1615/setup.py
```

### Comparing `krutils-0.20230411.1609/krutils/CONST.py` & `krutils-0.20230411.1615/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1609/krutils/dbmgr.py` & `krutils-0.20230411.1615/krutils/dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1609/krutils/utils.py` & `krutils-0.20230411.1615/krutils/utils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1609/setup.py` & `krutils-0.20230411.1615/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230411.1609",
+    version="0.20230411.1615",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     # package_dir={"": "krutils"},
     # packages=setuptools.find_packages(where="krutils"),
     package_dir={"krutils": "krutils",
                  "krutils.test": "test" },
-    packages=["krutils", "krutils.test"],
+    packages=["krutils"],
     python_requires=">=3.0",
     install_requires=[
+        "PyMySQL>=1.0.3"
     ]
 )
```

