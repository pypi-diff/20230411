# Comparing `tmp/tfa-python-sdk-1.6.0.tar.gz` & `tmp/tfa-python-sdk-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfa-python-sdk-1.6.0.tar", last modified: Mon Aug  8 15:45:40 2022, max compression
+gzip compressed data, was "tfa-python-sdk-2.6.0.tar", last modified: Tue Apr 11 21:57:04 2023, max compression
```

## Comparing `tfa-python-sdk-1.6.0.tar` & `tfa-python-sdk-2.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 amir      (1000) amir      (1000)        0 2022-08-08 15:45:40.296956 tfa-python-sdk-1.6.0/
--rw-r--r--   0 amir      (1000) amir      (1000)     1111 2022-07-22 15:54:29.000000 tfa-python-sdk-1.6.0/LICENSE
--rw-r--r--   0 amir      (1000) amir      (1000)     2862 2022-08-08 15:45:40.296956 tfa-python-sdk-1.6.0/PKG-INFO
--rw-r--r--   0 amir      (1000) amir      (1000)     2525 2022-08-08 15:44:42.000000 tfa-python-sdk-1.6.0/README.md
--rw-r--r--   0 amir      (1000) amir      (1000)       79 2022-08-08 15:45:40.296956 tfa-python-sdk-1.6.0/setup.cfg
--rw-r--r--   0 amir      (1000) amir      (1000)      567 2022-08-08 15:44:44.000000 tfa-python-sdk-1.6.0/setup.py
-drwxr-xr-x   0 amir      (1000) amir      (1000)        0 2022-08-08 15:45:40.296956 tfa-python-sdk-1.6.0/tfa_python_sdk/
--rw-r--r--   0 amir      (1000) amir      (1000)       31 2022-06-23 22:04:24.000000 tfa-python-sdk-1.6.0/tfa_python_sdk/__init__.py
--rw-r--r--   0 amir      (1000) amir      (1000)      602 2022-08-08 15:44:45.000000 tfa-python-sdk-1.6.0/tfa_python_sdk/tfa_python_sdk.py
-drwxr-xr-x   0 amir      (1000) amir      (1000)        0 2022-08-08 15:45:40.296956 tfa-python-sdk-1.6.0/tfa_python_sdk.egg-info/
--rw-r--r--   0 amir      (1000) amir      (1000)     2862 2022-08-08 15:45:39.000000 tfa-python-sdk-1.6.0/tfa_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 amir      (1000) amir      (1000)      285 2022-08-08 15:45:40.000000 tfa-python-sdk-1.6.0/tfa_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 amir      (1000) amir      (1000)        1 2022-08-08 15:45:39.000000 tfa-python-sdk-1.6.0/tfa_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 amir      (1000) amir      (1000)       15 2022-08-08 15:45:40.000000 tfa-python-sdk-1.6.0/tfa_python_sdk.egg-info/requires.txt
--rw-r--r--   0 amir      (1000) amir      (1000)       15 2022-08-08 15:45:40.000000 tfa-python-sdk-1.6.0/tfa_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 amirhosseinmohammadi   (501) staff       (20)        0 2023-04-11 21:57:04.233758 tfa-python-sdk-2.6.0/
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)     1111 2023-04-11 20:08:32.000000 tfa-python-sdk-2.6.0/LICENSE
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)     2843 2023-04-11 21:57:04.233869 tfa-python-sdk-2.6.0/PKG-INFO
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)     2525 2023-04-11 20:08:32.000000 tfa-python-sdk-2.6.0/README.md
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)       79 2023-04-11 21:57:04.234123 tfa-python-sdk-2.6.0/setup.cfg
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)      568 2023-04-11 21:54:32.000000 tfa-python-sdk-2.6.0/setup.py
+drwxr-xr-x   0 amirhosseinmohammadi   (501) staff       (20)        0 2023-04-11 21:57:04.232539 tfa-python-sdk-2.6.0/tfa_python_sdk/
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)       31 2023-04-11 20:08:32.000000 tfa-python-sdk-2.6.0/tfa_python_sdk/__init__.py
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)      563 2023-04-11 21:50:36.000000 tfa-python-sdk-2.6.0/tfa_python_sdk/tfa_python_sdk.py
+drwxr-xr-x   0 amirhosseinmohammadi   (501) staff       (20)        0 2023-04-11 21:57:04.233622 tfa-python-sdk-2.6.0/tfa_python_sdk.egg-info/
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)     2843 2023-04-11 21:57:04.000000 tfa-python-sdk-2.6.0/tfa_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)      285 2023-04-11 21:57:04.000000 tfa-python-sdk-2.6.0/tfa_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)        1 2023-04-11 21:57:04.000000 tfa-python-sdk-2.6.0/tfa_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)       15 2023-04-11 21:57:04.000000 tfa-python-sdk-2.6.0/tfa_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 amirhosseinmohammadi   (501) staff       (20)       15 2023-04-11 21:57:04.000000 tfa-python-sdk-2.6.0/tfa_python_sdk.egg-info/top_level.txt
```

### Comparing `tfa-python-sdk-1.6.0/LICENSE` & `tfa-python-sdk-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tfa-python-sdk-1.6.0/PKG-INFO` & `tfa-python-sdk-2.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tfa-python-sdk
-Version: 1.6.0
+Version: 2.6.0
 Summary: Telegram Factor Authentication python library
 Home-page: https://github.com/tfasoft/sdk-python
 Author: Amirhossein Mohammadi
 Author-email: amirhosseinmohammadi1380@yahoo.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Telegram Factor Authentication - Python SDK
 
 [Python SDK document is in docs.tfasoft.com](https://docs.amirhossein.info/sdks/python)
 
@@ -115,8 +114,7 @@
 If you want to develop the library, it is so simple. Edit library codes and run `test.py` like this:
 
 ```shell
 $ python3 test.py
 ```
 
 > Before you start: **Remember the base or codes are stored in `tfa_python_sdk/tfa_python_sdk.py`. You need to edit there.
-
```

### Comparing `tfa-python-sdk-1.6.0/README.md` & `tfa-python-sdk-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `tfa-python-sdk-1.6.0/setup.py` & `tfa-python-sdk-2.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='tfa-python-sdk',
-    version='1.6.0',
+    version='2.6.0',
     author='Amirhossein Mohammadi',
     license='MIT',
     author_email="amirhosseinmohammadi1380@yahoo.com",
     description="Telegram Factor Authentication python library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tfasoft/sdk-python",
     packages=find_packages(),
     install_requires=find_packages()
-)
+)
```

### Comparing `tfa-python-sdk-1.6.0/tfa_python_sdk/tfa_python_sdk.py` & `tfa-python-sdk-2.6.0/tfa_python_sdk/tfa_python_sdk.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import requests as req
 
+session = req.Session()
+session.trust_env = False
+
+baseUrl = "http://localhost:25000/api"
+
+
 class TFA:
     def __init__(self, access_token) -> None:
         self.access_token = access_token
-        self.testUrl = "http://localhost:9000/api/auth"
-        self.baseUrl = "https://tfasoft-api.herokuapp.com/api/auth"
 
     def authUser(self, user_token):
         urlData = {
             "access_token": self.access_token,
             "user_token": user_token,
         }
 
-        response = req.post(f'{self.baseUrl}/auth/access', json = urlData)
+        response = session.post(f'{baseUrl}/access', json=urlData)
 
         data = {
             "status": response.status_code,
             "data": response.json()
         }
 
-        return data
+        return data
```

### Comparing `tfa-python-sdk-1.6.0/tfa_python_sdk.egg-info/PKG-INFO` & `tfa-python-sdk-2.6.0/tfa_python_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tfa-python-sdk
-Version: 1.6.0
+Version: 2.6.0
 Summary: Telegram Factor Authentication python library
 Home-page: https://github.com/tfasoft/sdk-python
 Author: Amirhossein Mohammadi
 Author-email: amirhosseinmohammadi1380@yahoo.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Telegram Factor Authentication - Python SDK
 
 [Python SDK document is in docs.tfasoft.com](https://docs.amirhossein.info/sdks/python)
 
@@ -115,8 +114,7 @@
 If you want to develop the library, it is so simple. Edit library codes and run `test.py` like this:
 
 ```shell
 $ python3 test.py
 ```
 
 > Before you start: **Remember the base or codes are stored in `tfa_python_sdk/tfa_python_sdk.py`. You need to edit there.
-
```

