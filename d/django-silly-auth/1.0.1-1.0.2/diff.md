# Comparing `tmp/django-silly-auth-1.0.1.tar.gz` & `tmp/django-silly-auth-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-silly-auth-1.0.1.tar", last modified: Mon Apr 10 21:33:02 2023, max compression
+gzip compressed data, was "django-silly-auth-1.0.2.tar", last modified: Mon Apr 10 23:01:35 2023, max compression
```

## Comparing `django-silly-auth-1.0.1.tar` & `django-silly-auth-1.0.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.988087 django-silly-auth-1.0.1/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-1.0.1/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1588 2023-04-10 21:33:02.988087 django-silly-auth-1.0.1/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      978 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.964087 django-silly-auth-1.0.1/django_silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4641 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/config.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     6655 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/forms.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.968087 django-silly-auth-1.0.1/django_silly_auth/locale/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    10385 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/locale/django.pot
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.956087 django-silly-auth-1.0.1/django_silly_auth/locale/en/
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.968087 django-silly-auth-1.0.1/django_silly_auth/locale/en/LC_MESSAGES/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    10399 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.956087 django-silly-auth-1.0.1/django_silly_auth/locale/fr/
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.968087 django-silly-auth-1.0.1/django_silly_auth/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     9661 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    14409 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2473 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/mixins.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5326 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/serializers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.968087 django-silly-auth-1.0.1/django_silly_auth/templates/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/templates/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.968087 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_base.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.972087 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_test/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_test/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4497 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_test/_base.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_test/_test.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      276 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_test/_users.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.980086 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      621 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/account.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      598 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/change_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      613 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/change_username.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      388 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/index.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1156 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/login.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      570 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      583 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      870 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/reset_password.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1147 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/signup.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.984087 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/emails/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/emails/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      300 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      311 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.984087 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/silly/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/silly/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      462 2023-04-10 01:22:43.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4565 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/urls.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3696 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/utils.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.988087 django-silly-auth-1.0.1/django_silly_auth/views/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/views/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3066 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/views/api_custom_login.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      325 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/views/api_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5187 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/views/api_views_if_drf.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    13439 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/views/classics.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1775 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/views/silly_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/views/test_views.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.968087 django-silly-auth-1.0.1/django_silly_auth.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1588 2023-04-10 21:33:02.000000 django-silly-auth-1.0.1/django_silly_auth.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2244 2023-04-10 21:33:02.000000 django-silly-auth-1.0.1/django_silly_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-10 21:33:02.000000 django-silly-auth-1.0.1/django_silly_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-04-10 21:33:02.000000 django-silly-auth-1.0.1/django_silly_auth.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-04-10 21:33:02.000000 django-silly-auth-1.0.1/django_silly_auth.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-10 21:33:02.988087 django-silly-auth-1.0.1/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.929559 django-silly-auth-1.0.2/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-1.0.2/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1588 2023-04-10 23:01:35.929559 django-silly-auth-1.0.2/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      978 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.897558 django-silly-auth-1.0.2/django_silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4641 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/config.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5820 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/forms.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.901558 django-silly-auth-1.0.2/django_silly_auth/locale/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10267 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/locale/django.pot
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.889557 django-silly-auth-1.0.2/django_silly_auth/locale/en/
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.905558 django-silly-auth-1.0.2/django_silly_auth/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10281 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.889557 django-silly-auth-1.0.2/django_silly_auth/locale/fr/
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.905558 django-silly-auth-1.0.2/django_silly_auth/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     9697 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    14485 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2473 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/mixins.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5326 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/serializers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.905558 django-silly-auth-1.0.2/django_silly_auth/templates/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/templates/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.909558 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_base.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.909558 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_test/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_test/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4497 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_test/_base.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_test/_test.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      276 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_test/_users.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.917559 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      621 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/account.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      598 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/change_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      613 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/change_username.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      388 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/index.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1156 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/login.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      570 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      583 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      870 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/reset_password.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1147 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/signup.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.921559 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/emails/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/emails/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      300 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      311 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.921559 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/silly/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/silly/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      462 2023-04-10 01:22:43.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4565 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/urls.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3256 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/utils.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.925559 django-silly-auth-1.0.2/django_silly_auth/views/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/views/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3066 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/views/api_custom_login.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      325 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/views/api_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5229 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/views/api_views_if_drf.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    13542 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/views/classics.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1775 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/views/silly_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/views/test_views.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.901558 django-silly-auth-1.0.2/django_silly_auth.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1588 2023-04-10 23:01:35.000000 django-silly-auth-1.0.2/django_silly_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2244 2023-04-10 23:01:35.000000 django-silly-auth-1.0.2/django_silly_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-10 23:01:35.000000 django-silly-auth-1.0.2/django_silly_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-04-10 23:01:35.000000 django-silly-auth-1.0.2/django_silly_auth.egg-info/requires.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-04-10 23:01:35.000000 django-silly-auth-1.0.2/django_silly_auth.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-10 23:01:35.929559 django-silly-auth-1.0.2/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/setup.py
```

### Comparing `django-silly-auth-1.0.1/LICENSE.md` & `django-silly-auth-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/PKG-INFO` & `django-silly-auth-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 1.0.1
+Version: 1.0.2
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
```

### Comparing `django-silly-auth-1.0.1/README.md` & `django-silly-auth-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/config.py` & `django-silly-auth-1.0.2/django_silly_auth/config.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/forms.py` & `django-silly-auth-1.0.2/django_silly_auth/forms.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,44 +12,14 @@
 
 if conf["VERBOSE"]:
     print("=== DSA IMPORT django_silly_auth.forms")
 
 User = get_user_model()
 
 
-class NewPasswordForm(forms.Form):
-
-    password = forms.CharField(
-        max_length=64, widget=forms.PasswordInput,
-        validators=[validate_password]
-    )
-    password2 = forms.CharField(
-        label=_("Confirm password"),
-        max_length=64, widget=forms.PasswordInput,
-        validators=[validate_password]
-    )
-
-    def clean_password2(self):
-        password = self.cleaned_data['password']
-        password2 = self.cleaned_data['password2']
-        if password != password2:
-            raise ValidationError(_("The passwords you entered do not match."))
-        return password2
-
-
-class NewEmailConfirmForm(forms.Form):
-
-    password = forms.CharField(
-        max_length=64, widget=forms.PasswordInput,
-        validators=[validate_password]
-    )
-
-#################### FULL CLASSIC FORMS ####################
-
-
 class LoginForm(forms.Form):
     credential = forms.CharField(
         label=_("Username or email"),
         max_length=64,
         widget=forms.TextInput({
             'placeholder': _('Username or email'),
         })
```

### Comparing `django-silly-auth-1.0.1/django_silly_auth/locale/django.pot` & `django-silly-auth-1.0.2/django_silly_auth/locale/django.pot`

 * *Files 2% similar despite different names*

```diff
@@ -4,85 +4,85 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-10 23:25+0200\n"
+"POT-Creation-Date: 2023-04-11 00:57+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: forms.py:26 forms.py:103 forms.py:166
-msgid "Confirm password"
-msgstr ""
-
-#: forms.py:35 forms.py:182 serializers.py:73
-msgid "The passwords you entered do not match."
-msgstr ""
-
-#: forms.py:51 forms.py:54 forms.py:138 forms.py:141
+#: forms.py:21 forms.py:24 forms.py:108 forms.py:111
 msgid "Username or email"
 msgstr ""
 
-#: forms.py:58 forms.py:61 forms.py:95 forms.py:99 forms.py:107 forms.py:158
-#: forms.py:161 forms.py:169
+#: forms.py:28 forms.py:31 forms.py:65 forms.py:69 forms.py:77 forms.py:128
+#: forms.py:131 forms.py:139
 msgid "Password"
 msgstr ""
 
-#: forms.py:73
+#: forms.py:43
 #, python-brace-format
 msgid "User '{credential}' unknown or unconfirmed"
 msgstr ""
 
-#: forms.py:79 forms.py:83 forms.py:192
+#: forms.py:49 forms.py:53 forms.py:162
 msgid "Username"
 msgstr ""
 
-#: forms.py:87 forms.py:90 forms.py:212
+#: forms.py:57 forms.py:60 forms.py:182
 msgid "Email"
 msgstr ""
 
-#: forms.py:115
+#: forms.py:73 forms.py:136
+msgid "Confirm password"
+msgstr ""
+
+#: forms.py:85
 msgid "different than password"
 msgstr ""
 
-#: forms.py:121 forms.py:199 mixins.py:76 serializers.py:44
+#: forms.py:91 forms.py:169 mixins.py:76 serializers.py:44
 msgid "A username cannot include the symbol '@'."
 msgstr ""
 
-#: forms.py:125 forms.py:203
+#: forms.py:95 forms.py:173
 #, python-brace-format
 msgid "'{username}' is already taken by someone else."
 msgstr ""
 
-#: forms.py:132
+#: forms.py:102
 #, python-brace-format
 msgid "'{email}' is already taken by someone else."
 msgstr ""
 
-#: forms.py:152
+#: forms.py:122
 #, python-brace-format
 msgid "'{credential}' unknown or unconfirmed"
 msgstr ""
 
-#: forms.py:188
+#: forms.py:152 serializers.py:73
+msgid "The passwords you entered do not match."
+msgstr ""
+
+#: forms.py:158
 msgid "New username"
 msgstr ""
 
-#: forms.py:209
+#: forms.py:179
 msgid "New email address"
 msgstr ""
 
-#: forms.py:220
+#: forms.py:190
 #, python-brace-format
 msgid "'{email}' already taken by someone else."
 msgstr ""
 
 #: mixins.py:29
 msgid "username"
 msgstr ""
@@ -325,33 +325,33 @@
 "confirmation link."
 msgstr ""
 
 #: views/api_custom_login.py:50
 msgid "Incorrect credentials."
 msgstr ""
 
-#: views/api_custom_login.py:65 views/classics.py:344
+#: views/api_custom_login.py:65 views/classics.py:347
 msgid "Your account has been confirmed."
 msgstr ""
 
-#: views/api_custom_login.py:70 views/classics.py:349
+#: views/api_custom_login.py:70 views/classics.py:352
 msgid "Your new email has been confirmed."
 msgstr ""
 
 #: views/api_custom_login.py:72
 msgid ""
 "You've been logged in via email confirmation, please change your password if "
 "necessary."
 msgstr ""
 
 #: views/api_views_if_drf.py:39
 msgid "no credential provided"
 msgstr ""
 
-#: views/api_views_if_drf.py:47 views/classics.py:352
+#: views/api_views_if_drf.py:47 views/classics.py:355
 msgid "Your account is already confirmed."
 msgstr ""
 
 #: views/api_views_if_drf.py:51 views/api_views_if_drf.py:81
 msgid "Email sent for password reset"
 msgstr ""
 
@@ -363,96 +363,99 @@
 msgid "No credentials were provided"
 msgstr ""
 
 #: views/api_views_if_drf.py:82
 msgid "Invalid credential"
 msgstr ""
 
-#: views/api_views_if_drf.py:99
-#, python-brace-format
-msgid "Please check your inbox at '{user.email}' to confirm your account. "
+#: views/api_views_if_drf.py:98
+msgid "Please check your inbox at '{}' to confirm your account. "
 msgstr ""
 
-#: views/api_views_if_drf.py:104 views/classics.py:111
+#: views/api_views_if_drf.py:100
 msgid "If you do not confirm your account within the next "
 msgstr ""
 
-#: views/api_views_if_drf.py:105 views/classics.py:112
-msgid "{conf['DELETE_UNCONFIRMED_TIME']} hours, "
+#: views/api_views_if_drf.py:101
+msgid "{} hours, "
 msgstr ""
 
-#: views/api_views_if_drf.py:106 views/classics.py:113
+#: views/api_views_if_drf.py:102
 msgid "it will be deleted."
 msgstr ""
 
-#: views/api_views_if_drf.py:132
+#: views/api_views_if_drf.py:129
 msgid "Password successfully changed."
 msgstr ""
 
-#: views/api_views_if_drf.py:150
-#, python-brace-format
-msgid "New email saved, check your inbox at '{new_email}' to activate it."
+#: views/api_views_if_drf.py:147
+msgid "New email saved, check your inbox at '{}' to activate it."
 msgstr ""
 
 #: views/classics.py:58
 msgid "Incorrect credentials or unconfirmed account."
 msgstr ""
 
-#: views/classics.py:106
-#, python-brace-format
-msgid "Please check your inbox at '{user.email}' "
+#: views/classics.py:105
+msgid "Please check your inbox at"
 msgstr ""
 
 #: views/classics.py:107
 msgid "to confirm your account."
 msgstr ""
 
-#: views/classics.py:153
+#: views/classics.py:111
+msgid " If you do not confirm your account within the next "
+msgstr ""
+
+#: views/classics.py:112
+msgid "{} hours, it will be deleted."
+msgstr ""
+
+#: views/classics.py:156
 msgid ""
 "Please check your inbox and follow the instructions to reset your password."
 msgstr ""
 
-#: views/classics.py:165
+#: views/classics.py:168
 msgid ""
 "Your account is no longer active. Please contact the administrator. No email "
 "has been sent."
 msgstr ""
 
-#: views/classics.py:208 views/classics.py:335 views/silly_views.py:20
+#: views/classics.py:211 views/classics.py:338 views/silly_views.py:20
 msgid "Token invalid or expired"
 msgstr ""
 
-#: views/classics.py:224
+#: views/classics.py:227
 msgid "Your password has been successfully reset. Please log in."
 msgstr ""
 
-#: views/classics.py:241
+#: views/classics.py:244
 msgid ""
 "You have been logged in via email confirmation. Please reset your password."
 msgstr ""
 
-#: views/classics.py:265
-#, python-brace-format
-msgid "New username set: '{username}'."
+#: views/classics.py:268
+msgid "New username set: '{}'."
 msgstr ""
 
 #: views/classics.py:305
 msgid "Please check your inbox to"
 msgstr ""
 
 #: views/classics.py:306
-#, python-brace-format
-msgid " confirm your new address at '{email}'"
+msgid " confirm your new address at '{}'"
 msgstr ""
 
-#: views/classics.py:379
+#: views/classics.py:382
 msgid "Your account is already confirmed. No email has been sent."
 msgstr ""
 
-#: views/classics.py:391
+#: views/classics.py:394
 msgid "Please check your inbox to confirm your account."
 msgstr ""
 
 #: views/silly_views.py:26
 msgid "Your account has been confirmed"
 msgstr ""
```

### Comparing `django-silly-auth-1.0.1/django_silly_auth/locale/en/LC_MESSAGES/django.po` & `django-silly-auth-1.0.2/django_silly_auth/locale/en/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,85 +4,85 @@
 # Vincent Fabre <peigne.plume@gmail.com>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-10 23:25+0200\n"
+"POT-Creation-Date: 2023-04-11 00:57+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: forms.py:26 forms.py:103 forms.py:166
-msgid "Confirm password"
-msgstr ""
-
-#: forms.py:35 forms.py:182 serializers.py:73
-msgid "The passwords you entered do not match."
-msgstr ""
-
-#: forms.py:51 forms.py:54 forms.py:138 forms.py:141
+#: forms.py:21 forms.py:24 forms.py:108 forms.py:111
 msgid "Username or email"
 msgstr ""
 
-#: forms.py:58 forms.py:61 forms.py:95 forms.py:99 forms.py:107 forms.py:158
-#: forms.py:161 forms.py:169
+#: forms.py:28 forms.py:31 forms.py:65 forms.py:69 forms.py:77 forms.py:128
+#: forms.py:131 forms.py:139
 msgid "Password"
 msgstr ""
 
-#: forms.py:73
+#: forms.py:43
 #, python-brace-format
 msgid "User '{credential}' unknown or unconfirmed"
 msgstr ""
 
-#: forms.py:79 forms.py:83 forms.py:192
+#: forms.py:49 forms.py:53 forms.py:162
 msgid "Username"
 msgstr ""
 
-#: forms.py:87 forms.py:90 forms.py:212
+#: forms.py:57 forms.py:60 forms.py:182
 msgid "Email"
 msgstr ""
 
-#: forms.py:115
+#: forms.py:73 forms.py:136
+msgid "Confirm password"
+msgstr ""
+
+#: forms.py:85
 msgid "different than password"
 msgstr ""
 
-#: forms.py:121 forms.py:199 mixins.py:76 serializers.py:44
+#: forms.py:91 forms.py:169 mixins.py:76 serializers.py:44
 msgid "A username cannot include the symbol '@'."
 msgstr ""
 
-#: forms.py:125 forms.py:203
+#: forms.py:95 forms.py:173
 #, python-brace-format
 msgid "'{username}' is already taken by someone else."
 msgstr ""
 
-#: forms.py:132
+#: forms.py:102
 #, python-brace-format
 msgid "'{email}' is already taken by someone else."
 msgstr ""
 
-#: forms.py:152
+#: forms.py:122
 #, python-brace-format
 msgid "'{credential}' unknown or unconfirmed"
 msgstr ""
 
-#: forms.py:188
+#: forms.py:152 serializers.py:73
+msgid "The passwords you entered do not match."
+msgstr ""
+
+#: forms.py:158
 msgid "New username"
 msgstr ""
 
-#: forms.py:209
+#: forms.py:179
 msgid "New email address"
 msgstr ""
 
-#: forms.py:220
+#: forms.py:190
 #, python-brace-format
 msgid "'{email}' already taken by someone else."
 msgstr ""
 
 #: mixins.py:29
 msgid "username"
 msgstr ""
@@ -325,33 +325,33 @@
 "confirmation link."
 msgstr ""
 
 #: views/api_custom_login.py:50
 msgid "Incorrect credentials."
 msgstr ""
 
-#: views/api_custom_login.py:65 views/classics.py:344
+#: views/api_custom_login.py:65 views/classics.py:347
 msgid "Your account has been confirmed."
 msgstr ""
 
-#: views/api_custom_login.py:70 views/classics.py:349
+#: views/api_custom_login.py:70 views/classics.py:352
 msgid "Your new email has been confirmed."
 msgstr ""
 
 #: views/api_custom_login.py:72
 msgid ""
 "You've been logged in via email confirmation, please change your password if "
 "necessary."
 msgstr ""
 
 #: views/api_views_if_drf.py:39
 msgid "no credential provided"
 msgstr ""
 
-#: views/api_views_if_drf.py:47 views/classics.py:352
+#: views/api_views_if_drf.py:47 views/classics.py:355
 msgid "Your account is already confirmed."
 msgstr ""
 
 #: views/api_views_if_drf.py:51 views/api_views_if_drf.py:81
 msgid "Email sent for password reset"
 msgstr ""
 
@@ -363,96 +363,99 @@
 msgid "No credentials were provided"
 msgstr ""
 
 #: views/api_views_if_drf.py:82
 msgid "Invalid credential"
 msgstr ""
 
-#: views/api_views_if_drf.py:99
-#, python-brace-format
-msgid "Please check your inbox at '{user.email}' to confirm your account. "
+#: views/api_views_if_drf.py:98
+msgid "Please check your inbox at '{}' to confirm your account. "
 msgstr ""
 
-#: views/api_views_if_drf.py:104 views/classics.py:111
+#: views/api_views_if_drf.py:100
 msgid "If you do not confirm your account within the next "
 msgstr ""
 
-#: views/api_views_if_drf.py:105 views/classics.py:112
-msgid "{conf['DELETE_UNCONFIRMED_TIME']} hours, "
+#: views/api_views_if_drf.py:101
+msgid "{} hours, "
 msgstr ""
 
-#: views/api_views_if_drf.py:106 views/classics.py:113
+#: views/api_views_if_drf.py:102
 msgid "it will be deleted."
 msgstr ""
 
-#: views/api_views_if_drf.py:132
+#: views/api_views_if_drf.py:129
 msgid "Password successfully changed."
 msgstr ""
 
-#: views/api_views_if_drf.py:150
-#, python-brace-format
-msgid "New email saved, check your inbox at '{new_email}' to activate it."
+#: views/api_views_if_drf.py:147
+msgid "New email saved, check your inbox at '{}' to activate it."
 msgstr ""
 
 #: views/classics.py:58
 msgid "Incorrect credentials or unconfirmed account."
 msgstr ""
 
-#: views/classics.py:106
-#, python-brace-format
-msgid "Please check your inbox at '{user.email}' "
+#: views/classics.py:105
+msgid "Please check your inbox at"
 msgstr ""
 
 #: views/classics.py:107
 msgid "to confirm your account."
 msgstr ""
 
-#: views/classics.py:153
+#: views/classics.py:111
+msgid " If you do not confirm your account within the next "
+msgstr ""
+
+#: views/classics.py:112
+msgid "{} hours, it will be deleted."
+msgstr ""
+
+#: views/classics.py:156
 msgid ""
 "Please check your inbox and follow the instructions to reset your password."
 msgstr ""
 
-#: views/classics.py:165
+#: views/classics.py:168
 msgid ""
 "Your account is no longer active. Please contact the administrator. No email "
 "has been sent."
 msgstr ""
 
-#: views/classics.py:208 views/classics.py:335 views/silly_views.py:20
+#: views/classics.py:211 views/classics.py:338 views/silly_views.py:20
 msgid "Token invalid or expired"
 msgstr ""
 
-#: views/classics.py:224
+#: views/classics.py:227
 msgid "Your password has been successfully reset. Please log in."
 msgstr ""
 
-#: views/classics.py:241
+#: views/classics.py:244
 msgid ""
 "You have been logged in via email confirmation. Please reset your password."
 msgstr ""
 
-#: views/classics.py:265
-#, python-brace-format
-msgid "New username set: '{username}'."
+#: views/classics.py:268
+msgid "New username set: '{}'."
 msgstr ""
 
 #: views/classics.py:305
 msgid "Please check your inbox to"
 msgstr ""
 
 #: views/classics.py:306
-#, python-brace-format
-msgid " confirm your new address at '{email}'"
+msgid " confirm your new address at '{}'"
 msgstr ""
 
-#: views/classics.py:379
+#: views/classics.py:382
 msgid "Your account is already confirmed. No email has been sent."
 msgstr ""
 
-#: views/classics.py:391
+#: views/classics.py:394
 msgid "Please check your inbox to confirm your account."
 msgstr ""
 
 #: views/silly_views.py:26
 msgid "Your account has been confirmed"
 msgstr ""
```

### Comparing `django-silly-auth-1.0.1/django_silly_auth/locale/fr/LC_MESSAGES/django.mo` & `django-silly-auth-1.0.2/django_silly_auth/locale/fr/LC_MESSAGES/django.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-04-10 23:27+0200\n"
+"PO-Revision-Date: 2023-04-11 00:57+0200\n"
 "Last-Translator: Vincent Fabre <peigne.plume@gmail.com>\n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -76,16 +76,19 @@
 "\n"
 "Si vous n'avez pas de compte enregistré,\n"
 "veuillez ignorer ce message.\n"
 "\n"
 "Cordialement\n"
 "\n"
 
-msgid " confirm your new address at '{email}'"
-msgstr " confirmer votre nouvelle adresse à '{email}'"
+msgid " If you do not confirm your account within the next "
+msgstr " Si vous ne confirmez pas votre compte dans les "
+
+msgid " confirm your new address at '{}'"
+msgstr " confirmer votre nouvelle adresse à '{}'"
 
 msgid "'{credential}' unknown or unconfirmed"
 msgstr "'{credential}' inconnu ou non confirmé"
 
 msgid "'{email}' already taken by someone else."
 msgstr "'{email}' déjà utilisé par quelqu'un."
 
@@ -183,24 +186,24 @@
 "My account exists but is unconfirmed, please send me the confirmation email "
 "again."
 msgstr "J'ai un compte non confirmé, renvoyez-moi l'email de confirmation."
 
 msgid "New email address"
 msgstr "Nouvelle adresse email"
 
-msgid "New email saved, check your inbox at '{new_email}' to activate it."
+msgid "New email saved, check your inbox at '{}' to activate it."
 msgstr ""
-"Nouvel email enregistré, veuillez vérifier votre boite de réception à "
-"'{new_email}' pour l'activer."
+"Nouvel email enregistré, veuillez vérifier votre boite de réception à '{}' "
+"pour l'activer."
 
 msgid "New username"
 msgstr "Nouveau nom d'utilisateur"
 
-msgid "New username set: '{username}'."
-msgstr "Nouveau nom d'utilisateur: '{username}'."
+msgid "New username set: '{}'."
+msgstr "Nouveau nom d'utilisateur: '{}'."
 
 msgid "No credentials were provided"
 msgstr "Aucun identifiant fourni"
 
 msgid "Password"
 msgstr "Mot de passe"
 
@@ -209,21 +212,19 @@
 
 msgid ""
 "Please check your inbox and follow the instructions to reset your password."
 msgstr ""
 "Veuillez consulter votre boite mail et cliquer sur le lien fourni pour "
 "réinitialiser votre mot de passe."
 
-msgid "Please check your inbox at '{user.email}' "
-msgstr "Vérifiez votre boite de réception à '{user.email}' "
+msgid "Please check your inbox at"
+msgstr "Veuillez consulter votre boite mail à"
 
-msgid "Please check your inbox at '{user.email}' to confirm your account. "
-msgstr ""
-"Veuillez confirmer votre email à  '{user.email}' pour confirmer votre "
-"compte. "
+msgid "Please check your inbox at '{}' to confirm your account. "
+msgstr "Veuillez confirmer votre email à  '{}' pour confirmer votre compte. "
 
 msgid "Please check your inbox to"
 msgstr "Veuillez consulter votre boite mail pour"
 
 msgid "Please check your inbox to confirm your account."
 msgstr "Consultez votre boite mail pour confirmer votre compte."
 
@@ -384,9 +385,12 @@
 
 msgid "user"
 msgstr "utilisateur"
 
 msgid "username"
 msgstr "nom d'utilisateur"
 
-msgid "{conf['DELETE_UNCONFIRMED_TIME']} hours, "
-msgstr "{conf['DELETE_UNCONFIRMED_TIME']} heures, "
+msgid "{} hours, "
+msgstr "{} heures, "
+
+msgid "{} hours, it will be deleted."
+msgstr "{} heures, il sera supprimé."
```

### Comparing `django-silly-auth-1.0.1/django_silly_auth/locale/fr/LC_MESSAGES/django.po` & `django-silly-auth-1.0.2/django_silly_auth/locale/fr/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,87 +3,87 @@
 # This file is distributed under the same license as the django-silly-auth package.
 # Vincent Fabre <peigne.plume@gmail.com>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-10 23:25+0200\n"
-"PO-Revision-Date: 2023-04-10 23:27+0200\n"
+"POT-Creation-Date: 2023-04-11 00:57+0200\n"
+"PO-Revision-Date: 2023-04-11 00:57+0200\n"
 "Last-Translator: Vincent Fabre <peigne.plume@gmail.com>\n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "X-Generator: Poedit 3.0.1\n"
 
-#: forms.py:26 forms.py:103 forms.py:166
-msgid "Confirm password"
-msgstr "Confirmez le mot de passe"
-
-#: forms.py:35 forms.py:182 serializers.py:73
-msgid "The passwords you entered do not match."
-msgstr "Les mots de passe saisis ne correspondent pas."
-
-#: forms.py:51 forms.py:54 forms.py:138 forms.py:141
+#: forms.py:21 forms.py:24 forms.py:108 forms.py:111
 msgid "Username or email"
 msgstr "Nom d'utilisateur ou email"
 
-#: forms.py:58 forms.py:61 forms.py:95 forms.py:99 forms.py:107 forms.py:158
-#: forms.py:161 forms.py:169
+#: forms.py:28 forms.py:31 forms.py:65 forms.py:69 forms.py:77 forms.py:128
+#: forms.py:131 forms.py:139
 msgid "Password"
 msgstr "Mot de passe"
 
-#: forms.py:73
+#: forms.py:43
 #, python-brace-format
 msgid "User '{credential}' unknown or unconfirmed"
 msgstr "Utilisateur '{credential}' inconnu ou non confirmé"
 
-#: forms.py:79 forms.py:83 forms.py:192
+#: forms.py:49 forms.py:53 forms.py:162
 msgid "Username"
 msgstr "Nom d'utilisateur"
 
-#: forms.py:87 forms.py:90 forms.py:212
+#: forms.py:57 forms.py:60 forms.py:182
 msgid "Email"
 msgstr "Email"
 
-#: forms.py:115
+#: forms.py:73 forms.py:136
+msgid "Confirm password"
+msgstr "Confirmez le mot de passe"
+
+#: forms.py:85
 msgid "different than password"
 msgstr "mots de passe différents"
 
-#: forms.py:121 forms.py:199 mixins.py:76 serializers.py:44
+#: forms.py:91 forms.py:169 mixins.py:76 serializers.py:44
 msgid "A username cannot include the symbol '@'."
 msgstr "Un nom d'utilisateur ne peut pas inclure '@'."
 
-#: forms.py:125 forms.py:203
+#: forms.py:95 forms.py:173
 #, python-brace-format
 msgid "'{username}' is already taken by someone else."
 msgstr "'{username}' est déjà utilisé par quelqu'un."
 
-#: forms.py:132
+#: forms.py:102
 #, python-brace-format
 msgid "'{email}' is already taken by someone else."
 msgstr "'{email}' déjà utilisé par quelqu'un."
 
-#: forms.py:152
+#: forms.py:122
 #, python-brace-format
 msgid "'{credential}' unknown or unconfirmed"
 msgstr "'{credential}' inconnu ou non confirmé"
 
-#: forms.py:188
+#: forms.py:152 serializers.py:73
+msgid "The passwords you entered do not match."
+msgstr "Les mots de passe saisis ne correspondent pas."
+
+#: forms.py:158
 msgid "New username"
 msgstr "Nouveau nom d'utilisateur"
 
-#: forms.py:209
+#: forms.py:179
 msgid "New email address"
 msgstr "Nouvelle adresse email"
 
-#: forms.py:220
+#: forms.py:190
 #, python-brace-format
 msgid "'{email}' already taken by someone else."
 msgstr "'{email}' déjà utilisé par quelqu'un."
 
 #: mixins.py:29
 msgid "username"
 msgstr "nom d'utilisateur"
@@ -359,34 +359,34 @@
 "Votre compte n'a pas encore été confirmé. Veuillez vérifier votre boite mail "
 "et utiliser le lien de confirmation."
 
 #: views/api_custom_login.py:50
 msgid "Incorrect credentials."
 msgstr "Indentifiants incorrectes."
 
-#: views/api_custom_login.py:65 views/classics.py:344
+#: views/api_custom_login.py:65 views/classics.py:347
 msgid "Your account has been confirmed."
 msgstr "Votre compte a été confirmé."
 
-#: views/api_custom_login.py:70 views/classics.py:349
+#: views/api_custom_login.py:70 views/classics.py:352
 msgid "Your new email has been confirmed."
 msgstr "Votre nouvel email a été confirmé."
 
 #: views/api_custom_login.py:72
 msgid ""
 "You've been logged in via email confirmation, please change your password if "
 "necessary."
 msgstr ""
 "Connexion par email de confirmation, changez votre mot de passe si besoin."
 
 #: views/api_views_if_drf.py:39
 msgid "no credential provided"
 msgstr "aucun identifiant fourni"
 
-#: views/api_views_if_drf.py:47 views/classics.py:352
+#: views/api_views_if_drf.py:47 views/classics.py:355
 msgid "Your account is already confirmed."
 msgstr "Votre compte est déjà confirmé."
 
 #: views/api_views_if_drf.py:51 views/api_views_if_drf.py:81
 msgid "Email sent for password reset"
 msgstr "Email envoyé pour réinitialisation du mot de passe"
 
@@ -398,108 +398,109 @@
 msgid "No credentials were provided"
 msgstr "Aucun identifiant fourni"
 
 #: views/api_views_if_drf.py:82
 msgid "Invalid credential"
 msgstr "Identifiant non valide"
 
-#: views/api_views_if_drf.py:99
-#, python-brace-format
-msgid "Please check your inbox at '{user.email}' to confirm your account. "
-msgstr ""
-"Veuillez confirmer votre email à  '{user.email}' pour confirmer votre "
-"compte. "
+#: views/api_views_if_drf.py:98
+msgid "Please check your inbox at '{}' to confirm your account. "
+msgstr "Veuillez confirmer votre email à  '{}' pour confirmer votre compte. "
 
-#: views/api_views_if_drf.py:104 views/classics.py:111
+#: views/api_views_if_drf.py:100
 msgid "If you do not confirm your account within the next "
 msgstr "Si vous ne confirmez pas votre compte dans les "
 
-#: views/api_views_if_drf.py:105 views/classics.py:112
-msgid "{conf['DELETE_UNCONFIRMED_TIME']} hours, "
-msgstr "{conf['DELETE_UNCONFIRMED_TIME']} heures, "
+#: views/api_views_if_drf.py:101
+msgid "{} hours, "
+msgstr "{} heures, "
 
-#: views/api_views_if_drf.py:106 views/classics.py:113
+#: views/api_views_if_drf.py:102
 msgid "it will be deleted."
 msgstr "il sera supprimé."
 
-#: views/api_views_if_drf.py:132
+#: views/api_views_if_drf.py:129
 msgid "Password successfully changed."
 msgstr "Mot de passe changé avec succès."
 
-#: views/api_views_if_drf.py:150
-#, python-brace-format
-msgid "New email saved, check your inbox at '{new_email}' to activate it."
+#: views/api_views_if_drf.py:147
+msgid "New email saved, check your inbox at '{}' to activate it."
 msgstr ""
-"Nouvel email enregistré, veuillez vérifier votre boite de réception à "
-"'{new_email}' pour l'activer."
+"Nouvel email enregistré, veuillez vérifier votre boite de réception à '{}' "
+"pour l'activer."
 
 #: views/classics.py:58
 msgid "Incorrect credentials or unconfirmed account."
 msgstr "Identifiants incorrects ou compte non confirmé."
 
-#: views/classics.py:106
-#, python-brace-format
-msgid "Please check your inbox at '{user.email}' "
-msgstr "Vérifiez votre boite de réception à '{user.email}' "
+#: views/classics.py:105
+msgid "Please check your inbox at"
+msgstr "Veuillez consulter votre boite mail à"
 
 #: views/classics.py:107
 msgid "to confirm your account."
 msgstr "pour confirmer votre compte."
 
-#: views/classics.py:153
+#: views/classics.py:111
+msgid " If you do not confirm your account within the next "
+msgstr " Si vous ne confirmez pas votre compte dans les "
+
+#: views/classics.py:112
+msgid "{} hours, it will be deleted."
+msgstr "{} heures, il sera supprimé."
+
+#: views/classics.py:156
 msgid ""
 "Please check your inbox and follow the instructions to reset your password."
 msgstr ""
 "Veuillez consulter votre boite mail et cliquer sur le lien fourni pour "
 "réinitialiser votre mot de passe."
 
-#: views/classics.py:165
+#: views/classics.py:168
 msgid ""
 "Your account is no longer active. Please contact the administrator. No email "
 "has been sent."
 msgstr ""
 "Votre compte est inactif. Contactez l'administrateur. L'envoi de l'email a "
 "été annulé."
 
-#: views/classics.py:208 views/classics.py:335 views/silly_views.py:20
+#: views/classics.py:211 views/classics.py:338 views/silly_views.py:20
 msgid "Token invalid or expired"
 msgstr "Token invalide ou expiré"
 
-#: views/classics.py:224
+#: views/classics.py:227
 msgid "Your password has been successfully reset. Please log in."
 msgstr ""
 "Votre mot de passe a été réinitialisé avec succès. Vous pouvez vous "
 "connecter."
 
-#: views/classics.py:241
+#: views/classics.py:244
 msgid ""
 "You have been logged in via email confirmation. Please reset your password."
 msgstr ""
 "Vous avez été connecté via un email de confirmation. Réinitialisez votre mot "
 "de passe si besoin."
 
-#: views/classics.py:265
-#, python-brace-format
-msgid "New username set: '{username}'."
-msgstr "Nouveau nom d'utilisateur: '{username}'."
+#: views/classics.py:268
+msgid "New username set: '{}'."
+msgstr "Nouveau nom d'utilisateur: '{}'."
 
 #: views/classics.py:305
 msgid "Please check your inbox to"
 msgstr "Veuillez consulter votre boite mail pour"
 
 #: views/classics.py:306
-#, python-brace-format
-msgid " confirm your new address at '{email}'"
-msgstr " confirmer votre nouvelle adresse à '{email}'"
+msgid " confirm your new address at '{}'"
+msgstr " confirmer votre nouvelle adresse à '{}'"
 
-#: views/classics.py:379
+#: views/classics.py:382
 msgid "Your account is already confirmed. No email has been sent."
 msgstr "Votre compte est déjà confirmé, l'email n'est pas envoyé."
 
-#: views/classics.py:391
+#: views/classics.py:394
 msgid "Please check your inbox to confirm your account."
 msgstr "Consultez votre boite mail pour confirmer votre compte."
 
 #: views/silly_views.py:26
 msgid "Your account has been confirmed"
 msgstr "Votre compte a été confirmé"
 
@@ -511,9 +512,15 @@
 msgid "Your account has already been confirmed."
 msgstr "Votre compte a déjà été confirmé."
 
 #: views/silly_views.py:50
 msgid "Your password has been successfully reset."
 msgstr "Votre mot de passe a été réinitialisé avec succès."
 
+#~ msgid "Please check your inbox at '{}' "
+#~ msgstr "Vérifiez votre boite mail à '{}' "
+
+#~ msgid "{conf['DELETE_UNCONFIRMED_TIME']} hours, "
+#~ msgstr "{conf['DELETE_UNCONFIRMED_TIME']} heures, "
+
 #~ msgid "Lang."
 #~ msgstr "Lang."
```

### Comparing `django-silly-auth-1.0.1/django_silly_auth/mixins.py` & `django-silly-auth-1.0.2/django_silly_auth/mixins.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/serializers.py` & `django-silly-auth-1.0.2/django_silly_auth/serializers.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_base.html` & `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_base.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_test/_base.html` & `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_test/_base.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/account.html` & `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/account.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/change_email.html` & `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/change_email.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/change_username.html` & `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/change_username.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/login.html` & `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/login.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/request_password_reset.html` & `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/request_password_reset.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html` & `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/reset_password.html` & `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/reset_password.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/signup.html` & `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/signup.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/urls.py` & `django-silly-auth-1.0.2/django_silly_auth/urls.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/utils.py` & `django-silly-auth-1.0.2/django_silly_auth/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 from threading import Thread
 import time
 
 from django.conf import settings
 from django.shortcuts import reverse
 from django.core.mail import send_mail
 from django.template.loader import get_template
-from django.contrib import messages
 from django.utils.translation import gettext_lazy as _
 
 from smtplib import SMTPServerDisconnected
 
 from django_silly_auth.config import SILLY_AUTH_SETTINGS as conf
-import django_silly_auth
+
 
 if conf["VERBOSE"]:
     print("=== DSA IMPORT django_silly_auth.utils")
 
 
 def dsa_thread(func):
     """decorator that simply runs the function in parallel thread"""
@@ -79,21 +78,14 @@
     # if new_email:
     if conf["USE_SILLY"]:
         link = domain + reverse('silly_confirm_email', args=[token])
     elif conf["CONFIRMATION_METHOD"] == 'GET':
         link = domain + reverse('classic_confirm_email', args=[token])
     if conf["CONFIRMATION_METHOD"] == 'POST':
         link = conf['SPA_EMAIL_LOGIN_LINK'] + f"{token}"
-    # else:
-    #     if conf["CONFIRMATION_METHOD"] == 'GET':
-    #         link = domain + reverse('classic_confirm_email', args=[token])
-    #         if conf["AUTO_SET"] == "SILLY":
-    #             link = domain + reverse('silly_confirm_email', args=[token])
-    #     if conf["CONFIRMATION_METHOD"] == 'POST':
-    #         link = conf['SPA_EMAIL_LOGIN_LINK'] + f"{token}"
     context = {
         'user': user,
         'link': link,
         'site_name': conf["SITE_NAME"],
     }
 
     msg_text = get_template(conf["EMAIL_CONFIRM_ACCOUNT_TEMPLATE"])
```

### Comparing `django-silly-auth-1.0.1/django_silly_auth/views/api_custom_login.py` & `django-silly-auth-1.0.2/django_silly_auth/views/api_custom_login.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/views/api_views_if_drf.py` & `django-silly-auth-1.0.2/django_silly_auth/views/api_views_if_drf.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,27 +91,24 @@
         """Create a new user"""
         serializer = CreateUserSerializer(data=request.data)
         if serializer.is_valid():
             user = serializer.save()
             user.set_password(request.data['password'])
             user.save()
             delete_unconfirmed(user)
-            message = _(
-                    f"Please check your inbox at '{user.email}' "
-                    "to confirm your account. "
-            )
+            message = _("Please check your inbox at '{}' to confirm your account. ").format(user.email)
             if conf["DELETE_UNCONFIRMED_TIME"] != 0:
-                message += (
-                    _("If you do not confirm your account within the next "),
-                    _(f"{conf['DELETE_UNCONFIRMED_TIME']} hours, "),
-                    _("it will be deleted.")
-                )
+                part1 = _("If you do not confirm your account within the next "),
+                part2 = _("{} hours, ").format(conf['DELETE_UNCONFIRMED_TIME']),
+                part3 = _("it will be deleted.")
+                message = "{}{}{}{}".format(message, part1, part2, part3)
             serializer = GetAllUsersSerializer(user)
             msg = {
                 "user": serializer.data,
+                "message": message,
             }
 
             send_confirm_email(request, user)
 
             return Response(msg)
         else:
             msg = serializer.errors
@@ -143,10 +140,10 @@
     if serializer.is_valid():
         new_email = request.data.get('email')
         user.new_email = new_email
         user.save()
         send_confirm_email(request, user, new_email=True)
 
         return Response(
-            {'success': _(f"New email saved, check your inbox at '{new_email}' to activate it.")})
+            {'success': _("New email saved, check your inbox at '{}' to activate it.").format(new_email)})
     msg = serializer.errors
     raise ValidationError({"error": msg}, code='authorization')
```

### Comparing `django-silly-auth-1.0.1/django_silly_auth/views/classics.py` & `django-silly-auth-1.0.2/django_silly_auth/views/classics.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,24 +98,27 @@
             email = form.cleaned_data['email']
             password = form.cleaned_data['password']
             user = User(username=username, email=email, is_active=True)
             user.set_password(password)
             user.save()
             send_confirm_email(request, user)
             delete_unconfirmed(user)
-            message = (
-                    _(f"Please check your inbox at '{user.email}' "),
-                    _("to confirm your account.")
-            )
+            part1 = _("Please check your inbox at")
+            part2 = f" '{user.email}' "
+            part3 = _("to confirm your account.")
+
             if conf["DELETE_UNCONFIRMED_TIME"] != 0.0:
-                message += (
-                    _("If you do not confirm your account within the next "),
-                    _(f"{conf['DELETE_UNCONFIRMED_TIME']} hours, "),
-                    _("it will be deleted.")
-                )
+
+                part4 = _(" If you do not confirm your account within the next ")
+                part5 = _("{} hours, it will be deleted.").format(conf['DELETE_UNCONFIRMED_TIME'])
+            else:
+                part4 = part5 = ""
+
+            message = "{}{}{}{}{}".format(part1, part2, part3, part4, part5)
+
             messages.add_message(
                 request, messages.INFO,
                 message=message,
                 extra_tags="info"
             )
             return redirect('classic_login')
         else:
@@ -258,15 +261,15 @@
         if form.is_valid():
             username = form.cleaned_data['username']
             user = request.user
             user.username = username
             user.save()
             messages.add_message(
                 request, messages.SUCCESS,
-                message=_(f"New username set: '{username}'."),
+                message=_("New username set: '{}'.").format(username),
                 extra_tags="success"
             )
             return redirect("classic_account")
         else:
             context = {
                 'form': form,
                 "base_template": conf["BASE_TEMPLATE"],
@@ -295,20 +298,20 @@
         if form.is_valid():
             email = form.cleaned_data['email']
             user = request.user
             user.new_email = email
             user.save()
             send_confirm_email(request, user)
 
+            part1 = _("Please check your inbox to"),
+            part2 = _(" confirm your new address at '{}'").format(email)
+            message = "{}{}.".format(part1, part2)
             messages.add_message(
                 request, messages.INFO,
-                message=(
-                    _("Please check your inbox to"),
-                    _(f" confirm your new address at '{email}'")
-                    ),
+                message,
                 extra_tags="info"
             )
             return redirect("classic_account")
         else:
             context = {
                 'form': form,
                 "base_template": conf["BASE_TEMPLATE"],
```

### Comparing `django-silly-auth-1.0.1/django_silly_auth/views/silly_views.py` & `django-silly-auth-1.0.2/django_silly_auth/views/silly_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth/views/test_views.py` & `django-silly-auth-1.0.2/django_silly_auth/views/test_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/django_silly_auth.egg-info/PKG-INFO` & `django-silly-auth-1.0.2/django_silly_auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 1.0.1
+Version: 1.0.2
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
```

### Comparing `django-silly-auth-1.0.1/django_silly_auth.egg-info/SOURCES.txt` & `django-silly-auth-1.0.2/django_silly_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.1/setup.py` & `django-silly-auth-1.0.2/setup.py`

 * *Files identical despite different names*

