# Comparing `tmp/django-admin-safe-login-0.3.4.tar.gz` & `tmp/django-admin-safe-login-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-admin-safe-login-0.3.4.tar", last modified: Mon Apr 12 12:01:57 2021, max compression
+gzip compressed data, was "django-admin-safe-login-0.3.5.tar", last modified: Tue Apr 11 14:09:23 2023, max compression
```

## Comparing `django-admin-safe-login-0.3.4.tar` & `django-admin-safe-login-0.3.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/
--rw-rw-rw-   0        0        0     1067 2021-04-12 11:47:18.000000 django-admin-safe-login-0.3.4/LICENSE
--rw-rw-rw-   0        0        0      237 2021-04-12 11:47:18.000000 django-admin-safe-login-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6632 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     4950 2021-04-12 12:01:30.000000 django-admin-safe-login-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/
--rw-rw-rw-   0        0        0      205 2021-04-12 11:47:18.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/__init__.py
--rw-rw-rw-   0        0        0       33 2021-04-12 11:47:18.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/admin.py
--rw-rw-rw-   0        0        0      876 2021-04-12 11:47:18.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/apps.py
--rw-rw-rw-   0        0        0      514 2021-04-12 11:47:18.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/forms.py
-drwxrwxrwx   0        0        0        0 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/locale/
-drwxrwxrwx   0        0        0        0 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/locale/zh_hans/
-drwxrwxrwx   0        0        0        0 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/locale/zh_hans/LC_MESSAGES/
--rw-rw-rw-   0        0        0      415 2021-04-12 11:47:18.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/locale/zh_hans/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      782 2021-04-12 11:47:18.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/locale/zh_hans/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/migrations/
--rw-rw-rw-   0        0        0        0 2021-04-12 11:47:18.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/static/
-drwxrwxrwx   0        0        0        0 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/static/django-admin-safe-login/
-drwxrwxrwx   0        0        0        0 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/static/django-admin-safe-login/css/
--rw-rw-rw-   0        0        0      490 2021-04-12 11:47:18.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/static/django-admin-safe-login/css/django-admin-safe-login.css
-drwxrwxrwx   0        0        0        0 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/static/django-admin-safe-login/js/
--rw-rw-rw-   0        0        0      495 2021-04-12 11:55:15.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/static/django-admin-safe-login/js/django-admin-safe-login.js
-drwxrwxrwx   0        0        0        0 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/templates/
-drwxrwxrwx   0        0        0        0 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/templates/admin/
--rw-rw-rw-   0        0        0     4084 2021-04-12 11:52:15.000000 django-admin-safe-login-0.3.4/django_admin_safe_login/templates/admin/login.html
-drwxrwxrwx   0        0        0        0 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login.egg-info/
--rw-rw-rw-   0        0        0     6632 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-04-12 12:00:19.000000 django-admin-safe-login-0.3.4/django_admin_safe_login.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      136 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/django_admin_safe_login.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2021-04-12 11:47:18.000000 django-admin-safe-login-0.3.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2021-04-12 12:01:57.000000 django-admin-safe-login-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1390 2021-04-12 11:47:18.000000 django-admin-safe-login-0.3.4/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-11 14:09:23.929083 django-admin-safe-login-0.3.5/
+-rw-r--r--   0 test       (501) staff       (20)     1067 2022-04-24 06:30:05.000000 django-admin-safe-login-0.3.5/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      237 2022-04-24 06:30:05.000000 django-admin-safe-login-0.3.5/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     5624 2023-04-11 14:09:23.928980 django-admin-safe-login-0.3.5/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     4987 2023-04-11 14:07:15.000000 django-admin-safe-login-0.3.5/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-11 14:09:23.927194 django-admin-safe-login-0.3.5/django_admin_safe_login/
+-rw-r--r--   0 test       (501) staff       (20)      205 2022-04-24 06:30:05.000000 django-admin-safe-login-0.3.5/django_admin_safe_login/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       33 2022-04-24 06:30:05.000000 django-admin-safe-login-0.3.5/django_admin_safe_login/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      876 2022-04-24 06:30:05.000000 django-admin-safe-login-0.3.5/django_admin_safe_login/apps.py
+-rw-r--r--   0 test       (501) staff       (20)      513 2023-04-11 13:53:01.000000 django-admin-safe-login-0.3.5/django_admin_safe_login/forms.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-11 14:09:23.925547 django-admin-safe-login-0.3.5/django_admin_safe_login/locale/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-11 14:09:23.925585 django-admin-safe-login-0.3.5/django_admin_safe_login/locale/zh_hans/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-11 14:09:23.928247 django-admin-safe-login-0.3.5/django_admin_safe_login/locale/zh_hans/LC_MESSAGES/
+-rw-r--r--   0 test       (501) staff       (20)      415 2022-04-24 06:30:05.000000 django-admin-safe-login-0.3.5/django_admin_safe_login/locale/zh_hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 test       (501) staff       (20)      782 2022-04-24 06:30:05.000000 django-admin-safe-login-0.3.5/django_admin_safe_login/locale/zh_hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-11 14:09:23.928395 django-admin-safe-login-0.3.5/django_admin_safe_login/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2022-04-24 06:30:05.000000 django-admin-safe-login-0.3.5/django_admin_safe_login/migrations/__init__.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-11 14:09:23.925734 django-admin-safe-login-0.3.5/django_admin_safe_login/static/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-11 14:09:23.925825 django-admin-safe-login-0.3.5/django_admin_safe_login/static/django-admin-safe-login/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-11 14:09:23.928519 django-admin-safe-login-0.3.5/django_admin_safe_login/static/django-admin-safe-login/css/
+-rw-r--r--   0 test       (501) staff       (20)      490 2022-04-24 06:30:05.000000 django-admin-safe-login-0.3.5/django_admin_safe_login/static/django-admin-safe-login/css/django-admin-safe-login.css
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-11 14:09:23.928672 django-admin-safe-login-0.3.5/django_admin_safe_login/static/django-admin-safe-login/js/
+-rw-r--r--   0 test       (501) staff       (20)      495 2022-04-24 06:30:05.000000 django-admin-safe-login-0.3.5/django_admin_safe_login/static/django-admin-safe-login/js/django-admin-safe-login.js
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-11 14:09:23.925921 django-admin-safe-login-0.3.5/django_admin_safe_login/templates/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-11 14:09:23.928810 django-admin-safe-login-0.3.5/django_admin_safe_login/templates/admin/
+-rw-r--r--   0 test       (501) staff       (20)     4084 2022-04-24 06:30:05.000000 django-admin-safe-login-0.3.5/django_admin_safe_login/templates/admin/login.html
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-11 14:09:23.927999 django-admin-safe-login-0.3.5/django_admin_safe_login.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     5624 2023-04-11 14:09:23.000000 django-admin-safe-login-0.3.5/django_admin_safe_login.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      861 2023-04-11 14:09:23.000000 django-admin-safe-login-0.3.5/django_admin_safe_login.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-04-11 14:09:23.000000 django-admin-safe-login-0.3.5/django_admin_safe_login.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-04-11 14:09:23.000000 django-admin-safe-login-0.3.5/django_admin_safe_login.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)      136 2023-04-11 14:09:23.000000 django-admin-safe-login-0.3.5/django_admin_safe_login.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       24 2023-04-11 14:09:23.000000 django-admin-safe-login-0.3.5/django_admin_safe_login.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)      136 2022-04-24 06:30:05.000000 django-admin-safe-login-0.3.5/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2023-04-11 14:09:23.929114 django-admin-safe-login-0.3.5/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1390 2023-04-11 13:58:34.000000 django-admin-safe-login-0.3.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-admin-safe-login-0.3.4/LICENSE` & `django-admin-safe-login-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-safe-login-0.3.4/PKG-INFO` & `django-admin-safe-login-0.3.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-Metadata-Version: 2.1
-Name: django-admin-safe-login
-Version: 0.3.4
-Summary: Add captcha field for django admin's login page.
-Home-page: UNKNOWN
-Author: zencore
-Author-email: dobetter@zencore.cn
-License: MIT
-Description: # django-admin-safe-login
-        
-        Add captcha field and rsa encryption password field for django admin's login page.
-        
-        ## Install
-        
-        ```shell
-        pip install django-admin-safe-login
-        ```
-        
-        ## Usage
-        
-        **pro/settings.py**
-        
-        ```python
-        INSTALLED_APPS = [
-            ...
-            'django_static_jquery3',
-            'django_secure_password_input',
-            'django_simple_tags',
-            'captcha',
-            'django_admin_safe_login',
-            ...
-        ]
-        
-        CAPTCHA_IMAGE_SIZE = (100, 30)  # required
-        DJANGO_ADMIN_SAFE_LOGIN_ENABLE_CAPTCHA = True # optional, default to True
-        DJANGO_ADMIN_SAFE_LOGIN_BACKGROUND_IMAGE = "django-admin-safe-login/img/example-background.jpg"  # optional, default to no-image.
-        DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_RIGHT = "200px" # optional, default to auto
-        DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_LEFT = "auto" # optional, default to auto
-        DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_TOP = "100px" # optional, default to auto
-        DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_BOTTOM = "100px" # optional, default to auto
-        DJANGO_ADMIN_SAFE_LOGIN_TEMPLATE = "" # optional, default to "admin/login.html".
-        ```
-        
-        **Note:**
-        
-        1. Insert django_static_jquery3, django_secure_password_input, django-simple-tags, captcha and django_admin_safe_login into INSTALLED_APPS.
-        1. Application django_static_jquery3 provides static jquery.js.
-        1. Application django_secure_password_input provides rsa encryption and decryption function for password field.
-        1. Application django_admin_safe_login provides all functions about safe login.
-        1. Application captcha provides image captcha functions.
-        1. Application django-simple-tags provides custom template tags used in our admin/login.html.
-        1. Configuration item CAPTCHA_IMAGE_SIZE is required, and must set to (100, 30) so that it will not break the display style. If you want other size image, you have to rewrite some css code.
-        1. Configurations about password RSA encryption, see details at https://pypi.org/project/django-secure-password-input/.
-        1. Configurations about captcha, see detail at https://pypi.org/project/django-simple-captcha/.
-        1. Configurations about password reset, see detail at https://docs.djangoproject.com/en/3.0/ref/contrib/admin/ (search: Adding a password reset feature).
-        
-        **pro/urls.py**
-        
-        ```python
-        from django.urls import path
-        from django.urls import include
-        from django.contrib.auth import views as auth_views
-        
-        urlpatterns = [
-            ...
-            path(
-                'admin/password_reset/',
-                auth_views.PasswordResetView.as_view(),
-                name='admin_password_reset',
-            ),
-            path(
-                'admin/password_reset/done/',
-                auth_views.PasswordResetDoneView.as_view(),
-                name='password_reset_done',
-            ),
-            path(
-                'reset/<uidb64>/<token>/',
-                auth_views.PasswordResetConfirmView.as_view(),
-                name='password_reset_confirm',
-            ),
-            path(
-                'reset/done/',
-                auth_views.PasswordResetCompleteView.as_view(),
-                name='password_reset_complete',
-            ),
-            path('captcha/', include("captcha.urls")),
-            ...
-        ]
-        ```
-        
-        **Note:**
-        
-        1. Include captcha.urls is required so that the captcha image can be displayed.
-        1. `Reset Password Link` only shows when you enabled `admin_password_reset` views in your urls.
-        
-        ## Changes about admin/login.html
-        
-        We have override some part of admin/login.html. But the admin/login.html content may change in future releases. So you should known what part is overrided.
-        
-        1. Our new admin/login.html extends from system's admin/login.html.
-        1. We override the extrastyle block to add extra js and css.
-        1. The function adding background image and changing login box position is implemented in our new extrastyle block.
-        1. We override the whole content block.
-        1. We copied the whole content block from django's default admin/login.html.
-        1. We added blocks inside content block: form, form-row-username, from-row-password, form-row-extra, form-row-captcha, password-reset-url, before-submit-row, submit-row, after-submit-row.
-        
-        
-        
-        ## Releases
-        
-        | Release | Time | Changes                                                     | Notice |
-        | ------ | ---------- | ---------------------------------------------------------------- | ---- |
-        | v0.1.0 | 2020/03/06 | 1. First release. | |
-        | v0.2.0 | 2020/03/07 | 2. Add rsa encryption and decrption functions for password field.<br />3. Fix requirements.txt missing django-static-jquery3 problem. | |
-        | v0.3.0 | 2020/05/20 | 4. Add background image setting.<br />5. Add login box position setting.<br />6. Use admin/login.html override instead of creating a new template.<br />7. Fix document.<br />8. Fix translation.<br />9. Fix setup.py problem that include demo and example code in the final package. | |
-        | v0.3.1 | 2020/09/01 | 10. Rename zh_Hans to zh_hans.<br />11. Depends on django-static-jquery3>=5.0.0. | |
-        | v0.3.2 | 2020/09/01 | 12. Depends on django-secure-password-input>=0.1.1. | |
-        | v0.3.3 | 2020/09/24 | 13. Add app_requires.<br />14. Add License file. | |
-        | v0.3.4 | 2021/04/12 | 15. Test with django 3.2.<br />16. Auto get captcha refresh url. | |
-        
-Keywords: django admin extentions,django admin safe login
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: django-admin-safe-login
+Version: 0.3.5
+Summary: Add captcha field for django admin's login page.
+Author: zencore
+Author-email: dobetter@zencore.cn
+License: MIT
+Keywords: django admin extentions,django admin safe login
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django-admin-safe-login
+
+Add captcha field and rsa encryption password field for django admin's login page.
+
+## Install
+
+```shell
+pip install django-admin-safe-login
+```
+
+## Usage
+
+**pro/settings.py**
+
+```python
+INSTALLED_APPS = [
+    ...
+    'django_static_jquery3',
+    'django_secure_password_input',
+    'django_simple_tags',
+    'captcha',
+    'django_admin_safe_login',
+    ...
+]
+
+CAPTCHA_IMAGE_SIZE = (100, 30)  # required
+DJANGO_ADMIN_SAFE_LOGIN_ENABLE_CAPTCHA = True # optional, default to True
+DJANGO_ADMIN_SAFE_LOGIN_BACKGROUND_IMAGE = "django-admin-safe-login/img/example-background.jpg"  # optional, default to no-image.
+DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_RIGHT = "200px" # optional, default to auto
+DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_LEFT = "auto" # optional, default to auto
+DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_TOP = "100px" # optional, default to auto
+DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_BOTTOM = "100px" # optional, default to auto
+DJANGO_ADMIN_SAFE_LOGIN_TEMPLATE = "" # optional, default to "admin/login.html".
+```
+
+**Note:**
+
+1. Insert django_static_jquery3, django_secure_password_input, django-simple-tags, captcha and django_admin_safe_login into INSTALLED_APPS.
+1. Application django_static_jquery3 provides static jquery.js.
+1. Application django_secure_password_input provides rsa encryption and decryption function for password field.
+1. Application django_admin_safe_login provides all functions about safe login.
+1. Application captcha provides image captcha functions.
+1. Application django-simple-tags provides custom template tags used in our admin/login.html.
+1. Configuration item CAPTCHA_IMAGE_SIZE is required, and must set to (100, 30) so that it will not break the display style. If you want other size image, you have to rewrite some css code.
+1. Configurations about password RSA encryption, see details at https://pypi.org/project/django-secure-password-input/.
+1. Configurations about captcha, see detail at https://pypi.org/project/django-simple-captcha/.
+1. Configurations about password reset, see detail at https://docs.djangoproject.com/en/3.0/ref/contrib/admin/ (search: Adding a password reset feature).
+
+**pro/urls.py**
+
+```python
+from django.urls import path
+from django.urls import include
+from django.contrib.auth import views as auth_views
+
+urlpatterns = [
+    ...
+    path(
+        'admin/password_reset/',
+        auth_views.PasswordResetView.as_view(),
+        name='admin_password_reset',
+    ),
+    path(
+        'admin/password_reset/done/',
+        auth_views.PasswordResetDoneView.as_view(),
+        name='password_reset_done',
+    ),
+    path(
+        'reset/<uidb64>/<token>/',
+        auth_views.PasswordResetConfirmView.as_view(),
+        name='password_reset_confirm',
+    ),
+    path(
+        'reset/done/',
+        auth_views.PasswordResetCompleteView.as_view(),
+        name='password_reset_complete',
+    ),
+    path('captcha/', include("captcha.urls")),
+    ...
+]
+```
+
+**Note:**
+
+1. Include captcha.urls is required so that the captcha image can be displayed.
+1. `Reset Password Link` only shows when you enabled `admin_password_reset` views in your urls.
+
+## Changes about admin/login.html
+
+We have override some part of admin/login.html. But the admin/login.html content may change in future releases. So you should known what part is overrided.
+
+1. Our new admin/login.html extends from system's admin/login.html.
+1. We override the extrastyle block to add extra js and css.
+1. The function adding background image and changing login box position is implemented in our new extrastyle block.
+1. We override the whole content block.
+1. We copied the whole content block from django's default admin/login.html.
+1. We added blocks inside content block: form, form-row-username, from-row-password, form-row-extra, form-row-captcha, password-reset-url, before-submit-row, submit-row, after-submit-row.
+
+
+
+## Releases
+
+| Release | Time | Changes                                                     |
+| ------ | ---------- | ---------------------------------------------------------------- |
+| v0.1.0 | 2020/03/06 | 1. First release. |
+| v0.2.0 | 2020/03/07 | 2. Add rsa encryption and decrption functions for password field.<br />3. Fix requirements.txt missing django-static-jquery3 problem. |
+| v0.3.0 | 2020/05/20 | 4. Add background image setting.<br />5. Add login box position setting.<br />6. Use admin/login.html override instead of creating a new template.<br />7. Fix document.<br />8. Fix translation.<br />9. Fix setup.py problem that include demo and example code in the final package. |
+| v0.3.1 | 2020/09/01 | 10. Rename zh_Hans to zh_hans.<br />11. Depends on django-static-jquery3>=5.0.0. |
+| v0.3.2 | 2020/09/01 | 12. Depends on django-secure-password-input>=0.1.1. |
+| v0.3.3 | 2020/09/24 | 13. Add app_requires.<br />14. Add License file. |
+| v0.3.4 | 2021/04/12 | 15. Test with django 3.2.<br />16. Auto get captcha refresh url. |
+| v0.3.5 | 2023/04/11 | 17. Fix ugettext problem for Django 4.2. |
```

### Comparing `django-admin-safe-login-0.3.4/README.md` & `django-admin-safe-login-0.3.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -96,16 +96,17 @@
 1. We copied the whole content block from django's default admin/login.html.
 1. We added blocks inside content block: form, form-row-username, from-row-password, form-row-extra, form-row-captcha, password-reset-url, before-submit-row, submit-row, after-submit-row.
 
 
 
 ## Releases
 
-| Release | Time | Changes                                                     | Notice |
-| ------ | ---------- | ---------------------------------------------------------------- | ---- |
-| v0.1.0 | 2020/03/06 | 1. First release. | |
-| v0.2.0 | 2020/03/07 | 2. Add rsa encryption and decrption functions for password field.<br />3. Fix requirements.txt missing django-static-jquery3 problem. | |
-| v0.3.0 | 2020/05/20 | 4. Add background image setting.<br />5. Add login box position setting.<br />6. Use admin/login.html override instead of creating a new template.<br />7. Fix document.<br />8. Fix translation.<br />9. Fix setup.py problem that include demo and example code in the final package. | |
-| v0.3.1 | 2020/09/01 | 10. Rename zh_Hans to zh_hans.<br />11. Depends on django-static-jquery3>=5.0.0. | |
-| v0.3.2 | 2020/09/01 | 12. Depends on django-secure-password-input>=0.1.1. | |
-| v0.3.3 | 2020/09/24 | 13. Add app_requires.<br />14. Add License file. | |
-| v0.3.4 | 2021/04/12 | 15. Test with django 3.2.<br />16. Auto get captcha refresh url. | |
+| Release | Time | Changes                                                     |
+| ------ | ---------- | ---------------------------------------------------------------- |
+| v0.1.0 | 2020/03/06 | 1. First release. |
+| v0.2.0 | 2020/03/07 | 2. Add rsa encryption and decrption functions for password field.<br />3. Fix requirements.txt missing django-static-jquery3 problem. |
+| v0.3.0 | 2020/05/20 | 4. Add background image setting.<br />5. Add login box position setting.<br />6. Use admin/login.html override instead of creating a new template.<br />7. Fix document.<br />8. Fix translation.<br />9. Fix setup.py problem that include demo and example code in the final package. |
+| v0.3.1 | 2020/09/01 | 10. Rename zh_Hans to zh_hans.<br />11. Depends on django-static-jquery3>=5.0.0. |
+| v0.3.2 | 2020/09/01 | 12. Depends on django-secure-password-input>=0.1.1. |
+| v0.3.3 | 2020/09/24 | 13. Add app_requires.<br />14. Add License file. |
+| v0.3.4 | 2021/04/12 | 15. Test with django 3.2.<br />16. Auto get captcha refresh url. |
+| v0.3.5 | 2023/04/11 | 17. Fix ugettext problem for Django 4.2. |
```

### Comparing `django-admin-safe-login-0.3.4/django_admin_safe_login/apps.py` & `django-admin-safe-login-0.3.5/django_admin_safe_login/apps.py`

 * *Files identical despite different names*

### Comparing `django-admin-safe-login-0.3.4/django_admin_safe_login/forms.py` & `django-admin-safe-login-0.3.5/django_admin_safe_login/forms.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.contrib.admin.forms import AdminAuthenticationForm
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from captcha.fields import CaptchaField
 from django_secure_password_input.fields import DjangoSecurePasswordInput
 from django.conf import settings
 
 class AdminSafeAuthenticationForm(AdminAuthenticationForm):
     password = DjangoSecurePasswordInput(label=_("Password"))
     if getattr(settings, "DJANGO_ADMIN_SAFE_LOGIN_ENABLE_CAPTCHA", True):
```

### Comparing `django-admin-safe-login-0.3.4/django_admin_safe_login/locale/zh_hans/LC_MESSAGES/django.po` & `django-admin-safe-login-0.3.5/django_admin_safe_login/locale/zh_hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-safe-login-0.3.4/django_admin_safe_login/templates/admin/login.html` & `django-admin-safe-login-0.3.5/django_admin_safe_login/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django-admin-safe-login-0.3.4/django_admin_safe_login.egg-info/PKG-INFO` & `django-admin-safe-login-0.3.5/django_admin_safe_login.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-Metadata-Version: 2.1
-Name: django-admin-safe-login
-Version: 0.3.4
-Summary: Add captcha field for django admin's login page.
-Home-page: UNKNOWN
-Author: zencore
-Author-email: dobetter@zencore.cn
-License: MIT
-Description: # django-admin-safe-login
-        
-        Add captcha field and rsa encryption password field for django admin's login page.
-        
-        ## Install
-        
-        ```shell
-        pip install django-admin-safe-login
-        ```
-        
-        ## Usage
-        
-        **pro/settings.py**
-        
-        ```python
-        INSTALLED_APPS = [
-            ...
-            'django_static_jquery3',
-            'django_secure_password_input',
-            'django_simple_tags',
-            'captcha',
-            'django_admin_safe_login',
-            ...
-        ]
-        
-        CAPTCHA_IMAGE_SIZE = (100, 30)  # required
-        DJANGO_ADMIN_SAFE_LOGIN_ENABLE_CAPTCHA = True # optional, default to True
-        DJANGO_ADMIN_SAFE_LOGIN_BACKGROUND_IMAGE = "django-admin-safe-login/img/example-background.jpg"  # optional, default to no-image.
-        DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_RIGHT = "200px" # optional, default to auto
-        DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_LEFT = "auto" # optional, default to auto
-        DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_TOP = "100px" # optional, default to auto
-        DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_BOTTOM = "100px" # optional, default to auto
-        DJANGO_ADMIN_SAFE_LOGIN_TEMPLATE = "" # optional, default to "admin/login.html".
-        ```
-        
-        **Note:**
-        
-        1. Insert django_static_jquery3, django_secure_password_input, django-simple-tags, captcha and django_admin_safe_login into INSTALLED_APPS.
-        1. Application django_static_jquery3 provides static jquery.js.
-        1. Application django_secure_password_input provides rsa encryption and decryption function for password field.
-        1. Application django_admin_safe_login provides all functions about safe login.
-        1. Application captcha provides image captcha functions.
-        1. Application django-simple-tags provides custom template tags used in our admin/login.html.
-        1. Configuration item CAPTCHA_IMAGE_SIZE is required, and must set to (100, 30) so that it will not break the display style. If you want other size image, you have to rewrite some css code.
-        1. Configurations about password RSA encryption, see details at https://pypi.org/project/django-secure-password-input/.
-        1. Configurations about captcha, see detail at https://pypi.org/project/django-simple-captcha/.
-        1. Configurations about password reset, see detail at https://docs.djangoproject.com/en/3.0/ref/contrib/admin/ (search: Adding a password reset feature).
-        
-        **pro/urls.py**
-        
-        ```python
-        from django.urls import path
-        from django.urls import include
-        from django.contrib.auth import views as auth_views
-        
-        urlpatterns = [
-            ...
-            path(
-                'admin/password_reset/',
-                auth_views.PasswordResetView.as_view(),
-                name='admin_password_reset',
-            ),
-            path(
-                'admin/password_reset/done/',
-                auth_views.PasswordResetDoneView.as_view(),
-                name='password_reset_done',
-            ),
-            path(
-                'reset/<uidb64>/<token>/',
-                auth_views.PasswordResetConfirmView.as_view(),
-                name='password_reset_confirm',
-            ),
-            path(
-                'reset/done/',
-                auth_views.PasswordResetCompleteView.as_view(),
-                name='password_reset_complete',
-            ),
-            path('captcha/', include("captcha.urls")),
-            ...
-        ]
-        ```
-        
-        **Note:**
-        
-        1. Include captcha.urls is required so that the captcha image can be displayed.
-        1. `Reset Password Link` only shows when you enabled `admin_password_reset` views in your urls.
-        
-        ## Changes about admin/login.html
-        
-        We have override some part of admin/login.html. But the admin/login.html content may change in future releases. So you should known what part is overrided.
-        
-        1. Our new admin/login.html extends from system's admin/login.html.
-        1. We override the extrastyle block to add extra js and css.
-        1. The function adding background image and changing login box position is implemented in our new extrastyle block.
-        1. We override the whole content block.
-        1. We copied the whole content block from django's default admin/login.html.
-        1. We added blocks inside content block: form, form-row-username, from-row-password, form-row-extra, form-row-captcha, password-reset-url, before-submit-row, submit-row, after-submit-row.
-        
-        
-        
-        ## Releases
-        
-        | Release | Time | Changes                                                     | Notice |
-        | ------ | ---------- | ---------------------------------------------------------------- | ---- |
-        | v0.1.0 | 2020/03/06 | 1. First release. | |
-        | v0.2.0 | 2020/03/07 | 2. Add rsa encryption and decrption functions for password field.<br />3. Fix requirements.txt missing django-static-jquery3 problem. | |
-        | v0.3.0 | 2020/05/20 | 4. Add background image setting.<br />5. Add login box position setting.<br />6. Use admin/login.html override instead of creating a new template.<br />7. Fix document.<br />8. Fix translation.<br />9. Fix setup.py problem that include demo and example code in the final package. | |
-        | v0.3.1 | 2020/09/01 | 10. Rename zh_Hans to zh_hans.<br />11. Depends on django-static-jquery3>=5.0.0. | |
-        | v0.3.2 | 2020/09/01 | 12. Depends on django-secure-password-input>=0.1.1. | |
-        | v0.3.3 | 2020/09/24 | 13. Add app_requires.<br />14. Add License file. | |
-        | v0.3.4 | 2021/04/12 | 15. Test with django 3.2.<br />16. Auto get captcha refresh url. | |
-        
-Keywords: django admin extentions,django admin safe login
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: django-admin-safe-login
+Version: 0.3.5
+Summary: Add captcha field for django admin's login page.
+Author: zencore
+Author-email: dobetter@zencore.cn
+License: MIT
+Keywords: django admin extentions,django admin safe login
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django-admin-safe-login
+
+Add captcha field and rsa encryption password field for django admin's login page.
+
+## Install
+
+```shell
+pip install django-admin-safe-login
+```
+
+## Usage
+
+**pro/settings.py**
+
+```python
+INSTALLED_APPS = [
+    ...
+    'django_static_jquery3',
+    'django_secure_password_input',
+    'django_simple_tags',
+    'captcha',
+    'django_admin_safe_login',
+    ...
+]
+
+CAPTCHA_IMAGE_SIZE = (100, 30)  # required
+DJANGO_ADMIN_SAFE_LOGIN_ENABLE_CAPTCHA = True # optional, default to True
+DJANGO_ADMIN_SAFE_LOGIN_BACKGROUND_IMAGE = "django-admin-safe-login/img/example-background.jpg"  # optional, default to no-image.
+DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_RIGHT = "200px" # optional, default to auto
+DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_LEFT = "auto" # optional, default to auto
+DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_TOP = "100px" # optional, default to auto
+DJANGO_ADMIN_SAFE_LOGIN_BOX_MARGIN_BOTTOM = "100px" # optional, default to auto
+DJANGO_ADMIN_SAFE_LOGIN_TEMPLATE = "" # optional, default to "admin/login.html".
+```
+
+**Note:**
+
+1. Insert django_static_jquery3, django_secure_password_input, django-simple-tags, captcha and django_admin_safe_login into INSTALLED_APPS.
+1. Application django_static_jquery3 provides static jquery.js.
+1. Application django_secure_password_input provides rsa encryption and decryption function for password field.
+1. Application django_admin_safe_login provides all functions about safe login.
+1. Application captcha provides image captcha functions.
+1. Application django-simple-tags provides custom template tags used in our admin/login.html.
+1. Configuration item CAPTCHA_IMAGE_SIZE is required, and must set to (100, 30) so that it will not break the display style. If you want other size image, you have to rewrite some css code.
+1. Configurations about password RSA encryption, see details at https://pypi.org/project/django-secure-password-input/.
+1. Configurations about captcha, see detail at https://pypi.org/project/django-simple-captcha/.
+1. Configurations about password reset, see detail at https://docs.djangoproject.com/en/3.0/ref/contrib/admin/ (search: Adding a password reset feature).
+
+**pro/urls.py**
+
+```python
+from django.urls import path
+from django.urls import include
+from django.contrib.auth import views as auth_views
+
+urlpatterns = [
+    ...
+    path(
+        'admin/password_reset/',
+        auth_views.PasswordResetView.as_view(),
+        name='admin_password_reset',
+    ),
+    path(
+        'admin/password_reset/done/',
+        auth_views.PasswordResetDoneView.as_view(),
+        name='password_reset_done',
+    ),
+    path(
+        'reset/<uidb64>/<token>/',
+        auth_views.PasswordResetConfirmView.as_view(),
+        name='password_reset_confirm',
+    ),
+    path(
+        'reset/done/',
+        auth_views.PasswordResetCompleteView.as_view(),
+        name='password_reset_complete',
+    ),
+    path('captcha/', include("captcha.urls")),
+    ...
+]
+```
+
+**Note:**
+
+1. Include captcha.urls is required so that the captcha image can be displayed.
+1. `Reset Password Link` only shows when you enabled `admin_password_reset` views in your urls.
+
+## Changes about admin/login.html
+
+We have override some part of admin/login.html. But the admin/login.html content may change in future releases. So you should known what part is overrided.
+
+1. Our new admin/login.html extends from system's admin/login.html.
+1. We override the extrastyle block to add extra js and css.
+1. The function adding background image and changing login box position is implemented in our new extrastyle block.
+1. We override the whole content block.
+1. We copied the whole content block from django's default admin/login.html.
+1. We added blocks inside content block: form, form-row-username, from-row-password, form-row-extra, form-row-captcha, password-reset-url, before-submit-row, submit-row, after-submit-row.
+
+
+
+## Releases
+
+| Release | Time | Changes                                                     |
+| ------ | ---------- | ---------------------------------------------------------------- |
+| v0.1.0 | 2020/03/06 | 1. First release. |
+| v0.2.0 | 2020/03/07 | 2. Add rsa encryption and decrption functions for password field.<br />3. Fix requirements.txt missing django-static-jquery3 problem. |
+| v0.3.0 | 2020/05/20 | 4. Add background image setting.<br />5. Add login box position setting.<br />6. Use admin/login.html override instead of creating a new template.<br />7. Fix document.<br />8. Fix translation.<br />9. Fix setup.py problem that include demo and example code in the final package. |
+| v0.3.1 | 2020/09/01 | 10. Rename zh_Hans to zh_hans.<br />11. Depends on django-static-jquery3>=5.0.0. |
+| v0.3.2 | 2020/09/01 | 12. Depends on django-secure-password-input>=0.1.1. |
+| v0.3.3 | 2020/09/24 | 13. Add app_requires.<br />14. Add License file. |
+| v0.3.4 | 2021/04/12 | 15. Test with django 3.2.<br />16. Auto get captcha refresh url. |
+| v0.3.5 | 2023/04/11 | 17. Fix ugettext problem for Django 4.2. |
```

### Comparing `django-admin-safe-login-0.3.4/django_admin_safe_login.egg-info/SOURCES.txt` & `django-admin-safe-login-0.3.5/django_admin_safe_login.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-safe-login-0.3.4/setup.py` & `django-admin-safe-login-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description = fobj.read()
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="django-admin-safe-login",
-    version="0.3.4",
+    version="0.3.5",
     description="Add captcha field for django admin's login page.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="zencore",
     author_email="dobetter@zencore.cn",
     license="MIT",
     classifiers=[
```

