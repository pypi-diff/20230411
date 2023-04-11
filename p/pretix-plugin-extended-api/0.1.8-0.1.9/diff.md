# Comparing `tmp/pretix-plugin-extended-api-0.1.8.tar.gz` & `tmp/pretix-plugin-extended-api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-plugin-extended-api-0.1.8.tar", max compression
+gzip compressed data, was "pretix-plugin-extended-api-0.1.9.tar", max compression
```

## Comparing `pretix-plugin-extended-api-0.1.8.tar` & `pretix-plugin-extended-api-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1070 2022-05-07 14:00:28.799329 pretix-plugin-extended-api-0.1.8/LICENSE
--rw-r--r--   0        0        0      836 2022-05-07 14:00:28.799329 pretix-plugin-extended-api-0.1.8/pretix_extended_api/__init__.py
--rw-r--r--   0        0        0      313 2022-05-07 14:00:28.799329 pretix-plugin-extended-api-0.1.8/pretix_extended_api/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2022-05-07 14:00:28.799329 pretix-plugin-extended-api-0.1.8/pretix_extended_api/locale/de_Informal/.gitkeep
--rw-r--r--   0        0        0      313 2022-05-07 14:00:28.799329 pretix-plugin-extended-api-0.1.8/pretix_extended_api/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0        0        0       31 2022-05-07 14:00:28.799329 pretix-plugin-extended-api-0.1.8/pretix_extended_api/signals.py
--rw-r--r--   0        0        0        0 2022-05-07 14:00:28.799329 pretix-plugin-extended-api-0.1.8/pretix_extended_api/static/pretix_extended_api/.gitkeep
--rw-r--r--   0        0        0        0 2022-05-07 14:00:28.799329 pretix-plugin-extended-api-0.1.8/pretix_extended_api/templates/pretix_extended_api/.gitkeep
--rw-r--r--   0        0        0      278 2022-05-07 14:00:28.799329 pretix-plugin-extended-api-0.1.8/pretix_extended_api/urls.py
--rw-r--r--   0        0        0        0 2022-05-07 14:00:28.799329 pretix-plugin-extended-api-0.1.8/pretix_extended_api/views/__init__.py
--rw-r--r--   0        0        0     1061 2022-05-07 14:00:28.799329 pretix-plugin-extended-api-0.1.8/pretix_extended_api/views/orders.py
--rw-r--r--   0        0        0     1840 2022-05-07 14:00:28.799329 pretix-plugin-extended-api-0.1.8/pretix_extended_api/views/serializers.py
--rw-r--r--   0        0        0     2931 2022-05-07 14:00:28.799329 pretix-plugin-extended-api-0.1.8/pretix_extended_api/views/tickets.py
--rw-r--r--   0        0        0      577 2022-05-07 14:00:38.935499 pretix-plugin-extended-api-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1059 2022-05-07 14:00:39.785462 pretix-plugin-extended-api-0.1.8/setup.py
--rw-r--r--   0        0        0      364 2022-05-07 14:00:39.785737 pretix-plugin-extended-api-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-08-02 14:39:23.947836 pretix-plugin-extended-api-0.1.9/LICENSE
+-rw-r--r--   0        0        0      836 2022-08-02 14:39:23.951836 pretix-plugin-extended-api-0.1.9/pretix_extended_api/__init__.py
+-rw-r--r--   0        0        0      313 2022-08-02 14:39:23.951836 pretix-plugin-extended-api-0.1.9/pretix_extended_api/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2022-08-02 14:39:23.951836 pretix-plugin-extended-api-0.1.9/pretix_extended_api/locale/de_Informal/.gitkeep
+-rw-r--r--   0        0        0      313 2022-08-02 14:39:23.951836 pretix-plugin-extended-api-0.1.9/pretix_extended_api/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0       31 2022-08-02 14:39:23.951836 pretix-plugin-extended-api-0.1.9/pretix_extended_api/signals.py
+-rw-r--r--   0        0        0        0 2022-08-02 14:39:23.951836 pretix-plugin-extended-api-0.1.9/pretix_extended_api/static/pretix_extended_api/.gitkeep
+-rw-r--r--   0        0        0        0 2022-08-02 14:39:23.951836 pretix-plugin-extended-api-0.1.9/pretix_extended_api/templates/pretix_extended_api/.gitkeep
+-rw-r--r--   0        0        0      418 2022-08-02 14:39:23.951836 pretix-plugin-extended-api-0.1.9/pretix_extended_api/urls.py
+-rw-r--r--   0        0        0        0 2022-08-02 14:39:23.951836 pretix-plugin-extended-api-0.1.9/pretix_extended_api/views/__init__.py
+-rw-r--r--   0        0        0      762 2022-08-02 14:39:23.951836 pretix-plugin-extended-api-0.1.9/pretix_extended_api/views/orders.py
+-rw-r--r--   0        0        0      435 2022-08-02 14:39:23.951836 pretix-plugin-extended-api-0.1.9/pretix_extended_api/views/permissions.py
+-rw-r--r--   0        0        0     2288 2022-08-02 14:39:23.951836 pretix-plugin-extended-api-0.1.9/pretix_extended_api/views/serializers.py
+-rw-r--r--   0        0        0     2594 2022-08-02 14:39:23.951836 pretix-plugin-extended-api-0.1.9/pretix_extended_api/views/tickets.py
+-rw-r--r--   0        0        0      820 2022-08-02 14:39:23.951836 pretix-plugin-extended-api-0.1.9/pretix_extended_api/views/vouchers.py
+-rw-r--r--   0        0        0      577 2022-08-02 14:39:33.843838 pretix-plugin-extended-api-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1059 2022-08-02 14:39:34.935444 pretix-plugin-extended-api-0.1.9/setup.py
+-rw-r--r--   0        0        0      364 2022-08-02 14:39:34.935795 pretix-plugin-extended-api-0.1.9/PKG-INFO
```

### Comparing `pretix-plugin-extended-api-0.1.8/LICENSE` & `pretix-plugin-extended-api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-plugin-extended-api-0.1.8/pretix_extended_api/__init__.py` & `pretix-plugin-extended-api-0.1.9/pretix_extended_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pretix-plugin-extended-api-0.1.8/pretix_extended_api/views/orders.py` & `pretix-plugin-extended-api-0.1.9/pretix_extended_api/views/orders.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from pretix.api.serializers.order import OrderSerializer
 from pretix.api.views.order import OrderViewSet
-from pretix.base.models import TeamAPIToken
-from rest_framework import exceptions, viewsets
+from rest_framework import viewsets
 from rest_framework.response import Response
 
+from .permissions import check_permission
+
 
 class OrdersViewSet(viewsets.ViewSet):
     def retrieve(self, request, pk: str, **kwargs):
-        # Only allow Team API tokens to call this API.
-        perm_holder = request.auth if isinstance(request.auth, TeamAPIToken) else None
-        if not perm_holder or not perm_holder.has_event_permission(
-            request.event.organizer, request.event, "can_view_orders"
-        ):
-            raise exceptions.PermissionDenied()
+        check_permission(request, "can_view_orders")
 
         codes = pk.split(",")
         qs = OrderViewSet(request=request).get_queryset()
         orders = qs.filter(code__in=codes)
 
         serializer = OrderSerializer(
             instance=orders,
```

### Comparing `pretix-plugin-extended-api-0.1.8/pretix_extended_api/views/serializers.py` & `pretix-plugin-extended-api-0.1.9/pretix_extended_api/views/serializers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pretix.api.serializers.i18n import I18nAwareModelSerializer
 from pretix.api.serializers.item import ItemSerializer, QuestionSerializer
+from pretix.api.serializers.voucher import VoucherSerializer
 from pretix.base.models import OrderPosition, QuestionAnswer
 from rest_framework import serializers
 
 
 class EventBodySerializer(serializers.Serializer):
     organizer_slug = serializers.CharField(required=True)
     event_slug = serializers.CharField(required=True)
@@ -57,7 +58,20 @@
             "zipcode",
         )
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.fields["item"] = ItemSerializer(read_only=True, context=self.context)
+
+
+class ExtendedVoucherSerializer(VoucherSerializer):
+    quota_items = serializers.SerializerMethodField()
+
+    def get_quota_items(self, instance):
+        if not instance.quota_id:
+            return None
+
+        return list(instance.quota.items.values_list("id", flat=True))
+
+    class Meta(VoucherSerializer.Meta):
+        fields = VoucherSerializer.Meta.fields + ("quota_items",)
```

### Comparing `pretix-plugin-extended-api-0.1.8/pretix_extended_api/views/tickets.py` & `pretix-plugin-extended-api-0.1.9/pretix_extended_api/views/tickets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 from django.db.models import Q
 from django_scopes import scopes_disabled
-from pretix.base.models import Order, OrderPosition, TeamAPIToken
-from rest_framework import exceptions, viewsets
+from pretix.base.models import Order, OrderPosition
+from rest_framework import viewsets
 from rest_framework.decorators import action
 from rest_framework.response import Response
 
+from .permissions import check_permission
 from .serializers import (
     AttendeeHasTicketBodySerializer,
     AttendeeTicketBodySerializer,
     OrderPositionSerializer,
 )
 
 
-def check_permission(request, permission):
-    # Only allow Team API tokens to call this API.
-    perm_holder = request.auth if isinstance(request.auth, TeamAPIToken) else None
-    if not perm_holder or not perm_holder.has_event_permission(
-        request.event.organizer, request.event, permission
-    ):
-        raise exceptions.PermissionDenied()
-
-
 class TicketsViewSet(viewsets.ViewSet):
     # Disable scoping because we want to allow cross-organization checking
     # This allows us to do stuff like, you can attend PyCon Italia 2022
     # if you attended europython 2021
     @scopes_disabled()
     @action(url_path="attendee-has-ticket", detail=False, methods=["post"])
     def attendee_has_ticket(self, request, **kwargs):
```

### Comparing `pretix-plugin-extended-api-0.1.8/pyproject.toml` & `pretix-plugin-extended-api-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pretix-plugin-extended-api"
-version = "0.1.8"
+version = "0.1.9"
 description = "Extend the REST API to expose more information needed by the PyCon Italia repository."
 authors = ["Python Italia"]
 packages = [ { include = "pretix_extended_api" } ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pretix-plugin-extended-api-0.1.8/setup.py` & `pretix-plugin-extended-api-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 entry_points = \
 {'pretix.plugin': ['pretix_extended_api = '
                    'pretix_extended_api:PretixPluginMeta']}
 
 setup_kwargs = {
     'name': 'pretix-plugin-extended-api',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Extend the REST API to expose more information needed by the PyCon Italia repository.',
     'long_description': None,
     'author': 'Python Italia',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

