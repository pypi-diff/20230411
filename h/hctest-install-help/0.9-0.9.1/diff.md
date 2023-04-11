# Comparing `tmp/hctest_install_help-0.9.tar.gz` & `tmp/hctest_install_help-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hctest_install_help-0.9.tar", last modified: Mon Apr  3 07:39:14 2023, max compression
+gzip compressed data, was "dist/hctest_install_help-0.9.1.tar", last modified: Tue Apr 11 14:35:38 2023, max compression
```

## Comparing `hctest_install_help-0.9.tar` & `hctest_install_help-0.9.1.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-03 07:39:14.191491 hctest_install_help-0.9/
--rw-r--r--   0 mrding     (501) staff       (20)      411 2023-04-03 07:39:14.190662 hctest_install_help-0.9/PKG-INFO
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-03 07:39:14.137049 hctest_install_help-0.9/hctest_install_help/
--rw-r--r--   0 mrding     (501) staff       (20)      109 2023-04-01 06:47:13.000000 hctest_install_help-0.9/hctest_install_help/__init__.py
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-03 07:39:14.148559 hctest_install_help-0.9/hctest_install_help/install_adb_env/
--rwxr--r--   0 mrding     (501) staff       (20)       83 2023-03-31 07:59:08.000000 hctest_install_help-0.9/hctest_install_help/install_adb_env/__init__.py
--rwxr--r--   0 mrding     (501) staff       (20)     2032 2023-04-01 06:05:31.000000 hctest_install_help-0.9/hctest_install_help/install_adb_env/adb_env.py
--rw-r--r--   0 mrding     (501) staff       (20)      612 2023-04-01 07:06:08.000000 hctest_install_help-0.9/hctest_install_help/install_adb_env/check_env.py
--rwxr--r--   0 mrding     (501) staff       (20)      684 2023-04-01 05:46:48.000000 hctest_install_help-0.9/hctest_install_help/install_adb_env/run.py
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-03 07:39:14.156858 hctest_install_help-0.9/hctest_install_help/package/
--rwxr--r--   0 mrding     (501) staff       (20)       83 2023-03-31 07:59:08.000000 hctest_install_help-0.9/hctest_install_help/package/__init__.py
--rwxr--r--   0 mrding     (501) staff       (20)      399 2023-03-31 07:59:08.000000 hctest_install_help-0.9/hctest_install_help/package/mac_env.py
--rwxr--r--   0 mrding     (501) staff       (20)      610 2023-04-01 11:49:32.000000 hctest_install_help-0.9/hctest_install_help/package/unzip.py
--rwxr--r--   0 mrding     (501) staff       (20)     1826 2023-04-01 06:47:13.000000 hctest_install_help-0.9/hctest_install_help/package/windows_env.py
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-03 07:39:14.141410 hctest_install_help-0.9/hctest_install_help.egg-info/
--rw-r--r--   0 mrding     (501) staff       (20)      411 2023-04-03 07:39:14.000000 hctest_install_help-0.9/hctest_install_help.egg-info/PKG-INFO
--rw-r--r--   0 mrding     (501) staff       (20)      558 2023-04-03 07:39:14.000000 hctest_install_help-0.9/hctest_install_help.egg-info/SOURCES.txt
--rw-r--r--   0 mrding     (501) staff       (20)        1 2023-04-03 07:39:14.000000 hctest_install_help-0.9/hctest_install_help.egg-info/dependency_links.txt
--rw-r--r--   0 mrding     (501) staff       (20)       20 2023-04-03 07:39:14.000000 hctest_install_help-0.9/hctest_install_help.egg-info/top_level.txt
--rw-r--r--   0 mrding     (501) staff       (20)       38 2023-04-03 07:39:14.193468 hctest_install_help-0.9/setup.cfg
--rw-r--r--   0 mrding     (501) staff       (20)      624 2023-04-03 07:38:15.000000 hctest_install_help-0.9/setup.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-11 14:35:38.650975 hctest_install_help-0.9.1/
+-rw-r--r--   0 mrding     (501) staff       (20)      413 2023-04-11 14:35:38.650570 hctest_install_help-0.9.1/PKG-INFO
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-11 14:35:38.640054 hctest_install_help-0.9.1/hctest_install_help/
+-rw-r--r--   0 mrding     (501) staff       (20)      109 2023-04-01 06:47:13.000000 hctest_install_help-0.9.1/hctest_install_help/__init__.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-11 14:35:38.644767 hctest_install_help-0.9.1/hctest_install_help/install_adb_env/
+-rwxr--r--   0 mrding     (501) staff       (20)       83 2023-03-31 07:59:08.000000 hctest_install_help-0.9.1/hctest_install_help/install_adb_env/__init__.py
+-rwxr--r--   0 mrding     (501) staff       (20)     2098 2023-04-11 14:29:26.000000 hctest_install_help-0.9.1/hctest_install_help/install_adb_env/adb_env.py
+-rw-r--r--   0 mrding     (501) staff       (20)      612 2023-04-01 07:06:08.000000 hctest_install_help-0.9.1/hctest_install_help/install_adb_env/check_env.py
+-rwxr--r--   0 mrding     (501) staff       (20)      684 2023-04-01 05:46:48.000000 hctest_install_help-0.9.1/hctest_install_help/install_adb_env/run.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-11 14:35:38.646312 hctest_install_help-0.9.1/hctest_install_help/install_java_env/
+-rw-r--r--   0 mrding     (501) staff       (20)       83 2023-04-03 11:03:37.000000 hctest_install_help-0.9.1/hctest_install_help/install_java_env/__init__.py
+-rw-r--r--   0 mrding     (501) staff       (20)     1361 2023-04-11 14:33:30.000000 hctest_install_help-0.9.1/hctest_install_help/install_java_env/java_env.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-11 14:35:38.649686 hctest_install_help-0.9.1/hctest_install_help/package/
+-rwxr--r--   0 mrding     (501) staff       (20)       83 2023-03-31 07:59:08.000000 hctest_install_help-0.9.1/hctest_install_help/package/__init__.py
+-rwxr--r--   0 mrding     (501) staff       (20)      399 2023-03-31 07:59:08.000000 hctest_install_help-0.9.1/hctest_install_help/package/mac_env.py
+-rwxr--r--   0 mrding     (501) staff       (20)      610 2023-04-01 11:49:32.000000 hctest_install_help-0.9.1/hctest_install_help/package/unzip.py
+-rwxr--r--   0 mrding     (501) staff       (20)     1826 2023-04-01 06:47:13.000000 hctest_install_help-0.9.1/hctest_install_help/package/windows_env.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-11 14:35:38.641933 hctest_install_help-0.9.1/hctest_install_help.egg-info/
+-rw-r--r--   0 mrding     (501) staff       (20)      413 2023-04-11 14:35:38.000000 hctest_install_help-0.9.1/hctest_install_help.egg-info/PKG-INFO
+-rw-r--r--   0 mrding     (501) staff       (20)      656 2023-04-11 14:35:38.000000 hctest_install_help-0.9.1/hctest_install_help.egg-info/SOURCES.txt
+-rw-r--r--   0 mrding     (501) staff       (20)        1 2023-04-11 14:35:38.000000 hctest_install_help-0.9.1/hctest_install_help.egg-info/dependency_links.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       20 2023-04-11 14:35:38.000000 hctest_install_help-0.9.1/hctest_install_help.egg-info/top_level.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       38 2023-04-11 14:35:38.651114 hctest_install_help-0.9.1/setup.cfg
+-rw-r--r--   0 mrding     (501) staff       (20)      625 2023-04-11 14:35:07.000000 hctest_install_help-0.9.1/setup.py
```

### Comparing `hctest_install_help-0.9/hctest_install_help/install_adb_env/check_env.py` & `hctest_install_help-0.9.1/hctest_install_help/install_adb_env/check_env.py`

 * *Files identical despite different names*

### Comparing `hctest_install_help-0.9/hctest_install_help/install_adb_env/run.py` & `hctest_install_help-0.9.1/hctest_install_help/install_adb_env/run.py`

 * *Files identical despite different names*

### Comparing `hctest_install_help-0.9/hctest_install_help/package/unzip.py` & `hctest_install_help-0.9.1/hctest_install_help/package/unzip.py`

 * *Files identical despite different names*

### Comparing `hctest_install_help-0.9/hctest_install_help/package/windows_env.py` & `hctest_install_help-0.9.1/hctest_install_help/package/windows_env.py`

 * *Files identical despite different names*

### Comparing `hctest_install_help-0.9/hctest_install_help.egg-info/SOURCES.txt` & `hctest_install_help-0.9.1/hctest_install_help.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,11 +4,13 @@
 hctest_install_help.egg-info/SOURCES.txt
 hctest_install_help.egg-info/dependency_links.txt
 hctest_install_help.egg-info/top_level.txt
 hctest_install_help/install_adb_env/__init__.py
 hctest_install_help/install_adb_env/adb_env.py
 hctest_install_help/install_adb_env/check_env.py
 hctest_install_help/install_adb_env/run.py
+hctest_install_help/install_java_env/__init__.py
+hctest_install_help/install_java_env/java_env.py
 hctest_install_help/package/__init__.py
 hctest_install_help/package/mac_env.py
 hctest_install_help/package/unzip.py
 hctest_install_help/package/windows_env.py
```

### Comparing `hctest_install_help-0.9/setup.py` & `hctest_install_help-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # author: 华测-长风老师
 # file name：setup.py
 from setuptools import setup, find_packages
 
 setup(
     name="hctest_install_help",
-    version="0.9",
+    version="0.9.1",
     description="辅助帮你下载安装文件",
     author="cf",
     author_email="dingjun_baby@yeah.net",
     url="https://github.com/pypa/sampleproject",
     packages=find_packages(),
     # install_requires=[
     #     'requests',
@@ -17,8 +17,7 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
-
```

