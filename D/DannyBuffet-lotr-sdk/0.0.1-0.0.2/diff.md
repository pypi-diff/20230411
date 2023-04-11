# Comparing `tmp/DannyBuffet-lotr-sdk-0.0.1.tar.gz` & `tmp/DannyBuffet-lotr-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DannyBuffet-lotr-sdk-0.0.1.tar", last modified: Tue Apr 11 20:10:09 2023, max compression
+gzip compressed data, was "DannyBuffet-lotr-sdk-0.0.2.tar", last modified: Tue Apr 11 20:30:43 2023, max compression
```

## Comparing `DannyBuffet-lotr-sdk-0.0.1.tar` & `DannyBuffet-lotr-sdk-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 20:10:09.893572 DannyBuffet-lotr-sdk-0.0.1/
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 20:10:09.891172 DannyBuffet-lotr-sdk-0.0.1/DannyBuffet_lotr_sdk.egg-info/
--rw-r--r--   0 dannyreliford   (501) staff       (20)     3080 2023-04-11 20:10:09.000000 DannyBuffet-lotr-sdk-0.0.1/DannyBuffet_lotr_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dannyreliford   (501) staff       (20)      424 2023-04-11 20:10:09.000000 DannyBuffet-lotr-sdk-0.0.1/DannyBuffet_lotr_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)        1 2023-04-11 20:10:09.000000 DannyBuffet-lotr-sdk-0.0.1/DannyBuffet_lotr_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)        9 2023-04-11 20:10:09.000000 DannyBuffet-lotr-sdk-0.0.1/DannyBuffet_lotr_sdk.egg-info/requires.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)       24 2023-04-11 20:10:09.000000 DannyBuffet-lotr-sdk-0.0.1/DannyBuffet_lotr_sdk.egg-info/top_level.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1071 2023-04-10 19:42:02.000000 DannyBuffet-lotr-sdk-0.0.1/LICENSE.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)     3080 2023-04-11 20:10:09.893412 DannyBuffet-lotr-sdk-0.0.1/PKG-INFO
--rw-r--r--   0 dannyreliford   (501) staff       (20)     2186 2023-04-11 20:04:05.000000 DannyBuffet-lotr-sdk-0.0.1/README.md
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 20:10:09.892515 DannyBuffet-lotr-sdk-0.0.1/lordoftheringssdk/
--rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-10 17:32:46.000000 DannyBuffet-lotr-sdk-0.0.1/lordoftheringssdk/__init__.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1533 2023-04-11 17:17:00.000000 DannyBuffet-lotr-sdk-0.0.1/lordoftheringssdk/api_methods.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)       72 2023-04-08 19:37:27.000000 DannyBuffet-lotr-sdk-0.0.1/lordoftheringssdk/conf.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1344 2023-04-10 18:31:09.000000 DannyBuffet-lotr-sdk-0.0.1/lordoftheringssdk/movie.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)      910 2023-04-11 14:23:38.000000 DannyBuffet-lotr-sdk-0.0.1/lordoftheringssdk/quote.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)       38 2023-04-11 20:10:09.893616 DannyBuffet-lotr-sdk-0.0.1/setup.cfg
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1151 2023-04-11 20:09:26.000000 DannyBuffet-lotr-sdk-0.0.1/setup.py
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 20:10:09.893022 DannyBuffet-lotr-sdk-0.0.1/tests/
--rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-10 17:46:44.000000 DannyBuffet-lotr-sdk-0.0.1/tests/__init__.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)      969 2023-04-11 14:32:05.000000 DannyBuffet-lotr-sdk-0.0.1/tests/test.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 20:30:43.833341 DannyBuffet-lotr-sdk-0.0.2/
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 20:30:43.830087 DannyBuffet-lotr-sdk-0.0.2/DannyBuffet_lotr_sdk.egg-info/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     3089 2023-04-11 20:30:43.000000 DannyBuffet-lotr-sdk-0.0.2/DannyBuffet_lotr_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      424 2023-04-11 20:30:43.000000 DannyBuffet-lotr-sdk-0.0.2/DannyBuffet_lotr_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        1 2023-04-11 20:30:43.000000 DannyBuffet-lotr-sdk-0.0.2/DannyBuffet_lotr_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        9 2023-04-11 20:30:43.000000 DannyBuffet-lotr-sdk-0.0.2/DannyBuffet_lotr_sdk.egg-info/requires.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       24 2023-04-11 20:30:43.000000 DannyBuffet-lotr-sdk-0.0.2/DannyBuffet_lotr_sdk.egg-info/top_level.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1071 2023-04-10 19:42:02.000000 DannyBuffet-lotr-sdk-0.0.2/LICENSE.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     3089 2023-04-11 20:30:43.832592 DannyBuffet-lotr-sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     2195 2023-04-11 20:27:09.000000 DannyBuffet-lotr-sdk-0.0.2/README.md
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 20:30:43.831454 DannyBuffet-lotr-sdk-0.0.2/lordoftheringssdk/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-10 17:32:46.000000 DannyBuffet-lotr-sdk-0.0.2/lordoftheringssdk/__init__.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1922 2023-04-11 20:29:38.000000 DannyBuffet-lotr-sdk-0.0.2/lordoftheringssdk/api_methods.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       72 2023-04-08 19:37:27.000000 DannyBuffet-lotr-sdk-0.0.2/lordoftheringssdk/conf.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1344 2023-04-10 18:31:09.000000 DannyBuffet-lotr-sdk-0.0.2/lordoftheringssdk/movie.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      910 2023-04-11 14:23:38.000000 DannyBuffet-lotr-sdk-0.0.2/lordoftheringssdk/quote.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       38 2023-04-11 20:30:43.833397 DannyBuffet-lotr-sdk-0.0.2/setup.cfg
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1151 2023-04-11 20:29:55.000000 DannyBuffet-lotr-sdk-0.0.2/setup.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 20:30:43.832148 DannyBuffet-lotr-sdk-0.0.2/tests/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-10 17:46:44.000000 DannyBuffet-lotr-sdk-0.0.2/tests/__init__.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      969 2023-04-11 14:32:05.000000 DannyBuffet-lotr-sdk-0.0.2/tests/test.py
```

### Comparing `DannyBuffet-lotr-sdk-0.0.1/DannyBuffet_lotr_sdk.egg-info/PKG-INFO` & `DannyBuffet-lotr-sdk-0.0.2/DannyBuffet_lotr_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DannyBuffet-lotr-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for interacting with the Lord of the Rings API
 Home-page: https://github.com/DannyBuffet/Lord-sdk
 Author: Daniel Reliford
 Author-email: dreliford@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,15 @@
 The Lord of the Rings SDK is a Python package that provides easy access to the Lord of the Rings API. It includes modules for interacting with the movies, and quotes from the Lord of the Rings movies.
 
 ## Installation
 
 To get started, you'll need to install the DR_lotr_sdk package.
 
 ```bash
-pip install DR_lotr_sdk
+pip install DannyBuffet-lotr-sdk
 ```
 
 This will install all the necessary dependencies.
 
 
 
 ## Importing the SDK
```

### Comparing `DannyBuffet-lotr-sdk-0.0.1/LICENSE.txt` & `DannyBuffet-lotr-sdk-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DannyBuffet-lotr-sdk-0.0.1/PKG-INFO` & `DannyBuffet-lotr-sdk-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DannyBuffet-lotr-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for interacting with the Lord of the Rings API
 Home-page: https://github.com/DannyBuffet/Lord-sdk
 Author: Daniel Reliford
 Author-email: dreliford@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,15 @@
 The Lord of the Rings SDK is a Python package that provides easy access to the Lord of the Rings API. It includes modules for interacting with the movies, and quotes from the Lord of the Rings movies.
 
 ## Installation
 
 To get started, you'll need to install the DR_lotr_sdk package.
 
 ```bash
-pip install DR_lotr_sdk
+pip install DannyBuffet-lotr-sdk
 ```
 
 This will install all the necessary dependencies.
 
 
 
 ## Importing the SDK
```

### Comparing `DannyBuffet-lotr-sdk-0.0.1/README.md` & `DannyBuffet-lotr-sdk-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 The Lord of the Rings SDK is a Python package that provides easy access to the Lord of the Rings API. It includes modules for interacting with the movies, and quotes from the Lord of the Rings movies.
 
 ## Installation
 
 To get started, you'll need to install the DR_lotr_sdk package.
 
 ```bash
-pip install DR_lotr_sdk
+pip install DannyBuffet-lotr-sdk
 ```
 
 This will install all the necessary dependencies.
 
 
 
 ## Importing the SDK
```

### Comparing `DannyBuffet-lotr-sdk-0.0.1/lordoftheringssdk/api_methods.py` & `DannyBuffet-lotr-sdk-0.0.2/lordoftheringssdk/api_methods.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 import requests
+from urllib3.util.retry import Retry
+from requests.adapters import HTTPAdapter
 from lordoftheringssdk.conf import BASE_URL, API_KEY
 
-# Create a session and add authorization header
+# Create session and add authorization header
 session = requests.Session()
 session.headers.update({"Accept": "application/json", "Authorization": f"Bearer {API_KEY}"})
-    
+
+# Create Retry object with desired settings
+retries = Retry(
+    total=5,  
+    backoff_factor=0.1, 
+    status_forcelist=[500, 501, 502, 504],  
+)
+
+# Mount Retry to the session for all requests
+session.mount("http://", HTTPAdapter(max_retries=retries))
+session.mount("https://", HTTPAdapter(max_retries=retries))
+
+
 class ApiMethods:
     """Class containing methods for making API calls"""
 
     def __repr__(self):
         return f"<{self.__class__.__name__}: {self.name}>"
 
     @property
```

### Comparing `DannyBuffet-lotr-sdk-0.0.1/lordoftheringssdk/movie.py` & `DannyBuffet-lotr-sdk-0.0.2/lordoftheringssdk/movie.py`

 * *Files identical despite different names*

### Comparing `DannyBuffet-lotr-sdk-0.0.1/lordoftheringssdk/quote.py` & `DannyBuffet-lotr-sdk-0.0.2/lordoftheringssdk/quote.py`

 * *Files identical despite different names*

### Comparing `DannyBuffet-lotr-sdk-0.0.1/setup.py` & `DannyBuffet-lotr-sdk-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='DannyBuffet-lotr-sdk',
-    version='0.0.1',
+    version='0.0.2',
     description='SDK for interacting with the Lord of the Rings API',
     author='Daniel Reliford',
     author_email='dreliford@gmail.com',
     url='https://github.com/DannyBuffet/Lord-sdk',
     packages=setuptools.find_packages(),
     install_requires=['requests'],
     classifiers=[
```

### Comparing `DannyBuffet-lotr-sdk-0.0.1/tests/test.py` & `DannyBuffet-lotr-sdk-0.0.2/tests/test.py`

 * *Files identical despite different names*

