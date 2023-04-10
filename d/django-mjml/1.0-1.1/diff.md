# Comparing `tmp/django-mjml-1.0.tar.gz` & `tmp/django-mjml-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-mjml-1.0.tar", last modified: Thu Oct  6 23:54:23 2022, max compression
+gzip compressed data, was "django-mjml-1.1.tar", last modified: Mon Apr 10 23:25:19 2023, max compression
```

## Comparing `django-mjml-1.0.tar` & `django-mjml-1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 igor      (1000) igor      (1000)        0 2022-10-06 23:54:23.000000 django-mjml-1.0/
-drwxrwxr-x   0 igor      (1000) igor      (1000)        0 2022-10-06 23:54:23.000000 django-mjml-1.0/django_mjml.egg-info/
--rw-rw-r--   0 igor      (1000) igor      (1000)     7695 2022-10-06 23:54:23.000000 django-mjml-1.0/django_mjml.egg-info/PKG-INFO
--rw-rw-r--   0 igor      (1000) igor      (1000)       44 2022-10-06 23:54:23.000000 django-mjml-1.0/django_mjml.egg-info/requires.txt
--rw-rw-r--   0 igor      (1000) igor      (1000)      377 2022-10-06 23:54:23.000000 django-mjml-1.0/django_mjml.egg-info/SOURCES.txt
--rw-rw-r--   0 igor      (1000) igor      (1000)        1 2022-10-06 23:54:23.000000 django-mjml-1.0/django_mjml.egg-info/dependency_links.txt
--rw-rw-r--   0 igor      (1000) igor      (1000)        5 2022-10-06 23:54:23.000000 django-mjml-1.0/django_mjml.egg-info/top_level.txt
--rw-rw-r--   0 igor      (1000) igor      (1000)        1 2022-10-06 23:54:23.000000 django-mjml-1.0/django_mjml.egg-info/not-zip-safe
--rw-rw-r--   0 igor      (1000) igor      (1000)     7695 2022-10-06 23:54:23.000000 django-mjml-1.0/PKG-INFO
--rw-rw-r--   0 igor      (1000) igor      (1000)     3948 2022-10-06 23:42:22.000000 django-mjml-1.0/CHANGELOG.md
--rw-rw-r--   0 igor      (1000) igor      (1000)       56 2022-10-06 23:42:22.000000 django-mjml-1.0/MANIFEST.in
--rw-rw-r--   0 igor      (1000) igor      (1000)     1668 2022-10-06 23:42:22.000000 django-mjml-1.0/setup.py
--rw-rw-r--   0 igor      (1000) igor      (1000)     5059 2022-10-06 23:42:22.000000 django-mjml-1.0/README.rst
-drwxrwxr-x   0 igor      (1000) igor      (1000)        0 2022-10-06 23:54:23.000000 django-mjml-1.0/mjml/
--rw-rw-r--   0 igor      (1000) igor      (1000)       65 2022-10-06 23:42:22.000000 django-mjml-1.0/mjml/__init__.py
-drwxrwxr-x   0 igor      (1000) igor      (1000)        0 2022-10-06 23:54:23.000000 django-mjml-1.0/mjml/templatetags/
--rw-r--r--   0 igor      (1000) igor      (1000)        0 2018-11-02 11:14:43.000000 django-mjml-1.0/mjml/templatetags/__init__.py
--rw-rw-r--   0 igor      (1000) igor      (1000)      822 2022-10-06 23:42:22.000000 django-mjml-1.0/mjml/templatetags/mjml.py
--rw-rw-r--   0 igor      (1000) igor      (1000)     1263 2022-10-06 23:42:22.000000 django-mjml-1.0/mjml/settings.py
--rw-rw-r--   0 igor      (1000) igor      (1000)     5512 2022-10-06 23:42:22.000000 django-mjml-1.0/mjml/tools.py
--rw-rw-r--   0 igor      (1000) igor      (1000)     1194 2022-10-06 23:42:22.000000 django-mjml-1.0/mjml/apps.py
--rw-r--r--   0 igor      (1000) igor      (1000)     1078 2018-11-02 11:14:43.000000 django-mjml-1.0/LICENSE
--rw-rw-r--   0 igor      (1000) igor      (1000)       38 2022-10-06 23:54:23.000000 django-mjml-1.0/setup.cfg
+drwxr-xr-x   0 igor       (501) staff       (20)        0 2023-04-10 23:25:19.368121 django-mjml-1.1/
+-rw-r--r--   0 igor       (501) staff       (20)     4091 2023-04-10 23:22:51.000000 django-mjml-1.1/CHANGELOG.md
+-rw-r--r--   0 igor       (501) staff       (20)     1078 2022-12-21 14:26:08.000000 django-mjml-1.1/LICENSE
+-rw-r--r--   0 igor       (501) staff       (20)       56 2022-12-21 14:26:08.000000 django-mjml-1.1/MANIFEST.in
+-rw-r--r--   0 igor       (501) staff       (20)     4914 2023-04-10 23:25:19.367940 django-mjml-1.1/PKG-INFO
+-rw-r--r--   0 igor       (501) staff       (20)     3698 2023-04-10 23:22:51.000000 django-mjml-1.1/README.rst
+drwxr-xr-x   0 igor       (501) staff       (20)        0 2023-04-10 23:25:19.366620 django-mjml-1.1/django_mjml.egg-info/
+-rw-r--r--   0 igor       (501) staff       (20)     4914 2023-04-10 23:25:19.000000 django-mjml-1.1/django_mjml.egg-info/PKG-INFO
+-rw-r--r--   0 igor       (501) staff       (20)      377 2023-04-10 23:25:19.000000 django-mjml-1.1/django_mjml.egg-info/SOURCES.txt
+-rw-r--r--   0 igor       (501) staff       (20)        1 2023-04-10 23:25:19.000000 django-mjml-1.1/django_mjml.egg-info/dependency_links.txt
+-rw-r--r--   0 igor       (501) staff       (20)        1 2023-04-10 23:25:19.000000 django-mjml-1.1/django_mjml.egg-info/not-zip-safe
+-rw-r--r--   0 igor       (501) staff       (20)       44 2023-04-10 23:25:19.000000 django-mjml-1.1/django_mjml.egg-info/requires.txt
+-rw-r--r--   0 igor       (501) staff       (20)        5 2023-04-10 23:25:19.000000 django-mjml-1.1/django_mjml.egg-info/top_level.txt
+drwxr-xr-x   0 igor       (501) staff       (20)        0 2023-04-10 23:25:19.367356 django-mjml-1.1/mjml/
+-rw-r--r--   0 igor       (501) staff       (20)       65 2023-04-10 23:22:51.000000 django-mjml-1.1/mjml/__init__.py
+-rw-r--r--   0 igor       (501) staff       (20)     1194 2022-12-21 14:26:08.000000 django-mjml-1.1/mjml/apps.py
+-rw-r--r--   0 igor       (501) staff       (20)     1263 2022-12-21 14:26:08.000000 django-mjml-1.1/mjml/settings.py
+drwxr-xr-x   0 igor       (501) staff       (20)        0 2023-04-10 23:25:19.367693 django-mjml-1.1/mjml/templatetags/
+-rw-r--r--   0 igor       (501) staff       (20)        0 2022-12-21 14:26:08.000000 django-mjml-1.1/mjml/templatetags/__init__.py
+-rw-r--r--   0 igor       (501) staff       (20)      822 2022-12-21 14:26:08.000000 django-mjml-1.1/mjml/templatetags/mjml.py
+-rw-r--r--   0 igor       (501) staff       (20)     5512 2022-12-21 14:26:08.000000 django-mjml-1.1/mjml/tools.py
+-rw-r--r--   0 igor       (501) staff       (20)       38 2023-04-10 23:25:19.368184 django-mjml-1.1/setup.cfg
+-rw-r--r--   0 igor       (501) staff       (20)     1718 2023-04-10 23:22:51.000000 django-mjml-1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-mjml-1.0/CHANGELOG.md` & `django-mjml-1.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+1.1 (2023-04-11)
+================
+ * Added Python 3.11 in tests
+ * Added supporting Django 4.2
+ * Added MJML 4.14 in tests
+ * Updated README
+
+
 1.0 (2022-10-07)
 ================
  * Stopped supporting Python 2.7
  * Stopped supporting Django 1.8, 1.9, 1.10, 1.11, 2.0 and 2.1
  * Removed MJML 4.5 from tests
  * Added MJML 4.12 and 4.13 in tests
  * Moved MJML TCP-Server into separated repo https://github.com/danihodovic/mjml-server
```

### Comparing `django-mjml-1.0/setup.py` & `django-mjml-1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     url='https://github.com/liminspace/django-mjml',
     packages=find_packages(exclude=('testprj', 'testprj.*')),
     include_package_data=True,
     zip_safe=False,  # because include static
     platforms=['OS Independent'],
     python_requires='>=3.6',
     install_requires=[
-        'django >=2.2,<4.2',
+        'django >=2.2,<5.0',
     ],
     extras_require={
         'requests': [
             'requests >=2.24',
         ],
     },
     keywords=[
@@ -34,14 +34,15 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Application Frameworks',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Framework :: Django',
         'License :: OSI Approved :: MIT License',
     ],
```

### Comparing `django-mjml-1.0/mjml/templatetags/mjml.py` & `django-mjml-1.1/mjml/templatetags/mjml.py`

 * *Files identical despite different names*

### Comparing `django-mjml-1.0/mjml/settings.py` & `django-mjml-1.1/mjml/settings.py`

 * *Files identical despite different names*

### Comparing `django-mjml-1.0/mjml/tools.py` & `django-mjml-1.1/mjml/tools.py`

 * *Files identical despite different names*

### Comparing `django-mjml-1.0/mjml/apps.py` & `django-mjml-1.1/mjml/apps.py`

 * *Files identical despite different names*

### Comparing `django-mjml-1.0/LICENSE` & `django-mjml-1.1/LICENSE`

 * *Files identical despite different names*

