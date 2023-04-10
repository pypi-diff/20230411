# Comparing `tmp/pyhOn-0.6.3.tar.gz` & `tmp/pyhOn-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.6.3.tar", last modified: Mon Apr 10 18:35:11 2023, max compression
+gzip compressed data, was "pyhOn-0.6.4.tar", last modified: Mon Apr 10 23:02:44 2023, max compression
```

## Comparing `pyhOn-0.6.3.tar` & `pyhOn-0.6.4.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:11.378888 pyhOn-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 18:35:01.000000 pyhOn-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 18:35:11.378888 pyhOn-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-10 18:35:01.000000 pyhOn-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:11.374888 pyhOn-0.6.3/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 18:35:11.000000 pyhOn-0.6.3/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-10 18:35:11.000000 pyhOn-0.6.3/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:35:11.000000 pyhOn-0.6.3/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 18:35:11.000000 pyhOn-0.6.3/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 18:35:11.000000 pyhOn-0.6.3/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 18:35:11.000000 pyhOn-0.6.3/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:11.378888 pyhOn-0.6.3/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4839 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:11.378888 pyhOn-0.6.3/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:11.378888 pyhOn-0.6.3/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/connection/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/connection/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-10 18:35:01.000000 pyhOn-0.6.3/pyhon/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:35:11.378888 pyhOn-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-10 18:35:01.000000 pyhOn-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:02:44.945554 pyhOn-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 23:02:32.000000 pyhOn-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 23:02:44.945554 pyhOn-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-10 23:02:32.000000 pyhOn-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:02:44.941554 pyhOn-0.6.4/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 23:02:44.000000 pyhOn-0.6.4/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-10 23:02:44.000000 pyhOn-0.6.4/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 23:02:44.000000 pyhOn-0.6.4/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 23:02:44.000000 pyhOn-0.6.4/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 23:02:44.000000 pyhOn-0.6.4/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 23:02:44.000000 pyhOn-0.6.4/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:02:44.941554 pyhOn-0.6.4/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4839 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:02:44.941554 pyhOn-0.6.4/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:02:44.945554 pyhOn-0.6.4/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/connection/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/connection/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 23:02:44.945554 pyhOn-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-10 23:02:32.000000 pyhOn-0.6.4/setup.py
```

### Comparing `pyhOn-0.6.3/LICENSE` & `pyhOn-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.3/PKG-INFO` & `pyhOn-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.6.3
+Version: 0.6.4
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.6.3/README.md` & `pyhOn-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.3/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.6.4/pyhOn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.6.3
+Version: 0.6.4
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.6.3/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.6.4/pyhOn.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 pyhOn.egg-info/requires.txt
 pyhOn.egg-info/top_level.txt
 pyhon/__init__.py
 pyhon/__main__.py
 pyhon/appliance.py
 pyhon/commands.py
 pyhon/const.py
+pyhon/exceptions.py
 pyhon/hon.py
 pyhon/parameter.py
 pyhon/appliances/__init__.py
 pyhon/appliances/ov.py
 pyhon/appliances/td.py
 pyhon/appliances/wd.py
 pyhon/appliances/wm.py
```

### Comparing `pyhOn-0.6.3/pyhon/__main__.py` & `pyhOn-0.6.4/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.3/pyhon/appliance.py` & `pyhOn-0.6.4/pyhon/appliance.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.3/pyhon/appliances/ov.py` & `pyhOn-0.6.4/pyhon/appliances/ov.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.3/pyhon/commands.py` & `pyhOn-0.6.4/pyhon/commands.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.3/pyhon/connection/api.py` & `pyhOn-0.6.4/pyhon/connection/api.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.3/pyhon/connection/auth.py` & `pyhOn-0.6.4/pyhon/connection/auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import json
 import logging
 import re
 import secrets
-import sys
 import urllib
 from pprint import pformat
 from urllib import parse
 
 from yarl import URL
 
 from pyhon import const
+from pyhon.exceptions import HonAuthenticationError
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class HonAuth:
     def __init__(self, session, email, password, device) -> None:
         self._session = session
         self._email = email
         self._password = password
         self._access_token = ""
         self._refresh_token = ""
         self._cognito_token = ""
         self._id_token = ""
         self._device = device
+        self._called_urls = []
 
     @property
     def cognito_token(self):
         return self._cognito_token
 
     @property
     def id_token(self):
@@ -37,14 +38,24 @@
     def access_token(self):
         return self._access_token
 
     @property
     def refresh_token(self):
         return self._refresh_token
 
+    async def _error_logger(self, response, fail=True):
+        result = "hOn Authentication Error\n"
+        for i, (status, url) in enumerate(self._called_urls):
+            result += f" {i + 1: 2d}     {status} - {url}\n"
+        result += f"ERROR - {response.status} - {response.request_info.url}\n"
+        result += f"{15 * '='} Response {15 * '='}\n{await response.text()}\n{40 * '='}"
+        _LOGGER.error(result)
+        if fail:
+            raise HonAuthenticationError("Can't login")
+
     async def _load_login(self):
         nonce = secrets.token_hex(16)
         nonce = f"{nonce[:8]}-{nonce[8:12]}-{nonce[12:16]}-{nonce[16:20]}-{nonce[20:]}"
         params = {
             "response_type": "token+id_token",
             "client_id": const.CLIENT_ID,
             "redirect_uri": urllib.parse.quote(
@@ -54,39 +65,45 @@
             "scope": "api openid refresh_token web",
             "nonce": nonce,
         }
         params = "&".join([f"{k}={v}" for k, v in params.items()])
         async with self._session.get(
             f"{const.AUTH_API}/services/oauth2/authorize/expid_Login?{params}"
         ) as response:
-            _LOGGER.debug("%s - %s", response.status, response.request_info.url)
+            self._called_urls.append((response.status, response.request_info.url))
             if not (login_url := re.findall("url = '(.+?)'", await response.text())):
+                await self._error_logger(response)
                 return False
         async with self._session.get(login_url[0], allow_redirects=False) as redirect1:
-            _LOGGER.debug("%s - %s", redirect1.status, redirect1.request_info.url)
+            self._called_urls.append((redirect1.status, redirect1.request_info.url))
             if not (url := redirect1.headers.get("Location")):
+                await self._error_logger(redirect1)
                 return False
         async with self._session.get(url, allow_redirects=False) as redirect2:
-            _LOGGER.debug("%s - %s", redirect2.status, redirect2.request_info.url)
+            self._called_urls.append((redirect2.status, redirect2.request_info.url))
             if not (
                 url := redirect2.headers.get("Location")
                 + "&System=IoT_Mobile_App&RegistrationSubChannel=hOn"
             ):
+                await self._error_logger(redirect2)
                 return False
         async with self._session.get(URL(url, encoded=True)) as login_screen:
-            _LOGGER.debug("%s - %s", login_screen.status, login_screen.request_info.url)
+            self._called_urls.append(
+                (login_screen.status, login_screen.request_info.url)
+            )
             if context := re.findall(
                 '"fwuid":"(.*?)","loaded":(\\{.*?})', await login_screen.text()
             ):
                 fw_uid, loaded_str = context[0]
                 loaded = json.loads(loaded_str)
                 login_url = login_url[0].replace(
                     "/".join(const.AUTH_API.split("/")[:-1]), ""
                 )
                 return fw_uid, loaded, login_url
+            await self._error_logger(login_screen)
         return False
 
     async def _login(self, fw_uid, loaded, login_url):
         data = {
             "message": {
                 "actions": [
                     {
@@ -118,54 +135,50 @@
         params = {"r": 3, "other.LightningLoginCustom.login": 1}
         async with self._session.post(
             const.AUTH_API + "/s/sfsites/aura",
             headers={"Content-Type": "application/x-www-form-urlencoded"},
             data="&".join(f"{k}={json.dumps(v)}" for k, v in data.items()),
             params=params,
         ) as response:
-            _LOGGER.debug("%s - %s", response.status, response.request_info.url)
+            self._called_urls.append((response.status, response.request_info.url))
             if response.status == 200:
                 try:
                     data = await response.json()
                     return data["events"][0]["attributes"]["values"]["url"]
                 except json.JSONDecodeError:
                     pass
                 except KeyError:
                     _LOGGER.error(
                         "Can't get login url - %s", pformat(await response.json())
                     )
-            _LOGGER.error(
-                "Unable to login: %s\n%s", response.status, await response.text()
-            )
+            await self._error_logger(response)
             return ""
 
     async def _get_token(self, url):
         async with self._session.get(url) as response:
-            _LOGGER.debug("%s - %s", response.status, response.request_info.url)
+            self._called_urls.append((response.status, response.request_info.url))
             if response.status != 200:
-                _LOGGER.error("Unable to get token: %s", response.status)
+                await self._error_logger(response)
                 return False
             url = re.findall("href\\s*=\\s*[\"'](.+?)[\"']", await response.text())
-        if not url:
-            _LOGGER.error("Can't get login url - \n%s", await response.text())
-            raise PermissionError
+            if not url:
+                await self._error_logger(response)
+                return False
         if "ProgressiveLogin" in url[0]:
             async with self._session.get(url[0]) as response:
-                _LOGGER.debug("%s - %s", response.status, response.request_info.url)
+                self._called_urls.append((response.status, response.request_info.url))
                 if response.status != 200:
-                    _LOGGER.error("Unable to get token: %s", response.status)
+                    await self._error_logger(response)
                     return False
                 url = re.findall("href\\s*=\\s*[\"'](.*?)[\"']", await response.text())
         url = "/".join(const.AUTH_API.split("/")[:-1]) + url[0]
         async with self._session.get(url) as response:
-            _LOGGER.debug("%s - %s", response.status, response.request_info.url)
+            self._called_urls.append((response.status, response.request_info.url))
             if response.status != 200:
-                _LOGGER.error(
-                    "Unable to connect to the login service: %s", response.status
-                )
+                await self._error_logger(response)
                 return False
             text = await response.text()
         if access_token := re.findall("access_token=(.*?)&", text):
             self._access_token = access_token[0]
         if refresh_token := re.findall("refresh_token=(.*?)&", text):
             self._refresh_token = refresh_token[0]
         if id_token := re.findall("id_token=(.*?)&", text):
@@ -183,32 +196,33 @@
             return False
 
         post_headers = {"id-token": self._id_token}
         data = self._device.get()
         async with self._session.post(
             f"{const.API_URL}/auth/v1/login", headers=post_headers, json=data
         ) as response:
-            _LOGGER.debug("%s - %s", response.status, response.request_info.url)
+            self._called_urls.append((response.status, response.request_info.url))
             try:
                 json_data = await response.json()
             except json.JSONDecodeError:
-                _LOGGER.error("No JSON Data after POST: %s", await response.text())
+                await self._error_logger(response)
                 return False
             self._cognito_token = json_data["cognitoUser"]["Token"]
         return True
 
     async def refresh(self):
         params = {
             "client_id": const.CLIENT_ID,
             "refresh_token": self._refresh_token,
             "grant_type": "refresh_token",
         }
         async with self._session.post(
             f"{const.AUTH_API}/services/oauth2/token", params=params
         ) as response:
-            _LOGGER.debug("%s - %s", response.status, response.request_info.url)
+            self._called_urls.append((response.status, response.request_info.url))
             if response.status >= 400:
+                await self._error_logger(response, fail=False)
                 return False
             data = await response.json()
         self._id_token = data["id_token"]
         self._access_token = data["access_token"]
         return True
```

### Comparing `pyhOn-0.6.3/pyhon/connection/device.py` & `pyhOn-0.6.4/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.3/pyhon/connection/handler.py` & `pyhOn-0.6.4/pyhon/connection/handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from contextlib import asynccontextmanager
 
 import aiohttp
 
 from pyhon import const
 from pyhon.connection.auth import HonAuth, _LOGGER
 from pyhon.connection.device import HonDevice
+from pyhon.exceptions import HonAuthenticationError
 
 
 class HonBaseConnectionHandler:
     _HEADERS = {"user-agent": const.USER_AGENT, "Content-Type": "application/json"}
 
     def __init__(self, session=None):
         self._session = session
@@ -46,17 +47,17 @@
 class HonConnectionHandler(HonBaseConnectionHandler):
     def __init__(self, email, password, session=None):
         super().__init__(session=session)
         self._device = HonDevice()
         self._email = email
         self._password = password
         if not self._email:
-            raise PermissionError("Login-Error - An email address must be specified")
+            raise HonAuthenticationError("An email address must be specified")
         if not self._password:
-            raise PermissionError("Login-Error - A password address must be specified")
+            raise HonAuthenticationError("A password address must be specified")
         self._request_headers = {}
 
     @property
     def device(self):
         return self._device
 
     async def create(self):
@@ -69,15 +70,15 @@
             "cognito-token" not in self._request_headers
             or "id-token" not in self._request_headers
         ):
             if await self._auth.authorize():
                 self._request_headers["cognito-token"] = self._auth.cognito_token
                 self._request_headers["id-token"] = self._auth.id_token
             else:
-                raise PermissionError("Can't Login")
+                raise HonAuthenticationError("Can't login")
         return {h: v for h, v in self._request_headers.items() if h not in headers}
 
     @asynccontextmanager
     async def _intercept(self, method, *args, loop=0, **kwargs):
         kwargs["headers"] = await self._check_headers(kwargs.get("headers", {}))
         async with method(*args, **kwargs) as response:
             if response.status == 403 and not loop:
@@ -96,15 +97,15 @@
             elif loop >= 2:
                 _LOGGER.error(
                     "%s - Error %s - %s",
                     response.request_info.url,
                     response.status,
                     await response.text(),
                 )
-                raise PermissionError("Login failure")
+                raise HonAuthenticationError("Login failure")
             else:
                 try:
                     await response.json()
                     yield response
                 except json.JSONDecodeError:
                     _LOGGER.warning(
                         "%s - JsonDecodeError %s - %s",
@@ -119,9 +120,9 @@
     _HEADERS = HonBaseConnectionHandler._HEADERS | {"x-api-key": const.API_KEY}
 
     @asynccontextmanager
     async def _intercept(self, method, *args, loop=0, **kwargs):
         kwargs["headers"] = kwargs.pop("headers", {}) | self._HEADERS
         async with method(*args, **kwargs) as response:
             if response.status == 403:
-                print("Can't authorize")
+                _LOGGER.error("Can't authenticate anymore")
             yield response
```

### Comparing `pyhOn-0.6.3/pyhon/hon.py` & `pyhOn-0.6.4/pyhon/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.3/pyhon/parameter.py` & `pyhOn-0.6.4/pyhon/parameter.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.3/setup.py` & `pyhOn-0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.6.3",
+    version="0.6.4",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```

