# Comparing `tmp/openapify-0.1.3.tar.gz` & `tmp/openapify-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapify-0.1.3.tar", last modified: Fri Apr  7 14:47:27 2023, max compression
+gzip compressed data, was "openapify-0.3.tar", last modified: Tue Apr 11 15:01:19 2023, max compression
```

## Comparing `openapify-0.1.3.tar` & `openapify-0.3.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 14:47:27.023633 openapify-0.1.3/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      732 2023-04-07 14:47:27.023498 openapify-0.1.3/PKG-INFO
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 14:47:27.019027 openapify-0.1.3/openapify/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      239 2023-04-07 14:25:34.000000 openapify-0.1.3/openapify/__init__.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 14:47:27.022041 openapify-0.1.3/openapify/core/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-03 13:14:57.000000 openapify-0.1.3/openapify/core/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1123 2023-04-07 11:40:06.000000 openapify-0.1.3/openapify/core/apispec.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    15544 2023-04-07 14:43:54.000000 openapify-0.1.3/openapify/core/builder.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       92 2023-03-20 20:50:13.000000 openapify-0.1.3/openapify/core/const.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      591 2023-04-03 13:10:22.000000 openapify-0.1.3/openapify/core/jsonschema.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1748 2023-04-07 11:38:54.000000 openapify-0.1.3/openapify/core/models.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 14:47:27.022457 openapify-0.1.3/openapify/core/openapi/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-03-20 12:12:59.000000 openapify-0.1.3/openapify/core/openapi/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5270 2023-04-07 14:46:46.000000 openapify-0.1.3/openapify/core/openapi/models.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4769 2023-04-07 11:42:13.000000 openapify-0.1.3/openapify/decorators.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 14:47:27.022698 openapify-0.1.3/openapify/ext/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-03-17 15:48:32.000000 openapify-0.1.3/openapify/ext/__init__.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 14:47:27.022883 openapify-0.1.3/openapify/ext/web/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-03-18 09:45:46.000000 openapify-0.1.3/openapify/ext/web/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4332 2023-04-03 13:47:08.000000 openapify-0.1.3/openapify/ext/web/aiohttp.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-03-17 11:19:37.000000 openapify-0.1.3/openapify/py.typed
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 14:47:27.020439 openapify-0.1.3/openapify.egg-info/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      732 2023-04-07 14:47:26.000000 openapify-0.1.3/openapify.egg-info/PKG-INFO
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      616 2023-04-07 14:47:26.000000 openapify-0.1.3/openapify.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-07 14:47:26.000000 openapify-0.1.3/openapify.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-07 10:28:17.000000 openapify-0.1.3/openapify.egg-info/not-zip-safe
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       42 2023-04-07 14:47:26.000000 openapify-0.1.3/openapify.egg-info/requires.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       10 2023-04-07 14:47:26.000000 openapify-0.1.3/openapify.egg-info/top_level.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      364 2023-04-07 11:44:47.000000 openapify-0.1.3/pyproject.toml
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       38 2023-04-07 14:47:27.023672 openapify-0.1.3/setup.cfg
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1099 2023-04-07 14:45:10.000000 openapify-0.1.3/setup.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-07 14:47:27.023145 openapify-0.1.3/tests/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       85 2023-03-20 20:36:26.000000 openapify-0.1.3/tests/test_aiohttp.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:01:19.765096 openapify-0.3/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      749 2023-04-11 15:01:19.764962 openapify-0.3/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    29266 2023-04-11 15:00:22.000000 openapify-0.3/README.md
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:01:19.762002 openapify-0.3/openapify/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      282 2023-04-09 19:40:13.000000 openapify-0.3/openapify/__init__.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:01:19.763783 openapify-0.3/openapify/core/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-04-03 13:14:57.000000 openapify-0.3/openapify/core/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    14737 2023-04-11 12:57:05.000000 openapify-0.3/openapify/core/builder.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       92 2023-03-20 20:50:13.000000 openapify-0.3/openapify/core/const.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2002 2023-04-11 12:57:05.000000 openapify-0.3/openapify/core/document.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1630 2023-04-09 15:42:39.000000 openapify-0.3/openapify/core/jsonschema.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1748 2023-04-09 15:04:29.000000 openapify-0.3/openapify/core/models.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:01:19.764085 openapify-0.3/openapify/core/openapi/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-20 12:12:59.000000 openapify-0.3/openapify/core/openapi/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5270 2023-04-09 09:42:43.000000 openapify-0.3/openapify/core/openapi/models.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5208 2023-04-10 17:45:46.000000 openapify-0.3/openapify/decorators.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:01:19.764317 openapify-0.3/openapify/ext/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 15:48:32.000000 openapify-0.3/openapify/ext/__init__.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:01:19.764494 openapify-0.3/openapify/ext/web/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-18 09:45:46.000000 openapify-0.3/openapify/ext/web/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     4767 2023-04-11 10:22:05.000000 openapify-0.3/openapify/ext/web/aiohttp.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 11:19:37.000000 openapify-0.3/openapify/py.typed
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-11 15:01:19.762644 openapify-0.3/openapify.egg-info/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      749 2023-04-11 15:01:19.000000 openapify-0.3/openapify.egg-info/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      605 2023-04-11 15:01:19.000000 openapify-0.3/openapify.egg-info/SOURCES.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-11 15:01:19.000000 openapify-0.3/openapify.egg-info/dependency_links.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-11 15:01:19.000000 openapify-0.3/openapify.egg-info/not-zip-safe
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       42 2023-04-11 15:01:19.000000 openapify-0.3/openapify.egg-info/requires.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       10 2023-04-11 15:01:19.000000 openapify-0.3/openapify.egg-info/top_level.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      364 2023-04-07 11:44:47.000000 openapify-0.3/pyproject.toml
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       38 2023-04-11 15:01:19.765135 openapify-0.3/setup.cfg
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1132 2023-04-11 14:59:28.000000 openapify-0.3/setup.py
```

### Comparing `openapify-0.1.3/PKG-INFO` & `openapify-0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openapify
-Version: 0.1.3
-Summary: Generate Open API Specification using decorators
+Version: 0.3
+Summary: Framework agnostic OpenAPI Specification generation for code lovers
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `openapify-0.1.3/openapify/core/builder.py` & `openapify-0.3/openapify/core/builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from contextlib import suppress
-from enum import Enum
 from typing import (
     Any,
     Dict,
     Iterable,
     List,
     Mapping,
     Optional,
     Sequence,
     Tuple,
     Type,
     Union,
     overload,
 )
 
-from apispec import BasePlugin
-from mashumaro.core.meta.helpers import type_name
+import apispec
 from typing_extensions import TypeAlias
 
-from openapify.core.apispec import APISpec
-from openapify.core.jsonschema import build_json_schema
+from openapify.core.const import (
+    DEFAULT_OPENAPI_VERSION,
+    DEFAULT_SPEC_TITLE,
+    DEFAULT_SPEC_VERSION,
+)
+from openapify.core.document import OpenAPIDocument
+from openapify.core.jsonschema import ComponentType, build_json_schema
 from openapify.core.models import (
     Body,
     Cookie,
     Header,
     QueryParam,
     RouteDef,
     SecurityRequirement,
@@ -42,116 +44,56 @@
     "delete",
     "head",
     "options",
     "trace",
 ]
 
 
-class APISpecObjectType(Enum):
-    SCHEMA = "schema"
-    HEADER = "header"
-    PARAMETER = "parameter"
-
-
-def _build_object_schema(
-    spec: APISpec,
-    instance_type: Union[Type, openapi.Schema],
-    object_type: APISpecObjectType = APISpecObjectType.SCHEMA,
-    component_id: Optional[ComponentID] = None,
-    parameter_location: Optional[str] = None,
-) -> Union[ComponentID, openapi.Schema]:
-    schema = build_json_schema(instance_type, spec)
-    if schema:
-        return schema
-    if not component_id:
-        component_id = type_name(instance_type)
-    with suppress(Exception):
-        if isinstance(instance_type, dict):
-            schema = instance_type
-    # FIXME: The following code won't work properly
-    if schema:
-        # Use dict schema as is
-        if object_type is APISpecObjectType.PARAMETER:
-            if not parameter_location:
-                raise Exception(
-                    "parameter_location can't be empty for parameters"
-                )
-            spec.components.parameter(
-                component_id, location=parameter_location
-            )
-        getattr(spec.components, object_type.value)(component_id, schema)
-        return schema
-    else:
-        # Try to apply apispec plugins
-        getattr(spec.components, object_type.value)(
-            component_id, schema=instance_type
-        )
-        return component_id
-
-
 def _merge_parameters(
     old_parameters: Sequence[openapi.Parameter], new_parameters: Dict[str, str]
 ) -> Sequence[openapi.Parameter]:
     for parameter in old_parameters or []:
         parameter_description = new_parameters.get(parameter.name)
         if parameter_description:
             parameter.description = parameter_description
     return old_parameters
 
 
-@overload
-def build_spec(routes: Iterable[RouteDef], spec: APISpec) -> APISpec:
-    ...
-
-
-@overload
-def build_spec(
-    routes: Iterable[RouteDef],
-    *,
-    title: str = "API",
-    version: str = "1.0.0",
-    openapi_version: str = "3.1.0",
-    plugins: Sequence[BasePlugin] = (),
-    **options: Any,
-) -> APISpec:
-    ...
-
-
 class OpenAPISpecBuilder:
     def __init__(
         self,
-        spec: Optional[APISpec] = None,
-        title: str = "API",
-        version: str = "1.0.0",
-        openapi_version: str = "3.1.0",
-        plugins: Sequence[BasePlugin] = (),
+        spec: Optional[apispec.APISpec] = None,
+        title: str = DEFAULT_SPEC_TITLE,
+        version: str = DEFAULT_SPEC_VERSION,
+        openapi_version: str = DEFAULT_OPENAPI_VERSION,
+        plugins: Sequence[apispec.BasePlugin] = (),
         servers: Optional[List[Union[str, openapi.Server]]] = None,
         security_schemes: Optional[Dict[str, openapi.SecurityScheme]] = None,
         **options: Any,
     ):
         if spec is None:
-            spec = APISpec(
+            spec = OpenAPIDocument(
                 title=title,
                 version=version,
                 openapi_version=openapi_version,
                 plugins=plugins,
                 servers=servers,
                 security_schemes=security_schemes,
                 **options,
             )
         self.spec = spec
 
-    def feed_routes(self, routes: Iterable[RouteDef]):
+    def feed_routes(self, routes: Iterable[RouteDef]) -> None:
         for route in sorted(
             routes,
             key=lambda r: (r.path, METHOD_ORDER.index(r.method.lower())),
         ):
             self._process_route(route)
 
-    def _process_route(self, route: RouteDef):
+    def _process_route(self, route: RouteDef) -> None:
         method = route.method.lower()
         meta = getattr(route.handler, "__openapify__", [])
         code_responses = {}
         summary = route.summary
         description = route.description
         tags = route.tags.copy() if route.tags else []
         deprecated = None
@@ -186,28 +128,32 @@
                         examples=body_examples,
                     )
                 query_params = args.get("query_params")
                 if query_params:
                     parameters.extend(self._build_query_params(query_params))
                 headers = args.get("headers")
                 if headers:
-                    parameters.extend(self._build_headers(headers))
+                    parameters.extend(self._build_request_headers(headers))
                 cookies = args.get("cookies")
                 if cookies:
                     parameters.extend(self._build_cookies(cookies))
 
             elif args_type == "response":
                 args = args.copy()
                 http_code = args.pop("http_code")
-                code_responses[http_code] = self._build_response(**args)
+                body_value_type = args.pop("body")
+                if body_value_type is not None:
+                    code_responses[http_code] = self._build_response(
+                        body=body_value_type, **args
+                    )
             elif args_type == "path_docs":
                 summary = args.get("summary")
                 description = args.get("description")
                 tags.extend(args.get("tags") or [])
-                _merge_parameters(parameters, args.get("parameters") or {})
+                # _merge_parameters(parameters, args.get("parameters") or {})
                 external_docs = self._build_external_docs(
                     args.get("external_docs")
                 )
                 deprecated = args.pop("deprecated")
             elif args_type == "security_requirements":
                 security = self._build_security_requirements(
                     args.get("requirements")
@@ -236,16 +182,16 @@
     def _build_query_params(
         self, query_params: Dict[str, Union[Type, QueryParam]]
     ) -> Sequence[openapi.Parameter]:
         result = []
         for name, param in query_params.items():
             if not isinstance(param, QueryParam):
                 param = QueryParam(param)
-            parameter_schema = _build_object_schema(
-                self.spec, param.value_type, APISpecObjectType.PARAMETER
+            parameter_schema = build_json_schema(
+                param.value_type, self.spec, ComponentType.PARAMETER
             )
             if param.default is not None:
                 parameter_schema["default"] = param.default
             result.append(
                 openapi.Parameter(
                     name=name,
                     location=openapi.ParameterLocation.QUERY,
@@ -256,23 +202,23 @@
                     schema=parameter_schema,
                     example=param.example,
                     examples=self._build_examples(param.examples),
                 )
             )
         return result
 
-    def _build_headers(
+    def _build_request_headers(
         self, headers: Dict[str, Union[str, Header]]
     ) -> Sequence[openapi.Parameter]:
         result = []
         for name, header in headers.items():
             if not isinstance(header, Header):
                 header = Header(description=header)
-            parameter_schema = _build_object_schema(
-                self.spec, header.value_type, APISpecObjectType.PARAMETER
+            parameter_schema = build_json_schema(
+                header.value_type, self.spec, ComponentType.PARAMETER
             )
             result.append(
                 openapi.Parameter(
                     name=name,
                     location=openapi.ParameterLocation.HEADER,
                     description=header.description,
                     required=header.required,
@@ -281,23 +227,46 @@
                     schema=parameter_schema,
                     example=header.example,
                     examples=self._build_examples(header.examples),
                 )
             )
         return result
 
+    def _build_response_headers(
+        self, headers: Dict[str, Union[str, Header]]
+    ) -> Sequence[openapi.Header]:
+        result = []
+        for name, header in headers.items():
+            if not isinstance(header, Header):
+                header = Header(description=header)
+            header_schema = build_json_schema(
+                header.value_type, self.spec, ComponentType.HEADER
+            )
+            result.append(
+                openapi.Header(
+                    schema=header_schema,
+                    description=header.description,
+                    required=header.required,
+                    deprecated=header.deprecated,
+                    allowEmptyValue=header.allowEmptyValue,
+                    example=header.example,
+                    examples=self._build_examples(header.examples),
+                )
+            )
+        return result
+
     def _build_cookies(
-        self, cookies: Optional[Dict[str, Union[str, Cookie]]] = None
+        self, cookies: Dict[str, Union[str, Cookie]]
     ) -> Sequence[openapi.Parameter]:
         result = []
         for name, cookie in cookies.items():
             if not isinstance(cookie, Cookie):
                 cookie = Cookie(cookie)
-            parameter_schema = _build_object_schema(
-                self.spec, cookie.value_type, APISpecObjectType.PARAMETER
+            parameter_schema = build_json_schema(
+                cookie.value_type, self.spec, ComponentType.PARAMETER
             )
             result.append(
                 openapi.Parameter(
                     name=name,
                     location=openapi.ParameterLocation.QUERY,
                     description=cookie.description,
                     required=cookie.required,
@@ -313,66 +282,46 @@
     def _build_request_body(
         self,
         value_type: Type,
         media_type: str = "application/json",
         required: Optional[bool] = None,
         description: Optional[str] = None,
         example: Optional[Any] = None,
-        examples: Optional[Dict[str, Union[openapi.Example, Any]]] = None,
+        examples: Optional[Mapping[str, Union[openapi.Example, Any]]] = None,
     ) -> openapi.RequestBody:
-        component_id = type_name(value_type, short=True)
-        component_schema = build_json_schema(value_type, self.spec)
-        if component_schema:
-            schema = component_schema
-        else:
-            # Try to apply plugins with schema_helper
-            self.spec.components.schema(component_id, schema=value_type)
-            schema = component_id  # FIXME: type violation
         return openapi.RequestBody(
             description=description,
             content={
                 media_type: openapi.MediaType(
-                    schema=schema,
+                    schema=build_json_schema(value_type, self.spec),
                     example=example,
                     examples=self._build_examples(examples),
                 )
             },
             required=required,
         )
 
     def _build_response(
         self,
-        schema: Type,
+        body: Type,
         media_type: str = "application/json",
         description: Optional[str] = None,
-        headers: Optional[Dict[str, Union[openapi.Header, Type]]] = None,
+        headers: Optional[Dict[str, Union[str, Header]]] = None,
         example: Optional[Any] = None,
         examples: Optional[Dict[str, Union[openapi.Example, Any]]] = None,
     ) -> openapi.Response:
+        header_objects = {}
         if headers:
-            for key, value in headers.items():
-                if not isinstance(value, openapi.Header):
-                    header_schema = _build_object_schema(
-                        self.spec, value, APISpecObjectType.HEADER, key
-                    )
-                    headers[key] = openapi.Header(header_schema)
-        component_id = type_name(schema, short=True)
-        component_schema = build_json_schema(schema, self.spec)
-        if component_schema:
-            schema = component_schema
-        else:
-            # Try to apply plugins with schema_helper
-            self.spec.components.schema(component_id, schema=schema)
-            schema = component_id
+            header_objects = self._build_response_headers(headers)
         return openapi.Response(
             description=description,
-            headers=headers,
+            headers=header_objects or None,
             content={
                 media_type: openapi.MediaType(
-                    schema=schema,
+                    schema=build_json_schema(body, self.spec),
                     example=example,
                     examples=self._build_examples(examples),
                 ),
             },
         )
 
     @staticmethod
@@ -387,22 +336,22 @@
             return openapi.ExternalDocumentation(data)
 
     def _build_security_requirements(
         self,
         security: Optional[
             Union[SecurityRequirement, List[SecurityRequirement]]
         ] = None,
-    ) -> Optional[List[Dict[str, List[str]]]]:
+    ) -> Optional[List[Mapping[str, List[str]]]]:
         if security is None:
             return None
-        result = []
+        result: List[Mapping[str, List[str]]] = []
         if isinstance(security, dict):
             security = [security]
         for requirement in security:
-            for name, scheme in requirement.items():
+            for name, scheme in requirement.items():  # type: ignore
                 if name not in self.spec.components.security_schemes:
                     self.spec.components.security_scheme(
                         name, scheme.to_dict()
                     )
                 # TODO: include list of scopes for oauth2 or openIdConnect
                 result.append({name: []})
         return result
@@ -416,26 +365,48 @@
         result = {}
         for key, value in examples.items():
             if not isinstance(value, openapi.Example):
                 result[key] = openapi.Example(value)
         return result
 
 
+@overload
+def build_spec(
+    routes: Iterable[RouteDef], spec: apispec.APISpec
+) -> apispec.APISpec:
+    ...
+
+
+@overload
+def build_spec(
+    routes: Iterable[RouteDef],
+    *,
+    title: str = DEFAULT_SPEC_TITLE,
+    version: str = DEFAULT_SPEC_VERSION,
+    openapi_version: str = DEFAULT_OPENAPI_VERSION,
+    plugins: Sequence[apispec.BasePlugin] = (),
+    servers: Optional[List[Union[str, openapi.Server]]] = None,
+    security_schemes: Optional[Dict[str, openapi.SecurityScheme]] = None,
+    **options: Any,
+) -> apispec.APISpec:
+    ...
+
+
 def build_spec(
     routes: Iterable[RouteDef],
-    spec: Optional[APISpec] = None,
+    spec: Optional[apispec.APISpec] = None,
     *,
-    title: str = "API",
-    version: str = "1.0.0",
-    openapi_version: str = "3.1.0",
-    plugins: Sequence[BasePlugin] = (),
+    title: str = DEFAULT_SPEC_TITLE,
+    version: str = DEFAULT_SPEC_VERSION,
+    openapi_version: str = DEFAULT_OPENAPI_VERSION,
+    plugins: Sequence[apispec.BasePlugin] = (),
     servers: Optional[List[Union[str, openapi.Server]]] = None,
     security_schemes: Optional[Dict[str, openapi.SecurityScheme]] = None,
     **options: Any,
-) -> APISpec:
+) -> apispec.APISpec:
     builder = OpenAPISpecBuilder(
         spec=spec,
         title=title,
         version=version,
         openapi_version=openapi_version,
         plugins=plugins,
         servers=servers,
```

### Comparing `openapify-0.1.3/openapify/core/models.py` & `openapify-0.3/openapify/core/models.py`

 * *Files identical despite different names*

### Comparing `openapify-0.1.3/openapify/core/openapi/models.py` & `openapify-0.3/openapify/core/openapi/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 
 @dataclass
 class Responses(Object):
     default: Optional[Response] = None
     codes: Optional[Mapping[HttpCode, Response]] = None
 
-    def __post_serialize__(self, d: Dict[Any, Any]):
+    def __post_serialize__(self, d: Dict[Any, Any]) -> Dict[Any, Any]:
         codes = d.pop("codes", None)
         if codes:
             d.update(codes)
         return d
 
 
 class ParameterLocation(Enum):
@@ -92,16 +92,16 @@
 class ParameterStyle(Enum):
     SIMPLE = "simple"
     FORM = "form"
 
 
 @dataclass
 class Parameter(Object):
-    name: Optional[str] = None
-    location: Optional[ParameterLocation] = None
+    name: str
+    location: ParameterLocation
     description: Optional[str] = None
     required: Optional[bool] = None
     deprecated: Optional[bool] = None
     allowEmptyValue: Optional[bool] = None
     style: Optional[ParameterStyle] = None
     explode: Optional[bool] = None
     schema: Optional[Schema] = None
@@ -161,15 +161,15 @@
 @dataclass
 class OAuthFlows(Object):
     pass
 
 
 @dataclass
 class OAuth2SecurityScheme(SecurityScheme):
-    flows: OAuthFlows = None
+    flows: Optional[OAuthFlows] = None
     type: Literal[SecuritySchemeType.OAUTH2] = SecuritySchemeType.OAUTH2
     description: Optional[str] = None
 
 
 @dataclass
 class OpenIDConnectSecurityScheme(SecurityScheme):
     openIdConnectUrl: str = ""
@@ -185,15 +185,15 @@
     summary: Optional[str] = None
     description: Optional[str] = None
     externalDocs: Optional[ExternalDocumentation] = None
     parameters: Optional[List[Parameter]] = None
     requestBody: Optional[RequestBody] = None
     responses: Optional[Responses] = None
     deprecated: Optional[bool] = None
-    security: Optional[List[Mapping[str, str]]] = None
+    security: Optional[List[Mapping[str, List[str]]]] = None
 
 
 @dataclass
 class PathItem(Object):
     # TODO: Do we need this class?
     ref: Optional[str] = None
     summary: Optional[str] = None
```

### Comparing `openapify-0.1.3/openapify/decorators.py` & `openapify-0.3/openapify/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,30 +50,30 @@
     query_params: Optional[Mapping[str, Union[Type, QueryParam]]] = None,
     headers: Optional[Mapping[str, Union[str, Header]]] = None,
     cookies: Optional[Mapping[str, Union[str, Cookie]]] = None,
 ) -> Callable[[Handler], Handler]:
     ...
 
 
-def request_schema(
+def request_schema(  # type: ignore[misc]
     body: Optional[Type] = None,
     *,
     media_type: str = "application/json",
     body_required: bool = False,
     body_description: Optional[str] = None,
     body_example: Optional[Any] = None,
     body_examples: Optional[Mapping[str, Union[Example, Any]]] = None,
     query_params: Optional[Mapping[str, Union[Type, QueryParam]]] = None,
     headers: Optional[Mapping[str, Union[str, Header]]] = None,
     cookies: Optional[Mapping[str, Union[str, Cookie]]] = None,
 ) -> Callable[[Handler], Handler]:
     def decorator(handler: Handler) -> Handler:
         meta = getattr(handler, __openapify__, [])
         if not meta:
-            handler.__openapify__ = meta
+            handler.__openapify__ = meta  # type: ignore[attr-defined]
         meta.append(
             (
                 "request",
                 {
                     "body": body,
                     "media_type": media_type,
                     "body_required": body_required,
@@ -88,31 +88,33 @@
         )
         return handler
 
     return decorator
 
 
 def response_schema(
-    schema: Type,
+    body: Optional[Type] = None,
     http_code: HttpCode = 200,
     media_type: str = "application/json",
     description: Optional[str] = None,
+    # TODO: Generate a required description depending on http_code
+    # https://spec.openapis.org/oas/v3.1.0#response-object
     headers: Optional[Mapping[str, Union[str, Header]]] = None,
     example: Optional[Any] = None,
     examples: Optional[Mapping[str, Union[Example, Any]]] = None,
-):
-    def decorator(handler):
+) -> Callable[[Handler], Handler]:
+    def decorator(handler: Handler) -> Handler:
         meta = getattr(handler, __openapify__, [])
         if not meta:
-            handler.__openapify__ = meta
+            handler.__openapify__ = meta  # type: ignore[attr-defined]
         meta.append(
             (
                 "response",
                 {
-                    "schema": schema,
+                    "body": body,
                     "http_code": http_code,
                     "media_type": media_type,
                     "description": description,
                     "headers": headers,
                     "example": example,
                     "examples": examples,
                 },
@@ -123,46 +125,46 @@
     return decorator
 
 
 def path_docs(
     summary: Optional[str] = None,
     description: Optional[str] = None,
     tags: Optional[Sequence[str]] = None,
-    parameters: Optional[Mapping[str, Union[str, Parameter]]] = None,
+    # parameters: Optional[Mapping[str, Union[str, Parameter]]] = None,
     external_docs: Optional[Union[str, Tuple[str, str]]] = None,
     deprecated: Optional[bool] = None,
-):
-    def decorator(handler):
+) -> Callable[[Handler], Handler]:
+    def decorator(handler: Handler) -> Handler:
         meta = getattr(handler, __openapify__, [])
         if not meta:
-            handler.__openapify__ = meta
+            handler.__openapify__ = meta  # type: ignore[attr-defined]
         meta.append(
             (
                 "path_docs",
                 {
                     "summary": summary,
                     "description": description,
                     "tags": tags,
-                    "parameters": parameters,
+                    # "parameters": parameters,
                     "external_docs": external_docs,
                     "deprecated": deprecated,
                 },
             ),
         )
         return handler
 
     return decorator
 
 
 def security_requirements(
     requirements: Optional[
         Union[SecurityRequirement, List[SecurityRequirement]]
     ] = None,
-):
-    def decorator(handler):
+) -> Callable[[Handler], Handler]:
+    def decorator(handler: Handler) -> Handler:
         meta = getattr(handler, __openapify__, [])
         if not meta:
-            handler.__openapify__ = meta
+            handler.__openapify__ = meta  # type: ignore[attr-defined]
         meta.append(("security_requirements", {"requirements": requirements}))
         return handler
 
     return decorator
```

### Comparing `openapify-0.1.3/openapify/ext/web/aiohttp.py` & `openapify-0.3/openapify/ext/web/aiohttp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 from typing import (
     Any,
     Callable,
     Iterable,
     List,
+    Mapping,
     Optional,
     Protocol,
     Sequence,
     Tuple,
     Type,
     Union,
     overload,
@@ -25,28 +26,37 @@
 from openapify.core.const import (
     DEFAULT_OPENAPI_VERSION,
     DEFAULT_SPEC_TITLE,
     DEFAULT_SPEC_VERSION,
 )
 from openapify.core.jsonschema import build_json_schema
 from openapify.core.models import RouteDef
-from openapify.core.openapi.models import Parameter, ParameterLocation
+from openapify.core.openapi.models import (
+    Parameter,
+    ParameterLocation,
+    SecurityScheme,
+    Server,
+)
 
 PARAMETER_TEMPLATE = re.compile(r"{([^:{}]+)(?::(.+))?}")
 
 
 class AioHttpRouteDef(Protocol):
     method: str
     path: str
     handler: Union[Type[AbstractView], Handler]
 
 
 def _aiohttp_app_to_route_defs(app: Application) -> Iterable[RouteDef]:
     for route in app.router.routes():
-        yield RouteDef(route.resource.canonical, route.method, route.handler)
+        yield RouteDef(
+            path=route.resource.canonical,  # type: ignore
+            method=route.method,
+            handler=route.handler,
+        )
 
 
 def _aiohttp_route_defs_to_route_defs(
     route_defs: Iterable[AioHttpRouteDef],
 ) -> Iterable[RouteDef]:
     for route in route_defs:
         if route.method == hdrs.METH_ANY:
@@ -57,21 +67,21 @@
         else:
             yield RouteDef(route.path, route.method, route.handler)
 
 
 def _pull_out_path_parameters(path: str) -> Tuple[str, List[Parameter]]:
     parameters = []
 
-    def _sub(match):
+    def _sub(match: re.Match) -> str:
         name = match.group(1)
         regex = match.group(2)
         if regex:
             instance_type = Annotated[str, Pattern(regex)]
         else:
-            instance_type = str
+            instance_type = str  # type: ignore[misc]
         parameters.append(
             Parameter(
                 name=name,
                 location=ParameterLocation.PATH,
                 required=True,
                 schema=build_json_schema(instance_type),
             )
@@ -86,20 +96,22 @@
         route.path, parameters = _pull_out_path_parameters(route.path)
         if parameters:
             route.parameters = parameters
         yield route
 
 
 @overload
-def build_spec(app: Application, spec: APISpec) -> APISpec:
+def build_spec(app: Application, spec: Optional[APISpec] = None) -> APISpec:
     ...
 
 
 @overload
-def build_spec(routes: Iterable[AioHttpRouteDef], spec: APISpec) -> APISpec:
+def build_spec(
+    routes: Iterable[AioHttpRouteDef], spec: Optional[APISpec] = None
+) -> APISpec:
     ...
 
 
 @overload
 def build_spec(
     app: Application,
     *,
@@ -123,22 +135,24 @@
     plugins: Sequence[BasePlugin] = (),
     route_postprocessor: Optional[Callable[[RouteDef], RouteDef]] = None,
     **options: Any,
 ) -> APISpec:
     ...
 
 
-def build_spec(
+def build_spec(  # type: ignore[misc]
     app_or_routes: Union[Application, Iterable[AioHttpRouteDef]],
     spec: Optional[APISpec] = None,
     *,
     title: str = DEFAULT_SPEC_TITLE,
     version: str = DEFAULT_SPEC_VERSION,
     openapi_version: str = DEFAULT_OPENAPI_VERSION,
     plugins: Sequence[BasePlugin] = (),
+    servers: Optional[List[Union[str, Server]]] = None,
+    security_schemes: Optional[Mapping[str, SecurityScheme]] = None,
     route_postprocessor: Optional[Callable[[RouteDef], RouteDef]] = None,
     **options: Any,
 ) -> APISpec:
     if isinstance(app_or_routes, Application):
         routes = _aiohttp_app_to_route_defs(app_or_routes)
     else:
         routes = _aiohttp_route_defs_to_route_defs(app_or_routes)
@@ -148,12 +162,14 @@
     return core_build_spec(
         routes=routes,
         spec=spec,
         title=title,
         version=version,
         openapi_version=openapi_version,
         plugins=plugins,
+        servers=servers,
+        security_schemes=security_schemes,
         **options,
     )
 
 
 __all__ = ["build_spec"]
```

### Comparing `openapify-0.1.3/openapify.egg-info/PKG-INFO` & `openapify-0.3/openapify.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openapify
-Version: 0.1.3
-Summary: Generate Open API Specification using decorators
+Version: 0.3
+Summary: Framework agnostic OpenAPI Specification generation for code lovers
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `openapify-0.1.3/openapify.egg-info/SOURCES.txt` & `openapify-0.3/openapify.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
+README.md
 pyproject.toml
 setup.py
 openapify/__init__.py
 openapify/decorators.py
 openapify/py.typed
 openapify.egg-info/PKG-INFO
 openapify.egg-info/SOURCES.txt
 openapify.egg-info/dependency_links.txt
 openapify.egg-info/not-zip-safe
 openapify.egg-info/requires.txt
 openapify.egg-info/top_level.txt
 openapify/core/__init__.py
-openapify/core/apispec.py
 openapify/core/builder.py
 openapify/core/const.py
+openapify/core/document.py
 openapify/core/jsonschema.py
 openapify/core/models.py
 openapify/core/openapi/__init__.py
 openapify/core/openapi/models.py
 openapify/ext/__init__.py
 openapify/ext/web/__init__.py
-openapify/ext/web/aiohttp.py
-tests/test_aiohttp.py
+openapify/ext/web/aiohttp.py
```

### Comparing `openapify-0.1.3/setup.py` & `openapify-0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="openapify",
-    version="0.1.3",
-    description="Generate Open API Specification using decorators",
+    version="0.3",
+    description=(
+        "Framework agnostic OpenAPI Specification generation for code lovers"
+    ),
     platforms="all",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

