# Comparing `tmp/commugen_api-0.5.tar.gz` & `tmp/commugen_api-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commugen_api-0.5.tar", last modified: Mon Dec 12 15:26:31 2022, max compression
+gzip compressed data, was "commugen_api-0.6.tar", last modified: Tue Apr 11 08:45:10 2023, max compression
```

## Comparing `commugen_api-0.5.tar` & `commugen_api-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-12-12 15:26:31.757301 commugen_api-0.5/
--rw-rw-rw-   0        0        0      516 2022-12-12 15:26:31.756309 commugen_api-0.5/PKG-INFO
--rw-rw-rw-   0        0        0      191 2022-10-18 06:07:28.000000 commugen_api-0.5/README.md
-drwxrwxrwx   0        0        0        0 2022-12-12 15:26:31.728516 commugen_api-0.5/commugen_api/
--rw-rw-rw-   0        0        0       39 2022-10-11 09:14:21.000000 commugen_api-0.5/commugen_api/__init__.py
--rw-rw-rw-   0        0        0     7928 2022-12-12 15:20:13.000000 commugen_api-0.5/commugen_api/commugen_api.py
--rw-rw-rw-   0        0        0     7522 2022-10-27 12:56:36.000000 commugen_api-0.5/commugen_api/response_objects.py
-drwxrwxrwx   0        0        0        0 2022-12-12 15:26:31.755305 commugen_api-0.5/commugen_api.egg-info/
--rw-rw-rw-   0        0        0      516 2022-12-12 15:26:31.000000 commugen_api-0.5/commugen_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2022-12-12 15:26:31.000000 commugen_api-0.5/commugen_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-12 15:26:31.000000 commugen_api-0.5/commugen_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2022-12-12 15:26:31.000000 commugen_api-0.5/commugen_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-12-12 15:26:31.000000 commugen_api-0.5/commugen_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-12 15:26:31.757301 commugen_api-0.5/setup.cfg
--rw-rw-rw-   0        0        0      843 2022-12-12 15:23:14.000000 commugen_api-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:45:10.353068 commugen_api-0.6/
+-rw-rw-rw-   0        0        0      516 2023-04-11 08:45:10.353068 commugen_api-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2022-10-18 06:07:28.000000 commugen_api-0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 08:45:10.325873 commugen_api-0.6/commugen_api/
+-rw-rw-rw-   0        0        0       39 2022-10-11 09:14:21.000000 commugen_api-0.6/commugen_api/__init__.py
+-rw-rw-rw-   0        0        0     8728 2023-04-11 08:43:06.000000 commugen_api-0.6/commugen_api/commugen_api.py
+-rw-rw-rw-   0        0        0     7522 2022-10-27 12:56:36.000000 commugen_api-0.6/commugen_api/response_objects.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:45:10.351423 commugen_api-0.6/commugen_api.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-04-11 08:45:10.000000 commugen_api-0.6/commugen_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-11 08:45:10.000000 commugen_api-0.6/commugen_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 08:45:10.000000 commugen_api-0.6/commugen_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 08:45:10.000000 commugen_api-0.6/commugen_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 08:45:10.000000 commugen_api-0.6/commugen_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 08:45:10.353068 commugen_api-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      893 2023-04-11 08:43:06.000000 commugen_api-0.6/setup.py
```

### Comparing `commugen_api-0.5/PKG-INFO` & `commugen_api-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commugen_api
-Version: 0.5
+Version: 0.6
 Summary: Python wrapper for commugen api
 Home-page: https://bitbucket.org/kobi_commugen/commugen_api/
 Author: kobi kolodner
 Author-email: kobi@commugen.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
```

### Comparing `commugen_api-0.5/commugen_api/commugen_api.py` & `commugen_api-0.6/commugen_api/commugen_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import base64
+import json
 
 import requests
 from curlify import to_curl
+from keyring import get_password, set_password
+from stdiomask import getpass
 
 from commugen_api.response_objects import CommugenModel, CommugenDomains, CommugenTables, CommugenSingleRecord, \
     CommugenOptions
 
 MAX_COUNT = 100
 
 
@@ -42,14 +45,33 @@
         """
         self.prefix = f'https://{host}:{port}/v0'
         self.headers = self._authentication_header(user, password)
         self._session = requests.api
         self.verify = kwargs.pop('verify', True)
         self.verbose = kwargs.pop('verbose', False)
 
+    @classmethod
+    def init_from_json_file(cls, path='params.json'):
+        with open(path, encoding='utf-8') as f:
+            params = json.load(f)
+        password = get_password(service_name=params['host'], username=params['user'])
+        if password and 'password' not in params.keys():
+            params['password'] = password
+        return cls(**params)
+
+    @classmethod
+    def store_password(cls, path='params.json'):
+        with open(path, encoding='utf-8') as f:
+            params = json.load(f)
+        password = getpass(prompt=f'Enter password for {params["user"]}:')
+        set_password(service_name=params['host'], username=params['user'], password=password)
+
+
+
+
     def _authentication_header(self, user, password):
         """
         :param str user:
         :param str password:
         :return dict: authentication header
         """
```

### Comparing `commugen_api-0.5/commugen_api/response_objects.py` & `commugen_api-0.6/commugen_api/response_objects.py`

 * *Files identical despite different names*

### Comparing `commugen_api-0.5/commugen_api.egg-info/PKG-INFO` & `commugen_api-0.6/commugen_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commugen-api
-Version: 0.5
+Version: 0.6
 Summary: Python wrapper for commugen api
 Home-page: https://bitbucket.org/kobi_commugen/commugen_api/
 Author: kobi kolodner
 Author-email: kobi@commugen.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
```

### Comparing `commugen_api-0.5/setup.py` & `commugen_api-0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 from setuptools import setup
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 setup(name='commugen_api',
-      version='0.5',
+      version='0.6',
       description='Python wrapper for commugen api',
       url='https://bitbucket.org/kobi_commugen/commugen_api/',
       author='kobi kolodner',
       author_email='kobi@commugen.com',
       license='MIT',
       packages=['commugen_api'],
       install_requires=[
             'requests',
             'tablib',
-            'curlify'
+            'curlify',
+            'keyring',
+            'stdiomask'
       ],
       classifiers=[
             'Development Status :: 2 - Pre-Alpha'
       ],
       long_description=long_description,  # Optional
       long_description_content_type="text/markdown",  # Optional (see note above)
```

