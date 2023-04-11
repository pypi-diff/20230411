# Comparing `tmp/django-composite-auto-field-0.1.3-dist.tar.gz` & `tmp/django-composite-auto-field-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-composite-auto-field-0.1.3.tar", last modified: Tue Apr 11 10:34:52 2023, max compression
+gzip compressed data, was "django-composite-auto-field-0.1.4.tar", last modified: Tue Apr 11 10:56:56 2023, max compression
```

## Comparing `django-composite-auto-field-0.1.3-dist.tar` & `django-composite-auto-field-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 10:34:52.415839 django-composite-auto-field-0.1.3/
--rw-rw-rw-   0        0        0     1497 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      170 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4161 2023-04-11 10:34:52.415839 django-composite-auto-field-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2873 2023-04-11 10:34:25.000000 django-composite-auto-field-0.1.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-11 10:34:52.411954 django-composite-auto-field-0.1.3/django_composite_auto_field/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.3/django_composite_auto_field/__init__.py
--rw-rw-rw-   0        0        0     2430 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.3/django_composite_auto_field/fields.py
--rw-rw-rw-   0        0        0       18 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.3/django_composite_auto_field/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:34:52.414837 django-composite-auto-field-0.1.3/django_composite_auto_field.egg-info/
--rw-rw-rw-   0        0        0     4161 2023-04-11 10:34:52.000000 django-composite-auto-field-0.1.3/django_composite_auto_field.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-04-11 10:34:52.000000 django-composite-auto-field-0.1.3/django_composite_auto_field.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 10:34:52.000000 django-composite-auto-field-0.1.3/django_composite_auto_field.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-11 10:34:52.000000 django-composite-auto-field-0.1.3/django_composite_auto_field.egg-info/requires.txt
--rw-rw-rw-   0        0        0       68 2023-04-11 10:34:52.000000 django-composite-auto-field-0.1.3/django_composite_auto_field.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1230 2023-04-11 10:34:52.416354 django-composite-auto-field-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 10:56:56.112321 django-composite-auto-field-0.1.4/
+-rw-rw-rw-   0        0        0     1497 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      170 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4232 2023-04-11 10:56:56.113326 django-composite-auto-field-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2944 2023-04-11 10:56:38.000000 django-composite-auto-field-0.1.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 10:56:56.109832 django-composite-auto-field-0.1.4/django_composite_auto_field/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.4/django_composite_auto_field/__init__.py
+-rw-rw-rw-   0        0        0     2430 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.4/django_composite_auto_field/fields.py
+-rw-rw-rw-   0        0        0       18 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.4/django_composite_auto_field/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-11 10:56:56.112321 django-composite-auto-field-0.1.4/django_composite_auto_field.egg-info/
+-rw-rw-rw-   0        0        0     4232 2023-04-11 10:56:56.000000 django-composite-auto-field-0.1.4/django_composite_auto_field.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2023-04-11 10:56:56.000000 django-composite-auto-field-0.1.4/django_composite_auto_field.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 10:56:56.000000 django-composite-auto-field-0.1.4/django_composite_auto_field.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-11 10:56:56.000000 django-composite-auto-field-0.1.4/django_composite_auto_field.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       68 2023-04-11 10:56:56.000000 django-composite-auto-field-0.1.4/django_composite_auto_field.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1230 2023-04-11 10:56:56.113326 django-composite-auto-field-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.4/setup.py
```

### Comparing `django-composite-auto-field-0.1.3/LICENSE` & `django-composite-auto-field-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-composite-auto-field-0.1.3/PKG-INFO` & `django-composite-auto-field-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-composite-auto-field
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple Django Field for storing auto-incrementing field.
 Home-page: https://github.com/N1K1TAS95/django_composite_auto_field
 Author: Nikita Sinko
 Author-email: n.sinko95@gmail.com
 License: BSD-2-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -96,14 +96,17 @@
     python manage.py migrate
 
     # run tests
     python manage.py test
 
 Release Notes
 -------------
+* 0.1.4
+    - fixed setup
+    - fixed description file (README.rst)
 * 0.1.3
     - added tests
     - added support for custom string as argument
     - added support for Django 4.2 on python 3.8, 3.9, 3.10 and 3.11 - as per the `official django docs <https://docs.djangoproject.com/en/dev/faq/install/#what-python-version-can-i-use-with-django>`_
 * 0.1.2
     - fixed year change
 * 0.1.1 - initial release
```

### Comparing `django-composite-auto-field-0.1.3/README.rst` & `django-composite-auto-field-0.1.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,17 @@
     python manage.py migrate
 
     # run tests
     python manage.py test
 
 Release Notes
 -------------
+* 0.1.4
+    - fixed setup
+    - fixed description file (README.rst)
 * 0.1.3
     - added tests
     - added support for custom string as argument
     - added support for Django 4.2 on python 3.8, 3.9, 3.10 and 3.11 - as per the `official django docs <https://docs.djangoproject.com/en/dev/faq/install/#what-python-version-can-i-use-with-django>`_
 * 0.1.2
     - fixed year change
 * 0.1.1 - initial release
```

### Comparing `django-composite-auto-field-0.1.3/django_composite_auto_field/fields.py` & `django-composite-auto-field-0.1.4/django_composite_auto_field/fields.py`

 * *Files identical despite different names*

### Comparing `django-composite-auto-field-0.1.3/django_composite_auto_field.egg-info/PKG-INFO` & `django-composite-auto-field-0.1.4/django_composite_auto_field.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-composite-auto-field
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple Django Field for storing auto-incrementing field.
 Home-page: https://github.com/N1K1TAS95/django_composite_auto_field
 Author: Nikita Sinko
 Author-email: n.sinko95@gmail.com
 License: BSD-2-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -96,14 +96,17 @@
     python manage.py migrate
 
     # run tests
     python manage.py test
 
 Release Notes
 -------------
+* 0.1.4
+    - fixed setup
+    - fixed description file (README.rst)
 * 0.1.3
     - added tests
     - added support for custom string as argument
     - added support for Django 4.2 on python 3.8, 3.9, 3.10 and 3.11 - as per the `official django docs <https://docs.djangoproject.com/en/dev/faq/install/#what-python-version-can-i-use-with-django>`_
 * 0.1.2
     - fixed year change
 * 0.1.1 - initial release
```

### Comparing `django-composite-auto-field-0.1.3/setup.cfg` & `django-composite-auto-field-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 636f 6d70 6f73   = django-compos
 00000020: 6974 652d 6175 746f 2d66 6965 6c64 0d0a  ite-auto-field..
-00000030: 7665 7273 696f 6e20 3d20 302e 312e 330d  version = 0.1.3.
+00000030: 7665 7273 696f 6e20 3d20 302e 312e 340d  version = 0.1.4.
 00000040: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000050: 2073 696d 706c 6520 446a 616e 676f 2046   simple Django F
 00000060: 6965 6c64 2066 6f72 2073 746f 7269 6e67  ield for storing
 00000070: 2061 7574 6f2d 696e 6372 656d 656e 7469   auto-incrementi
 00000080: 6e67 2066 6965 6c64 2e0d 0a6c 6f6e 675f  ng field...long_
 00000090: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 000000a0: 6c65 3a20 5245 4144 4d45 2e72 7374 0d0a  le: README.rst..
```

