# Comparing `tmp/django-unical-bootstrap-italia-1.2.0.tar.gz` & `tmp/django-unical-bootstrap-italia-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-unical-bootstrap-italia-1.2.0.tar", last modified: Tue Apr 11 13:00:46 2023, max compression
+gzip compressed data, was "django-unical-bootstrap-italia-2.0.1.tar", last modified: Tue Apr 11 12:24:17 2023, max compression
```

## Comparing `django-unical-bootstrap-italia-1.2.0.tar` & `django-unical-bootstrap-italia-2.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 13:00:46.302482 django-unical-bootstrap-italia-1.2.0/
--rw-r--r--   0 francesco  (1000) francesco  (1000)    11352 2021-11-05 07:31:39.000000 django-unical-bootstrap-italia-1.2.0/LICENSE
--rw-r--r--   0 francesco  (1000) francesco  (1000)      203 2020-02-26 11:51:00.000000 django-unical-bootstrap-italia-1.2.0/MANIFEST.in
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    15068 2023-04-11 13:00:46.302482 django-unical-bootstrap-italia-1.2.0/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11519 2023-04-11 08:11:10.000000 django-unical-bootstrap-italia-1.2.0/README.md
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 13:00:46.302482 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/
--rw-r--r--   0 francesco  (1000) francesco  (1000)        0 2019-06-07 12:01:41.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/__init__.py
--rw-r--r--   0 francesco  (1000) francesco  (1000)      139 2020-02-26 11:41:44.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/apps.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 13:00:46.302482 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 13:00:46.302482 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/css/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4882 2023-04-11 08:34:39.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/css/unical-style.css
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 13:00:46.302482 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 13:00:46.302482 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/favicon/
--rw-r--r--   0 francesco  (1000) francesco  (1000)        9 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/favicon/README.md
--rw-r--r--   0 francesco  (1000) francesco  (1000)      507 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/favicon/favicon-32x32.png
--rw-r--r--   0 francesco  (1000) francesco  (1000)     1972 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/logo.svg
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    27664 2020-11-13 09:00:35.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/logo1.svg
--rw-r--r--   0 francesco  (1000) francesco  (1000)     3499 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/logo_back.svg
--rw-r--r--   0 francesco  (1000) francesco  (1000)      799 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/logo_white.png
--rw-r--r--   0 francesco  (1000) francesco  (1000)   508364 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/unical_banner.jpg
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    23187 2019-07-04 09:22:35.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/unical_logo.svg
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 13:00:46.302482 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/templates/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      240 2020-03-25 08:08:38.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/templates/404.html
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      267 2020-03-25 08:09:09.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/templates/500.html
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    11877 2023-04-11 12:59:52.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/templates/base-setup.html
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1135 2023-04-11 12:57:02.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/templates/error-page.html
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)     8227 2023-04-11 12:57:02.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/templates/index.html
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 13:00:46.302482 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia.egg-info/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    15068 2023-04-11 13:00:46.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia.egg-info/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1200 2023-04-11 13:00:46.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia.egg-info/SOURCES.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2023-04-11 13:00:46.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia.egg-info/dependency_links.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       32 2023-04-11 13:00:46.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia.egg-info/requires.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       31 2023-04-11 13:00:46.000000 django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia.egg-info/top_level.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2023-04-11 13:00:46.302482 django-unical-bootstrap-italia-1.2.0/setup.cfg
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1363 2023-04-11 12:57:33.000000 django-unical-bootstrap-italia-1.2.0/setup.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 12:24:17.437218 django-unical-bootstrap-italia-2.0.1/
+-rw-r--r--   0 francesco  (1000) francesco  (1000)    11352 2021-11-05 07:31:39.000000 django-unical-bootstrap-italia-2.0.1/LICENSE
+-rw-r--r--   0 francesco  (1000) francesco  (1000)      203 2020-02-26 11:51:00.000000 django-unical-bootstrap-italia-2.0.1/MANIFEST.in
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    15068 2023-04-11 12:24:17.437218 django-unical-bootstrap-italia-2.0.1/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    11519 2023-04-11 08:11:10.000000 django-unical-bootstrap-italia-2.0.1/README.md
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 12:24:17.433218 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/
+-rw-r--r--   0 francesco  (1000) francesco  (1000)        0 2019-06-07 12:01:41.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/__init__.py
+-rw-r--r--   0 francesco  (1000) francesco  (1000)      139 2020-02-26 11:41:44.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/apps.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 12:24:17.433218 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 12:24:17.433218 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/css/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     4882 2023-04-11 08:34:39.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/css/unical-style.css
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 12:24:17.433218 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 12:24:17.433218 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/favicon/
+-rw-r--r--   0 francesco  (1000) francesco  (1000)        9 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/favicon/README.md
+-rw-r--r--   0 francesco  (1000) francesco  (1000)      507 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/favicon/favicon-32x32.png
+-rw-r--r--   0 francesco  (1000) francesco  (1000)     1972 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/logo.svg
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    27664 2020-11-13 09:00:35.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/logo1.svg
+-rw-r--r--   0 francesco  (1000) francesco  (1000)     3499 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/logo_back.svg
+-rw-r--r--   0 francesco  (1000) francesco  (1000)      799 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/logo_white.png
+-rw-r--r--   0 francesco  (1000) francesco  (1000)   508364 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/unical_banner.jpg
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    23187 2019-07-04 09:22:35.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/unical_logo.svg
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 12:24:17.433218 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/templates/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      240 2020-03-25 08:08:38.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/templates/404.html
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      267 2020-03-25 08:09:09.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/templates/500.html
+-rwxr-xr-x   0 francesco  (1000) francesco  (1000)    11908 2023-04-11 08:44:07.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/templates/base-setup.html
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1136 2023-04-11 08:44:10.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/templates/error-page.html
+-rwxr-xr-x   0 francesco  (1000) francesco  (1000)     8236 2023-04-11 08:43:59.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/templates/index.html
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-11 12:24:17.433218 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia.egg-info/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)    15068 2023-04-11 12:24:17.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia.egg-info/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1200 2023-04-11 12:24:17.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia.egg-info/SOURCES.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2023-04-11 12:24:17.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia.egg-info/dependency_links.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       20 2023-04-11 12:24:17.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia.egg-info/requires.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       31 2023-04-11 12:24:17.000000 django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia.egg-info/top_level.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2023-04-11 12:24:17.437218 django-unical-bootstrap-italia-2.0.1/setup.cfg
+-rw-r--r--   0 francesco  (1000) francesco  (1000)     1351 2023-04-11 08:44:56.000000 django-unical-bootstrap-italia-2.0.1/setup.py
```

### Comparing `django-unical-bootstrap-italia-1.2.0/LICENSE` & `django-unical-bootstrap-italia-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.2.0/PKG-INFO` & `django-unical-bootstrap-italia-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-unical-bootstrap-italia
-Version: 1.2.0
+Version: 2.0.1
 Summary: Django theme for Università della Calabria (UNICAL) based on Bootstrap Italia theme
 Home-page: https://github.com/UniversitaDellaCalabria/django-unical-bootstrap-italia
 Author: Giuseppe De Marco, Francesco Filicetti
 Author-email: giuseppe.demarco@unical.it, francesco.filicetti@unical.it
 License: Apache 2.0
 Description: Template Django conforme a linee guida AGID per l'Università della Calabria
         ---------------------------------------------------------------------------
```

### Comparing `django-unical-bootstrap-italia-1.2.0/README.md` & `django-unical-bootstrap-italia-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/css/unical-style.css` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/css/unical-style.css`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/logo.svg` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/logo1.svg` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/logo1.svg`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/logo_back.svg` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/logo_back.svg`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/logo_white.png` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/logo_white.png`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/unical_banner.jpg` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/unical_banner.jpg`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/static/images/unical_logo.svg` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/unical_logo.svg`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/templates/base-setup.html` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/templates/base-setup.html`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 {% load static %}
 
 <!-- Page Title -->
 {% block page_title %}
 Università della Calabria
 {% endblock page_title %}
 
+<!-- My custom scss sheet -->
 {% block extra_head %}
 <link rel="shortcut icon" href="{% static 'images/favicon/favicon-32x32.png' %}">
 <link rel="stylesheet" href="{% static 'css/unical-style.css' %}" type="text/css" />
 {% endblock extra_head %}
 
 <!-- URL link top left -->
 {% block header_slim_org_url %}
@@ -33,51 +34,51 @@
     <span>Seguici su</span>
     <ul>
         <li>
             <a href="https://it-it.facebook.com/pages/Universit%C3%A0-della-Calabria/166678814380"
                aria-label="Facebook"
                target="_blank">
                 <svg class="icon">
-                    <use xlink:href="{% static 'svg/sprite.svg' %}#it-facebook"></use>
+                    <use xlink:href="{% static 'svg/sprites.svg' %}#it-facebook"></use>
                 </svg>
             </a>
         </li>
         <li>
             <a href="https://twitter.com/UnicalPortale"
                aria-label="Twitter"
                target="_blank">
                 <svg class="icon">
-                <use xlink:href="{% static 'svg/sprite.svg' %}#it-twitter"></use>
+                <use xlink:href="{% static 'svg/sprites.svg' %}#it-twitter"></use>
                 </svg>
             </a>
         </li>
         <li>
             <a href="https://www.instagram.com/unical_official/"
                target="_blank"
                aria-label="Instagram">
                 <svg class="icon">
-                <use xlink:href="{% static 'svg/sprite.svg' %}#it-instagram"></use>
+                <use xlink:href="{% static 'svg/sprites.svg' %}#it-instagram"></use>
                 </svg>
             </a>
         </li>
         <li>
             <a href="https://www.youtube.com/channel/UCnd5Oen95TMO9aLfVRUAABQ"
                target="_blank"
                aria-label="YouTube">
                 <svg class="icon">
-                <use xlink:href="{% static 'svg/sprite.svg' %}#it-youtube"></use>
+                <use xlink:href="{% static 'svg/sprites.svg' %}#it-youtube"></use>
                 </svg>
             </a>
         </li>
         <li>
             <a href="https://github.com/UniversitaDellaCalabria"
                target="_blank"
                aria-label="GitHub">
                 <svg class="icon">
-                <use xlink:href="{% static 'svg/sprite.svg' %}#it-github"></use>
+                <use xlink:href="{% static 'svg/sprites.svg' %}#it-github"></use>
                 </svg>
             </a>
         </li>
     </ul>
 </div>
 {% endblock header_center_social %}
 
@@ -188,57 +189,57 @@
                     </li>
                 </ul>
             </div>
         </div>
         <div class="col-lg-4 col-md-4 pb-2">
             <div class="pb-2">
                 <h4><a href="#" title="Vai alla pagina: Seguici su">Seguici su</a></h4>
-                <ul class="list-inline social text-left">
+                <ul class="list-inline social">
                     <li class="list-inline-item">
                         <a class="p-2 text-white"
                            href="https://it-it.facebook.com/pages/Universit%C3%A0-della-Calabria/166678814380"
                            target="_blank">
                             <svg class="icon icon-sm icon-white align-top">
-                                <use xlink:href="{% static 'svg/sprite.svg' %}#it-facebook"></use>
+                                <use xlink:href="{% static 'svg/sprites.svg' %}#it-facebook"></use>
                             </svg><span class="sr-only">Facebook</span>
                         </a>
                     </li>
                     <li class="list-inline-item">
                         <a class="p-2 text-white"
                            href="https://twitter.com/UnicalPortale"
                            target="_blank">
                             <svg class="icon icon-sm icon-white align-top">
-                                <use xlink:href="{% static 'svg/sprite.svg' %}#it-twitter"></use>
+                                <use xlink:href="{% static 'svg/sprites.svg' %}#it-twitter"></use>
                             </svg><span class="sr-only">Twitter</span>
                         </a>
                     </li>
                     <li class="list-inline-item">
                         <a class="p-2 text-white"
                            href="https://www.instagram.com/unical_official/"
                            target="_blank">
                             <svg class="icon icon-sm icon-white align-top">
-                                <use xlink:href="{% static 'svg/sprite.svg' %}#it-instagram"></use>
+                                <use xlink:href="{% static 'svg/sprites.svg' %}#it-instagram"></use>
                             </svg><span class="sr-only">Instagram</span>
                         </a>
                     </li>
                     <li class="list-inline-item">
                         <a class="p-2 text-white"
                            href="https://www.youtube.com/channel/UCnd5Oen95TMO9aLfVRUAABQ"
                            target="_blank">
                             <svg class="icon icon-sm icon-white align-top">
-                                <use xlink:href="{% static 'svg/sprite.svg' %}#it-youtube"></use>
+                                <use xlink:href="{% static 'svg/sprites.svg' %}#it-youtube"></use>
                             </svg><span class="sr-only">YouTube</span>
                         </a>
                     </li>
                     <li class="list-inline-item">
                         <a class="p-2 text-white"
                            href="https://github.com/UniversitaDellaCalabria"
                            target="_blank">
                             <svg class="icon icon-sm icon-white align-top">
-                                <use xlink:href="{% static 'svg/sprite.svg' %}#it-github"></use>
+                                <use xlink:href="{% static 'svg/sprites.svg' %}#it-github"></use>
                             </svg> <span class="sr-only">GitHub</span>
                         </a>
                     </li>
                 </ul>
             </div>
             {% comment %}
             <div class="pb-2">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
  {% extends 'bootstrap-italia-base.html' %} {% load static %}  {% block
-page_title %} UniversitÃ  della Calabria {% endblock page_title %} {% block
+page_title %} UniversitÃ  della Calabria {% endblock page_title %}  {% block
 extra_head %}
 
  {% endblock extra_head %}  {% block header_slim_org_url %} https://
 www.unical.it {% endblock header_slim_org_url %}  {% block header_slim_org_name
 %} UniversitÃ  della Calabria {% endblock header_slim_org_name %}  {% block
 header_slim_mobile_org_name %} UniversitÃ  della Calabria {% endblock
 header_slim_mobile_org_name %} {% block header_center_social %}
```

### Comparing `django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/templates/error-page.html` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/templates/error-page.html`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     {% endblock menu_post_buttons %}
 {% endblock menu_links %}
 
 {% block centered_container %}
 <div class="callout danger mt-5">
 	<div class="callout-title">
         <svg class="icon icon-primary icon-danger">
-            <use xlink:href="{% static 'svg/sprite.svg' %}#it-close-circle"></use>
+            <use xlink:href="{% static 'svg/sprites.svg' %}#it-close-circle"></use>
         </svg>
         {% block error_type %}
             {% trans "Error" %}
         {% endblock error_type %}</div>
 	<p>
         {% block error_description %}
             {% trans "Error description" %}
```

### Comparing `django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia/templates/index.html` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/templates/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         <div class="card card-bg">
           <div class="card-body">
             <h5 class="card-title">1. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor…</h5>
             <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
             <a class="read-more" href="#">
               <span class="text">Leggi di più</span>
               <svg class="icon">
-                <use xlink:href="{% static 'svg/sprite.svg' %}#it-arrow-right"></use>
+                <use xlink:href="{% static 'svg/sprites.svg' %}#it-arrow-right"></use>
               </svg>
             </a>
           </div>
         </div>
       </div>
     </div>
     <div class="it-single-slide-wrapper">
@@ -66,15 +66,15 @@
         <div class="card card-bg">
           <div class="card-body">
             <h5 class="card-title">2. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor…</h5>
             <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
             <a class="read-more" href="#">
               <span class="text">Leggi di più</span>
               <svg class="icon">
-                <use xlink:href="{% static 'svg/sprite.svg' %}#it-arrow-right"></use>
+                <use xlink:href="{% static 'svg/sprites.svg' %}#it-arrow-right"></use>
               </svg>
             </a>
           </div>
         </div>
       </div>
     </div>
     <div class="it-single-slide-wrapper">
@@ -82,15 +82,15 @@
         <div class="card card-bg">
           <div class="card-body">
             <h5 class="card-title">3. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor…</h5>
             <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
             <a class="read-more" href="#">
               <span class="text">Leggi di più</span>
               <svg class="icon">
-                <use xlink:href="{% static 'svg/sprite.svg' %}#it-arrow-right"></use>
+                <use xlink:href="{% static 'svg/sprites.svg' %}#it-arrow-right"></use>
               </svg>
             </a>
           </div>
         </div>
       </div>
     </div>
     <div class="it-single-slide-wrapper">
@@ -98,15 +98,15 @@
         <div class="card card-bg">
           <div class="card-body">
             <h5 class="card-title">4. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor…</h5>
             <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
             <a class="read-more" href="#">
               <span class="text">Leggi di più</span>
               <svg class="icon">
-                <use xlink:href="{% static 'svg/sprite.svg' %}#it-arrow-right"></use>
+                <use xlink:href="{% static 'svg/sprites.svg' %}#it-arrow-right"></use>
               </svg>
             </a>
           </div>
         </div>
       </div>
     </div>
     <div class="it-single-slide-wrapper">
@@ -114,15 +114,15 @@
         <div class="card card-bg">
           <div class="card-body">
             <h5 class="card-title">4. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor…</h5>
             <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
             <a class="read-more" href="#">
               <span class="text">Leggi di più</span>
               <svg class="icon">
-                <use xlink:href="{% static 'svg/sprite.svg' %}#it-arrow-right"></use>
+                <use xlink:href="{% static 'svg/sprites.svg' %}#it-arrow-right"></use>
               </svg>
             </a>
           </div>
         </div>
       </div>
     </div>
     <div class="it-single-slide-wrapper">
@@ -130,15 +130,15 @@
         <div class="card card-bg">
           <div class="card-body">
             <h5 class="card-title">4. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor…</h5>
             <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
             <a class="read-more" href="#">
               <span class="text">Leggi di più</span>
               <svg class="icon">
-                <use xlink:href="{% static 'svg/sprite.svg' %}#it-arrow-right"></use>
+                <use xlink:href="{% static 'svg/sprites.svg' %}#it-arrow-right"></use>
               </svg>
             </a>
           </div>
         </div>
       </div>
     </div>
     <div class="it-single-slide-wrapper">
@@ -146,15 +146,15 @@
         <div class="card card-bg">
           <div class="card-body">
             <h5 class="card-title">4. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor…</h5>
             <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
             <a class="read-more" href="#">
               <span class="text">Leggi di più</span>
               <svg class="icon">
-                <use xlink:href="{% static 'svg/sprite.svg' %}#it-arrow-right"></use>
+                <use xlink:href="{% static 'svg/sprites.svg' %}#it-arrow-right"></use>
               </svg>
             </a>
           </div>
         </div>
       </div>
     </div>
   </div>
@@ -168,23 +168,23 @@
 {% block bottom_scripts %}
 <script src="{% static 'js/bootstrap-italia.bundle.min.js' %}"></script>
 
 <!-- Notification per tornare alla pagina principale -->
 <div class="notification dismissable with-icon" role="alert" id="notification-esempi" aria-labelledby="notification-esempi-title">
     <h5 id="notification-esempi-title">
         <svg class="icon">
-            <use xlink:href="{% static 'svg/sprite.svg' %}#it-info-circle"></use>
+            <use xlink:href="{% static 'svg/sprites.svg' %}#it-info-circle"></use>
         </svg>Esempio di template vuoto
     </h5>
     <p>
         <a href="{{ site.baseurl }}/docs/esempi/">Torna alla pagina principale degli esempi</a>
     </p>
     <button type="button" class="btn notification-close">
         <svg class="icon">
-            <use xlink:href="{% static 'svg/sprite.svg' %}#it-close"></use>
+            <use xlink:href="{% static 'svg/sprites.svg' %}#it-close"></use>
         </svg>
         <span class="sr-only">Chiudi notifica: Titolo notification</span>
     </button>
 </div>
 
 <script>
 $(document).ready(function() {
```

### Comparing `django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia.egg-info/PKG-INFO` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-unical-bootstrap-italia
-Version: 1.2.0
+Version: 2.0.1
 Summary: Django theme for Università della Calabria (UNICAL) based on Bootstrap Italia theme
 Home-page: https://github.com/UniversitaDellaCalabria/django-unical-bootstrap-italia
 Author: Giuseppe De Marco, Francesco Filicetti
 Author-email: giuseppe.demarco@unical.it, francesco.filicetti@unical.it
 License: Apache 2.0
 Description: Template Django conforme a linee guida AGID per l'Università della Calabria
         ---------------------------------------------------------------------------
```

### Comparing `django-unical-bootstrap-italia-1.2.0/django_unical_bootstrap_italia.egg-info/SOURCES.txt` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.2.0/setup.py` & `django-unical-bootstrap-italia-2.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-unical-bootstrap-italia',
-    version='1.2.0',
+    version='2.0.1',
     packages=find_packages(),
     include_package_data=True,
     license='Apache 2.0',
     description="Django theme for Università della Calabria (UNICAL) based on Bootstrap Italia theme",
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/UniversitaDellaCalabria/django-unical-bootstrap-italia',
@@ -28,10 +28,10 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
     ],
     install_requires=[
-        'design-django-theme==1.6.4post4',
+        'design-django-theme',
     ]
 )
```

