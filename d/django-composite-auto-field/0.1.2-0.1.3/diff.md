# Comparing `tmp/django-composite-auto-field-0.1.2.tar.gz` & `tmp/django-composite-auto-field-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-composite-auto-field-0.1.2.tar", last modified: Wed Jan  5 08:59:46 2022, max compression
+gzip compressed data, was "django-composite-auto-field-0.1.3.tar", last modified: Tue Apr 11 10:05:39 2023, max compression
```

## Comparing `django-composite-auto-field-0.1.2.tar` & `django-composite-auto-field-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 nik        (501) staff       (20)        0 2022-01-05 08:59:46.010982 django-composite-auto-field-0.1.2/
--rw-r--r--   0 nik        (501) staff       (20)     1486 2021-10-14 20:10:12.000000 django-composite-auto-field-0.1.2/LICENSE
--rw-r--r--   0 nik        (501) staff       (20)      165 2021-10-14 19:59:46.000000 django-composite-auto-field-0.1.2/MANIFEST.in
--rw-r--r--   0 nik        (501) staff       (20)     3156 2022-01-05 08:59:46.011047 django-composite-auto-field-0.1.2/PKG-INFO
--rw-r--r--   0 nik        (501) staff       (20)     2100 2021-10-16 10:40:21.000000 django-composite-auto-field-0.1.2/README.rst
-drwxr-xr-x   0 nik        (501) staff       (20)        0 2022-01-05 08:59:46.010166 django-composite-auto-field-0.1.2/django_composite_auto_field/
--rw-r--r--   0 nik        (501) staff       (20)        0 2021-10-09 14:21:39.000000 django-composite-auto-field-0.1.2/django_composite_auto_field/__init__.py
--rw-r--r--   0 nik        (501) staff       (20)     2688 2022-01-05 08:52:48.000000 django-composite-auto-field-0.1.2/django_composite_auto_field/fields.py
-drwxr-xr-x   0 nik        (501) staff       (20)        0 2022-01-05 08:59:46.010888 django-composite-auto-field-0.1.2/django_composite_auto_field.egg-info/
--rw-r--r--   0 nik        (501) staff       (20)     3156 2022-01-05 08:59:46.000000 django-composite-auto-field-0.1.2/django_composite_auto_field.egg-info/PKG-INFO
--rw-r--r--   0 nik        (501) staff       (20)      381 2022-01-05 08:59:46.000000 django-composite-auto-field-0.1.2/django_composite_auto_field.egg-info/SOURCES.txt
--rw-r--r--   0 nik        (501) staff       (20)        1 2022-01-05 08:59:46.000000 django-composite-auto-field-0.1.2/django_composite_auto_field.egg-info/dependency_links.txt
--rw-r--r--   0 nik        (501) staff       (20)       12 2022-01-05 08:59:46.000000 django-composite-auto-field-0.1.2/django_composite_auto_field.egg-info/requires.txt
--rw-r--r--   0 nik        (501) staff       (20)       68 2022-01-05 08:59:46.000000 django-composite-auto-field-0.1.2/django_composite_auto_field.egg-info/top_level.txt
--rw-r--r--   0 nik        (501) staff       (20)     1024 2022-01-05 08:59:46.011289 django-composite-auto-field-0.1.2/setup.cfg
--rw-r--r--   0 nik        (501) staff       (20)       38 2021-10-14 19:17:59.000000 django-composite-auto-field-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 10:05:39.578329 django-composite-auto-field-0.1.3/
+-rw-rw-rw-   0        0        0     1497 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      170 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4108 2023-04-11 10:05:39.578329 django-composite-auto-field-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2820 2023-04-11 10:01:38.000000 django-composite-auto-field-0.1.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 10:05:39.575330 django-composite-auto-field-0.1.3/django_composite_auto_field/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.3/django_composite_auto_field/__init__.py
+-rw-rw-rw-   0        0        0     2430 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.3/django_composite_auto_field/fields.py
+-rw-rw-rw-   0        0        0       18 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.3/django_composite_auto_field/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-11 10:05:39.578329 django-composite-auto-field-0.1.3/django_composite_auto_field.egg-info/
+-rw-rw-rw-   0        0        0     4108 2023-04-11 10:05:39.000000 django-composite-auto-field-0.1.3/django_composite_auto_field.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2023-04-11 10:05:39.000000 django-composite-auto-field-0.1.3/django_composite_auto_field.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 10:05:39.000000 django-composite-auto-field-0.1.3/django_composite_auto_field.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-11 10:05:39.000000 django-composite-auto-field-0.1.3/django_composite_auto_field.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       68 2023-04-11 10:05:39.000000 django-composite-auto-field-0.1.3/django_composite_auto_field.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1230 2023-04-11 10:05:39.579328 django-composite-auto-field-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-04-11 07:32:19.000000 django-composite-auto-field-0.1.3/setup.py
```

### Comparing `django-composite-auto-field-0.1.2/LICENSE` & `django-composite-auto-field-0.1.3/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-Copyright (c) 2017, Nikita Sinko
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
-
-* Neither the name of django-composite-auto-field nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
-
+Copyright (c) 2017, Nikita Sinko
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+* Neither the name of django-composite-auto-field nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `django-composite-auto-field-0.1.2/PKG-INFO` & `django-composite-auto-field-0.1.3/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,81 @@
-Metadata-Version: 2.1
-Name: django-composite-auto-field
-Version: 0.1.2
-Summary: A simple Django Field for storing auto-incrementing field.
-Home-page: https://github.com/N1K1TAS95/django_composite_auto_field
-Author: Nikita Sinko
-Author-email: n.sinko95@gmail.com
-License: BSD-2-Clause
-Platform: UNKNOWN
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.1
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.6
-License-File: LICENSE
-
-=============================
-django-composite-auto-field
-=============================
-
-.. contents:: A simple Django Field for storing auto-incrementing field. It's useful for storing such as orders code for much easier reading.
-
-----
-
-Installation
-------------
-Install django-composite-auto-field::
-
-    pip install django-composite-auto-field
-
-Usage
------
-This field uses Django's Aggregate and Max functions to extract the latest code from the database and does a minimum of parsing to calculate the next code. This avoids having to store a counter in the database. Therefore, for correct operation, once the field arguments have been set, it is advisable not to modify them anymore, or to manually act on the codes already calculated and stored in the database.
-
-Import to your models::
-
-    from django_composite_auto_field.fields import CompositeAutoField
-
-Usage::
-
-    class Order(models.Model):
-        code = CompositeAutoField(prefix='ORD', use_year=True, zeros=5)
-
-Arguments::
-
-    prefix      # It's used to indicate prefix for the code
-    use_year    # When it's True, last two numbers of current year will be used after prefix
-    zero        # Indicated number of zeros before the number
-
-Run::
-
-    python manage.py makemigrations
-    python manage.py migrate
-
-For example. Using Arguments from above as shown, will result in codes::
-
-    ORD2100001
-    ORD2100002
-    ORD2100003
-    ...
-
-If the year is used, every year the counter will be automatically reset and the count will restart with 1.
-
-Release Notes
--------------
-* 0.1.1 - initial release
-    - provides CompositeAutoField for storing auto-incrementing field
-    - supports Django 3.1 on python 3.6, 3.7, 3.8 and 3.9 - as per the `official django docs <https://docs.djangoproject.com/en/dev/faq/install/#what-python-version-can-i-use-with-django>`_
-
-Todo
-----
-    - ❌ Create test cases
-    - ✔️ Initial release on GitHub
-    - ✔️ Initial release on PyPi
-    - ❌ Improve last code parsing for make arguments changeable
-
-Contributing
-------------
-It's an open source project, so any contributions are welcome!
-
+=============================
+django-composite-auto-field
+=============================
+
+.. contents:: A simple Django Field for storing auto-incrementing field. It's useful for storing such as orders code for much easier reading.
+
+----
+
+Installation
+------------
+Install django-composite-auto-field::
+
+    pip install django-composite-auto-field
+
+Usage
+-----
+This field uses Django's Aggregate and Max functions to extract the latest code from the database and does a minimum of parsing to calculate the next code. This avoids having to store a counter in the database. Therefore, for correct operation, once the field arguments have been set, it is advisable not to modify them anymore, or to manually act on the codes already calculated and stored in the database.
+
+Import to your models::
+
+    from django_composite_auto_field.fields import CompositeAutoField
+
+Usage::
+
+    class Order(models.Model):
+        code = CompositeAutoField(prefix='ORD', use_year=True, zeros=5)
+
+Arguments::
+
+    prefix      # It's used to indicate prefix for the code, default is "CC"
+    use_year    # When it's True, last two numbers of current year will be used after prefix
+    zero        # Indicated number of zeros before the number
+
+Run::
+
+    python manage.py makemigrations
+    python manage.py migrate
+
+For example. Using Arguments from above as shown, will result in codes::
+
+    ORD2100001
+    ORD2100002
+    ORD2100003
+    ...
+
+If the year is used, every year the counter will be automatically reset and the count will restart with 1.
+If you pass a string to the field, it will be used instead of the generated value. Pay attention to the passed values, they will be used for the generation of subsequent values.
+
+Tests
+-------------
+To run tests::
+
+    # clone this repository on your PC
+
+    # create the virtual environment
+    python -m venv venv
+
+    # activate the virtual environment
+    source venv\bin\activate
+
+    # installa requirements
+    pip install -r .\requirements.txt
+
+    # run tests
+    python manage.py test
+
+Release Notes
+-------------
+* 0.1.3
+    - added tests
+    - added support for custom string as argument
+    - added support for Django 4.2 on python 3.8, 3.9, 3.10 and 3.11 - as per the `official django docs <https://docs.djangoproject.com/en/dev/faq/install/#what-python-version-can-i-use-with-django>`_
+* 0.1.2
+    - fixed year change
+* 0.1.1 - initial release
+    - provides CompositeAutoField for storing auto-incrementing field
+    - supports Django 3.1 on python 3.6, 3.7, 3.8 and 3.9 - as per the `official django docs <https://docs.djangoproject.com/en/dev/faq/install/#what-python-version-can-i-use-with-django>`_
+
+Contributing
+------------
+It's an open source project, so any contributions are welcome!
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-composite-auto-field-0.1.2/django_composite_auto_field/fields.py` & `django-composite-auto-field-0.1.3/django_composite_auto_field/fields.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,58 @@
-import warnings
-
-from django.db import models
-from django.db.models import Max
-from django.utils.timezone import now
-from django.utils.translation import gettext_lazy as _
-
-
-class CompositeAutoField(models.CharField):
-    warning = ("You passed an argument to CodeField that will be "
-               "ignored. Avoid args and following kwargs: max_length, unique, editable, null.")
-    description = _('custom auto incrementing field')
-    defaults = dict(max_length=255, unique=True, editable=False, null=True)
-
-    def __init__(self, *args, db_collation=None, prefix='CC', use_year=False, zeros=4, **kwargs):
-        self.prefix = prefix
-        self.use_year = use_year
-        self.zeros = zeros
-        self._warn_for_shadowing_args(*args, **kwargs)
-        kwargs['max_length'] = 255
-        kwargs['unique'] = True
-        kwargs['editable'] = False
-        kwargs['null'] = True
-        kwargs.update(self.defaults)
-        super().__init__(*args, db_collation=db_collation, **kwargs)
-
-    def deconstruct(self):
-        name, path, args, kwargs = super(CompositeAutoField, self).deconstruct()
-        if self.prefix != 'CC':
-            kwargs['prefix'] = self.prefix
-        kwargs['use_year'] = self.use_year
-        if self.zeros != 4:
-            kwargs['zeros'] = self.zeros
-        del kwargs['max_length']
-        del kwargs['unique']
-        del kwargs['editable']
-        del kwargs['null']
-        return name, path, args, kwargs
-
-    def pre_save(self, model_instance, add):
-        if self.prefix and self.zeros and add:
-            max_res = self.model.objects.aggregate(**{self.name + '_max': Max(self.name)})[self.name + '_max']
-            next_num = 1
-            cur_year = str(now().year)[2:]
-            if max_res:
-                if self.use_year:
-                    last_year = int(max_res[len(self.prefix):4])
-                    if last_year == int(cur_year):
-                        next_num = int(max_res[len(self.prefix) + 2:]) + 1
-                else:
-                    next_num = int(max_res[len(self.prefix):]) + 1
-            next_num = str(next_num).zfill(self.zeros)
-            value = f'{self.prefix}{cur_year if self.use_year else str()}{next_num}'
-            setattr(model_instance, self.attname, value)
-            return value
-        else:
-            return super().pre_save(model_instance, add)
-
-    def _warn_for_shadowing_args(self, *args, **kwargs):
-        if args:
-            warnings.warn(self.warning)
-        else:
-            for key in set(kwargs).intersection(set(self.defaults.keys())):
-                if not kwargs[key] == self.defaults[key]:
-                    warnings.warn(self.warning)
-                    break
+import warnings
+
+from django.db import models
+from django.db.models import Max
+from django.utils.timezone import now
+from django.utils.translation import gettext_lazy as _
+
+
+class CompositeAutoField(models.CharField):
+    warning = ("You passed an argument to CodeField that will be "
+               "ignored. Avoid args and following kwargs: max_length.")
+    description = _('Custom auto incrementing field')
+    defaults = dict(max_length=250)
+
+    def __init__(self, *args, db_collation=None, prefix='CC', use_year=False, zeros=4, **kwargs):
+        self.prefix = prefix
+        self.use_year = use_year
+        self.zeros = zeros
+        self._warn_for_shadowing_args(*args, **kwargs)
+        kwargs.update(self.defaults)
+        super().__init__(*args, db_collation=db_collation, **kwargs)
+
+    def deconstruct(self):
+        name, path, args, kwargs = super(CompositeAutoField, self).deconstruct()
+        if self.prefix != 'CC':
+            kwargs['prefix'] = self.prefix
+        kwargs['use_year'] = self.use_year
+        if self.zeros != 4:
+            kwargs['zeros'] = self.zeros
+        return name, path, args, kwargs
+
+    def pre_save(self, model_instance, add):
+        if self.prefix and self.zeros and add:
+            max_res = self.model.objects.aggregate(**{self.name + '_max': Max(self.name)})[self.name + '_max']
+            next_num = 1
+            cur_year = str(now().year)[2:]
+            if max_res:
+                if self.use_year:
+                    last_year = int(max_res[len(self.prefix):4])
+                    if last_year == int(cur_year):
+                        next_num = int(max_res[len(self.prefix) + 2:]) + 1
+                else:
+                    next_num = int(max_res[len(self.prefix):]) + 1
+            next_num = str(next_num).zfill(self.zeros)
+            value = f'{self.prefix}{cur_year if self.use_year else str()}{next_num}'
+            setattr(model_instance, self.attname, value)
+            return value
+        else:
+            return super().pre_save(model_instance, add)
+
+    def _warn_for_shadowing_args(self, *args, **kwargs):
+        if args:
+            warnings.warn(self.warning)
+        else:
+            for key in set(kwargs).intersection(set(self.defaults.keys())):
+                if not kwargs[key] == self.defaults[key]:
+                    warnings.warn(self.warning)
+                    break
```

### Comparing `django-composite-auto-field-0.1.2/setup.cfg` & `django-composite-auto-field-0.1.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,77 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 646a 616e 676f 2d63 6f6d 706f 7369  = django-composi
-00000020: 7465 2d61 7574 6f2d 6669 656c 640a 7665  te-auto-field.ve
-00000030: 7273 696f 6e20 3d20 302e 312e 320a 6465  rsion = 0.1.2.de
-00000040: 7363 7269 7074 696f 6e20 3d20 4120 7369  scription = A si
-00000050: 6d70 6c65 2044 6a61 6e67 6f20 4669 656c  mple Django Fiel
-00000060: 6420 666f 7220 7374 6f72 696e 6720 6175  d for storing au
-00000070: 746f 2d69 6e63 7265 6d65 6e74 696e 6720  to-incrementing 
-00000080: 6669 656c 642e 0a6c 6f6e 675f 6465 7363  field..long_desc
-00000090: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
-000000a0: 5245 4144 4d45 2e72 7374 0a75 726c 203d  README.rst.url =
-000000b0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000000c0: 636f 6d2f 4e31 4b31 5441 5339 352f 646a  com/N1K1TAS95/dj
-000000d0: 616e 676f 5f63 6f6d 706f 7369 7465 5f61  ango_composite_a
-000000e0: 7574 6f5f 6669 656c 640a 6175 7468 6f72  uto_field.author
-000000f0: 203d 204e 696b 6974 6120 5369 6e6b 6f0a   = Nikita Sinko.
-00000100: 6175 7468 6f72 5f65 6d61 696c 203d 206e  author_email = n
-00000110: 2e73 696e 6b6f 3935 4067 6d61 696c 2e63  .sinko95@gmail.c
-00000120: 6f6d 0a6c 6963 656e 7365 203d 2042 5344  om.license = BSD
-00000130: 2d32 2d43 6c61 7573 650a 636c 6173 7369  -2-Clause.classi
-00000140: 6669 6572 7320 3d20 0a09 456e 7669 726f  fiers = ..Enviro
-00000150: 6e6d 656e 7420 3a3a 2057 6562 2045 6e76  nment :: Web Env
-00000160: 6972 6f6e 6d65 6e74 0a09 4672 616d 6577  ironment..Framew
-00000170: 6f72 6b20 3a3a 2044 6a61 6e67 6f0a 0946  ork :: Django..F
-00000180: 7261 6d65 776f 726b 203a 3a20 446a 616e  ramework :: Djan
-00000190: 676f 203a 3a20 332e 310a 0949 6e74 656e  go :: 3.1..Inten
-000001a0: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-000001b0: 4465 7665 6c6f 7065 7273 0a09 4c69 6365  Developers..Lice
-000001c0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-000001d0: 7665 6420 3a3a 2042 5344 204c 6963 656e  ved :: BSD Licen
-000001e0: 7365 0a09 4f70 6572 6174 696e 6720 5379  se..Operating Sy
-000001f0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-00000200: 656e 6465 6e74 0a09 5072 6f67 7261 6d6d  endent..Programm
-00000210: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000220: 5079 7468 6f6e 0a09 5072 6f67 7261 6d6d  Python..Programm
-00000230: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000240: 5079 7468 6f6e 203a 3a20 330a 0950 726f  Python :: 3..Pro
-00000250: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000260: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000270: 203a 3a20 4f6e 6c79 0a09 5072 6f67 7261   :: Only..Progra
-00000280: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000290: 3a20 5079 7468 6f6e 203a 3a20 332e 360a  : Python :: 3.6.
-000002a0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000002b0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002c0: 3a3a 2033 2e37 0a09 5072 6f67 7261 6d6d  :: 3.7..Programm
-000002d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000002e0: 5079 7468 6f6e 203a 3a20 332e 380a 0950  Python :: 3.8..P
-000002f0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000300: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000310: 2033 2e39 0a09 546f 7069 6320 3a3a 2049   3.9..Topic :: I
-00000320: 6e74 6572 6e65 7420 3a3a 2057 5757 2f48  nternet :: WWW/H
-00000330: 5454 500a 0954 6f70 6963 203a 3a20 496e  TTP..Topic :: In
-00000340: 7465 726e 6574 203a 3a20 5757 572f 4854  ternet :: WWW/HT
-00000350: 5450 203a 3a20 4479 6e61 6d69 6320 436f  TP :: Dynamic Co
-00000360: 6e74 656e 740a 0a5b 6f70 7469 6f6e 735d  ntent..[options]
-00000370: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
-00000380: 5f64 6174 6120 3d20 7472 7565 0a70 6163  _data = true.pac
-00000390: 6b61 6765 7320 3d20 6669 6e64 3a0a 7079  kages = find:.py
-000003a0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-000003b0: 3e3d 332e 360a 696e 7374 616c 6c5f 7265  >=3.6.install_re
-000003c0: 7175 6972 6573 203d 200a 0944 6a61 6e67  quires = ..Djang
-000003d0: 6f20 3e3d 2033 2e31 0a0a 5b65 6767 5f69  o >= 3.1..[egg_i
-000003e0: 6e66 6f5d 0a74 6167 5f62 7569 6c64 203d  nfo].tag_build =
-000003f0: 200a 7461 675f 6461 7465 203d 2030 0a0a   .tag_date = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2064 6a61 6e67 6f2d 636f 6d70 6f73   = django-compos
+00000020: 6974 652d 6175 746f 2d66 6965 6c64 0d0a  ite-auto-field..
+00000030: 7665 7273 696f 6e20 3d20 302e 312e 330d  version = 0.1.3.
+00000040: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
+00000050: 2073 696d 706c 6520 446a 616e 676f 2046   simple Django F
+00000060: 6965 6c64 2066 6f72 2073 746f 7269 6e67  ield for storing
+00000070: 2061 7574 6f2d 696e 6372 656d 656e 7469   auto-incrementi
+00000080: 6e67 2066 6965 6c64 2e0d 0a6c 6f6e 675f  ng field...long_
+00000090: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+000000a0: 6c65 3a20 5245 4144 4d45 2e72 7374 0d0a  le: README.rst..
+000000b0: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
+000000c0: 7468 7562 2e63 6f6d 2f4e 314b 3154 4153  thub.com/N1K1TAS
+000000d0: 3935 2f64 6a61 6e67 6f5f 636f 6d70 6f73  95/django_compos
+000000e0: 6974 655f 6175 746f 5f66 6965 6c64 0d0a  ite_auto_field..
+000000f0: 6175 7468 6f72 203d 204e 696b 6974 6120  author = Nikita 
+00000100: 5369 6e6b 6f0d 0a61 7574 686f 725f 656d  Sinko..author_em
+00000110: 6169 6c20 3d20 6e2e 7369 6e6b 6f39 3540  ail = n.sinko95@
+00000120: 676d 6169 6c2e 636f 6d0d 0a6c 6963 656e  gmail.com..licen
+00000130: 7365 203d 2042 5344 2d32 2d43 6c61 7573  se = BSD-2-Claus
+00000140: 650d 0a63 6c61 7373 6966 6965 7273 203d  e..classifiers =
+00000150: 200d 0a09 456e 7669 726f 6e6d 656e 7420   ...Environment 
+00000160: 3a3a 2057 6562 2045 6e76 6972 6f6e 6d65  :: Web Environme
+00000170: 6e74 0d0a 0946 7261 6d65 776f 726b 203a  nt...Framework :
+00000180: 3a20 446a 616e 676f 0d0a 0946 7261 6d65  : Django...Frame
+00000190: 776f 726b 203a 3a20 446a 616e 676f 203a  work :: Django :
+000001a0: 3a20 332e 320d 0a09 4672 616d 6577 6f72  : 3.2...Framewor
+000001b0: 6b20 3a3a 2044 6a61 6e67 6f20 3a3a 2034  k :: Django :: 4
+000001c0: 2e30 0d0a 0946 7261 6d65 776f 726b 203a  .0...Framework :
+000001d0: 3a20 446a 616e 676f 203a 3a20 342e 310d  : Django :: 4.1.
+000001e0: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
+000001f0: 6a61 6e67 6f20 3a3a 2034 2e32 0d0a 0949  jango :: 4.2...I
+00000200: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+00000210: 203a 3a20 4465 7665 6c6f 7065 7273 0d0a   :: Developers..
+00000220: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
+00000230: 4170 7072 6f76 6564 203a 3a20 4253 4420  Approved :: BSD 
+00000240: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
+00000250: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+00000260: 2049 6e64 6570 656e 6465 6e74 0d0a 0950   Independent...P
+00000270: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000280: 6167 6520 3a3a 2050 7974 686f 6e0d 0a09  age :: Python...
+00000290: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000002a0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000002b0: 3a20 330d 0a09 5072 6f67 7261 6d6d 696e  : 3...Programmin
+000002c0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000002d0: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
+000002e0: 790d 0a09 5072 6f67 7261 6d6d 696e 6720  y...Programming 
+000002f0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000300: 6f6e 203a 3a20 332e 360d 0a09 5072 6f67  on :: 3.6...Prog
+00000310: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000320: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000330: 370d 0a09 5072 6f67 7261 6d6d 696e 6720  7...Programming 
+00000340: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000350: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
+00000360: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000370: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000380: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
+00000390: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000003a0: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
+000003b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000003c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000003d0: 2e31 310d 0a09 546f 7069 6320 3a3a 2049  .11...Topic :: I
+000003e0: 6e74 6572 6e65 7420 3a3a 2057 5757 2f48  nternet :: WWW/H
+000003f0: 5454 500d 0a09 546f 7069 6320 3a3a 2049  TTP...Topic :: I
+00000400: 6e74 6572 6e65 7420 3a3a 2057 5757 2f48  nternet :: WWW/H
+00000410: 5454 5020 3a3a 2044 796e 616d 6963 2043  TTP :: Dynamic C
+00000420: 6f6e 7465 6e74 0d0a 0d0a 5b6f 7074 696f  ontent....[optio
+00000430: 6e73 5d0d 0a69 6e63 6c75 6465 5f70 6163  ns]..include_pac
+00000440: 6b61 6765 5f64 6174 6120 3d20 7472 7565  kage_data = true
+00000450: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
+00000460: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
+00000470: 7265 7320 3d20 3e3d 332e 360d 0a69 6e73  res = >=3.6..ins
+00000480: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
+00000490: 0d0a 0944 6a61 6e67 6f20 3e3d 2033 2e32  ...Django >= 3.2
+000004a0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+000004b0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+000004c0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

