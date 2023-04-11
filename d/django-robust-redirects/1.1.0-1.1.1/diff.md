# Comparing `tmp/django-robust-redirects-1.1.0.tar.gz` & `tmp/django-robust-redirects-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-robust-redirects-1.1.0.tar", last modified: Mon Apr 10 16:22:04 2023, max compression
+gzip compressed data, was "django-robust-redirects-1.1.1.tar", last modified: Mon Apr 10 20:34:58 2023, max compression
```

## Comparing `django-robust-redirects-1.1.0.tar` & `django-robust-redirects-1.1.1.tar`

### file list

```diff
@@ -1,46 +1,44 @@
-drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:22:04.196822 django-robust-redirects-1.1.0/
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1719 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.0/LICENSE
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)      170 2023-04-10 14:42:46.000000 django-robust-redirects-1.1.0/MANIFEST.in
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)      639 2023-04-10 16:22:04.196652 django-robust-redirects-1.1.0/PKG-INFO
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1425 2023-04-08 00:10:15.000000 django-robust-redirects-1.1.0/README.md
-drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:22:04.189199 django-robust-redirects-1.1.0/django_robust_redirects.egg-info/
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)      639 2023-04-10 16:22:04.000000 django-robust-redirects-1.1.0/django_robust_redirects.egg-info/PKG-INFO
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1048 2023-04-10 16:22:04.000000 django-robust-redirects-1.1.0/django_robust_redirects.egg-info/SOURCES.txt
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        1 2023-04-10 16:22:04.000000 django-robust-redirects-1.1.0/django_robust_redirects.egg-info/dependency_links.txt
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        1 2023-04-10 14:47:42.000000 django-robust-redirects-1.1.0/django_robust_redirects.egg-info/not-zip-safe
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)       27 2023-04-10 16:22:04.000000 django-robust-redirects-1.1.0/django_robust_redirects.egg-info/requires.txt
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)       16 2023-04-10 16:22:04.000000 django-robust-redirects-1.1.0/django_robust_redirects.egg-info/top_level.txt
-drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:22:04.194504 django-robust-redirects-1.1.0/robustredirects/
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        0 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.0/robustredirects/__init__.py
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     2638 2023-04-10 15:09:01.000000 django-robust-redirects-1.1.0/robustredirects/admin.py
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)      143 2023-04-10 15:09:01.000000 django-robust-redirects-1.1.0/robustredirects/apps.py
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)       95 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.0/robustredirects/dynamic_urls.py
-drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:22:04.186850 django-robust-redirects-1.1.0/robustredirects/locale/
-drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:22:04.186632 django-robust-redirects-1.1.0/robustredirects/locale/en/
-drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:22:04.194676 django-robust-redirects-1.1.0/robustredirects/locale/en/LC_MESSAGES/
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1497 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.0/robustredirects/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:22:04.186769 django-robust-redirects-1.1.0/robustredirects/locale/ru/
-drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:22:04.195200 django-robust-redirects-1.1.0/robustredirects/locale/ru/LC_MESSAGES/
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1974 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.0/robustredirects/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     2479 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.0/robustredirects/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:22:04.186905 django-robust-redirects-1.1.0/robustredirects/locale/uk/
-drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:22:04.195567 django-robust-redirects-1.1.0/robustredirects/locale/uk/LC_MESSAGES/
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1944 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.0/robustredirects/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     2446 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.0/robustredirects/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:22:04.195775 django-robust-redirects-1.1.0/robustredirects/management/
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        0 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.0/robustredirects/management/__init__.py
-drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:22:04.196061 django-robust-redirects-1.1.0/robustredirects/management/commands/
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        0 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.0/robustredirects/management/commands/__init__.py
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1053 2023-04-10 15:09:01.000000 django-robust-redirects-1.1.0/robustredirects/management/commands/convert_redirects.py
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     3479 2023-04-10 15:09:01.000000 django-robust-redirects-1.1.0/robustredirects/middleware.py
-drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:22:04.196257 django-robust-redirects-1.1.0/robustredirects/migrations/
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        0 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.0/robustredirects/migrations/__init__.py
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     2429 2023-04-10 15:09:01.000000 django-robust-redirects-1.1.0/robustredirects/models.py
-drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 16:22:04.196388 django-robust-redirects-1.1.0/robustredirects/templates/
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1598 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.0/robustredirects/templates/change_form.html
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     6054 2023-04-10 15:09:01.000000 django-robust-redirects-1.1.0/robustredirects/tests.py
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)       14 2023-04-10 15:09:01.000000 django-robust-redirects-1.1.0/robustredirects/urls.py
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1823 2023-04-10 15:09:01.000000 django-robust-redirects-1.1.0/robustredirects/utils.py
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1493 2023-04-10 15:09:01.000000 django-robust-redirects-1.1.0/robustredirects/views.py
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)       38 2023-04-10 16:22:04.196874 django-robust-redirects-1.1.0/setup.cfg
--rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)      945 2023-04-10 16:12:48.000000 django-robust-redirects-1.1.0/setup.py
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 20:34:58.536433 django-robust-redirects-1.1.1/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1719 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.1/LICENSE
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)      170 2023-04-10 14:42:46.000000 django-robust-redirects-1.1.1/MANIFEST.in
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)      639 2023-04-10 20:34:58.536249 django-robust-redirects-1.1.1/PKG-INFO
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1425 2023-04-10 20:24:50.000000 django-robust-redirects-1.1.1/README.md
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 20:34:58.531107 django-robust-redirects-1.1.1/django_robust_redirects.egg-info/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)      639 2023-04-10 20:34:58.000000 django-robust-redirects-1.1.1/django_robust_redirects.egg-info/PKG-INFO
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1009 2023-04-10 20:34:58.000000 django-robust-redirects-1.1.1/django_robust_redirects.egg-info/SOURCES.txt
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        1 2023-04-10 20:34:58.000000 django-robust-redirects-1.1.1/django_robust_redirects.egg-info/dependency_links.txt
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        1 2023-04-10 14:47:42.000000 django-robust-redirects-1.1.1/django_robust_redirects.egg-info/not-zip-safe
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)       27 2023-04-10 20:34:58.000000 django-robust-redirects-1.1.1/django_robust_redirects.egg-info/requires.txt
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)       16 2023-04-10 20:34:58.000000 django-robust-redirects-1.1.1/django_robust_redirects.egg-info/top_level.txt
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 20:34:58.533844 django-robust-redirects-1.1.1/robustredirects/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        0 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.1/robustredirects/__init__.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     2638 2023-04-10 15:09:01.000000 django-robust-redirects-1.1.1/robustredirects/admin.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)      143 2023-04-10 15:09:01.000000 django-robust-redirects-1.1.1/robustredirects/apps.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)       95 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.1/robustredirects/dynamic_urls.py
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 20:34:58.528370 django-robust-redirects-1.1.1/robustredirects/locale/
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 20:34:58.528043 django-robust-redirects-1.1.1/robustredirects/locale/en/
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 20:34:58.534092 django-robust-redirects-1.1.1/robustredirects/locale/en/LC_MESSAGES/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1497 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.1/robustredirects/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 20:34:58.528253 django-robust-redirects-1.1.1/robustredirects/locale/ru/
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 20:34:58.534654 django-robust-redirects-1.1.1/robustredirects/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1974 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.1/robustredirects/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     2479 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.1/robustredirects/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 20:34:58.528440 django-robust-redirects-1.1.1/robustredirects/locale/uk/
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 20:34:58.535107 django-robust-redirects-1.1.1/robustredirects/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1944 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.1/robustredirects/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     2446 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.1/robustredirects/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 20:34:58.535334 django-robust-redirects-1.1.1/robustredirects/management/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        0 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.1/robustredirects/management/__init__.py
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 20:34:58.535666 django-robust-redirects-1.1.1/robustredirects/management/commands/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)        0 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.1/robustredirects/management/commands/__init__.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1053 2023-04-10 15:09:01.000000 django-robust-redirects-1.1.1/robustredirects/management/commands/convert_redirects.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     3479 2023-04-10 20:24:50.000000 django-robust-redirects-1.1.1/robustredirects/middleware.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     2429 2023-04-10 15:09:01.000000 django-robust-redirects-1.1.1/robustredirects/models.py
+drwxr-xr-x   0 Cezar.Jenkins   (502) staff       (20)        0 2023-04-10 20:34:58.535932 django-robust-redirects-1.1.1/robustredirects/templates/
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1598 2023-03-21 14:42:59.000000 django-robust-redirects-1.1.1/robustredirects/templates/change_form.html
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     6054 2023-04-10 20:24:50.000000 django-robust-redirects-1.1.1/robustredirects/tests.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)       14 2023-04-10 15:09:01.000000 django-robust-redirects-1.1.1/robustredirects/urls.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1823 2023-04-10 20:24:50.000000 django-robust-redirects-1.1.1/robustredirects/utils.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)     1493 2023-04-10 15:09:01.000000 django-robust-redirects-1.1.1/robustredirects/views.py
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)       38 2023-04-10 20:34:58.536489 django-robust-redirects-1.1.1/setup.cfg
+-rw-r--r--   0 Cezar.Jenkins   (502) staff       (20)      945 2023-04-10 20:31:37.000000 django-robust-redirects-1.1.1/setup.py
```

### Comparing `django-robust-redirects-1.1.0/LICENSE` & `django-robust-redirects-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.1.0/PKG-INFO` & `django-robust-redirects-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-robust-redirects
-Version: 1.1.0
+Version: 1.1.1
 Summary: A more robust and feature full django redirect package
 Home-page: http://github.com/spothero/django-robust-redirects
 Download-URL: http://github.com/spothero/django-robust-redirects/tarball/0.10.0
 Author: SpotHero
 Author-email: pypi@spothero.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
```

### Comparing `django-robust-redirects-1.1.0/README.md` & `django-robust-redirects-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.1.0/django_robust_redirects.egg-info/PKG-INFO` & `django-robust-redirects-1.1.1/django_robust_redirects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-robust-redirects
-Version: 1.1.0
+Version: 1.1.1
 Summary: A more robust and feature full django redirect package
 Home-page: http://github.com/spothero/django-robust-redirects
 Download-URL: http://github.com/spothero/django-robust-redirects/tarball/0.10.0
 Author: SpotHero
 Author-email: pypi@spothero.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
```

### Comparing `django-robust-redirects-1.1.0/django_robust_redirects.egg-info/SOURCES.txt` & `django-robust-redirects-1.1.1/django_robust_redirects.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 robustredirects/locale/ru/LC_MESSAGES/django.mo
 robustredirects/locale/ru/LC_MESSAGES/django.po
 robustredirects/locale/uk/LC_MESSAGES/django.mo
 robustredirects/locale/uk/LC_MESSAGES/django.po
 robustredirects/management/__init__.py
 robustredirects/management/commands/__init__.py
 robustredirects/management/commands/convert_redirects.py
-robustredirects/migrations/__init__.py
 robustredirects/templates/change_form.html
```

### Comparing `django-robust-redirects-1.1.0/robustredirects/admin.py` & `django-robust-redirects-1.1.1/robustredirects/admin.py`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.1.0/robustredirects/locale/en/LC_MESSAGES/django.po` & `django-robust-redirects-1.1.1/robustredirects/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.1.0/robustredirects/locale/ru/LC_MESSAGES/django.mo` & `django-robust-redirects-1.1.1/robustredirects/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.1.0/robustredirects/locale/ru/LC_MESSAGES/django.po` & `django-robust-redirects-1.1.1/robustredirects/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.1.0/robustredirects/locale/uk/LC_MESSAGES/django.mo` & `django-robust-redirects-1.1.1/robustredirects/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.1.0/robustredirects/locale/uk/LC_MESSAGES/django.po` & `django-robust-redirects-1.1.1/robustredirects/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.1.0/robustredirects/management/commands/convert_redirects.py` & `django-robust-redirects-1.1.1/robustredirects/management/commands/convert_redirects.py`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.1.0/robustredirects/middleware.py` & `django-robust-redirects-1.1.1/robustredirects/middleware.py`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.1.0/robustredirects/models.py` & `django-robust-redirects-1.1.1/robustredirects/models.py`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.1.0/robustredirects/templates/change_form.html` & `django-robust-redirects-1.1.1/robustredirects/templates/change_form.html`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.1.0/robustredirects/tests.py` & `django-robust-redirects-1.1.1/robustredirects/tests.py`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.1.0/robustredirects/utils.py` & `django-robust-redirects-1.1.1/robustredirects/utils.py`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.1.0/robustredirects/views.py` & `django-robust-redirects-1.1.1/robustredirects/views.py`

 * *Files identical despite different names*

### Comparing `django-robust-redirects-1.1.0/setup.py` & `django-robust-redirects-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name="django-robust-redirects",
-    version="1.1.0",
+    version="1.1.1",
     url="http://github.com/spothero/django-robust-redirects",
     download_url="http://github.com/spothero/django-robust-redirects/tarball/0.10.0",
     description="A more robust and feature full django redirect package",
     author="SpotHero",
     author_email="pypi@spothero.com",
     packages=find_packages(exclude=['redirecttest*']),
     include_package_data=True,
```

