# Comparing `tmp/admin-form-image-preivew-1.1.tar.gz` & `tmp/admin-form-image-preivew-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admin-form-image-preivew-1.1.tar", last modified: Tue Apr 11 06:48:48 2023, max compression
+gzip compressed data, was "admin-form-image-preivew-1.2.tar", last modified: Tue Apr 11 11:19:42 2023, max compression
```

## Comparing `admin-form-image-preivew-1.1.tar` & `admin-form-image-preivew-1.2.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.357658 admin-form-image-preivew-1.1/
--rw-rw-r--   0 sami      (1000) sami      (1000)      419 2023-04-11 05:45:07.000000 admin-form-image-preivew-1.1/.gitignore
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.1/CHANGES.rst
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.1/LICENSE.txt
--rw-rw-r--   0 sami      (1000) sami      (1000)     1521 2023-04-11 06:48:48.357658 admin-form-image-preivew-1.1/PKG-INFO
--rw-rw-r--   0 sami      (1000) sami      (1000)      724 2023-04-11 04:50:21.000000 admin-form-image-preivew-1.1/README.md
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.337658 admin-form-image-preivew-1.1/admin_form_image_preivew/
--rw-rw-r--   0 sami      (1000) sami      (1000)       22 2023-04-01 14:28:33.000000 admin-form-image-preivew-1.1/admin_form_image_preivew/__init__.py
--rw-rw-r--   0 sami      (1000) sami      (1000)     3845 2023-04-08 06:36:12.000000 admin-form-image-preivew-1.1/admin_form_image_preivew/settings.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      185 2023-04-01 14:28:25.000000 admin-form-image-preivew-1.1/admin_form_image_preivew/wsgi.py
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.337658 admin-form-image-preivew-1.1/admin_form_image_preivew.egg-info/
--rw-rw-r--   0 sami      (1000) sami      (1000)     1521 2023-04-11 06:48:48.000000 admin-form-image-preivew-1.1/admin_form_image_preivew.egg-info/PKG-INFO
--rw-rw-r--   0 sami      (1000) sami      (1000)     1541 2023-04-11 06:48:48.000000 admin-form-image-preivew-1.1/admin_form_image_preivew.egg-info/SOURCES.txt
--rw-rw-r--   0 sami      (1000) sami      (1000)        1 2023-04-11 06:48:48.000000 admin-form-image-preivew-1.1/admin_form_image_preivew.egg-info/dependency_links.txt
--rw-rw-r--   0 sami      (1000) sami      (1000)      159 2023-04-11 06:48:48.000000 admin-form-image-preivew-1.1/admin_form_image_preivew.egg-info/requires.txt
--rw-rw-r--   0 sami      (1000) sami      (1000)       20 2023-04-11 06:48:48.000000 admin-form-image-preivew-1.1/admin_form_image_preivew.egg-info/top_level.txt
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.337658 admin-form-image-preivew-1.1/admin_image_preview/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-04 08:52:37.000000 admin-form-image-preivew-1.1/admin_image_preview/__init__.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      168 2023-04-08 06:26:54.000000 admin-form-image-preivew-1.1/admin_image_preview/apps.py
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.341658 admin-form-image-preivew-1.1/admin_image_preview/migrations/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-04 08:52:37.000000 admin-form-image-preivew-1.1/admin_image_preview/migrations/__init__.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      293 2023-04-07 14:30:35.000000 admin-form-image-preivew-1.1/admin_image_preview/models.py
--rw-rw-r--   0 sami      (1000) sami      (1000)     1767 2023-04-10 12:09:04.000000 admin-form-image-preivew-1.1/admin_image_preview/readme.md
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.325658 admin-form-image-preivew-1.1/admin_image_preview/static/
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.341658 admin-form-image-preivew-1.1/admin_image_preview/static/admin_image_preview/
--rw-rw-r--   0 sami      (1000) sami      (1000)     3872 2023-04-11 04:52:02.000000 admin-form-image-preivew-1.1/admin_image_preview/static/admin_image_preview/image_preview.js
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.329658 admin-form-image-preivew-1.1/admin_image_preview/templates/
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.341658 admin-form-image-preivew-1.1/admin_image_preview/templates/admin/
--rw-rw-r--   0 sami      (1000) sami      (1000)      213 2023-04-10 12:05:52.000000 admin-form-image-preivew-1.1/admin_image_preview/templates/admin/change_form.html
--rw-rw-r--   0 sami      (1000) sami      (1000)     3804 2023-04-10 08:30:05.000000 admin-form-image-preivew-1.1/admin_image_preview/templates/admin/original_change_form.html
--rw-rw-r--   0 sami      (1000) sami      (1000)     1113 2023-04-08 07:03:57.000000 admin-form-image-preivew-1.1/del.py
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.341658 admin-form-image-preivew-1.1/docs/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.1/docs/index.rst
--rw-rw-r--   0 sami      (1000) sami      (1000)     1025 2023-04-11 06:48:44.000000 admin-form-image-preivew-1.1/docs/make_pip.md
--rw-rw-r--   0 sami      (1000) sami      (1000)     1096 2023-04-10 12:10:33.000000 admin-form-image-preivew-1.1/pyproject.toml
--rw-rw-r--   0 sami      (1000) sami      (1000)       74 2023-04-11 06:04:33.000000 admin-form-image-preivew-1.1/requirements.txt
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.345658 admin-form-image-preivew-1.1/sample_usage/
--rw-r--r--   0 sami      (1000) sami      (1000)    90636 2023-04-01 08:16:18.000000 admin-form-image-preivew-1.1/sample_usage/92news-logo.png
--rw-rw-r--   0 sami      (1000) sami      (1000)     1121 2023-04-10 07:55:08.000000 admin-form-image-preivew-1.1/sample_usage/del.py
--rw-rw-r--   0 sami      (1000) sami      (1000)     1413 2023-04-10 12:20:30.000000 admin-form-image-preivew-1.1/sample_usage/fixtures.json
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.329658 admin-form-image-preivew-1.1/sample_usage/initsql/
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.345658 admin-form-image-preivew-1.1/sample_usage/initsql/fixtures/
--rw-rw-r--   0 sami      (1000) sami      (1000)     1165 2023-04-10 12:21:32.000000 admin-form-image-preivew-1.1/sample_usage/initsql/fixtures/auth.json
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.329658 admin-form-image-preivew-1.1/sample_usage/initsql/management/
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.349658 admin-form-image-preivew-1.1/sample_usage/initsql/management/commands/
--rwxrwxr-x   0 sami      (1000) sami      (1000)     1791 2023-04-10 08:05:37.000000 admin-form-image-preivew-1.1/sample_usage/initsql/management/commands/initsql.py
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.349658 admin-form-image-preivew-1.1/sample_usage/main_app/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 11:55:49.000000 admin-form-image-preivew-1.1/sample_usage/main_app/__init__.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      169 2023-04-08 06:24:35.000000 admin-form-image-preivew-1.1/sample_usage/main_app/asgi.py
--rw-rw-r--   0 sami      (1000) sami      (1000)     3453 2023-04-10 12:18:16.000000 admin-form-image-preivew-1.1/sample_usage/main_app/settings.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      814 2023-04-10 12:02:30.000000 admin-form-image-preivew-1.1/sample_usage/main_app/urls.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      169 2023-04-08 06:25:37.000000 admin-form-image-preivew-1.1/sample_usage/main_app/wsgi.py
--rwxrwxr-x   0 sami      (1000) sami      (1000)      664 2023-04-08 06:24:26.000000 admin-form-image-preivew-1.1/sample_usage/manage.py
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.353658 admin-form-image-preivew-1.1/sample_usage/media/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-03 15:01:56.000000 admin-form-image-preivew-1.1/sample_usage/media/init.txt
--rw-rw-r--   0 sami      (1000) sami      (1000)       56 2023-04-11 06:04:53.000000 admin-form-image-preivew-1.1/sample_usage/requirements.txt
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.353658 admin-form-image-preivew-1.1/sample_usage/sample_app/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-01 14:38:44.000000 admin-form-image-preivew-1.1/sample_usage/sample_app/__init__.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      118 2023-04-01 08:12:10.000000 admin-form-image-preivew-1.1/sample_usage/sample_app/admin.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      151 2023-04-08 06:33:58.000000 admin-form-image-preivew-1.1/sample_usage/sample_app/apps.py
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.357658 admin-form-image-preivew-1.1/sample_usage/sample_app/migrations/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-01 08:06:44.000000 admin-form-image-preivew-1.1/sample_usage/sample_app/migrations/__init__.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      194 2023-04-01 08:46:06.000000 admin-form-image-preivew-1.1/sample_usage/sample_app/models.py
--rw-rw-r--   0 sami      (1000) sami      (1000)       60 2023-04-01 08:06:44.000000 admin-form-image-preivew-1.1/sample_usage/sample_app/tests.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      191 2023-04-01 08:08:31.000000 admin-form-image-preivew-1.1/sample_usage/sample_app/urls.py
--rw-rw-r--   0 sami      (1000) sami      (1000)       63 2023-04-01 08:06:44.000000 admin-form-image-preivew-1.1/sample_usage/sample_app/views.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      144 2023-04-11 06:48:48.357658 admin-form-image-preivew-1.1/setup.cfg
--rwxrwxr-x   0 sami      (1000) sami      (1000)     1852 2023-04-11 06:00:12.000000 admin-form-image-preivew-1.1/setup.py
-drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 06:48:48.357658 admin-form-image-preivew-1.1/test/
--rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.1/test/__init__.py
--rw-rw-r--   0 sami      (1000) sami      (1000)      118 2023-04-10 12:08:38.000000 admin-form-image-preivew-1.1/towncrier.toml
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.460836 admin-form-image-preivew-1.2/
+-rw-rw-r--   0 sami      (1000) sami      (1000)      419 2023-04-11 05:45:07.000000 admin-form-image-preivew-1.2/.gitignore
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.2/CHANGES.rst
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.2/LICENSE.txt
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1852 2023-04-11 11:19:42.460836 admin-form-image-preivew-1.2/PKG-INFO
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1055 2023-04-11 08:11:29.000000 admin-form-image-preivew-1.2/README.md
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.440836 admin-form-image-preivew-1.2/admin_form_image_preivew/
+-rw-rw-r--   0 sami      (1000) sami      (1000)       22 2023-04-01 14:28:33.000000 admin-form-image-preivew-1.2/admin_form_image_preivew/__init__.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)     3845 2023-04-08 06:36:12.000000 admin-form-image-preivew-1.2/admin_form_image_preivew/settings.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      185 2023-04-01 14:28:25.000000 admin-form-image-preivew-1.2/admin_form_image_preivew/wsgi.py
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.440836 admin-form-image-preivew-1.2/admin_form_image_preivew.egg-info/
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1852 2023-04-11 11:19:42.000000 admin-form-image-preivew-1.2/admin_form_image_preivew.egg-info/PKG-INFO
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1564 2023-04-11 11:19:42.000000 admin-form-image-preivew-1.2/admin_form_image_preivew.egg-info/SOURCES.txt
+-rw-rw-r--   0 sami      (1000) sami      (1000)        1 2023-04-11 11:19:42.000000 admin-form-image-preivew-1.2/admin_form_image_preivew.egg-info/dependency_links.txt
+-rw-rw-r--   0 sami      (1000) sami      (1000)      159 2023-04-11 11:19:42.000000 admin-form-image-preivew-1.2/admin_form_image_preivew.egg-info/requires.txt
+-rw-rw-r--   0 sami      (1000) sami      (1000)       20 2023-04-11 11:19:42.000000 admin-form-image-preivew-1.2/admin_form_image_preivew.egg-info/top_level.txt
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.444836 admin-form-image-preivew-1.2/admin_image_preview/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-04 08:52:37.000000 admin-form-image-preivew-1.2/admin_image_preview/__init__.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      168 2023-04-08 06:26:54.000000 admin-form-image-preivew-1.2/admin_image_preview/apps.py
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.444836 admin-form-image-preivew-1.2/admin_image_preview/migrations/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-04 08:52:37.000000 admin-form-image-preivew-1.2/admin_image_preview/migrations/__init__.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      293 2023-04-07 14:30:35.000000 admin-form-image-preivew-1.2/admin_image_preview/models.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1767 2023-04-10 12:09:04.000000 admin-form-image-preivew-1.2/admin_image_preview/readme.md
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.428836 admin-form-image-preivew-1.2/admin_image_preview/static/
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.444836 admin-form-image-preivew-1.2/admin_image_preview/static/admin_image_preview/
+-rw-rw-r--   0 sami      (1000) sami      (1000)     3872 2023-04-11 04:52:02.000000 admin-form-image-preivew-1.2/admin_image_preview/static/admin_image_preview/image_preview.js
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.432836 admin-form-image-preivew-1.2/admin_image_preview/templates/
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.448836 admin-form-image-preivew-1.2/admin_image_preview/templates/admin/
+-rw-rw-r--   0 sami      (1000) sami      (1000)      213 2023-04-10 12:05:52.000000 admin-form-image-preivew-1.2/admin_image_preview/templates/admin/change_form.html
+-rw-rw-r--   0 sami      (1000) sami      (1000)     3804 2023-04-10 08:30:05.000000 admin-form-image-preivew-1.2/admin_image_preview/templates/admin/original_change_form.html
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1113 2023-04-08 07:03:57.000000 admin-form-image-preivew-1.2/del.py
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.452836 admin-form-image-preivew-1.2/docs/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.2/docs/index.rst
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1348 2023-04-11 11:18:56.000000 admin-form-image-preivew-1.2/docs/make_pip.md
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1096 2023-04-10 12:10:33.000000 admin-form-image-preivew-1.2/pyproject.toml
+-rw-rw-r--   0 sami      (1000) sami      (1000)       74 2023-04-11 06:04:33.000000 admin-form-image-preivew-1.2/requirements.txt
+-rw-rw-r--   0 sami      (1000) sami      (1000)      230 2023-04-11 08:00:45.000000 admin-form-image-preivew-1.2/sample_pypirc_test.txt
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.452836 admin-form-image-preivew-1.2/sample_usage/
+-rw-r--r--   0 sami      (1000) sami      (1000)    90636 2023-04-01 08:16:18.000000 admin-form-image-preivew-1.2/sample_usage/92news-logo.png
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1121 2023-04-10 07:55:08.000000 admin-form-image-preivew-1.2/sample_usage/del.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1413 2023-04-10 12:20:30.000000 admin-form-image-preivew-1.2/sample_usage/fixtures.json
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.432836 admin-form-image-preivew-1.2/sample_usage/initsql/
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.452836 admin-form-image-preivew-1.2/sample_usage/initsql/fixtures/
+-rw-rw-r--   0 sami      (1000) sami      (1000)     1165 2023-04-10 12:21:32.000000 admin-form-image-preivew-1.2/sample_usage/initsql/fixtures/auth.json
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.432836 admin-form-image-preivew-1.2/sample_usage/initsql/management/
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.456836 admin-form-image-preivew-1.2/sample_usage/initsql/management/commands/
+-rwxrwxr-x   0 sami      (1000) sami      (1000)     1791 2023-04-10 08:05:37.000000 admin-form-image-preivew-1.2/sample_usage/initsql/management/commands/initsql.py
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.456836 admin-form-image-preivew-1.2/sample_usage/main_app/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 11:55:49.000000 admin-form-image-preivew-1.2/sample_usage/main_app/__init__.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      169 2023-04-08 06:24:35.000000 admin-form-image-preivew-1.2/sample_usage/main_app/asgi.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)     3453 2023-04-10 12:18:16.000000 admin-form-image-preivew-1.2/sample_usage/main_app/settings.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      814 2023-04-10 12:02:30.000000 admin-form-image-preivew-1.2/sample_usage/main_app/urls.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      169 2023-04-08 06:25:37.000000 admin-form-image-preivew-1.2/sample_usage/main_app/wsgi.py
+-rwxrwxr-x   0 sami      (1000) sami      (1000)      664 2023-04-08 06:24:26.000000 admin-form-image-preivew-1.2/sample_usage/manage.py
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.456836 admin-form-image-preivew-1.2/sample_usage/media/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-03 15:01:56.000000 admin-form-image-preivew-1.2/sample_usage/media/init.txt
+-rw-rw-r--   0 sami      (1000) sami      (1000)       56 2023-04-11 06:04:53.000000 admin-form-image-preivew-1.2/sample_usage/requirements.txt
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.460836 admin-form-image-preivew-1.2/sample_usage/sample_app/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-01 14:38:44.000000 admin-form-image-preivew-1.2/sample_usage/sample_app/__init__.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      118 2023-04-01 08:12:10.000000 admin-form-image-preivew-1.2/sample_usage/sample_app/admin.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      151 2023-04-08 06:33:58.000000 admin-form-image-preivew-1.2/sample_usage/sample_app/apps.py
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.460836 admin-form-image-preivew-1.2/sample_usage/sample_app/migrations/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-04-01 08:06:44.000000 admin-form-image-preivew-1.2/sample_usage/sample_app/migrations/__init__.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      194 2023-04-01 08:46:06.000000 admin-form-image-preivew-1.2/sample_usage/sample_app/models.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)       60 2023-04-01 08:06:44.000000 admin-form-image-preivew-1.2/sample_usage/sample_app/tests.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      191 2023-04-01 08:08:31.000000 admin-form-image-preivew-1.2/sample_usage/sample_app/urls.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)       63 2023-04-01 08:06:44.000000 admin-form-image-preivew-1.2/sample_usage/sample_app/views.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      144 2023-04-11 11:19:42.460836 admin-form-image-preivew-1.2/setup.cfg
+-rwxrwxr-x   0 sami      (1000) sami      (1000)     1852 2023-04-11 06:00:12.000000 admin-form-image-preivew-1.2/setup.py
+drwxrwxr-x   0 sami      (1000) sami      (1000)        0 2023-04-11 11:19:42.460836 admin-form-image-preivew-1.2/test/
+-rw-rw-r--   0 sami      (1000) sami      (1000)        0 2023-03-30 08:00:47.000000 admin-form-image-preivew-1.2/test/__init__.py
+-rw-rw-r--   0 sami      (1000) sami      (1000)      118 2023-04-10 12:08:38.000000 admin-form-image-preivew-1.2/towncrier.toml
```

### Comparing `admin-form-image-preivew-1.1/PKG-INFO` & `admin-form-image-preivew-1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admin-form-image-preivew
-Version: 1.1
+Version: 1.2
 Summary: Sami Test Pip
 Home-page: https://github.com/humblesami/admin_form_image_preivew.git
 Author: Sami Akram
 Author-email: Sami Akram <samiakram@live.com>
 Maintainer-email: Sami Akram <samiakram@live.com>
 Project-URL: Changelog, https://github.com/humblesami/admin_form_image_preivew/CHANGES.rst
 Project-URL: Code, https://github.com/humblesami/admin_form_image_preivew
@@ -14,20 +14,27 @@
 Classifier: Programming Language :: Python :: 3.5
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: deploy
 License-File: LICENSE.txt
 
-Test Django Package
+**Insallation**
+1. `pip install admin-form-image-preivew==1.1`
+2. Add `admin_image_preview` in installed apps in `settings.py` of django project
+    INSTALLED_APPS = [
+        'admin_image_preview',
+        # ...
+    ] (at top)
 
-See the sample app for usage/code
 
+**Description**
+It show the preview of every image field in every admin change_form (add/edit) for all models and apps
 
-**Instructions to install/use**
+**Instructions to run the sample usage**
 1. `git clone https://github.com/humblesami/admin_form_image_preivew.git`
 2. `cd admin_form_image_preivew/sample_usage`
 3. `pip install -r requirements.txt`
 
 *Not required* but if you want to reset the database, you can do this
 3.1. `python manage.py initsql.py`
 
@@ -42,9 +49,9 @@
 123
 
 6. Go to
 http://127.0.0.1:8000/admin/admin_image_preview/model1/add/
 
 7. Add image to check preview
 
-8. See docs/make_pip.txt to make/build/test and upload your own pip package
-
+**Make you own pip package**
+See `docs/make_pip.txt` to make/build/test and upload `your own pip package`
```

### Comparing `admin-form-image-preivew-1.1/README.md` & `admin-form-image-preivew-1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,20 @@
-Test Django Package
+**Insallation**
+1. `pip install admin-form-image-preivew==1.1`
+2. Add `admin_image_preview` in installed apps in `settings.py` of django project
+    INSTALLED_APPS = [
+        'admin_image_preview',
+        # ...
+    ] (at top)
 
-See the sample app for usage/code
 
+**Description**
+It show the preview of every image field in every admin change_form (add/edit) for all models and apps
 
-**Instructions to install/use**
+**Instructions to run the sample usage**
 1. `git clone https://github.com/humblesami/admin_form_image_preivew.git`
 2. `cd admin_form_image_preivew/sample_usage`
 3. `pip install -r requirements.txt`
 
 *Not required* but if you want to reset the database, you can do this
 3.1. `python manage.py initsql.py`
 
@@ -22,9 +29,9 @@
 123
 
 6. Go to
 http://127.0.0.1:8000/admin/admin_image_preview/model1/add/
 
 7. Add image to check preview
 
-8. See docs/make_pip.txt to make/build/test and upload your own pip package
-
+**Make you own pip package**
+See `docs/make_pip.txt` to make/build/test and upload `your own pip package`
```

### Comparing `admin-form-image-preivew-1.1/admin_form_image_preivew/settings.py` & `admin-form-image-preivew-1.2/admin_form_image_preivew/settings.py`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.1/admin_form_image_preivew.egg-info/PKG-INFO` & `admin-form-image-preivew-1.2/admin_form_image_preivew.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admin-form-image-preivew
-Version: 1.1
+Version: 1.2
 Summary: Sami Test Pip
 Home-page: https://github.com/humblesami/admin_form_image_preivew.git
 Author: Sami Akram
 Author-email: Sami Akram <samiakram@live.com>
 Maintainer-email: Sami Akram <samiakram@live.com>
 Project-URL: Changelog, https://github.com/humblesami/admin_form_image_preivew/CHANGES.rst
 Project-URL: Code, https://github.com/humblesami/admin_form_image_preivew
@@ -14,20 +14,27 @@
 Classifier: Programming Language :: Python :: 3.5
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: deploy
 License-File: LICENSE.txt
 
-Test Django Package
+**Insallation**
+1. `pip install admin-form-image-preivew==1.1`
+2. Add `admin_image_preview` in installed apps in `settings.py` of django project
+    INSTALLED_APPS = [
+        'admin_image_preview',
+        # ...
+    ] (at top)
 
-See the sample app for usage/code
 
+**Description**
+It show the preview of every image field in every admin change_form (add/edit) for all models and apps
 
-**Instructions to install/use**
+**Instructions to run the sample usage**
 1. `git clone https://github.com/humblesami/admin_form_image_preivew.git`
 2. `cd admin_form_image_preivew/sample_usage`
 3. `pip install -r requirements.txt`
 
 *Not required* but if you want to reset the database, you can do this
 3.1. `python manage.py initsql.py`
 
@@ -42,9 +49,9 @@
 123
 
 6. Go to
 http://127.0.0.1:8000/admin/admin_image_preview/model1/add/
 
 7. Add image to check preview
 
-8. See docs/make_pip.txt to make/build/test and upload your own pip package
-
+**Make you own pip package**
+See `docs/make_pip.txt` to make/build/test and upload `your own pip package`
```

### Comparing `admin-form-image-preivew-1.1/admin_form_image_preivew.egg-info/SOURCES.txt` & `admin-form-image-preivew-1.2/admin_form_image_preivew.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitignore
 CHANGES.rst
 LICENSE.txt
 README.md
 del.py
 pyproject.toml
 requirements.txt
+sample_pypirc_test.txt
 setup.cfg
 setup.py
 towncrier.toml
 admin_form_image_preivew/__init__.py
 admin_form_image_preivew/settings.py
 admin_form_image_preivew/wsgi.py
 admin_form_image_preivew.egg-info/PKG-INFO
```

### Comparing `admin-form-image-preivew-1.1/admin_image_preview/readme.md` & `admin-form-image-preivew-1.2/admin_image_preview/readme.md`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.1/admin_image_preview/static/admin_image_preview/image_preview.js` & `admin-form-image-preivew-1.2/admin_image_preview/static/admin_image_preview/image_preview.js`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.1/admin_image_preview/templates/admin/original_change_form.html` & `admin-form-image-preivew-1.2/admin_image_preview/templates/admin/original_change_form.html`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.1/del.py` & `admin-form-image-preivew-1.2/del.py`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.1/pyproject.toml` & `admin-form-image-preivew-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.1/sample_usage/92news-logo.png` & `admin-form-image-preivew-1.2/sample_usage/92news-logo.png`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.1/sample_usage/del.py` & `admin-form-image-preivew-1.2/sample_usage/del.py`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.1/sample_usage/fixtures.json` & `admin-form-image-preivew-1.2/sample_usage/fixtures.json`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.1/sample_usage/initsql/fixtures/auth.json` & `admin-form-image-preivew-1.2/sample_usage/initsql/fixtures/auth.json`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.1/sample_usage/initsql/management/commands/initsql.py` & `admin-form-image-preivew-1.2/sample_usage/initsql/management/commands/initsql.py`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.1/sample_usage/main_app/settings.py` & `admin-form-image-preivew-1.2/sample_usage/main_app/settings.py`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.1/sample_usage/main_app/urls.py` & `admin-form-image-preivew-1.2/sample_usage/main_app/urls.py`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.1/sample_usage/manage.py` & `admin-form-image-preivew-1.2/sample_usage/manage.py`

 * *Files identical despite different names*

### Comparing `admin-form-image-preivew-1.1/setup.py` & `admin-form-image-preivew-1.2/setup.py`

 * *Files identical despite different names*

