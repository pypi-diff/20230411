# Comparing `tmp/django-silly-auth-1.0.2.tar.gz` & `tmp/django-silly-auth-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-silly-auth-1.0.2.tar", last modified: Mon Apr 10 23:01:35 2023, max compression
+gzip compressed data, was "django-silly-auth-1.0.3.tar", last modified: Tue Apr 11 19:05:34 2023, max compression
```

## Comparing `django-silly-auth-1.0.2.tar` & `django-silly-auth-1.0.3.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.929559 django-silly-auth-1.0.2/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-1.0.2/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1588 2023-04-10 23:01:35.929559 django-silly-auth-1.0.2/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      978 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.897558 django-silly-auth-1.0.2/django_silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4641 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/config.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5820 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/forms.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.901558 django-silly-auth-1.0.2/django_silly_auth/locale/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    10267 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/locale/django.pot
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.889557 django-silly-auth-1.0.2/django_silly_auth/locale/en/
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.905558 django-silly-auth-1.0.2/django_silly_auth/locale/en/LC_MESSAGES/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    10281 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.889557 django-silly-auth-1.0.2/django_silly_auth/locale/fr/
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.905558 django-silly-auth-1.0.2/django_silly_auth/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     9697 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    14485 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2473 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/mixins.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5326 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/serializers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.905558 django-silly-auth-1.0.2/django_silly_auth/templates/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/templates/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.909558 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_base.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.909558 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_test/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_test/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4497 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_test/_base.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_test/_test.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      276 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_test/_users.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.917559 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      621 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/account.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      598 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/change_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      613 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/change_username.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      388 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/index.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1156 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/login.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      570 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      583 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      870 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/reset_password.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1147 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/signup.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.921559 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/emails/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/emails/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      300 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      311 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.921559 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/silly/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/silly/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      462 2023-04-10 01:22:43.000000 django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4565 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/urls.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3256 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/utils.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.925559 django-silly-auth-1.0.2/django_silly_auth/views/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/views/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3066 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/views/api_custom_login.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      325 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/views/api_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5229 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/views/api_views_if_drf.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    13542 2023-04-10 23:00:33.000000 django-silly-auth-1.0.2/django_silly_auth/views/classics.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1775 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/django_silly_auth/views/silly_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-10 01:52:00.000000 django-silly-auth-1.0.2/django_silly_auth/views/test_views.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 23:01:35.901558 django-silly-auth-1.0.2/django_silly_auth.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1588 2023-04-10 23:01:35.000000 django-silly-auth-1.0.2/django_silly_auth.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2244 2023-04-10 23:01:35.000000 django-silly-auth-1.0.2/django_silly_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-10 23:01:35.000000 django-silly-auth-1.0.2/django_silly_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-04-10 23:01:35.000000 django-silly-auth-1.0.2/django_silly_auth.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-04-10 23:01:35.000000 django-silly-auth-1.0.2/django_silly_auth.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-10 23:01:35.929559 django-silly-auth-1.0.2/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.2/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.828432 django-silly-auth-1.0.3/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-1.0.3/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1591 2023-04-11 19:05:34.828432 django-silly-auth-1.0.3/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      981 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.820432 django-silly-auth-1.0.3/django_silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4732 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/config.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6302 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/forms.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.820432 django-silly-auth-1.0.3/django_silly_auth/locale/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10296 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/locale/django.pot
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.816431 django-silly-auth-1.0.3/django_silly_auth/locale/en/
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.820432 django-silly-auth-1.0.3/django_silly_auth/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      337 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10310 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.816431 django-silly-auth-1.0.3/django_silly_auth/locale/fr/
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.824432 django-silly-auth-1.0.3/django_silly_auth/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     9766 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    15445 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2473 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/mixins.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5326 2023-04-11 18:50:34.000000 django-silly-auth-1.0.3/django_silly_auth/serializers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.824432 django-silly-auth-1.0.3/django_silly_auth/templates/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/templates/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.824432 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_base.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.824432 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_test/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_test/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4497 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_test/_base.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_test/_test.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      276 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_test/_users.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.824432 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      621 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/account.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      598 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/change_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      613 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/change_username.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      388 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/index.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1156 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/login.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      570 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      583 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      870 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/reset_password.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1147 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/signup.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.828432 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/emails/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/emails/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      300 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      311 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.828432 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/silly/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/silly/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      497 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4565 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/urls.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3256 2023-04-11 18:51:15.000000 django-silly-auth-1.0.3/django_silly_auth/utils.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.828432 django-silly-auth-1.0.3/django_silly_auth/views/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/views/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3066 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/views/api_custom_login.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      325 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/views/api_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5459 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/views/api_views_if_drf.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    13685 2023-04-11 19:05:08.000000 django-silly-auth-1.0.3/django_silly_auth/views/classics.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1775 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/django_silly_auth/views/silly_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-10 01:52:00.000000 django-silly-auth-1.0.3/django_silly_auth/views/test_views.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-11 19:05:34.820432 django-silly-auth-1.0.3/django_silly_auth.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1591 2023-04-11 19:05:34.000000 django-silly-auth-1.0.3/django_silly_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2294 2023-04-11 19:05:34.000000 django-silly-auth-1.0.3/django_silly_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-11 19:05:34.000000 django-silly-auth-1.0.3/django_silly_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-04-11 19:05:34.000000 django-silly-auth-1.0.3/django_silly_auth.egg-info/requires.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-04-11 19:05:34.000000 django-silly-auth-1.0.3/django_silly_auth.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-11 19:05:34.828432 django-silly-auth-1.0.3/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.3/setup.py
```

### Comparing `django-silly-auth-1.0.2/LICENSE.md` & `django-silly-auth-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/PKG-INFO` & `django-silly-auth-1.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 1.0.2
+Version: 1.0.3
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
@@ -13,20 +13,20 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# Django Silly Auth (v1.0.0)
+# Django Silly Auth
 
 ## Why one more authentication system for Django and DRF? again !
 
 I've used a few ones, and did not find the one that behaves the way I want,
-efficient, but flexible, I want to win time, and get what I need straight to the point.
+efficient, but flexible, I wanted to gain som time, and get what I need straight to the point.
 
 The aim of DSA it to provide a good-enough-to-go authentication out of the box, but still remains highly
 modular through its SILLY_AUTH config in **settings.py**, so it is always possible to improve your
 authentication when you have the time for it.
 
 ## DRF and Django Classic supported
 DSA works as well with both DRF and Classic, just use differents simple settings, and you're done.
@@ -38,10 +38,11 @@
 
 ## [Read this FIRST](https://github.com/byoso/django_silly_auth/wiki/Must-read-this-few-lines-!)
 
 ### :coffee: [If you find this package usefull, consider buying me a coffee](https://www.buymeacoffee.com/byoso)
 
 
 ### Changelog
-- 1.0.1: i18n fr + en
+
+- 1.0.1: **i18n** fr + en
```

### Comparing `django-silly-auth-1.0.2/README.md` & `django-silly-auth-1.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Django Silly Auth (v1.0.0)
+# Django Silly Auth
 
 ## Why one more authentication system for Django and DRF? again !
 
 I've used a few ones, and did not find the one that behaves the way I want,
-efficient, but flexible, I want to win time, and get what I need straight to the point.
+efficient, but flexible, I wanted to gain som time, and get what I need straight to the point.
 
 The aim of DSA it to provide a good-enough-to-go authentication out of the box, but still remains highly
 modular through its SILLY_AUTH config in **settings.py**, so it is always possible to improve your
 authentication when you have the time for it.
 
 ## DRF and Django Classic supported
 DSA works as well with both DRF and Classic, just use differents simple settings, and you're done.
@@ -19,8 +19,9 @@
 
 ## [Read this FIRST](https://github.com/byoso/django_silly_auth/wiki/Must-read-this-few-lines-!)
 
 ### :coffee: [If you find this package usefull, consider buying me a coffee](https://www.buymeacoffee.com/byoso)
 
 
 ### Changelog
-- 1.0.1: i18n fr + en
+
+- 1.0.1: **i18n** fr + en
```

### Comparing `django-silly-auth-1.0.2/django_silly_auth/config.py` & `django-silly-auth-1.0.3/django_silly_auth/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class SillyAuthError(Exception):
     pass
 
 
 SILLY_AUTH_SETTINGS = {
     # Quick settings
     "AUTO_SET": 'TEST',  # 'CLASSIC', 'SPA', 'SILLY or 'TEST'
-    "DSA_PREFIX": 'auth/',
+    "DSA_PREFIX": 'auth/',  # only the CLASSIC_INDEX view has a blank prefix, it's the entry point in a classic site.
 
     # Secondary settings
     "SITE_NAME": None,  # str used in templates if provided
     "DELETE_UNCONFIRMED_TIME": 24.0,  # hours after what an unconfirmed account is deleted, O to set off
 
     # Classic settings
     "USE_CLASSIC": True,
```

### Comparing `django-silly-auth-1.0.2/django_silly_auth/forms.py` & `django-silly-auth-1.0.3/django_silly_auth/forms.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,18 @@
     def clean_login(self):
         credential = self.cleaned_data['credential']
         if "@" in credential:
             user = User.objects.filter(email=credential)
         else:
             user = User.objects.filter(username=credential)
         if not user or not user[0].is_confirmed:
-            raise ValidationError(_(f"User '{credential}' unknown or unconfirmed"))
+            raise ValidationError(_(
+                "User '%(credential)s' unknown or unconfirmed"
+                ) % {"credential": credential}
+                )
         return credential
 
 
 class SignUpForm(forms.Form):
     username = forms.CharField(
         label=_("Username"),
         validators=[MinLengthValidator(4), MaxLengthValidator(64)],
@@ -88,22 +91,28 @@
     def clean_username(self):
         username = self.cleaned_data['username']
         if "@" in username:
             raise ValidationError(_("A username cannot include the symbol '@'."))
         else:
             user = User.objects.filter(username=username)
             if user:
-                raise ValidationError(_(f"'{username}' is already taken by someone else."))
+                raise ValidationError(_(
+                    "'%(username)s' is already taken by someone else."
+                    ) % {"username": username}
+                    )
         return username
 
     def clean_email(self):
         email = self.cleaned_data['email']
         user = User.objects.filter(email=email)
         if user:
-            raise ValidationError(_(f"'{email}' is already taken by someone else."))
+            raise ValidationError(_(
+                "'%(email)s' is already taken by someone else."
+                ) % {"email": email}
+                )
         return email
 
 
 class CredentialForm(forms.Form):
     credential = forms.CharField(
         label=_("Username or email"),
         validators=[],
@@ -115,15 +124,18 @@
     def clean_credential(self):
         credential = self.cleaned_data['credential']
         if "@" in credential:
             user = User.objects.filter(email=credential)
         else:
             user = User.objects.filter(username=credential)
         if not user:
-            raise ValidationError(_(f"'{credential}' unknown or unconfirmed"))
+            raise ValidationError(_(
+                "'%(credential)s' unknown or unconfirmed"
+                ) % {"credential": credential}
+                )
         return credential
 
 
 class ResetPasswordForm(forms.Form):
     password = forms.CharField(
         label=_("Password"),
         max_length=64,
@@ -166,15 +178,18 @@
     def clean_username(self):
         username = self.cleaned_data['username']
         if "@" in username:
             raise ValidationError(_("A username cannot include the symbol '@'."))
         else:
             user = User.objects.filter(username=username)
             if user:
-                raise ValidationError(_(f"'{username}' is already taken by someone else."))
+                raise ValidationError(_(
+                    "'%(username)s' is already taken by someone else."
+                    ) % {"username": username}
+                    )
         return username
 
 
 class ChangeEmailForm(forms.Form):
     email = forms.EmailField(
         label=_("New email address"),
         validators=[EmailValidator()],
@@ -183,9 +198,12 @@
         }),
         )
 
     def clean_email(self):
         email = self.cleaned_data['email']
         user = User.objects.filter(email=email)
         if user:
-            raise ValidationError(_(f"'{email}' already taken by someone else."))
+            raise ValidationError(_(
+                "'%(email)s' already taken by someone else."
+                ) % {"email": email}
+                )
         return email
```

### Comparing `django-silly-auth-1.0.2/django_silly_auth/locale/django.pot` & `django-silly-auth-1.0.3/django_silly_auth/locale/django.pot`

 * *Files 3% similar despite different names*

```diff
@@ -4,87 +4,87 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 00:57+0200\n"
+"POT-Creation-Date: 2023-04-11 21:00+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: forms.py:21 forms.py:24 forms.py:108 forms.py:111
+#: forms.py:21 forms.py:24 forms.py:117 forms.py:120
 msgid "Username or email"
 msgstr ""
 
-#: forms.py:28 forms.py:31 forms.py:65 forms.py:69 forms.py:77 forms.py:128
-#: forms.py:131 forms.py:139
+#: forms.py:28 forms.py:31 forms.py:68 forms.py:72 forms.py:80 forms.py:140
+#: forms.py:143 forms.py:151
 msgid "Password"
 msgstr ""
 
-#: forms.py:43
-#, python-brace-format
-msgid "User '{credential}' unknown or unconfirmed"
+#: forms.py:44
+#, python-format
+msgid "User '%(credential)s' unknown or unconfirmed"
 msgstr ""
 
-#: forms.py:49 forms.py:53 forms.py:162
+#: forms.py:52 forms.py:56 forms.py:174
 msgid "Username"
 msgstr ""
 
-#: forms.py:57 forms.py:60 forms.py:182
+#: forms.py:60 forms.py:63 forms.py:197
 msgid "Email"
 msgstr ""
 
-#: forms.py:73 forms.py:136
+#: forms.py:76 forms.py:148
 msgid "Confirm password"
 msgstr ""
 
-#: forms.py:85
+#: forms.py:88
 msgid "different than password"
 msgstr ""
 
-#: forms.py:91 forms.py:169 mixins.py:76 serializers.py:44
+#: forms.py:94 forms.py:181 mixins.py:76 serializers.py:44
 msgid "A username cannot include the symbol '@'."
 msgstr ""
 
-#: forms.py:95 forms.py:173
-#, python-brace-format
-msgid "'{username}' is already taken by someone else."
+#: forms.py:99 forms.py:186
+#, python-format
+msgid "'%(username)s' is already taken by someone else."
 msgstr ""
 
-#: forms.py:102
-#, python-brace-format
-msgid "'{email}' is already taken by someone else."
+#: forms.py:109
+#, python-format
+msgid "'%(email)s' is already taken by someone else."
 msgstr ""
 
-#: forms.py:122
-#, python-brace-format
-msgid "'{credential}' unknown or unconfirmed"
+#: forms.py:132
+#, python-format
+msgid "'%(credential)s' unknown or unconfirmed"
 msgstr ""
 
-#: forms.py:152 serializers.py:73
+#: forms.py:164 serializers.py:73
 msgid "The passwords you entered do not match."
 msgstr ""
 
-#: forms.py:158
+#: forms.py:170
 msgid "New username"
 msgstr ""
 
-#: forms.py:179
+#: forms.py:194
 msgid "New email address"
 msgstr ""
 
-#: forms.py:190
-#, python-brace-format
-msgid "'{email}' already taken by someone else."
+#: forms.py:206
+#, python-format
+msgid "'%(email)s' already taken by someone else."
 msgstr ""
 
 #: mixins.py:29
 msgid "username"
 msgstr ""
 
 #: mixins.py:33
@@ -315,43 +315,47 @@
 "\n"
 "If you did not request a password reset, please ignore this message.\n"
 "\n"
 "Best regards\n"
 "\n"
 msgstr ""
 
+#: templates/silly_auth/silly/silly_confirm_email.html:11
+msgid "Account Confirmation"
+msgstr ""
+
 #: views/api_custom_login.py:45
 msgid ""
 "Your account has not been confirmed yet. Please check your inbox for a "
 "confirmation link."
 msgstr ""
 
 #: views/api_custom_login.py:50
 msgid "Incorrect credentials."
 msgstr ""
 
-#: views/api_custom_login.py:65 views/classics.py:347
+#: views/api_custom_login.py:65 views/classics.py:354
 msgid "Your account has been confirmed."
 msgstr ""
 
-#: views/api_custom_login.py:70 views/classics.py:352
+#: views/api_custom_login.py:70 views/classics.py:359
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
 
-#: views/api_views_if_drf.py:47 views/classics.py:355
+#: views/api_views_if_drf.py:47 views/classics.py:362
 msgid "Your account is already confirmed."
 msgstr ""
 
 #: views/api_views_if_drf.py:51 views/api_views_if_drf.py:81
 msgid "Email sent for password reset"
 msgstr ""
 
@@ -363,99 +367,90 @@
 msgid "No credentials were provided"
 msgstr ""
 
 #: views/api_views_if_drf.py:82
 msgid "Invalid credential"
 msgstr ""
 
-#: views/api_views_if_drf.py:98
-msgid "Please check your inbox at '{}' to confirm your account. "
-msgstr ""
-
-#: views/api_views_if_drf.py:100
-msgid "If you do not confirm your account within the next "
-msgstr ""
-
-#: views/api_views_if_drf.py:101
-msgid "{} hours, "
+#: views/api_views_if_drf.py:99
+#, python-format
+msgid "Please check your inbox at '%(email)s' to confirm your account. "
 msgstr ""
 
-#: views/api_views_if_drf.py:102
-msgid "it will be deleted."
+#: views/api_views_if_drf.py:103
+#, python-format
+msgid ""
+"If you do not confirm your account within the next %(hours)s hours, it will "
+"be deleted."
 msgstr ""
 
-#: views/api_views_if_drf.py:129
+#: views/api_views_if_drf.py:136
 msgid "Password successfully changed."
 msgstr ""
 
-#: views/api_views_if_drf.py:147
-msgid "New email saved, check your inbox at '{}' to activate it."
+#: views/api_views_if_drf.py:155
+#, python-format
+msgid "New email saved, check your inbox at '%(new_email)s' to activate it."
 msgstr ""
 
 #: views/classics.py:58
 msgid "Incorrect credentials or unconfirmed account."
 msgstr ""
 
-#: views/classics.py:105
-msgid "Please check your inbox at"
-msgstr ""
-
 #: views/classics.py:107
-msgid "to confirm your account."
-msgstr ""
-
-#: views/classics.py:111
-msgid " If you do not confirm your account within the next "
+#, python-format
+msgid "Please check your inbox at '%(email)s' to confirm your account."
 msgstr ""
 
-#: views/classics.py:112
-msgid "{} hours, it will be deleted."
+#: views/classics.py:114
+#, python-format
+msgid ""
+" If you do not confirm your account within the next %(time)s hours, it will "
+"be deleted."
 msgstr ""
 
-#: views/classics.py:156
+#: views/classics.py:161
 msgid ""
 "Please check your inbox and follow the instructions to reset your password."
 msgstr ""
 
-#: views/classics.py:168
+#: views/classics.py:173
 msgid ""
 "Your account is no longer active. Please contact the administrator. No email "
 "has been sent."
 msgstr ""
 
-#: views/classics.py:211 views/classics.py:338 views/silly_views.py:20
+#: views/classics.py:216 views/classics.py:345 views/silly_views.py:20
 msgid "Token invalid or expired"
 msgstr ""
 
-#: views/classics.py:227
+#: views/classics.py:232
 msgid "Your password has been successfully reset. Please log in."
 msgstr ""
 
-#: views/classics.py:244
+#: views/classics.py:249
 msgid ""
 "You have been logged in via email confirmation. Please reset your password."
 msgstr ""
 
-#: views/classics.py:268
-msgid "New username set: '{}'."
-msgstr ""
-
-#: views/classics.py:305
-msgid "Please check your inbox to"
+#: views/classics.py:274
+#, python-format
+msgid "New username set: '%(username)s'."
 msgstr ""
 
-#: views/classics.py:306
-msgid " confirm your new address at '{}'"
+#: views/classics.py:313
+#, python-format
+msgid "Please check your inbox to confirm your new address at '%(email)s'"
 msgstr ""
 
-#: views/classics.py:382
+#: views/classics.py:389
 msgid "Your account is already confirmed. No email has been sent."
 msgstr ""
 
-#: views/classics.py:394
+#: views/classics.py:401
 msgid "Please check your inbox to confirm your account."
 msgstr ""
 
 #: views/silly_views.py:26
 msgid "Your account has been confirmed"
 msgstr ""
```

### Comparing `django-silly-auth-1.0.2/django_silly_auth/locale/en/LC_MESSAGES/django.po` & `django-silly-auth-1.0.3/django_silly_auth/locale/en/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,87 +4,87 @@
 # Vincent Fabre <peigne.plume@gmail.com>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 00:57+0200\n"
+"POT-Creation-Date: 2023-04-11 21:00+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: forms.py:21 forms.py:24 forms.py:108 forms.py:111
+#: forms.py:21 forms.py:24 forms.py:117 forms.py:120
 msgid "Username or email"
 msgstr ""
 
-#: forms.py:28 forms.py:31 forms.py:65 forms.py:69 forms.py:77 forms.py:128
-#: forms.py:131 forms.py:139
+#: forms.py:28 forms.py:31 forms.py:68 forms.py:72 forms.py:80 forms.py:140
+#: forms.py:143 forms.py:151
 msgid "Password"
 msgstr ""
 
-#: forms.py:43
-#, python-brace-format
-msgid "User '{credential}' unknown or unconfirmed"
+#: forms.py:44
+#, python-format
+msgid "User '%(credential)s' unknown or unconfirmed"
 msgstr ""
 
-#: forms.py:49 forms.py:53 forms.py:162
+#: forms.py:52 forms.py:56 forms.py:174
 msgid "Username"
 msgstr ""
 
-#: forms.py:57 forms.py:60 forms.py:182
+#: forms.py:60 forms.py:63 forms.py:197
 msgid "Email"
 msgstr ""
 
-#: forms.py:73 forms.py:136
+#: forms.py:76 forms.py:148
 msgid "Confirm password"
 msgstr ""
 
-#: forms.py:85
+#: forms.py:88
 msgid "different than password"
 msgstr ""
 
-#: forms.py:91 forms.py:169 mixins.py:76 serializers.py:44
+#: forms.py:94 forms.py:181 mixins.py:76 serializers.py:44
 msgid "A username cannot include the symbol '@'."
 msgstr ""
 
-#: forms.py:95 forms.py:173
-#, python-brace-format
-msgid "'{username}' is already taken by someone else."
+#: forms.py:99 forms.py:186
+#, python-format
+msgid "'%(username)s' is already taken by someone else."
 msgstr ""
 
-#: forms.py:102
-#, python-brace-format
-msgid "'{email}' is already taken by someone else."
+#: forms.py:109
+#, python-format
+msgid "'%(email)s' is already taken by someone else."
 msgstr ""
 
-#: forms.py:122
-#, python-brace-format
-msgid "'{credential}' unknown or unconfirmed"
+#: forms.py:132
+#, python-format
+msgid "'%(credential)s' unknown or unconfirmed"
 msgstr ""
 
-#: forms.py:152 serializers.py:73
+#: forms.py:164 serializers.py:73
 msgid "The passwords you entered do not match."
 msgstr ""
 
-#: forms.py:158
+#: forms.py:170
 msgid "New username"
 msgstr ""
 
-#: forms.py:179
+#: forms.py:194
 msgid "New email address"
 msgstr ""
 
-#: forms.py:190
-#, python-brace-format
-msgid "'{email}' already taken by someone else."
+#: forms.py:206
+#, python-format
+msgid "'%(email)s' already taken by someone else."
 msgstr ""
 
 #: mixins.py:29
 msgid "username"
 msgstr ""
 
 #: mixins.py:33
@@ -315,43 +315,47 @@
 "\n"
 "If you did not request a password reset, please ignore this message.\n"
 "\n"
 "Best regards\n"
 "\n"
 msgstr ""
 
+#: templates/silly_auth/silly/silly_confirm_email.html:11
+msgid "Account Confirmation"
+msgstr ""
+
 #: views/api_custom_login.py:45
 msgid ""
 "Your account has not been confirmed yet. Please check your inbox for a "
 "confirmation link."
 msgstr ""
 
 #: views/api_custom_login.py:50
 msgid "Incorrect credentials."
 msgstr ""
 
-#: views/api_custom_login.py:65 views/classics.py:347
+#: views/api_custom_login.py:65 views/classics.py:354
 msgid "Your account has been confirmed."
 msgstr ""
 
-#: views/api_custom_login.py:70 views/classics.py:352
+#: views/api_custom_login.py:70 views/classics.py:359
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
 
-#: views/api_views_if_drf.py:47 views/classics.py:355
+#: views/api_views_if_drf.py:47 views/classics.py:362
 msgid "Your account is already confirmed."
 msgstr ""
 
 #: views/api_views_if_drf.py:51 views/api_views_if_drf.py:81
 msgid "Email sent for password reset"
 msgstr ""
 
@@ -363,99 +367,90 @@
 msgid "No credentials were provided"
 msgstr ""
 
 #: views/api_views_if_drf.py:82
 msgid "Invalid credential"
 msgstr ""
 
-#: views/api_views_if_drf.py:98
-msgid "Please check your inbox at '{}' to confirm your account. "
-msgstr ""
-
-#: views/api_views_if_drf.py:100
-msgid "If you do not confirm your account within the next "
-msgstr ""
-
-#: views/api_views_if_drf.py:101
-msgid "{} hours, "
+#: views/api_views_if_drf.py:99
+#, python-format
+msgid "Please check your inbox at '%(email)s' to confirm your account. "
 msgstr ""
 
-#: views/api_views_if_drf.py:102
-msgid "it will be deleted."
+#: views/api_views_if_drf.py:103
+#, python-format
+msgid ""
+"If you do not confirm your account within the next %(hours)s hours, it will "
+"be deleted."
 msgstr ""
 
-#: views/api_views_if_drf.py:129
+#: views/api_views_if_drf.py:136
 msgid "Password successfully changed."
 msgstr ""
 
-#: views/api_views_if_drf.py:147
-msgid "New email saved, check your inbox at '{}' to activate it."
+#: views/api_views_if_drf.py:155
+#, python-format
+msgid "New email saved, check your inbox at '%(new_email)s' to activate it."
 msgstr ""
 
 #: views/classics.py:58
 msgid "Incorrect credentials or unconfirmed account."
 msgstr ""
 
-#: views/classics.py:105
-msgid "Please check your inbox at"
-msgstr ""
-
 #: views/classics.py:107
-msgid "to confirm your account."
-msgstr ""
-
-#: views/classics.py:111
-msgid " If you do not confirm your account within the next "
+#, python-format
+msgid "Please check your inbox at '%(email)s' to confirm your account."
 msgstr ""
 
-#: views/classics.py:112
-msgid "{} hours, it will be deleted."
+#: views/classics.py:114
+#, python-format
+msgid ""
+" If you do not confirm your account within the next %(time)s hours, it will "
+"be deleted."
 msgstr ""
 
-#: views/classics.py:156
+#: views/classics.py:161
 msgid ""
 "Please check your inbox and follow the instructions to reset your password."
 msgstr ""
 
-#: views/classics.py:168
+#: views/classics.py:173
 msgid ""
 "Your account is no longer active. Please contact the administrator. No email "
 "has been sent."
 msgstr ""
 
-#: views/classics.py:211 views/classics.py:338 views/silly_views.py:20
+#: views/classics.py:216 views/classics.py:345 views/silly_views.py:20
 msgid "Token invalid or expired"
 msgstr ""
 
-#: views/classics.py:227
+#: views/classics.py:232
 msgid "Your password has been successfully reset. Please log in."
 msgstr ""
 
-#: views/classics.py:244
+#: views/classics.py:249
 msgid ""
 "You have been logged in via email confirmation. Please reset your password."
 msgstr ""
 
-#: views/classics.py:268
-msgid "New username set: '{}'."
-msgstr ""
-
-#: views/classics.py:305
-msgid "Please check your inbox to"
+#: views/classics.py:274
+#, python-format
+msgid "New username set: '%(username)s'."
 msgstr ""
 
-#: views/classics.py:306
-msgid " confirm your new address at '{}'"
+#: views/classics.py:313
+#, python-format
+msgid "Please check your inbox to confirm your new address at '%(email)s'"
 msgstr ""
 
-#: views/classics.py:382
+#: views/classics.py:389
 msgid "Your account is already confirmed. No email has been sent."
 msgstr ""
 
-#: views/classics.py:394
+#: views/classics.py:401
 msgid "Please check your inbox to confirm your account."
 msgstr ""
 
 #: views/silly_views.py:26
 msgid "Your account has been confirmed"
 msgstr ""
```

### Comparing `django-silly-auth-1.0.2/django_silly_auth/locale/fr/LC_MESSAGES/django.mo` & `django-silly-auth-1.0.3/django_silly_auth/locale/fr/LC_MESSAGES/django.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-04-11 00:57+0200\n"
+"PO-Revision-Date: 2023-04-11 21:01+0200\n"
 "Last-Translator: Vincent Fabre <peigne.plume@gmail.com>\n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -76,41 +76,45 @@
 "\n"
 "Si vous n'avez pas de compte enregistré,\n"
 "veuillez ignorer ce message.\n"
 "\n"
 "Cordialement\n"
 "\n"
 
-msgid " If you do not confirm your account within the next "
-msgstr " Si vous ne confirmez pas votre compte dans les "
-
-msgid " confirm your new address at '{}'"
-msgstr " confirmer votre nouvelle adresse à '{}'"
+msgid ""
+" If you do not confirm your account within the next %(time)s hours, it will "
+"be deleted."
+msgstr ""
+" Si vous ne confirmez pas votre compte dans les %(time)s heures, il sera "
+"supprimé."
 
-msgid "'{credential}' unknown or unconfirmed"
-msgstr "'{credential}' inconnu ou non confirmé"
+msgid "'%(credential)s' unknown or unconfirmed"
+msgstr "'%(credential)s' inconnu ou non confirmé"
 
-msgid "'{email}' already taken by someone else."
-msgstr "'{email}' déjà utilisé par quelqu'un."
+msgid "'%(email)s' already taken by someone else."
+msgstr "'%(email)s' déjà utilisé par quelqu'un."
 
-msgid "'{email}' is already taken by someone else."
-msgstr "'{email}' déjà utilisé par quelqu'un."
+msgid "'%(email)s' is already taken by someone else."
+msgstr "'%(email)s' déjà utilisé par quelqu'un."
 
-msgid "'{username}' is already taken by someone else."
-msgstr "'{username}' est déjà utilisé par quelqu'un."
+msgid "'%(username)s' is already taken by someone else."
+msgstr "'%(username)s' est déjà utilisé par quelqu'un."
 
 msgid "A user with that username already exists."
 msgstr "Un utilisateur utilise déjà ce nom."
 
 msgid "A username cannot include the symbol '@'."
 msgstr "Un nom d'utilisateur ne peut pas inclure '@'."
 
 msgid "Account"
 msgstr "Compte"
 
+msgid "Account Confirmation"
+msgstr "Confirmation du compte"
+
 msgid "Buy me a coffee"
 msgstr "Offrez-moi un café"
 
 msgid "Change Email"
 msgstr "Changer d'email"
 
 msgid "Change Username"
@@ -151,16 +155,20 @@
 
 msgid "Home"
 msgstr "Accueil"
 
 msgid "I forgot my password."
 msgstr "J'ai oublié mon mot de passe."
 
-msgid "If you do not confirm your account within the next "
-msgstr "Si vous ne confirmez pas votre compte dans les "
+msgid ""
+"If you do not confirm your account within the next %(hours)s hours, it will "
+"be deleted."
+msgstr ""
+"Si vous ne confirmez pas votre compte dans les %(hours)s heures, il sera "
+"supprimé."
 
 msgid "Incorrect credentials or unconfirmed account."
 msgstr "Identifiants incorrects ou compte non confirmé."
 
 msgid "Incorrect credentials."
 msgstr "Indentifiants incorrectes."
 
@@ -186,24 +194,24 @@
 "My account exists but is unconfirmed, please send me the confirmation email "
 "again."
 msgstr "J'ai un compte non confirmé, renvoyez-moi l'email de confirmation."
 
 msgid "New email address"
 msgstr "Nouvelle adresse email"
 
-msgid "New email saved, check your inbox at '{}' to activate it."
+msgid "New email saved, check your inbox at '%(new_email)s' to activate it."
 msgstr ""
-"Nouvel email enregistré, veuillez vérifier votre boite de réception à '{}' "
-"pour l'activer."
+"Nouvel email enregistré, veuillez vérifier votre boite de réception à "
+"'%(new_email)s' pour l'activer."
 
 msgid "New username"
 msgstr "Nouveau nom d'utilisateur"
 
-msgid "New username set: '{}'."
-msgstr "Nouveau nom d'utilisateur: '{}'."
+msgid "New username set: '%(username)s'."
+msgstr "Nouveau nom d'utilisateur: '%(username)s'."
 
 msgid "No credentials were provided"
 msgstr "Aucun identifiant fourni"
 
 msgid "Password"
 msgstr "Mot de passe"
 
@@ -212,26 +220,29 @@
 
 msgid ""
 "Please check your inbox and follow the instructions to reset your password."
 msgstr ""
 "Veuillez consulter votre boite mail et cliquer sur le lien fourni pour "
 "réinitialiser votre mot de passe."
 
-msgid "Please check your inbox at"
-msgstr "Veuillez consulter votre boite mail à"
-
-msgid "Please check your inbox at '{}' to confirm your account. "
-msgstr "Veuillez confirmer votre email à  '{}' pour confirmer votre compte. "
+msgid "Please check your inbox at '%(email)s' to confirm your account."
+msgstr ""
+"Veuillez consulter votre email à '%(email)s' pour confirmer votre compte."
 
-msgid "Please check your inbox to"
-msgstr "Veuillez consulter votre boite mail pour"
+msgid "Please check your inbox at '%(email)s' to confirm your account. "
+msgstr ""
+"Veuillez consulter votre boite mail à '%(email)s' pour confirmer votre "
+"compte. "
 
 msgid "Please check your inbox to confirm your account."
 msgstr "Consultez votre boite mail pour confirmer votre compte."
 
+msgid "Please check your inbox to confirm your new address at '%(email)s'"
+msgstr "Consultez votre boite mail à '%(email)s' pour confirmer votre compte."
+
 msgid "Report an issue"
 msgstr "Signaler un problème"
 
 msgid "Request password reset"
 msgstr "Demander réinitialisation du mot de passe"
 
 msgid "Request resend account confirmation email"
@@ -272,16 +283,16 @@
 
 msgid "This email is already associated with an existing account."
 msgstr "Cet email est déjà associé à un compte existant."
 
 msgid "Token invalid or expired"
 msgstr "Token invalide ou expiré"
 
-msgid "User '{credential}' unknown or unconfirmed"
-msgstr "Utilisateur '{credential}' inconnu ou non confirmé"
+msgid "User '%(credential)s' unknown or unconfirmed"
+msgstr "Utilisateur '%(credential)s' inconnu ou non confirmé"
 
 msgid "User not found"
 msgstr "Utilisateur inconnu"
 
 msgid "Username"
 msgstr "Nom d'utilisateur"
 
@@ -361,36 +372,24 @@
 
 msgid "email address"
 msgstr "adresse email"
 
 msgid "id:"
 msgstr "id:"
 
-msgid "it will be deleted."
-msgstr "il sera supprimé."
-
 msgid "jwt token invalid or expired"
 msgstr "le token jwt est invalide ou expiré"
 
 msgid "log in"
 msgstr "se connecter"
 
 msgid "no credential provided"
 msgstr "aucun identifiant fourni"
 
 msgid "send me an email"
 msgstr "envoyez moi un email"
 
-msgid "to confirm your account."
-msgstr "pour confirmer votre compte."
-
 msgid "user"
 msgstr "utilisateur"
 
 msgid "username"
 msgstr "nom d'utilisateur"
-
-msgid "{} hours, "
-msgstr "{} heures, "
-
-msgid "{} hours, it will be deleted."
-msgstr "{} heures, il sera supprimé."
```

### Comparing `django-silly-auth-1.0.2/django_silly_auth/locale/fr/LC_MESSAGES/django.po` & `django-silly-auth-1.0.3/django_silly_auth/locale/fr/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -3,90 +3,90 @@
 # This file is distributed under the same license as the django-silly-auth package.
 # Vincent Fabre <peigne.plume@gmail.com>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 00:57+0200\n"
-"PO-Revision-Date: 2023-04-11 00:57+0200\n"
+"POT-Creation-Date: 2023-04-11 21:00+0200\n"
+"PO-Revision-Date: 2023-04-11 21:01+0200\n"
 "Last-Translator: Vincent Fabre <peigne.plume@gmail.com>\n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "X-Generator: Poedit 3.0.1\n"
 
-#: forms.py:21 forms.py:24 forms.py:108 forms.py:111
+#: forms.py:21 forms.py:24 forms.py:117 forms.py:120
 msgid "Username or email"
 msgstr "Nom d'utilisateur ou email"
 
-#: forms.py:28 forms.py:31 forms.py:65 forms.py:69 forms.py:77 forms.py:128
-#: forms.py:131 forms.py:139
+#: forms.py:28 forms.py:31 forms.py:68 forms.py:72 forms.py:80 forms.py:140
+#: forms.py:143 forms.py:151
 msgid "Password"
 msgstr "Mot de passe"
 
-#: forms.py:43
-#, python-brace-format
-msgid "User '{credential}' unknown or unconfirmed"
-msgstr "Utilisateur '{credential}' inconnu ou non confirmé"
+#: forms.py:44
+#, python-format
+msgid "User '%(credential)s' unknown or unconfirmed"
+msgstr "Utilisateur '%(credential)s' inconnu ou non confirmé"
 
-#: forms.py:49 forms.py:53 forms.py:162
+#: forms.py:52 forms.py:56 forms.py:174
 msgid "Username"
 msgstr "Nom d'utilisateur"
 
-#: forms.py:57 forms.py:60 forms.py:182
+#: forms.py:60 forms.py:63 forms.py:197
 msgid "Email"
 msgstr "Email"
 
-#: forms.py:73 forms.py:136
+#: forms.py:76 forms.py:148
 msgid "Confirm password"
 msgstr "Confirmez le mot de passe"
 
-#: forms.py:85
+#: forms.py:88
 msgid "different than password"
 msgstr "mots de passe différents"
 
-#: forms.py:91 forms.py:169 mixins.py:76 serializers.py:44
+#: forms.py:94 forms.py:181 mixins.py:76 serializers.py:44
 msgid "A username cannot include the symbol '@'."
 msgstr "Un nom d'utilisateur ne peut pas inclure '@'."
 
-#: forms.py:95 forms.py:173
-#, python-brace-format
-msgid "'{username}' is already taken by someone else."
-msgstr "'{username}' est déjà utilisé par quelqu'un."
-
-#: forms.py:102
-#, python-brace-format
-msgid "'{email}' is already taken by someone else."
-msgstr "'{email}' déjà utilisé par quelqu'un."
-
-#: forms.py:122
-#, python-brace-format
-msgid "'{credential}' unknown or unconfirmed"
-msgstr "'{credential}' inconnu ou non confirmé"
+#: forms.py:99 forms.py:186
+#, python-format
+msgid "'%(username)s' is already taken by someone else."
+msgstr "'%(username)s' est déjà utilisé par quelqu'un."
 
-#: forms.py:152 serializers.py:73
+#: forms.py:109
+#, python-format
+msgid "'%(email)s' is already taken by someone else."
+msgstr "'%(email)s' déjà utilisé par quelqu'un."
+
+#: forms.py:132
+#, python-format
+msgid "'%(credential)s' unknown or unconfirmed"
+msgstr "'%(credential)s' inconnu ou non confirmé"
+
+#: forms.py:164 serializers.py:73
 msgid "The passwords you entered do not match."
 msgstr "Les mots de passe saisis ne correspondent pas."
 
-#: forms.py:158
+#: forms.py:170
 msgid "New username"
 msgstr "Nouveau nom d'utilisateur"
 
-#: forms.py:179
+#: forms.py:194
 msgid "New email address"
 msgstr "Nouvelle adresse email"
 
-#: forms.py:190
-#, python-brace-format
-msgid "'{email}' already taken by someone else."
-msgstr "'{email}' déjà utilisé par quelqu'un."
+#: forms.py:206
+#, python-format
+msgid "'%(email)s' already taken by someone else."
+msgstr "'%(email)s' déjà utilisé par quelqu'un."
 
 #: mixins.py:29
 msgid "username"
 msgstr "nom d'utilisateur"
 
 #: mixins.py:33
 msgid "Required. 150 characters or fewer. Letters, digits and ./+/-/_ only."
@@ -347,46 +347,50 @@
 "\n"
 "Si vous n'êtes pas à l'origine de cette demande, veuillez ignorer ce "
 "message.\n"
 "\n"
 "Cordialement\n"
 "\n"
 
+#: templates/silly_auth/silly/silly_confirm_email.html:11
+msgid "Account Confirmation"
+msgstr "Confirmation du compte"
+
 #: views/api_custom_login.py:45
 msgid ""
 "Your account has not been confirmed yet. Please check your inbox for a "
 "confirmation link."
 msgstr ""
 "Votre compte n'a pas encore été confirmé. Veuillez vérifier votre boite mail "
 "et utiliser le lien de confirmation."
 
 #: views/api_custom_login.py:50
 msgid "Incorrect credentials."
 msgstr "Indentifiants incorrectes."
 
-#: views/api_custom_login.py:65 views/classics.py:347
+#: views/api_custom_login.py:65 views/classics.py:354
 msgid "Your account has been confirmed."
 msgstr "Votre compte a été confirmé."
 
-#: views/api_custom_login.py:70 views/classics.py:352
+#: views/api_custom_login.py:70 views/classics.py:359
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
 
-#: views/api_views_if_drf.py:47 views/classics.py:355
+#: views/api_views_if_drf.py:47 views/classics.py:362
 msgid "Your account is already confirmed."
 msgstr "Votre compte est déjà confirmé."
 
 #: views/api_views_if_drf.py:51 views/api_views_if_drf.py:81
 msgid "Email sent for password reset"
 msgstr "Email envoyé pour réinitialisation du mot de passe"
 
@@ -398,109 +402,107 @@
 msgid "No credentials were provided"
 msgstr "Aucun identifiant fourni"
 
 #: views/api_views_if_drf.py:82
 msgid "Invalid credential"
 msgstr "Identifiant non valide"
 
-#: views/api_views_if_drf.py:98
-msgid "Please check your inbox at '{}' to confirm your account. "
-msgstr "Veuillez confirmer votre email à  '{}' pour confirmer votre compte. "
-
-#: views/api_views_if_drf.py:100
-msgid "If you do not confirm your account within the next "
-msgstr "Si vous ne confirmez pas votre compte dans les "
-
-#: views/api_views_if_drf.py:101
-msgid "{} hours, "
-msgstr "{} heures, "
-
-#: views/api_views_if_drf.py:102
-msgid "it will be deleted."
-msgstr "il sera supprimé."
+#: views/api_views_if_drf.py:99
+#, python-format
+msgid "Please check your inbox at '%(email)s' to confirm your account. "
+msgstr ""
+"Veuillez consulter votre boite mail à '%(email)s' pour confirmer votre "
+"compte. "
+
+#: views/api_views_if_drf.py:103
+#, python-format
+msgid ""
+"If you do not confirm your account within the next %(hours)s hours, it will "
+"be deleted."
+msgstr ""
+"Si vous ne confirmez pas votre compte dans les %(hours)s heures, il sera "
+"supprimé."
 
-#: views/api_views_if_drf.py:129
+#: views/api_views_if_drf.py:136
 msgid "Password successfully changed."
 msgstr "Mot de passe changé avec succès."
 
-#: views/api_views_if_drf.py:147
-msgid "New email saved, check your inbox at '{}' to activate it."
+#: views/api_views_if_drf.py:155
+#, python-format
+msgid "New email saved, check your inbox at '%(new_email)s' to activate it."
 msgstr ""
-"Nouvel email enregistré, veuillez vérifier votre boite de réception à '{}' "
-"pour l'activer."
+"Nouvel email enregistré, veuillez vérifier votre boite de réception à "
+"'%(new_email)s' pour l'activer."
 
 #: views/classics.py:58
 msgid "Incorrect credentials or unconfirmed account."
 msgstr "Identifiants incorrects ou compte non confirmé."
 
-#: views/classics.py:105
-msgid "Please check your inbox at"
-msgstr "Veuillez consulter votre boite mail à"
-
 #: views/classics.py:107
-msgid "to confirm your account."
-msgstr "pour confirmer votre compte."
+#, python-format
+msgid "Please check your inbox at '%(email)s' to confirm your account."
+msgstr ""
+"Veuillez consulter votre email à '%(email)s' pour confirmer votre compte."
 
-#: views/classics.py:111
-msgid " If you do not confirm your account within the next "
-msgstr " Si vous ne confirmez pas votre compte dans les "
-
-#: views/classics.py:112
-msgid "{} hours, it will be deleted."
-msgstr "{} heures, il sera supprimé."
+#: views/classics.py:114
+#, python-format
+msgid ""
+" If you do not confirm your account within the next %(time)s hours, it will "
+"be deleted."
+msgstr ""
+" Si vous ne confirmez pas votre compte dans les %(time)s heures, il sera "
+"supprimé."
 
-#: views/classics.py:156
+#: views/classics.py:161
 msgid ""
 "Please check your inbox and follow the instructions to reset your password."
 msgstr ""
 "Veuillez consulter votre boite mail et cliquer sur le lien fourni pour "
 "réinitialiser votre mot de passe."
 
-#: views/classics.py:168
+#: views/classics.py:173
 msgid ""
 "Your account is no longer active. Please contact the administrator. No email "
 "has been sent."
 msgstr ""
 "Votre compte est inactif. Contactez l'administrateur. L'envoi de l'email a "
 "été annulé."
 
-#: views/classics.py:211 views/classics.py:338 views/silly_views.py:20
+#: views/classics.py:216 views/classics.py:345 views/silly_views.py:20
 msgid "Token invalid or expired"
 msgstr "Token invalide ou expiré"
 
-#: views/classics.py:227
+#: views/classics.py:232
 msgid "Your password has been successfully reset. Please log in."
 msgstr ""
 "Votre mot de passe a été réinitialisé avec succès. Vous pouvez vous "
 "connecter."
 
-#: views/classics.py:244
+#: views/classics.py:249
 msgid ""
 "You have been logged in via email confirmation. Please reset your password."
 msgstr ""
 "Vous avez été connecté via un email de confirmation. Réinitialisez votre mot "
 "de passe si besoin."
 
-#: views/classics.py:268
-msgid "New username set: '{}'."
-msgstr "Nouveau nom d'utilisateur: '{}'."
-
-#: views/classics.py:305
-msgid "Please check your inbox to"
-msgstr "Veuillez consulter votre boite mail pour"
-
-#: views/classics.py:306
-msgid " confirm your new address at '{}'"
-msgstr " confirmer votre nouvelle adresse à '{}'"
+#: views/classics.py:274
+#, python-format
+msgid "New username set: '%(username)s'."
+msgstr "Nouveau nom d'utilisateur: '%(username)s'."
+
+#: views/classics.py:313
+#, python-format
+msgid "Please check your inbox to confirm your new address at '%(email)s'"
+msgstr "Consultez votre boite mail à '%(email)s' pour confirmer votre compte."
 
-#: views/classics.py:382
+#: views/classics.py:389
 msgid "Your account is already confirmed. No email has been sent."
 msgstr "Votre compte est déjà confirmé, l'email n'est pas envoyé."
 
-#: views/classics.py:394
+#: views/classics.py:401
 msgid "Please check your inbox to confirm your account."
 msgstr "Consultez votre boite mail pour confirmer votre compte."
 
 #: views/silly_views.py:26
 msgid "Your account has been confirmed"
 msgstr "Votre compte a été confirmé"
 
@@ -512,14 +514,42 @@
 msgid "Your account has already been confirmed."
 msgstr "Votre compte a déjà été confirmé."
 
 #: views/silly_views.py:50
 msgid "Your password has been successfully reset."
 msgstr "Votre mot de passe a été réinitialisé avec succès."
 
+#~ msgid "Please check your inbox at '{}' to confirm your account. "
+#~ msgstr ""
+#~ "Veuillez consulter votre email à  '{}' pour confirmer votre compte. "
+
+#~ msgid "If you do not confirm your account within the next "
+#~ msgstr "Si vous ne confirmez pas votre compte dans les "
+
+#~ msgid "{} hours, "
+#~ msgstr "{} heures, "
+
+#~ msgid "it will be deleted."
+#~ msgstr "il sera supprimé."
+
+#~ msgid "Please check your inbox at"
+#~ msgstr "Veuillez consulter votre boite mail à"
+
+#~ msgid "to confirm your account."
+#~ msgstr "pour confirmer votre compte."
+
+#~ msgid "{} hours, it will be deleted."
+#~ msgstr "{} heures, il sera supprimé."
+
+#~ msgid "Please check your inbox to"
+#~ msgstr "Veuillez consulter votre boite mail pour"
+
+#~ msgid " confirm your new address at '{}'"
+#~ msgstr " confirmer votre nouvelle adresse à '{}'"
+
 #~ msgid "Please check your inbox at '{}' "
 #~ msgstr "Vérifiez votre boite mail à '{}' "
 
 #~ msgid "{conf['DELETE_UNCONFIRMED_TIME']} hours, "
 #~ msgstr "{conf['DELETE_UNCONFIRMED_TIME']} heures, "
 
 #~ msgid "Lang."
```

### Comparing `django-silly-auth-1.0.2/django_silly_auth/mixins.py` & `django-silly-auth-1.0.3/django_silly_auth/mixins.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/serializers.py` & `django-silly-auth-1.0.3/django_silly_auth/serializers.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_base.html` & `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_base.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/_test/_base.html` & `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/_test/_base.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/account.html` & `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/account.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/change_email.html` & `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/change_email.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/change_username.html` & `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/change_username.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/login.html` & `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/login.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/request_password_reset.html` & `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/request_password_reset.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html` & `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/reset_password.html` & `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/reset_password.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/templates/silly_auth/classic/signup.html` & `django-silly-auth-1.0.3/django_silly_auth/templates/silly_auth/classic/signup.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/urls.py` & `django-silly-auth-1.0.3/django_silly_auth/urls.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/utils.py` & `django-silly-auth-1.0.3/django_silly_auth/utils.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/views/api_custom_login.py` & `django-silly-auth-1.0.3/django_silly_auth/views/api_custom_login.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/views/api_views_if_drf.py` & `django-silly-auth-1.0.3/django_silly_auth/views/api_views_if_drf.py`

 * *Files 10% similar despite different names*

```diff
@@ -91,20 +91,27 @@
         """Create a new user"""
         serializer = CreateUserSerializer(data=request.data)
         if serializer.is_valid():
             user = serializer.save()
             user.set_password(request.data['password'])
             user.save()
             delete_unconfirmed(user)
-            message = _("Please check your inbox at '{}' to confirm your account. ").format(user.email)
+            message1 = _(
+                "Please check your inbox at '%(email)s' to confirm your account. "
+                ) % {'email': user.email}
             if conf["DELETE_UNCONFIRMED_TIME"] != 0:
-                part1 = _("If you do not confirm your account within the next "),
-                part2 = _("{} hours, ").format(conf['DELETE_UNCONFIRMED_TIME']),
-                part3 = _("it will be deleted.")
-                message = "{}{}{}{}".format(message, part1, part2, part3)
+                message2 = _(
+                    "If you do not confirm your account within the next "
+                    "%(hours)s hours, it will be deleted."
+                    ) % {'hours': conf['DELETE_UNCONFIRMED_TIME']}
+
+                message = "%(message1)s %(message2)s" % {
+                    'message1': message1,
+                    'message2': message2,
+                }
             serializer = GetAllUsersSerializer(user)
             msg = {
                 "user": serializer.data,
                 "message": message,
             }
 
             send_confirm_email(request, user)
@@ -140,10 +147,14 @@
     if serializer.is_valid():
         new_email = request.data.get('email')
         user.new_email = new_email
         user.save()
         send_confirm_email(request, user, new_email=True)
 
         return Response(
-            {'success': _("New email saved, check your inbox at '{}' to activate it.").format(new_email)})
+            {'success': _(
+                "New email saved, check your inbox at '%(new_email)s' "
+                "to activate it."
+            ) % {'new_email': new_email}}
+        )
     msg = serializer.errors
     raise ValidationError({"error": msg}, code='authorization')
```

### Comparing `django-silly-auth-1.0.2/django_silly_auth/views/classics.py` & `django-silly-auth-1.0.3/django_silly_auth/views/classics.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,26 +98,31 @@
             email = form.cleaned_data['email']
             password = form.cleaned_data['password']
             user = User(username=username, email=email, is_active=True)
             user.set_password(password)
             user.save()
             send_confirm_email(request, user)
             delete_unconfirmed(user)
-            part1 = _("Please check your inbox at")
-            part2 = f" '{user.email}' "
-            part3 = _("to confirm your account.")
 
+            message1 = _(
+                "Please check your inbox at"
+                " '%(email)s' to confirm your account."
+            ) % {'email': user.email}
+            message2 = ""
             if conf["DELETE_UNCONFIRMED_TIME"] != 0.0:
 
-                part4 = _(" If you do not confirm your account within the next ")
-                part5 = _("{} hours, it will be deleted.").format(conf['DELETE_UNCONFIRMED_TIME'])
-            else:
-                part4 = part5 = ""
-
-            message = "{}{}{}{}{}".format(part1, part2, part3, part4, part5)
+                message2 = _(
+                    " If you do not confirm your account within the next "
+                    "%(time)s hours, it will be deleted."
+                ) % {'time': conf['DELETE_UNCONFIRMED_TIME']}
+
+            message = "%(message1)s%(message2)s" % {
+                'message1': message1,
+                'message2': message2,
+            }
 
             messages.add_message(
                 request, messages.INFO,
                 message=message,
                 extra_tags="info"
             )
             return redirect('classic_login')
@@ -261,15 +266,17 @@
         if form.is_valid():
             username = form.cleaned_data['username']
             user = request.user
             user.username = username
             user.save()
             messages.add_message(
                 request, messages.SUCCESS,
-                message=_("New username set: '{}'.").format(username),
+                message=_(
+                    "New username set: '%(username)s'."
+                ) % {'username': username},
                 extra_tags="success"
             )
             return redirect("classic_account")
         else:
             context = {
                 'form': form,
                 "base_template": conf["BASE_TEMPLATE"],
@@ -298,17 +305,17 @@
         if form.is_valid():
             email = form.cleaned_data['email']
             user = request.user
             user.new_email = email
             user.save()
             send_confirm_email(request, user)
 
-            part1 = _("Please check your inbox to"),
-            part2 = _(" confirm your new address at '{}'").format(email)
-            message = "{}{}.".format(part1, part2)
+            message = _(
+                "Please check your inbox to confirm your new "
+                "address at '%(email)s'") % {"email": user.new_email}
             messages.add_message(
                 request, messages.INFO,
                 message,
                 extra_tags="info"
             )
             return redirect("classic_account")
         else:
```

### Comparing `django-silly-auth-1.0.2/django_silly_auth/views/silly_views.py` & `django-silly-auth-1.0.3/django_silly_auth/views/silly_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth/views/test_views.py` & `django-silly-auth-1.0.3/django_silly_auth/views/test_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.2/django_silly_auth.egg-info/PKG-INFO` & `django-silly-auth-1.0.3/django_silly_auth.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 1.0.2
+Version: 1.0.3
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
@@ -13,20 +13,20 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# Django Silly Auth (v1.0.0)
+# Django Silly Auth
 
 ## Why one more authentication system for Django and DRF? again !
 
 I've used a few ones, and did not find the one that behaves the way I want,
-efficient, but flexible, I want to win time, and get what I need straight to the point.
+efficient, but flexible, I wanted to gain som time, and get what I need straight to the point.
 
 The aim of DSA it to provide a good-enough-to-go authentication out of the box, but still remains highly
 modular through its SILLY_AUTH config in **settings.py**, so it is always possible to improve your
 authentication when you have the time for it.
 
 ## DRF and Django Classic supported
 DSA works as well with both DRF and Classic, just use differents simple settings, and you're done.
@@ -38,10 +38,11 @@
 
 ## [Read this FIRST](https://github.com/byoso/django_silly_auth/wiki/Must-read-this-few-lines-!)
 
 ### :coffee: [If you find this package usefull, consider buying me a coffee](https://www.buymeacoffee.com/byoso)
 
 
 ### Changelog
-- 1.0.1: i18n fr + en
+
+- 1.0.1: **i18n** fr + en
```

### Comparing `django-silly-auth-1.0.2/django_silly_auth.egg-info/SOURCES.txt` & `django-silly-auth-1.0.3/django_silly_auth.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 django_silly_auth/utils.py
 django_silly_auth.egg-info/PKG-INFO
 django_silly_auth.egg-info/SOURCES.txt
 django_silly_auth.egg-info/dependency_links.txt
 django_silly_auth.egg-info/requires.txt
 django_silly_auth.egg-info/top_level.txt
 django_silly_auth/locale/django.pot
+django_silly_auth/locale/en/LC_MESSAGES/django.mo
 django_silly_auth/locale/en/LC_MESSAGES/django.po
 django_silly_auth/locale/fr/LC_MESSAGES/django.mo
 django_silly_auth/locale/fr/LC_MESSAGES/django.po
 django_silly_auth/templates/__init__.py
 django_silly_auth/templates/silly_auth/__init__.py
 django_silly_auth/templates/silly_auth/_base.html
 django_silly_auth/templates/silly_auth/_test/__init__.py
```

### Comparing `django-silly-auth-1.0.2/setup.py` & `django-silly-auth-1.0.3/setup.py`

 * *Files identical despite different names*

