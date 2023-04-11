# Comparing `tmp/runzero_sdk-0.1.1.tar.gz` & `tmp/runzero_sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runzero_sdk-0.1.1.tar", max compression
+gzip compressed data, was "runzero_sdk-0.2.0.tar", max compression
```

## Comparing `runzero_sdk-0.1.1.tar` & `runzero_sdk-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      193 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/LICENSE
--rw-r--r--   0        0        0     6342 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/README.md
--rw-r--r--   0        0        0     4402 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      507 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/__init__.py
--rw-r--r--   0        0        0      402 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/api/__init__.py
--rw-r--r--   0        0        0      335 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/api/admin/__init__.py
--rw-r--r--   0        0        0    11420 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/api/admin/_sdk_source_icon.py
--rw-r--r--   0        0        0     5513 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/api/admin/asset_data_sources.py
--rw-r--r--   0        0        0     3462 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/api/admin/orgs.py
--rw-r--r--   0        0        0     2670 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/api/asset_data_sources.py
--rw-r--r--   0        0        0      274 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/api/imports/__init__.py
--rw-r--r--   0        0        0     4571 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/api/imports/assets.py
--rw-r--r--   0        0        0     4409 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/api/sites.py
--rw-r--r--   0        0        0     3167 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/api/tasks.py
--rw-r--r--   0        0        0      328 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/client/__init__.py
--rw-r--r--   0        0        0      318 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/client/_http/__init__.py
--rw-r--r--   0        0        0     2496 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/client/_http/auth.py
--rw-r--r--   0        0        0     8168 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/client/_http/io.py
--rw-r--r--   0        0        0    10892 2023-03-30 15:34:29.598529 runzero_sdk-0.1.1/runzero/client/client.py
--rw-r--r--   0        0        0     4901 2023-03-30 15:34:29.602529 runzero_sdk-0.1.1/runzero/client/errors.py
--rw-r--r--   0        0        0     1077 2023-03-30 15:34:29.602529 runzero_sdk-0.1.1/runzero/errors.py
--rw-r--r--   0        0        0        0 2023-03-30 15:34:29.602529 runzero_sdk-0.1.1/runzero/py.typed
--rw-r--r--   0        0        0     1120 2023-03-30 15:34:29.602529 runzero_sdk-0.1.1/runzero/types/__init__.py
--rw-r--r--   0        0        0    18115 2023-03-30 15:34:29.602529 runzero_sdk-0.1.1/runzero/types/_data_models_gen.py
--rw-r--r--   0        0        0     2126 2023-03-30 15:34:29.602529 runzero_sdk-0.1.1/runzero/types/_wrapped.py
--rw-r--r--   0        0        0      762 2023-03-30 15:34:29.602529 runzero_sdk-0.1.1/runzero/types/errors.py
--rw-r--r--   0        0        0       64 2023-03-30 15:34:29.602529 runzero_sdk-0.1.1/runzero/version.py
--rw-r--r--   0        0        0     7514 1970-01-01 00:00:00.000000 runzero_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      193 2023-04-11 04:00:57.041114 runzero_sdk-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6467 2023-04-11 04:00:57.041114 runzero_sdk-0.2.0/README.md
+-rw-r--r--   0        0        0     4402 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      507 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/__init__.py
+-rw-r--r--   0        0        0      423 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/__init__.py
+-rw-r--r--   0        0        0      346 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/admin/__init__.py
+-rw-r--r--   0        0        0    11425 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/admin/_sdk_source_icon.py
+-rw-r--r--   0        0        0     5728 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/admin/custom_integrations.py
+-rw-r--r--   0        0        0     3462 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/admin/orgs.py
+-rw-r--r--   0        0        0     2775 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/custom_integrations.py
+-rw-r--r--   0        0        0      274 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/imports/__init__.py
+-rw-r--r--   0        0        0     4675 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/imports/assets.py
+-rw-r--r--   0        0        0     4409 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/sites.py
+-rw-r--r--   0        0        0     3167 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/api/tasks.py
+-rw-r--r--   0        0        0      441 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/client/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/client/_http/__init__.py
+-rw-r--r--   0        0        0     2496 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/client/_http/auth.py
+-rw-r--r--   0        0        0     8637 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/client/_http/io.py
+-rw-r--r--   0        0        0    11384 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/client/client.py
+-rw-r--r--   0        0        0     6443 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/client/errors.py
+-rw-r--r--   0        0        0     1077 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/errors.py
+-rw-r--r--   0        0        0        0 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/py.typed
+-rw-r--r--   0        0        0     1298 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/types/__init__.py
+-rw-r--r--   0        0        0    18695 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/types/_data_models_gen.py
+-rw-r--r--   0        0        0     2319 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/types/_rate_limit_information.py
+-rw-r--r--   0        0        0     2126 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/types/_wrapped.py
+-rw-r--r--   0        0        0      762 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/types/errors.py
+-rw-r--r--   0        0        0       64 2023-04-11 04:00:57.045113 runzero_sdk-0.2.0/runzero/version.py
+-rw-r--r--   0        0        0     7639 1970-01-01 00:00:00.000000 runzero_sdk-0.2.0/PKG-INFO
```

### Comparing `runzero_sdk-0.1.1/README.md` & `runzero_sdk-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,30 +49,31 @@
 
 ## Modules
 
 The runzero-sdk package contains the following modules to group functionality.
 
 ### runzero.api
 
-The `api` module contains all the http handlers for interacting with runZero api resources such as Sites, Orgs, Tasks, Custom Sources, etc.
+The `api` module contains all the http handlers for interacting with runZero api resources such as Sites, Orgs, Tasks, Custom Integrations, etc.
 
 ### runzero.types
 
 The `types` module contains all the pydantic classes required for interacting with the runZero API resources such as Import Assets, Sites, Tasks, etc.
 
 ## Custom Import Asset field mappings
 
-The following fields are available to be set for custom source asset imports. Any field which matches the below field
+The following fields are available to be set for custom integration asset imports. Any field which matches the below field
 names, either directly or via remapping, will be inserted into the corresponding `ImportAsset` field and validated to
 ensure it meets the outlined constraints.
 
 Any field which does not match the fields below will be placed under the `custom_attributes` field. Please see the
 `ImportAsset` schema definition for more details: #/components/schemas/ImportAsset
 
-* `id` - this `str` field is ***required*** to be set for all custom source assets and is the unique identifier for the asset. If your asset does not have a unique id then we recommend you create one using `uuid.uuid4()`.
+* `id` - this `str` field is ***required*** to be set for all custom integration assets and is the unique identifier for the asset. If your asset does not have a unique id then we recommend you create one using `uuid.uuid4()`.
+* `runZeroID` - a `uuid` field representing the unique identifier of an existing runZero asset to merge into.
 * `network_interfaces` - this field is an array of objects representing the network interfaces of the asset. Please see the API Schema for details. #/components/schemas/ImportAsset/properties/networkInterfaces.
 * `hostnames` - a `List[str]` field of all the hostnames associated with the asset. Each hostname has a maximum length of 260 characters and the `list` has a maximum of 100 hostnames.
 * `domain` - a `str` field representing the domain associated with the asset. Maximum length of 260 characters.
 * `first_seen_ts` - a `datetime.datetime` field representing the first time an asset was seen.
 * `last_seen_ts` - a `datetime.datetime` field representing the last time an asset was seen.
 * `os` - a `str` field which describes the operating system on the asset. Maximum length of 1024 characters.
 * `os_version` - a `str` field which describes the version of the operating system running on the asset. Maximum length of 1024 characters.
```

### Comparing `runzero_sdk-0.1.1/pyproject.toml` & `runzero_sdk-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "runzero-sdk"
-version = "0.1.1"
+version = "0.2.0"
 description = "The runZero platform sdk"
 license = "BSD-2-Clause"
 authors = ["runZero <support@runzero.com>"]
 readme = "README.md"
 homepage = "https://runzero.com/"
 repository = "https://github.com/runZeroInc/runzero-sdk-py"
 keywords = ["runzero", "api", "sdk"]
```

### Comparing `runzero_sdk-0.1.1/runzero/api/admin/_sdk_source_icon.py` & `runzero_sdk-0.2.0/runzero/api/admin/_sdk_source_icon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""this private module holds only the default python SDK custom source icon in base64 encoded format"""
+"""this private module holds only the default python SDK custom integration icon in base64 encoded format"""
 # pylint: disable=C0301
 _PY_ICON_BYTES = (
     b"\x89PNG\r\n\x1a\n\x00\x00\x00\rIHDR\x00\x00\x00 \x00\x00\x00"
     b" \x08\x06\x00\x00\x00szz\xf4\x00\x00\x00\x04gAMA\x00\x00\xb1\x8f\x0b\xfca\x05\x00\x00\nIiCCPsRGB"
     b' IEC61966-2.1\x00\x00H\x89\x9dSwX\x93\xf7\x16>\xdf\xf7e\x0fVB\xd8\xf0\xb1\x97l\x81\x00"#\xac\x08\xc8\x10Y\xa2\x10\x92\x00a\x84\x10\x12@\xc5\x85\x88\nV\x14\x15\x11\x9cHU\xc4\x82\xd5\nH\x9d\x88\xe2\xa0(\xb8gA\x8a\x88Z\x8bU\\8\xee\x1f\xdc\xa7\xb5}z\xef\xed\xed\xfb\xd7\xfb\xbc\xe7\x9c\xe7\xfc\xcey\xcf\x0f\x80\x11\x12&\x91\xe6\xa2j\x009R\x85<:\xd8\x1f\x8fOH\xc4\xc9\xbd\x80\x02\x15H\xe0\x04'
     b" \x10\xe6\xcb\xc2g\x05\xc5\x00\x00\xf0\x03yx~t\xb0?\xfc\x01\xafo\x00\x02\x00p\xd5.$\x12\xc7\xe1\xff\x83\xbaP&W\x00"
     b' \x91\x00\xe0"\x12\xe7\x0b\x01\x90R\x00\xc8.T\xc8\x14\x00\xc8\x18\x00\xb0S\xb3d\n\x00\x94\x00\x00ly|B"\x00\xaa\r\x00\xec\xf4I>\x05\x00\xd8\xa9\x93\xdc\x17\x00\xd8\xa2\x1c\xa9\x08\x00\x8d\x01\x00\x99(G$\x02@\xbb\x00`U\x81R,\x02\xc0\xc2\x00\xa0\xac@".\x04\xc0\xae\x01\x80Y\xb62G\x02\x80\xbd\x05\x00v\x8eX\x90\x0f@`\x00\x80\x99B,\xcc\x00'
```

### Comparing `runzero_sdk-0.1.1/runzero/api/admin/asset_data_sources.py` & `runzero_sdk-0.2.0/runzero/api/admin/custom_integrations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,138 +1,140 @@
 """
-enables administrative management of runZero asset data sources, including write operations.
+enables administrative management of runZero custom integrations, including write operations.
 
 These operations are privileged and require an account token directly or an OAuth key that can generate one.
 """
 import base64
 import pathlib
 import uuid
 from pathlib import Path
 from typing import Any, List, Optional, Union
 
 from runzero.client import Client
 from runzero.errors import Error
-from runzero.types import AssetCustomSource, BaseAssetCustomSource, NewAssetCustomSource
+from runzero.types import BaseCustomIntegration, CustomIntegration, NewCustomIntegration
 
 from ._sdk_source_icon import _PY_ICON_BYTES
 
 
-class CustomSourcesAdmin:
-    """Full Management of Custom Asset data sources.
+class CustomIntegrationsAdmin:
+    """Full Management of custom integrations.
 
-    Full management of custom data sources are descriptive registered associations
-    between sources of data and assets imported which are associated with those sources.
+    Full management of custom integrations are descriptive registered associations
+    between integrations of data and assets imported which are associated with those integrations.
 
-    This is a superset of operations available in runzero.asset_data_sources.CustomSources
+    This is a superset of operations available in runzero.custom_integrations.CustomIntegrations
     which allows only read operations.
 
     :param client: A handle to the :class:`runzero.Client` which manages interactions
         with the runZero server.
     """
 
-    _ENDPOINT = "api/v1.0/account/sources"
+    _ENDPOINT = "api/v1.0/account/custom-integrations"
 
     PYTHON_ICON = _PY_ICON_BYTES
-    """A default icon representing a custom source defined via this Python SDK."""
+    """A default icon representing a custom integration defined via this Python SDK."""
 
     def __init__(self, client: Client):
         """Constructor method"""
         self._client = client
 
-    def get_all(self) -> List[AssetCustomSource]:
+    def get_all(self) -> List[CustomIntegration]:
         """
-        Lists all custom asset sources available to your account.
+        Lists all custom integrations available to your account.
 
-        :return: List of custom asset sources
+        :return: List of custom integrations
         :raises AuthError, ClientError, ServerError
         """
         res = self._client.execute("GET", self._ENDPOINT)
-        result: List[AssetCustomSource] = []
+        result: List[CustomIntegration] = []
         for src in res.json_obj:
             result.append(_resp_to_source(src))
         return result
 
-    def get(self, name: Optional[str] = None, source_id: Optional[uuid.UUID] = None) -> Optional[AssetCustomSource]:
+    def get(
+        self, name: Optional[str] = None, custom_integration_id: Optional[uuid.UUID] = None
+    ) -> Optional[CustomIntegration]:
         """
-        Retrieves runZero custom sources with either the matching ID or Name.
+        Retrieves runZero custom integrations with either the matching ID or Name.
 
         :param name: Optional, name of the organization you want the UUID for
-        :param source_id: Optional, the id of the source you want returned
+        :param custom_integration_id: Optional, the id of the source you want returned
         :raises AuthError, ClientError, ServerError
-            ValueError if neither source_id nor name are provided.
-        :return: The matching AssetCustomSource or None
+            ValueError if neither custom_integration_id nor name are provided.
+        :return: The matching CustomIntegration or None
         """
-        if name is None and source_id is None:
-            raise ValueError("must provide source_id or source name")
-        if source_id is not None:
-            res = self._client.execute("GET", f"{self._ENDPOINT}/{str(source_id)}")
+        if name is None and custom_integration_id is None:
+            raise ValueError("must provide custom_integration_id or source name")
+        if custom_integration_id is not None:
+            res = self._client.execute("GET", f"{self._ENDPOINT}/{str(custom_integration_id)}")
             return _resp_to_source(res.json_obj)
         # name
         for src in self.get_all():
             if src.name == name:
                 return src
         return None
 
     def create(
         self,
         name: str,
         description: Optional[str] = None,
         icon: Optional[Union[bytes, bytearray, memoryview, Path, str]] = PYTHON_ICON,
-    ) -> AssetCustomSource:
+    ) -> CustomIntegration:
         """
-        Creates a new custom asset source.
+        Creates a new custom integration.
 
-        :param name: Name of custom source to be created in to your account. The
+        :param name: Name of custom integration to be created in to your account. The
             name may not contain spaces, tabs, or other whitespace
-        :param description: Optional description of custom source to be created
+        :param description: Optional description of custom integration to be created
         :param icon: Optional file path to, or bytes of icon data. The icon must be
             a png formatted image with a maximum size of 32x32. Icon format
             is validated by the server. The default value assigns your custom
             data source the Python logo to indicate it was created by this SDK.
-            Use None to have the server choose the default Custom Source logo,
+            Use None to have the server choose the default custom integration logo,
             a grey runZero logo
 
-        :return AssetCustomSource created
+        :return CustomIntegration created
         :raises AuthError, ClientError, ServerError
         """
 
         if isinstance(icon, (Path, str)):
             try:
                 icon = pathlib.Path(icon).resolve()
                 with icon.open("rb") as iconf:
                     icon = iconf.read()
             except (IOError, OSError) as exc:
                 raise Error from exc
         if isinstance(icon, (bytes, bytearray, memoryview)):
             icon = base64.b64encode(icon).decode("utf-8")
-        req = NewAssetCustomSource(name=name, description=description, icon=icon)
+        req = NewCustomIntegration(name=name, description=description, icon=icon)
         res = self._client.execute("POST", self._ENDPOINT, data=req)
         return _resp_to_source(res.json_obj)
 
-    def update(self, source_id: uuid.UUID, source_options: BaseAssetCustomSource) -> AssetCustomSource:
+    def update(self, custom_integration_id: uuid.UUID, source_options: BaseCustomIntegration) -> CustomIntegration:
         """
-        Updates a custom asset source associated with your account.
+        Updates a custom integration associated with your account.
 
-        :param source_id: Custom asset source with updated values
-        :param source_options: Custom asset source request values to update
-        :return AssetCustomSource updated
+        :param custom_integration_id: custom integration with updated values
+        :param source_options: custom integration request values to update
+        :return CustomIntegration updated
         :raises AuthError, ClientError, ServerError
         """
-        res = self._client.execute("PATCH", f"{self._ENDPOINT}/{str(source_id)}", data=source_options)
+        res = self._client.execute("PATCH", f"{self._ENDPOINT}/{str(custom_integration_id)}", data=source_options)
         return _resp_to_source(res.json_obj)
 
-    def delete(self, source_id: uuid.UUID) -> AssetCustomSource:
+    def delete(self, custom_integration_id: uuid.UUID) -> CustomIntegration:
         """
-        Deletes a custom asset source from your account.
+        Deletes a custom integration from your account.
 
-        :param source_id: Custom asset source id to delete
+        :param custom_integration_id: custom integration id to delete
         :raises AuthError, ClientError, ServerError
         """
-        res = self._client.execute("DELETE", f"{self._ENDPOINT}/{source_id}")
+        res = self._client.execute("DELETE", f"{self._ENDPOINT}/{custom_integration_id}")
         return _resp_to_source(res.json_obj)
 
 
-def _resp_to_source(json_obj: Any) -> AssetCustomSource:
-    source = AssetCustomSource.parse_obj(json_obj)
+def _resp_to_source(json_obj: Any) -> CustomIntegration:
+    source = CustomIntegration.parse_obj(json_obj)
     if source.icon is not None:
         source.icon = base64.b64decode(source.icon)
     return source
```

### Comparing `runzero_sdk-0.1.1/runzero/api/admin/orgs.py` & `runzero_sdk-0.2.0/runzero/api/admin/orgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Management of asset custom data sources.
+Management of asset custom integrations.
 """
 import uuid
 from typing import List, Optional
 
 from runzero.client import Client
 from runzero.types import Organization, OrgOptions
```

### Comparing `runzero_sdk-0.1.1/runzero/api/imports/assets.py` & `runzero_sdk-0.2.0/runzero/api/imports/assets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """
-enables management of runZero asset data sources.
+enables management of runZero custom integrations.
 
 These operations are privileged and require an account token directly or an OAuth key that can generate one.
 """
 import gzip
 import tempfile
 import time
 import uuid
-from typing import IO, Iterable, List, Optional
+from typing import Iterable, List, Optional
 
 from runzero.client import Client
 from runzero.types import ImportAsset, ImportTask, NewAssetImport, Task
 
 
 class CustomAssets:
     """Management of Custom Asset Data for your own custom integrations.
 
-    Custom data sources are descriptive registered associations between sources of data
-    and assets imported which are associated with those sources.
+    Custom data integrations are descriptive registered associations between integrations of data
+    and assets imported which are associated with those integrations.
 
     The data sent to the server has basic checks performed and is loaded as an import task
     when it can find the next available worker to do so. Therefore, the result
     is a `class:runzero.Task` which you can check the status of.
 
-    See related :class:`runzero.account.CustomSources` to work with the custom asset data
-    sources registered to the account.
+    See related :class:`runzero.account.CustomIntegrations` to work with the custom asset data
+    integrations registered to the account.
 
     :param client: A handle to the :class:`runzero.Client` which manages interactions
         with the runZero server.
     """
 
     _ENDPOINT = "api/v1.0/import/org/{oid}/assets"
 
@@ -36,24 +36,24 @@
         """Constructor method"""
         self._client = client
 
     def upload_assets(
         self,
         org_id: uuid.UUID,
         site_id: uuid.UUID,
-        source_id: uuid.UUID,
+        custom_integration_id: uuid.UUID,
         assets: List[ImportAsset],
         task_info: Optional[ImportTask] = None,
     ) -> Task:
         """
         Upload your custom assets to the runZero platform.
 
         :param org_id: Organization ID to import these assets into
         :param site_id: ID of the Site to import these asstes into
-        :param source_id: Custom asset source id for the provided Import Assets
+        :param custom_integration_id: custom integration id for the provided Import Assets
         :param assets: A collection of ImportAssets to upload
         :param task_info: Descriptive information associated with the import
             task to be created. If omitted, a task name is generated for you
 
         :return Task: The runZero task associated with processing the asset upload
         :raises ServerError, ClientError, AuthError
         """
@@ -65,48 +65,48 @@
             if task_info.name == "":
                 task_info.name = f"Custom Asset Import {time.time_ns():.0f}"
             if task_info.description is None or task_info.description == "":
                 task_info.description = "py-sdk import"
 
         asset_import_req = _create_custom_asset_request(
             site_id=site_id,
-            source_id=source_id,
+            custom_integration_id=custom_integration_id,
             import_task=task_info,
             assets=assets,
         )
 
         tags_as_str = ""
         if asset_import_req.import_task.tags is not None:
             tags_as_str = ",".join([tag.__root__ for tag in asset_import_req.import_task.tags])
         multipart_form_data = (
             ("assetData", ("asset_data.jsonl.gz", asset_import_req.asset_data)),
             ("siteId", (None, str(asset_import_req.site_id))),
-            ("sourceId", (None, str(asset_import_req.source_id))),
+            ("customIntegrationId", (None, str(asset_import_req.custom_integration_id))),
             ("importTask.name", (None, asset_import_req.import_task.name)),
             ("importTask.description", (None, asset_import_req.import_task.description)),
             ("importTask.tags", (None, tags_as_str)),
         )
         res = self._client.execute("POST", self._ENDPOINT.format(oid=org_id), files=multipart_form_data, multipart=True)
         return Task.parse_obj(res.json_obj)
 
 
-def _import_assets_into_gzip_jsonl(import_assets: Iterable[ImportAsset]) -> IO[bytes]:
+def _import_assets_into_gzip_jsonl(import_assets: Iterable[ImportAsset]) -> bytes:
     tmp = tempfile.TemporaryFile(mode="w+b")
     with gzip.GzipFile(fileobj=tmp, mode="wb") as gzw:
         for asset_obj in import_assets:
             gzw.write(asset_obj.json(by_alias=True).encode("utf-8") + "\n".encode("utf-8"))
     tmp.seek(0)
-    return tmp
+    return tmp.read()
 
 
 def _create_custom_asset_request(
-    site_id: uuid.UUID, source_id: uuid.UUID, assets: Iterable[ImportAsset], import_task: ImportTask
+    site_id: uuid.UUID, custom_integration_id: uuid.UUID, assets: Iterable[ImportAsset], import_task: ImportTask
 ) -> NewAssetImport:
     # TODO: We are disabling validation on all fields with .construct
     # until openapi 'bytes' type and pydantic can agree on a file-like.
     # See FastAPI implementation of UploadFile for ref
-    return NewAssetImport.construct(
+    return NewAssetImport(
         siteId=site_id,
-        sourceId=source_id,
+        customIntegrationId=custom_integration_id,
         importTask=import_task,
-        assetData=_import_assets_into_gzip_jsonl(assets),  # type: ignore
+        assetData=_import_assets_into_gzip_jsonl(assets),
     )
```

### Comparing `runzero_sdk-0.1.1/runzero/api/sites.py` & `runzero_sdk-0.2.0/runzero/api/sites.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.1.1/runzero/api/tasks.py` & `runzero_sdk-0.2.0/runzero/api/tasks.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.1.1/runzero/client/_http/auth.py` & `runzero_sdk-0.2.0/runzero/client/_http/auth.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.1.1/runzero/client/_http/io.py` & `runzero_sdk-0.2.0/runzero/client/_http/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 from runzero.client.errors import (
     AuthError,
     ClientError,
     CommunicationError,
     ConnError,
     ConnTimeoutError,
     ErrInfo,
+    RateLimitError,
     ServerError,
     UnknownAPIError,
     UnsupportedRequestError,
 )
+from runzero.types import RateLimitInformation
 
 ALLOWED_VERBS = frozenset(["GET", "POST", "PUT", "DELETE", "PATCH"])
 
 DEFAULT_CONTENT_HEADERS = {"content-type": "application/json"}
 
 if TYPE_CHECKING:
     from mypy_extensions import Arg, KwArg
@@ -40,14 +42,15 @@
 class Response:
     """The response from an HTTP request."""
 
     def __init__(self, response: RequestsResponse):
         """Constructor method"""
         self.status_code = response.status_code
         self.headers = response.headers
+        self.rate_limit_information = RateLimitInformation.from_headers(response.headers)
         try:
             self.json_obj = response.json()
         except JSONDecodeError:
             self.json_obj = None
 
 
 class Request:
@@ -205,28 +208,33 @@
     error_info = None
     try:
         content_type = response.headers.get("content-type", "")
         if not content_type:
             content_type = response.headers.get("Content-Type", "")
         if content_type.startswith("application/json") or content_type.startswith("application/problem+json"):
             body = response.json().copy()
-            # {"detail":"sourceId UUID cannot be all zeroes","error":"request failed","status":"error",
+            # {"detail":"customIntegrationId UUID cannot be all zeroes","error":"request failed","status":"error",
             # "title":"request failed"}
             try:
                 error_info = ErrInfo(
                     detail=body.pop("detail"),
                     status=response.status_code,
                     title=body.pop("title"),
                 )
             except KeyError:
                 pass
     except (KeyError, JSONDecodeError) as exc:
         raise UnknownAPIError(str(response), response.reason) from exc
 
     if 400 <= response.status_code <= 499:
+        if response.status_code == 429:
+            rate_limit = RateLimitInformation.from_headers(response.headers)
+            remaining = rate_limit.usage_remaining
+            if isinstance(remaining, int) and remaining < 1:
+                raise RateLimitError(rate_limit_information=rate_limit)
         raise ClientError(
             unparsed_response=str(response),
             message=f"The request was rejected by the server: {error_message}",
             error_info=error_info,
         )
 
     if 500 <= response.status_code <= 599:
```

### Comparing `runzero_sdk-0.1.1/runzero/client/client.py` & `runzero_sdk-0.2.0/runzero/client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 """
 client provides the runZero platform Client which must be provided to all objects which interact
 with the runZero API.
 """
+
+from __future__ import annotations
+
 from enum import Enum
 from typing import Any, Optional
 from urllib.parse import urlparse
 
 import requests
 from pydantic import BaseModel
 from requests.exceptions import ConnectionError as RequestsConnectionError
 from requests.exceptions import ConnectTimeout as RequestsConnectTimeout
 from requests.exceptions import ContentDecodingError
 from requests.exceptions import HTTPError as RequestsHTTPError
 
+from runzero.types import RateLimitInformation
+
 from ._http.auth import OAuthToken, RegisteredAPIClient
 from ._http.io import Request, Response
 from .errors import AuthError
 
 
 class Client:
     """
@@ -41,15 +46,15 @@
         preferred.
 
     :param server_url: Optional URL to the server hosting the API. Self-hosted API
         server targets must provide the server url in string form,
         e.g. 'https://runzero.local:8443'
         If not provided, the default hosted infrastructure URL
         'https://console.runzero.com' is used.
-    :type validate_certificate: bool
+    :type server_url: str
 
     :param validate_certificate: Optional bool to change whether Client checks
         the validity of the API server's certificate before proceeding. We recommend
         not setting this to false unless you are doing local development or testing.
         Ignoring certificate validation errors can result in credential theft or other
         bad outcomes.
     :type validate_certificate: bool
@@ -94,14 +99,15 @@
         if timeout_seconds is not None and timeout_seconds <= 0:
             raise ValueError("Timeout must be greater than 0")
         self._timeout = timeout_seconds or self.__default_timeout__
         if validate_certificate is None:
             self._validate_cert = True
         else:
             self._validate_cert = validate_certificate
+        self._rate_limit_information: Optional[RateLimitInformation] = None
 
     @property
     def oauth_token_is_expired(self) -> bool:
         """Returns true if the oauth token is no longer valid.
 
         Note that the token is automatically refreshed for you when
         possible. This value doesn't need to be checked and manually
@@ -219,14 +225,22 @@
         if scope is self._AuthScope.ORG:
             if self.__org_key is None:
                 if self.__account_key is None:
                     raise AuthError("missing organization or account key")
             return
 
     @property
+    def last_rate_limit_information(self) -> Optional[RateLimitInformation]:
+        """
+        The last rate limit information retrieved from the server.
+        :return: Optional[RateLimitInformation]
+        """
+        return self._rate_limit_information
+
+    @property
     def timeout(self) -> int:
         """
         The set request timeout value in seconds
         :return: int
         """
         return self._timeout
 
@@ -277,10 +291,11 @@
             params=params,
             timeout=self.timeout,
             validate_certificate=self.validate_cert,
             data=form_data,
             files=files,
             multipart=multipart,
         ).execute()
+        self._rate_limit_information = resp.rate_limit_information
         # If the result doesn't have JSON decoded, it's not a valid result.
         # TODO: Decide if absolutely anything else else should be a raised error here
         return resp
```

### Comparing `runzero_sdk-0.1.1/runzero/client/errors.py` & `runzero_sdk-0.2.0/runzero/client/errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """all client errors listed here"""
 
 from __future__ import annotations
 
 from typing import Optional
 
 from runzero.errors import APIError, Error
+from runzero.types import RateLimitInformation
 from runzero.types.errors import RFC7807Error
 
 
 class UnsupportedRequestError(ValueError, Error):
     """
     UnsupportedRequestError is a named Exception class representing any Error from the runZero API
     which cannot be properly interpreted into a friendlier form.
@@ -98,14 +99,55 @@
     * Misconfigured credentials
     * Missing credentials
     """
 
     pass
 
 
+class RateLimitError(APIError):
+    """
+    RateLimitError is a named Exception class errors resulting from API rate limiting.
+
+    See https://www.runzero.com/docs/leveraging-the-api/#api-client-credentials for details.
+
+    Consider an exponential backoff retry, or a more calculated approach by examining the returned
+    numbers.
+
+    :param message: A top-level error description. The default value None provides a reasonable
+        message.
+
+    :param unparsed_response: optional string which holds the unparsed response body.
+    :type unparsed_response: str, optional
+
+    :param rate_limit_information: a RateLimitInformation object which holds the rate limit data
+    :type rate_limit_information: RateLimitInformation
+
+    """
+
+    def __init__(
+        self,
+        rate_limit_information: RateLimitInformation,
+        message: Optional[str] = None,
+        unparsed_response: Optional[str] = None,
+    ):
+        """Constructor method"""
+        if not message:
+            message = (
+                "Too many API requests for licensed rate limit. See runZero documentation for details on API "
+                "rate limiting."
+            )
+        super().__init__(message)
+        self.message = message
+        self.unparsed_response: Optional[str] = unparsed_response
+        self.rate_limit_information: RateLimitInformation = rate_limit_information
+
+    def __str__(self) -> str:
+        return f"{self.message} Rate limit information: {self.rate_limit_information}"
+
+
 class UnknownAPIError(APIError):
     """
     UnknownAPIError is a named Exception class raised when the response indicates a structured
     error message that cannot be parsed.
 
     Effort is made to receive and interpret errors returned from runZero services. These
     errors should be rare to non-existent.
```

### Comparing `runzero_sdk-0.1.1/runzero/errors.py` & `runzero_sdk-0.2.0/runzero/errors.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.1.1/runzero/types/__init__.py` & `runzero_sdk-0.2.0/runzero/types/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 """
-types provides the Pydantic data model representations of the runZero Platform API schema.
+types provides the Pydantic data model representations of the runZero Platform
+API schema, as well as other data types which wrap looser runZero API data.
 
-Public runZero API types contained inside this package are made available here. Not all
-objects in the private module, which is generated from OpenAPI specs, are usable in this
-project today.
+Public, SDK-supported runZero API types contained inside this package are made
+available here. Not all objects in the private module, which is generated from
+OpenAPI specs, are usable in this project today.
 """
 from ipaddress import IPv4Address, IPv6Address
 
 from runzero.types._data_models_gen import (
-    BaseAssetCustomSource,
+    BaseCustomIntegration,
     ImportAsset,
     ImportTask,
     NetworkInterface,
-    NewAssetCustomSource,
     NewAssetImport,
+    NewCustomIntegration,
     Organization,
     OrgOptions,
     Problem,
     Site,
     SiteOptions,
     Task,
 )
-from runzero.types._wrapped import AssetCustomSource, CustomAttribute, Hostname, Tag
+from runzero.types._rate_limit_information import RateLimitInformation
+from runzero.types._wrapped import CustomAttribute, CustomIntegration, Hostname, Tag
 from runzero.types.errors import ValidationError
 
 __all__ = [
-    "AssetCustomSource",
-    "BaseAssetCustomSource",
+    "CustomIntegration",
+    "BaseCustomIntegration",
     "CustomAttribute",
     "Hostname",
     "IPv4Address",
     "IPv6Address",
     "ImportAsset",
     "ImportTask",
     "NetworkInterface",
-    "NewAssetCustomSource",
+    "NewCustomIntegration",
     "NewAssetImport",
     "Organization",
     "OrgOptions",
     "Problem",
+    "RateLimitInformation",
     "Site",
     "SiteOptions",
     "Tag",
     "Task",
     "ValidationError",
 ]
```

### Comparing `runzero_sdk-0.1.1/runzero/types/_data_models_gen.py` & `runzero_sdk-0.2.0/runzero/types/_data_models_gen.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  proposed-runzero-api.yml
-#   timestamp: 2023-03-23T01:31:43+00:00
+#   timestamp: 2023-04-08T05:51:55+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from ipaddress import IPv4Address, IPv6Address
 from typing import Any, Dict, List, Optional
 from uuid import UUID
@@ -19,15 +19,15 @@
 
     id: UUID = Field(..., example="f6cfb91a-52ea-4a86-bf9a-5a891a26f52b")
     """
     The unique ID of the object
     """
     client_id: UUID = Field(..., alias="clientId", example="e77602e0-3fb8-4734-aef9-fbc6fdcb0fa8")
     """
-    The unique ID of the runZero client/customer account that created the custom source
+    The unique ID of the runZero client/customer account that created the custom integration
     """
     created_by_id: UUID = Field(..., alias="createdById", example="f6cfb91a-52ea-4a86-bf9a-5a891a26f52b")
     """
     The unique ID of the entity that created the object
     """
     created_at: datetime = Field(..., alias="createdAt", example="2023-03-06T18:14:50.52Z")
     """
@@ -39,66 +39,66 @@
     """
     destroyed_at: Optional[datetime] = Field(None, alias="destroyedAt", example="2023-03-06T18:14:50.52Z")
     """
     A timestamp indicating deletion time of the object
     """
 
 
-class BaseAssetCustomSource(BaseModel):
-    name: Optional[str] = Field(None, example="Custom Source One", regex="^\\S+$")
+class BaseCustomIntegration(BaseModel):
+    name: Optional[str] = Field(None, example="my-custom-integration", regex="^\\S+$")
     """
-    The unique name of the custom source, without spaces.
+    The unique name of the custom integration, without spaces.
     """
     icon: Optional[str] = Field(
         None,
         example="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",
     )
     """
-    Base64 encoded png with maximum size 32x32 pixels
+    Base64 encoded png with maximum size 256x256 pixels
     """
-    description: Optional[str] = Field(None, example="My custom source description.")
+    description: Optional[str] = Field(None, example="My custom integration description.")
     """
-    A text description of the custom source
+    A text description of the custom integration
     """
 
 
-class AssetCustomSource(BaseAssetCustomSource, BaseResponse):
-    name: str = Field(..., example="Custom Source One", regex="^\\S+$")
+class CustomIntegration(BaseCustomIntegration, BaseResponse):
+    name: str = Field(..., example="my-custom-integration", regex="^\\S+$")
     """
-    The unique name of the custom source, without spaces.
+    The unique name of the custom integration, without spaces.
     """
 
 
-class NewAssetCustomSource(BaseAssetCustomSource):
-    name: str = Field(..., example="Custom Source One", regex="^\\S+$")
+class NewCustomIntegration(BaseCustomIntegration):
+    name: str = Field(..., example="my-custom-integration", regex="^\\S+$")
     """
-    The unique name of the custom source, without spaces.
+    The unique name of the custom integration, without spaces.
     """
 
 
 class Tag(BaseModel):
     __root__: str = Field(..., max_length=1024)
 
 
 class ImportTask(BaseModel):
     """
     Information which describes the task created when asset data is imported.
     """
 
     name: str = Field(..., example="my import task", max_length=100)
-    description: Optional[str] = Field(None, example="importing assets from source A", max_length=1024)
+    description: Optional[str] = Field(None, example="importing assets from custom integration A", max_length=1024)
     tags: Optional[List[Tag]] = Field(None, example=["tag1", "tag2"], max_items=100)
     """
     Arbitrary string tag values which are applied to the asset data import task created.
     """
 
 
 class NewAssetImport(BaseModel):
     """
-    Represents a request to import asset data described by the specified source into the specified site.
+    Represents a request to import asset data described by the specified custom integration into the specified site.
 
     Assets will be created new or merged according to merge rules defined by the version of the platform
     you are uploading the asset data file to. Typically, this involves matching network and other unique
     single or grouped properties.
 
     There is a maximum of 256 custom asset properties that can be applied to any asset. This means
     that, aside from the per-import asset property limit set on ImportAsset, if a new import sets
@@ -107,17 +107,19 @@
 
     """
 
     site_id: UUID = Field(..., alias="siteId", example="e77602e0-3fb8-4734-aef9-fbc6fdcb0fa8")
     """
     The ID of the site assets are to be imported into.
     """
-    source_id: UUID = Field(..., alias="sourceId", example="e77602e0-3fb8-4734-aef9-fbc6fdcb0fa8")
+    custom_integration_id: UUID = Field(
+        ..., alias="customIntegrationId", example="e77602e0-3fb8-4734-aef9-fbc6fdcb0fa8"
+    )
     """
-    The unique ID of the registered custom source which produced the asset data. See /account/sources api.
+    The unique ID of the registered custom integration which produced the asset data. See /account/custom-integrations api.
     """
     import_task: ImportTask = Field(..., alias="importTask", title="ImportTask")
     """
     Information which describes the task created when asset data is imported.
     """
     asset_data: bytes = Field(..., alias="assetData")
     """
@@ -134,18 +136,33 @@
     Represents IPV4 addresses. Addresses are ordered from most to least likely to uniquely identify the asset.
     """
     ipv6_addresses: Optional[List[IPv6Address]] = Field(None, alias="ipv6Addresses", max_items=100)
     """
     Represents the IPV6 addresses. Addresses are ordered from most to least likely to uniquely identify the asset.
     """
     mac_address: Optional[str] = Field(
-        None, alias="macAddress", example="01:23:45:67:89:0A", max_length=17, regex="^([A-F0-9]{2}:){5}[A-F0-9]{2}$"
+        None,
+        alias="macAddress",
+        example="01:23:45:67:89:0A",
+        max_length=23,
+        regex=(
+            "^([A-Fa-f0-9]{2}:){5}[A-Fa-f0-9]{2}$|^([A-Fa-f0-9]{2}:){7}[A-Fa-f0-9]{2}$|^([A-Fa-f0-9]{2}-){5}[A-Fa-f0-9]{2}$|^([A-Fa-f0-9]{2}-){7}[A-Fa-f0-9]{2}$|^([A-Fa-f0-9]{4}\\.){2}[A-Fa-f0-9]{4}$|^([A-Fa-f0-9]{4}\\.){3}[A-Fa-f0-9]{4}$|^([A-Fa-f0-9]{4}"
+            " ){3}[A-Fa-f0-9]{4}$"
+        ),
     )
     """
-    Represents a MAC address using colons as hexadecimal octet delimiters.
+    Represents a MAC address in IEEE 802 MAC/EUI-48, or EUI-64 form in one of the following formats:
+      01:23:45:67:89:AB
+      01:23:45:67:89:ab:cd:ef
+      01-23-45-67-89-ab
+      01-23-45-67-89-ab-cd-ef
+      0123.4567.89ab
+      0123.4567.89ab.cdef
+      0123 4567 89ab cdEF
+
     """
 
 
 class Hostname(BaseModel):
     __root__: str = Field(..., example="host.domain.com", max_length=260)
 
 
@@ -156,15 +173,19 @@
 class ImportAsset(BaseModel):
     """
     Represents a custom asset to be created or merged after import.
     """
 
     id: str = Field(..., max_length=1024)
     """
-    Any value which can uniquely identify the asset within the custom source.
+    Any value which can uniquely identify the asset within the custom integration.
+    """
+    run_zero_id: Optional[UUID] = Field(None, alias="runZeroID", example="e77602e0-3fb8-4734-aef9-fbc6fdcb0fa8")
+    """
+    The unique identifier of the runZero asset to merge into.
     """
     network_interfaces: Optional[List[NetworkInterface]] = Field(
         None, alias="networkInterfaces", max_items=256, title="NetworkInterfaces"
     )
     """
     The asset's networking configuration.
     """
@@ -174,19 +195,15 @@
     """
     domain: Optional[str] = Field(None, example="domain.com", max_length=260)
     """
     Represents a single domain name which could be applied to all non-fqdns in the hostnames field.
     """
     first_seen_ts: Optional[datetime] = Field(None, alias="firstSeenTS", example="2023-03-06T18:14:50.52Z")
     """
-    Represents the earliest time the asset was seen by the source reporting it, using a date string as defined by RFC 3339, section 5.6.
-    """
-    last_seen_ts: Optional[datetime] = Field(None, alias="lastSeenTS", example="2023-03-06T18:14:50.52Z")
-    """
-    Represents the most recent time the asset was seen by the source reporting it, using a date string as defined by RFC 3339, section 5.6.
+    Represents the earliest time the asset was seen by the custom integration reporting it, using a date string as defined by RFC 3339, section 5.6.
     """
     os: Optional[str] = Field(None, example="Ubuntu Linux 22.04", max_length=1024)
     """
     The name of the asset's operating system. It is advisable to keep the data clean by normalizing to existing values when possible.
     """
     os_version: Optional[str] = Field(None, alias="osVersion", example="22.04", max_length=1024)
     """
```

### Comparing `runzero_sdk-0.1.1/runzero/types/_wrapped.py` & `runzero_sdk-0.2.0/runzero/types/_wrapped.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 was insufficient.
 """
 
 from typing import Optional
 
 from pydantic import Field
 
-from ._data_models_gen import AssetCustomSource as RESTAssetCustomSource
 from ._data_models_gen import CustomAttribute as RESTCustomAttribute
+from ._data_models_gen import CustomIntegration as RESTCustomIntegration
 from ._data_models_gen import Hostname as RESTHostname
 from ._data_models_gen import Tag as RESTTag
 
 
-class AssetCustomSource(RESTAssetCustomSource):
-    """AssetCustomSource represents a custom asset data source for custom integrations use"""
+class CustomIntegration(RESTCustomIntegration):
+    """CustomIntegration represents a custom asset data source for custom integrations use"""
 
     # The REST API uses base-64 encoded strings, but inside this SDK
     # we want always use bytes and hide the transport encoding.
     # Note that it's unsafe to override types in a subclass
     # according to mypy - it would be better to compose than
     # inherit. But we are wrapping our own API :)
```

### Comparing `runzero_sdk-0.1.1/runzero/types/errors.py` & `runzero_sdk-0.2.0/runzero/types/errors.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.1.1/PKG-INFO` & `runzero_sdk-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runzero-sdk
-Version: 0.1.1
+Version: 0.2.0
 Summary: The runZero platform sdk
 Home-page: https://runzero.com/
 License: BSD-2-Clause
 Keywords: runzero,api,sdk
 Author: runZero
 Author-email: support@runzero.com
 Requires-Python: >=3.8,<4.0
@@ -80,30 +80,31 @@
 
 ## Modules
 
 The runzero-sdk package contains the following modules to group functionality.
 
 ### runzero.api
 
-The `api` module contains all the http handlers for interacting with runZero api resources such as Sites, Orgs, Tasks, Custom Sources, etc.
+The `api` module contains all the http handlers for interacting with runZero api resources such as Sites, Orgs, Tasks, Custom Integrations, etc.
 
 ### runzero.types
 
 The `types` module contains all the pydantic classes required for interacting with the runZero API resources such as Import Assets, Sites, Tasks, etc.
 
 ## Custom Import Asset field mappings
 
-The following fields are available to be set for custom source asset imports. Any field which matches the below field
+The following fields are available to be set for custom integration asset imports. Any field which matches the below field
 names, either directly or via remapping, will be inserted into the corresponding `ImportAsset` field and validated to
 ensure it meets the outlined constraints.
 
 Any field which does not match the fields below will be placed under the `custom_attributes` field. Please see the
 `ImportAsset` schema definition for more details: #/components/schemas/ImportAsset
 
-* `id` - this `str` field is ***required*** to be set for all custom source assets and is the unique identifier for the asset. If your asset does not have a unique id then we recommend you create one using `uuid.uuid4()`.
+* `id` - this `str` field is ***required*** to be set for all custom integration assets and is the unique identifier for the asset. If your asset does not have a unique id then we recommend you create one using `uuid.uuid4()`.
+* `runZeroID` - a `uuid` field representing the unique identifier of an existing runZero asset to merge into.
 * `network_interfaces` - this field is an array of objects representing the network interfaces of the asset. Please see the API Schema for details. #/components/schemas/ImportAsset/properties/networkInterfaces.
 * `hostnames` - a `List[str]` field of all the hostnames associated with the asset. Each hostname has a maximum length of 260 characters and the `list` has a maximum of 100 hostnames.
 * `domain` - a `str` field representing the domain associated with the asset. Maximum length of 260 characters.
 * `first_seen_ts` - a `datetime.datetime` field representing the first time an asset was seen.
 * `last_seen_ts` - a `datetime.datetime` field representing the last time an asset was seen.
 * `os` - a `str` field which describes the operating system on the asset. Maximum length of 1024 characters.
 * `os_version` - a `str` field which describes the version of the operating system running on the asset. Maximum length of 1024 characters.
```

