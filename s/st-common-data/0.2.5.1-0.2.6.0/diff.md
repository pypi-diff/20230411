# Comparing `tmp/st_common_data-0.2.5.1.tar.gz` & `tmp/st_common_data-0.2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_common_data-0.2.5.1.tar", last modified: Fri Mar 31 16:34:15 2023, max compression
+gzip compressed data, was "st_common_data-0.2.6.0.tar", last modified: Tue Apr 11 10:32:17 2023, max compression
```

## Comparing `st_common_data-0.2.5.1.tar` & `st_common_data-0.2.6.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-03-31 16:34:15.942618 st_common_data-0.2.5.1/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1073 2022-04-19 17:26:26.000000 st_common_data-0.2.5.1/LICENCE
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-03-31 16:34:15.942618 st_common_data-0.2.5.1/PKG-INFO
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      703 2022-12-07 11:03:09.000000 st_common_data-0.2.5.1/README.md
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      103 2022-04-19 17:26:26.000000 st_common_data-0.2.5.1/pyproject.toml
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      669 2023-03-31 16:34:15.942618 st_common_data-0.2.5.1/setup.cfg
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-03-31 16:34:15.938618 st_common_data-0.2.5.1/st_common_data/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      143 2023-03-31 16:34:06.000000 st_common_data-0.2.5.1/st_common_data/__init__.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-03-31 16:34:15.938618 st_common_data-0.2.5.1/st_common_data/auth/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      350 2023-03-28 10:57:12.000000 st_common_data-0.2.5.1/st_common_data/auth/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      118 2022-12-07 11:03:09.000000 st_common_data-0.2.5.1/st_common_data/auth/apps.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     8494 2023-03-28 10:57:12.000000 st_common_data-0.2.5.1/st_common_data/auth/django_auth.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     8962 2023-03-31 16:29:28.000000 st_common_data-0.2.5.1/st_common_data/auth/fastapi_auth.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      386 2022-08-23 10:22:22.000000 st_common_data-0.2.5.1/st_common_data/auth/serializers.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      278 2022-08-23 10:22:22.000000 st_common_data-0.2.5.1/st_common_data/auth/urls.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     3266 2023-01-31 09:47:17.000000 st_common_data-0.2.5.1/st_common_data/auth/views.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    30488 2023-02-16 13:38:13.000000 st_common_data-0.2.5.1/st_common_data/datum.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     5940 2023-01-05 08:33:40.000000 st_common_data-0.2.5.1/st_common_data/nyse_holidays.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      398 2022-08-23 10:22:22.000000 st_common_data-0.2.5.1/st_common_data/pagination.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-03-31 16:34:15.938618 st_common_data-0.2.5.1/st_common_data/trading_accounts/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.5.1/st_common_data/trading_accounts/__init__.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-03-31 16:34:15.942618 st_common_data-0.2.5.1/st_common_data/trading_accounts/migrations/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4299 2022-08-23 10:22:22.000000 st_common_data-0.2.5.1/st_common_data/trading_accounts/migrations/0001_initial.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      652 2023-02-24 09:24:45.000000 st_common_data-0.2.5.1/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      456 2023-03-22 00:17:46.000000 st_common_data-0.2.5.1/st_common_data/trading_accounts/migrations/0003_tradingaccount_personal_status.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.5.1/st_common_data/trading_accounts/migrations/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     2929 2023-03-22 00:17:46.000000 st_common_data-0.2.5.1/st_common_data/trading_accounts/models.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      214 2022-08-23 10:22:22.000000 st_common_data-0.2.5.1/st_common_data/trading_accounts/serializers.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      200 2022-08-23 10:22:22.000000 st_common_data-0.2.5.1/st_common_data/trading_accounts/urls.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4193 2022-12-07 11:03:09.000000 st_common_data-0.2.5.1/st_common_data/trading_accounts/views.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-03-31 16:34:15.942618 st_common_data-0.2.5.1/st_common_data/utils/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-07-21 20:22:31.000000 st_common_data-0.2.5.1/st_common_data/utils/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4305 2022-07-21 20:25:41.000000 st_common_data-0.2.5.1/st_common_data/utils/common.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-03-31 16:34:15.938618 st_common_data-0.2.5.1/st_common_data.egg-info/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-03-31 16:34:15.000000 st_common_data-0.2.5.1/st_common_data.egg-info/PKG-INFO
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1080 2023-03-31 16:34:15.000000 st_common_data-0.2.5.1/st_common_data.egg-info/SOURCES.txt
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        1 2023-03-31 16:34:15.000000 st_common_data-0.2.5.1/st_common_data.egg-info/dependency_links.txt
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)       15 2023-03-31 16:34:15.000000 st_common_data-0.2.5.1/st_common_data.egg-info/top_level.txt
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-11 10:32:17.649301 st_common_data-0.2.6.0/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1073 2022-04-19 17:26:26.000000 st_common_data-0.2.6.0/LICENCE
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-04-11 10:32:17.649301 st_common_data-0.2.6.0/PKG-INFO
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      703 2022-12-07 11:03:09.000000 st_common_data-0.2.6.0/README.md
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      103 2022-04-19 17:26:26.000000 st_common_data-0.2.6.0/pyproject.toml
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      669 2023-04-11 10:32:17.649301 st_common_data-0.2.6.0/setup.cfg
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-11 10:32:17.645300 st_common_data-0.2.6.0/st_common_data/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      143 2023-04-11 10:31:33.000000 st_common_data-0.2.6.0/st_common_data/__init__.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-11 10:32:17.649301 st_common_data-0.2.6.0/st_common_data/auth/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      443 2023-04-11 10:31:33.000000 st_common_data-0.2.6.0/st_common_data/auth/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      118 2022-12-07 11:03:09.000000 st_common_data-0.2.6.0/st_common_data/auth/apps.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     9562 2023-04-11 10:31:33.000000 st_common_data-0.2.6.0/st_common_data/auth/django_auth.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10010 2023-04-11 10:31:33.000000 st_common_data-0.2.6.0/st_common_data/auth/fastapi_auth.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      386 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/auth/serializers.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      278 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/auth/urls.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     3266 2023-01-31 09:47:17.000000 st_common_data-0.2.6.0/st_common_data/auth/views.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    30488 2023-02-16 13:38:13.000000 st_common_data-0.2.6.0/st_common_data/datum.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     5940 2023-01-05 08:33:40.000000 st_common_data-0.2.6.0/st_common_data/nyse_holidays.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      398 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/pagination.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-11 10:32:17.649301 st_common_data-0.2.6.0/st_common_data/trading_accounts/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/__init__.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-11 10:32:17.649301 st_common_data-0.2.6.0/st_common_data/trading_accounts/migrations/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4299 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/migrations/0001_initial.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      652 2023-02-24 09:24:45.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      456 2023-03-22 00:17:46.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/migrations/0003_tradingaccount_personal_status.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/migrations/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     2929 2023-03-22 00:17:46.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/models.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      214 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/serializers.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      200 2022-08-23 10:22:22.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/urls.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4193 2022-12-07 11:03:09.000000 st_common_data-0.2.6.0/st_common_data/trading_accounts/views.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-11 10:32:17.649301 st_common_data-0.2.6.0/st_common_data/utils/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-07-21 20:22:31.000000 st_common_data-0.2.6.0/st_common_data/utils/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4305 2022-07-21 20:25:41.000000 st_common_data-0.2.6.0/st_common_data/utils/common.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2023-04-11 10:32:17.645300 st_common_data-0.2.6.0/st_common_data.egg-info/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1279 2023-04-11 10:32:17.000000 st_common_data-0.2.6.0/st_common_data.egg-info/PKG-INFO
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1080 2023-04-11 10:32:17.000000 st_common_data-0.2.6.0/st_common_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        1 2023-04-11 10:32:17.000000 st_common_data-0.2.6.0/st_common_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)       15 2023-04-11 10:32:17.000000 st_common_data-0.2.6.0/st_common_data.egg-info/top_level.txt
```

### Comparing `st_common_data-0.2.5.1/LICENCE` & `st_common_data-0.2.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.5.1/PKG-INFO` & `st_common_data-0.2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st_common_data
-Version: 0.2.5.1
+Version: 0.2.6.0
 Summary: Data that is used in different ST projects
 Home-page: https://github.com/ivanovds/st_common_data
 Author: Daniil Ivanov
 Author-email: danil.98and@gmail.com
 Project-URL: Bug Tracker, https://github.com/ivanovds/st_common_data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `st_common_data-0.2.5.1/README.md` & `st_common_data-0.2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.5.1/setup.cfg` & `st_common_data-0.2.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.5.1/st_common_data/auth/django_auth.py` & `st_common_data-0.2.6.0/st_common_data/auth/django_auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import importlib
 import json
 import datetime
 import os
 import pickle
-from typing import Optional
+from typing import Optional, Union
 from urllib.request import urlopen
 
 import requests
 from django.contrib.auth import get_user_model
 from django.conf import settings
 from rest_framework import HTTP_HEADER_ENCODING, authentication
 from rest_framework.exceptions import AuthenticationFailed
 import jose.exceptions
 from jose import jwt
 
-from . import SingletonMeta, SERVICE_TOKEN_FILENAME
+from . import SingletonMeta, SERVICE_TOKEN_FILENAME, MANAGEMENT_TOKEN_FILENAME
 
 UserModel = get_user_model()
 
 
 class JWKS(metaclass=SingletonMeta):
     """
     Auth0 json web keys set for local token verification
@@ -185,14 +185,16 @@
             return None
 
 
 class ServiceAuth0Token(metaclass=SingletonMeta):
     """
     Auth0 token from service app for machine-to-machine communication (between services)
     """
+    TOKEN_FILENAME = SERVICE_TOKEN_FILENAME
+
     def __init__(self,
                  audience: str,
                  grant_type: str,
                  client_id: str,
                  client_secret: str,
                  services_token_url: str):
         self.audience = audience
@@ -209,15 +211,15 @@
             self._update_token()
         return self._token
 
     def _update_token(self):
         token_data = self._get_token()
         self._token = token_data['access_token']
         self.expire = datetime.datetime.now() + datetime.timedelta(seconds=token_data['expires_in'] - 10)
-        create_or_update_token_file(obj_to_set=self)
+        create_or_update_token_file(obj_to_set=self, token_filename=self.TOKEN_FILENAME)
 
     def _get_token(self, retry: int = 2):
         response = requests.post(
             url=self.token_url,
             data={
                 'audience': self.audience,
                 'grant_type': self.grant_type,
@@ -237,40 +239,58 @@
                 details = response.text
             raise Exception(f'Unable to get token, status code: {response.status_code}. Server returned: {details}')
 
     def __str__(self):
         return self.token
 
 
-def create_or_update_token_file(obj_to_set: ServiceAuth0Token = None) -> None:
+class ManagementAuth0Token(ServiceAuth0Token):
+    """
+    Auth0 token from management app for communication with auth0 API
+    """
+    TOKEN_FILENAME = MANAGEMENT_TOKEN_FILENAME
+
+
+def create_or_update_token_file(token_filename: str,
+                                obj_to_set: Union[ServiceAuth0Token, ManagementAuth0Token] = None) -> None:
     if obj_to_set is None:
-        obj_to_set = ServiceAuth0Token(
-            audience=settings.AUTH0_API_AUDIENCE,
-            grant_type='client_credentials',
-            client_id=settings.AUTH0_SERVICE_CLIENT_ID,
-            client_secret=settings.AUTH0_SERVICE_CLIENT_SECRET,
-            services_token_url=settings.AUTH0_SERVICE_TOKEN_URL)
+
+        if token_filename == SERVICE_TOKEN_FILENAME:
+            obj_to_set = ServiceAuth0Token(
+                audience=settings.AUTH0_API_AUDIENCE,
+                grant_type='client_credentials',
+                client_id=settings.AUTH0_SERVICE_CLIENT_ID,
+                client_secret=settings.AUTH0_SERVICE_CLIENT_SECRET,
+                services_token_url=settings.AUTH0_SERVICE_TOKEN_URL)
+        elif token_filename == MANAGEMENT_TOKEN_FILENAME:
+            obj_to_set = ManagementAuth0Token(
+                audience=f'https://{settings.AUTH0_DOMAIN}/api/v2/',
+                grant_type='client_credentials',
+                client_id=settings.AUTH0_MANAGEMENT_CLIENT_ID,
+                client_secret=settings.AUTH0_MANAGEMENT_CLIENT_SECRET,
+                services_token_url=settings.AUTH0_SERVICE_TOKEN_URL
+            )
 
     obj_to_set.token  # Important! In order to set token before saving into file
 
-    with open(SERVICE_TOKEN_FILENAME, 'wb') as wb_handle:
+    with open(token_filename, 'wb') as wb_handle:
         pickle.dump(obj_to_set, wb_handle, protocol=pickle.HIGHEST_PROTOCOL)
 
 
-def get_service_auth0_token(retry: int = 0) -> ServiceAuth0Token:
+def get_auth0_token(token_filename: str, retry: int = 0) -> Union[ServiceAuth0Token, ManagementAuth0Token]:
     if retry > 2:
         raise Exception('Failed to get_service_auth0_token after several retries')
 
-    if not os.path.exists(SERVICE_TOKEN_FILENAME):
-        create_or_update_token_file()
+    if not os.path.exists(token_filename):
+        create_or_update_token_file(token_filename=token_filename)
 
-    with open(SERVICE_TOKEN_FILENAME, 'rb') as rb_handle:
+    with open(token_filename, 'rb') as rb_handle:
         try:
             token = pickle.load(rb_handle)
         except:
-            os.remove(SERVICE_TOKEN_FILENAME)
-            token = get_service_auth0_token(retry=retry + 1)
+            os.remove(token_filename)
+            token = get_auth0_token(token_filename=token_filename, retry=retry + 1)
     return token
 
 
-service_auth0_token = get_service_auth0_token()
-
+service_auth0_token = get_auth0_token(token_filename=SERVICE_TOKEN_FILENAME)
+management_auth0_token = get_auth0_token(token_filename=MANAGEMENT_TOKEN_FILENAME)
```

### Comparing `st_common_data-0.2.5.1/st_common_data/auth/fastapi_auth.py` & `st_common_data-0.2.6.0/st_common_data/auth/fastapi_auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import importlib
 import json
 import os
 import pickle
 from dataclasses import dataclass
 import datetime
-from typing import Optional
+from typing import Optional, Union
 from urllib.request import urlopen
 
 import jose.exceptions
 import requests
 from fastapi import Request, Depends
 from jose import jwt
 from fastapi_exceptions.exceptions import AuthenticationFailed, PermissionDenied
@@ -17,15 +17,15 @@
 
 from app.dependencies import get_db
 from app.settings import config
 
 UserModel = getattr(
     importlib.import_module('app.models'), config.auth_user_model
 )  # in tier_system AUTH_USER_MODEL="UserDataModel"
-from . import SingletonMeta, SERVICE_TOKEN_FILENAME
+from . import SingletonMeta, SERVICE_TOKEN_FILENAME, MANAGEMENT_TOKEN_FILENAME
 
 
 class JWKS(metaclass=SingletonMeta):
     """
     Auth0 json web keys set for local token verification
     """
 
@@ -195,14 +195,16 @@
         claims=claims)
 
 
 class ServiceAuth0Token(metaclass=SingletonMeta):
     """
     Auth0 token from service app for machine-to-machine communication (between services)
     """
+    TOKEN_FILENAME = SERVICE_TOKEN_FILENAME
+
     def __init__(self,
                  audience: str,
                  grant_type: str,
                  client_id: str,
                  client_secret: str,
                  services_token_url: str):
         self.audience = audience
@@ -219,15 +221,15 @@
             self._update_token()
         return self._token
 
     def _update_token(self):
         token_data = self._get_token()
         self._token = token_data['access_token']
         self.expire = datetime.datetime.now() + datetime.timedelta(seconds=token_data['expires_in'] - 10)
-        create_or_update_token_file(obj_to_set=self)
+        create_or_update_token_file(obj_to_set=self, token_filename=self.TOKEN_FILENAME)
 
     def _get_token(self, retry: int = 2):
         response = requests.post(
             url=self.token_url,
             data={
                 'audience': self.audience,
                 'grant_type': self.grant_type,
@@ -247,39 +249,57 @@
                 details = response.text
             raise Exception(f'Unable to get token, status code: {response.status_code}. Server returned: {details}')
 
     def __str__(self):
         return self.token
 
 
-def create_or_update_token_file(obj_to_set: ServiceAuth0Token = None) -> None:
+class ManagementAuth0Token(ServiceAuth0Token):
+    """
+    Auth0 token from management app for communication with auth0 API
+    """
+    TOKEN_FILENAME = MANAGEMENT_TOKEN_FILENAME
+
+
+def create_or_update_token_file(token_filename: str,
+                                obj_to_set: Union[ServiceAuth0Token, ManagementAuth0Token] = None) -> None:
     if obj_to_set is None:
-        obj_to_set = ServiceAuth0Token(
-            audience=config.auth0_oa_api_audience,
-            grant_type='client_credentials',
-            client_id=config.auth0_service_client_id,
-            client_secret=config.auth0_service_client_secret,
-            services_token_url=config.auth0_service_token_url)
+
+        if token_filename == SERVICE_TOKEN_FILENAME:
+            obj_to_set = ServiceAuth0Token(
+                audience=config.auth0_oa_api_audience,
+                grant_type='client_credentials',
+                client_id=config.auth0_service_client_id,
+                client_secret=config.auth0_service_client_secret,
+                services_token_url=config.auth0_service_token_url)
+        elif token_filename == MANAGEMENT_TOKEN_FILENAME:
+            obj_to_set = ManagementAuth0Token(
+                audience=f'https://{config.auth0_domain}/api/v2/',
+                grant_type='client_credentials',
+                client_id=config.auth0_management_client_id,
+                client_secret=config.auth0_management_client_secret,
+                services_token_url=config.auth0_service_token_url)
 
     obj_to_set.token  # Important! In order to set token before saving into file
 
-    with open(SERVICE_TOKEN_FILENAME, 'wb') as wb_handle:
+    with open(token_filename, 'wb') as wb_handle:
         pickle.dump(obj_to_set, wb_handle, protocol=pickle.HIGHEST_PROTOCOL)
 
 
-def get_service_auth0_token(retry: int = 0) -> ServiceAuth0Token:
+def get_auth0_token(token_filename: str, retry: int = 0) -> Union[ServiceAuth0Token, ManagementAuth0Token]:
     if retry > 2:
         raise Exception('Failed to get_service_auth0_token after several retries')
 
-    if not os.path.exists(SERVICE_TOKEN_FILENAME):
-        create_or_update_token_file()
+    if not os.path.exists(token_filename):
+        create_or_update_token_file(token_filename=token_filename)
 
-    with open(SERVICE_TOKEN_FILENAME, 'rb') as rb_handle:
+    with open(token_filename, 'rb') as rb_handle:
         try:
             token = pickle.load(rb_handle)
         except:
-            os.remove(SERVICE_TOKEN_FILENAME)
-            token = get_service_auth0_token(retry=retry + 1)
+            os.remove(token_filename)
+            token = get_auth0_token(token_filename=token_filename, retry=retry + 1)
     return token
 
 
-service_auth0_token = get_service_auth0_token()
+service_auth0_token = get_auth0_token(token_filename=SERVICE_TOKEN_FILENAME)
+management_auth0_token = get_auth0_token(token_filename=MANAGEMENT_TOKEN_FILENAME)
```

### Comparing `st_common_data-0.2.5.1/st_common_data/auth/views.py` & `st_common_data-0.2.6.0/st_common_data/auth/views.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.5.1/st_common_data/datum.py` & `st_common_data-0.2.6.0/st_common_data/datum.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.5.1/st_common_data/nyse_holidays.py` & `st_common_data-0.2.6.0/st_common_data/nyse_holidays.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.5.1/st_common_data/trading_accounts/migrations/0001_initial.py` & `st_common_data-0.2.6.0/st_common_data/trading_accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.5.1/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py` & `st_common_data-0.2.6.0/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.5.1/st_common_data/trading_accounts/models.py` & `st_common_data-0.2.6.0/st_common_data/trading_accounts/models.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.5.1/st_common_data/trading_accounts/views.py` & `st_common_data-0.2.6.0/st_common_data/trading_accounts/views.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.5.1/st_common_data/utils/common.py` & `st_common_data-0.2.6.0/st_common_data/utils/common.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.5.1/st_common_data.egg-info/PKG-INFO` & `st_common_data-0.2.6.0/st_common_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-common-data
-Version: 0.2.5.1
+Version: 0.2.6.0
 Summary: Data that is used in different ST projects
 Home-page: https://github.com/ivanovds/st_common_data
 Author: Daniil Ivanov
 Author-email: danil.98and@gmail.com
 Project-URL: Bug Tracker, https://github.com/ivanovds/st_common_data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `st_common_data-0.2.5.1/st_common_data.egg-info/SOURCES.txt` & `st_common_data-0.2.6.0/st_common_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

