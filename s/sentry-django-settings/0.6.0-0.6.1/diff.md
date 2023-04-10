# Comparing `tmp/sentry_django_settings-0.6.0.tar.gz` & `tmp/sentry_django_settings-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_django_settings-0.6.0.tar", max compression
+gzip compressed data, was "sentry_django_settings-0.6.1.tar", last modified: Mon Apr 10 23:26:45 2023, max compression
```

## Comparing `sentry_django_settings-0.6.0.tar` & `sentry_django_settings-0.6.1.tar`

### file list

```diff
@@ -1,5 +1,20 @@
--rw-r--r--   0        0        0     1487 2022-02-25 21:51:49.124961 sentry_django_settings-0.6.0/LICENSE
--rw-r--r--   0        0        0      423 2023-04-10 22:56:22.589817 sentry_django_settings-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-02-25 21:51:49.125929 sentry_django_settings-0.6.0/sentry_django_settings/__init__.py
--rw-r--r--   0        0        0     2402 2023-04-10 22:23:23.223916 sentry_django_settings-0.6.0/sentry_django_settings/apps.py
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 sentry_django_settings-0.6.0/PKG-INFO
+drwxr-xr-x   0 aaronc     (501) staff       (20)        0 2023-04-10 23:26:45.529610 sentry_django_settings-0.6.1/
+-rw-r--r--   0 aaronc     (501) staff       (20)     1487 2022-02-25 21:51:49.000000 sentry_django_settings-0.6.1/LICENSE
+-rw-r--r--   0 aaronc     (501) staff       (20)       34 2022-02-25 21:51:49.000000 sentry_django_settings-0.6.1/MANIFEST.in
+-rw-r--r--   0 aaronc     (501) staff       (20)     2531 2023-04-10 23:26:45.529192 sentry_django_settings-0.6.1/PKG-INFO
+-rw-r--r--   0 aaronc     (501) staff       (20)     1578 2023-04-10 22:23:23.000000 sentry_django_settings-0.6.1/README.md
+-rw-r--r--   0 aaronc     (501) staff       (20)      423 2023-04-10 23:13:07.000000 sentry_django_settings-0.6.1/pyproject.toml
+drwxr-xr-x   0 aaronc     (501) staff       (20)        0 2023-04-10 23:26:45.523141 sentry_django_settings-0.6.1/sentry_django_settings/
+-rw-r--r--   0 aaronc     (501) staff       (20)        0 2022-02-25 21:51:49.000000 sentry_django_settings-0.6.1/sentry_django_settings/__init__.py
+-rw-r--r--   0 aaronc     (501) staff       (20)     2402 2023-04-10 22:23:23.000000 sentry_django_settings-0.6.1/sentry_django_settings/apps.py
+drwxr-xr-x   0 aaronc     (501) staff       (20)        0 2023-04-10 23:26:45.526408 sentry_django_settings-0.6.1/sentry_django_settings.egg-info/
+-rw-r--r--   0 aaronc     (501) staff       (20)     2531 2023-04-10 23:26:45.000000 sentry_django_settings-0.6.1/sentry_django_settings.egg-info/PKG-INFO
+-rw-r--r--   0 aaronc     (501) staff       (20)      408 2023-04-10 23:26:45.000000 sentry_django_settings-0.6.1/sentry_django_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 aaronc     (501) staff       (20)        1 2023-04-10 23:26:45.000000 sentry_django_settings-0.6.1/sentry_django_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 aaronc     (501) staff       (20)       11 2023-04-10 23:26:45.000000 sentry_django_settings-0.6.1/sentry_django_settings.egg-info/requires.txt
+-rw-r--r--   0 aaronc     (501) staff       (20)       23 2023-04-10 23:26:45.000000 sentry_django_settings-0.6.1/sentry_django_settings.egg-info/top_level.txt
+-rw-r--r--   0 aaronc     (501) staff       (20)       38 2023-04-10 23:26:45.529759 sentry_django_settings-0.6.1/setup.cfg
+-rw-r--r--   0 aaronc     (501) staff       (20)     1387 2023-04-10 23:22:10.000000 sentry_django_settings-0.6.1/setup.py
+drwxr-xr-x   0 aaronc     (501) staff       (20)        0 2023-04-10 23:26:45.528137 sentry_django_settings-0.6.1/tests/
+-rw-r--r--   0 aaronc     (501) staff       (20)     2972 2023-04-10 22:23:23.000000 sentry_django_settings-0.6.1/tests/test_sentry_app.py
+-rw-r--r--   0 aaronc     (501) staff       (20)     3937 2023-04-10 22:56:46.000000 sentry_django_settings-0.6.1/tests/test_sentry_django_config.py
```

### Comparing `sentry_django_settings-0.6.0/LICENSE` & `sentry_django_settings-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_django_settings-0.6.0/sentry_django_settings/apps.py` & `sentry_django_settings-0.6.1/sentry_django_settings/apps.py`

 * *Files identical despite different names*

