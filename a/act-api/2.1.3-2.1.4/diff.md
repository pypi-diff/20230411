# Comparing `tmp/act-api-2.1.3.tar.gz` & `tmp/act-api-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "act-api-2.1.3.tar", last modified: Wed Mar 15 09:44:21 2023, max compression
+gzip compressed data, was "act-api-2.1.4.tar", last modified: Tue Apr 11 11:20:14 2023, max compression
```

## Comparing `act-api-2.1.3.tar` & `act-api-2.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-15 09:44:21.580736 act-api-2.1.3/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      196 2019-08-02 08:09:43.000000 act-api-2.1.3/AUTHORS
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      767 2022-10-12 05:45:17.000000 act-api-2.1.3/LICENSE
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    20551 2023-03-15 09:44:21.580736 act-api-2.1.3/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    20030 2023-03-15 09:44:18.000000 act-api-2.1.3/README.md
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-15 09:44:21.580736 act-api-2.1.3/act/
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-15 09:44:21.580736 act-api-2.1.3/act/api/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      781 2022-10-12 05:45:17.000000 act-api-2.1.3/act/api/__init__.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    13593 2022-10-13 09:55:52.000000 act-api-2.1.3/act/api/base.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    24604 2022-10-13 09:55:52.000000 act-api-2.1.3/act/api/fact.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    23312 2022-10-12 05:45:17.000000 act-api-2.1.3/act/api/helpers.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-15 09:44:21.580736 act-api-2.1.3/act/api/libs/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        0 2021-11-04 13:40:58.000000 act-api-2.1.3/act/api/libs/__init__.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9063 2023-03-15 09:44:18.000000 act-api-2.1.3/act/api/libs/cli.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     4716 2022-08-05 07:30:50.000000 act-api-2.1.3/act/api/obj.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      299 2021-11-04 13:40:58.000000 act-api-2.1.3/act/api/re.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     8820 2022-10-13 09:16:01.000000 act-api-2.1.3/act/api/schema.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2002 2021-11-04 13:40:58.000000 act-api-2.1.3/act/api/utils.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-15 09:44:21.580736 act-api-2.1.3/act_api.egg-info/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    20551 2023-03-15 09:44:21.000000 act-api-2.1.3/act_api.egg-info/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      535 2023-03-15 09:44:21.000000 act-api-2.1.3/act_api.egg-info/SOURCES.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2023-03-15 09:44:21.000000 act-api-2.1.3/act_api.egg-info/dependency_links.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        4 2023-03-15 09:44:21.000000 act-api-2.1.3/act_api.egg-info/namespace_packages.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       31 2023-03-15 09:44:21.000000 act-api-2.1.3/act_api.egg-info/requires.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        4 2023-03-15 09:44:21.000000 act-api-2.1.3/act_api.egg-info/top_level.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       79 2023-03-15 09:44:21.584069 act-api-2.1.3/setup.cfg
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1035 2023-03-15 09:44:18.000000 act-api-2.1.3/setup.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-03-15 09:44:21.580736 act-api-2.1.3/test/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      986 2021-11-04 13:40:58.000000 act-api-2.1.3/test/test_base.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    14442 2022-10-12 05:45:17.000000 act-api-2.1.3/test/test_fact.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     4367 2021-11-11 14:27:54.000000 act-api-2.1.3/test/test_helpers.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     4487 2021-11-04 13:40:58.000000 act-api-2.1.3/test/test_object.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1341 2021-11-04 13:40:58.000000 act-api-2.1.3/test/test_origin.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     4230 2021-11-04 13:40:58.000000 act-api-2.1.3/test/test_schema.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-11 11:20:14.069187 act-api-2.1.4/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      196 2019-08-02 08:09:43.000000 act-api-2.1.4/AUTHORS
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      767 2022-10-12 05:45:17.000000 act-api-2.1.4/LICENSE
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    20551 2023-04-11 11:20:14.069187 act-api-2.1.4/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    20030 2023-03-15 09:44:18.000000 act-api-2.1.4/README.md
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-11 11:20:14.069187 act-api-2.1.4/act/
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-11 11:20:14.069187 act-api-2.1.4/act/api/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      928 2023-04-11 11:20:11.000000 act-api-2.1.4/act/api/__init__.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    13741 2023-04-11 11:20:11.000000 act-api-2.1.4/act/api/base.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    24910 2023-04-11 11:20:11.000000 act-api-2.1.4/act/api/fact.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    23349 2023-04-11 11:20:11.000000 act-api-2.1.4/act/api/helpers.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-11 11:20:14.069187 act-api-2.1.4/act/api/libs/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        0 2021-11-04 13:40:58.000000 act-api-2.1.4/act/api/libs/__init__.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9672 2023-04-11 11:20:11.000000 act-api-2.1.4/act/api/libs/cli.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     4716 2022-08-05 07:30:50.000000 act-api-2.1.4/act/api/obj.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      299 2021-11-04 13:40:58.000000 act-api-2.1.4/act/api/re.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     8820 2022-10-13 09:16:01.000000 act-api-2.1.4/act/api/schema.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2002 2021-11-04 13:40:58.000000 act-api-2.1.4/act/api/utils.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-11 11:20:14.069187 act-api-2.1.4/act_api.egg-info/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    20551 2023-04-11 11:20:14.000000 act-api-2.1.4/act_api.egg-info/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      535 2023-04-11 11:20:14.000000 act-api-2.1.4/act_api.egg-info/SOURCES.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2023-04-11 11:20:14.000000 act-api-2.1.4/act_api.egg-info/dependency_links.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        4 2023-04-11 11:20:14.000000 act-api-2.1.4/act_api.egg-info/namespace_packages.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       31 2023-04-11 11:20:14.000000 act-api-2.1.4/act_api.egg-info/requires.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        4 2023-04-11 11:20:14.000000 act-api-2.1.4/act_api.egg-info/top_level.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       79 2023-04-11 11:20:14.069187 act-api-2.1.4/setup.cfg
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1035 2023-04-11 11:20:11.000000 act-api-2.1.4/setup.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-11 11:20:14.069187 act-api-2.1.4/test/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      986 2021-11-04 13:40:58.000000 act-api-2.1.4/test/test_base.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    14442 2022-10-12 05:45:17.000000 act-api-2.1.4/test/test_fact.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     4367 2021-11-11 14:27:54.000000 act-api-2.1.4/test/test_helpers.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     4487 2021-11-04 13:40:58.000000 act-api-2.1.4/test/test_object.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1341 2021-11-04 13:40:58.000000 act-api-2.1.4/test/test_origin.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     4230 2021-11-04 13:40:58.000000 act-api-2.1.4/test/test_schema.py
```

### Comparing `act-api-2.1.3/LICENSE` & `act-api-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `act-api-2.1.3/PKG-INFO` & `act-api-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: act-api
-Version: 2.1.3
+Version: 2.1.4
 Summary: Python library to connect to the ACT rest API
 Home-page: https://github.com/mnemonic-no
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: MIT
 Keywords: ACT,mnemonic
 Classifier: Development Status :: 4 - Beta
```

### Comparing `act-api-2.1.3/README.md` & `act-api-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `act-api-2.1.3/act/api/base.py` & `act-api-2.1.4/act/api/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,15 @@
         origin_name=None,
         origin_id=None,
         access_mode=DEFAULT_ACCESS_MODE,
         organization=None,
         object_validator=None,
         object_formatter=None,
         strict_validator=False,
+        acl=[],
     ):
         """
         act_baseurl - url to ACT instance
         use_id - ACT user ID
         requests_common_kwargs - options that will be passed to requests when connecting to ACT api
         origin_name - ACT origin name that will be added to all facts where origin is not set
         origin_id - ACT origin id that will be added to all facts where origin is not set
@@ -233,24 +234,28 @@
 
         Only one of origin_name of origin_id must be specified.
         """
 
         if origin_id and not re.search(UUID_MATCH, origin_id):
             raise ArgumentError("origin_id id not a valaid UUID: {}".format(origin_id))
 
+        if not isinstance(acl, list):
+            raise ArgumentError("acl must be a list: {}".format(acl))
+
         self.act_baseurl = act_baseurl
         self.user_id = user_id
         self.requests_common_kwargs = requests_common_kwargs
         self.origin_name = origin_name
         self.origin_id = origin_id
         self.access_mode = access_mode
         self.organization = organization
         self.object_validator = object_validator
         self.object_formatter = object_formatter
         self.strict_validator = strict_validator
+        self.acl = acl
 
 
 class ActBase(Schema):
     """Act object inheriting Schema, to support serializing and
     deserializing."""
 
     config = None
```

### Comparing `act-api-2.1.3/act/api/fact.py` & `act-api-2.1.4/act/api/fact.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,23 @@
 from logging import error, info, warning
 from typing import Any, Iterable, Union
 
 import act.api
 from act.api.re import UUID_MATCH
 
 from . import DEFAULT_FACT_VALIDATOR
-from .base import (ActBase, Comment, NameSpace, Organization, Origin,
-                   UserReference, origin_serializer)
+from .base import (
+    ActBase,
+    Comment,
+    NameSpace,
+    Organization,
+    Origin,
+    UserReference,
+    origin_serializer,
+)
 from .obj import Object, ObjectType
 from .schema import Field, MissingField, ValidationError, schema_doc
 
 
 class IllegalFactChain(Exception):
     def __init__(self, *args, **kwargs):
         Exception.__init__(self, *args, **kwargs)
@@ -113,15 +120,16 @@
     def add_object_binding(
         self, source_object_type, destination_object_type, bidirectional_binding=False
     ):
         """Add bindings
         Args:
             source_object_type (objectType):        Source Object Type
             destination_object_type (objectType):   Destination Object Type
-            bidirectional_binding (boolean):        Whether the binding is bidirectional"""
+            bidirectional_binding (boolean):        Whether the binding is bidirectional
+        """
         return self.add_object_bindings(
             [
                 RelevantObjectBindings(
                     source_object_type, destination_object_type, bidirectional_binding
                 )
             ]
         )
@@ -246,15 +254,14 @@
     if obj.id:
         return obj.id
 
     return "{}/{}".format(obj.type.name, obj.value)
 
 
 class AbstractFact(ActBase):
-
     SCHEMA = [
         Field(
             "type", deserializer=FactType, serializer=lambda fact_type: fact_type.name
         ),
         Field("value", default=None),
         Field("id", serializer=False),
         Field("flags", serializer=False),
@@ -264,14 +271,15 @@
         Field("trust", serializer=False),
         Field("confidence"),
         Field("certainty", serializer=False),
         Field("timestamp", serializer=False),
         Field("last_seen_timestamp", serializer=False),
         Field("organization", deserializer=Organization),
         Field("access_mode"),
+        Field("acl"),
         Field("source_object", deserializer=Object),
         Field("destination_object", deserializer=Object),
         Field("bidirectional_binding", default=False),
         Field("last_seen_by", deserializer=UserReference, serializer=False),
     ]
 
     @schema_doc(SCHEMA)
@@ -289,27 +297,33 @@
         self.deserialize(**fact)
         return self
 
     def set_defaults(self):
         """
         Set fact defaults from config if we have not specified
         - access_mode
+        - acl
         - origin
         - organization
         """
 
+        self.acl = self.acl or self.config.acl
         self.access_mode = self.access_mode or self.config.access_mode
         self.organization = self.organization or self.config.organization
 
         if self.access_mode not in act.api.ACCESS_MODES:
             raise act.api.base.ArgumentError(
                 f"Illegal access_mode: {self.access_mode}. Must be one of "
                 + f"{','.join(act.api.ACCESS_MODES)}"
             )
 
+        # If ACL is set, access mode should always be explicit
+        if self.acl and not self.access_mode == act.api.ACCESS_MODES_EXPLICIT:
+            self.access_mode == act.api.ACCESS_MODES_EXPLICIT
+
         if not self.origin:
             # If origin is not specified explicit on the fact, use origin from default config
             if self.config.origin_id:
                 self.origin = Origin(id=self.config.origin_id)
             elif self.config.origin_name:
                 self.origin = Origin(name=self.config.origin_name)
 
@@ -429,15 +443,14 @@
         # Add value if set
         if self.value and not self.value.startswith("-"):
             out += "/{}".format(self.value)
         out += "]"
 
         # Add destination object if set
         if self.destination_object:
-
             # Use arrow unless bidirectional
             if self.bidirectional_binding:
                 out += "-"
             else:
                 out += "->"
 
             out += " ({}/{})".format(
@@ -520,15 +533,14 @@
                 self.destination_object.type.name,
                 self.destination_object.value,
             )
 
         return self
 
     def validate_and_raise(self, object_validator=None):
-
         if not object_validator:
             if not self.config or not self.config.object_validator:
                 raise act.api.base.ArgumentError(
                     "object_validator must be specified as argument or in configuration"
                 )
 
             object_validator = self.config.object_validator
```

### Comparing `act-api-2.1.3/act/api/helpers.py` & `act-api-2.1.4/act/api/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
         log_level="debug",
         log_file=None,
         log_prefix="act",
         requests_common_kwargs=None,
         origin_name=None,
         origin_id=None,
         access_mode="RoleBased",
+        acl=[],
         organization=None,
         object_validator=None,
         object_formatter=None,
         strict_validator=False,
     ):
         super(Act, self).__init__()
 
@@ -144,14 +145,15 @@
                 origin_name,
                 origin_id,
                 access_mode,
                 organization,
                 object_validator,
                 object_formatter,
                 strict_validator,
+                acl,
             )
         )
 
         act.api.utils.setup_logging(log_level, log_file, log_prefix)
 
     # pylint: disable=unused-argument,dangerous-default-value
     def fact_search(
```

### Comparing `act-api-2.1.3/act/api/libs/cli.py` & `act-api-2.1.4/act/api/libs/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,27 @@
 
 import argparse
 import inspect
 import os
 import re
 import sys
 from logging import debug, error
-from typing import (Any, Callable, Dict, Optional, Text, Type, TypeVar, Union,
-                    cast)
+from typing import Any, Callable, Dict, List, Optional, Text, Type, TypeVar, Union, cast
 
 import caep
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, root_validator
 from pydantic.typing import Literal  # type: ignore
 
 import act.api
 
 CONFIG_ID = "act"
 CONFIG_NAME = "act.ini"
 
 
 class Config(BaseModel):
-
     http_timeout: int = Field(default=120, description="Timeout")
     proxy_string: Optional[str] = Field(description="Proxy to use for external queries")
     proxy_platform: bool = Field(
         default=False, description="Use proxy-string towards the ACT platform"
     )
     cert_file: Optional[str] = Field(
         description="Cerfiticate to add if you are behind a SSL/TLS "
@@ -43,36 +41,53 @@
     )
 
     http_user: Optional[str] = Field(description="ACT HTTP Basic Auth user")
     http_password: Optional[str] = Field(description="ACT HTTP Basic Auth password")
 
 
 class FactConfig(Config):
-
     # choices=["str", "json"],
     output_format: Literal["str", "json"] = Field(
         default="json",
         description="Output format for fact (default=json)",
     )
 
     access_mode: Literal["Public", "RoleBased", "Explicit"] = Field(
         default=act.api.DEFAULT_ACCESS_MODE,
         description="Specify default access mode used for all facts",
     )
+
+    acl: List[str] = Field(
+        description="Specify ACLs (commaseparated list of uuid or string) "
+        "for all facts. Requires `Explicit` access_mode.",
+    )
     organization: Optional[str] = Field(
         description="Specify default organization applied to all facts",
     )
 
     origin_name: Optional[str] = Field(
         description="Origin name. This name must be defined in the platform",
     )
     origin_id: Optional[str] = Field(
         description="Origin id. This must be the UUID of the origin in the platform",
     )
 
+    @root_validator
+    def check_arguments(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+        """If acl is set, access_mode *must* be `Explicit`"""
+
+        # If ACL is set, access mode should always be explicit
+        if (
+            values.get("acl")
+            and not values.get("access_mode") == act.api.ACCESS_MODES_EXPLICIT
+        ):
+            values["access_mode"] = act.api.ACCESS_MODES_EXPLICIT
+
+        return values
+
 
 ConfigType = TypeVar("ConfigType", bound=Config)
 
 
 def parseargs(description: str, fact_arguments=False) -> argparse.ArgumentParser:
     """Parse arguments"""
     parser = argparse.ArgumentParser(
```

### Comparing `act-api-2.1.3/act/api/obj.py` & `act-api-2.1.4/act/api/obj.py`

 * *Files identical despite different names*

### Comparing `act-api-2.1.3/act/api/schema.py` & `act-api-2.1.4/act/api/schema.py`

 * *Files identical despite different names*

### Comparing `act-api-2.1.3/act/api/utils.py` & `act-api-2.1.4/act/api/utils.py`

 * *Files identical despite different names*

### Comparing `act-api-2.1.3/act_api.egg-info/PKG-INFO` & `act-api-2.1.4/act_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: act-api
-Version: 2.1.3
+Version: 2.1.4
 Summary: Python library to connect to the ACT rest API
 Home-page: https://github.com/mnemonic-no
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: MIT
 Keywords: ACT,mnemonic
 Classifier: Development Status :: 4 - Beta
```

### Comparing `act-api-2.1.3/act_api.egg-info/SOURCES.txt` & `act-api-2.1.4/act_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `act-api-2.1.3/setup.py` & `act-api-2.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), "rb") as f:
     long_description = f.read().decode("utf-8")
 
 setup(
     name="act-api",
-    version="2.1.3",
+    version="2.1.4",
     author="mnemonic AS",
     author_email="opensource@mnemonic.no",
     description="Python library to connect to the ACT rest API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     keywords="ACT, mnemonic",
```

### Comparing `act-api-2.1.3/test/test_base.py` & `act-api-2.1.4/test/test_base.py`

 * *Files identical despite different names*

### Comparing `act-api-2.1.3/test/test_fact.py` & `act-api-2.1.4/test/test_fact.py`

 * *Files identical despite different names*

### Comparing `act-api-2.1.3/test/test_helpers.py` & `act-api-2.1.4/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `act-api-2.1.3/test/test_object.py` & `act-api-2.1.4/test/test_object.py`

 * *Files identical despite different names*

### Comparing `act-api-2.1.3/test/test_origin.py` & `act-api-2.1.4/test/test_origin.py`

 * *Files identical despite different names*

### Comparing `act-api-2.1.3/test/test_schema.py` & `act-api-2.1.4/test/test_schema.py`

 * *Files identical despite different names*

