# Comparing `tmp/kaiterra-async-client-1.0.0.tar.gz` & `tmp/kaiterra-async-client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaiterra-async-client-1.0.0.tar", last modified: Thu Jul  7 21:52:57 2022, max compression
+gzip compressed data, was "kaiterra-async-client-1.0.1.tar", last modified: Tue Apr 11 17:29:35 2023, max compression
```

## Comparing `kaiterra-async-client-1.0.0.tar` & `kaiterra-async-client-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2022-07-07 21:52:57.919760 kaiterra-async-client-1.0.0/
--rw-r--r--   0 michal    (1000) michal    (1000)     1065 2022-07-07 20:59:04.000000 kaiterra-async-client-1.0.0/LICENSE
--rw-r--r--   0 michal    (1000) michal    (1000)       73 2022-07-07 20:59:04.000000 kaiterra-async-client-1.0.0/MANIFEST.in
--rw-r--r--   0 michal    (1000) michal    (1000)      517 2022-07-07 20:59:04.000000 kaiterra-async-client-1.0.0/Makefile
--rw-r--r--   0 michal    (1000) michal    (1000)     1801 2022-07-07 21:52:57.919760 kaiterra-async-client-1.0.0/PKG-INFO
--rw-r--r--   0 michal    (1000) michal    (1000)     1151 2022-07-07 20:59:04.000000 kaiterra-async-client-1.0.0/README.rst
-drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2022-07-07 21:52:57.919760 kaiterra-async-client-1.0.0/kaiterra_async_client/
--rw-r--r--   0 michal    (1000) michal    (1000)      183 2022-07-07 20:59:04.000000 kaiterra-async-client-1.0.0/kaiterra_async_client/__init__.py
--rw-r--r--   0 michal    (1000) michal    (1000)     8086 2022-07-07 21:19:41.000000 kaiterra-async-client-1.0.0/kaiterra_async_client/client.py
--rw-r--r--   0 michal    (1000) michal    (1000)      492 2022-07-07 20:59:04.000000 kaiterra-async-client-1.0.0/kaiterra_async_client/dateutil.py
-drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2022-07-07 21:52:57.919760 kaiterra-async-client-1.0.0/kaiterra_async_client.egg-info/
--rw-r--r--   0 michal    (1000) michal    (1000)     1801 2022-07-07 21:52:57.000000 kaiterra-async-client-1.0.0/kaiterra_async_client.egg-info/PKG-INFO
--rw-r--r--   0 michal    (1000) michal    (1000)      372 2022-07-07 21:52:57.000000 kaiterra-async-client-1.0.0/kaiterra_async_client.egg-info/SOURCES.txt
--rw-r--r--   0 michal    (1000) michal    (1000)        1 2022-07-07 21:52:57.000000 kaiterra-async-client-1.0.0/kaiterra_async_client.egg-info/dependency_links.txt
--rw-r--r--   0 michal    (1000) michal    (1000)       15 2022-07-07 21:52:57.000000 kaiterra-async-client-1.0.0/kaiterra_async_client.egg-info/requires.txt
--rw-r--r--   0 michal    (1000) michal    (1000)       22 2022-07-07 21:52:57.000000 kaiterra-async-client-1.0.0/kaiterra_async_client.egg-info/top_level.txt
--rw-r--r--   0 michal    (1000) michal    (1000)       38 2022-07-07 21:52:57.919760 kaiterra-async-client-1.0.0/setup.cfg
--rw-r--r--   0 michal    (1000) michal    (1000)     1118 2022-07-07 21:52:51.000000 kaiterra-async-client-1.0.0/setup.py
+drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2023-04-11 17:29:35.663001 kaiterra-async-client-1.0.1/
+-rw-r--r--   0 michal    (1000) michal    (1000)     1065 2022-07-07 20:59:04.000000 kaiterra-async-client-1.0.1/LICENSE
+-rw-r--r--   0 michal    (1000) michal    (1000)       73 2022-07-07 20:59:04.000000 kaiterra-async-client-1.0.1/MANIFEST.in
+-rw-r--r--   0 michal    (1000) michal    (1000)      517 2022-07-07 20:59:04.000000 kaiterra-async-client-1.0.1/Makefile
+-rw-r--r--   0 michal    (1000) michal    (1000)     1803 2023-04-11 17:29:35.663001 kaiterra-async-client-1.0.1/PKG-INFO
+-rw-r--r--   0 michal    (1000) michal    (1000)     1153 2023-04-11 16:33:21.000000 kaiterra-async-client-1.0.1/README.rst
+drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2023-04-11 17:29:35.663001 kaiterra-async-client-1.0.1/kaiterra_async_client/
+-rw-r--r--   0 michal    (1000) michal    (1000)      183 2022-07-07 20:59:04.000000 kaiterra-async-client-1.0.1/kaiterra_async_client/__init__.py
+-rw-r--r--   0 michal    (1000) michal    (1000)     8088 2023-04-11 16:34:31.000000 kaiterra-async-client-1.0.1/kaiterra_async_client/client.py
+-rw-r--r--   0 michal    (1000) michal    (1000)      484 2023-04-11 16:18:08.000000 kaiterra-async-client-1.0.1/kaiterra_async_client/dateutil.py
+drwxr-xr-x   0 michal    (1000) michal    (1000)        0 2023-04-11 17:29:35.663001 kaiterra-async-client-1.0.1/kaiterra_async_client.egg-info/
+-rw-r--r--   0 michal    (1000) michal    (1000)     1803 2023-04-11 17:29:35.000000 kaiterra-async-client-1.0.1/kaiterra_async_client.egg-info/PKG-INFO
+-rw-r--r--   0 michal    (1000) michal    (1000)      372 2023-04-11 17:29:35.000000 kaiterra-async-client-1.0.1/kaiterra_async_client.egg-info/SOURCES.txt
+-rw-r--r--   0 michal    (1000) michal    (1000)        1 2023-04-11 17:29:35.000000 kaiterra-async-client-1.0.1/kaiterra_async_client.egg-info/dependency_links.txt
+-rw-r--r--   0 michal    (1000) michal    (1000)       15 2023-04-11 17:29:35.000000 kaiterra-async-client-1.0.1/kaiterra_async_client.egg-info/requires.txt
+-rw-r--r--   0 michal    (1000) michal    (1000)       22 2023-04-11 17:29:35.000000 kaiterra-async-client-1.0.1/kaiterra_async_client.egg-info/top_level.txt
+-rw-r--r--   0 michal    (1000) michal    (1000)       38 2023-04-11 17:29:35.663001 kaiterra-async-client-1.0.1/setup.cfg
+-rw-r--r--   0 michal    (1000) michal    (1000)     1118 2023-04-11 17:04:37.000000 kaiterra-async-client-1.0.1/setup.py
```

### Comparing `kaiterra-async-client-1.0.0/LICENSE` & `kaiterra-async-client-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kaiterra-async-client-1.0.0/Makefile` & `kaiterra-async-client-1.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `kaiterra-async-client-1.0.0/PKG-INFO` & `kaiterra-async-client-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiterra-async-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: Kaiterra API Async Client
 Home-page: https://github.com/Michsior14/python-kaiterra-async-client
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,17 +14,17 @@
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 python-kaiterra-async-client
 ============================
 
-Python 3 client for retrieving readings from your Laser Egg or Sensedge using the `Kaiterra REST API <https://www.kaiterra.com/dev>`__.
+Python 3 client for retrieving readings from your Laser Egg or Sensedge using the `Kaiterra REST API <https://dashboard.kaiterra.com>`__.
 
-To use it, you'll first need to create an account at the `Kaiterra Dashboard <https://dashboard.kaiterra.cn/>`__, then create an API key under Settings -> Profile -> Developer.
+To use it, you'll first need to create an account at the `Kaiterra Dashboard <https://dashboard.kaiterra.com>`__, then create an API key under Settings -> Profile -> Developer.
 
 
 Getting Started
 -------------------
 
 Install the library using pip:
```

### Comparing `kaiterra-async-client-1.0.0/README.rst` & `kaiterra-async-client-1.0.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 python-kaiterra-async-client
 ============================
 
-Python 3 client for retrieving readings from your Laser Egg or Sensedge using the `Kaiterra REST API <https://www.kaiterra.com/dev>`__.
+Python 3 client for retrieving readings from your Laser Egg or Sensedge using the `Kaiterra REST API <https://dashboard.kaiterra.com>`__.
 
-To use it, you'll first need to create an account at the `Kaiterra Dashboard <https://dashboard.kaiterra.cn/>`__, then create an API key under Settings -> Profile -> Developer.
+To use it, you'll first need to create an account at the `Kaiterra Dashboard <https://dashboard.kaiterra.com>`__, then create an API key under Settings -> Profile -> Developer.
 
 
 Getting Started
 -------------------
 
 Install the library using pip:
```

### Comparing `kaiterra-async-client-1.0.0/kaiterra_async_client/client.py` & `kaiterra-async-client-1.0.1/kaiterra_async_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,29 +52,29 @@
 class KaiterraAPIClient(object):
     """
     KaiterraAPIClient connects to the Kaiterra API over HTTP.
 
     :param base_url: URL under which the API can be found.  The default value is sufficient
     for most cases.
     :param api_key: Secret key, obtained from the Kaiterra dashboard at
-    https://dashboard.kaiterra.cn, that uniquely identifies the client making the request.
+    https://dashboard.kaiterra.com, that uniquely identifies the client making the request.
     :param hmac_secret: Secret key that can be used to authorize requests without
     transmitting the key over the wire.  (Note: most clients don't use this)
     :param aqi_standard: Indicates that air quality index (AQI) should be calculated
     for reported polluants where applicable, according to the standard set by the
     US EPA, Chinese MEP, or other given governing body.  The index returned is the Kaiterra
     Overall Index described at https://support.kaiterra.com/hc/en-us/articles/360016529993-What-is-the-Overall-Index-
     :param preferred_units: List of Units preferred by the client.  For instance,
     passing [Units.DegreesFahrenheit] will cause all temperature quantities to be reported
     in degrees Fahrenheit instead of the default, which is degrees Celsius.
     """
 
     def __init__(self,
                  session,
-                 base_url='https://api.kaiterra.cn',
+                 base_url='https://api.kaiterra.com',
                  api_key=None,
                  hmac_secret=None,
                  aqi_standard=None,
                  preferred_units=None
                  ):
         """Constructs a new KaiterraAPIClient object."""
         self._base_url = base_url.rstrip('/')
```

### Comparing `kaiterra-async-client-1.0.0/kaiterra_async_client.egg-info/PKG-INFO` & `kaiterra-async-client-1.0.1/kaiterra_async_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiterra-async-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: Kaiterra API Async Client
 Home-page: https://github.com/Michsior14/python-kaiterra-async-client
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,17 +14,17 @@
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 python-kaiterra-async-client
 ============================
 
-Python 3 client for retrieving readings from your Laser Egg or Sensedge using the `Kaiterra REST API <https://www.kaiterra.com/dev>`__.
+Python 3 client for retrieving readings from your Laser Egg or Sensedge using the `Kaiterra REST API <https://dashboard.kaiterra.com>`__.
 
-To use it, you'll first need to create an account at the `Kaiterra Dashboard <https://dashboard.kaiterra.cn/>`__, then create an API key under Settings -> Profile -> Developer.
+To use it, you'll first need to create an account at the `Kaiterra Dashboard <https://dashboard.kaiterra.com>`__, then create an API key under Settings -> Profile -> Developer.
 
 
 Getting Started
 -------------------
 
 Install the library using pip:
```

### Comparing `kaiterra-async-client-1.0.0/setup.py` & `kaiterra-async-client-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open('README.rst', 'r') as f:
     readme = f.read()
 
 
 setuptools.setup(
     name='kaiterra-async-client',
-    version='1.0.0',
+    version='1.0.1',
     description="Kaiterra API Async Client",
     long_description=readme,
     long_description_content_type="text/x-rst",
     url='https://github.com/Michsior14/python-kaiterra-async-client',
     license='MIT License',
     packages=setuptools.find_packages(exclude=['*.tests', '*.tests.*']),
     test_suite='kaiterra_async_client.tests',
```

