# Comparing `tmp/easytradetesting-0.1.8.tar.gz` & `tmp/easytradetesting-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easytradetesting-0.1.8.tar", last modified: Wed Sep  7 12:09:46 2022, max compression
+gzip compressed data, was "dist/easytradetesting-0.1.9.tar", last modified: Wed Sep  7 12:14:43 2022, max compression
```

## Comparing `easytradetesting-0.1.8.tar` & `easytradetesting-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2022-09-07 12:09:46.576710 easytradetesting-0.1.8/
--rw-r--r--   0 josh       (501) staff       (20)     1070 2022-06-19 12:49:17.000000 easytradetesting-0.1.8/LICENSE.txt
--rw-r--r--   0 josh       (501) staff       (20)      666 2022-09-07 12:09:46.576476 easytradetesting-0.1.8/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)       41 2022-07-11 11:31:26.000000 easytradetesting-0.1.8/README.md
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2022-09-07 12:09:46.573924 easytradetesting-0.1.8/easytradetesting/
--rw-r--r--   0 josh       (501) staff       (20)     5293 2022-07-16 09:18:00.000000 easytradetesting-0.1.8/easytradetesting/BackTestContext.py
--rw-r--r--   0 josh       (501) staff       (20)     8466 2022-08-27 06:30:06.000000 easytradetesting-0.1.8/easytradetesting/BackTestEngine.py
--rw-r--r--   0 josh       (501) staff       (20)     2550 2022-07-16 14:18:13.000000 easytradetesting-0.1.8/easytradetesting/BackTestOrder.py
--rw-r--r--   0 josh       (501) staff       (20)     3707 2022-07-11 11:26:47.000000 easytradetesting-0.1.8/easytradetesting/BackTestResult.py
--rw-r--r--   0 josh       (501) staff       (20)     4598 2022-07-16 09:25:55.000000 easytradetesting-0.1.8/easytradetesting/DataFetcher.py
--rw-r--r--   0 josh       (501) staff       (20)     1679 2022-07-16 09:27:33.000000 easytradetesting-0.1.8/easytradetesting/DataSource.py
--rw-r--r--   0 josh       (501) staff       (20)    17480 2022-07-16 09:29:40.000000 easytradetesting-0.1.8/easytradetesting/MySqlDataSource.py
--rw-r--r--   0 josh       (501) staff       (20)        0 2022-06-20 07:04:25.000000 easytradetesting-0.1.8/easytradetesting/__init__.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2022-09-07 12:09:46.576216 easytradetesting-0.1.8/easytradetesting/api/
--rw-r--r--   0 josh       (501) staff       (20)     2860 2022-07-16 09:07:53.000000 easytradetesting-0.1.8/easytradetesting/api/MarketApi.py
--rw-r--r--   0 josh       (501) staff       (20)     5009 2022-08-30 13:33:46.000000 easytradetesting-0.1.8/easytradetesting/api/TradeApi.py
--rw-r--r--   0 josh       (501) staff       (20)        0 2022-06-20 07:04:25.000000 easytradetesting-0.1.8/easytradetesting/api/__init__.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2022-09-07 12:09:46.574953 easytradetesting-0.1.8/easytradetesting.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)      666 2022-09-07 12:09:46.000000 easytradetesting-0.1.8/easytradetesting.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)      597 2022-09-07 12:09:46.000000 easytradetesting-0.1.8/easytradetesting.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2022-09-07 12:09:46.000000 easytradetesting-0.1.8/easytradetesting.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)       52 2022-09-07 12:09:46.000000 easytradetesting-0.1.8/easytradetesting.egg-info/requires.txt
--rw-r--r--   0 josh       (501) staff       (20)       17 2022-09-07 12:09:46.000000 easytradetesting-0.1.8/easytradetesting.egg-info/top_level.txt
--rw-r--r--   0 josh       (501) staff       (20)       38 2022-09-07 12:09:46.576789 easytradetesting-0.1.8/setup.cfg
--rw-r--r--   0 josh       (501) staff       (20)     3837 2022-09-07 12:09:26.000000 easytradetesting-0.1.8/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2022-09-07 12:14:43.638154 easytradetesting-0.1.9/
+-rw-r--r--   0 josh       (501) staff       (20)     1070 2022-06-19 12:49:17.000000 easytradetesting-0.1.9/LICENSE.txt
+-rw-r--r--   0 josh       (501) staff       (20)      666 2022-09-07 12:14:43.637941 easytradetesting-0.1.9/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)       41 2022-07-11 11:31:26.000000 easytradetesting-0.1.9/README.md
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2022-09-07 12:14:43.635227 easytradetesting-0.1.9/easytradetesting/
+-rw-r--r--   0 josh       (501) staff       (20)     5293 2022-07-16 09:18:00.000000 easytradetesting-0.1.9/easytradetesting/BackTestContext.py
+-rw-r--r--   0 josh       (501) staff       (20)     8466 2022-08-27 06:30:06.000000 easytradetesting-0.1.9/easytradetesting/BackTestEngine.py
+-rw-r--r--   0 josh       (501) staff       (20)     2550 2022-07-16 14:18:13.000000 easytradetesting-0.1.9/easytradetesting/BackTestOrder.py
+-rw-r--r--   0 josh       (501) staff       (20)     3707 2022-07-11 11:26:47.000000 easytradetesting-0.1.9/easytradetesting/BackTestResult.py
+-rw-r--r--   0 josh       (501) staff       (20)     4598 2022-07-16 09:25:55.000000 easytradetesting-0.1.9/easytradetesting/DataFetcher.py
+-rw-r--r--   0 josh       (501) staff       (20)     1679 2022-07-16 09:27:33.000000 easytradetesting-0.1.9/easytradetesting/DataSource.py
+-rw-r--r--   0 josh       (501) staff       (20)    17480 2022-07-16 09:29:40.000000 easytradetesting-0.1.9/easytradetesting/MySqlDataSource.py
+-rw-r--r--   0 josh       (501) staff       (20)        0 2022-06-20 07:04:25.000000 easytradetesting-0.1.9/easytradetesting/__init__.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2022-09-07 12:14:43.637520 easytradetesting-0.1.9/easytradetesting/api/
+-rw-r--r--   0 josh       (501) staff       (20)     2860 2022-07-16 09:07:53.000000 easytradetesting-0.1.9/easytradetesting/api/MarketApi.py
+-rw-r--r--   0 josh       (501) staff       (20)     5009 2022-08-30 13:33:46.000000 easytradetesting-0.1.9/easytradetesting/api/TradeApi.py
+-rw-r--r--   0 josh       (501) staff       (20)        0 2022-06-20 07:04:25.000000 easytradetesting-0.1.9/easytradetesting/api/__init__.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2022-09-07 12:14:43.636488 easytradetesting-0.1.9/easytradetesting.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)      666 2022-09-07 12:14:43.000000 easytradetesting-0.1.9/easytradetesting.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)      597 2022-09-07 12:14:43.000000 easytradetesting-0.1.9/easytradetesting.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2022-09-07 12:14:43.000000 easytradetesting-0.1.9/easytradetesting.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)       52 2022-09-07 12:14:43.000000 easytradetesting-0.1.9/easytradetesting.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       17 2022-09-07 12:14:43.000000 easytradetesting-0.1.9/easytradetesting.egg-info/top_level.txt
+-rw-r--r--   0 josh       (501) staff       (20)       38 2022-09-07 12:14:43.638227 easytradetesting-0.1.9/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)     3837 2022-09-07 12:14:28.000000 easytradetesting-0.1.9/setup.py
```

### Comparing `easytradetesting-0.1.8/LICENSE.txt` & `easytradetesting-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easytradetesting-0.1.8/PKG-INFO` & `easytradetesting-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytradetesting
-Version: 0.1.8
+Version: 0.1.9
 Summary: The simple sdk for testing strategy
 Home-page: 
 Author: EasyTrade Tech Team
 Author-email: tech_team@easytrade.cloud
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `easytradetesting-0.1.8/easytradetesting/BackTestContext.py` & `easytradetesting-0.1.9/easytradetesting/BackTestContext.py`

 * *Files identical despite different names*

### Comparing `easytradetesting-0.1.8/easytradetesting/BackTestEngine.py` & `easytradetesting-0.1.9/easytradetesting/BackTestEngine.py`

 * *Files identical despite different names*

### Comparing `easytradetesting-0.1.8/easytradetesting/BackTestOrder.py` & `easytradetesting-0.1.9/easytradetesting/BackTestOrder.py`

 * *Files identical despite different names*

### Comparing `easytradetesting-0.1.8/easytradetesting/BackTestResult.py` & `easytradetesting-0.1.9/easytradetesting/BackTestResult.py`

 * *Files identical despite different names*

### Comparing `easytradetesting-0.1.8/easytradetesting/DataFetcher.py` & `easytradetesting-0.1.9/easytradetesting/DataFetcher.py`

 * *Files identical despite different names*

### Comparing `easytradetesting-0.1.8/easytradetesting/DataSource.py` & `easytradetesting-0.1.9/easytradetesting/DataSource.py`

 * *Files identical despite different names*

### Comparing `easytradetesting-0.1.8/easytradetesting/MySqlDataSource.py` & `easytradetesting-0.1.9/easytradetesting/MySqlDataSource.py`

 * *Files identical despite different names*

### Comparing `easytradetesting-0.1.8/easytradetesting/api/MarketApi.py` & `easytradetesting-0.1.9/easytradetesting/api/MarketApi.py`

 * *Files identical despite different names*

### Comparing `easytradetesting-0.1.8/easytradetesting/api/TradeApi.py` & `easytradetesting-0.1.9/easytradetesting/api/TradeApi.py`

 * *Files identical despite different names*

### Comparing `easytradetesting-0.1.8/easytradetesting.egg-info/PKG-INFO` & `easytradetesting-0.1.9/easytradetesting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytradetesting
-Version: 0.1.8
+Version: 0.1.9
 Summary: The simple sdk for testing strategy
 Home-page: 
 Author: EasyTrade Tech Team
 Author-email: tech_team@easytrade.cloud
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `easytradetesting-0.1.8/easytradetesting.egg-info/SOURCES.txt` & `easytradetesting-0.1.9/easytradetesting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easytradetesting-0.1.8/setup.py` & `easytradetesting-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # Package meta-data.
 NAME = 'easytradetesting'
 DESCRIPTION = 'The simple sdk for testing strategy'
 URL = ''
 EMAIL = 'tech_team@easytrade.cloud'
 AUTHOR = 'EasyTrade Tech Team'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    'easytradesdk >= 0.1.6', 'obspy', 'openpyxl', 'requests', 'pymysql'
+    'easytradesdk >= 0.1.7', 'obspy', 'openpyxl', 'requests', 'pymysql'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

