# Comparing `tmp/django-unical-bootstrap-italia-1.0.5.tar.gz` & `tmp/django-unical-bootstrap-italia-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-unical-bootstrap-italia-1.0.5.tar", last modified: Fri Nov  5 07:42:12 2021, max compression
+gzip compressed data, was "django-unical-bootstrap-italia-2.0.1.tar", last modified: Tue Apr 11 12:24:17 2023, max compression
```

## Comparing `django-unical-bootstrap-italia-1.0.5.tar` & `django-unical-bootstrap-italia-2.0.1.tar`

### file list

```diff
@@ -1,42 +1,35 @@
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2021-11-05 07:42:12.127514 django-unical-bootstrap-italia-1.0.5/
--rw-r--r--   0 francesco  (1000) francesco  (1000)    11352 2021-11-05 07:31:39.000000 django-unical-bootstrap-italia-1.0.5/LICENSE
--rw-r--r--   0 francesco  (1000) francesco  (1000)      203 2020-02-26 11:51:00.000000 django-unical-bootstrap-italia-1.0.5/MANIFEST.in
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    16226 2021-11-05 07:42:12.127514 django-unical-bootstrap-italia-1.0.5/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    12480 2020-11-23 16:13:18.000000 django-unical-bootstrap-italia-1.0.5/README.md
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2021-11-05 07:42:12.127514 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/
--rw-r--r--   0 francesco  (1000) francesco  (1000)        0 2019-06-07 12:01:41.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/__init__.py
--rw-r--r--   0 francesco  (1000) francesco  (1000)       63 2019-06-07 12:01:41.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/admin.py
--rw-r--r--   0 francesco  (1000) francesco  (1000)      139 2020-02-26 11:41:44.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/apps.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2021-11-05 07:42:12.127514 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/migrations/
--rw-r--r--   0 francesco  (1000) francesco  (1000)        0 2019-06-07 12:01:41.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/migrations/__init__.py
--rw-r--r--   0 francesco  (1000) francesco  (1000)       57 2019-06-07 12:01:41.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/models.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2021-11-05 07:42:12.123515 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2021-11-05 07:42:12.127514 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/css/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4630 2020-03-02 13:13:57.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/css/unical-style.scss
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2021-11-05 07:42:12.127514 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2021-11-05 07:42:12.127514 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/favicon/
--rw-r--r--   0 francesco  (1000) francesco  (1000)        9 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/favicon/README.md
--rw-r--r--   0 francesco  (1000) francesco  (1000)      507 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/favicon/favicon-32x32.png
--rw-r--r--   0 francesco  (1000) francesco  (1000)     1972 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/logo.svg
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    27664 2020-11-13 09:00:35.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/logo1.svg
--rw-r--r--   0 francesco  (1000) francesco  (1000)     3499 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/logo_back.svg
--rw-r--r--   0 francesco  (1000) francesco  (1000)      799 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/logo_white.png
--rw-r--r--   0 francesco  (1000) francesco  (1000)   508364 2019-05-10 10:06:58.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/unical_banner.jpg
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    23187 2019-07-04 09:22:35.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/unical_logo.svg
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2021-11-05 07:42:12.127514 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/templates/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      240 2020-03-25 08:08:38.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/templates/404.html
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      267 2020-03-25 08:09:09.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/templates/500.html
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)    11933 2021-11-05 07:40:10.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/templates/base-setup.html
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1135 2021-06-24 06:40:43.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/templates/error-page.html
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)     8227 2019-09-24 07:38:37.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/templates/index.html
--rw-r--r--   0 francesco  (1000) francesco  (1000)       60 2019-06-07 12:01:41.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/tests.py
--rw-r--r--   0 francesco  (1000) francesco  (1000)      329 2020-02-26 11:41:57.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/urls.py
--rw-r--r--   0 francesco  (1000) francesco  (1000)      128 2019-06-07 12:01:41.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/views.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2021-11-05 07:42:12.127514 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia.egg-info/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    16226 2021-11-05 07:42:11.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia.egg-info/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1455 2021-11-05 07:42:11.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia.egg-info/SOURCES.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2021-11-05 07:42:11.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia.egg-info/dependency_links.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       33 2021-11-05 07:42:11.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia.egg-info/requires.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       31 2021-11-05 07:42:11.000000 django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia.egg-info/top_level.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2021-11-05 07:42:12.127514 django-unical-bootstrap-italia-1.0.5/setup.cfg
--rw-r--r--   0 francesco  (1000) francesco  (1000)     1314 2021-11-05 07:41:09.000000 django-unical-bootstrap-italia-1.0.5/setup.py
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

### Comparing `django-unical-bootstrap-italia-1.0.5/LICENSE` & `django-unical-bootstrap-italia-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.0.5/PKG-INFO` & `django-unical-bootstrap-italia-2.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-unical-bootstrap-italia
-Version: 1.0.5
+Version: 2.0.1
 Summary: Django theme for Università della Calabria (UNICAL) based on Bootstrap Italia theme
 Home-page: https://github.com/UniversitaDellaCalabria/django-unical-bootstrap-italia
 Author: Giuseppe De Marco, Francesco Filicetti
 Author-email: giuseppe.demarco@unical.it, francesco.filicetti@unical.it
 License: Apache 2.0
 Description: Template Django conforme a linee guida AGID per l'Università della Calabria
         ---------------------------------------------------------------------------
@@ -19,26 +19,17 @@
         _**Frontend**: Schermata di default del template_
         
         
         Requirements
         ------------
         
         ```
-        django-bootstrap-italia
-        libsass
-        django-compressor
-        django-sass-processor
+        design-django-theme
         ```
         
-        #### django-sass-processor
-        
-        Compilazione di SASS 3 (file .scss) per Django.
-        
-        https://pypi.org/project/django-sass-processor/
-        
         
         Installazione
         -------------
         
         ```
         pip install django-unical-boostrap-italia
         ```
@@ -56,60 +47,38 @@
         principali, al fine di personalizzare le sezioni di interesse;
         - Ogni pagina HTML del proprio progetto dovrà estendere ```base-setup.html```
         e definire il contenuto del blocco ```{% container %}```. Header e Footer
         saranno sempre ereditati da ```base-setup.html```, a meno di variazioni su
         singole pagine.
         
         
-        Stile e CSS/SCSS
+        Stile e CSS
         ----------------
         
-        Si utilizza [django-sass-processor](https://github.com/jrief/django-sass-processor).
-        
-        Per la personalizzazione dello stile del template (colori, dimensioni, sfondi)
-        si utilizza SASS 3 (Syntactically Awesome Style Sheets), in modo
-        da rispettare le caratteristiche responsive ereditate.
-        
         Il foglio di stile che ridefinisce l'aspetto del tema di default è
         ```static/css/unical-style.scss```.
         
         Per la compilazione offline del file .scss in .css,  generando l corrispettivo
         ```unical-style.css```, questi i comandi:
         
         ```
-        python manage.py compilescss
         python manage.py collectstatic
-        ``` 
-        
-        Se si vuole creare il file .css compilato nella directory SASS_PROCESSOR_ROOT (se non specificata STATIC_ROOT):
         ```
-        python manage.py collectstatic  --use-processor-root
-        ```
-        
-        Nel caso in cui non si volessero esporre i file SASS/SCSS in un ambiente
-        di produzione utilizzare:
-        
-        ```python manage.py collectstatic --ignore=*.scss```
-        
-        Per eliminare i file css compilati nelle directory statiche:
-        
-        ```python manage.py compilescss --delete-files```
         
         E' sempre possibile integrare fogli di stile o javascript
         effettuando l'overload del blocco ```{% extra_head %}```.
         
         
         Esempio di base-setup.html
         --------------------
         
         ```
         <!-- Extends default Bootstrap Italia template -->
         {% extends 'bootstrap-italia-base.html' %}
         
-        {% load sass_tags %}
         {% load static %}
         
         <!-- Page Title -->
         {% block page_title %}
         Università della Calabria
         {% endblock page_title %}
         
@@ -370,13 +339,14 @@
         ```
         
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `django-unical-bootstrap-italia-1.0.5/README.md` & `django-unical-bootstrap-italia-2.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,26 +11,17 @@
 _**Frontend**: Schermata di default del template_
 
 
 Requirements
 ------------
 
 ```
-django-bootstrap-italia
-libsass
-django-compressor
-django-sass-processor
+design-django-theme
 ```
 
-#### django-sass-processor
-
-Compilazione di SASS 3 (file .scss) per Django.
-
-https://pypi.org/project/django-sass-processor/
-
 
 Installazione
 -------------
 
 ```
 pip install django-unical-boostrap-italia
 ```
@@ -48,60 +39,38 @@
 principali, al fine di personalizzare le sezioni di interesse;
 - Ogni pagina HTML del proprio progetto dovrà estendere ```base-setup.html```
 e definire il contenuto del blocco ```{% container %}```. Header e Footer
 saranno sempre ereditati da ```base-setup.html```, a meno di variazioni su
 singole pagine.
 
 
-Stile e CSS/SCSS
+Stile e CSS
 ----------------
 
-Si utilizza [django-sass-processor](https://github.com/jrief/django-sass-processor).
-
-Per la personalizzazione dello stile del template (colori, dimensioni, sfondi)
-si utilizza SASS 3 (Syntactically Awesome Style Sheets), in modo
-da rispettare le caratteristiche responsive ereditate.
-
 Il foglio di stile che ridefinisce l'aspetto del tema di default è
 ```static/css/unical-style.scss```.
 
 Per la compilazione offline del file .scss in .css,  generando l corrispettivo
 ```unical-style.css```, questi i comandi:
 
 ```
-python manage.py compilescss
 python manage.py collectstatic
-``` 
-
-Se si vuole creare il file .css compilato nella directory SASS_PROCESSOR_ROOT (se non specificata STATIC_ROOT):
 ```
-python manage.py collectstatic  --use-processor-root
-```
-
-Nel caso in cui non si volessero esporre i file SASS/SCSS in un ambiente
-di produzione utilizzare:
-
-```python manage.py collectstatic --ignore=*.scss```
-
-Per eliminare i file css compilati nelle directory statiche:
-
-```python manage.py compilescss --delete-files```
 
 E' sempre possibile integrare fogli di stile o javascript
 effettuando l'overload del blocco ```{% extra_head %}```.
 
 
 Esempio di base-setup.html
 --------------------
 
 ```
 <!-- Extends default Bootstrap Italia template -->
 {% extends 'bootstrap-italia-base.html' %}
 
-{% load sass_tags %}
 {% load static %}
 
 <!-- Page Title -->
 {% block page_title %}
 Università della Calabria
 {% endblock page_title %}
```

### Comparing `django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/logo.svg` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/logo1.svg` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/logo1.svg`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/logo_back.svg` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/logo_back.svg`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/logo_white.png` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/logo_white.png`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/unical_banner.jpg` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/unical_banner.jpg`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/static/images/unical_logo.svg` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/static/images/unical_logo.svg`

 * *Files identical despite different names*

### Comparing `django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/templates/base-setup.html` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/templates/base-setup.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 <!-- Extends default Bootstrap Italia template -->
 {% extends 'bootstrap-italia-base.html' %}
 
-{% load sass_tags %}
 {% load static %}
 
 <!-- Page Title -->
 {% block page_title %}
 Università della Calabria
 {% endblock page_title %}
 
 <!-- My custom scss sheet -->
 {% block extra_head %}
 <link rel="shortcut icon" href="{% static 'images/favicon/favicon-32x32.png' %}">
-<link rel="stylesheet" href="{% sass_src 'css/unical-style.scss' %}" type="text/css" />
+<link rel="stylesheet" href="{% static 'css/unical-style.css' %}" type="text/css" />
 {% endblock extra_head %}
 
 <!-- URL link top left -->
 {% block header_slim_org_url %}
 https://www.unical.it
 {% endblock header_slim_org_url %}
 
@@ -35,51 +34,51 @@
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
 
@@ -190,57 +189,57 @@
                     </li>
                 </ul>
             </div>
         </div>
         <div class="col-lg-4 col-md-4 pb-2">
             <div class="pb-2">
                 <h4><a href="#" title="Vai alla pagina: Seguici su">Seguici su</a></h4>
-                <ul class="list-inline text-left social">
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
@@ -1,10 +1,10 @@
- {% extends 'bootstrap-italia-base.html' %} {% load sass_tags %} {% load static
-%}  {% block page_title %} UniversitÃ  della Calabria {% endblock page_title %}
-{% block extra_head %}
+ {% extends 'bootstrap-italia-base.html' %} {% load static %}  {% block
+page_title %} UniversitÃ  della Calabria {% endblock page_title %}  {% block
+extra_head %}
 
  {% endblock extra_head %}  {% block header_slim_org_url %} https://
 www.unical.it {% endblock header_slim_org_url %}  {% block header_slim_org_name
 %} UniversitÃ  della Calabria {% endblock header_slim_org_name %}  {% block
 header_slim_mobile_org_name %} UniversitÃ  della Calabria {% endblock
 header_slim_mobile_org_name %} {% block header_center_social %}
 Seguici su
```

### Comparing `django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/templates/error-page.html` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/templates/error-page.html`

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

### Comparing `django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia/templates/index.html` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia/templates/index.html`

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

### Comparing `django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia.egg-info/PKG-INFO` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-unical-bootstrap-italia
-Version: 1.0.5
+Version: 2.0.1
 Summary: Django theme for Università della Calabria (UNICAL) based on Bootstrap Italia theme
 Home-page: https://github.com/UniversitaDellaCalabria/django-unical-bootstrap-italia
 Author: Giuseppe De Marco, Francesco Filicetti
 Author-email: giuseppe.demarco@unical.it, francesco.filicetti@unical.it
 License: Apache 2.0
 Description: Template Django conforme a linee guida AGID per l'Università della Calabria
         ---------------------------------------------------------------------------
@@ -19,26 +19,17 @@
         _**Frontend**: Schermata di default del template_
         
         
         Requirements
         ------------
         
         ```
-        django-bootstrap-italia
-        libsass
-        django-compressor
-        django-sass-processor
+        design-django-theme
         ```
         
-        #### django-sass-processor
-        
-        Compilazione di SASS 3 (file .scss) per Django.
-        
-        https://pypi.org/project/django-sass-processor/
-        
         
         Installazione
         -------------
         
         ```
         pip install django-unical-boostrap-italia
         ```
@@ -56,60 +47,38 @@
         principali, al fine di personalizzare le sezioni di interesse;
         - Ogni pagina HTML del proprio progetto dovrà estendere ```base-setup.html```
         e definire il contenuto del blocco ```{% container %}```. Header e Footer
         saranno sempre ereditati da ```base-setup.html```, a meno di variazioni su
         singole pagine.
         
         
-        Stile e CSS/SCSS
+        Stile e CSS
         ----------------
         
-        Si utilizza [django-sass-processor](https://github.com/jrief/django-sass-processor).
-        
-        Per la personalizzazione dello stile del template (colori, dimensioni, sfondi)
-        si utilizza SASS 3 (Syntactically Awesome Style Sheets), in modo
-        da rispettare le caratteristiche responsive ereditate.
-        
         Il foglio di stile che ridefinisce l'aspetto del tema di default è
         ```static/css/unical-style.scss```.
         
         Per la compilazione offline del file .scss in .css,  generando l corrispettivo
         ```unical-style.css```, questi i comandi:
         
         ```
-        python manage.py compilescss
         python manage.py collectstatic
-        ``` 
-        
-        Se si vuole creare il file .css compilato nella directory SASS_PROCESSOR_ROOT (se non specificata STATIC_ROOT):
         ```
-        python manage.py collectstatic  --use-processor-root
-        ```
-        
-        Nel caso in cui non si volessero esporre i file SASS/SCSS in un ambiente
-        di produzione utilizzare:
-        
-        ```python manage.py collectstatic --ignore=*.scss```
-        
-        Per eliminare i file css compilati nelle directory statiche:
-        
-        ```python manage.py compilescss --delete-files```
         
         E' sempre possibile integrare fogli di stile o javascript
         effettuando l'overload del blocco ```{% extra_head %}```.
         
         
         Esempio di base-setup.html
         --------------------
         
         ```
         <!-- Extends default Bootstrap Italia template -->
         {% extends 'bootstrap-italia-base.html' %}
         
-        {% load sass_tags %}
         {% load static %}
         
         <!-- Page Title -->
         {% block page_title %}
         Università della Calabria
         {% endblock page_title %}
         
@@ -370,13 +339,14 @@
         ```
         
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `django-unical-bootstrap-italia-1.0.5/django_unical_bootstrap_italia.egg-info/SOURCES.txt` & `django-unical-bootstrap-italia-2.0.1/django_unical_bootstrap_italia.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 django_unical_bootstrap_italia/__init__.py
-django_unical_bootstrap_italia/admin.py
 django_unical_bootstrap_italia/apps.py
-django_unical_bootstrap_italia/models.py
-django_unical_bootstrap_italia/tests.py
-django_unical_bootstrap_italia/urls.py
-django_unical_bootstrap_italia/views.py
 django_unical_bootstrap_italia.egg-info/PKG-INFO
 django_unical_bootstrap_italia.egg-info/SOURCES.txt
 django_unical_bootstrap_italia.egg-info/dependency_links.txt
 django_unical_bootstrap_italia.egg-info/requires.txt
 django_unical_bootstrap_italia.egg-info/top_level.txt
-django_unical_bootstrap_italia/migrations/__init__.py
-django_unical_bootstrap_italia/static/css/unical-style.scss
+django_unical_bootstrap_italia/static/css/unical-style.css
 django_unical_bootstrap_italia/static/images/logo.svg
 django_unical_bootstrap_italia/static/images/logo1.svg
 django_unical_bootstrap_italia/static/images/logo_back.svg
 django_unical_bootstrap_italia/static/images/logo_white.png
 django_unical_bootstrap_italia/static/images/unical_banner.jpg
 django_unical_bootstrap_italia/static/images/unical_logo.svg
 django_unical_bootstrap_italia/static/images/favicon/README.md
```

### Comparing `django-unical-bootstrap-italia-1.0.5/setup.py` & `django-unical-bootstrap-italia-2.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,32 +5,33 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-unical-bootstrap-italia',
-    version='1.0.5',
+    version='2.0.1',
     packages=find_packages(),
     include_package_data=True,
     license='Apache 2.0',
     description="Django theme for Università della Calabria (UNICAL) based on Bootstrap Italia theme",
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/UniversitaDellaCalabria/django-unical-bootstrap-italia',
     author='Giuseppe De Marco, Francesco Filicetti',
     author_email='giuseppe.demarco@unical.it, francesco.filicetti@unical.it',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 2.0',
         'Framework :: Django :: 3.0',
+        'Framework :: Django :: 4.0',
         'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
+        'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
     ],
     install_requires=[
-        'design-django-theme>=1.3.9.post3',
+        'design-django-theme',
     ]
 )
```

