# Comparing `tmp/krutils-0.20230411.1438.tar.gz` & `tmp/krutils-0.20230411.1450.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230411.1438.tar", last modified: Tue Apr 11 05:38:15 2023, max compression
+gzip compressed data, was "krutils-0.20230411.1450.tar", last modified: Tue Apr 11 05:50:28 2023, max compression
```

## Comparing `krutils-0.20230411.1438.tar` & `krutils-0.20230411.1450.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 05:38:15.790619 krutils-0.20230411.1438/
--rw-rw-rw-   0        0        0      332 2023-04-11 05:38:15.790028 krutils-0.20230411.1438/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1438/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 05:38:15.625976 krutils-0.20230411.1438/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1438/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1438/krutils/CONST.py
--rw-rw-rw-   0        0        0        0 2023-03-24 07:19:02.000000 krutils-0.20230411.1438/krutils/__init__.py
--rw-rw-rw-   0        0        0     5524 2021-10-04 16:16:25.000000 krutils-0.20230411.1438/krutils/dbmgr.py
--rw-rw-rw-   0        0        0    33462 2023-04-11 05:38:11.000000 krutils-0.20230411.1438/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 05:38:15.781407 krutils-0.20230411.1438/krutils.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-11 05:38:15.000000 krutils-0.20230411.1438/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-04-11 05:38:15.000000 krutils-0.20230411.1438/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 05:38:15.000000 krutils-0.20230411.1438/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 05:38:15.000000 krutils-0.20230411.1438/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 05:38:15.790619 krutils-0.20230411.1438/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-04-11 05:38:13.000000 krutils-0.20230411.1438/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 05:38:15.788386 krutils-0.20230411.1438/test/
--rw-rw-rw-   0        0        0    11009 2023-04-11 02:27:48.000000 krutils-0.20230411.1438/test/KRLog.py
--rw-rw-rw-   0        0        0      176 2023-04-10 05:10:21.000000 krutils-0.20230411.1438/test/KRUtils.py
--rw-rw-rw-   0        0        0      320 2023-04-11 05:26:00.000000 krutils-0.20230411.1438/test/module_tester.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:50:28.140241 krutils-0.20230411.1450/
+-rw-rw-rw-   0        0        0      332 2023-04-11 05:50:28.096984 krutils-0.20230411.1450/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1450/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 05:50:27.884838 krutils-0.20230411.1450/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1450/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1450/krutils/CONST.py
+-rw-rw-rw-   0        0        0        0 2023-03-24 07:19:02.000000 krutils-0.20230411.1450/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5524 2021-10-04 16:16:25.000000 krutils-0.20230411.1450/krutils/dbmgr.py
+-rw-rw-rw-   0        0        0    33497 2023-04-11 05:50:23.000000 krutils-0.20230411.1450/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:50:28.076815 krutils-0.20230411.1450/krutils.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-11 05:50:27.000000 krutils-0.20230411.1450/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-04-11 05:50:27.000000 krutils-0.20230411.1450/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 05:50:27.000000 krutils-0.20230411.1450/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 05:50:27.000000 krutils-0.20230411.1450/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 05:50:28.140998 krutils-0.20230411.1450/setup.cfg
+-rw-rw-rw-   0        0        0      697 2023-04-11 05:50:26.000000 krutils-0.20230411.1450/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:50:28.083773 krutils-0.20230411.1450/test/
+-rw-rw-rw-   0        0        0    11009 2023-04-11 02:27:48.000000 krutils-0.20230411.1450/test/KRLog.py
+-rw-rw-rw-   0        0        0      176 2023-04-10 05:10:21.000000 krutils-0.20230411.1450/test/KRUtils.py
+-rw-rw-rw-   0        0        0      320 2023-04-11 05:26:00.000000 krutils-0.20230411.1450/test/module_tester.py
```

### Comparing `krutils-0.20230411.1438/krutils/CONST.py` & `krutils-0.20230411.1450/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1438/krutils/dbmgr.py` & `krutils-0.20230411.1450/krutils/dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1438/krutils/utils.py` & `krutils-0.20230411.1450/krutils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1112,19 +1112,21 @@
         * LOG_CONSOLE_YN : Y*/N
         * LOG_FILE_YN : Y/N*
         * LOG_DIR_PATH : log directory path(None is default)
         * LOG_FILE_NAME : log file name(None is default)
 
     '''
 
-    def __init__(self, caller_path: str):
+    def __init__(self, ____file__: str):
 
         # logger에 필요한 변수와 기능이 담겨있는 super 클래스를 초기화 한다.
         super().__init__()
 
+        caller_path = ____file__
+
         # 인자로 받은 호출자 경로로 부터 root까지 탐색하며 config 파일을 찾는다.
         # 존재시 설정을 덮어 씌운다
         cfp = _logger_util().find_config_file_path(caller_path)
 
         if (is_empty(cfp) != True):
             parsed_config = _logger_util().parse_config_file(cfp)
```

### Comparing `krutils-0.20230411.1438/setup.py` & `krutils-0.20230411.1450/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230411.1438",
+    version="0.20230411.1450",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `krutils-0.20230411.1438/test/KRLog.py` & `krutils-0.20230411.1450/test/KRLog.py`

 * *Files identical despite different names*

