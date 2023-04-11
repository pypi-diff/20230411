# Comparing `tmp/hxq-1.0.5.tar.gz` & `tmp/hxq-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hxq-1.0.5.tar", last modified: Mon Apr 10 16:40:07 2023, max compression
+gzip compressed data, was "dist\hxq-1.0.6.tar", last modified: Tue Apr 11 12:29:53 2023, max compression
```

## Comparing `hxq-1.0.5.tar` & `hxq-1.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 16:40:07.000000 hxq-1.0.5/
--rw-rw-rw-   0        0        0      169 2023-04-10 16:40:07.000000 hxq-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 16:40:07.000000 hxq-1.0.5/hxq/
--rw-rw-rw-   0        0        0      141 2023-04-10 16:33:43.000000 hxq-1.0.5/hxq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:40:07.000000 hxq-1.0.5/hxq/interface/
--rw-rw-rw-   0        0        0      120 2023-04-10 15:28:34.000000 hxq-1.0.5/hxq/interface/__init__.py
--rw-rw-rw-   0        0        0      490 2023-04-10 16:19:54.000000 hxq-1.0.5/hxq/interface/db_helper.py
--rw-rw-rw-   0        0        0      300 2023-04-10 15:28:44.000000 hxq-1.0.5/hxq/interface/httpx.py
--rw-rw-rw-   0        0        0      117 2023-04-10 15:28:59.000000 hxq-1.0.5/hxq/interface/win32.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:40:07.000000 hxq-1.0.5/hxq/libs/
--rw-rw-rw-   0        0        0      123 2023-04-10 15:30:35.000000 hxq-1.0.5/hxq/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:40:07.000000 hxq-1.0.5/hxq/libs/db/
--rw-rw-rw-   0        0        0      120 2023-04-06 15:20:14.000000 hxq-1.0.5/hxq/libs/db/__init__.py
--rw-rw-rw-   0        0        0     4314 2023-04-10 16:30:41.000000 hxq-1.0.5/hxq/libs/db/db_helper.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:40:07.000000 hxq-1.0.5/hxq/libs/httpx/
--rw-rw-rw-   0        0        0      127 2022-07-07 15:51:40.000000 hxq-1.0.5/hxq/libs/httpx/__init__.py
--rw-rw-rw-   0        0        0      553 2022-08-21 03:37:18.000000 hxq-1.0.5/hxq/libs/httpx/chrome_agent.py
--rw-rw-rw-   0        0        0     8336 2023-04-10 15:29:33.000000 hxq-1.0.5/hxq/libs/httpx/http.py
--rw-rw-rw-   0        0        0     3022 2023-04-10 15:29:39.000000 hxq-1.0.5/hxq/libs/httpx/session.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:40:07.000000 hxq-1.0.5/hxq/libs/win32/
--rw-rw-rw-   0        0        0      123 2023-04-05 04:51:31.000000 hxq-1.0.5/hxq/libs/win32/__init__.py
--rw-rw-rw-   0        0        0     2024 2023-04-06 13:47:02.000000 hxq-1.0.5/hxq/libs/win32/api.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:40:07.000000 hxq-1.0.5/hxq/utils/
--rw-rw-rw-   0        0        0      123 2023-04-10 15:30:39.000000 hxq-1.0.5/hxq/utils/__init__.py
--rw-rw-rw-   0        0        0     3362 2023-04-10 15:35:13.000000 hxq-1.0.5/hxq/utils/common.py
--rw-rw-rw-   0        0        0     1676 2023-04-10 15:34:13.000000 hxq-1.0.5/hxq/utils/decorator.py
--rw-rw-rw-   0        0        0     1576 2023-04-10 16:12:31.000000 hxq-1.0.5/hxq/utils/encipher.py
--rw-rw-rw-   0        0        0      418 2023-04-10 15:33:03.000000 hxq-1.0.5/hxq/utils/pic_code.py
--rw-rw-rw-   0        0        0      314 2023-04-09 13:39:57.000000 hxq-1.0.5/hxq/utils/ran_func.py
--rw-rw-rw-   0        0        0     3463 2023-04-09 13:39:58.000000 hxq-1.0.5/hxq/utils/threadx.py
--rw-rw-rw-   0        0        0      948 2023-04-08 18:47:40.000000 hxq-1.0.5/hxq/utils/异步读取操作文件.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:40:07.000000 hxq-1.0.5/hxq.egg-info/
--rw-rw-rw-   0        0        0      169 2023-04-10 16:40:07.000000 hxq-1.0.5/hxq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-04-10 16:40:07.000000 hxq-1.0.5/hxq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 16:40:07.000000 hxq-1.0.5/hxq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-04-10 16:40:07.000000 hxq-1.0.5/hxq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-10 16:40:07.000000 hxq-1.0.5/hxq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 16:40:07.000000 hxq-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      699 2023-04-10 16:32:59.000000 hxq-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:53.000000 hxq-1.0.6/
+-rw-rw-rw-   0        0        0      169 2023-04-11 12:29:53.000000 hxq-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:53.000000 hxq-1.0.6/hxq/
+-rw-rw-rw-   0        0        0      141 2023-04-10 16:33:43.000000 hxq-1.0.6/hxq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:53.000000 hxq-1.0.6/hxq/interface/
+-rw-rw-rw-   0        0        0      120 2023-04-10 15:28:34.000000 hxq-1.0.6/hxq/interface/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-04-10 16:19:54.000000 hxq-1.0.6/hxq/interface/db_helper.py
+-rw-rw-rw-   0        0        0      300 2023-04-10 15:28:44.000000 hxq-1.0.6/hxq/interface/httpx.py
+-rw-rw-rw-   0        0        0      117 2023-04-10 15:28:59.000000 hxq-1.0.6/hxq/interface/win32.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:53.000000 hxq-1.0.6/hxq/libs/
+-rw-rw-rw-   0        0        0      123 2023-04-10 15:30:35.000000 hxq-1.0.6/hxq/libs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:53.000000 hxq-1.0.6/hxq/libs/db/
+-rw-rw-rw-   0        0        0      120 2023-04-06 15:20:14.000000 hxq-1.0.6/hxq/libs/db/__init__.py
+-rw-rw-rw-   0        0        0     4314 2023-04-10 16:30:41.000000 hxq-1.0.6/hxq/libs/db/db_helper.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:53.000000 hxq-1.0.6/hxq/libs/httpx/
+-rw-rw-rw-   0        0        0      127 2022-07-07 15:51:40.000000 hxq-1.0.6/hxq/libs/httpx/__init__.py
+-rw-rw-rw-   0        0        0      553 2022-08-21 03:37:18.000000 hxq-1.0.6/hxq/libs/httpx/chrome_agent.py
+-rw-rw-rw-   0        0        0     8336 2023-04-10 15:29:33.000000 hxq-1.0.6/hxq/libs/httpx/http.py
+-rw-rw-rw-   0        0        0     3022 2023-04-10 15:29:39.000000 hxq-1.0.6/hxq/libs/httpx/session.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:53.000000 hxq-1.0.6/hxq/libs/win32/
+-rw-rw-rw-   0        0        0      123 2023-04-05 04:51:31.000000 hxq-1.0.6/hxq/libs/win32/__init__.py
+-rw-rw-rw-   0        0        0     2024 2023-04-06 13:47:02.000000 hxq-1.0.6/hxq/libs/win32/api.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:53.000000 hxq-1.0.6/hxq/utils/
+-rw-rw-rw-   0        0        0      123 2023-04-10 15:30:39.000000 hxq-1.0.6/hxq/utils/__init__.py
+-rw-rw-rw-   0        0        0     3362 2023-04-10 15:35:13.000000 hxq-1.0.6/hxq/utils/common.py
+-rw-rw-rw-   0        0        0     1676 2023-04-10 15:34:13.000000 hxq-1.0.6/hxq/utils/decorator.py
+-rw-rw-rw-   0        0        0     1576 2023-04-10 16:12:31.000000 hxq-1.0.6/hxq/utils/encipher.py
+-rw-rw-rw-   0        0        0      418 2023-04-10 15:33:03.000000 hxq-1.0.6/hxq/utils/pic_code.py
+-rw-rw-rw-   0        0        0      314 2023-04-09 13:39:57.000000 hxq-1.0.6/hxq/utils/ran_func.py
+-rw-rw-rw-   0        0        0     3463 2023-04-09 13:39:58.000000 hxq-1.0.6/hxq/utils/threadx.py
+-rw-rw-rw-   0        0        0      948 2023-04-08 18:47:40.000000 hxq-1.0.6/hxq/utils/异步读取操作文件.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:29:53.000000 hxq-1.0.6/hxq.egg-info/
+-rw-rw-rw-   0        0        0      169 2023-04-11 12:29:53.000000 hxq-1.0.6/hxq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-04-11 12:29:53.000000 hxq-1.0.6/hxq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 12:29:53.000000 hxq-1.0.6/hxq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-11 12:29:53.000000 hxq-1.0.6/hxq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-11 12:29:53.000000 hxq-1.0.6/hxq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 12:29:53.000000 hxq-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      699 2023-04-11 12:29:46.000000 hxq-1.0.6/setup.py
```

### Comparing `hxq-1.0.5/hxq/libs/db/db_helper.py` & `hxq-1.0.6/hxq/libs/db/db_helper.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.5/hxq/libs/httpx/chrome_agent.py` & `hxq-1.0.6/hxq/libs/httpx/chrome_agent.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.5/hxq/libs/httpx/http.py` & `hxq-1.0.6/hxq/libs/httpx/http.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.5/hxq/libs/httpx/session.py` & `hxq-1.0.6/hxq/libs/httpx/session.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.5/hxq/libs/win32/api.py` & `hxq-1.0.6/hxq/libs/win32/api.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.5/hxq/utils/common.py` & `hxq-1.0.6/hxq/utils/common.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.5/hxq/utils/decorator.py` & `hxq-1.0.6/hxq/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.5/hxq/utils/encipher.py` & `hxq-1.0.6/hxq/utils/encipher.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.5/hxq/utils/threadx.py` & `hxq-1.0.6/hxq/utils/threadx.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.5/hxq/utils/异步读取操作文件.py` & `hxq-1.0.6/hxq/utils/异步读取操作文件.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.5/hxq.egg-info/SOURCES.txt` & `hxq-1.0.6/hxq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hxq-1.0.5/setup.py` & `hxq-1.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(name='hxq',
       author='hxq',
-      version='1.0.5',
+      version='1.0.6',
       packages=find_packages(exclude=["*.demo", "*.demo.*", "tests", "demos"]),
       author_email='337168530@qq.com',
       description="这是一个python工具包",
       license="GPL",
       # 而 extras_require 这里仅表示该模块会依赖这些包,深度使用模块时，才会用到，这里需要你手动安装
       extras_require={
           'HTML': ["bs4>=0.0.1", "xmltodict>=1.2"],
```

