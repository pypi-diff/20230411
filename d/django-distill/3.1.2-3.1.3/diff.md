# Comparing `tmp/django-distill-3.1.2.tar.gz` & `tmp/django-distill-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-distill-3.1.2.tar", last modified: Fri Mar 31 04:34:37 2023, max compression
+gzip compressed data, was "django-distill-3.1.3.tar", last modified: Tue Apr 11 11:18:28 2023, max compression
```

## Comparing `django-distill-3.1.2.tar` & `django-distill-3.1.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-03-31 04:34:37.928729 django-distill-3.1.2/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1081 2020-07-12 16:04:20.000000 django-distill-3.1.2/LICENSE
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2020-05-23 07:15:18.000000 django-distill-3.1.2/MANIFEST.in
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    20100 2023-03-31 04:34:37.928729 django-distill-3.1.2/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    18856 2023-03-31 04:33:32.000000 django-distill-3.1.2/README.md
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-03-31 04:34:37.924729 django-distill-3.1.2/django_distill/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1107 2023-03-31 04:34:33.000000 django-distill-3.1.2/django_distill/__init__.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-03-31 04:34:37.924729 django-distill-3.1.2/django_distill/backends/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     5195 2021-12-15 08:00:51.000000 django-distill-3.1.2/django_distill/backends/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     2106 2023-03-30 04:26:07.000000 django-distill-3.1.2/django_distill/backends/amazon_s3.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     2608 2023-03-30 04:26:07.000000 django-distill-3.1.2/django_distill/backends/google_storage.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     5205 2023-03-30 04:26:07.000000 django-distill-3.1.2/django_distill/backends/microsoft_azure_storage.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1512 2022-12-09 01:50:52.000000 django-distill-3.1.2/django_distill/distill.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      138 2021-12-15 08:00:51.000000 django-distill-3.1.2/django_distill/errors.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-03-31 04:34:37.924729 django-distill-3.1.2/django_distill/management/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-12-15 08:00:51.000000 django-distill-3.1.2/django_distill/management/__init__.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-03-31 04:34:37.924729 django-distill-3.1.2/django_distill/management/commands/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-12-15 08:00:51.000000 django-distill-3.1.2/django_distill/management/commands/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     3644 2022-12-09 01:50:52.000000 django-distill-3.1.2/django_distill/management/commands/distill-local.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     4718 2023-03-31 04:32:45.000000 django-distill-3.1.2/django_distill/management/commands/distill-publish.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     3229 2022-12-09 01:50:52.000000 django-distill-3.1.2/django_distill/management/commands/distill-test-publish.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     2137 2023-03-31 04:32:45.000000 django-distill-3.1.2/django_distill/publisher.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    16893 2023-03-30 07:25:43.000000 django-distill-3.1.2/django_distill/renderer.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-03-31 04:34:37.924729 django-distill-3.1.2/django_distill.egg-info/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    20100 2023-03-31 04:34:37.000000 django-distill-3.1.2/django_distill.egg-info/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1045 2023-03-31 04:34:37.000000 django-distill-3.1.2/django_distill.egg-info/SOURCES.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2023-03-31 04:34:37.000000 django-distill-3.1.2/django_distill.egg-info/dependency_links.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      120 2023-03-31 04:34:37.000000 django-distill-3.1.2/django_distill.egg-info/requires.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       21 2023-03-31 04:34:37.000000 django-distill-3.1.2/django_distill.egg-info/top_level.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       16 2020-04-16 06:00:59.000000 django-distill-3.1.2/requirements.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2023-03-31 04:34:37.928729 django-distill-3.1.2/setup.cfg
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1862 2023-03-31 04:34:27.000000 django-distill-3.1.2/setup.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-03-31 04:34:37.928729 django-distill-3.1.2/tests/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2020-06-08 04:28:45.000000 django-distill-3.1.2/tests/__init__.py
--rw-r--r--   0 meeb      (1000) meeb      (1000)      455 2023-03-30 05:22:40.000000 django-distill-3.1.2/tests/i18n_urls.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      505 2023-03-30 05:14:43.000000 django-distill-3.1.2/tests/namespaced_sub_urls.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      894 2023-03-30 05:14:48.000000 django-distill-3.1.2/tests/namespaced_urls.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      512 2023-03-30 05:14:54.000000 django-distill-3.1.2/tests/no_namespaced_urls.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1205 2023-03-30 06:34:38.000000 django-distill-3.1.2/tests/settings.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      511 2020-11-14 02:14:57.000000 django-distill-3.1.2/tests/test_commands.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      574 2020-06-08 04:29:21.000000 django-distill-3.1.2/tests/test_interface.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    19299 2023-03-30 06:59:41.000000 django-distill-3.1.2/tests/test_renderer.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1454 2022-12-09 01:50:52.000000 django-distill-3.1.2/tests/test_static.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     6888 2023-03-30 06:46:06.000000 django-distill-3.1.2/tests/urls.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-04-11 11:18:28.735405 django-distill-3.1.3/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1081 2020-07-12 16:04:20.000000 django-distill-3.1.3/LICENSE
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2020-05-23 07:15:18.000000 django-distill-3.1.3/MANIFEST.in
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    20444 2023-04-11 11:18:28.735405 django-distill-3.1.3/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    19200 2023-04-11 11:17:03.000000 django-distill-3.1.3/README.md
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-04-11 11:18:28.731405 django-distill-3.1.3/django_distill/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1107 2023-04-11 11:17:49.000000 django-distill-3.1.3/django_distill/__init__.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-04-11 11:18:28.731405 django-distill-3.1.3/django_distill/backends/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     5195 2021-12-15 08:00:51.000000 django-distill-3.1.3/django_distill/backends/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     2454 2023-04-11 11:16:33.000000 django-distill-3.1.3/django_distill/backends/amazon_s3.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     2642 2023-04-11 11:16:33.000000 django-distill-3.1.3/django_distill/backends/google_storage.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     5205 2023-03-30 04:26:07.000000 django-distill-3.1.3/django_distill/backends/microsoft_azure_storage.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1512 2022-12-09 01:50:52.000000 django-distill-3.1.3/django_distill/distill.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      138 2021-12-15 08:00:51.000000 django-distill-3.1.3/django_distill/errors.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-04-11 11:18:28.731405 django-distill-3.1.3/django_distill/management/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-12-15 08:00:51.000000 django-distill-3.1.3/django_distill/management/__init__.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-04-11 11:18:28.731405 django-distill-3.1.3/django_distill/management/commands/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-12-15 08:00:51.000000 django-distill-3.1.3/django_distill/management/commands/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     3644 2022-12-09 01:50:52.000000 django-distill-3.1.3/django_distill/management/commands/distill-local.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     4718 2023-03-31 04:32:45.000000 django-distill-3.1.3/django_distill/management/commands/distill-publish.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     3229 2022-12-09 01:50:52.000000 django-distill-3.1.3/django_distill/management/commands/distill-test-publish.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     2137 2023-03-31 04:32:45.000000 django-distill-3.1.3/django_distill/publisher.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    16893 2023-03-30 07:25:43.000000 django-distill-3.1.3/django_distill/renderer.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-04-11 11:18:28.731405 django-distill-3.1.3/django_distill.egg-info/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    20444 2023-04-11 11:18:28.000000 django-distill-3.1.3/django_distill.egg-info/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1045 2023-04-11 11:18:28.000000 django-distill-3.1.3/django_distill.egg-info/SOURCES.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2023-04-11 11:18:28.000000 django-distill-3.1.3/django_distill.egg-info/dependency_links.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      120 2023-04-11 11:18:28.000000 django-distill-3.1.3/django_distill.egg-info/requires.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       21 2023-04-11 11:18:28.000000 django-distill-3.1.3/django_distill.egg-info/top_level.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       16 2020-04-16 06:00:59.000000 django-distill-3.1.3/requirements.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2023-04-11 11:18:28.735405 django-distill-3.1.3/setup.cfg
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1862 2023-04-11 11:17:40.000000 django-distill-3.1.3/setup.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-04-11 11:18:28.735405 django-distill-3.1.3/tests/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2020-06-08 04:28:45.000000 django-distill-3.1.3/tests/__init__.py
+-rw-r--r--   0 meeb      (1000) meeb      (1000)      455 2023-03-30 05:22:40.000000 django-distill-3.1.3/tests/i18n_urls.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      505 2023-03-30 05:14:43.000000 django-distill-3.1.3/tests/namespaced_sub_urls.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      894 2023-03-30 05:14:48.000000 django-distill-3.1.3/tests/namespaced_urls.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      512 2023-03-30 05:14:54.000000 django-distill-3.1.3/tests/no_namespaced_urls.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1205 2023-03-30 06:34:38.000000 django-distill-3.1.3/tests/settings.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      511 2020-11-14 02:14:57.000000 django-distill-3.1.3/tests/test_commands.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      574 2020-06-08 04:29:21.000000 django-distill-3.1.3/tests/test_interface.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    19299 2023-03-30 06:59:41.000000 django-distill-3.1.3/tests/test_renderer.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1454 2022-12-09 01:50:52.000000 django-distill-3.1.3/tests/test_static.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     6888 2023-03-30 06:46:06.000000 django-distill-3.1.3/tests/urls.py
```

### Comparing `django-distill-3.1.2/LICENSE` & `django-distill-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/PKG-INFO` & `django-distill-3.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-distill
-Version: 3.1.2
+Version: 3.1.3
 Summary: Static site renderer and publisher for Django.
 Home-page: https://github.com/meeb/django-distill
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: MIT
 Keywords: django,distill,static,website,jamstack,s3,amazon s3,aws,amazon,google,microsoft,google cloud,google cloud storage,azure,azure storage,azure blob storage
 Platform: UNKNOWN
@@ -340,15 +340,15 @@
 
 `--ignore-remote-content`: Do not fetch the list of remote files. It means that all
 files will be uploaded, and no existing remote file will be  deleted. This can be
 useful if you have a lot of files on the remote server, and you know that you want
 to update most of them, and you don't care if old files remain on the server.
 
 `--parallel-publish [number of threads]`: Publish files in parallel on multiple
-threads, this can speed up upload. Defaults to 1 thread.
+threads, this can speed up publishing. Defaults to `1` thread.
 
 **Note** that this means if you use `--force` and `--quiet` that the output
 directory will have all files not part of the site export deleted without any
 confirmation.
 
 **Note**  If any of your views contain a Python error then rendering will fail
 then the stack trace will be printed to the terminal and the rendering command
@@ -503,19 +503,25 @@
   must already exist and be set up to host a public static website (use the
   Google Cloud control panel). Options:
 
 ```python
 'some-google-storage-bucket': {
     'ENGINE': 'django_distill.backends.google_storage',
     'PUBLIC_URL': 'https://storage.googleapis.com/[bucket.name.here]/',
-    'JSON_CREDENTIALS': '/path/to/some/credentials.json',
     'BUCKET': '[bucket.name.here]',
+    'JSON_CREDENTIALS': '/path/to/some/credentials.json',
 },
 ```
 
+Note that `JSON_CREDENTIALS` is optional; if it is not specified, the google libraries
+will try other authentication methods, in the search order described here:
+https://cloud.google.com/docs/authentication/application-default-credentials (e.g. the
+`GOOGLE_APPLICATION_CREDENTIALS` environment variable, attached service account, etc).
+
+
 **django_distill.backends.microsoft_azure_storage**: Publish to a Microsoft
   Azure Blob Storage container. Requires the Python library
   `azure-storage-blob` (`$ pip install django-distill[microsoft]`). The storage
   account must already exist and be set up to host a public static website
   (use the Microsoft Azure control panel). Options:
 
 ```python
```

### Comparing `django-distill-3.1.2/README.md` & `django-distill-3.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -311,15 +311,15 @@
 
 `--ignore-remote-content`: Do not fetch the list of remote files. It means that all
 files will be uploaded, and no existing remote file will be  deleted. This can be
 useful if you have a lot of files on the remote server, and you know that you want
 to update most of them, and you don't care if old files remain on the server.
 
 `--parallel-publish [number of threads]`: Publish files in parallel on multiple
-threads, this can speed up upload. Defaults to 1 thread.
+threads, this can speed up publishing. Defaults to `1` thread.
 
 **Note** that this means if you use `--force` and `--quiet` that the output
 directory will have all files not part of the site export deleted without any
 confirmation.
 
 **Note**  If any of your views contain a Python error then rendering will fail
 then the stack trace will be printed to the terminal and the rendering command
@@ -474,19 +474,25 @@
   must already exist and be set up to host a public static website (use the
   Google Cloud control panel). Options:
 
 ```python
 'some-google-storage-bucket': {
     'ENGINE': 'django_distill.backends.google_storage',
     'PUBLIC_URL': 'https://storage.googleapis.com/[bucket.name.here]/',
-    'JSON_CREDENTIALS': '/path/to/some/credentials.json',
     'BUCKET': '[bucket.name.here]',
+    'JSON_CREDENTIALS': '/path/to/some/credentials.json',
 },
 ```
 
+Note that `JSON_CREDENTIALS` is optional; if it is not specified, the google libraries
+will try other authentication methods, in the search order described here:
+https://cloud.google.com/docs/authentication/application-default-credentials (e.g. the
+`GOOGLE_APPLICATION_CREDENTIALS` environment variable, attached service account, etc).
+
+
 **django_distill.backends.microsoft_azure_storage**: Publish to a Microsoft
   Azure Blob Storage container. Requires the Python library
   `azure-storage-blob` (`$ pip install django-distill[microsoft]`). The storage
   account must already exist and be set up to host a public static website
   (use the Microsoft Azure control panel). Options:
 
 ```python
```

### Comparing `django-distill-3.1.2/django_distill/__init__.py` & `django-distill-3.1.3/django_distill/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '3.1.2'
+__version__ = '3.1.3'
 
 
 from django import __version__ as django_version
 from django_distill.errors import DistillError
 
 
 try:
```

### Comparing `django-distill-3.1.2/django_distill/backends/__init__.py` & `django-distill-3.1.3/django_distill/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/django_distill/backends/amazon_s3.py` & `django-distill-3.1.3/django_distill/backends/amazon_s3.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 import sys
-
+import mimetypes
 
 try:
     import boto3
 except ImportError:
     name = 'django_distill.backends.amazon_s3'
     pipm = 'boto3'
     sys.stdout.write('{} backend requires {}:\n'.format(name, pipm))
     sys.stdout.write('$ pip install .[amazon]{}\n\n'.format(pipm))
     raise
 
-
 from django_distill.errors import DistillPublishError
 from django_distill.backends import BackendBase
 
 
 class AmazonS3Backend(BackendBase):
     '''
         Publisher for Amazon S3. Implements the BackendBase.
     '''
 
     REQUIRED_OPTIONS = ('ENGINE', 'PUBLIC_URL', 'ACCESS_KEY_ID',
                         'SECRET_ACCESS_KEY', 'BUCKET')
 
     def _get_object(self, name):
         bucket = self.account_container()
-        return self.d['connection'].get_object(Bucket=bucket, Key=name)
+        return self.d['connection'].head_object(Bucket=bucket, Key=name)
 
     def account_username(self):
         return self.options.get('ACCESS_KEY_ID', '')
 
     def account_container(self):
         return self.options.get('BUCKET', '')
 
     def authenticate(self, calling_format=None):
         access_key_id = self.account_username()
         secret_access_key = self.options.get('SECRET_ACCESS_KEY', '')
         bucket = self.account_container()
         self.d['connection'] = boto3.client('s3', aws_access_key_id=access_key_id,
                                             aws_secret_access_key=secret_access_key)
-        self.d['bucket'] = self.d['connection'].get_bucket(bucket)
+        self.d['bucket'] = bucket
 
     def list_remote_files(self):
         rtn = set()
-        for obj in self.d['bucket'].objects.all():
-            rtn.add(obj.key)
+        response = self.d['connection'].list_objects_v2(Bucket=self.d['bucket'])
+        if 'Contents' in response:
+            for obj in response['Contents']:
+                rtn.add(obj['Key'])
         return rtn
 
     def delete_remote_file(self, remote_name):
-        obj = self._get_object(remote_name)
-        return obj.delete()
+        self.d['connection'].delete_object(Bucket=self.d['bucket'], Key=remote_name)
 
     def compare_file(self, local_name, remote_name):
         obj = self._get_object(remote_name)
         local_hash = self._get_local_file_hash(local_name)
-        return local_hash == obj.e_tag[1:-1]
+        return local_hash == obj['ETag'][1:-1]
 
     def upload_file(self, local_name, remote_name):
-        return self.d['bucket'].upload_file(local_name, remote_name)
+        content_type, _ = mimetypes.guess_type(local_name)
+        if content_type is None:
+            content_type = 'application/octet-stream'
+        extra_args = {'ContentType': content_type}
+        self.d['connection'].upload_file(local_name, self.d['bucket'], remote_name, ExtraArgs=extra_args)
 
     def create_remote_dir(self, remote_dir_name):
         # not required for S3 buckets
         return True
 
-
 backend_class = AmazonS3Backend
```

### Comparing `django-distill-3.1.2/django_distill/backends/google_storage.py` & `django-distill-3.1.3/django_distill/backends/google_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,28 +21,30 @@
 
 
 class GoogleCloudStorageBackend(BackendBase):
     '''
         Publisher for Google Cloud Storage. Implements the BackendBase.
     '''
 
-    REQUIRED_OPTIONS = ('ENGINE', 'JSON_CREDENTIALS', 'BUCKET')
+    REQUIRED_OPTIONS = ('ENGINE', 'BUCKET')
 
     def account_username(self):
         return
 
     def account_container(self):
         return self.options.get('BUCKET', '')
 
     def authenticate(self):
         credentials_file = self.options.get('JSON_CREDENTIALS', '')
-        if not os.path.exists(credentials_file):
-            err = 'Credentials file does not exist: {}'
-            raise DistillPublishError(err.format(credentials_file))
-        os.environ['GOOGLE_APPLICATION_CREDENTIALS'] = credentials_file
+        if credentials_file:
+            if not os.path.exists(credentials_file):
+                err = 'Credentials file does not exist: {}'
+                raise DistillPublishError(err.format(credentials_file))
+            os.environ['GOOGLE_APPLICATION_CREDENTIALS'] = credentials_file
+        
         bucket = self.account_container()
         self.d['connection'] = storage.Client()
         self.d['bucket'] = self.d['connection'].get_bucket(bucket)
 
     def list_remote_files(self):
         rtn = set()
         for b in self.d['bucket'].list_blobs():
```

### Comparing `django-distill-3.1.2/django_distill/backends/microsoft_azure_storage.py` & `django-distill-3.1.3/django_distill/backends/microsoft_azure_storage.py`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/django_distill/distill.py` & `django-distill-3.1.3/django_distill/distill.py`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/django_distill/management/commands/distill-local.py` & `django-distill-3.1.3/django_distill/management/commands/distill-local.py`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/django_distill/management/commands/distill-publish.py` & `django-distill-3.1.3/django_distill/management/commands/distill-publish.py`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/django_distill/management/commands/distill-test-publish.py` & `django-distill-3.1.3/django_distill/management/commands/distill-test-publish.py`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/django_distill/publisher.py` & `django-distill-3.1.3/django_distill/publisher.py`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/django_distill/renderer.py` & `django-distill-3.1.3/django_distill/renderer.py`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/django_distill.egg-info/PKG-INFO` & `django-distill-3.1.3/django_distill.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-distill
-Version: 3.1.2
+Version: 3.1.3
 Summary: Static site renderer and publisher for Django.
 Home-page: https://github.com/meeb/django-distill
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: MIT
 Keywords: django,distill,static,website,jamstack,s3,amazon s3,aws,amazon,google,microsoft,google cloud,google cloud storage,azure,azure storage,azure blob storage
 Platform: UNKNOWN
@@ -340,15 +340,15 @@
 
 `--ignore-remote-content`: Do not fetch the list of remote files. It means that all
 files will be uploaded, and no existing remote file will be  deleted. This can be
 useful if you have a lot of files on the remote server, and you know that you want
 to update most of them, and you don't care if old files remain on the server.
 
 `--parallel-publish [number of threads]`: Publish files in parallel on multiple
-threads, this can speed up upload. Defaults to 1 thread.
+threads, this can speed up publishing. Defaults to `1` thread.
 
 **Note** that this means if you use `--force` and `--quiet` that the output
 directory will have all files not part of the site export deleted without any
 confirmation.
 
 **Note**  If any of your views contain a Python error then rendering will fail
 then the stack trace will be printed to the terminal and the rendering command
@@ -503,19 +503,25 @@
   must already exist and be set up to host a public static website (use the
   Google Cloud control panel). Options:
 
 ```python
 'some-google-storage-bucket': {
     'ENGINE': 'django_distill.backends.google_storage',
     'PUBLIC_URL': 'https://storage.googleapis.com/[bucket.name.here]/',
-    'JSON_CREDENTIALS': '/path/to/some/credentials.json',
     'BUCKET': '[bucket.name.here]',
+    'JSON_CREDENTIALS': '/path/to/some/credentials.json',
 },
 ```
 
+Note that `JSON_CREDENTIALS` is optional; if it is not specified, the google libraries
+will try other authentication methods, in the search order described here:
+https://cloud.google.com/docs/authentication/application-default-credentials (e.g. the
+`GOOGLE_APPLICATION_CREDENTIALS` environment variable, attached service account, etc).
+
+
 **django_distill.backends.microsoft_azure_storage**: Publish to a Microsoft
   Azure Blob Storage container. Requires the Python library
   `azure-storage-blob` (`$ pip install django-distill[microsoft]`). The storage
   account must already exist and be set up to host a public static website
   (use the Microsoft Azure control panel). Options:
 
 ```python
```

### Comparing `django-distill-3.1.2/django_distill.egg-info/SOURCES.txt` & `django-distill-3.1.3/django_distill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/setup.py` & `django-distill-3.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 
-version = '3.1.2'
+version = '3.1.3'
 
 
 with open('README.md', 'rt') as f:
     long_description = f.read()
 
 
 with open('requirements.txt', 'rt') as f:
```

### Comparing `django-distill-3.1.2/tests/namespaced_urls.py` & `django-distill-3.1.3/tests/namespaced_urls.py`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/tests/no_namespaced_urls.py` & `django-distill-3.1.3/tests/no_namespaced_urls.py`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/tests/settings.py` & `django-distill-3.1.3/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/tests/test_interface.py` & `django-distill-3.1.3/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/tests/test_renderer.py` & `django-distill-3.1.3/tests/test_renderer.py`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/tests/test_static.py` & `django-distill-3.1.3/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `django-distill-3.1.2/tests/urls.py` & `django-distill-3.1.3/tests/urls.py`

 * *Files identical despite different names*

