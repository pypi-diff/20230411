# Comparing `tmp/krutils-0.20230411.1434.tar.gz` & `tmp/krutils-0.20230411.1438.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230411.1434.tar", last modified: Tue Apr 11 05:35:01 2023, max compression
+gzip compressed data, was "krutils-0.20230411.1438.tar", last modified: Tue Apr 11 05:38:15 2023, max compression
```

## Comparing `krutils-0.20230411.1434.tar` & `krutils-0.20230411.1438.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 05:35:01.645553 krutils-0.20230411.1434/
--rw-rw-rw-   0        0        0      332 2023-04-11 05:35:01.613992 krutils-0.20230411.1434/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1434/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 05:35:01.405711 krutils-0.20230411.1434/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1434/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1434/krutils/CONST.py
--rw-rw-rw-   0        0        0        0 2023-03-24 07:19:02.000000 krutils-0.20230411.1434/krutils/__init__.py
--rw-rw-rw-   0        0        0     5524 2021-10-04 16:16:25.000000 krutils-0.20230411.1434/krutils/dbmgr.py
--rw-rw-rw-   0        0        0    33547 2023-04-11 05:34:46.000000 krutils-0.20230411.1434/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 05:35:01.587293 krutils-0.20230411.1434/krutils.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-11 05:35:00.000000 krutils-0.20230411.1434/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-04-11 05:35:00.000000 krutils-0.20230411.1434/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 05:35:00.000000 krutils-0.20230411.1434/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 05:35:00.000000 krutils-0.20230411.1434/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 05:35:01.649626 krutils-0.20230411.1434/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-04-11 05:34:58.000000 krutils-0.20230411.1434/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 05:35:01.608655 krutils-0.20230411.1434/test/
--rw-rw-rw-   0        0        0    11009 2023-04-11 02:27:48.000000 krutils-0.20230411.1434/test/KRLog.py
--rw-rw-rw-   0        0        0      176 2023-04-10 05:10:21.000000 krutils-0.20230411.1434/test/KRUtils.py
--rw-rw-rw-   0        0        0      320 2023-04-11 05:26:00.000000 krutils-0.20230411.1434/test/module_tester.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:38:15.790619 krutils-0.20230411.1438/
+-rw-rw-rw-   0        0        0      332 2023-04-11 05:38:15.790028 krutils-0.20230411.1438/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1438/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 05:38:15.625976 krutils-0.20230411.1438/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1438/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1438/krutils/CONST.py
+-rw-rw-rw-   0        0        0        0 2023-03-24 07:19:02.000000 krutils-0.20230411.1438/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5524 2021-10-04 16:16:25.000000 krutils-0.20230411.1438/krutils/dbmgr.py
+-rw-rw-rw-   0        0        0    33462 2023-04-11 05:38:11.000000 krutils-0.20230411.1438/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:38:15.781407 krutils-0.20230411.1438/krutils.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-11 05:38:15.000000 krutils-0.20230411.1438/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-04-11 05:38:15.000000 krutils-0.20230411.1438/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 05:38:15.000000 krutils-0.20230411.1438/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 05:38:15.000000 krutils-0.20230411.1438/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 05:38:15.790619 krutils-0.20230411.1438/setup.cfg
+-rw-rw-rw-   0        0        0      697 2023-04-11 05:38:13.000000 krutils-0.20230411.1438/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:38:15.788386 krutils-0.20230411.1438/test/
+-rw-rw-rw-   0        0        0    11009 2023-04-11 02:27:48.000000 krutils-0.20230411.1438/test/KRLog.py
+-rw-rw-rw-   0        0        0      176 2023-04-10 05:10:21.000000 krutils-0.20230411.1438/test/KRUtils.py
+-rw-rw-rw-   0        0        0      320 2023-04-11 05:26:00.000000 krutils-0.20230411.1438/test/module_tester.py
```

### Comparing `krutils-0.20230411.1434/krutils/CONST.py` & `krutils-0.20230411.1438/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1434/krutils/dbmgr.py` & `krutils-0.20230411.1438/krutils/dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1434/krutils/utils.py` & `krutils-0.20230411.1438/krutils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -971,32 +971,29 @@
 
 
     def _gen_log_header(self, debug_level) -> str:
         '''[HH24MISS.FFF][CALLER_NAME:LINE5byte]'''
 
         from datetime import datetime
 
-        HEADER_LENGTH = 40
-
         header = ""
         if (debug_level == self.config.DEBUG_LEVEL_ALL):
             header = header + "[SYS]"
         elif (debug_level == self.config.DEBUG_LEVEL_DB):
             header = header + "[SQL]"
         elif (debug_level == self.config.DEBUG_LEVEL_DEBUG):
             header = header + "[DBG]"
         elif (debug_level == self.config.DEBUG_LEVEL_INFO):
             header = header + "[INF]"
         elif (debug_level == self.config.DEBUG_LEVEL_ERROR):
             header = header + "[ERR]"
 
-        header = header + " " + "[" + datetime.now().strftime("%H%M%S.%f")[:-3] + "]"                               # 일시
-        header = header + " " + "[" + self._caller_file_name() + ":" + str(self._caller_file_line()).zfill(5) + "]"       # 호출자
-        header = header.ljust(HEADER_LENGTH, " ")                                                                   # 길이 맞추기
-
+        header = header + " " + "[" + datetime.now().strftime("%H%M%S.%f")[:-3] + "]"                                   # 일시
+        header = header + " " + "[" + self._caller_file_name() + ":" + str(self._caller_file_line()).zfill(5) + "]"     # 호출자
+        # header = header.ljust(40, " ")                                                                                  # 길이 맞추기
 
         return header
 
 
 
     def _substitute_string(self, input: str, *args) -> str:
 
@@ -1050,15 +1047,14 @@
         # 남은 치환자 제거
         log_body = log_body.replace(self.config._LOG_SUBSTITUTOR, "")
 
 
         #################
         # CONSOLE PRINT
         if self.config.DEBUG_CONSOLE_PRINT_YN == "Y":
-            print (self._gen_log_header(debug_level) + '|')
             print (self._gen_log_header(debug_level) + " " + log_body)
 
 
         #################
         # FILE PRINT
         if self.config.DEBUG_FILE_PRINT_YN == "Y":
             print("파일프린트 시작한다[{}]".format(self.config.DEBUG_FILE_PRINT_PATH))
```

### Comparing `krutils-0.20230411.1434/setup.py` & `krutils-0.20230411.1438/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230411.1434",
+    version="0.20230411.1438",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `krutils-0.20230411.1434/test/KRLog.py` & `krutils-0.20230411.1438/test/KRLog.py`

 * *Files identical despite different names*

