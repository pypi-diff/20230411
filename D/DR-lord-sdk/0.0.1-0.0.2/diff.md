# Comparing `tmp/DR-lord-sdk-0.0.1.tar.gz` & `tmp/DR-lord-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DR-lord-sdk-0.0.1.tar", last modified: Tue Apr 11 15:55:01 2023, max compression
+gzip compressed data, was "DR-lord-sdk-0.0.2.tar", last modified: Tue Apr 11 16:13:06 2023, max compression
```

## Comparing `DR-lord-sdk-0.0.1.tar` & `DR-lord-sdk-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 15:55:01.452072 DR-lord-sdk-0.0.1/
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 15:55:01.449647 DR-lord-sdk-0.0.1/DR_lord_sdk.egg-info/
--rw-r--r--   0 dannyreliford   (501) staff       (20)     3568 2023-04-11 15:55:01.000000 DR-lord-sdk-0.0.1/DR_lord_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dannyreliford   (501) staff       (20)      379 2023-04-11 15:55:01.000000 DR-lord-sdk-0.0.1/DR_lord_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)        1 2023-04-11 15:55:01.000000 DR-lord-sdk-0.0.1/DR_lord_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)        9 2023-04-11 15:55:01.000000 DR-lord-sdk-0.0.1/DR_lord_sdk.egg-info/requires.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)       24 2023-04-11 15:55:01.000000 DR-lord-sdk-0.0.1/DR_lord_sdk.egg-info/top_level.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1071 2023-04-10 19:42:02.000000 DR-lord-sdk-0.0.1/LICENSE.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)     3568 2023-04-11 15:55:01.451908 DR-lord-sdk-0.0.1/PKG-INFO
--rw-r--r--   0 dannyreliford   (501) staff       (20)     2682 2023-04-11 13:45:15.000000 DR-lord-sdk-0.0.1/README.md
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 15:55:01.451036 DR-lord-sdk-0.0.1/lordoftheringssdk/
--rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-10 17:32:46.000000 DR-lord-sdk-0.0.1/lordoftheringssdk/__init__.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1421 2023-04-11 14:26:34.000000 DR-lord-sdk-0.0.1/lordoftheringssdk/api_methods.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)       72 2023-04-08 19:37:27.000000 DR-lord-sdk-0.0.1/lordoftheringssdk/conf.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1344 2023-04-10 18:31:09.000000 DR-lord-sdk-0.0.1/lordoftheringssdk/movie.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)      910 2023-04-11 14:23:38.000000 DR-lord-sdk-0.0.1/lordoftheringssdk/quote.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)       38 2023-04-11 15:55:01.452114 DR-lord-sdk-0.0.1/setup.cfg
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1142 2023-04-11 15:54:40.000000 DR-lord-sdk-0.0.1/setup.py
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 15:55:01.451488 DR-lord-sdk-0.0.1/tests/
--rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-10 17:46:44.000000 DR-lord-sdk-0.0.1/tests/__init__.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)      969 2023-04-11 14:32:05.000000 DR-lord-sdk-0.0.1/tests/test.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 16:13:06.935105 DR-lord-sdk-0.0.2/
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 16:13:06.932736 DR-lord-sdk-0.0.2/DR_lord_sdk.egg-info/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     3650 2023-04-11 16:13:06.000000 DR-lord-sdk-0.0.2/DR_lord_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      379 2023-04-11 16:13:06.000000 DR-lord-sdk-0.0.2/DR_lord_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        1 2023-04-11 16:13:06.000000 DR-lord-sdk-0.0.2/DR_lord_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        9 2023-04-11 16:13:06.000000 DR-lord-sdk-0.0.2/DR_lord_sdk.egg-info/requires.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       24 2023-04-11 16:13:06.000000 DR-lord-sdk-0.0.2/DR_lord_sdk.egg-info/top_level.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1071 2023-04-10 19:42:02.000000 DR-lord-sdk-0.0.2/LICENSE.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     3650 2023-04-11 16:13:06.934953 DR-lord-sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     2764 2023-04-11 16:12:12.000000 DR-lord-sdk-0.0.2/README.md
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 16:13:06.934059 DR-lord-sdk-0.0.2/lordoftheringssdk/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-10 17:32:46.000000 DR-lord-sdk-0.0.2/lordoftheringssdk/__init__.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1421 2023-04-11 14:26:34.000000 DR-lord-sdk-0.0.2/lordoftheringssdk/api_methods.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       72 2023-04-08 19:37:27.000000 DR-lord-sdk-0.0.2/lordoftheringssdk/conf.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1344 2023-04-10 18:31:09.000000 DR-lord-sdk-0.0.2/lordoftheringssdk/movie.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      910 2023-04-11 14:23:38.000000 DR-lord-sdk-0.0.2/lordoftheringssdk/quote.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       38 2023-04-11 16:13:06.935150 DR-lord-sdk-0.0.2/setup.cfg
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1142 2023-04-11 16:12:24.000000 DR-lord-sdk-0.0.2/setup.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 16:13:06.934541 DR-lord-sdk-0.0.2/tests/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-10 17:46:44.000000 DR-lord-sdk-0.0.2/tests/__init__.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      969 2023-04-11 14:32:05.000000 DR-lord-sdk-0.0.2/tests/test.py
```

### Comparing `DR-lord-sdk-0.0.1/DR_lord_sdk.egg-info/PKG-INFO` & `DR-lord-sdk-0.0.2/DR_lord_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DR-lord-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for interacting with the Lord of the Rings API
 Home-page: https://github.com/DannyBuffet/Lord-sdk
 Author: Daniel Reliford
 Author-email: dreliford@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -47,27 +47,29 @@
 
 
 ## Importing the SDK
 
 You can import the Lord of the Rings SDK in your Python script using the following import statement:
 
 ```python
-from lordoftheringssdk import Movie, Quote
+from lordoftheringssdk.movie import Movie
+from lordoftheringssdk.quote import Quote
 ```
 
 This will allow you to use the Movie, and Quote classes from the SDK in your code.
 
 
 
 ## Usage
 
 Here are some basic examples of how to use the Lord of the Rings SDK:
 
 ```python
-from lordoftheringssdk import Movie, Quote
+from lordoftheringssdk.movie import Movie
+from lordoftheringssdk.quote import Quote
 
 # Get all the movies
 movies = Movie.get()
 print(movies[1])
 print()
 
 # Get a specific quote
```

### Comparing `DR-lord-sdk-0.0.1/LICENSE.txt` & `DR-lord-sdk-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DR-lord-sdk-0.0.1/PKG-INFO` & `DR-lord-sdk-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DR-lord-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for interacting with the Lord of the Rings API
 Home-page: https://github.com/DannyBuffet/Lord-sdk
 Author: Daniel Reliford
 Author-email: dreliford@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -47,27 +47,29 @@
 
 
 ## Importing the SDK
 
 You can import the Lord of the Rings SDK in your Python script using the following import statement:
 
 ```python
-from lordoftheringssdk import Movie, Quote
+from lordoftheringssdk.movie import Movie
+from lordoftheringssdk.quote import Quote
 ```
 
 This will allow you to use the Movie, and Quote classes from the SDK in your code.
 
 
 
 ## Usage
 
 Here are some basic examples of how to use the Lord of the Rings SDK:
 
 ```python
-from lordoftheringssdk import Movie, Quote
+from lordoftheringssdk.movie import Movie
+from lordoftheringssdk.quote import Quote
 
 # Get all the movies
 movies = Movie.get()
 print(movies[1])
 print()
 
 # Get a specific quote
```

### Comparing `DR-lord-sdk-0.0.1/README.md` & `DR-lord-sdk-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,27 +25,29 @@
 
 
 ## Importing the SDK
 
 You can import the Lord of the Rings SDK in your Python script using the following import statement:
 
 ```python
-from lordoftheringssdk import Movie, Quote
+from lordoftheringssdk.movie import Movie
+from lordoftheringssdk.quote import Quote
 ```
 
 This will allow you to use the Movie, and Quote classes from the SDK in your code.
 
 
 
 ## Usage
 
 Here are some basic examples of how to use the Lord of the Rings SDK:
 
 ```python
-from lordoftheringssdk import Movie, Quote
+from lordoftheringssdk.movie import Movie
+from lordoftheringssdk.quote import Quote
 
 # Get all the movies
 movies = Movie.get()
 print(movies[1])
 print()
 
 # Get a specific quote
```

### Comparing `DR-lord-sdk-0.0.1/lordoftheringssdk/api_methods.py` & `DR-lord-sdk-0.0.2/lordoftheringssdk/api_methods.py`

 * *Files identical despite different names*

### Comparing `DR-lord-sdk-0.0.1/lordoftheringssdk/movie.py` & `DR-lord-sdk-0.0.2/lordoftheringssdk/movie.py`

 * *Files identical despite different names*

### Comparing `DR-lord-sdk-0.0.1/lordoftheringssdk/quote.py` & `DR-lord-sdk-0.0.2/lordoftheringssdk/quote.py`

 * *Files identical despite different names*

### Comparing `DR-lord-sdk-0.0.1/setup.py` & `DR-lord-sdk-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='DR-lord-sdk',
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

### Comparing `DR-lord-sdk-0.0.1/tests/test.py` & `DR-lord-sdk-0.0.2/tests/test.py`

 * *Files identical despite different names*

