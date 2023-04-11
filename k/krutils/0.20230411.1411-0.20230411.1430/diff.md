# Comparing `tmp/krutils-0.20230411.1411.tar.gz` & `tmp/krutils-0.20230411.1430.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230411.1411.tar", last modified: Tue Apr 11 05:11:59 2023, max compression
+gzip compressed data, was "krutils-0.20230411.1430.tar", last modified: Tue Apr 11 05:30:46 2023, max compression
```

## Comparing `krutils-0.20230411.1411.tar` & `krutils-0.20230411.1430.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 05:11:59.149078 krutils-0.20230411.1411/
--rw-rw-rw-   0        0        0      332 2023-04-11 05:11:59.142249 krutils-0.20230411.1411/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1411/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 05:11:59.030576 krutils-0.20230411.1411/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1411/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1411/krutils/CONST.py
--rw-rw-rw-   0        0        0     7385 2023-04-10 10:01:05.000000 krutils-0.20230411.1411/krutils/Loggert.py
--rw-rw-rw-   0        0        0        0 2023-03-24 07:19:02.000000 krutils-0.20230411.1411/krutils/__init__.py
--rw-rw-rw-   0        0        0     5524 2021-10-04 16:16:25.000000 krutils-0.20230411.1411/krutils/dbmgr.py
--rw-rw-rw-   0        0        0    33328 2023-04-11 04:57:05.000000 krutils-0.20230411.1411/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 05:11:59.132140 krutils-0.20230411.1411/krutils.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-11 05:11:58.000000 krutils-0.20230411.1411/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-04-11 05:11:58.000000 krutils-0.20230411.1411/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 05:11:58.000000 krutils-0.20230411.1411/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 05:11:58.000000 krutils-0.20230411.1411/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 05:11:59.151793 krutils-0.20230411.1411/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-04-11 05:11:56.000000 krutils-0.20230411.1411/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 05:11:59.142249 krutils-0.20230411.1411/test/
--rw-rw-rw-   0        0        0    11009 2023-04-11 02:27:48.000000 krutils-0.20230411.1411/test/KRLog.py
--rw-rw-rw-   0        0        0      176 2023-04-10 05:10:21.000000 krutils-0.20230411.1411/test/KRUtils.py
--rw-rw-rw-   0        0        0      388 2023-04-11 04:25:34.000000 krutils-0.20230411.1411/test/module_tester.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:30:46.868958 krutils-0.20230411.1430/
+-rw-rw-rw-   0        0        0      332 2023-04-11 05:30:46.854976 krutils-0.20230411.1430/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1430/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 05:30:46.404402 krutils-0.20230411.1430/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1430/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1430/krutils/CONST.py
+-rw-rw-rw-   0        0        0        0 2023-03-24 07:19:02.000000 krutils-0.20230411.1430/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5524 2021-10-04 16:16:25.000000 krutils-0.20230411.1430/krutils/dbmgr.py
+-rw-rw-rw-   0        0        0    33541 2023-04-11 05:30:27.000000 krutils-0.20230411.1430/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:30:46.767740 krutils-0.20230411.1430/krutils.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-11 05:30:45.000000 krutils-0.20230411.1430/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-04-11 05:30:45.000000 krutils-0.20230411.1430/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 05:30:45.000000 krutils-0.20230411.1430/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 05:30:45.000000 krutils-0.20230411.1430/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 05:30:46.871199 krutils-0.20230411.1430/setup.cfg
+-rw-rw-rw-   0        0        0      697 2023-04-11 05:30:43.000000 krutils-0.20230411.1430/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:30:46.850681 krutils-0.20230411.1430/test/
+-rw-rw-rw-   0        0        0    11009 2023-04-11 02:27:48.000000 krutils-0.20230411.1430/test/KRLog.py
+-rw-rw-rw-   0        0        0      176 2023-04-10 05:10:21.000000 krutils-0.20230411.1430/test/KRUtils.py
+-rw-rw-rw-   0        0        0      320 2023-04-11 05:26:00.000000 krutils-0.20230411.1430/test/module_tester.py
```

### Comparing `krutils-0.20230411.1411/krutils/CONST.py` & `krutils-0.20230411.1430/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1411/krutils/dbmgr.py` & `krutils-0.20230411.1430/krutils/dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230411.1411/krutils/utils.py` & `krutils-0.20230411.1430/krutils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1050,14 +1050,15 @@
         # 남은 치환자 제거
         log_body = log_body.replace(self.config._LOG_SUBSTITUTOR, "")
 
 
         #################
         # CONSOLE PRINT
         if self.config.DEBUG_CONSOLE_PRINT_YN == "Y":
+            print (self._gen_log_header(debug_level))
             print (self._gen_log_header(debug_level) + " " + log_body)
 
 
         #################
         # FILE PRINT
         if self.config.DEBUG_FILE_PRINT_YN == "Y":
             print("파일프린트 시작한다[{}]".format(self.config.DEBUG_FILE_PRINT_PATH))
@@ -1097,14 +1098,16 @@
     Options>
         Set option can redefine with 'logger.json' file.
         The 'logger.json' file can be caller program directory or above. krutil.logger will seek the 'logger.json' file from caller program directory to root diredctory.
         First found file will be adapted.
 
         SAMPLE> 'logger.json'
         {
+            "__KEYWORDS__" : "LOG_LEVEL/LOG_CONSOLE_YN/LOG_FILE_YN/LOG_DIR_PATH/LOG_FILE_NAME",
+            "__LOG_LEVEL__" : "SYSTEM/DB/DEBUG/INFO/ERROR",
             "LOG_LEVEL" : "INFO",
             "LOG_CONSOLE_YN" : "Y",
             "LOG_FILE_YN" : "N",
             "LOG_DIR_PATH" : "./logs",
             "LOG_FILE_NAME" : "mylog.log"
         }
```

### Comparing `krutils-0.20230411.1411/setup.py` & `krutils-0.20230411.1430/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230411.1411",
+    version="0.20230411.1430",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `krutils-0.20230411.1411/test/KRLog.py` & `krutils-0.20230411.1430/test/KRLog.py`

 * *Files identical despite different names*

