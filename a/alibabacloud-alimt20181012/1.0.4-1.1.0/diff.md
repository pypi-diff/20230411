# Comparing `tmp/alibabacloud_alimt20181012-1.0.4.tar.gz` & `tmp/alibabacloud_alimt20181012-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alimt20181012-1.0.4.tar", last modified: Tue Apr 11 08:51:38 2023, max compression
+gzip compressed data, was "dist/alibabacloud_alimt20181012-1.1.0.tar", last modified: Tue Apr 11 09:30:16 2023, max compression
```

## Comparing `alibabacloud_alimt20181012-1.0.4.tar` & `alibabacloud_alimt20181012-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      258 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1028 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85868 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012/client.py
--rw-r--r--   0 root         (0) root         (0)   105220 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      315 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2825 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85868 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012/client.py
+-rw-r--r--   0 root         (0) root         (0)   105220 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      315 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 09:30:16.000000 alibabacloud_alimt20181012-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-04-11 09:30:15.000000 alibabacloud_alimt20181012-1.1.0/setup.py
```

### Comparing `alibabacloud_alimt20181012-1.0.4/LICENSE` & `alibabacloud_alimt20181012-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012-1.0.4/PKG-INFO` & `alibabacloud_alimt20181012-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alimt20181012
-Version: 1.0.4
+Version: 1.1.0
 Summary: Alibaba Cloud Machine Translation (20181012) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alimt20181012-1.0.4/README-CN.md` & `alibabacloud_alimt20181012-1.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012-1.0.4/README.md` & `alibabacloud_alimt20181012-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012/client.py` & `alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012/models.py` & `alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012.egg-info/PKG-INFO` & `alibabacloud_alimt20181012-1.1.0/alibabacloud_alimt20181012.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alimt20181012
-Version: 1.0.4
+Version: 1.1.0
 Summary: Alibaba Cloud Machine Translation (20181012) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alimt20181012-1.0.4/setup.py` & `alibabacloud_alimt20181012-1.1.0/setup.py`

 * *Files identical despite different names*

