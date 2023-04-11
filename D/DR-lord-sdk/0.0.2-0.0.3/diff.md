# Comparing `tmp/DR-lord-sdk-0.0.2.tar.gz` & `tmp/DR-lord-sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DR-lord-sdk-0.0.2.tar", last modified: Tue Apr 11 16:13:06 2023, max compression
+gzip compressed data, was "DR-lord-sdk-0.0.3.tar", last modified: Tue Apr 11 20:06:12 2023, max compression
```

## Comparing `DR-lord-sdk-0.0.2.tar` & `DR-lord-sdk-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 16:13:06.935105 DR-lord-sdk-0.0.2/
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 16:13:06.932736 DR-lord-sdk-0.0.2/DR_lord_sdk.egg-info/
--rw-r--r--   0 dannyreliford   (501) staff       (20)     3650 2023-04-11 16:13:06.000000 DR-lord-sdk-0.0.2/DR_lord_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dannyreliford   (501) staff       (20)      379 2023-04-11 16:13:06.000000 DR-lord-sdk-0.0.2/DR_lord_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)        1 2023-04-11 16:13:06.000000 DR-lord-sdk-0.0.2/DR_lord_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)        9 2023-04-11 16:13:06.000000 DR-lord-sdk-0.0.2/DR_lord_sdk.egg-info/requires.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)       24 2023-04-11 16:13:06.000000 DR-lord-sdk-0.0.2/DR_lord_sdk.egg-info/top_level.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1071 2023-04-10 19:42:02.000000 DR-lord-sdk-0.0.2/LICENSE.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)     3650 2023-04-11 16:13:06.934953 DR-lord-sdk-0.0.2/PKG-INFO
--rw-r--r--   0 dannyreliford   (501) staff       (20)     2764 2023-04-11 16:12:12.000000 DR-lord-sdk-0.0.2/README.md
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 16:13:06.934059 DR-lord-sdk-0.0.2/lordoftheringssdk/
--rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-10 17:32:46.000000 DR-lord-sdk-0.0.2/lordoftheringssdk/__init__.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1421 2023-04-11 14:26:34.000000 DR-lord-sdk-0.0.2/lordoftheringssdk/api_methods.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)       72 2023-04-08 19:37:27.000000 DR-lord-sdk-0.0.2/lordoftheringssdk/conf.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1344 2023-04-10 18:31:09.000000 DR-lord-sdk-0.0.2/lordoftheringssdk/movie.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)      910 2023-04-11 14:23:38.000000 DR-lord-sdk-0.0.2/lordoftheringssdk/quote.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)       38 2023-04-11 16:13:06.935150 DR-lord-sdk-0.0.2/setup.cfg
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1142 2023-04-11 16:12:24.000000 DR-lord-sdk-0.0.2/setup.py
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 16:13:06.934541 DR-lord-sdk-0.0.2/tests/
--rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-10 17:46:44.000000 DR-lord-sdk-0.0.2/tests/__init__.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)      969 2023-04-11 14:32:05.000000 DR-lord-sdk-0.0.2/tests/test.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 20:06:12.099365 DR-lord-sdk-0.0.3/
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 20:06:12.096982 DR-lord-sdk-0.0.3/DR_lord_sdk.egg-info/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     3071 2023-04-11 20:06:12.000000 DR-lord-sdk-0.0.3/DR_lord_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      379 2023-04-11 20:06:12.000000 DR-lord-sdk-0.0.3/DR_lord_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        1 2023-04-11 20:06:12.000000 DR-lord-sdk-0.0.3/DR_lord_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        9 2023-04-11 20:06:12.000000 DR-lord-sdk-0.0.3/DR_lord_sdk.egg-info/requires.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       24 2023-04-11 20:06:12.000000 DR-lord-sdk-0.0.3/DR_lord_sdk.egg-info/top_level.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1071 2023-04-10 19:42:02.000000 DR-lord-sdk-0.0.3/LICENSE.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     3071 2023-04-11 20:06:12.099177 DR-lord-sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     2186 2023-04-11 20:04:05.000000 DR-lord-sdk-0.0.3/README.md
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 20:06:12.098433 DR-lord-sdk-0.0.3/lordoftheringssdk/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-10 17:32:46.000000 DR-lord-sdk-0.0.3/lordoftheringssdk/__init__.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1533 2023-04-11 17:17:00.000000 DR-lord-sdk-0.0.3/lordoftheringssdk/api_methods.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       72 2023-04-08 19:37:27.000000 DR-lord-sdk-0.0.3/lordoftheringssdk/conf.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1344 2023-04-10 18:31:09.000000 DR-lord-sdk-0.0.3/lordoftheringssdk/movie.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      910 2023-04-11 14:23:38.000000 DR-lord-sdk-0.0.3/lordoftheringssdk/quote.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       38 2023-04-11 20:06:12.099415 DR-lord-sdk-0.0.3/setup.cfg
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1142 2023-04-11 20:05:20.000000 DR-lord-sdk-0.0.3/setup.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-11 20:06:12.098816 DR-lord-sdk-0.0.3/tests/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-10 17:46:44.000000 DR-lord-sdk-0.0.3/tests/__init__.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      969 2023-04-11 14:32:05.000000 DR-lord-sdk-0.0.3/tests/test.py
```

### Comparing `DR-lord-sdk-0.0.2/DR_lord_sdk.egg-info/PKG-INFO` & `DR-lord-sdk-0.0.3/DR_lord_sdk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DR-lord-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: SDK for interacting with the Lord of the Rings API
 Home-page: https://github.com/DannyBuffet/Lord-sdk
 Author: Daniel Reliford
 Author-email: dreliford@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -31,24 +31,14 @@
 ```bash
 pip install DR_lotr_sdk
 ```
 
 This will install all the necessary dependencies.
 
 
-## Configuration
-
-1. Go to the website [https://the-one-api.dev/](https://the-one-api.dev/) and sign up to obtain an API key.
-2. Open a configuration file (e.g., `conf.py`).
-3. Update the configuration file with your API key.
-
-```python
-  API_KEY: "YOUR_API_KEY"
-```
-
 
 ## Importing the SDK
 
 You can import the Lord of the Rings SDK in your Python script using the following import statement:
 
 ```python
 from lordoftheringssdk.movie import Movie
@@ -81,15 +71,15 @@
 for movie in movies:
     print(movie.name)
 print()
 
 # Get all the quotes
 quotes = Quote.get()
 for quote in quotes:
-    print(quotes)
+    print(quote)
 print()
 
 # Get a specific quote
 print(quotes[3])
 print()
 
 # Get information about a specific movie
@@ -113,18 +103,7 @@
 - `/movie/<id>/quotes`: This endpoint returns a list of all the quotes from a specific movie, identified by the id parameter.
 
 - `/movie/<id>/quotes/<id>`: This endpoint returns a specific quote from a specific movie, identified by the id parameter.
 
 - `/quotes`: This endpoint returns a list of all the quotes from the Lord of the Rings movies.
 
 - `/quotes/<id>`: This endpoint returns information about a specific quote, identified by the id parameter.
-
-
-
-## Running Tests
-
-The tests directory in the package contains a test.py file that you can use to run tests for the SDK. To run the tests, navigate to the root directory of the package and run the following command:
-
-```bash
-python tests/test.py
-```
-This will execute the tests and provide the test results.
```

### Comparing `DR-lord-sdk-0.0.2/LICENSE.txt` & `DR-lord-sdk-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DR-lord-sdk-0.0.2/PKG-INFO` & `DR-lord-sdk-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DR-lord-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: SDK for interacting with the Lord of the Rings API
 Home-page: https://github.com/DannyBuffet/Lord-sdk
 Author: Daniel Reliford
 Author-email: dreliford@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -31,24 +31,14 @@
 ```bash
 pip install DR_lotr_sdk
 ```
 
 This will install all the necessary dependencies.
 
 
-## Configuration
-
-1. Go to the website [https://the-one-api.dev/](https://the-one-api.dev/) and sign up to obtain an API key.
-2. Open a configuration file (e.g., `conf.py`).
-3. Update the configuration file with your API key.
-
-```python
-  API_KEY: "YOUR_API_KEY"
-```
-
 
 ## Importing the SDK
 
 You can import the Lord of the Rings SDK in your Python script using the following import statement:
 
 ```python
 from lordoftheringssdk.movie import Movie
@@ -81,15 +71,15 @@
 for movie in movies:
     print(movie.name)
 print()
 
 # Get all the quotes
 quotes = Quote.get()
 for quote in quotes:
-    print(quotes)
+    print(quote)
 print()
 
 # Get a specific quote
 print(quotes[3])
 print()
 
 # Get information about a specific movie
@@ -113,18 +103,7 @@
 - `/movie/<id>/quotes`: This endpoint returns a list of all the quotes from a specific movie, identified by the id parameter.
 
 - `/movie/<id>/quotes/<id>`: This endpoint returns a specific quote from a specific movie, identified by the id parameter.
 
 - `/quotes`: This endpoint returns a list of all the quotes from the Lord of the Rings movies.
 
 - `/quotes/<id>`: This endpoint returns information about a specific quote, identified by the id parameter.
-
-
-
-## Running Tests
-
-The tests directory in the package contains a test.py file that you can use to run tests for the SDK. To run the tests, navigate to the root directory of the package and run the following command:
-
-```bash
-python tests/test.py
-```
-This will execute the tests and provide the test results.
```

### Comparing `DR-lord-sdk-0.0.2/README.md` & `DR-lord-sdk-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,24 +9,14 @@
 ```bash
 pip install DR_lotr_sdk
 ```
 
 This will install all the necessary dependencies.
 
 
-## Configuration
-
-1. Go to the website [https://the-one-api.dev/](https://the-one-api.dev/) and sign up to obtain an API key.
-2. Open a configuration file (e.g., `conf.py`).
-3. Update the configuration file with your API key.
-
-```python
-  API_KEY: "YOUR_API_KEY"
-```
-
 
 ## Importing the SDK
 
 You can import the Lord of the Rings SDK in your Python script using the following import statement:
 
 ```python
 from lordoftheringssdk.movie import Movie
@@ -59,15 +49,15 @@
 for movie in movies:
     print(movie.name)
 print()
 
 # Get all the quotes
 quotes = Quote.get()
 for quote in quotes:
-    print(quotes)
+    print(quote)
 print()
 
 # Get a specific quote
 print(quotes[3])
 print()
 
 # Get information about a specific movie
@@ -91,18 +81,7 @@
 - `/movie/<id>/quotes`: This endpoint returns a list of all the quotes from a specific movie, identified by the id parameter.
 
 - `/movie/<id>/quotes/<id>`: This endpoint returns a specific quote from a specific movie, identified by the id parameter.
 
 - `/quotes`: This endpoint returns a list of all the quotes from the Lord of the Rings movies.
 
 - `/quotes/<id>`: This endpoint returns information about a specific quote, identified by the id parameter.
-
-
-
-## Running Tests
-
-The tests directory in the package contains a test.py file that you can use to run tests for the SDK. To run the tests, navigate to the root directory of the package and run the following command:
-
-```bash
-python tests/test.py
-```
-This will execute the tests and provide the test results.
```

### Comparing `DR-lord-sdk-0.0.2/lordoftheringssdk/api_methods.py` & `DR-lord-sdk-0.0.3/lordoftheringssdk/api_methods.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,17 +17,21 @@
 
     @classmethod
     def serialize(cls, json):
         """
         Serializes a response into an object and returns a list of objects if multiple objects are present in the response
         """
         results = []
-        for item in json:            
-            item = cls(*item.values())
+        for item in json:
+            try:             
+                item = cls(*item.values())
+            except Exception:
+                item = cls(*item.values(), "")
             results.append(item)
+            
         return results[0] if len(results) == 1 else results
 
     @classmethod
     def get(cls, id=None):
         """
         Retrieves data from the API and returns the result of the query
         :param id (str): the unique identifier to query
```

### Comparing `DR-lord-sdk-0.0.2/lordoftheringssdk/movie.py` & `DR-lord-sdk-0.0.3/lordoftheringssdk/movie.py`

 * *Files identical despite different names*

### Comparing `DR-lord-sdk-0.0.2/lordoftheringssdk/quote.py` & `DR-lord-sdk-0.0.3/lordoftheringssdk/quote.py`

 * *Files identical despite different names*

### Comparing `DR-lord-sdk-0.0.2/setup.py` & `DR-lord-sdk-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='DR-lord-sdk',
-    version='0.0.2',
+    version='0.0.3',
     description='SDK for interacting with the Lord of the Rings API',
     author='Daniel Reliford',
     author_email='dreliford@gmail.com',
     url='https://github.com/DannyBuffet/Lord-sdk',
     packages=setuptools.find_packages(),
     install_requires=['requests'],
     classifiers=[
```

### Comparing `DR-lord-sdk-0.0.2/tests/test.py` & `DR-lord-sdk-0.0.3/tests/test.py`

 * *Files identical despite different names*

