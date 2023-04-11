# Comparing `tmp/django-oscar-pg-search-0.8.9.tar.gz` & `tmp/django-oscar-pg-search-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oscar-pg-search-0.8.9.tar", last modified: Mon Mar 21 12:54:53 2022, max compression
+gzip compressed data, was "django-oscar-pg-search-0.9.0.tar", last modified: Tue Apr 11 20:00:08 2023, max compression
```

## Comparing `django-oscar-pg-search-0.8.9.tar` & `django-oscar-pg-search-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 12:54:53.688756 django-oscar-pg-search-0.8.9/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3344 2022-03-21 12:54:53.688756 django-oscar-pg-search-0.8.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2505 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-21 12:54:45.000000 django-oscar-pg-search-0.8.9/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-21 12:54:53.688756 django-oscar-pg-search-0.8.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 12:54:53.684756 django-oscar-pg-search-0.8.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 12:54:53.684756 django-oscar-pg-search-0.8.9/src/django_oscar_pg_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3344 2022-03-21 12:54:53.000000 django-oscar-pg-search-0.8.9/src/django_oscar_pg_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-03-21 12:54:53.000000 django-oscar-pg-search-0.8.9/src/django_oscar_pg_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-21 12:54:53.000000 django-oscar-pg-search-0.8.9/src/django_oscar_pg_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-03-21 12:54:53.000000 django-oscar-pg-search-0.8.9/src/django_oscar_pg_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-03-21 12:54:53.000000 django-oscar-pg-search-0.8.9/src/django_oscar_pg_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 12:54:53.684756 django-oscar-pg-search-0.8.9/src/oscar_pg_search/
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/src/oscar_pg_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/src/oscar_pg_search/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)    18322 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/src/oscar_pg_search/filter_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     4433 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/src/oscar_pg_search/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/src/oscar_pg_search/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     2674 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/src/oscar_pg_search/order_by_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     9341 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/src/oscar_pg_search/postgres_search_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/src/oscar_pg_search/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 12:54:53.684756 django-oscar-pg-search-0.8.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      655 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/tests/manage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1691 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/tests/test_search_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-03-21 12:54:40.000000 django-oscar-pg-search-0.8.9/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:00:08.807106 django-oscar-pg-search-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-11 20:00:08.803106 django-oscar-pg-search-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 20:00:01.000000 django-oscar-pg-search-0.9.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 20:00:08.807106 django-oscar-pg-search-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:00:08.795106 django-oscar-pg-search-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:00:08.799106 django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-11 20:00:08.000000 django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-11 20:00:08.000000 django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:00:08.000000 django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 20:00:08.000000 django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 20:00:08.000000 django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:00:08.799106 django-oscar-pg-search-0.9.0/src/oscar_pg_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:00:08.803106 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/attribute_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/base_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/base_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/filter_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/offer_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/filter_options/product_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/order_by_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/postgres_search_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/src/oscar_pg_search/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:00:08.803106 django-oscar-pg-search-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/tests/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/tests/test_search_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-11 19:59:58.000000 django-oscar-pg-search-0.9.0/tests/urls.py
```

### Comparing `django-oscar-pg-search-0.8.9/PKG-INFO` & `django-oscar-pg-search-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,111 +1,99 @@
 Metadata-Version: 2.1
 Name: django-oscar-pg-search
-Version: 0.8.9
+Version: 0.9.0
 Summary: Pure Postgresql search backend for Django Oscar
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
 
+[![Maintainability](https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml/badge.svg)](https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml)
+[![Maintainability](https://api.codeclimate.com/v1/badges/a289293e4e1af1114d74/maintainability)](https://codeclimate.com/github/snake-soft/django-oscar-pg-search/maintainability)
+[![image](https://codecov.io/gh/snake-soft/django-oscar-pg-search/branch/master/graph/badge.svg?token=TALCIZ5E3Q)](https://codecov.io/gh/snake-soft/django-oscar-pg-search)
+[![image](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
-.. image:: https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml/badge.svg
-   :target: https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml
-   :alt: Maintainability
-
-.. image:: https://api.codeclimate.com/v1/badges/a289293e4e1af1114d74/maintainability
-   :target: https://codeclimate.com/github/snake-soft/django-oscar-pg-search/maintainability
-   :alt: Maintainability
 
-.. image:: https://codecov.io/gh/snake-soft/django-oscar-pg-search/branch/master/graph/badge.svg?token=TALCIZ5E3Q
-   :target: https://codecov.io/gh/snake-soft/django-oscar-pg-search
-
-.. image:: https://img.shields.io/badge/License-GPLv3-blue.svg
-   :target: https://www.gnu.org/licenses/gpl-3.0
-
-==========================================
 Postgresql search handler for Django-Oscar
 ==========================================
+This creates a search handler without the need of any search backend. It is designed for the e-commerce framework [Oscar](https://github.com/django-oscar/django-oscar).
 
-Careful: This is originally created inside a project not tested in a reusable environment, yet.
-
-This creates a search handler without the need of any search backend.
-It is designed for the e-commerce framework `Oscar`_.
-
-.. _`Oscar`: https://github.com/django-oscar/django-oscar
-
-
-It is implemented a little bit expensive but uses 4 annotated search vectors:
-* upc
-* title
-* meta_description
-* meta_title
+It is implemented a little bit expensive but uses 4 annotated search vectors: \* upc \* title \* meta\_description \* meta\_title
 
-This way the search can be manipulated through the meta fields.
-This package is not testet against generic sites, yet.
-It is running productive in a heavily customized env for many months now.
-I think it should scale up to 5000 Products with 10 Attributes depending on how the products are loaded.
-We use it fully lazy with endless scrolling.
+This way the search can be manipulated through the meta fields. It is running productive in a heavily customized env for many months now. I think it should scale up to 5000 Products with 10 Attributes depending on how the products are loaded. We use it fully lazy with endless scrolling.
 
 
 To-Do
 -----
-* Dynamic creation of the filter fields
-* Writing Tests
+
+- Provide a generic way to use filter forms
+- Writing Tests
 
 
 Features
 --------
 
-* Don't need to use some additional search backend like elastic
-* Creates filters (facets) for:
-	* Data that is directly attached to the Product model including foreign key choices
-	* AttributeValues of the products
-	* StockRecord entries
++ Don't need to use some additional search backend like elastic
++ Creates filters (facets) for:
+    - Data that is directly attached to the Product model
+    - including foreign key choices
+    - AttributeValues of the products
+    - StockRecord entries
 
 
 Installation
 ------------
 
 Install using pip:
 
-.. code-block:: bash
-
-	pip install django-oscar-pg-search
-
-
-.. code-block:: python
+```bash
+pip install django-oscar-pg-search
+```
+
+```python
+# settings.py
+
+# replace 'oscar.apps.search.apps.SearchConfig' by 'oscar_pg_search.apps.PgSearchConfig'
+INSTALLED_APPS = [
+	# 'oscar.apps.search.apps.SearchConfig',
+    'oscar_pg_search.apps.PgSearchConfig',
+]
+
+OSCAR_PRODUCT_SEARCH_HANDLER = 'oscar_pg_search.postgres_search_handler.PostgresSearchHandler'
+
+# To avoid exception, haystack is not used:
+HAYSTACK_CONNECTIONS = {"default": {}}
+```
+
+Trigram search is our search algorithm. Enable it at your database by executing the following sql:
+
+```
+CREATE EXTENSION pg_trgm;
+```
 
-   # settings.py
-   INSTALLED_APPS = [
-       # ...
-       'oscar_pg_search.apps.PgSearchConfig',
-       # ...
-   ]
-   OSCAR_PRODUCT_SEARCH_HANDLER = 'oscar_pg_search.postgres_search_handler.PostgresSearchHandler'
 
 Settings
 --------
 
-If you want to add some fields that are directly attached to the Product model:
-
-.. code-block:: python
-
-   # settings.py
-   OSCAR_ATTACHED_PRODUCT_FIELDS = ['is_public', 'deposit', 'volume', 'weight',]
-
+If you want to add some fields that are directly attached to the Product
+model:
 
+```python
+# settings.py
+OSCAR_ATTACHED_PRODUCT_FIELDS = ['is_public', 'deposit', 'volume', 'weight',]
+```
```

### Comparing `django-oscar-pg-search-0.8.9/README.rst` & `django-oscar-pg-search-0.9.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,74 @@
+[![Maintainability](https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml/badge.svg)](https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml)
+[![Maintainability](https://api.codeclimate.com/v1/badges/a289293e4e1af1114d74/maintainability)](https://codeclimate.com/github/snake-soft/django-oscar-pg-search/maintainability)
+[![image](https://codecov.io/gh/snake-soft/django-oscar-pg-search/branch/master/graph/badge.svg?token=TALCIZ5E3Q)](https://codecov.io/gh/snake-soft/django-oscar-pg-search)
+[![image](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
-.. image:: https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml/badge.svg
-   :target: https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml
-   :alt: Maintainability
-
-.. image:: https://api.codeclimate.com/v1/badges/a289293e4e1af1114d74/maintainability
-   :target: https://codeclimate.com/github/snake-soft/django-oscar-pg-search/maintainability
-   :alt: Maintainability
 
-.. image:: https://codecov.io/gh/snake-soft/django-oscar-pg-search/branch/master/graph/badge.svg?token=TALCIZ5E3Q
-   :target: https://codecov.io/gh/snake-soft/django-oscar-pg-search
-
-.. image:: https://img.shields.io/badge/License-GPLv3-blue.svg
-   :target: https://www.gnu.org/licenses/gpl-3.0
-
-==========================================
 Postgresql search handler for Django-Oscar
 ==========================================
+This creates a search handler without the need of any search backend. It is designed for the e-commerce framework [Oscar](https://github.com/django-oscar/django-oscar).
 
-Careful: This is originally created inside a project not tested in a reusable environment, yet.
-
-This creates a search handler without the need of any search backend.
-It is designed for the e-commerce framework `Oscar`_.
-
-.. _`Oscar`: https://github.com/django-oscar/django-oscar
-
+It is implemented a little bit expensive but uses 4 annotated search vectors: \* upc \* title \* meta\_description \* meta\_title
 
-It is implemented a little bit expensive but uses 4 annotated search vectors:
-* upc
-* title
-* meta_description
-* meta_title
-
-This way the search can be manipulated through the meta fields.
-This package is not testet against generic sites, yet.
-It is running productive in a heavily customized env for many months now.
-I think it should scale up to 5000 Products with 10 Attributes depending on how the products are loaded.
-We use it fully lazy with endless scrolling.
+This way the search can be manipulated through the meta fields. It is running productive in a heavily customized env for many months now. I think it should scale up to 5000 Products with 10 Attributes depending on how the products are loaded. We use it fully lazy with endless scrolling.
 
 
 To-Do
 -----
-* Dynamic creation of the filter fields
-* Writing Tests
+
+- Provide a generic way to use filter forms
+- Writing Tests
 
 
 Features
 --------
 
-* Don't need to use some additional search backend like elastic
-* Creates filters (facets) for:
-	* Data that is directly attached to the Product model including foreign key choices
-	* AttributeValues of the products
-	* StockRecord entries
++ Don't need to use some additional search backend like elastic
++ Creates filters (facets) for:
+    - Data that is directly attached to the Product model
+    - including foreign key choices
+    - AttributeValues of the products
+    - StockRecord entries
 
 
 Installation
 ------------
 
 Install using pip:
 
-.. code-block:: bash
-
-	pip install django-oscar-pg-search
+```bash
+pip install django-oscar-pg-search
+```
+
+```python
+# settings.py
+
+# replace 'oscar.apps.search.apps.SearchConfig' by 'oscar_pg_search.apps.PgSearchConfig'
+INSTALLED_APPS = [
+	# 'oscar.apps.search.apps.SearchConfig',
+    'oscar_pg_search.apps.PgSearchConfig',
+]
+
+OSCAR_PRODUCT_SEARCH_HANDLER = 'oscar_pg_search.postgres_search_handler.PostgresSearchHandler'
+
+# To avoid exception, haystack is not used:
+HAYSTACK_CONNECTIONS = {"default": {}}
+```
+
+Trigram search is our search algorithm. Enable it at your database by executing the following sql:
+
+```
+CREATE EXTENSION pg_trgm;
+```
 
 
-.. code-block:: python
-
-   # settings.py
-   INSTALLED_APPS = [
-       # ...
-       'oscar_pg_search.apps.PgSearchConfig',
-       # ...
-   ]
-   OSCAR_PRODUCT_SEARCH_HANDLER = 'oscar_pg_search.postgres_search_handler.PostgresSearchHandler'
-
 Settings
 --------
 
-If you want to add some fields that are directly attached to the Product model:
-
-.. code-block:: python
+If you want to add some fields that are directly attached to the Product
+model:
 
-   # settings.py
-   OSCAR_ATTACHED_PRODUCT_FIELDS = ['is_public', 'deposit', 'volume', 'weight',]
+```python
+# settings.py
+OSCAR_ATTACHED_PRODUCT_FIELDS = ['is_public', 'deposit', 'volume', 'weight',]
+```
```

### Comparing `django-oscar-pg-search-0.8.9/setup.py` & `django-oscar-pg-search-0.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #!/usr/bin/env python
 from setuptools import find_packages, setup
 from src.oscar_pg_search import __version__
 
 
 install_requires = [
     'django>=3.0,<3.3',
-    'django-oscar>=2.0,<3.2',
+    'django-oscar>=2.0,<3.3',
 ]
 
 tests_require = [
     'coverage>=5.5,<5.6',
 ]
 
 setup(
     name='django-oscar-pg-search',
     version=__version__,
     author="Snake-Soft",
     author_email="info@snake-soft.com",
     description="Pure Postgresql search backend for Django Oscar",
-    long_description=open('README.rst').read(),
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     license='BSD',
     package_dir={'': 'src'},
     packages=find_packages('src'),
     include_package_data=True,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Web Environment',
```

### Comparing `django-oscar-pg-search-0.8.9/src/django_oscar_pg_search.egg-info/PKG-INFO` & `django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,111 +1,99 @@
 Metadata-Version: 2.1
 Name: django-oscar-pg-search
-Version: 0.8.9
+Version: 0.9.0
 Summary: Pure Postgresql search backend for Django Oscar
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
 
+[![Maintainability](https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml/badge.svg)](https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml)
+[![Maintainability](https://api.codeclimate.com/v1/badges/a289293e4e1af1114d74/maintainability)](https://codeclimate.com/github/snake-soft/django-oscar-pg-search/maintainability)
+[![image](https://codecov.io/gh/snake-soft/django-oscar-pg-search/branch/master/graph/badge.svg?token=TALCIZ5E3Q)](https://codecov.io/gh/snake-soft/django-oscar-pg-search)
+[![image](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
-.. image:: https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml/badge.svg
-   :target: https://github.com/snake-soft/django-oscar-pg-search/actions/workflows/django.yml
-   :alt: Maintainability
-
-.. image:: https://api.codeclimate.com/v1/badges/a289293e4e1af1114d74/maintainability
-   :target: https://codeclimate.com/github/snake-soft/django-oscar-pg-search/maintainability
-   :alt: Maintainability
 
-.. image:: https://codecov.io/gh/snake-soft/django-oscar-pg-search/branch/master/graph/badge.svg?token=TALCIZ5E3Q
-   :target: https://codecov.io/gh/snake-soft/django-oscar-pg-search
-
-.. image:: https://img.shields.io/badge/License-GPLv3-blue.svg
-   :target: https://www.gnu.org/licenses/gpl-3.0
-
-==========================================
 Postgresql search handler for Django-Oscar
 ==========================================
+This creates a search handler without the need of any search backend. It is designed for the e-commerce framework [Oscar](https://github.com/django-oscar/django-oscar).
 
-Careful: This is originally created inside a project not tested in a reusable environment, yet.
-
-This creates a search handler without the need of any search backend.
-It is designed for the e-commerce framework `Oscar`_.
-
-.. _`Oscar`: https://github.com/django-oscar/django-oscar
-
-
-It is implemented a little bit expensive but uses 4 annotated search vectors:
-* upc
-* title
-* meta_description
-* meta_title
+It is implemented a little bit expensive but uses 4 annotated search vectors: \* upc \* title \* meta\_description \* meta\_title
 
-This way the search can be manipulated through the meta fields.
-This package is not testet against generic sites, yet.
-It is running productive in a heavily customized env for many months now.
-I think it should scale up to 5000 Products with 10 Attributes depending on how the products are loaded.
-We use it fully lazy with endless scrolling.
+This way the search can be manipulated through the meta fields. It is running productive in a heavily customized env for many months now. I think it should scale up to 5000 Products with 10 Attributes depending on how the products are loaded. We use it fully lazy with endless scrolling.
 
 
 To-Do
 -----
-* Dynamic creation of the filter fields
-* Writing Tests
+
+- Provide a generic way to use filter forms
+- Writing Tests
 
 
 Features
 --------
 
-* Don't need to use some additional search backend like elastic
-* Creates filters (facets) for:
-	* Data that is directly attached to the Product model including foreign key choices
-	* AttributeValues of the products
-	* StockRecord entries
++ Don't need to use some additional search backend like elastic
++ Creates filters (facets) for:
+    - Data that is directly attached to the Product model
+    - including foreign key choices
+    - AttributeValues of the products
+    - StockRecord entries
 
 
 Installation
 ------------
 
 Install using pip:
 
-.. code-block:: bash
-
-	pip install django-oscar-pg-search
-
-
-.. code-block:: python
+```bash
+pip install django-oscar-pg-search
+```
+
+```python
+# settings.py
+
+# replace 'oscar.apps.search.apps.SearchConfig' by 'oscar_pg_search.apps.PgSearchConfig'
+INSTALLED_APPS = [
+	# 'oscar.apps.search.apps.SearchConfig',
+    'oscar_pg_search.apps.PgSearchConfig',
+]
+
+OSCAR_PRODUCT_SEARCH_HANDLER = 'oscar_pg_search.postgres_search_handler.PostgresSearchHandler'
+
+# To avoid exception, haystack is not used:
+HAYSTACK_CONNECTIONS = {"default": {}}
+```
+
+Trigram search is our search algorithm. Enable it at your database by executing the following sql:
+
+```
+CREATE EXTENSION pg_trgm;
+```
 
-   # settings.py
-   INSTALLED_APPS = [
-       # ...
-       'oscar_pg_search.apps.PgSearchConfig',
-       # ...
-   ]
-   OSCAR_PRODUCT_SEARCH_HANDLER = 'oscar_pg_search.postgres_search_handler.PostgresSearchHandler'
 
 Settings
 --------
 
-If you want to add some fields that are directly attached to the Product model:
-
-.. code-block:: python
-
-   # settings.py
-   OSCAR_ATTACHED_PRODUCT_FIELDS = ['is_public', 'deposit', 'volume', 'weight',]
-
+If you want to add some fields that are directly attached to the Product
+model:
 
+```python
+# settings.py
+OSCAR_ATTACHED_PRODUCT_FIELDS = ['is_public', 'deposit', 'volume', 'weight',]
+```
```

### Comparing `django-oscar-pg-search-0.8.9/src/django_oscar_pg_search.egg-info/SOURCES.txt` & `django-oscar-pg-search-0.9.0/src/django_oscar_pg_search.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+LICENSE
 MANIFEST.in
-README.rst
+README.md
 VERSION
 setup.py
 src/django_oscar_pg_search.egg-info/PKG-INFO
 src/django_oscar_pg_search.egg-info/SOURCES.txt
 src/django_oscar_pg_search.egg-info/dependency_links.txt
 src/django_oscar_pg_search.egg-info/requires.txt
 src/django_oscar_pg_search.egg-info/top_level.txt
 src/oscar_pg_search/__init__.py
 src/oscar_pg_search/apps.py
-src/oscar_pg_search/filter_options.py
 src/oscar_pg_search/forms.py
 src/oscar_pg_search/mixins.py
 src/oscar_pg_search/order_by_options.py
 src/oscar_pg_search/postgres_search_handler.py
 src/oscar_pg_search/utils.py
+src/oscar_pg_search/filter_options/__init__.py
+src/oscar_pg_search/filter_options/attribute_fields.py
+src/oscar_pg_search/filter_options/base_fields.py
+src/oscar_pg_search/filter_options/base_form.py
+src/oscar_pg_search/filter_options/filter_forms.py
+src/oscar_pg_search/filter_options/offer_fields.py
+src/oscar_pg_search/filter_options/product_fields.py
 tests/__init__.py
 tests/manage.py
 tests/settings.py
 tests/test_search_handler.py
 tests/urls.py
```

### Comparing `django-oscar-pg-search-0.8.9/src/oscar_pg_search/apps.py` & `django-oscar-pg-search-0.9.0/src/oscar_pg_search/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.8.9/src/oscar_pg_search/forms.py` & `django-oscar-pg-search-0.9.0/src/oscar_pg_search/forms.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import defaultdict
 from django.conf import settings
 from django import forms
 from django.utils.translation import gettext_lazy as _
 from django.forms.widgets import Input
+from django.http.request import QueryDict
 from .order_by_options import *
 
 
 class SearchInput(Input):
     """
     Defining a search type widget
 
@@ -26,74 +27,83 @@
 
 class OrderForm(forms.Form):
     sort_by = forms.ChoiceField(
         label=_("Sort by"), choices=[],
         widget=forms.Select(), required=False)
     sort_by.widget.attrs.update({'onchange': 'submitOrderForm(this.form);'})
 
-    def __init__(self, request, request_data, *args, **kwargs):
-        super().__init__(request_data, *args, **kwargs)
+    def __init__(self, request_data, *args, request=None, **kwargs):
+        assert isinstance(request_data, QueryDict)
+        self.request_data = request_data
         self.request = request
+        super().__init__(request_data, *args, **kwargs)
         self.fields['sort_by'].choices = self.get_sort_by_choices()
 
     @property
     def choice_objects(self):
         return [
             RankOrderByOption(
-                self.request,
+                self.request_data,
                 'relevancy',
                 _('Relevancy'),
                 '-rank',
+                request=self.request,
             ),
             OrderByOption(
-                self.request,
+                self.request_data,
                 'newest',
                 'Neuste Artikel',
                 '-date_created',
+                request=self.request,
             ),
             OrderByOption(
-                self.request,
+                self.request_data,
                 'updated',
                 'Letzte Änderungen',
                 '-date_updated',
+                request=self.request,
             ),
             OrderByOption(
-                self.request,
+                self.request_data,
                 'title-asc',
                 _('Title A to Z'),
                 'title',
+                request=self.request,
             ),
             OrderByOption(
-                self.request,
+                self.request_data,
                 'title-desc',
                 _('Title Z to A'),
                 '-title',
+                request=self.request,
             ),
         ]
 
     @property
     def choice_objects_with_price(self):
         return [
             PriceOrderByOption(
-                self.request,
+                self.request_data,
                 'price-asc',
                 _('Price low to high'),
-                'price',
+                'base_price',
+                request=self.request,
             ),
             PriceOrderByOption(
-                self.request,
+                self.request_data,
                 'price-desc',
                 _('Price high to low'),
-                '-price',
+                '-base_price',
+                request=self.request,
             ),
         ]
 
     def get_sort_by_choices(self):
         options = self.choice_objects
-        if not self.request.user.hide_price:
+        if self.request and not getattr(self.request.user, 'hide_price', False):
             options += self.choice_objects_with_price
         return ((choice.code, choice.name) for choice in options)
 
     def get_sort_by(self):
         if self.is_valid():
             sort_by = self.cleaned_data.get('sort_by')
             for choice in self.choice_objects + self.choice_objects_with_price:
```

### Comparing `django-oscar-pg-search-0.8.9/src/oscar_pg_search/mixins.py` & `django-oscar-pg-search-0.9.0/src/oscar_pg_search/mixins.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,21 +14,24 @@
     search_signal = user_search
     form_class = SearchForm
     http_method_names = ['get', ]
     results_per_page = settings.OSCAR_PRODUCTS_PER_PAGE
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
-        context['order_form'] = OrderForm(self.request, self.request.GET)
+        context['order_form'] = OrderForm(
+            self.request.GET,
+            request=self.request,
+        )
         context['summary'] = 'Suchergebnisse'
         if self.request.GET.get('q') and not context.get('products'):
             self.search_signal.send(
                 sender=self, session=self.request.session,
                 user=self.request.user, query=self.request.GET.get('q'))
         return context
 
     def get_search_handler(self, *args, **kwargs):
         """ Need request in the search handler """
         search_handler_class = import_string(
             settings.OSCAR_PRODUCT_SEARCH_HANDLER
         )
-        return search_handler_class(self.request, *args, **kwargs)
+        return search_handler_class(*args, request=self.request, **kwargs)
```

### Comparing `django-oscar-pg-search-0.8.9/src/oscar_pg_search/order_by_options.py` & `django-oscar-pg-search-0.9.0/src/oscar_pg_search/order_by_options.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """
 OrderByOptions are used to order the queryset just before executed on the db
 
 Therefore it is converted to a Choice in the OrderForm
 apps.search.forms.OrderForm
 """
-from django.utils.translation import gettext_lazy as _
-from django.contrib.postgres.search import SearchRank, SearchQuery
-from django.db.models.aggregates import Min
-from django.db.models import Q, When, Case, Value, BooleanField, F
+from django.contrib.postgres.search import SearchRank, SearchQuery, SearchVector
+from django.db.models import F
 from oscar.core.loading import get_class
 
 __all__ = ['OrderByOption', 'RankOrderByOption', 'PriceOrderByOption', ]
 
 Selector = get_class('partner.strategy', 'Selector')
 
 
 class OrderByOption:
     """
     This is the base class for doing every step to order the qs
     """
-    def __init__(self, request, code, name, sort_by=None):
-        self.request = request
+    def __init__(self, request_data, code, name, sort_by=None, request=None):
+        self.request_data = request_data
         self.code = code
         self.name = name
         self.sort_by = sort_by
+        self.request = request
 
     def get_ordered_qs(self, qs, query_string):
         """ This should be accessed from outside """
         return self.dispatch(qs, query_string)
 
     def dispatch(self, qs, query_string):
         qs = self.pre_order(qs, query_string)
@@ -52,35 +51,44 @@
         return qs
 
     def post_order(self, qs, *args):
         return qs
 
 
 class RankOrderByOption(OrderByOption):
-
     def order(self, qs, query_string, *args):
         if query_string:
             qs = qs.order_by('-rank')
         return qs
 
     def pre_union(self, qs, query_string, *args):
         if query_string:
-            vector = qs.model.get_search_vector()
+            default_search_fields = [
+                'title',
+                'slug',
+                'description',
+            ]
+            search_fields = getattr(
+                qs.model, 'search_fields', default_search_fields
+            )
+            vector = SearchVector(*search_fields)
             query = SearchQuery(query_string)
             qs = qs.annotate(rank=SearchRank(vector, query))
-        else:
+        elif hasattr(qs.model, 'priority'):
             qs = qs.order_by('-priority', '-date_created')
+        else:
+            qs = qs.order_by('-date_created')
         return qs
 
 
 class PriceOrderByOption(OrderByOption):
-
     def pre_union(self, qs, *args):
         """
         TODO: Need to make this domain agnostic!!!
         Currently it needs a strategy method to annotate the valid base price
         """
-        request = self.request
-        strategy = Selector().strategy(request=request, user=request.user)
-        qs = strategy.annotate_price(qs)
+        user = getattr(self.request, 'user') if self.request else None
+        strategy = Selector().strategy(request=self.request, user=user)
+        if hasattr(strategy, 'annotate_price'):
+            qs = strategy.annotate_price(qs)
         qs = qs.filter(base_price__isnull=False)
-        return qs.annotate(price=F('base_price'))
+        return qs
```

### Comparing `django-oscar-pg-search-0.8.9/src/oscar_pg_search/postgres_search_handler.py` & `django-oscar-pg-search-0.9.0/src/oscar_pg_search/postgres_search_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 
 
 class PostgresSearchHandler(SimpleProductSearchHandler):
     search_fields = ['title', 'slug', 'description']
     search_form_class = SearchForm
     order_form_class = OrderForm
 
-    def __init__(self, request, request_data, full_path, categories=None):
-        self.request = request
+    def __init__(self, request_data, full_path, categories=None, request=None):
         self.request_data = request_data
+        self.request = request
 
         self.search_form = self.search_form_class(request_data)
         self.query_string = self.search_form.get_query_string()
 
-        self.order_form = self.order_form_class(request, request_data)
+        self.order_form = self.order_form_class(request_data, request=request)
         self.order_by_option = self.order_form.get_sort_by()
 
         super().__init__(request_data, full_path, categories)
 
     @property
     def vector(self):
         return SearchVector('title', weight='A')\
@@ -54,17 +54,17 @@
     @property
     def paginate_by(self):
         if self.request_data.get('format') == 'ajax':
             return settings.OSCAR_PRODUCTS_PER_PAGE_AJAX
         return settings.OSCAR_PRODUCTS_PER_PAGE
 
     def get_queryset(self):
-        if hasattr(self.request, 'products'):
+        if self.request and hasattr(self.request, 'products'):
             qs = self.request.products
-        elif hasattr(Product, 'for_user'):
+        elif self.request and hasattr(Product, 'for_user'):
             qs = Product.for_user(self.request.user)
         else:
             qs = Product.objects.browsable()
 
         query_string = self.query_string
         if not self.categories:
             if query_string:
@@ -73,15 +73,17 @@
                 self.categories = Category.objects.browsable()
 
         if self.order_by_option:
             qs = self.order_by_option.pre_union(qs, query_string)
 
         qs = self.search(qs, query_string)
 
-        self.filter_manager = FilterManager(self.request, qs)
+        self.filter_manager = FilterManager(
+            self.request_data, qs, request=self.request
+        )
         qs = self.filter_manager.result
 
         if self.order_by_option:
             qs = self.order_by_option.post_union(qs, query_string)
             qs = self.order_by_option.get_ordered_qs(qs, self.query_string)
 
         return qs
@@ -114,14 +116,21 @@
         if connection.vendor != 'postgresql':
             ''' fallback '''
             if settings.DEBUG:
                 return qs
             else:
                 raise NotImplementedError('Create fallback for non postgres db')
         if query_string:
+            exact_query = Q(upc=query_string)
+            if hasattr(Product, 'gtins'):
+                exact_query |= Q(gtins__gtin=query_string)
+            exact_qs = qs.filter(exact_query)
+            if exact_qs.exists():
+                return exact_qs
+
             qs = qs.annotate(
                 upc_rank=Coalesce(
                     TrigramSimilarity('upc', query_string), 0,
                     output_field=models.DecimalField(),
                 ),
             )
             qs = qs.annotate(
```

### Comparing `django-oscar-pg-search-0.8.9/src/oscar_pg_search/utils.py` & `django-oscar-pg-search-0.9.0/src/oscar_pg_search/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,34 +7,33 @@
     This is the interface to all search filters.
     :param request: Request of the search
     :param qs: Product objects may be prefiltered by search or user rules
     """
     fltr_cls = FILTERS
     wishlist_as_link = False
 
-    def __init__(self, request, qs, attributes, **kwargs):
-        self.request = request
+    def __init__(self, request_data, qs, request=None):
+        self.request_data = request_data
         self.qs = qs
-        self.attributes = attributes
 
         # Domain specific logic for creating Partner based options:
-        if hasattr(request, 'partners'):
+        if request and hasattr(request, 'partners'):
             main_partner = getattr(request, 'partners')[0]
             self.wishlist_as_link = main_partner.wishlist_as_link
-        self.filters = self.get_filters()
+        self.filters = self.get_filters(request=request)
         self.result = self.get_result()
         self.initialize_filters()
 
-    def get_filters(self):
+    def get_filters(self, **kwargs):
         """
         :returns: All filter instances
         """
         fltrs = []
         for _cls in self.fltr_cls:
-            fltr = _cls(self.request, self, self.qs)
+            fltr = _cls(self.request_data, self, self.qs, **kwargs)
             fltrs.append(fltr)
         return fltrs
 
     def get_queries(self, exclude=None):
         """
         :returns: List of all queries from the filters to be combined
         """
```

### Comparing `django-oscar-pg-search-0.8.9/tests/manage.py` & `django-oscar-pg-search-0.9.0/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.8.9/tests/settings.py` & `django-oscar-pg-search-0.9.0/tests/settings.py`

 * *Files identical despite different names*

