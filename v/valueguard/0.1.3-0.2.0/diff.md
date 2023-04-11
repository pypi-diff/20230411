# Comparing `tmp/valueguard-0.1.3.tar.gz` & `tmp/valueguard-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/valueguard-0.1.3.tar", last modified: Thu May 13 07:01:08 2021, max compression
+gzip compressed data, was "valueguard-0.2.0.tar", last modified: Tue Apr 11 08:55:48 2023, max compression
```

## Comparing `valueguard-0.1.3.tar` & `valueguard-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2021-05-13 07:01:08.693469 valueguard-0.1.3/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     4156 2021-05-13 07:01:08.689469 valueguard-0.1.3/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     3064 2021-01-21 08:39:58.000000 valueguard-0.1.3/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2021-05-13 07:01:08.693469 valueguard-0.1.3/setup.cfg
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      649 2021-05-13 06:59:54.000000 valueguard-0.1.3/setup.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2021-05-13 07:01:08.689469 valueguard-0.1.3/valueguard/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       26 2020-06-12 08:33:15.000000 valueguard-0.1.3/valueguard/__init__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)    12799 2021-05-13 06:58:32.000000 valueguard-0.1.3/valueguard/valueguard.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2021-05-13 07:01:08.689469 valueguard-0.1.3/valueguard.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     4156 2021-05-13 07:01:08.000000 valueguard-0.1.3/valueguard.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      235 2021-05-13 07:01:08.000000 valueguard-0.1.3/valueguard.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2021-05-13 07:01:08.000000 valueguard-0.1.3/valueguard.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       12 2021-05-13 07:01:08.000000 valueguard-0.1.3/valueguard.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       11 2021-05-13 07:01:08.000000 valueguard-0.1.3/valueguard.egg-info/top_level.txt
+drwxrwxr-x   0 valueguard  (1000) valueguard  (1000)        0 2023-04-11 08:55:48.046731 valueguard-0.2.0/
+-rw-rw-r--   0 valueguard  (1000) valueguard  (1000)     4299 2023-04-11 08:55:48.046731 valueguard-0.2.0/PKG-INFO
+-rw-rw-r--   0 valueguard  (1000) valueguard  (1000)     3958 2023-04-11 08:09:05.000000 valueguard-0.2.0/README.md
+-rw-rw-r--   0 valueguard  (1000) valueguard  (1000)       38 2023-04-11 08:55:48.046731 valueguard-0.2.0/setup.cfg
+-rw-rw-r--   0 valueguard  (1000) valueguard  (1000)      649 2023-04-11 08:16:11.000000 valueguard-0.2.0/setup.py
+drwxrwxr-x   0 valueguard  (1000) valueguard  (1000)        0 2023-04-11 08:55:48.042731 valueguard-0.2.0/valueguard/
+-rw-rw-r--   0 valueguard  (1000) valueguard  (1000)       26 2023-04-11 08:09:05.000000 valueguard-0.2.0/valueguard/__init__.py
+-rw-rw-r--   0 valueguard  (1000) valueguard  (1000)    28575 2023-04-11 08:09:05.000000 valueguard-0.2.0/valueguard/valueguard.py
+drwxrwxr-x   0 valueguard  (1000) valueguard  (1000)        0 2023-04-11 08:55:48.042731 valueguard-0.2.0/valueguard.egg-info/
+-rw-rw-r--   0 valueguard  (1000) valueguard  (1000)     4299 2023-04-11 08:55:47.000000 valueguard-0.2.0/valueguard.egg-info/PKG-INFO
+-rw-rw-r--   0 valueguard  (1000) valueguard  (1000)      235 2023-04-11 08:55:48.000000 valueguard-0.2.0/valueguard.egg-info/SOURCES.txt
+-rw-rw-r--   0 valueguard  (1000) valueguard  (1000)        1 2023-04-11 08:55:47.000000 valueguard-0.2.0/valueguard.egg-info/dependency_links.txt
+-rw-rw-r--   0 valueguard  (1000) valueguard  (1000)       12 2023-04-11 08:55:48.000000 valueguard-0.2.0/valueguard.egg-info/requires.txt
+-rw-rw-r--   0 valueguard  (1000) valueguard  (1000)       11 2023-04-11 08:55:48.000000 valueguard-0.2.0/valueguard.egg-info/top_level.txt
```

### Comparing `valueguard-0.1.3/README.md` & `valueguard-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,23 @@
+Metadata-Version: 2.1
+Name: valueguard
+Version: 0.2.0
+Summary: The official client for the Valueguard API
+Home-page: https://github.com/Valueguard-Index-Sweden/valueguard-python-client
+Author: Valueguard
+Author-email: info@valueguard.se
+License: MIT
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+
  <img src="https://valueguard.se/static/media/valueguardlogo_black.f3a4c174.png" width="200">
- 
+
 # Valueguard Python Client
 
+
 ## Index
 
 - [Introduction](#introduction)
   - [Description](#description)
   - [Installing](#installing)
 - [Usage](#usage)
 - [Community](#community)
@@ -16,16 +28,18 @@
 
 # Introduction
 
 ## Description
 
 **Valueguard Python Client** is the official client used to interact with the new **Valueguards API**
 
-- For **python client** documentation see [usage](#usage) and [wiki-page](https://github.com/Valueguard-Index-Sweden/valueguard-python-client/wiki)
-- For the **core Valueguard API** documentation, see the [api documentation](https://api.valueguard.se/swagger-ui.html).
+Valueguard is a Swedish company that provides real estate valuation and analysis services for the housing market. The company was founded in 2007. Our primary service is to provide independent home valuations and analyses to banks, brokers and other companies that need reliable and accurate property information. Our services are based on various data sources, including historical transaction data, information about the property's location and condition, and other market data.
+
+In addition to price statistics and valuations, Valueguard provides various other services, such as a complete registry of all homes in Sweden, called the Residential Registry. We have a team of experienced analysts who work to provide high-quality services to our clients.
+We are proud to have a strong reputation in the Swedish real estate industry and are considered one of the country's leading providers of housing statistics.
 
 ## Installing
 
 Install by pip
 
 ```
 pip3 install git+https://github.com/Valueguard-Index-Sweden/valueguard-python-client#egg=valueguard
@@ -36,24 +50,27 @@
 ```
 pip3 install valueguard
 ```
 
 
 # Usage
 
+- For **python client** documentation see [wiki-page](https://github.com/Valueguard-Index-Sweden/valueguard-python-client/wiki)
+- For the **core Valueguard API** documentation, see the [api documentation](https://api.valueguard.se/swagger-ui.html).
+
 ```python
 import valueguard
 
 # Create object
 vgClient = valueguard.Client()
 
 # Generate a access token
 vgClient.authenticate(<username>,<password>)
 
-# Use wished function 
+# Use wished function
 print(vgClient.residential_registry(offset=0, limit=800, search_criteria={
                                                             "construction_year_min": 2018,
                                                             "construction_year_max": 2019
                                                             }))
 ```
 
 # Community
```

### Comparing `valueguard-0.1.3/setup.py` & `valueguard-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["requests>=2"]
 
 setup(
     name="valueguard",
-    version="0.1.3",
+    version="0.2.0",
     author="Valueguard",
     author_email="info@valueguard.se",
     description="The official client for the Valueguard API",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/Valueguard-Index-Sweden/valueguard-python-client",
```

