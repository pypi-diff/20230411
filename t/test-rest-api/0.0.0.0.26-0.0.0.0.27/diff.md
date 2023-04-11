# Comparing `tmp/test_rest_api-0.0.0.0.26.tar.gz` & `tmp/test_rest_api-0.0.0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_rest_api-0.0.0.0.26.tar", last modified: Sat Apr  8 17:34:40 2023, max compression
+gzip compressed data, was "test_rest_api-0.0.0.0.27.tar", last modified: Tue Apr 11 07:20:02 2023, max compression
```

## Comparing `test_rest_api-0.0.0.0.26.tar` & `test_rest_api-0.0.0.0.27.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:34:40.631475 test_rest_api-0.0.0.0.26/
--rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.26/LICENSE
--rw-r--r--   0 trjose     (501) staff       (20)    64005 2023-04-08 17:34:40.630886 test_rest_api-0.0.0.0.26/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)    62282 2023-04-08 17:31:55.000000 test_rest_api-0.0.0.0.26/README.md
--rw-r--r--   0 trjose     (501) staff       (20)       38 2023-04-08 17:34:40.631678 test_rest_api-0.0.0.0.26/setup.cfg
--rw-r--r--   0 trjose     (501) staff       (20)     2917 2023-04-08 17:33:07.000000 test_rest_api-0.0.0.0.26/setup.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:34:40.609251 test_rest_api-0.0.0.0.26/test_rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)      236 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.26/test_rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1608 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.26/test_rest_api/__main__.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:34:40.614128 test_rest_api-0.0.0.0.26/test_rest_api/global_variables/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.26/test_rest_api/global_variables/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1161 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.26/test_rest_api/global_variables/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)     2716 2023-04-08 13:00:44.000000 test_rest_api-0.0.0.0.26/test_rest_api/global_variables/global_variables.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:34:40.615985 test_rest_api-0.0.0.0.26/test_rest_api/logger/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.26/test_rest_api/logger/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1237 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.26/test_rest_api/logger/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      848 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.26/test_rest_api/logger/logger.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:34:40.618206 test_rest_api-0.0.0.0.26/test_rest_api/reporting/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.26/test_rest_api/reporting/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)    34587 2023-04-07 17:27:51.000000 test_rest_api-0.0.0.0.26/test_rest_api/reporting/html.py
--rw-r--r--   0 trjose     (501) staff       (20)     5404 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.26/test_rest_api/reporting/report.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:34:40.621559 test_rest_api-0.0.0.0.26/test_rest_api/rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.26/test_rest_api/rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1824 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.26/test_rest_api/rest_api/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.26/test_rest_api/rest_api/method.py
--rw-r--r--   0 trjose     (501) staff       (20)      332 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.26/test_rest_api/rest_api/response.py
--rw-r--r--   0 trjose     (501) staff       (20)     6174 2023-04-08 13:55:22.000000 test_rest_api-0.0.0.0.26/test_rest_api/rest_api/rest_api.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:34:40.625173 test_rest_api-0.0.0.0.26/test_rest_api/testing/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.26/test_rest_api/testing/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     3904 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.26/test_rest_api/testing/bug.py
--rw-r--r--   0 trjose     (501) staff       (20)    14788 2023-04-08 13:49:13.000000 test_rest_api-0.0.0.0.26/test_rest_api/testing/decorator.py
--rw-r--r--   0 trjose     (501) staff       (20)      863 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.26/test_rest_api/testing/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)    13772 2023-04-07 17:27:51.000000 test_rest_api-0.0.0.0.26/test_rest_api/testing/runner.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:34:40.629772 test_rest_api-0.0.0.0.26/test_rest_api/utils/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.26/test_rest_api/utils/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.26/test_rest_api/utils/aiohttp_session.py
--rw-r--r--   0 trjose     (501) staff       (20)      546 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.26/test_rest_api/utils/colors.py
--rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.26/test_rest_api/utils/decorator_hints.py
--rw-r--r--   0 trjose     (501) staff       (20)     2027 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.26/test_rest_api/utils/error_msg.py
--rw-r--r--   0 trjose     (501) staff       (20)     1127 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.26/test_rest_api/utils/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.26/test_rest_api/utils/logger.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-08 17:34:40.612221 test_rest_api-0.0.0.0.26/test_rest_api.egg-info/
--rw-r--r--   0 trjose     (501) staff       (20)    64005 2023-04-08 17:34:40.000000 test_rest_api-0.0.0.0.26/test_rest_api.egg-info/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)     1175 2023-04-08 17:34:40.000000 test_rest_api-0.0.0.0.26/test_rest_api.egg-info/SOURCES.txt
--rw-r--r--   0 trjose     (501) staff       (20)        1 2023-04-08 17:34:40.000000 test_rest_api-0.0.0.0.26/test_rest_api.egg-info/dependency_links.txt
--rw-r--r--   0 trjose     (501) staff       (20)       29 2023-04-08 17:34:40.000000 test_rest_api-0.0.0.0.26/test_rest_api.egg-info/requires.txt
--rw-r--r--   0 trjose     (501) staff       (20)       14 2023-04-08 17:34:40.000000 test_rest_api-0.0.0.0.26/test_rest_api.egg-info/top_level.txt
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.226214 test_rest_api-0.0.0.0.27/
+-rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/LICENSE
+-rw-r--r--   0 trjose     (501) staff       (20)    64368 2023-04-11 07:20:02.225214 test_rest_api-0.0.0.0.27/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)    62645 2023-04-09 10:36:09.000000 test_rest_api-0.0.0.0.27/README.md
+-rw-r--r--   0 trjose     (501) staff       (20)       38 2023-04-11 07:20:02.226532 test_rest_api-0.0.0.0.27/setup.cfg
+-rw-r--r--   0 trjose     (501) staff       (20)     2917 2023-04-11 07:19:21.000000 test_rest_api-0.0.0.0.27/setup.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.199678 test_rest_api-0.0.0.0.27/test_rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)      236 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/test_rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1608 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/test_rest_api/__main__.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.203755 test_rest_api-0.0.0.0.27/test_rest_api/global_variables/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.27/test_rest_api/global_variables/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1161 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/test_rest_api/global_variables/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2716 2023-04-08 13:00:44.000000 test_rest_api-0.0.0.0.27/test_rest_api/global_variables/global_variables.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.205268 test_rest_api-0.0.0.0.27/test_rest_api/logger/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.27/test_rest_api/logger/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1237 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/test_rest_api/logger/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      850 2023-04-09 11:31:24.000000 test_rest_api-0.0.0.0.27/test_rest_api/logger/logger.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.207582 test_rest_api-0.0.0.0.27/test_rest_api/reporting/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.27/test_rest_api/reporting/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)    34587 2023-04-07 17:27:51.000000 test_rest_api-0.0.0.0.27/test_rest_api/reporting/html.py
+-rw-r--r--   0 trjose     (501) staff       (20)     5404 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/test_rest_api/reporting/report.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.212992 test_rest_api-0.0.0.0.27/test_rest_api/rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.27/test_rest_api/rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1824 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/test_rest_api/rest_api/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.27/test_rest_api/rest_api/method.py
+-rw-r--r--   0 trjose     (501) staff       (20)      332 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.27/test_rest_api/rest_api/response.py
+-rw-r--r--   0 trjose     (501) staff       (20)     6226 2023-04-09 11:13:23.000000 test_rest_api-0.0.0.0.27/test_rest_api/rest_api/rest_api.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.217184 test_rest_api-0.0.0.0.27/test_rest_api/testing/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.27/test_rest_api/testing/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     3904 2023-04-09 10:39:13.000000 test_rest_api-0.0.0.0.27/test_rest_api/testing/bug.py
+-rw-r--r--   0 trjose     (501) staff       (20)    14788 2023-04-08 13:49:13.000000 test_rest_api-0.0.0.0.27/test_rest_api/testing/decorator.py
+-rw-r--r--   0 trjose     (501) staff       (20)      863 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.27/test_rest_api/testing/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)    13772 2023-04-07 17:27:51.000000 test_rest_api-0.0.0.0.27/test_rest_api/testing/runner.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.223390 test_rest_api-0.0.0.0.27/test_rest_api/utils/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.27/test_rest_api/utils/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.27/test_rest_api/utils/aiohttp_session.py
+-rw-r--r--   0 trjose     (501) staff       (20)      546 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.27/test_rest_api/utils/colors.py
+-rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.27/test_rest_api/utils/decorator_hints.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2027 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.27/test_rest_api/utils/error_msg.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1127 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.27/test_rest_api/utils/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.27/test_rest_api/utils/logger.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-11 07:20:02.202379 test_rest_api-0.0.0.0.27/test_rest_api.egg-info/
+-rw-r--r--   0 trjose     (501) staff       (20)    64368 2023-04-11 07:20:02.000000 test_rest_api-0.0.0.0.27/test_rest_api.egg-info/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)     1175 2023-04-11 07:20:02.000000 test_rest_api-0.0.0.0.27/test_rest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 trjose     (501) staff       (20)        1 2023-04-11 07:20:02.000000 test_rest_api-0.0.0.0.27/test_rest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       29 2023-04-11 07:20:02.000000 test_rest_api-0.0.0.0.27/test_rest_api.egg-info/requires.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       14 2023-04-11 07:20:02.000000 test_rest_api-0.0.0.0.27/test_rest_api.egg-info/top_level.txt
```

### Comparing `test_rest_api-0.0.0.0.26/LICENSE` & `test_rest_api-0.0.0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/PKG-INFO` & `test_rest_api-0.0.0.0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_rest_api
-Version: 0.0.0.0.26
+Version: 0.0.0.0.27
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
 Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
 Project-URL: Source, https://github.com/troymjose/test_rest_api
 Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
@@ -166,24 +166,27 @@
 - Tests like login, logout etc. are __perfect candidates__ for #ALL
 
 <h4 id="5-project-structure">5. Project structure</h4>
 
 - - -
 
 ```
-.
+my_project
+│── __init__.py                   # Python module
 ├── api                           # Store all your rest api files
+│   │── __init__.py               # Python module
 │   ├── auth                      # Custom structure for subfolders & files
 │   │   ├── login.py              # Python file to store rest_api code
 │   │   │   ├── def user_login()  # Python function to create rest_api
 │   │   │   ├── def admin_login()
 │   │   │   └── ...    
 │   │   └── ...
 │   └── ...
 ├── testsuite                     # Root testsuite folder
+│   │── __init__.py               # Python module
 │   ├── auth                      # Custom structure for subfolders & files
 │   │   ├── login.py              # Python file as testsuite to store tests
 │   │   │   ├── async def t001()  # Python async function as testcases
 │   │   │   ├── async def t002()
 │   │   │   └── ...    
 │   │   └── ...
 │   └── ...
@@ -274,15 +277,17 @@
     - Mandatory: False
     - Data Type: bool
     - Expected: True or False. Provide False, to run tests sequentially
     - Default: True
 - __execution_order__
     - Mandatory: False
     - Data Type: str
-    - Expected: Custom text for ordering. This will work only when is_async = False
+    - Expected: Custom text for ordering. This will work only when is_async = False. Execution order '14' will run
+      before '2' even though the number 2 is less than 14. This is because execution_order uses alphabetic string
+      ordering & not number ordering
     - Default: 'zzzzz'
 
 <h4 id="3-my-first-logger">3. My first logger</h4>
 
 - - -
 
 ```python
```

### Comparing `test_rest_api-0.0.0.0.26/README.md` & `test_rest_api-0.0.0.0.27/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -135,24 +135,27 @@
 - Tests like login, logout etc. are __perfect candidates__ for #ALL
 
 <h4 id="5-project-structure">5. Project structure</h4>
 
 - - -
 
 ```
-.
+my_project
+│── __init__.py                   # Python module
 ├── api                           # Store all your rest api files
+│   │── __init__.py               # Python module
 │   ├── auth                      # Custom structure for subfolders & files
 │   │   ├── login.py              # Python file to store rest_api code
 │   │   │   ├── def user_login()  # Python function to create rest_api
 │   │   │   ├── def admin_login()
 │   │   │   └── ...    
 │   │   └── ...
 │   └── ...
 ├── testsuite                     # Root testsuite folder
+│   │── __init__.py               # Python module
 │   ├── auth                      # Custom structure for subfolders & files
 │   │   ├── login.py              # Python file as testsuite to store tests
 │   │   │   ├── async def t001()  # Python async function as testcases
 │   │   │   ├── async def t002()
 │   │   │   └── ...    
 │   │   └── ...
 │   └── ...
@@ -243,15 +246,17 @@
     - Mandatory: False
     - Data Type: bool
     - Expected: True or False. Provide False, to run tests sequentially
     - Default: True
 - __execution_order__
     - Mandatory: False
     - Data Type: str
-    - Expected: Custom text for ordering. This will work only when is_async = False
+    - Expected: Custom text for ordering. This will work only when is_async = False. Execution order '14' will run
+      before '2' even though the number 2 is less than 14. This is because execution_order uses alphabetic string
+      ordering & not number ordering
     - Default: 'zzzzz'
 
 <h4 id="3-my-first-logger">3. My first logger</h4>
 
 - - -
 
 ```python
```

### Comparing `test_rest_api-0.0.0.0.26/setup.py` & `test_rest_api-0.0.0.0.27/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Get README.md details
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
 # Setup
 setup(name='test_rest_api',
-      version='0.0.0.0.26',
+      version='0.0.0.0.27',
       author='Troy M Jose',
       author_email='',
       url='https://github.com/troymjose/test_rest_api',
       bugtrack_url='https://github.com/troymjose/test_rest_api/issues',
       project_urls={
           'Source': 'https://github.com/troymjose/test_rest_api',
           'Tracker': 'https://github.com/troymjose/test_rest_api/issues',
```

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/__main__.py` & `test_rest_api-0.0.0.0.27/test_rest_api/__main__.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/global_variables/exception.py` & `test_rest_api-0.0.0.0.27/test_rest_api/global_variables/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/global_variables/global_variables.py` & `test_rest_api-0.0.0.0.27/test_rest_api/global_variables/global_variables.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/logger/exception.py` & `test_rest_api-0.0.0.0.27/test_rest_api/logger/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/logger/logger.py` & `test_rest_api-0.0.0.0.27/test_rest_api/logger/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,8 +20,12 @@
         # Validate the message type
         if not isinstance(message, str):
             raise Exception('Invalid data type for message. Please provide a valid string')
         # Update the message tp Logger._logs instance variable with current time stamp
         self._logs += f'{datetime.now().strftime("%H:%M:%S") : <8}: {message}\n'
 
     def __str__(self):
-        return f'LOGS\n----\n{self._logs}\n'
+        return f'''
+LOGS
+----
+{self._logs}
+'''
```

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/reporting/html.py` & `test_rest_api-0.0.0.0.27/test_rest_api/reporting/html.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/reporting/report.py` & `test_rest_api-0.0.0.0.27/test_rest_api/reporting/report.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/rest_api/exception.py` & `test_rest_api-0.0.0.0.27/test_rest_api/rest_api/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/rest_api/rest_api.py` & `test_rest_api-0.0.0.0.27/test_rest_api/rest_api/rest_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,20 +79,19 @@
         self.parameters = parameters
         self.headers = headers
         self.body = body
         # Aiohttp variables
         self._session = AioHttpSession()
 
     def __str__(self):
-        return f"""
-Url:        {self.url}
-Headers:    {self.headers}
-Parameters: {self.parameters}
-Body:       {self.body}
-"""
+        return f"""Rest Api Info
+          Url:        {self.url}
+          Headers:    {self.headers}
+          Parameters: {self.parameters}
+          Body:       {self.body}"""
 
     async def send(self, method: str):
         """
         Send the rest api by providing the request method
         """
         try:
             # Check if method is of type string
```

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/testing/bug.py` & `test_rest_api-0.0.0.0.27/test_rest_api/testing/bug.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -75,21 +75,21 @@
     Class for creating a bug
     """
     PRIORITY = BugPriority()
 
     def __init__(self,
                  message: str = "",
                  priority: str = BugPriority.LOW,
-                 actual_result: str = "",
                  expected_result: str = "",
+                 actual_result: str = "",
                  steps_to_reproduce: str = ""):
         self.message = message
         self.priority = priority
-        self.actual_result = actual_result
         self.expected_result = expected_result
+        self.actual_result = actual_result
         self.steps_to_reproduce = steps_to_reproduce
 
 
 class BugException(Exception):
     """
     Exception raised when a Bug class instance is created.
     """
@@ -102,20 +102,20 @@
 ---------
 {bug.message.strip() if bug.message else self._no_data_to_display}
 
 PRIORITY
 ---------
 {bug.priority.strip() if bug.priority else self._no_data_to_display}
 
-ACTUAL RESULT
----------
-{bug.actual_result.strip() if bug.actual_result else self._no_data_to_display}
-
 EXPECTED RESULT
 ---------
 {bug.expected_result.strip() if bug.expected_result else self._no_data_to_display}
 
+ACTUAL RESULT
+---------
+{bug.actual_result.strip() if bug.actual_result else self._no_data_to_display}
+
 STEPS TO REPRODUCE
 -------------
 {bug.steps_to_reproduce.strip() if bug.steps_to_reproduce else self._no_data_to_display}
 """
         super().__init__(self.message)
```

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/testing/decorator.py` & `test_rest_api-0.0.0.0.27/test_rest_api/testing/decorator.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/testing/exception.py` & `test_rest_api-0.0.0.0.27/test_rest_api/testing/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/testing/runner.py` & `test_rest_api-0.0.0.0.27/test_rest_api/testing/runner.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/utils/aiohttp_session.py` & `test_rest_api-0.0.0.0.27/test_rest_api/utils/aiohttp_session.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/utils/colors.py` & `test_rest_api-0.0.0.0.27/test_rest_api/utils/colors.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/utils/error_msg.py` & `test_rest_api-0.0.0.0.27/test_rest_api/utils/error_msg.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/utils/exception.py` & `test_rest_api-0.0.0.0.27/test_rest_api/utils/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api/utils/logger.py` & `test_rest_api-0.0.0.0.27/test_rest_api/utils/logger.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api.egg-info/PKG-INFO` & `test_rest_api-0.0.0.0.27/test_rest_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-rest-api
-Version: 0.0.0.0.26
+Version: 0.0.0.0.27
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
 Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
 Project-URL: Source, https://github.com/troymjose/test_rest_api
 Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
@@ -166,24 +166,27 @@
 - Tests like login, logout etc. are __perfect candidates__ for #ALL
 
 <h4 id="5-project-structure">5. Project structure</h4>
 
 - - -
 
 ```
-.
+my_project
+│── __init__.py                   # Python module
 ├── api                           # Store all your rest api files
+│   │── __init__.py               # Python module
 │   ├── auth                      # Custom structure for subfolders & files
 │   │   ├── login.py              # Python file to store rest_api code
 │   │   │   ├── def user_login()  # Python function to create rest_api
 │   │   │   ├── def admin_login()
 │   │   │   └── ...    
 │   │   └── ...
 │   └── ...
 ├── testsuite                     # Root testsuite folder
+│   │── __init__.py               # Python module
 │   ├── auth                      # Custom structure for subfolders & files
 │   │   ├── login.py              # Python file as testsuite to store tests
 │   │   │   ├── async def t001()  # Python async function as testcases
 │   │   │   ├── async def t002()
 │   │   │   └── ...    
 │   │   └── ...
 │   └── ...
@@ -274,15 +277,17 @@
     - Mandatory: False
     - Data Type: bool
     - Expected: True or False. Provide False, to run tests sequentially
     - Default: True
 - __execution_order__
     - Mandatory: False
     - Data Type: str
-    - Expected: Custom text for ordering. This will work only when is_async = False
+    - Expected: Custom text for ordering. This will work only when is_async = False. Execution order '14' will run
+      before '2' even though the number 2 is less than 14. This is because execution_order uses alphabetic string
+      ordering & not number ordering
     - Default: 'zzzzz'
 
 <h4 id="3-my-first-logger">3. My first logger</h4>
 
 - - -
 
 ```python
```

### Comparing `test_rest_api-0.0.0.0.26/test_rest_api.egg-info/SOURCES.txt` & `test_rest_api-0.0.0.0.27/test_rest_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

