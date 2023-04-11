# Comparing `tmp/django_accounts_api-0.2.0.tar.gz` & `tmp/django_accounts_api-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_accounts_api-0.2.0.tar", max compression
+gzip compressed data, was "django_accounts_api-0.2.0a1.tar", max compression
```

## Comparing `django_accounts_api-0.2.0.tar` & `django_accounts_api-0.2.0a1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1204 2023-01-06 05:27:06.379634 django_accounts_api-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-01-05 07:41:34.771966 django_accounts_api-0.2.0/django_accounts_api/__init__.py
--rw-r--r--   0        0        0     2870 2023-01-18 05:07:02.825331 django_accounts_api-0.2.0/django_accounts_api/api_login_tests.py
--rw-r--r--   0        0        0     4437 2023-01-18 05:07:02.825752 django_accounts_api-0.2.0/django_accounts_api/api_password_change_tests.py
--rw-r--r--   0        0        0      159 2023-01-05 07:41:34.772082 django_accounts_api-0.2.0/django_accounts_api/apps.py
--rw-r--r--   0        0        0     5657 2023-01-18 05:07:02.826071 django_accounts_api-0.2.0/django_accounts_api/login_logout_tests.py
--rw-r--r--   0        0        0      622 2023-01-06 05:27:06.380104 django_accounts_api-0.2.0/django_accounts_api/manifest_tests.py
--rw-r--r--   0        0        0        0 2023-01-05 07:41:34.772396 django_accounts_api-0.2.0/django_accounts_api/migrations/__init__.py
--rw-r--r--   0        0        0     1844 2023-01-18 05:07:02.826459 django_accounts_api-0.2.0/django_accounts_api/password_change_tests.py
--rw-r--r--   0        0        0     2059 2023-03-22 04:20:55.389597 django_accounts_api-0.2.0/django_accounts_api/password_reset_confirm_tests.py
--rw-r--r--   0        0        0     1277 2023-03-22 04:12:48.587165 django_accounts_api-0.2.0/django_accounts_api/password_reset_tests.py
--rw-r--r--   0        0        0       18 2023-01-06 05:27:06.380468 django_accounts_api-0.2.0/django_accounts_api/templates/django_accounts_api/login.html
--rw-r--r--   0        0        0       18 2023-01-06 05:27:06.380624 django_accounts_api-0.2.0/django_accounts_api/templates/django_accounts_api/password_change.html
--rw-r--r--   0        0        0       47 2023-03-22 04:20:55.396743 django_accounts_api-0.2.0/django_accounts_api/templates/django_accounts_api/password_reset.html
--rw-r--r--   0        0        0       18 2023-03-22 04:12:48.577885 django_accounts_api-0.2.0/django_accounts_api/templates/django_accounts_api/password_reset_confirm.html
--rw-r--r--   0        0        0      575 2023-03-23 06:09:07.752765 django_accounts_api-0.2.0/django_accounts_api/templates/registration/password_reset_email.html
--rw-r--r--   0        0        0      906 2023-03-27 05:18:57.198176 django_accounts_api-0.2.0/django_accounts_api/urls.py
--rw-r--r--   0        0        0    10860 2023-03-27 05:18:27.766573 django_accounts_api-0.2.0/django_accounts_api/views.py
--rw-r--r--   0        0        0      793 2023-04-11 04:12:27.951619 django_accounts_api-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1813 1970-01-01 00:00:00.000000 django_accounts_api-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1204 2023-01-06 05:27:06.379634 django_accounts_api-0.2.0a1/README.md
+-rw-r--r--   0        0        0        0 2023-01-05 07:41:34.771966 django_accounts_api-0.2.0a1/django_accounts_api/__init__.py
+-rw-r--r--   0        0        0     2870 2023-01-18 05:07:02.825331 django_accounts_api-0.2.0a1/django_accounts_api/api_login_tests.py
+-rw-r--r--   0        0        0     4437 2023-01-18 05:07:02.825752 django_accounts_api-0.2.0a1/django_accounts_api/api_password_change_tests.py
+-rw-r--r--   0        0        0      159 2023-01-05 07:41:34.772082 django_accounts_api-0.2.0a1/django_accounts_api/apps.py
+-rw-r--r--   0        0        0     5657 2023-01-18 05:07:02.826071 django_accounts_api-0.2.0a1/django_accounts_api/login_logout_tests.py
+-rw-r--r--   0        0        0      622 2023-01-06 05:27:06.380104 django_accounts_api-0.2.0a1/django_accounts_api/manifest_tests.py
+-rw-r--r--   0        0        0        0 2023-01-05 07:41:34.772396 django_accounts_api-0.2.0a1/django_accounts_api/migrations/__init__.py
+-rw-r--r--   0        0        0     1844 2023-01-18 05:07:02.826459 django_accounts_api-0.2.0a1/django_accounts_api/password_change_tests.py
+-rw-r--r--   0        0        0     2059 2023-03-22 04:20:55.389597 django_accounts_api-0.2.0a1/django_accounts_api/password_reset_confirm_tests.py
+-rw-r--r--   0        0        0     1277 2023-03-22 04:12:48.587165 django_accounts_api-0.2.0a1/django_accounts_api/password_reset_tests.py
+-rw-r--r--   0        0        0       18 2023-01-06 05:27:06.380468 django_accounts_api-0.2.0a1/django_accounts_api/templates/django_accounts_api/login.html
+-rw-r--r--   0        0        0       18 2023-01-06 05:27:06.380624 django_accounts_api-0.2.0a1/django_accounts_api/templates/django_accounts_api/password_change.html
+-rw-r--r--   0        0        0       47 2023-03-22 04:20:55.396743 django_accounts_api-0.2.0a1/django_accounts_api/templates/django_accounts_api/password_reset.html
+-rw-r--r--   0        0        0       18 2023-03-22 04:12:48.577885 django_accounts_api-0.2.0a1/django_accounts_api/templates/django_accounts_api/password_reset_confirm.html
+-rw-r--r--   0        0        0      561 2023-03-22 04:20:55.396996 django_accounts_api-0.2.0a1/django_accounts_api/templates/registration/password_reset_email.html
+-rw-r--r--   0        0        0      724 2023-03-22 04:20:55.389855 django_accounts_api-0.2.0a1/django_accounts_api/urls.py
+-rw-r--r--   0        0        0    10430 2023-03-22 04:20:55.409075 django_accounts_api-0.2.0a1/django_accounts_api/views.py
+-rw-r--r--   0        0        0      795 2023-03-22 05:19:00.769640 django_accounts_api-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2077 1970-01-01 00:00:00.000000 django_accounts_api-0.2.0a1/setup.py
+-rw-r--r--   0        0        0     1815 1970-01-01 00:00:00.000000 django_accounts_api-0.2.0a1/PKG-INFO
```

### Comparing `django_accounts_api-0.2.0/README.md` & `django_accounts_api-0.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `django_accounts_api-0.2.0/django_accounts_api/api_login_tests.py` & `django_accounts_api-0.2.0a1/django_accounts_api/api_login_tests.py`

 * *Files identical despite different names*

### Comparing `django_accounts_api-0.2.0/django_accounts_api/api_password_change_tests.py` & `django_accounts_api-0.2.0a1/django_accounts_api/api_password_change_tests.py`

 * *Files identical despite different names*

### Comparing `django_accounts_api-0.2.0/django_accounts_api/login_logout_tests.py` & `django_accounts_api-0.2.0a1/django_accounts_api/login_logout_tests.py`

 * *Files identical despite different names*

### Comparing `django_accounts_api-0.2.0/django_accounts_api/manifest_tests.py` & `django_accounts_api-0.2.0a1/django_accounts_api/manifest_tests.py`

 * *Files identical despite different names*

### Comparing `django_accounts_api-0.2.0/django_accounts_api/password_change_tests.py` & `django_accounts_api-0.2.0a1/django_accounts_api/password_change_tests.py`

 * *Files identical despite different names*

### Comparing `django_accounts_api-0.2.0/django_accounts_api/password_reset_confirm_tests.py` & `django_accounts_api-0.2.0a1/django_accounts_api/password_reset_confirm_tests.py`

 * *Files identical despite different names*

### Comparing `django_accounts_api-0.2.0/django_accounts_api/password_reset_tests.py` & `django_accounts_api-0.2.0a1/django_accounts_api/password_reset_tests.py`

 * *Files identical despite different names*

### Comparing `django_accounts_api-0.2.0/django_accounts_api/urls.py` & `django_accounts_api-0.2.0a1/django_accounts_api/urls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from django.urls import path
-from django.contrib.auth import views as auth_views
 from .views import (
     Login,
     Logout,
     PasswordChange,
-    PasswordReset,
+    PasswordResetRequest,
     PasswordResetConfirmView,
-    PasswordResetConfirm,
-    PasswordResetComplete,
     login_check,
     manifest
 )
 
 app_name = 'django_accounts_api'
 urlpatterns = [
     path('', manifest, name='manifest'),
     path('check', login_check, name='login_check'),
     path('login', Login.as_view(), name='login'),
     path('logout', Logout.as_view(), name='logout'),
     path('password_change', PasswordChange.as_view(), name='password_change'),
-    path('password_reset', PasswordReset.as_view(), name='password_reset'),
+    path('password_reset', PasswordResetRequest.as_view(), name='password_reset'),
     path(
         "reset/<uidb64>/<token>/",
         PasswordResetConfirmView.as_view(),
         name='password_reset_confirm'
-    ),
-    path('reset/done/', PasswordResetComplete.as_view(), name='password_reset_complete'),
+    )
 ]
```

### Comparing `django_accounts_api-0.2.0/django_accounts_api/views.py` & `django_accounts_api-0.2.0a1/django_accounts_api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 from django.views.generic import View
 from django.contrib.auth.models import User as DjangoUser
 from django.contrib.auth import get_user_model
-from django.contrib.auth.views import LoginView, LogoutView, PasswordChangeView, PasswordResetView, PasswordResetCompleteView, PasswordResetConfirmView
+from django.contrib.auth.views import LoginView, LogoutView, PasswordChangeView, PasswordResetView, PasswordResetDoneView, PasswordResetCompleteView, PasswordResetConfirmView
 from django.urls.exceptions import NoReverseMatch
 from django.http import HttpRequest, HttpResponse, JsonResponse
 from django.urls import reverse
 from django.utils.decorators import method_decorator
 from django.utils.translation import gettext_lazy as _
 from django.views.decorators.csrf import csrf_protect
 from django.views.decorators.debug import sensitive_post_parameters
@@ -148,15 +148,15 @@
         except NoReverseMatch:
             pass
         return HttpResponse(status=200)
 
 
 @method_decorator(sensitive_post_parameters(), name='dispatch')
 @method_decorator(csrf_protect, name='dispatch')
-class PasswordReset(AcceptJsonMixin, PasswordResetView):
+class PasswordResetRequest(AcceptJsonMixin, PasswordResetView):
     ''' Override the Django password reset view to support API use
     GET - renders a password reset form - can be accessed without auth
     '''
 
     template_name = "django_accounts_api/password_reset.html"
 
     def dispatch(self, request, *args, **kwargs):
@@ -260,19 +260,7 @@
         """
         If the form is invalid, re-render the context data with the
         data-filled form and errors.
         """
         if self.json_response_requested():
             return JsonResponse({'errors': form.errors}, status=400)
         return super().form_invalid(form)
-
-class PasswordResetComplete(PasswordResetCompleteView):
-    """
-    Custom PasswordResetCompleteView to support API use
-    """
-    template_name = 'password_reset_complete.html'
-
-    def render_to_response(self, context, **response_kwargs):
-        if self.json_response_requested():
-            return JsonResponse({'message': 'Password reset successful.'}, status=200)
-        else:
-            return super().render_to_response(context, **response_kwargs)
```

### Comparing `django_accounts_api-0.2.0/pyproject.toml` & `django_accounts_api-0.2.0a1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-accounts-api"
-version = "0.2.0"
+version = "0.2.0a1"
 description = ""
 authors = ["PeteCoward <peter@catalpa.io>"]
 readme = "README.md"
 packages = [{include = "django_accounts_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `django_accounts_api-0.2.0/PKG-INFO` & `django_accounts_api-0.2.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-accounts-api
-Version: 0.2.0
+Version: 0.2.0a1
 Summary: 
 Author: PeteCoward
 Author-email: peter@catalpa.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

