# Comparing `tmp/cmdint-3.0.4.tar.gz` & `tmp/cmdint-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdint-3.0.4.tar", last modified: Thu Apr  6 19:07:32 2023, max compression
+gzip compressed data, was "cmdint-3.0.5.tar", last modified: Tue Apr 11 07:48:47 2023, max compression
```

## Comparing `cmdint-3.0.4.tar` & `cmdint-3.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-04-06 19:07:32.327518 cmdint-3.0.4/
--rw-rw-r--   0 neher     (1000) neher     (1000)    10172 2022-09-28 07:02:18.000000 cmdint-3.0.4/LICENSE
--rw-rw-r--   0 neher     (1000) neher     (1000)       37 2022-09-28 07:02:18.000000 cmdint-3.0.4/MANIFEST.in
--rw-rw-r--   0 neher     (1000) neher     (1000)      772 2023-04-06 19:07:32.327518 cmdint-3.0.4/PKG-INFO
--rw-rw-r--   0 neher     (1000) neher     (1000)     5890 2022-09-28 07:02:18.000000 cmdint-3.0.4/Readme.md
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-04-06 19:07:32.327518 cmdint-3.0.4/cmdint/
--rw-rw-r--   0 neher     (1000) neher     (1000)    46797 2023-04-06 18:57:45.000000 cmdint-3.0.4/cmdint/CmdInterface.py
--rw-rw-r--   0 neher     (1000) neher     (1000)     3723 2022-09-28 07:02:18.000000 cmdint-3.0.4/cmdint/MessageLogger.py
--rw-rw-r--   0 neher     (1000) neher     (1000)     6727 2022-09-28 07:09:09.000000 cmdint-3.0.4/cmdint/Utils.py
--rw-rw-r--   0 neher     (1000) neher     (1000)      201 2023-04-06 19:07:24.000000 cmdint-3.0.4/cmdint/__init__.py
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-04-06 19:07:32.327518 cmdint-3.0.4/cmdint.egg-info/
--rw-rw-r--   0 neher     (1000) neher     (1000)      772 2023-04-06 19:07:32.000000 cmdint-3.0.4/cmdint.egg-info/PKG-INFO
--rw-rw-r--   0 neher     (1000) neher     (1000)      298 2023-04-06 19:07:32.000000 cmdint-3.0.4/cmdint.egg-info/SOURCES.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)        1 2023-04-06 19:07:32.000000 cmdint-3.0.4/cmdint.egg-info/dependency_links.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)        1 2022-09-29 13:25:31.000000 cmdint-3.0.4/cmdint.egg-info/not-zip-safe
--rw-rw-r--   0 neher     (1000) neher     (1000)       67 2023-04-06 19:07:32.000000 cmdint-3.0.4/cmdint.egg-info/requires.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)        7 2023-04-06 19:07:32.000000 cmdint-3.0.4/cmdint.egg-info/top_level.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)       38 2023-04-06 19:07:32.327518 cmdint-3.0.4/setup.cfg
--rw-rw-r--   0 neher     (1000) neher     (1000)     1078 2023-04-06 19:07:24.000000 cmdint-3.0.4/setup.py
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-04-11 07:48:47.701757 cmdint-3.0.5/
+-rw-rw-r--   0 neher     (1000) neher     (1000)    10172 2022-09-28 07:02:18.000000 cmdint-3.0.5/LICENSE
+-rw-rw-r--   0 neher     (1000) neher     (1000)       37 2022-09-28 07:02:18.000000 cmdint-3.0.5/MANIFEST.in
+-rw-rw-r--   0 neher     (1000) neher     (1000)      772 2023-04-11 07:48:47.701757 cmdint-3.0.5/PKG-INFO
+-rw-rw-r--   0 neher     (1000) neher     (1000)     5890 2022-09-28 07:02:18.000000 cmdint-3.0.5/Readme.md
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-04-11 07:48:47.701757 cmdint-3.0.5/cmdint/
+-rw-rw-r--   0 neher     (1000) neher     (1000)    47872 2023-04-11 07:47:26.000000 cmdint-3.0.5/cmdint/CmdInterface.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)     3723 2022-09-28 07:02:18.000000 cmdint-3.0.5/cmdint/MessageLogger.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)     6727 2022-09-28 07:09:09.000000 cmdint-3.0.5/cmdint/Utils.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)      201 2023-04-11 07:48:39.000000 cmdint-3.0.5/cmdint/__init__.py
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-04-11 07:48:47.701757 cmdint-3.0.5/cmdint.egg-info/
+-rw-rw-r--   0 neher     (1000) neher     (1000)      772 2023-04-11 07:48:47.000000 cmdint-3.0.5/cmdint.egg-info/PKG-INFO
+-rw-rw-r--   0 neher     (1000) neher     (1000)      298 2023-04-11 07:48:47.000000 cmdint-3.0.5/cmdint.egg-info/SOURCES.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)        1 2023-04-11 07:48:47.000000 cmdint-3.0.5/cmdint.egg-info/dependency_links.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)        1 2022-09-29 13:25:31.000000 cmdint-3.0.5/cmdint.egg-info/not-zip-safe
+-rw-rw-r--   0 neher     (1000) neher     (1000)       67 2023-04-11 07:48:47.000000 cmdint-3.0.5/cmdint.egg-info/requires.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)        7 2023-04-11 07:48:47.000000 cmdint-3.0.5/cmdint.egg-info/top_level.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)       38 2023-04-11 07:48:47.701757 cmdint-3.0.5/setup.cfg
+-rw-rw-r--   0 neher     (1000) neher     (1000)     1078 2023-04-11 07:48:39.000000 cmdint-3.0.5/setup.py
```

### Comparing `cmdint-3.0.4/LICENSE` & `cmdint-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdint-3.0.4/PKG-INFO` & `cmdint-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdint
-Version: 3.0.4
+Version: 3.0.5
 Summary: Enables detailed logging of command line calls in a very lightweight manner.
 Home-page: https://github.com/MIC-DKFZ/cmdint/
 Author: Peter F. Neher
 Author-email: p.neher@dkfz.de
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cmdint-3.0.4/Readme.md` & `cmdint-3.0.5/Readme.md`

 * *Files identical despite different names*

### Comparing `cmdint-3.0.4/cmdint/CmdInterface.py` & `cmdint-3.0.5/cmdint/CmdInterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import git
 import hashlib
 import inspect
 import json
 import io
 import chardet
 from pathlib import Path
-from shutil import which
+from shutil import which, move
 from cmdint.Utils import *
 from cmdint import MessageLogger
 import tarfile
 import uuid
 
 
 class CmdInterface:
@@ -503,15 +503,15 @@
 
         if tar is not None:
             tar.close()
 
         start_time = datetime.now()
         self.__log['time']['start'] = start_time.strftime("%Y-%m-%d %H:%M:%S")
         self.__log['time']['utc_offset'] = time.localtime().tm_gmtoff
-        CmdInterface.log_message(self.__log['name'] + ' START')
+        CmdInterface.log_message('START: ' + self.__log['name'] + ', ' + self.__log['description'])
         if CmdInterface.__message_log_level == MessageLogLevel.START_AND_END_MESSAGES and not self.__silent:
             CmdInterface.send_message('START ' + self.__log['name'])
         return start_time
 
     def __log_end(self, start_time: datetime, return_code: int) -> datetime:
         """
         Log end time and duration of command execution:
@@ -530,15 +530,15 @@
         hours, remainder = divmod(duration.seconds, 3600)
         hours += duration.days * 24
         minutes, seconds = divmod(remainder, 60)
         duration_formatted = '%d:%02d:%02d' % (hours, minutes, seconds)
         self.__log['time']['duration'] = duration_formatted
 
         # log end messages & return code
-        CmdInterface.log_message(self.__log['name'] + ' END')
+        CmdInterface.log_message('END: ' + self.__log['name'] + ', ' + self.__log['description'])
         if (CmdInterface.__throw_on_error or CmdInterface.__exit_on_error) and return_code <= 0:
             print('EXCEPTION:', self.__log['name'], self.__log['description'])
             CmdInterface.log_message('Exiting due to error: ' + self.__return_code_meanings[return_code])
         self.__log['return_code'] = return_code
         self.update_log()
 
         if not self.__silent and \
@@ -844,15 +844,30 @@
 
         log = list()
 
         try:
             if os.path.isfile(logfile_name):
                 with open(logfile_name) as f:
                     log = json.load(f)
+        except json.decoder.JSONDecodeError as err:
+            print('Error decoding logfile: ' + logfile_name)
+            print('Exception: ' + str(err))
+            print(err.args)
+            print('Creating backup of logfile and starting new one ...')
+            copy_id = 1
+            try:
+                while os.path.exists(logfile_name + '.bak' + str(copy_id)):
+                    copy_id += 1
+                move(logfile_name, logfile_name + '.bak' + str(copy_id))
+            except Exception as err:
+                print('Error creating backup of logfile: ' + logfile_name)
+                print('Exception: ' + str(err))
+                print(err.args)
         except Exception as err:
+            print('Error accessing logfile: ' + logfile_name)
             print('Exception: ' + str(err))
             print(err.args)
 
         return log
 
     @staticmethod
     def anonymize_log(out_log_name: str = None,
@@ -888,14 +903,15 @@
                 file_content = f.read()
                 for cl in clear_strings:
                     file_content = file_content.replace(cl, '')
 
             with open(out_log_name, 'w') as f:
                 f.write(file_content)
         except Exception as err:
+            print('Error anonymizing logfile: ' + CmdInterface.__logfile_name)
             print('Exception: ' + str(err))
             print(err.args)
 
         try:
             data = list()
             if os.path.isfile(out_log_name):
                 with open(out_log_name) as f:
@@ -913,14 +929,15 @@
                 del run_log['environment']['platform']['node']
                 if 'ip' in run_log['environment']['platform'].keys():
                     del run_log['environment']['platform']['ip']
             with open(out_log_name, 'w') as f:
                 j = json.dumps(data, indent=2, sort_keys=False)
                 f.write(j)
         except Exception as err:
+            print('Error anonymizing logfile: ' + out_log_name)
             print('Exception: ' + str(err))
             print(err.args)
 
         for file in files_to_clear:
             if os.path.isfile(file):
                 print('Anonymizing ' + file)
                 try:
@@ -929,23 +946,25 @@
                         for cl in clear_strings:
                             file_content = file_content.replace(cl, '')
 
                     with open(file, 'w') as f:
                         f.write(file_content)
 
                 except Exception as err:
+                    print('Error anonymizing file: ' + file)
                     print('Exception: ' + str(err))
                     print(err.args)
 
         for file in files_to_delete:
             if os.path.isfile(file):
                 print('Removing ' + file)
                 try:
                     os.remove(file)
                 except Exception as err:
+                    print('Error removing file: ' + file)
                     print('Exception: ' + str(err))
                     print(err.args)
 
     def run(self, version_arg: str = None,
             pre_command: str = None,
             check_input: list = None,
             check_output: list = None,
```

### Comparing `cmdint-3.0.4/cmdint/MessageLogger.py` & `cmdint-3.0.5/cmdint/MessageLogger.py`

 * *Files identical despite different names*

### Comparing `cmdint-3.0.4/cmdint/Utils.py` & `cmdint-3.0.5/cmdint/Utils.py`

 * *Files identical despite different names*

### Comparing `cmdint-3.0.4/cmdint.egg-info/PKG-INFO` & `cmdint-3.0.5/cmdint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdint
-Version: 3.0.4
+Version: 3.0.5
 Summary: Enables detailed logging of command line calls in a very lightweight manner.
 Home-page: https://github.com/MIC-DKFZ/cmdint/
 Author: Peter F. Neher
 Author-email: p.neher@dkfz.de
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cmdint-3.0.4/setup.py` & `cmdint-3.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='cmdint',
-      version='3.0.4',
+      version='3.0.5',
       description='Enables detailed logging of command line calls in a very lightweight manner.',
       long_description='CmdInterface enables detailed logging of command line and python experiments in a very lightweight manner (coding wise). It wraps your command line or python function calls in a few lines of code and logs everything you might need to reproduce the experiment later on or to simply check what you did a couple of years ago.',
       url='https://github.com/MIC-DKFZ/cmdint/',
       author='Peter F. Neher',
       author_email='p.neher@dkfz.de',
       license='Apache 2.0',
       packages=['cmdint'],
```

