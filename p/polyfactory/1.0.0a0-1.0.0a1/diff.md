# Comparing `tmp/polyfactory-1.0.0a0.tar.gz` & `tmp/polyfactory-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-1.0.0a0.tar", max compression
+gzip compressed data, was "polyfactory-1.0.0a1.tar", max compression
```

## Comparing `polyfactory-1.0.0a0.tar` & `polyfactory-1.0.0a1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     1091 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/LICENSE
--rw-r--r--   0        0        0     2199 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/README.md
--rw-r--r--   0        0        0      509 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/__init__.py
--rw-r--r--   0        0        0      605 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/constants.py
--rw-r--r--   0        0        0      578 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/exceptions.py
--rw-r--r--   0        0        0      154 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    28778 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2747 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1045 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0     9530 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1982 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3304 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/fields.py
--rw-r--r--   0        0        0     1201 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/py.typed
--rw-r--r--   0        0        0     2911 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     2134 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3384 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     3290 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1894 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1058 2023-04-01 12:04:48.623042 polyfactory-1.0.0a0/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13640 2023-04-01 12:04:48.627042 polyfactory-1.0.0a0/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0     3857 2023-04-01 12:04:48.627042 polyfactory-1.0.0a0/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0     3667 2023-04-01 12:04:48.627042 polyfactory-1.0.0a0/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6185 2023-04-01 12:04:48.627042 polyfactory-1.0.0a0/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     5589 2023-04-01 12:04:48.627042 polyfactory-1.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     4197 1970-01-01 00:00:00.000000 polyfactory-1.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-11 09:49:18.437820 polyfactory-1.0.0a1/LICENSE
+-rw-r--r--   0        0        0     4513 2023-04-11 09:49:18.437820 polyfactory-1.0.0a1/README.md
+-rw-r--r--   0        0        0      425 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/__init__.py
+-rw-r--r--   0        0        0      605 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/constants.py
+-rw-r--r--   0        0        0      578 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    26088 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2757 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1603 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     1074 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0     9542 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1471 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     1976 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3328 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/fields.py
+-rw-r--r--   0        0        0     1191 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/py.typed
+-rw-r--r--   0        0        0     2890 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     2162 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3401 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     3311 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1838 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1069 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13431 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0     3845 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0     3633 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6185 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     5964 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     6538 1970-01-01 00:00:00.000000 polyfactory-1.0.0a1/PKG-INFO
```

### Comparing `polyfactory-1.0.0a0/LICENSE` & `polyfactory-1.0.0a1/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021, 2022, 2023 Starlite-API
+Copyright (c) 2021, 2022, 2023 Litestar Org.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `polyfactory-1.0.0a0/polyfactory/constants.py` & `polyfactory-1.0.0a1/polyfactory/constants.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a0/polyfactory/exceptions.py` & `polyfactory-1.0.0a1/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a0/polyfactory/factories/base.py` & `polyfactory-1.0.0a1/polyfactory/factories/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,190 +1,184 @@
+from __future__ import annotations
 from abc import ABC, abstractmethod
 from collections import Counter, deque
 from contextlib import suppress
-from dataclasses import MISSING, fields, is_dataclass
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal
 from enum import EnumMeta
 from functools import partial
+from importlib import import_module
 from inspect import isclass
 from ipaddress import (
     IPv4Address,
     IPv4Interface,
     IPv4Network,
     IPv6Address,
     IPv6Interface,
     IPv6Network,
 )
-from math import nan
 from os.path import realpath
 from pathlib import Path
 from random import Random
-from typing import _TypedDictMeta  # type: ignore
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
-    Dict,
     Generic,
-    List,
     Mapping,
-    Optional,
     Sequence,
-    Tuple,
     Type,
     TypeVar,
-    Union,
     cast,
 )
 from uuid import NAMESPACE_DNS, UUID, uuid1, uuid3, uuid5
 
 from faker import Faker
-from typing_extensions import get_args, is_typeddict
+from typing_extensions import get_args
 
 from polyfactory.exceptions import (
     ConfigurationException,
     MissingBuildKwargException,
     ParameterException,
 )
-from polyfactory.field_meta import FieldMeta, Null
 from polyfactory.fields import Fixture, Ignore, PostGenerated, Require, Use
-from polyfactory.persistence import AsyncPersistenceProtocol, SyncPersistenceProtocol
+
 from polyfactory.utils.helpers import unwrap_annotation, unwrap_args, unwrap_optional
 from polyfactory.utils.predicates import (
     get_type_origin,
     is_literal,
     is_optional_union,
     is_safe_subclass,
 )
 from polyfactory.value_generators.complex_types import handle_complex_type
 from polyfactory.value_generators.primitives import (
     create_random_boolean,
     create_random_bytes,
 )
 
 if TYPE_CHECKING:
+    from polyfactory.persistence import AsyncPersistenceProtocol, SyncPersistenceProtocol
+    from polyfactory.field_meta import FieldMeta
     from typing_extensions import TypeGuard
 
-try:
-    from pydantic import (
-        UUID1,
-        UUID3,
-        UUID4,
-        UUID5,
-        AmqpDsn,
-        AnyHttpUrl,
-        AnyUrl,
-        ByteSize,
-        DirectoryPath,
-        EmailStr,
-        FilePath,
-        FutureDate,
-        HttpUrl,
-        IPvAnyAddress,
-        IPvAnyInterface,
-        IPvAnyNetwork,
-        Json,
-        KafkaDsn,
-        NameEmail,
-        NegativeFloat,
-        NegativeInt,
-        NonNegativeInt,
-        NonPositiveFloat,
-        PastDate,
-        PaymentCardNumber,
-        PositiveFloat,
-        PositiveInt,
-        PostgresDsn,
-        PyObject,
-        RedisDsn,
-        SecretBytes,
-        SecretStr,
-        StrictBool,
-        StrictBytes,
-        StrictFloat,
-        StrictInt,
-        StrictStr,
-    )
-    from pydantic.color import Color
-except ImportError:
-    # we use the fact that 'nan != nan' to ensure that these types are never matched
-    Color = nan  # type: ignore[misc, assignment]
-    UUID1 = nan  # type: ignore[misc, assignment]
-    UUID3 = nan  # type: ignore[misc, assignment]
-    UUID4 = nan  # type: ignore[misc, assignment]
-    UUID5 = nan  # type: ignore[misc, assignment]
-    AmqpDsn = nan  # type: ignore[misc]
-    AnyHttpUrl = nan  # type: ignore[misc]
-    AnyUrl = nan  # type: ignore[misc]
-    ByteSize = nan  # type: ignore[misc, assignment]
-    DirectoryPath = nan  # type: ignore[misc, assignment]
-    EmailStr = nan  # type: ignore[misc, assignment]
-    FilePath = nan  # type: ignore[misc, assignment]
-    FutureDate = nan  # type: ignore[misc, assignment]
-    HttpUrl = nan  # type: ignore[misc]
-    IPvAnyAddress = nan  # type: ignore[misc, assignment]
-    IPvAnyInterface = nan  # type: ignore[misc, assignment]
-    IPvAnyNetwork = nan  # type: ignore[misc, assignment]
-    Json = nan  # type: ignore[misc]
-    KafkaDsn = nan  # type: ignore[misc]
-    NameEmail = nan  # type: ignore[misc, assignment]
-    NegativeFloat = nan  # type: ignore[misc, assignment]
-    NegativeInt = nan  # type: ignore[misc, assignment]
-    NonNegativeInt = nan  # type: ignore[misc, assignment]
-    NonPositiveFloat = nan  # type: ignore[misc, assignment]
-    PastDate = nan  # type: ignore[misc, assignment]
-    PaymentCardNumber = nan  # type: ignore[misc, assignment]
-    PositiveFloat = nan  # type: ignore[misc, assignment]
-    PositiveInt = nan  # type: ignore[misc, assignment]
-    PostgresDsn = nan  # type: ignore[misc]
-    PyObject = nan  # type: ignore[misc]
-    RedisDsn = nan  # type: ignore[misc]
-    SecretBytes = nan  # type: ignore[misc, assignment]
-    SecretStr = nan  # type: ignore[misc, assignment]
-    StrictBool = nan  # type: ignore[misc, assignment]
-    StrictBytes = nan  # type: ignore[misc, assignment]
-    StrictFloat = nan  # type: ignore[misc, assignment]
-    StrictInt = nan  # type: ignore[misc, assignment]
-    StrictStr = nan  # type: ignore[misc, assignment]
+
+def _create_pydantic_type_map(cls: "type[BaseFactory]") -> dict[type, Callable[[], Any]]:
+    """Creates a mapping of pydantic types to mock data functions.
+
+    :param cls: The base factory class.
+    :return: A dict mapping types to callables.
+    """
+    try:
+        import pydantic
+
+        return {
+            pydantic.ByteSize: cls.__faker__.pyint,
+            pydantic.PositiveInt: cls.__faker__.pyint,
+            pydantic.FilePath: lambda: Path(realpath(__file__)),
+            pydantic.NegativeFloat: lambda: cls.__random__.uniform(-100, -1),
+            pydantic.NegativeInt: lambda: cls.__faker__.pyint() * -1,
+            pydantic.PositiveFloat: cls.__faker__.pyint,
+            pydantic.NonPositiveFloat: lambda: cls.__random__.uniform(-100, 0),
+            pydantic.NonNegativeInt: cls.__faker__.pyint,
+            pydantic.StrictInt: cls.__faker__.pyint,
+            pydantic.StrictBool: cls.__faker__.pybool,
+            pydantic.StrictBytes: partial(create_random_bytes, cls.__random__),
+            pydantic.StrictFloat: cls.__faker__.pyfloat,
+            pydantic.StrictStr: cls.__faker__.pystr,
+            pydantic.DirectoryPath: lambda: Path(realpath(__file__)).parent,
+            pydantic.EmailStr: cls.__faker__.free_email,
+            pydantic.NameEmail: cls.__faker__.free_email,
+            pydantic.PyObject: lambda: "decimal.Decimal",  # type: ignore[dict-item]
+            pydantic.color.Color: cls.__faker__.hex_color,  # pyright: ignore
+            pydantic.Json: cls.__faker__.json,
+            pydantic.PaymentCardNumber: cls.__faker__.credit_card_number,
+            pydantic.AnyUrl: cls.__faker__.url,
+            pydantic.AnyHttpUrl: cls.__faker__.url,
+            pydantic.HttpUrl: cls.__faker__.url,
+            pydantic.PostgresDsn: lambda: "postgresql://user:secret@localhost",
+            pydantic.RedisDsn: lambda: "redis://localhost:6379",
+            pydantic.UUID1: uuid1,
+            pydantic.UUID3: lambda: uuid3(NAMESPACE_DNS, cls.__faker__.pystr()),
+            pydantic.UUID4: cls.__faker__.uuid4,
+            pydantic.UUID5: lambda: uuid5(NAMESPACE_DNS, cls.__faker__.pystr()),
+            pydantic.SecretBytes: partial(create_random_bytes, cls.__random__),
+            pydantic.SecretStr: cls.__faker__.pystr,
+            pydantic.IPvAnyAddress: cls.__faker__.ipv4,
+            pydantic.IPvAnyInterface: cls.__faker__.ipv4,
+            pydantic.IPvAnyNetwork: lambda: cls.__faker__.ipv4(network=True),
+            pydantic.AmqpDsn: lambda: "amqps://",
+            pydantic.KafkaDsn: lambda: "kafka://",
+            pydantic.PastDate: cls.__faker__.past_date,
+            pydantic.FutureDate: cls.__faker__.future_date,
+        }
+    except ImportError:
+        return {}
 
 
 T = TypeVar("T")
 
 
-def is_factory(value: Any) -> "TypeGuard[Type[BaseFactory]]":
+def is_factory(value: Any) -> "TypeGuard[type[BaseFactory]]":
     """Determine if a given value is a subclass of ModelFactory.
 
     :param value: An arbitrary value.
     :returns: A boolean typeguard.
 
     """
     return isclass(value) and issubclass(value, BaseFactory)
 
 
 class BaseFactory(ABC, Generic[T]):
     """Base Factory class - this class holds the main logic of the library"""
 
     # configuration attributes
+    __model__: type[T]
+    """
+    The model for the factory.
+    This attribute is required for non-base factories and an exception will be raised if its not set.
+    """
     __allow_none_optionals__: ClassVar[bool] = True
-    __async_persistence__: Optional[Union[Type[AsyncPersistenceProtocol[T]], AsyncPersistenceProtocol[T]]] = None
+    """
+    Flag dictating whether to allow 'None' for optional values.
+    If 'True', 'None' will be randomly generated as a value for optional model fields
+    """
+    __sync_persistence__: type[SyncPersistenceProtocol[T]] | SyncPersistenceProtocol[T] | None = None
+    """A sync persistence handler. Can be a class or a class instance."""
+    __async_persistence__: type[AsyncPersistenceProtocol[T]] | AsyncPersistenceProtocol[T] | None = None
+    """An async persistence handler. Can be a class or a class instance."""
     __set_as_default_factory_for_type__ = False
+    """
+    Flag dictating whether to set as the default factory for the given type.
+    If 'True' the factory will be used instead of dynamically generating a factory for the type.
+    """
     __is_base_factory__: bool = False
+    """
+    Flag dictating whether the factory is a 'base' factory. Base factories are registered globally as handlers for types.
+    For example, the 'DataclassFactory', 'TypedDictFactory' and 'ModelFactory' are all base factories.
+    """
     __faker__: ClassVar["Faker"] = Faker()
+    """
+    A faker instance to use. Can be a user provided value.
+    """
     __random__: ClassVar["Random"] = Random()
-    __model__: Type[T]
+    """
+    An instance of 'random.Random' to use.
+    """
     __random_seed__: ClassVar[int]
-    __sync_persistence__: Optional[Union[Type[SyncPersistenceProtocol[T]], SyncPersistenceProtocol[T]]] = None
+    """
+    An integer to seed the factory's Faker and Random instances with.
+    This attribute can be used to control random generation.
+    """
 
     # cached attributes
-    _fields_metadata: List["FieldMeta"]
+    _fields_metadata: list["FieldMeta"]
     # BaseFactory only attributes
-    _factory_type_mapping: ClassVar[Dict[Any, Type["BaseFactory"]]]
-    _base_factories: ClassVar[List[Type["BaseFactory"]]]
+    _factory_type_mapping: ClassVar[dict[Any, type["BaseFactory"]]]
+    _base_factories: ClassVar[list[type["BaseFactory"]]]
 
     def __init_subclass__(cls, *args: Any, **kwargs: Any) -> None:
         super().__init_subclass__(*args, **kwargs)
 
         if not hasattr(BaseFactory, "_base_factories"):
             BaseFactory._base_factories = []
 
@@ -241,15 +235,15 @@
         if cls.__async_persistence__:
             return cls.__async_persistence__() if callable(cls.__async_persistence__) else cls.__async_persistence__
         raise ConfigurationException(
             "An '__async_persistence__' handler must be defined in the factory to use this method"
         )
 
     @classmethod
-    def _handle_factory_field(cls, field_value: Any, field_build_parameters: Optional[Any] = None) -> Any:
+    def _handle_factory_field(cls, field_value: Any, field_build_parameters: Any | None = None) -> Any:
         """Handle a value defined on the factory class itself.
 
         :param field_value: A value defined as an attribute on the factory class.
         :param field_build_parameters: Any build parameters passed to the factory as kwarg values.
 
         :returns: An arbitrary value correlating with the given field_meta value.
         """
@@ -272,16 +266,16 @@
             return field_value()
 
         return field_value
 
     @classmethod
     def _get_or_create_factory(
         cls,
-        model: Type,
-    ) -> Type["BaseFactory"]:
+        model: type,
+    ) -> type["BaseFactory"]:
         """Get a factory from registered factories or generate a factory dynamically.
 
         :param model: A model type.
         :returns: A Factory sub-class.
 
         """
         if factory := BaseFactory._factory_type_mapping.get(model):
@@ -313,15 +307,15 @@
         """
         origin = get_type_origin(annotation) or annotation
         if is_safe_subclass(origin, Sequence) and (args := unwrap_args(annotation)):  # type: ignore
             return len(args) == 1 and BaseFactory.is_factory_type(annotation=args[0])
         return False
 
     @classmethod
-    def extract_field_build_parameters(cls, field_meta: "FieldMeta", build_args: Dict[str, Any]) -> Any:
+    def extract_field_build_parameters(cls, field_meta: "FieldMeta", build_args: dict[str, Any]) -> Any:
         """Extract from the build kwargs any build parameters passed for a given field meta - if it is a factory type.
 
         :param field_meta: A field meta instance.
         :param build_args: Any kwargs passed to the factory.
         :returns: Any values
         """
         if build_arg := build_args.get(field_meta.name):
@@ -339,15 +333,15 @@
                 and not any(BaseFactory.is_factory_type(annotation=type(value)) for value in build_arg)
             ):
                 return build_args.pop(field_meta.name)
         return None
 
     @classmethod
     @abstractmethod
-    def is_supported_type(cls, value: Any) -> "TypeGuard[Type[T]]":  # pragma: no cover
+    def is_supported_type(cls, value: Any) -> "TypeGuard[type[T]]":  # pragma: no cover
         """Determine whether the given value is supported by the factory.
 
         :param value: An arbitrary value.
         :returns: A typeguard
         """
         raise NotImplementedError
 
@@ -373,113 +367,69 @@
 
         :returns: A boolean determining whether the value should be ignored.
 
         """
         return value is None
 
     @classmethod
-    def get_provider_map(cls) -> Dict[Any, Callable[[], Any]]:
+    def get_provider_map(cls) -> dict[Any, Callable[[], Any]]:
         """Map types to callables.
 
         :notes:
             - This method is distinct to allow overriding.
 
 
         :returns: a dictionary mapping types to callables.
 
         """
 
-        def _create_path() -> Path:
-            """Return the path to the current file"""
-            return Path(realpath(__file__))
-
         def _create_generic_fn() -> Callable:
             """Return a generic lambda"""
             return lambda *args: None
 
-        faker = cls.__faker__
-
         return {
             Any: lambda: None,
             # primitives
             object: object,
-            float: faker.pyfloat,
-            int: faker.pyint,
-            bool: faker.pybool,
-            str: faker.pystr,
+            float: cls.__faker__.pyfloat,
+            int: cls.__faker__.pyint,
+            bool: cls.__faker__.pybool,
+            str: cls.__faker__.pystr,
             bytes: partial(create_random_bytes, cls.__random__),
             # built-in objects
-            dict: faker.pydict,
-            tuple: faker.pytuple,
-            list: faker.pylist,
-            set: faker.pyset,
-            frozenset: lambda: frozenset(faker.pylist()),
-            deque: lambda: deque(faker.pylist()),
+            dict: cls.__faker__.pydict,
+            tuple: cls.__faker__.pytuple,
+            list: cls.__faker__.pylist,
+            set: cls.__faker__.pyset,
+            frozenset: lambda: frozenset(cls.__faker__.pylist()),
+            deque: lambda: deque(cls.__faker__.pylist()),
             # standard library objects
-            Path: _create_path,
-            Decimal: faker.pydecimal,
-            UUID: faker.uuid4,
+            Path: lambda: Path(realpath(__file__)),
+            Decimal: cls.__faker__.pydecimal,
+            UUID: cls.__faker__.uuid4,
             # datetime
-            datetime: faker.date_time_between,
-            date: faker.date_this_decade,
-            time: faker.time,
-            timedelta: faker.time_delta,
+            datetime: cls.__faker__.date_time_between,
+            date: cls.__faker__.date_this_decade,
+            time: cls.__faker__.time,
+            timedelta: cls.__faker__.time_delta,
             # ip addresses
-            IPv4Address: faker.ipv4,
-            IPv4Interface: faker.ipv4,
-            IPv4Network: lambda: faker.ipv4(network=True),
-            IPv6Address: faker.ipv6,
-            IPv6Interface: faker.ipv6,
-            IPv6Network: lambda: faker.ipv6(network=True),
+            IPv4Address: cls.__faker__.ipv4,
+            IPv4Interface: cls.__faker__.ipv4,
+            IPv4Network: lambda: cls.__faker__.ipv4(network=True),
+            IPv6Address: cls.__faker__.ipv6,
+            IPv6Interface: cls.__faker__.ipv6,
+            IPv6Network: lambda: cls.__faker__.ipv6(network=True),
             # types
             Callable: _create_generic_fn,
-            # pydantic specific
-            ByteSize: faker.pyint,
-            PositiveInt: faker.pyint,
-            FilePath: _create_path,
-            NegativeFloat: lambda: cls.__random__.uniform(-100, -1),
-            NegativeInt: lambda: faker.pyint() * -1,
-            PositiveFloat: faker.pyint,
-            NonPositiveFloat: lambda: cls.__random__.uniform(-100, 0),
-            NonNegativeInt: faker.pyint,
-            StrictInt: faker.pyint,
-            StrictBool: faker.pybool,
-            StrictBytes: partial(create_random_bytes, cls.__random__),
-            StrictFloat: faker.pyfloat,
-            StrictStr: faker.pystr,
-            DirectoryPath: lambda: _create_path().parent,
-            EmailStr: faker.free_email,
-            NameEmail: faker.free_email,
-            PyObject: lambda: "decimal.Decimal",
-            Color: faker.hex_color,
-            Json: faker.json,
-            PaymentCardNumber: faker.credit_card_number,
-            AnyUrl: faker.url,
-            AnyHttpUrl: faker.url,
-            HttpUrl: faker.url,
-            PostgresDsn: lambda: "postgresql://user:secret@localhost",
-            RedisDsn: lambda: "redis://localhost:6379",
-            UUID1: uuid1,
-            UUID3: lambda: uuid3(NAMESPACE_DNS, faker.pystr()),
-            UUID4: faker.uuid4,
-            UUID5: lambda: uuid5(NAMESPACE_DNS, faker.pystr()),
-            SecretBytes: partial(create_random_bytes, cls.__random__),
-            SecretStr: faker.pystr,
-            IPvAnyAddress: faker.ipv4,
-            IPvAnyInterface: faker.ipv4,
-            IPvAnyNetwork: lambda: faker.ipv4(network=True),
-            AmqpDsn: lambda: "amqps://",
-            KafkaDsn: lambda: "kafka://",
-            PastDate: faker.past_date,
-            FutureDate: faker.future_date,
-            Counter: lambda: Counter(faker.pystr()),
+            Counter: lambda: Counter(cls.__faker__.pystr()),
+            **_create_pydantic_type_map(cls),
         }
 
     @classmethod
-    def get_mock_value(cls, annotation: Type) -> Any:
+    def get_mock_value(cls, annotation: type) -> Any:
         """Return a mock value for a given type.
 
         :param annotation: An arbitrary type.
         :returns: An arbitrary value.
 
         """
 
@@ -496,18 +446,18 @@
             f"Unsupported type: {annotation!r}"
             f"\n\nEither extend the providers map or add a factory function for this type."
         )
 
     @classmethod
     def create_factory(
         cls,
-        model: Type,
-        bases: Optional[Tuple[Type["BaseFactory"], ...]] = None,
+        model: type,
+        bases: tuple[type["BaseFactory"], ...] | None = None,
         **kwargs: Any,
-    ) -> Type["BaseFactory"]:
+    ) -> type["BaseFactory"]:
         """Generate a factory for the given type dynamically.
 
         :param model: A type to model.
         :param bases: Base classes to use when generating the new class.
         :param kwargs: Any kwargs.
 
         :returns: A 'ModelFactory' subclass.
@@ -523,15 +473,15 @@
                 f"{model.__name__}Factory",
                 (*(bases or ()), cls),
                 {"__model__": model, **kwargs},
             ),
         )
 
     @classmethod
-    def get_field_value(cls, field_meta: "FieldMeta", field_build_parameters: Optional[Any] = None) -> Any:
+    def get_field_value(cls, field_meta: "FieldMeta", field_build_parameters: Any | None = None) -> Any:
         """Return a field value on the subclass if existing, otherwise returns a mock value.
 
         :param field_meta: FieldMeta instance.
         :param field_build_parameters: Any build parameters passed to the factory as kwarg values.
 
         :returns: An arbitrary value.
 
@@ -600,34 +550,34 @@
         :returns: A boolean determining whether a value should be set for the given field_meta.
 
         """
         return not field_meta.name.startswith("_") and field_meta.name not in kwargs
 
     @classmethod
     @abstractmethod
-    def get_model_fields(cls) -> List["FieldMeta"]:  # pragma: no cover
+    def get_model_fields(cls) -> list["FieldMeta"]:  # pragma: no cover
         """Retrieve a list of fields from the factory's model.
 
 
         :returns: A list of field MetaData instances.
 
         """
         raise NotImplementedError
 
     @classmethod
-    def process_kwargs(cls, **kwargs: Any) -> Dict[str, Any]:
+    def process_kwargs(cls, **kwargs: Any) -> dict[str, Any]:
         """Process the given kwargs and generate values for the factory's model.
 
         :param kwargs: Any build kwargs.
 
         :returns: A dictionary of build results.
 
         """
-        result: Dict[str, Any] = {**kwargs}
-        generate_post: Dict[str, PostGenerated] = {}
+        result: dict[str, Any] = {**kwargs}
+        generate_post: dict[str, PostGenerated] = {}
 
         for field_meta in cls.get_model_fields():
             field_build_parameters = cls.extract_field_build_parameters(field_meta=field_meta, build_args=kwargs)
             if cls.should_set_field_value(field_meta, **kwargs):
                 if hasattr(cls, field_meta.name) and field_meta.name in cls.__dict__:
                     field_value = getattr(cls, field_meta.name)
                     if isinstance(field_value, Ignore):
@@ -662,15 +612,15 @@
         :returns: An instance of type T.
 
         """
 
         return cast("T", cls.__model__(**cls.process_kwargs(**kwargs)))
 
     @classmethod
-    def batch(cls, size: int, **kwargs: Any) -> List[T]:
+    def batch(cls, size: int, **kwargs: Any) -> list[T]:
         """Build a batch of size n of the factory's Meta.model.
 
         :param size: Size of the batch.
         :param kwargs: Any kwargs. If field_meta names are set in kwargs, their values will be used.
 
         :returns: A list of instances of type T.
 
@@ -685,15 +635,15 @@
 
         :returns: An instance of type T.
 
         """
         return cls._get_sync_persistence().save(data=cls.build(**kwargs))
 
     @classmethod
-    def create_batch_sync(cls, size: int, **kwargs: Any) -> List[T]:
+    def create_batch_sync(cls, size: int, **kwargs: Any) -> list[T]:
         """Build and persists synchronously a batch of n size model instances.
 
         :param size: Size of the batch.
         :param kwargs: Any kwargs. If field_meta names are set in kwargs, their values will be used.
 
         :returns: A list of instances of type T.
 
@@ -707,98 +657,39 @@
         :param kwargs: Any kwargs. If field_meta names are set in kwargs, their values will be used.
 
         :returns: An instance of type T.
         """
         return await cls._get_async_persistence().save(data=cls.build(**kwargs))
 
     @classmethod
-    async def create_batch_async(cls, size: int, **kwargs: Any) -> List[T]:
+    async def create_batch_async(cls, size: int, **kwargs: Any) -> list[T]:
         """Build and persists asynchronously a batch of n size model instances.
 
 
         :param size: Size of the batch.
         :param kwargs: Any kwargs. If field_meta names are set in kwargs, their values will be used.
 
         :returns: A list of instances of type T.
         """
         return await cls._get_async_persistence().save_many(data=cls.batch(size, **kwargs))
 
 
-class DataclassFactory(Generic[T], BaseFactory[T]):
-    """Dataclass base factory"""
-
-    __is_base_factory__ = True
-
-    @classmethod
-    def is_supported_type(cls, value: Any) -> "TypeGuard[Type[T]]":
-        """Determine whether the given value is supported by the factory.
-
-        :param value: An arbitrary value.
-        :returns: A typeguard
-        """
-        try:
-            return isclass(value) and is_dataclass(value)
-        except (TypeError, AttributeError):  # pragma: no cover
-            return False
+def _register_builtin_factories() -> None:
+    """This function is used to register the base factories, if present.
 
-    @classmethod
-    def get_model_fields(cls) -> List["FieldMeta"]:
-        """Retrieve a list of fields from the factory's model.
-
-
-        :returns: A list of field MetaData instances.
-
-        """
-        fields_meta: List["FieldMeta"] = []
-
-        for field in fields(cls.__model__):  # type: ignore[arg-type]
-            if field.default_factory and field.default_factory is not MISSING:
-                default_value = field.default_factory()
-            elif field.default is not MISSING:
-                default_value = field.default
-            else:
-                default_value = Null
-
-            fields_meta.append(FieldMeta.from_type(annotation=field.type, name=field.name, default=default_value))
-
-        return fields_meta
-
-
-TypedDictT = TypeVar("TypedDictT", bound=_TypedDictMeta)
-
-
-class TypedDictFactory(Generic[TypedDictT], BaseFactory[TypedDictT]):
-    """TypedDict base factory"""
-
-    __is_base_factory__ = True
-
-    @classmethod
-    def is_supported_type(cls, value: Any) -> "TypeGuard[Type[TypedDictT]]":
-        """Determine whether the given value is supported by the factory.
+    :returns: None
+    """
+    import polyfactory.factories.dataclass_factory
+    import polyfactory.factories.typed_dict_factory  # noqa: F401
 
-        :param value: An arbitrary value.
-        :returns: A typeguard
-        """
+    for module in [
+        "polyfactory.factories.pydantic_factory",
+        "polyfactory.factories.beanie_odm_factory",
+        "polyfactory.factories.odmantic_odm_factory",
+    ]:
         try:
-            return is_typeddict(value)
-        except (TypeError, AttributeError):  # pragma: no cover
-            return False
+            import_module(module)
+        except ImportError:
+            continue
 
-    @classmethod
-    def get_model_fields(cls) -> List["FieldMeta"]:
-        """Retrieve a list of fields from the factory's model.
 
-
-        :returns: A list of field MetaData instances.
-
-        """
-        fields_meta: List["FieldMeta"] = []
-
-        for field_name, annotation in cls.__model__.__annotations__.items():
-            fields_meta.append(
-                FieldMeta.from_type(
-                    annotation=annotation,
-                    name=field_name,
-                    default=getattr(cls.__model__, field_name, Null),
-                )
-            )
-        return fields_meta
+_register_builtin_factories()
```

### Comparing `polyfactory-1.0.0a0/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-1.0.0a1/polyfactory/factories/beanie_odm_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import TYPE_CHECKING, Any, Generic, List, Optional, Type, TypeVar
+from __future__ import annotations
+from typing import TYPE_CHECKING, Any, Generic, TypeVar
 
 from typing_extensions import get_args
 
 from polyfactory.exceptions import MissingDependencyException
 from polyfactory.factories.pydantic_factory import ModelFactory
 from polyfactory.persistence import AsyncPersistenceProtocol
 from polyfactory.utils.predicates import is_safe_subclass
@@ -23,15 +24,15 @@
 class BeaniePersistenceHandler(Generic[T], AsyncPersistenceProtocol[T]):
     """Persistence Handler using beanie logic"""
 
     async def save(self, data: T) -> T:
         """Persist a single instance in mongoDB."""
         return await data.insert()  # type: ignore
 
-    async def save_many(self, data: List[T]) -> List[T]:
+    async def save_many(self, data: list[T]) -> list[T]:
         """Persist multiple instances in mongoDB.
 
         Note: we cannot use the .insert_many method from Beanie here because it doesn't return the created instances
         """
         result = []
         for doc in data:
             result.append(await doc.insert())  # pyright: ignore
@@ -41,24 +42,24 @@
 class BeanieDocumentFactory(Generic[T], ModelFactory[T]):
     """Base factory for Beanie Documents"""
 
     __async_persistence__ = BeaniePersistenceHandler
     __is_base_factory__ = True
 
     @classmethod
-    def is_supported_type(cls, value: Any) -> "TypeGuard[Type[T]]":
+    def is_supported_type(cls, value: Any) -> "TypeGuard[type[T]]":
         """Determine whether the given value is supported by the factory.
 
         :param value: An arbitrary value.
         :returns: A typeguard
         """
         return is_safe_subclass(value, Document)
 
     @classmethod
-    def get_field_value(cls, field_meta: "FieldMeta", field_build_parameters: Optional[Any] = None) -> Any:
+    def get_field_value(cls, field_meta: "FieldMeta", field_build_parameters: Any | None = None) -> Any:
         """Return a field value on the subclass if existing, otherwise returns a mock value.
 
         :param field_meta: FieldMeta instance.
         :param field_build_parameters: Any build parameters passed to the factory as kwarg values.
 
         :returns: An arbitrary value.
```

### Comparing `polyfactory-1.0.0a0/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-1.0.0a1/polyfactory/factories/odmantic_odm_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import TYPE_CHECKING, Any, Generic, Type, TypeVar, Union
+from __future__ import annotations
+from typing import TYPE_CHECKING, Any, Generic, TypeVar, Union
 
 from polyfactory.exceptions import MissingDependencyException
 from polyfactory.factories.pydantic_factory import ModelFactory
 from polyfactory.fields import Ignore
 from polyfactory.utils.predicates import is_safe_subclass
 
 try:
@@ -19,15 +20,15 @@
 
 class OdmanticModelFactory(Generic[T], ModelFactory[T]):
     """Base factory for odmantic models"""
 
     __is_base_factory__ = True
 
     @classmethod
-    def is_supported_type(cls, value: Any) -> "TypeGuard[Type[T]]":
+    def is_supported_type(cls, value: Any) -> "TypeGuard[type[T]]":
         """Determine whether the given value is supported by the factory.
 
         :param value: An arbitrary value.
         :returns: A typeguard
         """
         return is_safe_subclass(value, Model) or is_safe_subclass(value, EmbeddedModel)
```

### Comparing `polyfactory-1.0.0a0/polyfactory/factories/pydantic_factory.py` & `polyfactory-1.0.0a1/polyfactory/factories/pydantic_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
+from __future__ import annotations
 from contextlib import suppress
 from inspect import isclass
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Generic,
-    List,
     Mapping,
     Optional,
-    Type,
     TypeVar,
     cast,
 )
 
 from polyfactory.exceptions import MissingDependencyException
 from polyfactory.factories.base import BaseFactory
 from polyfactory.field_meta import FieldMeta, Null
@@ -51,15 +50,15 @@
     from decimal import Decimal
 
     from typing_extensions import TypeGuard
 
 T = TypeVar("T", bound=BaseModel)
 
 
-def is_pydantic_model(value: Any) -> "TypeGuard[Type[BaseModel]]":
+def is_pydantic_model(value: Any) -> "TypeGuard[type[BaseModel]]":
     """Determine whether the given value is a subclass of BaseModel.
 
     :param value: A value to test.
 
     :returns: A type guard.
 
     """
@@ -107,35 +106,35 @@
             constant=bool(model_field.field_info.const),
         )
 
 
 class ModelFactory(Generic[T], BaseFactory[T]):
     """Base factory for pydantic models"""
 
-    __forward_ref_resolution_type_mapping__: ClassVar[Mapping[str, Type]] = {}
+    __forward_ref_resolution_type_mapping__: ClassVar[Mapping[str, type]] = {}
     __is_base_factory__ = True
 
     def __init_subclass__(cls, *args: Any, **kwargs: Any) -> None:
         super().__init_subclass__(*args, **kwargs)
 
         if not cls.__is_base_factory__ and hasattr(cls.__model__, "update_forward_refs"):
             with suppress(NameError):  # pragma: no cover
                 cls.__model__.update_forward_refs(**cls.__forward_ref_resolution_type_mapping__)
 
     @classmethod
-    def is_supported_type(cls, value: Any) -> "TypeGuard[Type[T]]":
+    def is_supported_type(cls, value: Any) -> "TypeGuard[type[T]]":
         """Determine whether the given value is supported by the factory.
 
         :param value: An arbitrary value.
         :returns: A typeguard
         """
         return is_pydantic_model(value)
 
     @classmethod
-    def get_field_value(cls, field_meta: "FieldMeta", field_build_parameters: Optional[Any] = None) -> Any:
+    def get_field_value(cls, field_meta: "FieldMeta", field_build_parameters: Any | None = None) -> Any:
         """Return a field value on the subclass if existing, otherwise returns a mock value.
 
         :param field_meta: Field metadata.
         :param field_build_parameters: Any build parameters passed to the factory as kwarg values.
 
         :returns: An arbitrary value.
 
@@ -211,15 +210,15 @@
                 le=field_meta.annotation.le,
                 lt=field_meta.annotation.lt,
             )
 
         return super().get_field_value(field_meta=field_meta, field_build_parameters=field_build_parameters)
 
     @classmethod
-    def get_model_fields(cls) -> List["FieldMeta"]:
+    def get_model_fields(cls) -> list["FieldMeta"]:
         """Retrieve a list of fields from the factory's model.
 
 
         :returns: A list of field MetaData instances.
 
         """
         if not hasattr(cls, "_fields_metadata"):
```

### Comparing `polyfactory-1.0.0a0/polyfactory/field_meta.py` & `polyfactory-1.0.0a1/polyfactory/field_meta.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, List, Optional, Tuple, Type
+from __future__ import annotations
+from typing import Any
 
 from polyfactory.constants import TYPE_MAPPING
 from polyfactory.utils.helpers import unwrap_args, unwrap_new_type
 
 
 class Null:
     """Sentinel class for empty values"""
@@ -10,45 +11,45 @@
 
 class FieldMeta:
     """Factory field metadata container. This class is used to store the data about a field of a factory's model."""
 
     __slots__ = ("name", "annotation", "children", "default", "constant")
 
     annotation: Any
-    children: Optional[List["FieldMeta"]]
+    children: list[FieldMeta] | None
     constant: bool
     default: Any
     name: str
 
     def __init__(
         self,
         *,
         name: str,
-        annotation: Type,
+        annotation: type,
         default: Any = Null,
-        children: Optional[List["FieldMeta"]] = None,
+        children: list[FieldMeta] | None = None,
         constant: bool = False,
     ):
         """Create a factory field metadata instance."""
         self.annotation = annotation
         self.children = children
         self.default = default
         self.name = name
         self.constant = constant
 
     @property
-    def type_args(self) -> Tuple[Any, ...]:
+    def type_args(self) -> tuple[Any, ...]:
         """Return the normalized type args of the annotation, if any.
 
         :returns: a tuple of types.
         """
         return tuple(TYPE_MAPPING[arg] if arg in TYPE_MAPPING else arg for arg in unwrap_args(self.annotation))
 
     @classmethod
-    def from_type(cls, annotation: Any, name: str = "", default: Any = Null) -> "FieldMeta":
+    def from_type(cls, annotation: Any, name: str = "", default: Any = Null) -> FieldMeta:
         """Builder method to create a FieldMeta from a type annotation.
 
         :param annotation: A type annotation.
         :param name: Field name
         :param default: Default value, if any.
 
         :returns: A field meta instance.
```

### Comparing `polyfactory-1.0.0a0/polyfactory/fields.py` & `polyfactory-1.0.0a1/polyfactory/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Any, Callable, Dict, Generic, Optional, TypeVar, cast
+from __future__ import annotations
+from typing import Any, Callable, Generic, TypeVar, cast
 
 from typing_extensions import ParamSpec, TypedDict
 
 from polyfactory.exceptions import ParameterException
-from polyfactory.pytest_plugin import FactoryFixture
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
 class WrappedCallable(TypedDict):
     """A ref storing a callable. This class is a utility meant to prevent binding of methods."""
@@ -66,15 +66,15 @@
         :param args: Args for the callable.
         :param kwargs: Kwargs for the callable.
         """
         self.fn: WrappedCallable = {"value": fn}
         self.kwargs = kwargs
         self.args = args
 
-    def to_value(self, name: str, values: Dict[str, Any]) -> Any:
+    def to_value(self, name: str, values: dict[str, Any]) -> Any:
         """Invoke the post-generation callback passing to it the build results.
 
         :param name: Field name.
         :param values: Generated values.
 
         :returns: An arbitrary value.
         """
@@ -82,15 +82,15 @@
 
 
 class Fixture:
     """Factory field to create a pytest fixture from a factory."""
 
     __slots__ = ("fixture", "size", "kwargs")
 
-    def __init__(self, fixture: Callable, size: Optional[int] = None, **kwargs: Any) -> None:
+    def __init__(self, fixture: Callable, size: int | None = None, **kwargs: Any) -> None:
         """Create a fixture from a factory.
 
         :param fixture: A factory that was registered as a fixture.
         :param size: Optional batch size.
         :param kwargs: Any build kwargs.
         """
         self.fixture: WrappedCallable = {"value": fixture}
@@ -100,14 +100,15 @@
     def to_value(self) -> Any:
         """Call the factory's build or batch method.
 
         :raises: ParameterException
 
         :returns: The build result.
         """
+        from polyfactory.pytest_plugin import FactoryFixture
 
         if factory := FactoryFixture.factory_class_map.get(self.fixture["value"]):
             if self.size:
                 return factory.batch(self.size, **self.kwargs)
             return factory.build(**self.kwargs)
 
         raise ParameterException("fixture has not been registered using the register_factory decorator")
```

### Comparing `polyfactory-1.0.0a0/polyfactory/persistence.py` & `polyfactory-1.0.0a1/polyfactory/persistence.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# pylint: disable=unnecessary-ellipsis
-from typing import List, Protocol, TypeVar, runtime_checkable
+from __future__ import annotations
+from typing import Protocol, TypeVar, runtime_checkable
 
 T = TypeVar("T")
 
 
 @runtime_checkable
 class SyncPersistenceProtocol(Protocol[T]):
     """Protocol for sync persistence"""
@@ -14,15 +14,15 @@
         :param data: A single instance to persist.
 
         :returns: The persisted result.
 
         """
         ...
 
-    def save_many(self, data: List[T]) -> List[T]:
+    def save_many(self, data: list[T]) -> list[T]:
         """Persist multiple instances synchronously.
 
         :param data: A list of instances to persist.
 
         :returns: The persisted result
 
         """
@@ -38,15 +38,15 @@
 
         :param data: A single instance to persist.
 
         :returns: The persisted result.
         """
         ...
 
-    async def save_many(self, data: List[T]) -> List[T]:
+    async def save_many(self, data: list[T]) -> list[T]:
         """Persist multiple instances asynchronously.
 
         :param data: A list of instances to persist.
 
         :returns: The persisted result
         """
         ...
```

### Comparing `polyfactory-1.0.0a0/polyfactory/pytest_plugin.py` & `polyfactory-1.0.0a1/polyfactory/pytest_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
+from __future__ import annotations
 import re
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
-    Dict,
     Literal,
-    Optional,
-    Type,
     Union,
 )
 
 from pytest import fixture
 
 from polyfactory.exceptions import ParameterException
 
@@ -46,61 +44,60 @@
 
 
 class FactoryFixture:
     """Decorator that creates a pytest fixture from a factory"""
 
     __slots__ = ("scope", "autouse", "name")
 
-    factory_class_map: ClassVar[Dict[Callable, Type["BaseFactory"]]] = {}
+    factory_class_map: ClassVar[dict[Callable, type[BaseFactory]]] = {}
 
     def __init__(
         self,
-        scope: "Scope" = "function",
+        scope: Scope = "function",
         autouse: bool = False,
-        name: Optional[str] = None,
+        name: str | None = None,
     ):
         """Create a factory fixture decorator
 
         :param scope: Fixture scope
         :param autouse: Autouse the fixture
         :param name: Fixture name
         """
         self.scope = scope
         self.autouse = autouse
         self.name = name
 
-    def __call__(self, factory: Type["BaseFactory"]) -> Any:
+    def __call__(self, factory: type[BaseFactory]) -> Any:
         from polyfactory.factories.base import is_factory
 
         if not is_factory(factory):
             raise ParameterException(f"{factory.__name__} is not a BaseFactory subclass.")
 
         fixture_name = self.name or _get_fixture_name(factory.__name__)
         fixture_register = fixture(scope=self.scope, name=fixture_name, autouse=self.autouse)  # pyright: ignore
 
-        def _factory_fixture() -> Type["BaseFactory"]:
+        def _factory_fixture() -> type[BaseFactory]:
             """The wrapped factory"""
             return factory
 
         _factory_fixture.__doc__ = factory.__doc__
         marker = fixture_register(_factory_fixture)
         self.factory_class_map[marker] = factory
         return marker
 
 
 def register_fixture(
-    factory: Optional[Type["BaseFactory"]] = None,
+    factory: type[BaseFactory] | None = None,
     *,
-    scope: "Scope" = "function",
+    scope: Scope = "function",
     autouse: bool = False,
-    name: Optional[str] = None,
+    name: str | None = None,
 ) -> Any:
     """A decorator that allows registering model factories as fixtures.
 
-
     :param factory: An optional factory class to decorate.
     :param scope: Pytest scope.
     :param autouse: Auto use fixture.
     :param name: Fixture name.
 
     :returns: A fixture factory instance.
     """
```

### Comparing `polyfactory-1.0.0a0/polyfactory/utils/helpers.py` & `polyfactory-1.0.0a1/polyfactory/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Tuple, get_args
+from __future__ import annotations
+from typing import Any, get_args
 
 from polyfactory.utils.predicates import (
     is_annotated,
     is_new_type,
     is_optional_union,
     is_union,
 )
@@ -61,15 +62,15 @@
         elif is_annotated(annotation):
             annotation = get_args(annotation)[0]
         else:
             annotation = unwrap_union(annotation)
     return annotation
 
 
-def unwrap_args(annotation: Any) -> Tuple[Any, ...]:
+def unwrap_args(annotation: Any) -> tuple[Any, ...]:
     """Unwrap the annotation and return any type args.
 
     :param annotation: A type annotation
 
     :returns: A tuple of type args.
 
     """
```

### Comparing `polyfactory-1.0.0a0/polyfactory/utils/predicates.py` & `polyfactory-1.0.0a1/polyfactory/utils/predicates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
 import sys
 from inspect import isclass
-from typing import Any, Literal, NewType, Optional, Type, TypeVar, Union, get_args
+from typing import Any, Literal, NewType, Optional, TypeVar, Union, get_args
 
 from typing_extensions import (
     Annotated,
     NotRequired,
     ParamSpec,
     Required,
     TypeGuard,
@@ -22,15 +23,15 @@
     UNION_TYPES = {Union}
 
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
-def is_safe_subclass(annotation: Any, super_class: Type[T]) -> "TypeGuard[Type[T]]":
+def is_safe_subclass(annotation: Any, super_class: type[T]) -> "TypeGuard[type[T]]":
     """Determine whether a given annotation is a subclass of a give type
 
     :param annotation: A type annotation.
     :param super_class: A potential super class.
 
     :returns: A typeguard
     """
@@ -53,25 +54,25 @@
     return (
         annotation is Any
         or getattr(annotation, "_name", "") == "typing.Any"
         or (get_origin(annotation) in UNION_TYPES and Any in get_args(annotation))
     )
 
 
-def is_union(annotation: Any) -> "TypeGuard[Union[Any, Any]]":
+def is_union(annotation: Any) -> "TypeGuard[Any | Any]":
     """Determine whether a given annotation is 'typing.Union'.
 
     :param annotation: A type annotation.
 
     :returns: A typeguard.
     """
     return get_type_origin(annotation) in UNION_TYPES
 
 
-def is_optional_union(annotation: Any) -> "TypeGuard[Union[Any, None]]":
+def is_optional_union(annotation: Any) -> "TypeGuard[Any | None]":
     """Determine whether a given annotation is 'typing.Optional'.
 
     :param annotation: A type annotation.
 
     :returns: A typeguard.
     """
     origin = get_type_origin(annotation)
@@ -88,15 +89,15 @@
     return (
         get_type_origin(annotation) is Literal
         or repr(annotation).startswith("typing.Literal")
         or repr(annotation).startswith("typing_extensions.Literal")
     )
 
 
-def is_new_type(annotation: Any) -> "TypeGuard[Type[NewType]]":
+def is_new_type(annotation: Any) -> "TypeGuard[type[NewType]]":
     """Determine whether a given annotation is 'typing.NewType'.
 
     :param annotation: A type annotation.
 
     :returns: A typeguard.
     """
     return hasattr(annotation, "__supertype__")
```

### Comparing `polyfactory-1.0.0a0/polyfactory/value_generators/complex_types.py` & `polyfactory-1.0.0a1/polyfactory/value_generators/complex_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+from __future__ import annotations
 from collections import deque
-from typing import TYPE_CHECKING, Any, MutableMapping, Tuple, Type
+from typing import TYPE_CHECKING, Any, MutableMapping, Tuple
 
 from typing_extensions import is_typeddict
 
 from polyfactory.constants import TYPE_MAPPING
 from polyfactory.field_meta import FieldMeta
 from polyfactory.utils.helpers import unwrap_annotation, unwrap_args
 from polyfactory.utils.predicates import get_type_origin, is_any, is_union
 from polyfactory.value_generators.primitives import create_random_string
 
 if TYPE_CHECKING:
     from polyfactory.factories.base import BaseFactory
 
 
 def handle_container_type(
-    container_type: Type,
-    factory: Type["BaseFactory"],
-    field_meta: "FieldMeta",
+    container_type: type,
+    factory: type[BaseFactory],
+    field_meta: FieldMeta,
 ) -> Any:
     """Handle generation of container types recursively.
 
     :param container_type: A type that can accept type arguments.
     :param factory: A factory.
     :param field_meta: A field meta instance.
 
@@ -52,16 +53,16 @@
                 )
             )
 
     return container if container_type is not frozenset else container_type(*container)
 
 
 def handle_complex_type(
-    factory: Type["BaseFactory"],
-    field_meta: "FieldMeta",
+    factory: type[BaseFactory],
+    field_meta: FieldMeta,
 ) -> Any:
     """Recursive type generation based on typing info stored in the graph like structure of pydantic field_metas.
 
     :param factory: A factory.
     :param field_meta: A field meta instance.
 
     :returns: A built result.
```

### Comparing `polyfactory-1.0.0a0/polyfactory/value_generators/constrained_collections.py` & `polyfactory-1.0.0a1/polyfactory/value_generators/constrained_collections.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,26 @@
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    List,
-    Optional,
-    Set,
-    Type,
-    TypeVar,
-    Union,
-)
+from __future__ import annotations
+from typing import TYPE_CHECKING, Any, Callable, TypeVar
 
 from polyfactory.exceptions import ParameterException
 
 if TYPE_CHECKING:
     from polyfactory.factories.base import BaseFactory
     from polyfactory.field_meta import FieldMeta
 
 T = TypeVar("T", list, set, frozenset)
 
 
 def handle_constrained_collection(
     collection_type: Callable[..., T],
-    factory: Type["BaseFactory"],
-    field_meta: "FieldMeta",
+    factory: type[BaseFactory],
+    field_meta: FieldMeta,
     item_type: Any,
-    max_items: Optional[int] = None,
-    min_items: Optional[int] = None,
+    max_items: int | None = None,
+    min_items: int | None = None,
     unique_items: bool = False,
 ) -> T:
     """Generate a constrained list or set.
 
     :param collection_type: A type that can accept type arguments.
     :param factory: A factory.
     :param field_meta: A field meta instance.
@@ -42,15 +33,15 @@
     """
     min_items = min_items if min_items is not None else (max_items or 0)
     max_items = max_items if max_items is not None else min_items + 1
 
     if max_items < min_items:
         raise ParameterException("max_items must be larger or equal to min_items")
 
-    collection: Union[Set[T], List[T]] = set() if collection_type in (frozenset, set) or unique_items else []
+    collection: set[T] | list[T] = set() if collection_type in (frozenset, set) or unique_items else []
 
     try:
         while len(collection) < factory.__random__.randint(min_items, max_items):
             value = factory.get_field_value(field_meta)
             if isinstance(collection, set):
                 collection.add(value)
             else:
```

### Comparing `polyfactory-1.0.0a0/polyfactory/value_generators/constrained_dates.py` & `polyfactory-1.0.0a1/polyfactory/value_generators/constrained_dates.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from __future__ import annotations
 from datetime import date, timedelta, datetime, timezone
-from typing import TYPE_CHECKING, Optional, cast
+from typing import TYPE_CHECKING, cast
 
 
 if TYPE_CHECKING:
     from faker import Faker
 
 
 def handle_constrained_date(
-    faker: "Faker",
-    ge: Optional[date] = None,
-    gt: Optional[date] = None,
-    le: Optional[date] = None,
-    lt: Optional[date] = None,
+    faker: Faker,
+    ge: date | None = None,
+    gt: date | None = None,
+    le: date | None = None,
+    lt: date | None = None,
 ) -> date:
     """Generates a date value fulfilling the expected constraints.
 
     :param faker: An instance of faker.
     :param lt: Less than value.
     :param le: Less than or equal value.
     :param gt: Greater than value.
```

### Comparing `polyfactory-1.0.0a0/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-1.0.0a1/polyfactory/value_generators/constrained_numbers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,26 @@
-# pylint: disable=unnecessary-ellipsis
+from __future__ import annotations
 from decimal import Decimal
 from sys import float_info
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Dict,
-    Optional,
-    Protocol,
-    Tuple,
-    Type,
-    TypeVar,
-    cast,
-)
+from typing import TYPE_CHECKING, Any, Protocol, TypeVar, cast
 
 from polyfactory.exceptions import ParameterException
-from polyfactory.value_generators.primitives import (
-    create_random_decimal,
-    create_random_float,
-    create_random_integer,
-)
+from polyfactory.value_generators.primitives import create_random_decimal, create_random_float, create_random_integer
 
 if TYPE_CHECKING:
     from random import Random
 
 
 T = TypeVar("T", Decimal, int, float)
 
 
 class NumberGeneratorProtocol(Protocol[T]):
     """Protocol for custom callables used to generate numerical values"""
 
-    def __call__(self, random: "Random", minimum: Optional[T] = None, maximum: Optional[T] = None) -> T:
+    def __call__(self, random: "Random", minimum: T | None = None, maximum: T | None = None) -> T:
         """Signature of the callable.
 
         :param random: An instance of random.
         :param minimum: A minimum value.
         :param maximum: A maximum value.
         :return: The generated numeric value.
         """
@@ -124,30 +110,30 @@
     """
     if multiple_of == 0:
         return True
     mod = float(value) / float(multiple_of) % 1
     return almost_equal_floats(mod, 0.0) or almost_equal_floats(mod, 1.0)
 
 
-def get_increment(t_type: Type[T]) -> T:
+def get_increment(t_type: type[T]) -> T:
     """Get a small increment base to add to constrained values, i.e. lt/gt entries.
 
     :param t_type: A value of type T.
 
     :returns: An increment T.
     """
-    values: Dict[Any, Any] = {
+    values: dict[Any, Any] = {
         int: 1,
         float: float_info.epsilon,
         Decimal: Decimal("0.001"),
     }
     return cast("T", values[t_type])
 
 
-def get_value_or_none(equal_value: Optional[T], constrained: Optional[T], increment: T) -> Optional[T]:
+def get_value_or_none(equal_value: T | None, constrained: T | None, increment: T) -> T | None:
     """Return an optional value.
 
     :param equal_value: An GE/LE value.
     :param constrained: An GT/LT value.
     :param increment: increment
 
     :returns: Optional T.
@@ -156,22 +142,22 @@
         return equal_value
     if constrained is not None:
         return constrained + increment
     return None
 
 
 def get_constrained_number_range(
-    t_type: Type[T],
-    random: "Random",
-    lt: Optional[T] = None,
-    le: Optional[T] = None,
-    gt: Optional[T] = None,
-    ge: Optional[T] = None,
-    multiple_of: Optional[T] = None,
-) -> Tuple[Optional[T], Optional[T]]:
+    t_type: type[T],
+    random: Random,
+    lt: T | None = None,
+    le: T | None = None,
+    gt: T | None = None,
+    ge: T | None = None,
+    multiple_of: T | None = None,
+) -> tuple[T | None, T | None]:
     """Return the minimum and maximum values given a field_meta's constraints.
 
     :param t_type: A primitive constructor - int, float or Decimal.
     :param random: An instance of Random.
     :param lt: Less than value.
     :param le: Less than or equal value.
     :param gt: Greater than value.
@@ -204,18 +190,18 @@
         ):
             raise ParameterException("given range should include at least one multiply of multiple_of")
 
     return minimum, maximum
 
 
 def generate_constrained_number(
-    random: "Random",
-    minimum: Optional[T],
-    maximum: Optional[T],
-    multiple_of: Optional[T],
+    random: Random,
+    minimum: T | None,
+    maximum: T | None,
+    multiple_of: T | None,
     method: "NumberGeneratorProtocol[T]",
 ) -> T:
     """Generate a constrained number, output depends on the passed in callbacks.
 
     :param random: An instance of random.
     :param minimum: A minimum value.
     :param maximum: A maximum value.
@@ -235,20 +221,20 @@
         return result
     if multiple_of is not None:
         return multiple_of
     return method(random=random)
 
 
 def handle_constrained_int(
-    random: "Random",
-    multiple_of: Optional[int] = None,
-    gt: Optional[int] = None,
-    ge: Optional[int] = None,
-    lt: Optional[int] = None,
-    le: Optional[int] = None,
+    random: Random,
+    multiple_of: int | None = None,
+    gt: int | None = None,
+    ge: int | None = None,
+    lt: int | None = None,
+    le: int | None = None,
 ) -> int:
     """Handle constrained integers.
 
     :param random: An instance of Random.
     :param lt: Less than value.
     :param le: Less than or equal value.
     :param gt: Greater than value.
@@ -268,20 +254,20 @@
         maximum=maximum,
         multiple_of=multiple_of,
         method=create_random_integer,
     )
 
 
 def handle_constrained_float(
-    random: "Random",
-    multiple_of: Optional[float] = None,
-    gt: Optional[float] = None,
-    ge: Optional[float] = None,
-    lt: Optional[float] = None,
-    le: Optional[float] = None,
+    random: Random,
+    multiple_of: float | None = None,
+    gt: float | None = None,
+    ge: float | None = None,
+    lt: float | None = None,
+    le: float | None = None,
 ) -> float:
     """Handle constrained floats.
 
     :param random: An instance of Random.
     :param lt: Less than value.
     :param le: Less than or equal value.
     :param gt: Greater than value.
@@ -302,16 +288,16 @@
         multiple_of=multiple_of,
         method=create_random_float,
     )
 
 
 def validate_max_digits(
     max_digits: int,
-    minimum: Optional[Decimal],
-    decimal_places: Optional[int],
+    minimum: Decimal | None,
+    decimal_places: int | None,
 ) -> None:
     """Validate that max digits is greater than minimum and decimal places.
 
     :param max_digits: The maximal number of digits for the decimal.
     :param minimum: Minimal value.
     :param decimal_places: Number of decimal places
 
@@ -329,16 +315,16 @@
 
     if decimal_places is not None and max_digits <= decimal_places:
         raise ParameterException("max_digits must be greater than decimal places")
 
 
 def handle_decimal_length(
     generated_decimal: Decimal,
-    decimal_places: Optional[int],
-    max_digits: Optional[int],
+    decimal_places: int | None,
+    max_digits: int | None,
 ) -> Decimal:
     """Handle the length of the decimal.
 
     :param generated_decimal: A decimal value.
     :param decimal_places: Number of decimal places.
     :param max_digits: Maximal number of digits.
 
@@ -365,22 +351,22 @@
         return Decimal(sign + whole_numbers[:max_decimals])
 
     decimals = decimals[:max_decimals]
     return Decimal(sign + whole_numbers + "." + decimals[:decimal_places])
 
 
 def handle_constrained_decimal(
-    random: "Random",
-    multiple_of: Optional[Decimal] = None,
-    decimal_places: Optional[int] = None,
-    max_digits: Optional[int] = None,
-    gt: Optional[Decimal] = None,
-    ge: Optional[Decimal] = None,
-    lt: Optional[Decimal] = None,
-    le: Optional[Decimal] = None,
+    random: Random,
+    multiple_of: Decimal | None = None,
+    decimal_places: int | None = None,
+    max_digits: int | None = None,
+    gt: Decimal | None = None,
+    ge: Decimal | None = None,
+    lt: Decimal | None = None,
+    le: Decimal | None = None,
 ) -> Decimal:
     """Handle a constrained decimal.
 
     :param random: An instance of Random.
     :param multiple_of: Multiple of value.
     :param decimal_places: Number of decimal places.
     :param max_digits: Maximal number of digits.
```

### Comparing `polyfactory-1.0.0a0/polyfactory/value_generators/constrained_strings.py` & `polyfactory-1.0.0a1/polyfactory/value_generators/constrained_strings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from typing import TYPE_CHECKING, Callable, Optional, Pattern, TypeVar, Union, cast
+from __future__ import annotations
+from typing import TYPE_CHECKING, Callable, Pattern, TypeVar, Union, cast
 
 from polyfactory.exceptions import ParameterException
 from polyfactory.value_generators.primitives import create_random_bytes, create_random_string
 from polyfactory.value_generators.regex import RegexFactory
 
 T = TypeVar("T", bound=Union[bytes, str])
 
 if TYPE_CHECKING:
     from random import Random
 
 
 def _validate_length(
-    min_length: Optional[int] = None,
-    max_length: Optional[int] = None,
+    min_length: int | None = None,
+    max_length: int | None = None,
 ) -> None:
     """Validate the length parameters make sense.
 
     :param min_length: Minimum length.
     :param max_length: Maximum length.
 
     :raises: ParameterException.
@@ -30,20 +31,20 @@
         raise ParameterException("max_length must be greater or equal to 0")
 
     if max_length is not None and min_length is not None and max_length < min_length:
         raise ParameterException("max_length must be greater than min_length")
 
 
 def _generate_pattern(
-    random: "Random",
-    pattern: Union[str, Pattern],
+    random: Random,
+    pattern: str | Pattern,
     lower_case: bool = False,
     upper_case: bool = False,
-    min_length: Optional[int] = None,
-    max_length: Optional[int] = None,
+    min_length: int | None = None,
+    max_length: int | None = None,
 ) -> str:
     """Generate a regex.
 
     :param random: An instance of random.
     :param pattern: A regex or string pattern.
     :param lower_case: Whether to lowercase the result.
     :param upper_case: Whether to uppercase the result.
@@ -67,21 +68,21 @@
     if upper_case:
         result = result.upper()
 
     return result
 
 
 def handle_constrained_string_or_bytes(
-    random: "Random",
+    random: Random,
     t_type: Callable[[], T],
     lower_case: bool = False,
     upper_case: bool = False,
-    min_length: Optional[int] = None,
-    max_length: Optional[int] = None,
-    pattern: Optional[Union[str, Pattern]] = None,
+    min_length: int | None = None,
+    max_length: int | None = None,
+    pattern: str | Pattern | None = None,
 ) -> T:
     """Handle constrained string or bytes, for example - pydantic `constr` or `conbytes`.
 
     :param random: An instance of random.
     :param t_type: A type (str or bytes)
     :param lower_case: Whether to lowercase the result.
     :param upper_case: Whether to uppercase the result.
```

### Comparing `polyfactory-1.0.0a0/polyfactory/value_generators/primitives.py` & `polyfactory-1.0.0a1/polyfactory/value_generators/primitives.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from __future__ import annotations
 from binascii import hexlify
 from decimal import Decimal
 from os import urandom
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from random import Random
 
 
 def create_random_float(
-    random: "Random",
-    minimum: Optional[Union[Decimal, int, float]] = None,
-    maximum: Optional[Union[Decimal, int, float]] = None,
+    random: Random,
+    minimum: Decimal | int | float | None = None,
+    maximum: Decimal | int | float | None = None,
 ) -> float:
     """Generate a random float given the constraints.
 
     :param random: An instance of random.
     :param minimum: A minimum value
     :param maximum: A maximum value.
 
@@ -23,46 +24,46 @@
     if minimum is None:
         minimum = float(random.randint(0, 100)) if maximum is None else float(maximum) - 100.0
     if maximum is None:
         maximum = float(minimum) + 1.0 * 2.0 if minimum >= 0 else float(minimum) + 1.0 / 2.0
     return random.uniform(float(minimum), float(maximum))
 
 
-def create_random_integer(random: "Random", minimum: Optional[int] = None, maximum: Optional[int] = None) -> int:
+def create_random_integer(random: Random, minimum: int | None = None, maximum: int | None = None) -> int:
     """Generate a random int given the constraints.
 
     :param random: An instance of random.
     :param minimum: A minimum value
     :param maximum: A maximum value.
 
     :returns: A random integer.
     """
     return int(create_random_float(random=random, minimum=minimum, maximum=maximum))
 
 
 def create_random_decimal(
-    random: "Random",
-    minimum: Optional[Decimal] = None,
-    maximum: Optional[Decimal] = None,
+    random: Random,
+    minimum: Decimal | None = None,
+    maximum: Decimal | None = None,
 ) -> Decimal:
     """Generate a random Decimal given the constraints.
 
     :param random: An instance of random.
     :param minimum: A minimum value
     :param maximum: A maximum value.
 
     :returns: A random decimal.
     """
     return Decimal(str(create_random_float(random=random, minimum=minimum, maximum=maximum)))
 
 
 def create_random_bytes(
-    random: "Random",
-    min_length: Optional[int] = None,
-    max_length: Optional[int] = None,
+    random: Random,
+    min_length: int | None = None,
+    max_length: int | None = None,
     lower_case: bool = False,
     upper_case: bool = False,
 ) -> bytes:
     """Generate a random bytes given the constraints.
 
     :param random: An instance of random.
     :param min_length: A minimum length.
@@ -89,17 +90,17 @@
         end = random.randint(min_length or 0, max_length)
         return result[0:end]
 
     return result
 
 
 def create_random_string(
-    random: "Random",
-    min_length: Optional[int] = None,
-    max_length: Optional[int] = None,
+    random: Random,
+    min_length: int | None = None,
+    max_length: int | None = None,
     lower_case: bool = False,
     upper_case: bool = False,
 ) -> str:
     """Generate a random string given the constraints.
 
     :param random: An instance of random.
     :param min_length: A minimum length.
@@ -114,15 +115,15 @@
         min_length=min_length,
         max_length=max_length,
         lower_case=lower_case,
         upper_case=upper_case,
     ).decode("utf-8")
 
 
-def create_random_boolean(random: "Random") -> bool:
+def create_random_boolean(random: Random) -> bool:
     """Generate a random boolean value.
 
     :param random: An instance of random.
 
     :returns: A random boolean.
     """
     return bool(random.getrandbits(1))
```

### Comparing `polyfactory-1.0.0a0/polyfactory/value_generators/regex.py` & `polyfactory-1.0.0a1/polyfactory/value_generators/regex.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,26 +25,26 @@
 CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
-
+from __future__ import annotations
 from itertools import chain
 from string import (
     ascii_letters,
     ascii_lowercase,
     ascii_uppercase,
     digits,
     printable,
     punctuation,
     whitespace,
 )
-from typing import TYPE_CHECKING, Any, Dict, List, Pattern, Tuple, Union
+from typing import TYPE_CHECKING, Any, Pattern
 
 try:  # >=3.11
     from re._parser import SubPattern, parse  # pyright:ignore
 except ImportError:  # < 3.11
     from sre_parse import SubPattern, parse  # pylint: disable=deprecated-module
 
 if TYPE_CHECKING:
@@ -78,18 +78,18 @@
     "category_not_word": _alphabets["nonword"],
 }
 
 
 class RegexFactory:
     """Factory for regexes."""
 
-    def __init__(self, random: "Random", limit: int = 10) -> None:
+    def __init__(self, random: Random, limit: int = 10) -> None:
         """Create a RegexFactory"""
         self._limit = limit
-        self._cache: Dict[str, Any] = {}
+        self._cache: dict[str, Any] = {}
         self._random = random
 
         self._cases = {
             "literal": chr,
             "not_literal": lambda x: self._random.choice(printable.replace(chr(x), "")),
             "at": lambda x: "",
             "in": self._handle_in,
@@ -102,15 +102,15 @@
             "assert_not": lambda x: "",
             "groupref": lambda x: self._cache[x],
             "min_repeat": lambda x: self._handle_repeat(*x),
             "max_repeat": lambda x: self._handle_repeat(*x),
             "negate": lambda x: [False],
         }
 
-    def __call__(self, string_or_regex: Union[str, Pattern]) -> str:
+    def __call__(self, string_or_regex: str | Pattern) -> str:
         """Generate a string matching a regex.
 
         :param string_or_regex: A string or pattern.
 
         :return: The generated string.
         """
         pattern = string_or_regex.pattern if isinstance(string_or_regex, Pattern) else string_or_regex
@@ -118,32 +118,32 @@
         result = self._build_string(parsed)
         self._cache.clear()
         return result
 
     def _build_string(self, parsed: SubPattern) -> str:
         return "".join([self._handle_state(state) for state in parsed])  # pyright:ignore
 
-    def _handle_state(self, state: Tuple[SubPattern, Tuple[Any, ...]]) -> Any:
+    def _handle_state(self, state: tuple[SubPattern, tuple[Any, ...]]) -> Any:
         opcode, value = state
         return self._cases[str(opcode).lower()](value)  # type: ignore[no-untyped-call]
 
-    def _handle_group(self, value: Tuple[Any, ...]) -> str:
+    def _handle_group(self, value: tuple[Any, ...]) -> str:
         result = "".join(self._handle_state(i) for i in value[3])
         if value[0]:
             self._cache[value[0]] = result
         return result
 
-    def _handle_in(self, value: Tuple[Any, ...]) -> Any:
+    def _handle_in(self, value: tuple[Any, ...]) -> Any:
         candidates = list(chain(*(self._handle_state(i) for i in value)))
         if candidates and candidates[0] is False:
             candidates = list(set(printable).difference(candidates[1:]))
             return self._random.choice(candidates)
         return self._random.choice(candidates)
 
     def _handle_repeat(self, start_range: int, end_range: Any, value: SubPattern) -> str:
-        result: List[str] = []
+        result: list[str] = []
         end_range = min(end_range, self._limit)
 
         for i in range(self._random.randint(start_range, max(start_range, end_range))):
             result.append("".join(self._handle_state(i) for i in list(value)))  # pyright:ignore
 
         return "".join(result)
```

### Comparing `polyfactory-1.0.0a0/pyproject.toml` & `polyfactory-1.0.0a1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 [tool.poetry]
 name = "polyfactory"
-version = "1.0.0alpha0"
-description = "Mock data generation for pydantic based models and python dataclasses"
+version = "1.0.0alpha1"
+description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
 ]
 maintainers = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
 ]
 license = "MIT"
 readme = "README.md"
-homepage = "https://github.com/starlite-api/polyfactory"
-repository = "https://github.com/starlite-api/polyfactory"
-documentation = "https://github.com/starlite-api/polyfactory"
+homepage = "https://github.com/litestar-org/polyfactory"
+repository = "https://github.com/litestar-org/polyfactory"
+documentation = "https://github.com/litestar-org/polyfactory"
 keywords = [
     "dataclasses",
     "factory",
     "faker",
     "mock",
     "pydantic",
     "pytest",
-    "starlite",
+    "litestar",
     "tdd",
     "testing",
+    "typeddict",
 ]
 classifiers = [
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Framework :: Pytest",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
-    "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Topic :: Software Development",
+    "Programming Language :: Python",
     "Topic :: Software Development :: Libraries",
-    "Topic :: Software Development :: Testing",
     "Topic :: Software Development :: Testing :: Unit",
+    "Topic :: Software Development :: Testing",
+    "Topic :: Software Development",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 packages = [
     { include = "polyfactory" },
 ]
 
@@ -69,27 +71,39 @@
 pre-commit = "*"
 pydantic = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 mongomock-motor = "*"
 
+
+[tool.poetry.group.docs.dependencies]
+sphinx-autobuild = "*"
+blacken-docs = "*"
+auto-pytabs = "*"
+sphinxcontrib-mermaid = "*"
+sphinx-copybutton = "*"
+sphinx = "*"
+litestar-sphinx-theme = { git = "https://github.com/litestar-org/litestar-sphinx-theme.git" }
+
 [tool.poetry.extras]
 pydantic = ["pydantic"]
 odmantic = ["odmantic", "pydantic"]
 beanie = ["beanie", "pydantic"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 include = '\.pyi?$'
 
+[tool.pyright]
+include = ["polyfactory", "tests", "examples"]
 
 [tool.coverage.run]
 omit = ["*/tests/*"]
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
@@ -152,15 +166,15 @@
     "D205", # pydocstyle - 1 blank line required between summary line and description
     "D415", # pydocstyle - first line should end with a period, question mark, or exclamation point
     "E501", # pycodestyle line too long, handled by black
     "N818", # pep8-naming - exception name should be named with an Error suffix
     "UP037", # pyupgrade - removes quotes from type annotation
 ]
 line-length = 120
-src = ["polyfactory", "tests"]
+src = ["polyfactory", "tests", "docs/examples"]
 target-version = "py38"
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.pep8-naming]
 classmethod-decorators = [
@@ -172,8 +186,8 @@
 
 [tool.ruff.isort]
 known-first-party = ["polyfactory", "tests"]
 
 [tool.ruff.per-file-ignores]
 "tests/**/*.*" = ["S101", "D", "ARG", "PGH", "B", "FBT", "PTH", "A", "TCH", "DTZ", "TRY", "EM", "S", "N", "SIM", "PLR", "BLE", "RSE", "C901", "PLW", "G", "PIE"]
 "docs/examples/tests/**/*.*" = ["S101", "D", "ARG", "PGH", "B", "FBT", "PTH", "A", "TCH", "DTZ", "TRY", "EM", "S", "N", "SIM", "PLR", "BLE", "RSE", "C901", "PLW", "G", "PIE"]
-"docs/**/*.*" = ["S", "B", "DTZ", "A", "TCH", "ERA", "D", "RET"]
+"docs/**/*.*" = ["S", "B", "DTZ", "A", "TCH", "ERA", "D", "RET", "E731"]
```

