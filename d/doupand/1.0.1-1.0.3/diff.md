# Comparing `tmp/doupand-1.0.1.tar.gz` & `tmp/doupand-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/doupand-1.0.1.tar", last modified: Sat Apr  8 17:46:46 2023, max compression
+gzip compressed data, was "dist/doupand-1.0.3.tar", last modified: Tue Apr 11 13:57:19 2023, max compression
```

## Comparing `doupand-1.0.1.tar` & `doupand-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-08 17:46:46.000000 doupand-1.0.1/
--rw-r--r--   0 tongjun    (501) staff       (20)     2041 2023-04-08 17:46:46.000000 doupand-1.0.1/PKG-INFO
--rw-r--r--   0 tongjun    (501) staff       (20)     1469 2023-04-07 19:08:40.000000 doupand-1.0.1/LICENSE
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand/
--rw-r--r--   0 tongjun    (501) staff       (20)      133 2023-04-08 17:33:37.000000 doupand-1.0.1/doupand/__init__.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand/utils/
--rw-r--r--   0 tongjun    (501) staff       (20)      701 2023-04-07 14:51:56.000000 doupand-1.0.1/doupand/utils/userauth.py
--rw-r--r--   0 tongjun    (501) staff       (20)        0 2023-04-06 17:18:45.000000 doupand-1.0.1/doupand/utils/__init__.py
--rw-r--r--   0 tongjun    (501) staff       (20)      277 2023-04-08 17:11:54.000000 doupand-1.0.1/doupand/utils/cons.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand/api/
--rw-r--r--   0 tongjun    (501) staff       (20)     3182 2023-04-08 17:45:25.000000 doupand-1.0.1/doupand/api/client.py
--rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-06 17:31:40.000000 doupand-1.0.1/doupand/api/__init__.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand.egg-info/
--rw-r--r--   0 tongjun    (501) staff       (20)     2041 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand.egg-info/PKG-INFO
--rw-r--r--   0 tongjun    (501) staff       (20)      310 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand.egg-info/SOURCES.txt
--rw-r--r--   0 tongjun    (501) staff       (20)       16 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand.egg-info/requires.txt
--rw-r--r--   0 tongjun    (501) staff       (20)        8 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand.egg-info/top_level.txt
--rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-08 17:46:46.000000 doupand-1.0.1/doupand.egg-info/dependency_links.txt
--rw-r--r--   0 tongjun    (501) staff       (20)     2427 2023-04-07 19:13:54.000000 doupand-1.0.1/setup.py
--rw-r--r--   0 tongjun    (501) staff       (20)       38 2023-04-08 17:46:46.000000 doupand-1.0.1/setup.cfg
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-11 13:57:19.000000 doupand-1.0.3/
+-rw-r--r--   0 tongjun    (501) staff       (20)     2041 2023-04-11 13:57:19.000000 doupand-1.0.3/PKG-INFO
+-rw-r--r--   0 tongjun    (501) staff       (20)     1469 2023-04-07 19:08:40.000000 doupand-1.0.3/LICENSE
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand/
+-rw-r--r--   0 tongjun    (501) staff       (20)      133 2023-04-08 17:33:37.000000 doupand-1.0.3/doupand/__init__.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand/utils/
+-rw-r--r--   0 tongjun    (501) staff       (20)      701 2023-04-07 14:51:56.000000 doupand-1.0.3/doupand/utils/userauth.py
+-rw-r--r--   0 tongjun    (501) staff       (20)        0 2023-04-06 17:18:45.000000 doupand-1.0.3/doupand/utils/__init__.py
+-rw-r--r--   0 tongjun    (501) staff       (20)      277 2023-04-08 17:11:54.000000 doupand-1.0.3/doupand/utils/cons.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand/api/
+-rw-r--r--   0 tongjun    (501) staff       (20)     3183 2023-04-11 13:54:16.000000 doupand-1.0.3/doupand/api/client.py
+-rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-06 17:31:40.000000 doupand-1.0.3/doupand/api/__init__.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/
+-rw-r--r--   0 tongjun    (501) staff       (20)     2041 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/PKG-INFO
+-rw-r--r--   0 tongjun    (501) staff       (20)      310 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/SOURCES.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)       16 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/requires.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)        8 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/top_level.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/dependency_links.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)     2400 2023-04-11 13:39:22.000000 doupand-1.0.3/setup.py
+-rw-r--r--   0 tongjun    (501) staff       (20)       38 2023-04-11 13:57:19.000000 doupand-1.0.3/setup.cfg
```

### Comparing `doupand-1.0.1/PKG-INFO` & `doupand-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doupand
-Version: 1.0.1
+Version: 1.0.3
 Summary: A simple and easy-to-use financial data interface library built for normal investors!
 Home-page: https://doupand.com
 Author: DouBro
 Author-email: doupand@163.com
 License: BSD
 Keywords: Financial Data Interface
 Platform: all
@@ -37,15 +37,15 @@
 --------------
 
     pip install doupand
 
 Upgrade
 ---------------
 
-    pip install doupand --upgrade
+    pip install --upgrade doupand
 
 Quick Start
 --------------
 
 ::
 
     import doupand as dp
```

### Comparing `doupand-1.0.1/LICENSE` & `doupand-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `doupand-1.0.1/doupand/utils/userauth.py` & `doupand-1.0.3/doupand/utils/userauth.py`

 * *Files identical despite different names*

### Comparing `doupand-1.0.1/doupand/api/client.py` & `doupand-1.0.3/doupand/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
             if os.path.exists(fp):
                 df = pd.read_csv(fp)
                 if cur_time < int(df.loc[0]['expire_time']):
                     self.__url_expire_time = int(df.loc[0]['expire_time'])
                     return str(df.loc[0]['http_url'])
 
-            res = requests.get(self.__distribution_url, timeout=10, headers={'Connection': 'close'})
+            res = requests.post(self.__distribution_url, timeout=10, headers={'Connection': 'close'})
             result = res.json()
             if result['status'] == "success":
                 self.__http_url = res.json()['result']
                 self.__url_expire_time = cur_time + 12 * 60 * 60
                 df = pd.DataFrame([[self.__http_url, self.__url_expire_time]], columns=['http_url', 'expire_time'])
                 df.to_csv(fp, index=False)
                 return self.__http_url
```

### Comparing `doupand-1.0.1/doupand.egg-info/PKG-INFO` & `doupand-1.0.3/doupand.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doupand
-Version: 1.0.1
+Version: 1.0.3
 Summary: A simple and easy-to-use financial data interface library built for normal investors!
 Home-page: https://doupand.com
 Author: DouBro
 Author-email: doupand@163.com
 License: BSD
 Keywords: Financial Data Interface
 Platform: all
@@ -37,15 +37,15 @@
 --------------
 
     pip install doupand
 
 Upgrade
 ---------------
 
-    pip install doupand --upgrade
+    pip install --upgrade doupand
 
 Quick Start
 --------------
 
 ::
 
     import doupand as dp
```

### Comparing `doupand-1.0.1/setup.py` & `doupand-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*-coding: utf-8 -*-
 # @Time    : 2023/4/8 02:39
 # @Description  : PIPY INFO
 
 from setuptools import find_packages, setup
-import doupand
 
 long_desc = """
 DouPand
 ===============
 
 * easy to use as most of the data returned are pandas DataFrame objects
 * can be easily saved as csv, excel or json files
@@ -24,15 +23,15 @@
 --------------
 
     pip install doupand
 
 Upgrade
 ---------------
 
-    pip install doupand --upgrade
+    pip install --upgrade doupand
 
 Quick Start
 --------------
 
 ::
 
     import doupand as dp
@@ -53,15 +52,15 @@
     5331  873305.BJ  873305  ...          BSE         北交所
     5332  873339.BJ  873339  ...          BSE         北交所
     5333  873527.BJ  873527  ...          BSE         北交所
 """
 
 setup(
     name='doupand',
-    version=doupand.__version__,
+    version="1.0.3",
     description='A simple and easy-to-use financial data interface library built for normal investors!',
     long_description=long_desc,
     author='DouBro',
     author_email='doupand@163.com',
     packages=find_packages(),
     platforms=["all"],
     license='BSD',
```

