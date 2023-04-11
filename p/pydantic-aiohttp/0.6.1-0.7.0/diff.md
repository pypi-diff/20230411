# Comparing `tmp/pydantic_aiohttp-0.6.1.tar.gz` & `tmp/pydantic_aiohttp-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_aiohttp-0.6.1.tar", max compression
+gzip compressed data, was "pydantic_aiohttp-0.7.0.tar", max compression
```

## Comparing `pydantic_aiohttp-0.6.1.tar` & `pydantic_aiohttp-0.7.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1315 2023-03-02 12:13:38.096454 pydantic_aiohttp-0.6.1/CHANGELOG.md
--rw-r--r--   0        0        0     1064 2023-03-02 12:13:38.096454 pydantic_aiohttp-0.6.1/LICENSE
--rw-r--r--   0        0        0     4527 2023-03-02 12:13:38.096454 pydantic_aiohttp-0.6.1/README.md
--rw-r--r--   0        0        0       72 2023-03-02 12:13:38.100454 pydantic_aiohttp-0.6.1/pydantic_aiohttp/__init__.py
--rw-r--r--   0        0        0    11741 2023-03-02 12:13:38.100454 pydantic_aiohttp-0.6.1/pydantic_aiohttp/client.py
--rw-r--r--   0        0        0     6184 2023-03-02 12:13:38.100454 pydantic_aiohttp-0.6.1/pydantic_aiohttp/encoders.py
--rw-r--r--   0        0        0     8394 2023-03-02 12:13:38.100454 pydantic_aiohttp-0.6.1/pydantic_aiohttp/errors.py
--rw-r--r--   0        0        0     2391 2023-03-02 12:13:38.100454 pydantic_aiohttp-0.6.1/pydantic_aiohttp/responses.py
--rw-r--r--   0        0        0      904 2023-03-02 12:13:38.100454 pydantic_aiohttp-0.6.1/pydantic_aiohttp/utils.py
--rw-r--r--   0        0        0      967 2023-03-02 12:13:38.100454 pydantic_aiohttp-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5526 1970-01-01 00:00:00.000000 pydantic_aiohttp-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1865 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1064 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4527 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/README.md
+-rw-r--r--   0        0        0      136 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pydantic_aiohttp/__init__.py
+-rw-r--r--   0        0        0    11310 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pydantic_aiohttp/client.py
+-rw-r--r--   0        0        0    11770 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pydantic_aiohttp/encoders.py
+-rw-r--r--   0        0        0     8394 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pydantic_aiohttp/errors.py
+-rw-r--r--   0        0        0     2375 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pydantic_aiohttp/responses.py
+-rw-r--r--   0        0        0      506 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pydantic_aiohttp/types.py
+-rw-r--r--   0        0        0     1664 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pydantic_aiohttp/utils.py
+-rw-r--r--   0        0        0      967 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5526 1970-01-01 00:00:00.000000 pydantic_aiohttp-0.7.0/PKG-INFO
```

### Comparing `pydantic_aiohttp-0.6.1/CHANGELOG.md` & `pydantic_aiohttp-0.7.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,31 @@
 # CHANGELOG
 
+## 0.7.0
+
+### **BREAKING**
+
+* All types moved from `client` to separate `types` module
+
+* Removed unused `error_response_class` from `Client` constructur parameters
+
+___
+
+* Added custom `url_compatible_encoder` for params, cookies and headers because Aiohttp expects their values to be `int`, `float` or `str` instances
+
+## 0.6.2
+
+* `model_to_dict` now accepts all `pydantic.BaseModel.dict` parameters
+
+* `utils` module added to package export
+
+* `encoders` module added to package export
+
+* All absolute package path exports replaced with relative
+
 ## 0.6.1
 
 * Upgraded dependencies
 
 ## 0.6.0
 
 * Using custom json requests serializer for better pydantic model serialization
```

### Comparing `pydantic_aiohttp-0.6.1/LICENSE` & `pydantic_aiohttp-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_aiohttp-0.6.1/README.md` & `pydantic_aiohttp-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_aiohttp-0.6.1/pydantic_aiohttp/client.py` & `pydantic_aiohttp-0.7.0/pydantic_aiohttp/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,90 +1,85 @@
 import logging
 from typing import (
     Any,
     Optional,
     Type,
-    TypeVar,
     Union,
 )
 
 import aiohttp
 import pydantic
 import ujson
 from aiohttp.typedefs import PathLike
 from ujson import JSONDecodeError
 
+from .encoders import url_compatible_encoder
 from .errors import (
     HTTPError,
     ResponseParseError,
     errors_classes,
 )
 from .responses import (
     PydanticModelResponseClass,
     ResponseClass,
     StreamResponseClass,
 )
+from .types import (
+    Body,
+    Cookies,
+    ErrorResponseModels,
+    Headers,
+    Params,
+    ResponseType,
+)
 from .utils import (
     DEFAULT_DOWNLOAD_CHUNK_SIZE,
     json_serialize,
     model_to_dict,
     read_file_by_chunk,
 )
 
-StrIntMapping = dict[str, Union[str, int]]
-HttpEncodableMapping = dict[str, Union[str, int, list[Union[str, int]]]]
-Params = Union[HttpEncodableMapping, pydantic.BaseModel]
-Cookies = Union[StrIntMapping, pydantic.BaseModel]
-Headers = Union[StrIntMapping, pydantic.BaseModel]
-Body = Union[dict[str, Any], pydantic.BaseModel]
-ErrorResponseModels = dict[int, Type[pydantic.BaseModel]]
-
-ResponseType = TypeVar('ResponseType')
-
 
 class Client:
     def __init__(
             self,
             base_url: str = None,
             *,
             headers: Headers = None,
             cookies: Cookies = None,
             params: Params = None,
             error_response_models: ErrorResponseModels = None,
             bearer_token: Union[str, pydantic.SecretStr] = None,
             response_class: Type[ResponseClass] = PydanticModelResponseClass,
-            error_response_class: Type[ResponseClass] = PydanticModelResponseClass,
     ):
         self.logger = logging.getLogger("pydantic_aiohttp.Client")
         headers = model_to_dict(headers) or {}
         cookies = model_to_dict(cookies) or {}
         params = model_to_dict(params) or {}
 
         if bearer_token is not None:
             if isinstance(bearer_token, pydantic.SecretStr):
                 bearer_token = bearer_token.get_secret_value()
 
             headers["Authorization"] = f"Bearer {bearer_token}"
 
         self._error_response_models = error_response_models or {}
         self._response_class = response_class
-        self._error_response_class = error_response_class
         self._params = params
         self._session = aiohttp.ClientSession(
             base_url,
             headers=headers,
             cookies=cookies,
             json_serialize=json_serialize
         )
 
     async def _parse_response_error(
             self,
             response: aiohttp.ClientResponse,
             error_response_models: ErrorResponseModels = None,
-            error_response_class: Type[ResponseClass] = PydanticModelResponseClass,
     ):
         error_response_models = self._error_response_models | (error_response_models or {})
         error_class = errors_classes.get(response.status, HTTPError)
         error_response_model = error_response_models.get(response.status)
 
         try:
             response_json = await response.json(loads=ujson.loads, content_type=None)
@@ -196,17 +191,17 @@
 
         if bool(params):
             _params.update(model_to_dict(params) or {})
 
         async with self._session.request(
                 method,
                 path,
-                headers=model_to_dict(headers),
-                cookies=model_to_dict(cookies),
-                params=_params,
+                headers=url_compatible_encoder(model_to_dict(headers)),
+                cookies=url_compatible_encoder(model_to_dict(cookies)),
+                params=url_compatible_encoder(_params),
                 json=model_to_dict(body),
                 data=data,
                 timeout=aiohttp.ClientTimeout(total=timeout)
         ) as response:
             if response.ok:
                 return await response_class(response).parse(
                     response_model=response_model,
```

### Comparing `pydantic_aiohttp-0.6.1/pydantic_aiohttp/encoders.py` & `pydantic_aiohttp-0.7.0/pydantic_aiohttp/encoders.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,34 +13,36 @@
     Optional,
     Set,
     Tuple,
     Union,
 )
 
 from pydantic import BaseModel
+# noinspection PyProtectedMember
 from pydantic.json import ENCODERS_BY_TYPE
 
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
 def generate_encoders_by_class_tuples(
         type_encoder_map: Dict[Any, Callable[[Any], Any]]
 ) -> Dict[Callable[[Any], Any], Tuple[Any, ...]]:
-    encoders_by_class_tuples: Dict[Callable[[Any], Any], Tuple[Any, ...]] = defaultdict(
+    _encoders_by_class_tuples: Dict[Callable[[Any], Any], Tuple[Any, ...]] = defaultdict(
         tuple
     )
     for type_, encoder in type_encoder_map.items():
-        encoders_by_class_tuples[encoder] += (type_,)
-    return encoders_by_class_tuples
+        _encoders_by_class_tuples[encoder] += (type_,)
+    return _encoders_by_class_tuples
 
 
 encoders_by_class_tuples = generate_encoders_by_class_tuples(ENCODERS_BY_TYPE)
 
 
+# noinspection DuplicatedCode
 def jsonable_encoder(
         obj: Any,
         include: Optional[Union[SetIntStr, DictIntStrAny]] = None,
         exclude: Optional[Union[SetIntStr, DictIntStrAny]] = None,
         by_alias: bool = True,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
@@ -158,25 +160,181 @@
     for encoder, classes_tuple in encoders_by_class_tuples.items():
         if isinstance(obj, classes_tuple):
             return encoder(obj)
 
     try:
         data = dict(obj)
     except Exception as e:
-        errors: List[Exception] = []
-        errors.append(e)
+        errors: List[Exception] = [e]
         try:
             data = vars(obj)
         except Exception as e:
             errors.append(e)
             raise ValueError(errors) from e
     return jsonable_encoder(
         data,
         include=include,
         exclude=exclude,
         by_alias=by_alias,
         exclude_unset=exclude_unset,
         exclude_defaults=exclude_defaults,
         exclude_none=exclude_none,
+        custom_encoder=custom_encoder,
+        sqlalchemy_safe=sqlalchemy_safe,
+    )
+
+
+# noinspection DuplicatedCode
+def url_compatible_encoder(
+        obj: Any,
+        include: Optional[Union[SetIntStr, DictIntStrAny]] = None,
+        exclude: Optional[Union[SetIntStr, DictIntStrAny]] = None,
+        by_alias: bool = True,
+        exclude_unset: bool = True,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+        custom_encoder: Optional[Dict[Any, Callable[[Any], Any]]] = None,
+        sqlalchemy_safe: bool = True,
+) -> str | list[str] | dict[str, str | list[str]]:
+    custom_encoder = custom_encoder or {}
+    if custom_encoder:
+        if type(obj) in custom_encoder:
+            return custom_encoder[type(obj)](obj)
+        else:
+            for encoder_type, encoder_instance in custom_encoder.items():
+                if isinstance(obj, encoder_type):
+                    return encoder_instance(obj)
+    if include is not None and not isinstance(include, (set, dict)):
+        include = set(include)
+    if exclude is not None and not isinstance(exclude, (set, dict)):
+        exclude = set(exclude)
+    if isinstance(obj, BaseModel):
+        encoder = getattr(obj.__config__, "json_encoders", {})
+        if custom_encoder:
+            encoder.update(custom_encoder)
+        obj_dict = obj.dict(
+            include=include,
+            exclude=exclude,
+            by_alias=by_alias,
+            exclude_unset=exclude_unset,
+            exclude_none=exclude_none,
+            exclude_defaults=exclude_defaults,
+        )
+        if "__root__" in obj_dict:
+            obj_dict = obj_dict["__root__"]
+        return url_compatible_encoder(
+            obj_dict,
+            exclude_none=exclude_none,
+            exclude_defaults=exclude_defaults,
+            custom_encoder=encoder,
+            sqlalchemy_safe=sqlalchemy_safe,
+        )
+    if dataclasses.is_dataclass(obj):
+        obj_dict = dataclasses.asdict(obj)
+        return url_compatible_encoder(
+            obj_dict,
+            include=include,
+            exclude=exclude,
+            by_alias=by_alias,
+            exclude_unset=exclude_unset,
+            exclude_defaults=exclude_defaults,
+            exclude_none=exclude_none,
+            custom_encoder=custom_encoder,
+            sqlalchemy_safe=sqlalchemy_safe,
+        )
+    if isinstance(obj, Enum):
+        return obj.value
+    if isinstance(obj, PurePath):
+        return str(obj)
+    if isinstance(obj, type(None)):
+        return ""
+    if isinstance(obj, str):
+        return obj
+    if isinstance(obj, bool):
+        return str(obj).lower()
+    if isinstance(obj, (int, float)):
+        return str(obj)
+    if isinstance(obj, dict):
+        encoded_dict = {}
+        allowed_keys = set(obj.keys())
+        if include is not None:
+            allowed_keys &= set(include)
+        if exclude is not None:
+            allowed_keys -= set(exclude)
+        for key, value in obj.items():
+            if (
+                    (
+                            not sqlalchemy_safe
+                            or (not isinstance(key, str))
+                            or (not key.startswith("_sa"))
+                    )
+                    and (value is not None or not exclude_none)
+                    and key in allowed_keys
+            ):
+                encoded_key = url_compatible_encoder(
+                    key,
+                    by_alias=by_alias,
+                    exclude_unset=exclude_unset,
+                    exclude_none=exclude_none,
+                    custom_encoder=custom_encoder,
+                    sqlalchemy_safe=sqlalchemy_safe,
+                )
+                encoded_value = url_compatible_encoder(
+                    value,
+                    by_alias=by_alias,
+                    exclude_unset=exclude_unset,
+                    exclude_none=exclude_none,
+                    custom_encoder=custom_encoder,
+                    sqlalchemy_safe=sqlalchemy_safe,
+                )
+
+                if not bool(encoded_key):
+                    # '' or None
+                    continue
+
+                encoded_dict[encoded_key] = encoded_value
+        return encoded_dict
+    if isinstance(obj, (list, set, frozenset, GeneratorType, tuple)):
+        encoded_list = []
+        for item in obj:
+            encoded_list.append(
+                url_compatible_encoder(
+                    item,
+                    include=include,
+                    exclude=exclude,
+                    by_alias=by_alias,
+                    exclude_unset=exclude_unset,
+                    exclude_defaults=exclude_defaults,
+                    exclude_none=exclude_none,
+                    custom_encoder=custom_encoder,
+                    sqlalchemy_safe=sqlalchemy_safe,
+                )
+            )
+        return encoded_list
+
+    if type(obj) in ENCODERS_BY_TYPE:
+        return ENCODERS_BY_TYPE[type(obj)](obj)
+    for encoder, classes_tuple in encoders_by_class_tuples.items():
+        if isinstance(obj, classes_tuple):
+            return encoder(obj)
+
+    try:
+        data = dict(obj)
+    except Exception as e:
+        errors: List[Exception] = [e]
+        try:
+            data = vars(obj)
+        except Exception as e:
+            errors.append(e)
+            raise ValueError(errors) from e
+
+    return url_compatible_encoder(
+        data,
+        include=include,
+        exclude=exclude,
+        by_alias=by_alias,
+        exclude_unset=exclude_unset,
+        exclude_defaults=exclude_defaults,
+        exclude_none=exclude_none,
         custom_encoder=custom_encoder,
         sqlalchemy_safe=sqlalchemy_safe,
     )
```

### Comparing `pydantic_aiohttp-0.6.1/pydantic_aiohttp/errors.py` & `pydantic_aiohttp-0.7.0/pydantic_aiohttp/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic_aiohttp-0.6.1/pydantic_aiohttp/responses.py` & `pydantic_aiohttp-0.7.0/pydantic_aiohttp/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import aiofiles
 import aiohttp.web_response
 import pydantic
 import ujson
 from aiohttp.typedefs import PathLike
 
-from pydantic_aiohttp.utils import DEFAULT_DOWNLOAD_CHUNK_SIZE
+from .utils import DEFAULT_DOWNLOAD_CHUNK_SIZE
 
 ResponseContentType = TypeVar('ResponseContentType')
 PydanticModel = TypeVar('PydanticModel')
 
 
 class ResponseClass(abc.ABC, Generic[ResponseContentType]):
     charset: str = "utf-8"
```

### Comparing `pydantic_aiohttp-0.6.1/pyproject.toml` & `pydantic_aiohttp-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic_aiohttp"
-version = "0.6.1"
+version = "0.7.0"
 description = "Simple HTTP Client based on aiohttp with integration of pydantic"
 authors = ["pylakey <pylakey@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pylakey/pydantic_aiohttp"
 repository = "https://github.com/pylakey/pydantic_aiohttp"
 packages = [
```

### Comparing `pydantic_aiohttp-0.6.1/PKG-INFO` & `pydantic_aiohttp-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-aiohttp
-Version: 0.6.1
+Version: 0.7.0
 Summary: Simple HTTP Client based on aiohttp with integration of pydantic
 Home-page: https://github.com/pylakey/pydantic_aiohttp
 License: MIT
 Author: pylakey
 Author-email: pylakey@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Framework :: AsyncIO
```

