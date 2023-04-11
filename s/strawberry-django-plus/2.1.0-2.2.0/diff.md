# Comparing `tmp/strawberry_django_plus-2.1.0.tar.gz` & `tmp/strawberry_django_plus-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-2.1.0.tar", max compression
+gzip compressed data, was "strawberry_django_plus-2.2.0.tar", max compression
```

## Comparing `strawberry_django_plus-2.1.0.tar` & `strawberry_django_plus-2.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1077 2023-04-03 19:37:11.223132 strawberry_django_plus-2.1.0/LICENSE
--rw-r--r--   0        0        0     3299 2023-04-03 19:37:11.223132 strawberry_django_plus-2.1.0/README.md
--rw-r--r--   0        0        0     4162 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     2950 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5554 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5751 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    25354 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3069 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1641 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1389 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     1939 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1168 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0     6287 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/middlewares/debug_toolbar.py
--rw-r--r--   0        0        0        0 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    24686 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14819 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    24007 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1372 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    27509 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0    45263 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1107 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0     1445 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
--rw-r--r--   0        0        0        0 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2337 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    16932 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/type.py
--rw-r--r--   0        0        0    10174 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6924 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    12426 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     5865 2023-04-03 19:37:11.227132 strawberry_django_plus-2.1.0/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    13406 2023-04-03 19:37:11.231132 strawberry_django_plus-2.1.0/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0      938 2023-04-03 19:37:11.231132 strawberry_django_plus-2.1.0/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     5169 1970-01-01 00:00:00.000000 strawberry_django_plus-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/LICENSE
+-rw-r--r--   0        0        0     3299 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/README.md
+-rw-r--r--   0        0        0     4162 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2950 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5554 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5751 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    26052 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3069 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1641 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1389 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     1939 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1168 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0     6287 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/middlewares/debug_toolbar.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    25024 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14819 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    24443 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1372 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    27509 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0    45970 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1107 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0     1445 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
+-rw-r--r--   0        0        0        0 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2337 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    16988 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0    10174 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6924 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    12426 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     5865 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    13406 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0      938 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     5169 1970-01-01 00:00:00.000000 strawberry_django_plus-2.2.0/PKG-INFO
```

### Comparing `strawberry_django_plus-2.1.0/LICENSE` & `strawberry_django_plus-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/README.md` & `strawberry_django_plus-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/pyproject.toml` & `strawberry_django_plus-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "2.1.0"
+version = "2.2.0"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
```

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/__init__.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/descriptors.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/directives.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/field.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/field.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,23 +26,26 @@
     ReverseManyToOneDescriptor,
     ReverseOneToOneDescriptor,
 )
 from django.db.models.query_utils import DeferredAttribute
 from strawberry import UNSET
 from strawberry.annotation import StrawberryAnnotation
 from strawberry.arguments import StrawberryArgument
+from strawberry.extensions.field_extension import FieldExtension
 from strawberry.lazy_type import LazyType
 from strawberry.permission import BasePermission
 from strawberry.type import StrawberryContainer, StrawberryType
 from strawberry.types.fields.resolver import StrawberryResolver
 from strawberry.types.info import Info
 from strawberry.types.types import TypeDefinition
 from strawberry.union import StrawberryUnion
 from strawberry_django.arguments import argument
-from strawberry_django.fields.field import StrawberryDjangoField as _StrawberryDjangoField
+from strawberry_django.fields.field import (
+    StrawberryDjangoField as _StrawberryDjangoField,
+)
 from strawberry_django.utils import get_django_model, unwrap_type
 
 from . import optimizer, relay
 from .descriptors import ModelProperty
 from .permissions import filter_with_perms
 from .utils import resolvers
 from .utils.typing import TypeOrSequence
@@ -355,14 +358,15 @@
     pagination: Optional[bool] = UNSET,
     filters: Optional[type] = UNSET,
     order: Optional[type] = UNSET,
     only: Optional[TypeOrSequence[str]] = None,
     select_related: Optional[TypeOrSequence[str]] = None,
     prefetch_related: Optional[TypeOrSequence[optimizer.PrefetchType]] = None,
     disable_optimization: bool = False,
+    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> _T:
     ...
 
 
 @overload
 def field(
     *,
@@ -381,14 +385,15 @@
     pagination: Optional[bool] = UNSET,
     filters: Optional[type] = UNSET,
     order: Optional[type] = UNSET,
     only: Optional[TypeOrSequence[str]] = None,
     select_related: Optional[TypeOrSequence[str]] = None,
     prefetch_related: Optional[TypeOrSequence[optimizer.PrefetchType]] = None,
     disable_optimization: bool = False,
+    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> Any:
     ...
 
 
 @overload
 def field(
     resolver: Union[StrawberryResolver, Callable, staticmethod, classmethod],
@@ -407,14 +412,15 @@
     pagination: Optional[bool] = UNSET,
     filters: Optional[type] = UNSET,
     order: Optional[type] = UNSET,
     only: Optional[TypeOrSequence[str]] = None,
     select_related: Optional[TypeOrSequence[str]] = None,
     prefetch_related: Optional[TypeOrSequence[optimizer.PrefetchType]] = None,
     disable_optimization: bool = False,
+    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> StrawberryDjangoField:
     ...
 
 
 def field(
     resolver=None,
     *,
@@ -432,14 +438,15 @@
     pagination: Optional[bool] = UNSET,
     filters: Optional[type] = UNSET,
     order: Optional[type] = UNSET,
     only: Optional[TypeOrSequence[str]] = None,
     select_related: Optional[TypeOrSequence[str]] = None,
     prefetch_related: Optional[TypeOrSequence[optimizer.PrefetchType]] = None,
     disable_optimization: bool = False,
+    extensions: List[FieldExtension] = (),  # type: ignore
     # This init parameter is used by pyright to determine whether this field
     # is added in the constructor or not. It is not used to change
     # any behavior at the moment.
     init: Literal[True, False, None] = None,
 ) -> Any:
     """Annotate a method or property as a Django GraphQL field.
 
@@ -471,14 +478,15 @@
         filters=filters,
         pagination=pagination,
         order=order,
         only=only,
         select_related=select_related,
         prefetch_related=prefetch_related,
         disable_optimization=disable_optimization,
+        extensions=extensions,
     )
 
     if resolver:
         return f(resolver)
 
     return f
 
@@ -495,14 +503,15 @@
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
     only: Optional[TypeOrSequence[str]] = None,
     select_related: Optional[TypeOrSequence[str]] = None,
     prefetch_related: Optional[TypeOrSequence[optimizer.PrefetchType]] = None,
     disable_optimization: bool = False,
+    extensions: List[FieldExtension] = (),  # type: ignore
     # This init parameter is used by pyright to determine whether this field
     # is added in the constructor or not. It is not used to change
     # any behavior at the moment.
     init: Literal[True, False, None] = None,
 ) -> Any:
     """Annotate a property to create a relay query field.
 
@@ -537,14 +546,15 @@
         default_factory=default_factory,
         metadata=metadata,
         directives=directives or (),
         only=only,
         select_related=select_related,
         prefetch_related=prefetch_related,
         disable_optimization=disable_optimization,
+        extensions=extensions,
     )
 
 
 @overload
 def connection(
     *,
     resolver: Callable[[], _T],
@@ -561,14 +571,15 @@
     graphql_type: Optional[Any] = None,
     filters: Optional[type] = UNSET,
     order: Optional[type] = UNSET,
     only: Optional[TypeOrSequence[str]] = None,
     select_related: Optional[TypeOrSequence[str]] = None,
     prefetch_related: Optional[TypeOrSequence[optimizer.PrefetchType]] = None,
     disable_optimization: bool = False,
+    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> _T:
     ...
 
 
 @overload
 def connection(
     *,
@@ -585,14 +596,15 @@
     graphql_type: Optional[Any] = None,
     filters: Optional[type] = UNSET,
     order: Optional[type] = UNSET,
     only: Optional[TypeOrSequence[str]] = None,
     select_related: Optional[TypeOrSequence[str]] = None,
     prefetch_related: Optional[TypeOrSequence[optimizer.PrefetchType]] = None,
     disable_optimization: bool = False,
+    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> Any:
     ...
 
 
 @overload
 def connection(
     resolver: Union[StrawberryResolver, Callable, staticmethod, classmethod],
@@ -609,14 +621,15 @@
     graphql_type: Optional[Any] = None,
     filters: Optional[type] = UNSET,
     order: Optional[type] = UNSET,
     only: Optional[TypeOrSequence[str]] = None,
     select_related: Optional[TypeOrSequence[str]] = None,
     prefetch_related: Optional[TypeOrSequence[optimizer.PrefetchType]] = None,
     disable_optimization: bool = False,
+    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> StrawberryDjangoConnectionField:
     ...
 
 
 def connection(
     resolver=None,
     *,
@@ -632,14 +645,15 @@
     graphql_type: Optional[Any] = None,
     filters: Optional[type] = UNSET,
     order: Optional[type] = UNSET,
     only: Optional[TypeOrSequence[str]] = None,
     select_related: Optional[TypeOrSequence[str]] = None,
     prefetch_related: Optional[TypeOrSequence[optimizer.PrefetchType]] = None,
     disable_optimization: bool = False,
+    extensions: List[FieldExtension] = (),  # type: ignore
     # This init parameter is used by pyright to determine whether this field
     # is added in the constructor or not. It is not used to change
     # any behavior at the moment.
     init: Literal[True, False, None] = None,
 ) -> Any:
     """Annotate a property or a method to create a relay connection field.
 
@@ -705,13 +719,14 @@
         directives=directives or (),
         filters=filters,
         order=order,
         only=only,
         select_related=select_related,
         prefetch_related=prefetch_related,
         disable_optimization=disable_optimization,
+        extensions=extensions,
     )
 
     if resolver is not None:
         return f(resolver)
 
     return f
```

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/filters.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/filters.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/gql/django.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/gql/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/integrations/guardian.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/management/commands/export_schema.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/middlewares/debug_toolbar.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/middlewares/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/mutations/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     ObjectDoesNotExist,
     PermissionDenied,
     ValidationError,
 )
 from strawberry import UNSET
 from strawberry.annotation import StrawberryAnnotation
 from strawberry.arguments import StrawberryArgument
+from strawberry.extensions.field_extension import FieldExtension
 from strawberry.permission import BasePermission
 from strawberry.type import StrawberryType
 from strawberry.types.fields.resolver import StrawberryResolver
 from strawberry.types.info import Info
 from strawberry.utils.await_maybe import AwaitableOrValue
 from strawberry.utils.str_converters import to_camel_case
 
@@ -367,14 +368,15 @@
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
     handle_django_errors: bool = True,
+    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> _T:
     ...
 
 
 @overload
 def mutation(
     *,
@@ -388,14 +390,15 @@
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
     handle_django_errors: bool = True,
+    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> Any:
     ...
 
 
 @overload
 def mutation(
     resolver: Union[StrawberryResolver, Callable, staticmethod, classmethod],
@@ -409,14 +412,15 @@
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
     handle_django_errors: bool = True,
+    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> DjangoInputMutationField:
     ...
 
 
 def mutation(
     resolver=None,
     *,
@@ -429,14 +433,15 @@
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
     handle_django_errors: bool = True,
+    extensions: List[FieldExtension] = (),  # type: ignore
     # This init parameter is used by pyright to determine whether this field
     # is added in the constructor or not. It is not used to change
     # any behavior at the moment.
     init: Literal[True, False, None] = None,
 ) -> Any:
     """Annotate a property or a method to create a mutation field.
 
@@ -460,14 +465,15 @@
         deprecation_reason=deprecation_reason,
         default=default,
         default_factory=default_factory,
         metadata=metadata,
         directives=directives,
         filters=filters,
         handle_django_errors=handle_django_errors,
+        extensions=extensions or (),
     )
 
     if resolver is not None:
         return f(resolver)
 
     return f
```

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/mutations/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import contextvars
 import dataclasses
+import itertools
 from collections import defaultdict
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     List,
@@ -488,15 +489,19 @@
         if config.enable_prefetch_related and self.prefetch_related:
             # Add all str at the same time to make it easier to handle Prefetch below
             to_prefetch: Dict[str, Union[str, Prefetch]] = {
                 p: p for p in self.prefetch_related if isinstance(p, str)
             }
 
             abort_only = set()
-            for p in self.prefetch_related:
+            # Merge already existing prefetches together
+            for p in itertools.chain(
+                qs._prefetch_related_lookups,  # type: ignore
+                self.prefetch_related,
+            ):
                 # Already added above
                 if isinstance(p, str):
                     continue
 
                 if isinstance(p, Callable):
                     assert_type(p, PrefetchCallable)
                     p = p(info)  # noqa: PLW2901
@@ -523,15 +528,18 @@
 
                 to_prefetch[path] = ret.prefetch
 
             # Abort only optimization if one prefetch related was made for everything
             for ao in abort_only:
                 to_prefetch[ao].queryset.query.deferred_loading = ([], True)  # type: ignore
 
-            qs = qs.prefetch_related(*to_prefetch.values())
+            # First prefetch_related(None) to clear all existing prefetches, and them add ours,
+            # which also contains them. This is to avoid the
+            # "lookup was already seen with a different queryset" error
+            qs = qs.prefetch_related(None).prefetch_related(*to_prefetch.values())
 
         if config.enable_select_related and self.select_related:
             qs = qs.select_related(*self.select_related)
 
         if config.enable_only and self.only:
             qs = qs.only(*self.only)
```

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/ordering.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/ordering.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/permissions.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/permissions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/relay.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/relay.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 )
 
 import strawberry
 from graphql import GraphQLID
 from strawberry.annotation import StrawberryAnnotation
 from strawberry.arguments import StrawberryArgument
 from strawberry.custom_scalar import ScalarDefinition
+from strawberry.extensions.field_extension import FieldExtension
 from strawberry.field import StrawberryField
 from strawberry.lazy_type import LazyType
 from strawberry.permission import BasePermission
 from strawberry.schema.types.scalar import DEFAULT_SCALAR_REGISTRY
 from strawberry.type import StrawberryContainer, StrawberryList, StrawberryOptional
 from strawberry.types import Info
 from strawberry.types.fields.resolver import StrawberryResolver
@@ -1103,14 +1104,15 @@
     description: Optional[str] = None,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
+    extensions: List[FieldExtension] = (),  # type: ignore
     # This init parameter is used by pyright to determine whether this field
     # is added in the constructor or not. It is not used to change
     # any behavior at the moment.
     init: Literal[True, False, None] = None,
 ) -> Any:
     """Annotate a property to create a relay query field.
 
@@ -1141,14 +1143,15 @@
         is_subscription=is_subscription,
         permission_classes=permission_classes or [],
         deprecation_reason=deprecation_reason,
         default=default,
         default_factory=default_factory,
         metadata=metadata,
         directives=directives or (),
+        extensions=extensions or (),
     )
 
 
 @overload
 def connection(
     *,
     resolver: Callable[[], _T],
@@ -1159,14 +1162,15 @@
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
+    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> _T:
     ...
 
 
 @overload
 def connection(
     *,
@@ -1177,14 +1181,15 @@
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
+    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> Any:
     ...
 
 
 @overload
 def connection(
     resolver: Union[StrawberryResolver, Callable, staticmethod, classmethod],
@@ -1195,14 +1200,15 @@
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
+    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> ConnectionField:
     ...
 
 
 def connection(
     resolver=None,
     *,
@@ -1212,14 +1218,15 @@
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
     graphql_type: Optional[Any] = None,
+    extensions: List[FieldExtension] = (),  # type: ignore
     # This init parameter is used by pyright to determine whether this field
     # is added in the constructor or not. It is not used to change
     # any behavior at the moment.
     init: Literal[True, False, None] = None,
 ) -> Any:
     """Annotate a property or a method to create a relay connection field.
 
@@ -1279,14 +1286,15 @@
         is_subscription=is_subscription,
         permission_classes=permission_classes or [],
         deprecation_reason=deprecation_reason,
         default=default,
         default_factory=default_factory,
         metadata=metadata,
         directives=directives or (),
+        extensions=extensions or (),
     )
 
     if resolver is not None:
         return f(resolver)
 
     return f
 
@@ -1301,14 +1309,15 @@
     init: Literal[False] = False,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
+    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> _T:
     ...
 
 
 @overload
 def input_mutation(
     *,
@@ -1318,14 +1327,15 @@
     init: Literal[True] = True,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
+    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> Any:
     ...
 
 
 @overload
 def input_mutation(
     resolver: Union[StrawberryResolver, Callable, staticmethod, classmethod],
@@ -1335,14 +1345,15 @@
     description: Optional[str] = None,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
+    extensions: List[FieldExtension] = (),  # type: ignore
 ) -> InputMutationField:
     ...
 
 
 def input_mutation(
     resolver=None,
     *,
@@ -1351,14 +1362,15 @@
     description: Optional[str] = None,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
     directives: Optional[Sequence[object]] = (),
+    extensions: List[FieldExtension] = (),  # type: ignore
     # This init parameter is used by pyright to determine whether this field
     # is added in the constructor or not. It is not used to change
     # any behavior at the moment.
     init: Literal[True, False, None] = None,
 ) -> Any:
     """Annotate a property or a method to create an input mutation field.
 
@@ -1404,13 +1416,14 @@
         is_subscription=is_subscription,
         permission_classes=permission_classes or [],
         deprecation_reason=deprecation_reason,
         default=default,
         default_factory=default_factory,
         metadata=metadata,
         directives=directives or (),
+        extensions=extensions or (),
     )
 
     if resolver is not None:
         return f(resolver)
 
     return f
```

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/settings.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html` & `strawberry_django_plus-2.2.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/test/client.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/test/client.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/type.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/type.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
             type_annotation=type_annotation,
             filters=getattr(attr, "filters", UNSET),
             order=getattr(attr, "order", UNSET),
             only=store and store.only,
             select_related=store and store.select_related,
             prefetch_related=store and store.prefetch_related,
             disable_optimization=getattr(attr, "disable_optimization", False),
+            extensions=getattr(attr, "extensions", ()),
         )
     elif isinstance(attr, StrawberryResolver):
         field = StrawberryDjangoField(base_resolver=attr)
     elif callable(attr):
         field = cast(StrawberryDjangoField, StrawberryDjangoField()(attr))
     else:
         field = StrawberryDjangoField(default=attr)
```

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/types.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/utils/aio.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/utils/query.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/utils/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-2.2.0/strawberry_django_plus/utils/typing.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.1.0/PKG-INFO` & `strawberry_django_plus-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 2.1.0
+Version: 2.2.0
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```

