# Comparing `tmp/pyhOn-0.6.4.tar.gz` & `tmp/pyhOn-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.6.4.tar", last modified: Mon Apr 10 23:02:44 2023, max compression
+gzip compressed data, was "pyhOn-0.7.0.tar", last modified: Tue Apr 11 20:20:25 2023, max compression
```

## Comparing `pyhOn-0.6.4.tar` & `pyhOn-0.7.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:02:44.945554 pyhOn-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 23:02:32.000000 pyhOn-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 23:02:44.945554 pyhOn-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-10 23:02:32.000000 pyhOn-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:02:44.941554 pyhOn-0.6.4/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 23:02:44.000000 pyhOn-0.6.4/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-10 23:02:44.000000 pyhOn-0.6.4/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 23:02:44.000000 pyhOn-0.6.4/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 23:02:44.000000 pyhOn-0.6.4/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 23:02:44.000000 pyhOn-0.6.4/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 23:02:44.000000 pyhOn-0.6.4/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:02:44.941554 pyhOn-0.6.4/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4839 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:02:44.941554 pyhOn-0.6.4/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:02:44.945554 pyhOn-0.6.4/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/connection/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/connection/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-10 23:02:32.000000 pyhOn-0.6.4/pyhon/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 23:02:44.945554 pyhOn-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-10 23:02:32.000000 pyhOn-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:25.138927 pyhOn-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 20:20:12.000000 pyhOn-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-11 20:20:25.138927 pyhOn-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-11 20:20:12.000000 pyhOn-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:25.138927 pyhOn-0.7.0/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-11 20:20:25.000000 pyhOn-0.7.0/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-11 20:20:25.000000 pyhOn-0.7.0/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:20:25.000000 pyhOn-0.7.0/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 20:20:25.000000 pyhOn-0.7.0/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 20:20:25.000000 pyhOn-0.7.0/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 20:20:25.000000 pyhOn-0.7.0/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:25.138927 pyhOn-0.7.0/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:25.138927 pyhOn-0.7.0/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:25.138927 pyhOn-0.7.0/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/connection/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/connection/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 20:20:25.138927 pyhOn-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-11 20:20:12.000000 pyhOn-0.7.0/setup.py
```

### Comparing `pyhOn-0.6.4/LICENSE` & `pyhOn-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.4/PKG-INFO` & `pyhOn-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.6.4
+Version: 0.7.0
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.6.4/README.md` & `pyhOn-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.4/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.7.0/pyhOn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.6.4
+Version: 0.7.0
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.6.4/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.7.0/pyhOn.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 pyhOn.egg-info/top_level.txt
 pyhon/__init__.py
 pyhon/__main__.py
 pyhon/appliance.py
 pyhon/commands.py
 pyhon/const.py
 pyhon/exceptions.py
+pyhon/helper.py
 pyhon/hon.py
 pyhon/parameter.py
 pyhon/appliances/__init__.py
 pyhon/appliances/ov.py
 pyhon/appliances/td.py
 pyhon/appliances/wd.py
 pyhon/appliances/wm.py
```

### Comparing `pyhOn-0.6.4/pyhon/appliance.py` & `pyhOn-0.7.0/pyhon/appliance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import importlib
 from contextlib import suppress
 
+from pyhon import helper
 from pyhon.commands import HonCommand
 from pyhon.parameter import HonParameterFixed
 
 
 class HonAppliance:
     def __init__(self, api, info):
         if attributes := info.get("attributes"):
@@ -168,7 +169,19 @@
             "appliance": self.info,
             "statistics": self.statistics,
             **self.parameters,
         }
         if self._extra:
             return self._extra.data(result)
         return result
+
+    @property
+    def diagnose(self):
+        data = self.data.copy()
+        for sensible in ["PK", "SK", "serialNumber", "code"]:
+            data["appliance"].pop(sensible, None)
+        result = helper.pretty_print({"data": self.data}, whitespace="\u200B \u200B ")
+        result += helper.pretty_print(
+            {"commands": helper.create_command(self.commands)},
+            whitespace="\u200B \u200B ",
+        )
+        return result.replace(self.mac_address, "12-34-56-78-90-ab")
```

### Comparing `pyhOn-0.6.4/pyhon/appliances/ov.py` & `pyhOn-0.7.0/pyhon/appliances/ov.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.4/pyhon/commands.py` & `pyhOn-0.7.0/pyhon/commands.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.4/pyhon/connection/api.py` & `pyhOn-0.7.0/pyhon/connection/api.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.4/pyhon/connection/auth.py` & `pyhOn-0.7.0/pyhon/connection/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,17 @@
             fw_uid, loaded, login_url = login_site
         else:
             return False
         if not (url := await self._login(fw_uid, loaded, login_url)):
             return False
         if not await self._get_token(url):
             return False
+        return await self._api_auth()
 
+    async def _api_auth(self):
         post_headers = {"id-token": self._id_token}
         data = self._device.get()
         async with self._session.post(
             f"{const.API_URL}/auth/v1/login", headers=post_headers, json=data
         ) as response:
             self._called_urls.append((response.status, response.request_info.url))
             try:
@@ -221,8 +223,8 @@
             self._called_urls.append((response.status, response.request_info.url))
             if response.status >= 400:
                 await self._error_logger(response, fail=False)
                 return False
             data = await response.json()
         self._id_token = data["id_token"]
         self._access_token = data["access_token"]
-        return True
+        return await self._api_auth()
```

### Comparing `pyhOn-0.6.4/pyhon/connection/device.py` & `pyhOn-0.7.0/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.4/pyhon/connection/handler.py` & `pyhOn-0.7.0/pyhon/connection/handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,33 +71,39 @@
             or "id-token" not in self._request_headers
         ):
             if await self._auth.authorize():
                 self._request_headers["cognito-token"] = self._auth.cognito_token
                 self._request_headers["id-token"] = self._auth.id_token
             else:
                 raise HonAuthenticationError("Can't login")
-        return {h: v for h, v in self._request_headers.items() if h not in headers}
+        return headers | self._request_headers
 
     @asynccontextmanager
     async def _intercept(self, method, *args, loop=0, **kwargs):
         kwargs["headers"] = await self._check_headers(kwargs.get("headers", {}))
         async with method(*args, **kwargs) as response:
-            if response.status == 403 and not loop:
+            if response.status in [401, 403] and loop == 0:
                 _LOGGER.info("Try refreshing token...")
                 await self._auth.refresh()
-                yield await self._intercept(method, *args, loop=loop + 1, **kwargs)
-            elif response.status == 403 and loop < 2:
+                async with self._intercept(
+                    method, *args, loop=loop + 1, **kwargs
+                ) as result:
+                    yield result
+            elif response.status in [401, 403] and loop == 1:
                 _LOGGER.warning(
                     "%s - Error %s - %s",
                     response.request_info.url,
                     response.status,
                     await response.text(),
                 )
                 await self.create()
-                yield await self._intercept(method, *args, loop=loop + 1, **kwargs)
+                async with self._intercept(
+                    method, *args, loop=loop + 1, **kwargs
+                ) as result:
+                    yield result
             elif loop >= 2:
                 _LOGGER.error(
                     "%s - Error %s - %s",
                     response.request_info.url,
                     response.status,
                     await response.text(),
                 )
```

### Comparing `pyhOn-0.6.4/pyhon/hon.py` & `pyhOn-0.7.0/pyhon/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.6.4/pyhon/parameter.py` & `pyhOn-0.7.0/pyhon/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 
 
 def str_to_float(string):
     try:
         return int(string)
     except ValueError:
-        return float(str(string.replace(",", ".")))
+        return float(str(string).replace(",", "."))
 
 
 class HonParameter:
     def __init__(self, key, attributes):
         self._key = key
         self._category = attributes.get("category")
         self._typology = attributes.get("typology")
```

### Comparing `pyhOn-0.6.4/setup.py` & `pyhOn-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.6.4",
+    version="0.7.0",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```

