# Comparing `tmp/krutils-0.20230407.1511.tar.gz` & `tmp/krutils-0.20230411.1411.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230407.1511.tar", last modified: Fri Apr  7 06:11:08 2023, max compression
+gzip compressed data, was "krutils-0.20230411.1411.tar", last modified: Tue Apr 11 05:11:59 2023, max compression
```

## Comparing `krutils-0.20230407.1511.tar` & `krutils-0.20230411.1411.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 06:11:08.105163 krutils-0.20230407.1511/
--rw-rw-rw-   0        0        0      332 2023-04-07 06:11:08.105163 krutils-0.20230407.1511/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230407.1511/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 06:11:08.080515 krutils-0.20230407.1511/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230407.1511/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230407.1511/krutils/CONST.py
--rw-rw-rw-   0        0        0     7665 2023-04-07 06:10:48.000000 krutils-0.20230407.1511/krutils/Loggert.py
--rw-rw-rw-   0        0        0        0 2023-03-24 07:19:02.000000 krutils-0.20230407.1511/krutils/__init__.py
--rw-rw-rw-   0        0        0     5524 2021-10-04 16:16:25.000000 krutils-0.20230407.1511/krutils/dbmgr.py
--rw-rw-rw-   0        0        0    20842 2023-03-31 08:25:49.000000 krutils-0.20230407.1511/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 06:11:08.096863 krutils-0.20230407.1511/krutils.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-07 06:11:07.000000 krutils-0.20230407.1511/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-04-07 06:11:07.000000 krutils-0.20230407.1511/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 06:11:07.000000 krutils-0.20230407.1511/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-07 06:11:07.000000 krutils-0.20230407.1511/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 06:11:08.108318 krutils-0.20230407.1511/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-04-07 06:11:07.000000 krutils-0.20230407.1511/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 06:11:08.105163 krutils-0.20230407.1511/test/
--rw-rw-rw-   0        0        0      126 2023-04-05 07:27:05.000000 krutils-0.20230407.1511/test/Clz_test.py
--rw-rw-rw-   0        0        0      326 2023-04-05 07:27:58.000000 krutils-0.20230407.1511/test/Lg.py
--rw-rw-rw-   0        0        0       78 2023-04-05 07:24:42.000000 krutils-0.20230407.1511/test/ct2.py
--rw-rw-rw-   0        0        0      465 2023-03-31 08:43:41.000000 krutils-0.20230407.1511/test/module_tester.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:11:59.149078 krutils-0.20230411.1411/
+-rw-rw-rw-   0        0        0      332 2023-04-11 05:11:59.142249 krutils-0.20230411.1411/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-03-31 07:30:50.000000 krutils-0.20230411.1411/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 05:11:59.030576 krutils-0.20230411.1411/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230411.1411/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1660 2023-03-28 06:25:31.000000 krutils-0.20230411.1411/krutils/CONST.py
+-rw-rw-rw-   0        0        0     7385 2023-04-10 10:01:05.000000 krutils-0.20230411.1411/krutils/Loggert.py
+-rw-rw-rw-   0        0        0        0 2023-03-24 07:19:02.000000 krutils-0.20230411.1411/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5524 2021-10-04 16:16:25.000000 krutils-0.20230411.1411/krutils/dbmgr.py
+-rw-rw-rw-   0        0        0    33328 2023-04-11 04:57:05.000000 krutils-0.20230411.1411/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:11:59.132140 krutils-0.20230411.1411/krutils.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-11 05:11:58.000000 krutils-0.20230411.1411/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-04-11 05:11:58.000000 krutils-0.20230411.1411/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 05:11:58.000000 krutils-0.20230411.1411/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 05:11:58.000000 krutils-0.20230411.1411/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 05:11:59.151793 krutils-0.20230411.1411/setup.cfg
+-rw-rw-rw-   0        0        0      697 2023-04-11 05:11:56.000000 krutils-0.20230411.1411/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:11:59.142249 krutils-0.20230411.1411/test/
+-rw-rw-rw-   0        0        0    11009 2023-04-11 02:27:48.000000 krutils-0.20230411.1411/test/KRLog.py
+-rw-rw-rw-   0        0        0      176 2023-04-10 05:10:21.000000 krutils-0.20230411.1411/test/KRUtils.py
+-rw-rw-rw-   0        0        0      388 2023-04-11 04:25:34.000000 krutils-0.20230411.1411/test/module_tester.py
```

### Comparing `krutils-0.20230407.1511/krutils/CONST.py` & `krutils-0.20230411.1411/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230407.1511/krutils/Loggert.py` & `krutils-0.20230411.1411/krutils/Loggert.py`

 * *Files 12% similar despite different names*

```diff
@@ -85,27 +85,14 @@
 DEBUG_FILE_FILE_NAME  = datetime.now().strftime("%H%M%S") + '.log';
 
 
 
 
 
 
-
-
-#######################################
-# CLASS 초기화
-#   - CALLER 정보를 입력하는 경우 설정 파일을 탐색하여 발견되면 적용한다
-class init:
-    caller_file_name = ''
-
-    def __init__(self, caller_file_name):
-        self.caller_file_name = caller_file_name;
-        print(__name__ + ' is initiating... by ' + caller_file_name)
-
-
 # try:
 #     from krutils import utils
 #     config_file_path = utils.find_first_file_to_root(__LOGGER_CONFIG_FILE_NAME)
 
 #     if utils.is_empty(config_file_path) != True:
 
 #         import json
@@ -144,36 +131,36 @@
 
 
 
 ##########################################
 ##      시스템 정보
 ##########################################
 # 호출자 파일 명
-def __caller_file_name() -> str:
+def _caller_file_name(self) -> str:
     return os.path.basename(inspect.stack()[__CALLER_IDX][1])
 
 # 호출자 라인번호
-def __caller_file_line() -> int:
+def _caller_file_line(self) -> int:
     return inspect.stack()[__CALLER_IDX][2]
 
 
 ##########################################
 ##      log
 ##########################################
-def __gen_substitutor_dummy_string(cnt: int) -> str:
+def _gen_substitutor_dummy_string(self, cnt: int) -> str:
     '''Dummy 치환자 문자열 생성'''
     ret = ""
 
     for ii in range(cnt):
         ret = ret + __LOG_SUBSTITUTOR
 
     return ret
 
 
-def __gen_log_header(debug_level) -> str:
+def _gen_log_header(self, debug_level) -> str:
     '''[HH24MISS.FFF][CALLER_NAME:LINE5byte]'''
 
     HEADER_LENGTH = 40
 
     header = ""
     if (debug_level == DEBUG_LEVEL_ALL):
         header = header + "[SYSTEM]"
@@ -186,50 +173,49 @@
     elif (debug_level == DEBUG_LEVEL_ERR):
         header = header + "[ERROR ]"
 
     header = header + "[" + datetime.now().strftime("%H%M%S.%f")[:-3] + "]"                             # 일시
     header = header + "[" + __caller_file_name() + ":" + str(__caller_file_line()).zfill(5) + "]"       # 호출자
     header = header.ljust(HEADER_LENGTH, " ")                                                           # 길이 맞추기
 
-
     return header
 
 
 
-def __substitute_string(input: str, *args) -> str:
+def _substitute_string(self, input: str, *args) -> str:
 
     if input == None:
         return None
 
     # print ("len", str(len(args)))
     # print (args)
     for ii, arg in enumerate(args):
 
         idx = 0
         try:
-            idx = input.index(__LOG_SUBSTITUTOR)
+            idx = input.index(self.config._LOG_SUBSTITUTOR)
         except Exception as e:
             break;
 
         # print (idx)
         if (idx < 0):
             break;
 
         # print (__LOG_SUBSTITUTOR)
         # print (input, input.replace(__LOG_SUBSTITUTOR, str(arg), 1))
-        input = input.replace(__LOG_SUBSTITUTOR, str(arg), 1)
+        input = input.replace(self.config._LOG_SUBSTITUTOR, str(arg), 1)
 
     return input
 
 
 
 
 
 
-def __print_log(debug_level, template="", *args):
+def _print_log(self, debug_level, template="", *args):
     '''
     로그처리
     header + debug_strings...
     '''
 
     # 정합성 체크 : 시스템에 정의된 디버그레벨과 비교하여 로깅처리를 할지 정한다
     if (debug_level == None):
@@ -242,56 +228,56 @@
     template_str = str(template)
 
 
     ######################
     # 처리
 
     # 문자열 치환
-    log_body = __substitute_string(template_str, *args)
+    log_body = _substitute_string(template_str, *args)
 
     # 남은 치환자 제거
     log_body = log_body.replace(__LOG_SUBSTITUTOR, "")
 
 
     #################
     # CONSOLE PRINT
-    if DEBUG_CONSOLE_PRINT_YN == "Y":
+    if self.config.DEBUG_CONSOLE_PRINT_YN == "Y":
         print (__gen_log_header(debug_level) + " " + log_body)
 
 
     #################
     # FILE PRINT
-    if DEBUG_FILE_PRINT_YN == "Y":
+    if self.config.DEBUG_FILE_PRINT_YN == "Y":
         print("파일프린트 시작한다[{}]".format(DEBUG_FILE_PRINT_PATH))
         # writelog (__gen_log_header(debug_level) + " " + log_body)
         pass
 
 
-def syslog(template="", *args):
-    __print_log(DEBUG_LEVEL_ALL, template, *args)
+def syslog(self, template="", *args):
+    _print_log(DEBUG_LEVEL_ALL, template, *args)
 
 
 
-def dblog(template="", *args):
-    __print_log(DEBUG_LEVEL_DB, template, *args)
+def dblog(self, template="", *args):
+    _print_log(DEBUG_LEVEL_DB, template, *args)
 
 
 
-def debug(template="", *args):
-    __print_log(DEBUG_LEVEL_APP, template, *args)
+def debug(self, template="", *args):
+    _print_log(DEBUG_LEVEL_APP, template, *args)
 
 
 
-def info(template="", *args):
-    __print_log(DEBUG_LEVEL_INFO, template, *args)
+def info(self, template="", *args):
+    _print_log(DEBUG_LEVEL_INFO, template, *args)
 
 
 
-def error(template="", *args):
-    __print_log(DEBUG_LEVEL_ERR, template, *args)
+def error(self, template="", *args):
+    _print_log(DEBUG_LEVEL_ERR, template, *args)
```

### Comparing `krutils-0.20230407.1511/krutils/dbmgr.py` & `krutils-0.20230411.1411/krutils/dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230407.1511/setup.py` & `krutils-0.20230411.1411/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230407.1511",
+    version="0.20230411.1411",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

