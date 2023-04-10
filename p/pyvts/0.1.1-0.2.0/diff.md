# Comparing `tmp/pyvts-0.1.1.tar.gz` & `tmp/pyvts-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvts-0.1.1.tar", last modified: Sun Mar 26 06:56:22 2023, max compression
+gzip compressed data, was "pyvts-0.2.0.tar", last modified: Mon Apr 10 22:05:52 2023, max compression
```

## Comparing `pyvts-0.1.1.tar` & `pyvts-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-03-26 06:56:22.945027 pyvts-0.1.1/
--rw-r--r--   0 genteki    (501) staff       (20)     1064 2023-02-09 07:28:50.000000 pyvts-0.1.1/LICENSE
--rw-r--r--   0 genteki    (501) staff       (20)     2221 2023-03-26 06:56:22.944838 pyvts-0.1.1/PKG-INFO
--rw-r--r--   0 genteki    (501) staff       (20)     1425 2023-03-26 06:13:29.000000 pyvts-0.1.1/README.md
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-03-26 06:56:22.944038 pyvts-0.1.1/pyvts/
--rw-r--r--   0 genteki    (501) staff       (20)      166 2023-03-26 06:56:07.000000 pyvts-0.1.1/pyvts/__init__.py
--rw-r--r--   0 genteki    (501) staff       (20)      258 2023-03-02 20:34:19.000000 pyvts-0.1.1/pyvts/config.py
--rw-r--r--   0 genteki    (501) staff       (20)      355 2023-03-26 06:13:29.000000 pyvts-0.1.1/pyvts/error.py
--rw-r--r--   0 genteki    (501) staff       (20)     5032 2023-03-26 06:13:29.000000 pyvts-0.1.1/pyvts/vts.py
--rw-r--r--   0 genteki    (501) staff       (20)     8005 2023-03-26 06:16:58.000000 pyvts-0.1.1/pyvts/vts_request.py
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-03-26 06:56:22.944682 pyvts-0.1.1/pyvts.egg-info/
--rw-r--r--   0 genteki    (501) staff       (20)     2221 2023-03-26 06:56:22.000000 pyvts-0.1.1/pyvts.egg-info/PKG-INFO
--rw-r--r--   0 genteki    (501) staff       (20)      253 2023-03-26 06:56:22.000000 pyvts-0.1.1/pyvts.egg-info/SOURCES.txt
--rw-r--r--   0 genteki    (501) staff       (20)        1 2023-03-26 06:56:22.000000 pyvts-0.1.1/pyvts.egg-info/dependency_links.txt
--rw-r--r--   0 genteki    (501) staff       (20)       19 2023-03-26 06:56:22.000000 pyvts-0.1.1/pyvts.egg-info/requires.txt
--rw-r--r--   0 genteki    (501) staff       (20)        6 2023-03-26 06:56:22.000000 pyvts-0.1.1/pyvts.egg-info/top_level.txt
--rw-r--r--   0 genteki    (501) staff       (20)       38 2023-03-26 06:56:22.945067 pyvts-0.1.1/setup.cfg
--rw-r--r--   0 genteki    (501) staff       (20)     1349 2023-03-26 06:45:08.000000 pyvts-0.1.1/setup.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:05:52.715329 pyvts-0.2.0/
+-rw-r--r--   0 genteki    (501) staff       (20)     1064 2023-02-09 07:28:50.000000 pyvts-0.2.0/LICENSE
+-rw-r--r--   0 genteki    (501) staff       (20)     2987 2023-04-10 22:05:52.715210 pyvts-0.2.0/PKG-INFO
+-rw-r--r--   0 genteki    (501) staff       (20)     2191 2023-04-10 13:57:48.000000 pyvts-0.2.0/README.md
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:05:52.714304 pyvts-0.2.0/pyvts/
+-rw-r--r--   0 genteki    (501) staff       (20)      216 2023-04-10 22:02:46.000000 pyvts-0.2.0/pyvts/__init__.py
+-rw-r--r--   0 genteki    (501) staff       (20)      258 2023-03-02 20:34:19.000000 pyvts-0.2.0/pyvts/config.py
+-rw-r--r--   0 genteki    (501) staff       (20)      355 2023-03-26 06:13:29.000000 pyvts-0.2.0/pyvts/error.py
+-rw-r--r--   0 genteki    (501) staff       (20)     6103 2023-04-10 07:13:50.000000 pyvts-0.2.0/pyvts/vts.py
+-rw-r--r--   0 genteki    (501) staff       (20)    10273 2023-04-10 07:13:50.000000 pyvts-0.2.0/pyvts/vts_request.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:05:52.715005 pyvts-0.2.0/pyvts.egg-info/
+-rw-r--r--   0 genteki    (501) staff       (20)     2987 2023-04-10 22:05:52.000000 pyvts-0.2.0/pyvts.egg-info/PKG-INFO
+-rw-r--r--   0 genteki    (501) staff       (20)      253 2023-04-10 22:05:52.000000 pyvts-0.2.0/pyvts.egg-info/SOURCES.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:05:52.000000 pyvts-0.2.0/pyvts.egg-info/dependency_links.txt
+-rw-r--r--   0 genteki    (501) staff       (20)       19 2023-04-10 22:05:52.000000 pyvts-0.2.0/pyvts.egg-info/requires.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:05:52.000000 pyvts-0.2.0/pyvts.egg-info/top_level.txt
+-rw-r--r--   0 genteki    (501) staff       (20)       38 2023-04-10 22:05:52.715372 pyvts-0.2.0/setup.cfg
+-rw-r--r--   0 genteki    (501) staff       (20)     1196 2023-04-10 22:02:46.000000 pyvts-0.2.0/setup.py
```

### Comparing `pyvts-0.1.1/LICENSE` & `pyvts-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvts-0.1.1/PKG-INFO` & `pyvts-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvts
-Version: 0.1.1
+Version: 0.2.0
 Summary: A python library for interacting with the VTube Studio API
 Home-page: https://github.com/Genteki/pyvts
 Author: Genteki Zhang
 Author-email: zhangkaiyuan.null@gmail.com
 License: MIT
 Keywords: vtubestudio
 Classifier: Development Status :: 3 - Alpha
@@ -19,31 +19,71 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyvts
 [![License: MIT](https://img.shields.io/github/license/Genteki/pyvts?style=flat-square)](https://opensource.org/licenses/MIT) [![issue](https://img.shields.io/github/issues/genteki/pyvts?style=flat-square)](https://github.com/Genteki/pyvts/issues) [![build](https://img.shields.io/circleci/build/github/Genteki/pyvts?style=flat-square)](https://circleci.com/gh/Genteki/pyvts)
 [![codecov](https://img.shields.io/codecov/c/github/genteki/pyvts?color=informational&style=flat-square)](https://codecov.io/gh/Genteki/pyvts)
+[![PyPI](https://img.shields.io/pypi/v/pyvts?style=flat-square)](https://pypi.org/project/pyvts/)
+[![docs](https://img.shields.io/badge/docs-passing-success?style=flat-square)](https://genteki.github.io/pyvts)
 
 A python library for interacting with the [VTube Studio API](https://github.com/DenchiSoft/VTubeStudio).
 
 ## Overview
-Create a class `VTS` connecting to the server running on VTubeStudio (default port: `ws://localhost:8001`).
+`pyvts` is a python library for interacting with the [VTube Studio API](https://github.com/DenchiSoft/VTubeStudio).
 
-Implement functions in `VTS` to send/receive text messages to/from the server, to achieve developers' goals. For example, adding new tracking parameters to enable more actions on live2d avatars.
+You can easily use the library to develop VTubeStudio Plugin to achieve your goals. For example, adding new tracking parameters to enable more actions on live2d avatars.
 
-## Installation
+## Quick Start
 
-> pip3 install pyvts
+### Installation
+
+```
+pip3 install pyvts 
+```
+
+### Get Started
+
+First import library you need,
+```
+import pyvts
+import asyncio
+```
+
+Then specify your plugin information
+```
+plugin_info = {
+    "plugin_name": "[plugin name]",
+    "developer": "[your name]",
+    "authentication_token_path": "./token.txt",
+}
+```
+Create an instance and do whateveer you want!
+```
+async def main():
+    vts = pyvts.vts(plugin_info=plugin_info)
+    await vts.connect()
+    # Implement what you want to do
+    await vts.close()
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+
+### Demo
 
-## Quick Start
 Demo [examples/start.py](./examples/start.py) is a good startpoint to make plugin for VTubeStudio. 
 
-Before you get started, make sure you've installed all the dependcies
+Before you get started, make sure you've clone the library and installed all the dependcies
 
-> pip3 install -r requirements.txt
+```
+pip3 install -r requirements.txt 
+```
 
 Then, launch `VTubeStudio`, and run
 
-> python3 examples/start.py
+``` 
+python3 examples/start.py 
+```
 
 in command line. You will see a new tracking parameter "start_parameter" added to VTubeStudio and some information about it in command line ouput.
```

### Comparing `pyvts-0.1.1/README.md` & `pyvts-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,67 @@
 # pyvts
 [![License: MIT](https://img.shields.io/github/license/Genteki/pyvts?style=flat-square)](https://opensource.org/licenses/MIT) [![issue](https://img.shields.io/github/issues/genteki/pyvts?style=flat-square)](https://github.com/Genteki/pyvts/issues) [![build](https://img.shields.io/circleci/build/github/Genteki/pyvts?style=flat-square)](https://circleci.com/gh/Genteki/pyvts)
 [![codecov](https://img.shields.io/codecov/c/github/genteki/pyvts?color=informational&style=flat-square)](https://codecov.io/gh/Genteki/pyvts)
+[![PyPI](https://img.shields.io/pypi/v/pyvts?style=flat-square)](https://pypi.org/project/pyvts/)
+[![docs](https://img.shields.io/badge/docs-passing-success?style=flat-square)](https://genteki.github.io/pyvts)
 
 A python library for interacting with the [VTube Studio API](https://github.com/DenchiSoft/VTubeStudio).
 
 ## Overview
-Create a class `VTS` connecting to the server running on VTubeStudio (default port: `ws://localhost:8001`).
+`pyvts` is a python library for interacting with the [VTube Studio API](https://github.com/DenchiSoft/VTubeStudio).
 
-Implement functions in `VTS` to send/receive text messages to/from the server, to achieve developers' goals. For example, adding new tracking parameters to enable more actions on live2d avatars.
+You can easily use the library to develop VTubeStudio Plugin to achieve your goals. For example, adding new tracking parameters to enable more actions on live2d avatars.
 
-## Installation
+## Quick Start
 
-> pip3 install pyvts
+### Installation
+
+```
+pip3 install pyvts 
+```
+
+### Get Started
+
+First import library you need,
+```
+import pyvts
+import asyncio
+```
+
+Then specify your plugin information
+```
+plugin_info = {
+    "plugin_name": "[plugin name]",
+    "developer": "[your name]",
+    "authentication_token_path": "./token.txt",
+}
+```
+Create an instance and do whateveer you want!
+```
+async def main():
+    vts = pyvts.vts(plugin_info=plugin_info)
+    await vts.connect()
+    # Implement what you want to do
+    await vts.close()
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+
+### Demo
 
-## Quick Start
 Demo [examples/start.py](./examples/start.py) is a good startpoint to make plugin for VTubeStudio. 
 
-Before you get started, make sure you've installed all the dependcies
+Before you get started, make sure you've clone the library and installed all the dependcies
 
-> pip3 install -r requirements.txt
+```
+pip3 install -r requirements.txt 
+```
 
 Then, launch `VTubeStudio`, and run
 
-> python3 examples/start.py
+``` 
+python3 examples/start.py 
+```
 
 in command line. You will see a new tracking parameter "start_parameter" added to VTubeStudio and some information about it in command line ouput.
```

### Comparing `pyvts-0.1.1/pyvts/vts.py` & `pyvts-0.2.0/pyvts/vts.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,34 +2,43 @@
 import json
 import websockets
 import aiofiles
 from pyvts import vts_request, config, error
 
 
 class vts:
-    """VtubeStudio Connector"""
+    """``VtubeStudio API`` Connector"""
 
     def __init__(
         self,
         plugin_info: dict = config.plugin_default,
         vts_api_info: dict = config.vts_api,
         **kwargs
     ) -> None:
         """
-        plugin_info: {
-            "plugin_name": your plugin name (str),
-            "developer": your name (str),
-            "icon": (optional) your icon if exist (img),
-            "authentication_token_path": str
-        }
-        vts_api_info: {
-            "version": str,
-            "name": str,
-            "port": int
-        }
+        Parameters
+        ----------
+        plugin_info : dict
+            {
+                "plugin_name": str,
+                "developer": str,
+                "icon": (optional) str,
+                "authentication_token_path": str
+            }
+        vts_api_info: dict
+            {
+                "version": str,
+                "name": str,
+                "port": int
+            }
+
+        Returns
+        -------
+        pyvts.vts
+            ``VtubeStudio API`` connector
         """
         self.port = vts_api_info["port"]
         self.websocket = None
         self.authentic_token = None
         self.__connection_status = 0  # 0: not connected, 1: connected
         self.__authentic_status = (
             0  # 0:no authen & token, 1:has token, 2:authen, -1:wrong token
@@ -65,15 +74,24 @@
         """close the websocket connection"""
         await self.websocket.close(code=1000, reason="user closed")
         self.__connection_status = 0
 
     async def request(self, request_msg: dict) -> dict:
         """
         send request to VTubeStudio
-        request_msg: message generated from VTSRequest (dict)
+
+        Parameters
+        ----------
+        request_msg : dict
+            message generated from ``VTSRequest``
+
+        Returns
+        -------
+        dict
+            message from VTubeStudio API, data is stored in ``return_dict["data"]``
         """
         await self.websocket.send(json.dumps(request_msg))
         response_msg = await self.websocket.recv()
         response_dict = json.loads(response_msg)
         return response_dict
 
     async def request_authenticate_token(self) -> None:
@@ -85,15 +103,26 @@
             self.authentic_token = response_dict["data"]["authenticationToken"]
             if self.__authentic_status == 0 or self.__authentic_status == -1:
                 self.__authentic_status = 1
         except AssertionError:
             print("authentication failed")
 
     async def request_authenticate(self) -> bool:
-        """get authenticated from vtubestudio to have more access"""
+        """
+        get authenticated from vtubestudio to have more access
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        --------
+        bools
+            true - authentication succeed, fale - authentication failed
+        """
         require_msg = self.vts_request.authentication(self.authentic_token)
         responese_dict = await self.request(require_msg)
         try:
             assert responese_dict["data"]["authenticated"], "Authentication Failed"
             self.__authentic_status = 2
         except AssertionError:
             self.__authentic_status = -1
@@ -116,18 +145,44 @@
             async with aiofiles.open(self.token_path, mode="w") as f_token:
                 await f_token.seek(0)
                 await f_token.write(self.authentic_token)
         except FileNotFoundError:
             print("write authentic token files failed")
 
     def get_authentic_status(self) -> int:
-        """get authentic status"""
+        """
+        get authentic status
+
+        Returns
+        --------
+        int
+            authentic status,  0 - no authen & token, 1 - has token, 2 - authen, -1 - wrong token
+        """
         return self.__authentic_status
 
     def get_connection_status(self) -> int:
-        """get connection status"""
+        """
+        get connection status
+
+        Returns
+        --------
+        int
+            connection status, 0: not connected, 1: connected
+        """
         return self.__connection_status
 
     async def event_subscribe(self, msg: dict) -> dict:
-        """subscribe event from vts api"""
+        """
+        subscribe event from vts api
+
+        Parameters
+        -----------
+        msg : dict
+            event subscription message generated from method of `VTSRequest`
+
+        Returns
+        -------
+        dict
+            message returned from VTube Studio API
+        """
         # set up lisening action
         return await self.request(msg)
```

### Comparing `pyvts-0.1.1/pyvts/vts_request.py` & `pyvts-0.2.0/pyvts/vts_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,75 +6,144 @@
 
 
 class VTSRequest:
     """VtubeStudio API Request Generator"""
 
     def __init__(
         self,
-        developer: dict = config.plugin_default["developer"],
-        plugin_name: dict = config.plugin_default["plugin_name"],
+        developer: str = config.plugin_default["developer"],
+        plugin_name: str = config.plugin_default["plugin_name"],
         **kwargs
-    ) -> None:
+    ):
+        """
+        VtubeStudio API Request Generator
+
+        Parameters
+        ----------
+        developer : str
+            developer the your plugin
+        plugin_name : dict
+            plugin name
+        **kwargs
+            other parameters like ``api_version``, ``api_version``,
+            not needed in most cases
+
+        Returns:
+            pyvts.VTSRequest
+                request generator
+        """
         self.developer = developer
         self.plugin_name = plugin_name
         self.api_version = API_VERSION
         self.api_name = API_NAME
         self.icon = None
         for key, value in kwargs.items():
             setattr(self, key, value)
 
     def BaseRequest(
         self, message_type: str, data: dict = None, request_id: str = "SomeID"
     ) -> dict:
-        """Standard Request"""
+        """
+        Standard Request
+
+        Parameters
+        ----------
+        message_type : str
+            Message type of request
+        data : dict
+            optional, relavent data sending to ``VTubeStudio API``
+        request_id : str
+            string to mark the request, not important
+
+        Returns
+        -------
+        dict of {"apiName: str, "apiVersion": str, "requestID": str, "messageType: str, "data": dict}
+            the organized message sending to ``Vtubestudio API``
+        """
+
         msg = {
             "apiName": self.api_name,
             "apiVersion": self.api_version,
             "requestID": request_id,
             "messageType": message_type,
             "data": data,
         }
         return msg
 
     def authentication_token(self) -> dict:
-        """generate request msg to requirer authentication_token"""
+        """
+        generate request msg to requirer authentication_token
+
+        Returns
+        ------
+        dict
+            the organized message sending to ``Vtubestudio API``
+
+        Examples
+        ---------
+        >>> message = myvts.vts_request.authentication_token()
+        >>> return_msg = await myvts.request(message)
+        """
         # Plugin icons should be 128x128 pixel Base64-encoded PNGs.
         msg_type = "AuthenticationTokenRequest"
         data = {
             "pluginName": self.plugin_name,
             "pluginDeveloper": self.developer,
         }
         if self.icon is not None:
             data["pluginIcon"] = self.icon
         return self.BaseRequest(msg_type, data)
 
     def authentication(self, token) -> dict:
         """
         use auth_token to get more access
-        token: authenication token (str)
+
+        Parameters
+        ----------
+        token : str
+            authenication token
+
+        Returns
+        -------
+        dict
+            the organized message sending to ``Vtubestudio API``
         """
         msg_type = "AuthenticationRequest"
         data = {
             "pluginName": self.plugin_name,
             "pluginDeveloper": self.developer,
             "authenticationToken": token,
         }
         return self.BaseRequest(msg_type, data)
 
     def requestMoveModel(
         self, x, y, rot=0, size=1, relative=True, move_time=0.2
     ) -> dict:
         """
         request to move the model
-            x, y: location of model,
+
+        Parameters
+        -----------
+            x, y : float
+                location of model,
                 if relative == False:  [0, 0] means the middle of the model in the middle of the screen
                 else if relative == True: [0, 0] means location of model center point
-            rot: rotation, range [-360, 360]
-            size: zoom in/out
-            relative: the values are (not) considered to be relative to the current model position
+            rot : float
+                rotation angle, range [-360, 360]
+            size : float
+                zoom ratio, default: 1
+            relative : bool
+                whether the values are considered to be relative to the current model position
+            move_time : float
+                time of the move motion
+
+        Returns
+        -------
+        dict of {data: dict}
+            the organized message sending to ``Vtubestudio API``
         """
         msg_type = "MoveModelRequest"
         data = {
             "timeInSeconds": move_time,
             "valuesAreRelativeToModel": relative,
             "positionX": x,
             "positionY": y,
@@ -83,34 +152,47 @@
         }
         return self.BaseRequest(msg_type, data)
 
     def requestHotKeyList(self) -> dict:
         return self.BaseRequest("HotkeysInCurrentModelRequest")
 
     def requestTriggerHotKey(self, hotkeyID):
-        # TODO
+        """TODO"""
         pass
 
     def requestTrackingParameterList(self) -> dict:
         return self.BaseRequest("InputParameterListRequest")
 
     def requestParameterValue(self, parameter: str) -> dict:
         data = {"name": parameter}
         return self.BaseRequest("ParameterValueRequest", data=data)
 
     def requestCustomParameter(
         self, parameter: str, min=0, max=1, default_value=0, info=""
     ) -> dict:
         """
         Add your own new tracking parameters and use them in your VTube Studio models
-        parameter: parameter name (str)
-        min: minimum bound for the parameter (float)
-        max: maximum bound for the parameter (float)
-        default_value: default value (float)
-        info: description (str)
+
+        Parameters
+        -----------
+        parameter : str
+            name of parameter
+        min : float
+            minimum bound for the parameter
+        max : float
+            maximum bound for the parameter
+        default_value : float
+            default value
+        info : str
+            description of this parameter
+
+        Returns
+        -------
+        dict
+            the organized message sending to ``Vtubestudio API``
         """
         data = {
             "parameterName": parameter,
             "explanation": info,
             "min": min,
             "max": max,
             "defaultValue": default_value,
@@ -123,19 +205,32 @@
         value: float,
         weight: float = 1,
         face_found=False,
         mode="set",
     ) -> dict:
         """
         Set value for any default or custom parameter.
-        parameter: name of the parameter (str)
-        value: value of the data from -1000000 to 1000000 (float)
-        weight: you can mix the your value with vts face tracking parameter, from 0 to 1 (float)
-        face_found: if true, you will tell VTubeStudio to consider the user face as found,
+
+        Parameters
+        ----------
+        parameter : str
+            name of the parameter
+        value : float
+            value of the data from -1000000 to 1000000
+        weight : float
+            you can mix the your value with vts face tracking parameter, from 0 to 1,
+            defualt(no mixture): 1
+        face_found : bool
+            if true, you will tell VTubeStudio to consider the user face as found,
             s.t. you can control when the "tracking lost"
+
+        Returns
+        -------
+        dict
+            the organized message sending to ``Vtubestudio API``
         """
         data = {
             "faceFound": face_found,
             "mode": mode,
             "parameterValues": [{"id": parameter, "weight": weight, "value": value}],
         }
         return self.BaseRequest("InjectParameterDataRequest", data=data)
@@ -144,18 +239,24 @@
         data = {"parameterName": parameter}
         return self.BaseRequest("ParameterDeletionRequest", data=data)
 
     def eventSubscription(
         self, event_name: str, on: bool = True, cfg: dict = {"0": 0}
     ) -> dict:
         """
-        subscribe event from vtubestudio api
-        event_name: event name you want to substribe (str)
-        on: turn on or turn off (bool)
-        cfg: config message (dict, optional)
+        subscribe event from vtubestudio api (base function, seldom directly used)
+
+        Parameters
+        ----------
+        event_name : string
+            event name you want to substribe
+        on : bool
+            turn on or turn off
+        cfg : dict
+            optional, config message
         """
         msg_type = "EventSubscriptionRequest"
         data = {"eventName": event_name, "subscribe": on, "config": cfg}
         return self.BaseRequest(msg_type, data)
 
     def eventSubscriptionTest(self, test_msg="text the event will return"):
         """
```

### Comparing `pyvts-0.1.1/pyvts.egg-info/PKG-INFO` & `pyvts-0.2.0/pyvts.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvts
-Version: 0.1.1
+Version: 0.2.0
 Summary: A python library for interacting with the VTube Studio API
 Home-page: https://github.com/Genteki/pyvts
 Author: Genteki Zhang
 Author-email: zhangkaiyuan.null@gmail.com
 License: MIT
 Keywords: vtubestudio
 Classifier: Development Status :: 3 - Alpha
@@ -19,31 +19,71 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyvts
 [![License: MIT](https://img.shields.io/github/license/Genteki/pyvts?style=flat-square)](https://opensource.org/licenses/MIT) [![issue](https://img.shields.io/github/issues/genteki/pyvts?style=flat-square)](https://github.com/Genteki/pyvts/issues) [![build](https://img.shields.io/circleci/build/github/Genteki/pyvts?style=flat-square)](https://circleci.com/gh/Genteki/pyvts)
 [![codecov](https://img.shields.io/codecov/c/github/genteki/pyvts?color=informational&style=flat-square)](https://codecov.io/gh/Genteki/pyvts)
+[![PyPI](https://img.shields.io/pypi/v/pyvts?style=flat-square)](https://pypi.org/project/pyvts/)
+[![docs](https://img.shields.io/badge/docs-passing-success?style=flat-square)](https://genteki.github.io/pyvts)
 
 A python library for interacting with the [VTube Studio API](https://github.com/DenchiSoft/VTubeStudio).
 
 ## Overview
-Create a class `VTS` connecting to the server running on VTubeStudio (default port: `ws://localhost:8001`).
+`pyvts` is a python library for interacting with the [VTube Studio API](https://github.com/DenchiSoft/VTubeStudio).
 
-Implement functions in `VTS` to send/receive text messages to/from the server, to achieve developers' goals. For example, adding new tracking parameters to enable more actions on live2d avatars.
+You can easily use the library to develop VTubeStudio Plugin to achieve your goals. For example, adding new tracking parameters to enable more actions on live2d avatars.
 
-## Installation
+## Quick Start
 
-> pip3 install pyvts
+### Installation
+
+```
+pip3 install pyvts 
+```
+
+### Get Started
+
+First import library you need,
+```
+import pyvts
+import asyncio
+```
+
+Then specify your plugin information
+```
+plugin_info = {
+    "plugin_name": "[plugin name]",
+    "developer": "[your name]",
+    "authentication_token_path": "./token.txt",
+}
+```
+Create an instance and do whateveer you want!
+```
+async def main():
+    vts = pyvts.vts(plugin_info=plugin_info)
+    await vts.connect()
+    # Implement what you want to do
+    await vts.close()
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+
+### Demo
 
-## Quick Start
 Demo [examples/start.py](./examples/start.py) is a good startpoint to make plugin for VTubeStudio. 
 
-Before you get started, make sure you've installed all the dependcies
+Before you get started, make sure you've clone the library and installed all the dependcies
 
-> pip3 install -r requirements.txt
+```
+pip3 install -r requirements.txt 
+```
 
 Then, launch `VTubeStudio`, and run
 
-> python3 examples/start.py
+``` 
+python3 examples/start.py 
+```
 
 in command line. You will see a new tracking parameter "start_parameter" added to VTubeStudio and some information about it in command line ouput.
```

### Comparing `pyvts-0.1.1/setup.py` & `pyvts-0.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-
 """A python library for interacting with the VTube Studio API"""
 
 from setuptools import setup, find_packages
 import pyvts
 
 DESCRIPTION = "A python library for interacting with the VTube Studio API"
 VERSION = pyvts.__version__
 
-setup(name='pyvts',
-      version=VERSION,
-      description=DESCRIPTION,
-      long_description=open("README.md", encoding="utf-8").read(),
-      long_description_content_type='text/markdown',
-      keywords='vtubestudio',
-      classifiers=['Development Status :: 3 - Alpha',
-                   'Intended Audience :: Developers',
-                   'License :: OSI Approved :: MIT License',
-                   'Operating System :: Microsoft :: Windows',
-                   'Operating System :: MacOS',
-                   'Programming Language :: Python',
-                   'Programming Language :: Python :: 3',
-                   'Programming Language :: Python :: 3.8',
-                   'Programming Language :: Python :: 3.9',
-                   'Programming Language :: Python :: 3.10'],
-      author='Genteki Zhang',
-      author_email='zhangkaiyuan.null@gmail.com',
-      url='https://github.com/Genteki/pyvts',
-      license='MIT',
-      packages=find_packages(exclude=['*.tests',
-                                      '*.tests.*']),
-      install_requires=['websockets',
-                        'aiofile'])
+setup(
+    name="pyvts",
+    version=VERSION,
+    description=DESCRIPTION,
+    long_description=open("README.md", encoding="utf-8").read(),
+    long_description_content_type="text/markdown",
+    keywords="vtubestudio",
+    classifiers=[
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: MacOS",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+    ],
+    author="Genteki Zhang",
+    author_email="zhangkaiyuan.null@gmail.com",
+    url="https://github.com/Genteki/pyvts",
+    license="MIT",
+    packages=find_packages(where="pyvts", exclude=["tests.*", "tests"]),
+    install_requires=["websockets", "aiofile"],
+)
```

