# Comparing `tmp/ats_case-0.4.0.tar.gz` & `tmp/ats_case-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.4.0.tar", last modified: Mon Apr 10 01:57:22 2023, max compression
+gzip compressed data, was "ats_case-0.4.1.tar", last modified: Tue Apr 11 03:21:31 2023, max compression
```

## Comparing `ats_case-0.4.0.tar` & `ats_case-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 01:57:22.018436 ats_case-0.4.0/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.4.0/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-10 01:57:22.014444 ats_case-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 01:57:21.455945 ats_case-0.4.0/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.4.0/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:57:21.738186 ats_case-0.4.0/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.4.0/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17006 2023-04-10 01:53:21.000000 ats_case-0.4.0/ats_case/case/command.py
--rw-rw-rw-   0        0        0    10103 2023-04-07 01:41:51.000000 ats_case-0.4.0/ats_case/case/context.py
--rw-rw-rw-   0        0        0     4644 2023-04-07 01:42:05.000000 ats_case-0.4.0/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5448 2023-04-07 01:42:16.000000 ats_case-0.4.0/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:57:21.851879 ats_case-0.4.0/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.4.0/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      366 2023-02-21 08:40:11.000000 ats_case-0.4.0/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      203 2023-02-11 01:58:18.000000 ats_case-0.4.0/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:57:21.935655 ats_case-0.4.0/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.0/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.4.0/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     2584 2023-04-10 01:54:51.000000 ats_case-0.4.0/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:57:21.990506 ats_case-0.4.0/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.0/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-02-23 05:48:08.000000 ats_case-0.4.0/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-10 01:57:21.577618 ats_case-0.4.0/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-10 01:57:20.000000 ats_case-0.4.0/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-10 01:57:20.000000 ats_case-0.4.0/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 01:57:20.000000 ats_case-0.4.0/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-10 01:57:20.000000 ats_case-0.4.0/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-10 01:57:20.000000 ats_case-0.4.0/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 01:57:22.018436 ats_case-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      916 2023-04-10 01:56:57.000000 ats_case-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:31.625325 ats_case-0.4.1/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-11 03:21:31.618344 ats_case-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:31.092851 ats_case-0.4.1/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.4.1/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:31.304100 ats_case-0.4.1/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.4.1/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17233 2023-04-11 03:13:22.000000 ats_case-0.4.1/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    10103 2023-04-07 01:41:51.000000 ats_case-0.4.1/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     4644 2023-04-07 01:42:05.000000 ats_case-0.4.1/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5435 2023-04-10 06:53:43.000000 ats_case-0.4.1/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:31.491562 ats_case-0.4.1/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.4.1/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      381 2023-04-10 07:20:19.000000 ats_case-0.4.1/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      628 2023-04-11 03:13:44.000000 ats_case-0.4.1/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:31.561223 ats_case-0.4.1/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.1/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.4.1/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     2584 2023-04-10 01:54:51.000000 ats_case-0.4.1/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:31.600079 ats_case-0.4.1/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.1/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2334 2023-04-11 02:59:20.000000 ats_case-0.4.1/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-11 03:21:31.185604 ats_case-0.4.1/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-11 03:21:30.000000 ats_case-0.4.1/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-11 03:21:30.000000 ats_case-0.4.1/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 03:21:30.000000 ats_case-0.4.1/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-11 03:21:30.000000 ats_case-0.4.1/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-11 03:21:30.000000 ats_case-0.4.1/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 03:21:31.625325 ats_case-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      916 2023-04-11 03:14:31.000000 ats_case-0.4.1/setup.py
```

### Comparing `ats_case-0.4.0/PKG-INFO` & `ats_case-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.4.0
+Version: 0.4.1
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.4.0/README.md` & `ats_case-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.0/ats_case/case/command.py` & `ats_case-0.4.1/ats_case/case/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from ats_base.common import func
 from ats_base.log.logger import logger
 from ats_base.service import app, pro, em, udm, mm
 
 from ats_case.case.context import Context
 from ats_case.common.enum import ProClazz, OperationClazz
-from ats_case.common.error import APIError
+from ats_case.common.error import APIError, ClientReturnError
 
 """
     常用操作命令
 """
 
 
 def send(context: Context, todo: dict, types=2, retry_times: int = 3):
@@ -216,14 +216,19 @@
                                         addition=self._addition, security=self._security, session_key=context.session.basename))
         logger.info('~ @PRO-ENCODE<- protocol:{} frame:{}'.format(self._protocol, parse.get('frame')))
 
         self._frame = parse.get('frame')
         return self._frame
 
     def decode(self, context: Context):
+        if self._frame is None or len(self._frame) <= 0:
+            cre = ClientReturnError(self._frame)
+            client().operation("app:error").message(str(cre))
+            raise cre
+
         logger.info('~ @PRO-DECODE-> protocol:{} frame:{}'.format(self._protocol, self._frame))
         data = pro.decode(func.to_dict(protocol=self._protocol.name, frame=self._frame, session_key=context.session.basename))
         logger.info('~ @PRO-DECODE<- protocol:{} parse:{}'.format(self._protocol, data))
 
         self._handle_framing(context, data)
 
         self._parse = data.get('parse').get('link_data').get('mission').get('result')
@@ -273,15 +278,17 @@
 
         return result
 
     def exec(self, context: Context):
         self.encode(context)
         result = send(context,
                       todo={'meter:comm': {'channel': {'type': 'RS485', 'baudrate': 9600}, 'frame': self._frame}})
+
         self._frame = result.get('result')
+        
         self.decode(context)
 
         self._flush(context)
 
         send(context, todo={'app:show': {'msg': self.acv(context)}})
```

### Comparing `ats_case-0.4.0/ats_case/case/context.py` & `ats_case-0.4.1/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.0/ats_case/case/executor.py` & `ats_case-0.4.1/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.0/ats_case/case/translator.py` & `ats_case-0.4.1/ats_case/case/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 # if self._contain_keyword(step):
                 #     tab_count += 1
                 f.write(self._gen_line(2))
 
             return steps
 
     def _script(self):
-        user_dir = func.makeDir(os.environ.get('PROJECT_DIR'), 'script', 'debug', self._context.tester.username)
+        user_dir = func.makeDir(os.getenv('PWD'), 'script', 'debug', self._context.tester.username)
         script_file = os.path.join(user_dir, 'steps.py')
 
         if not os.path.exists(user_dir):
             Path(user_dir).mkdir(parents=True, exist_ok=True)
 
         return script_file
```

### Comparing `ats_case-0.4.0/ats_case/manage/core.py` & `ats_case-0.4.1/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.0/ats_case/manage/start.py` & `ats_case-0.4.1/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.0/ats_case/template/testcase_v1.tmp` & `ats_case-0.4.1/ats_case/template/testcase_v1.tmp`

 * *Files 3% similar despite different names*

```diff
@@ -47,7 +47,11 @@
         logger.info('~ @TCC-MSG-> SCRIPT START -mode "{}" -client "{}"'.
                     format(CaseContext.mode, CaseContext.tester.api))
         try:
             executor.execute(CaseContext)
         except APIError as ae:
             logger.info(str(ae))
             raise AssertionError(str(ae))
+        except ClientReturnError as ce:
+            logger.info(str(ce))
+            raise AssertionError(str(ce))
+
```

### Comparing `ats_case-0.4.0/ats_case.egg-info/PKG-INFO` & `ats_case-0.4.1/ats_case.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.4.0
+Version: 0.4.1
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.4.0/ats_case.egg-info/SOURCES.txt` & `ats_case-0.4.1/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.0/setup.py` & `ats_case-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.4.0",
+    version="0.4.1",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

