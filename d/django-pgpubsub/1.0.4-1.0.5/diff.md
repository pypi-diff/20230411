# Comparing `tmp/django_pgpubsub-1.0.4.tar.gz` & `tmp/django_pgpubsub-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgpubsub-1.0.4.tar", max compression
+gzip compressed data, was "django_pgpubsub-1.0.5.tar", max compression
```

## Comparing `django_pgpubsub-1.0.4.tar` & `django_pgpubsub-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,27 @@
--rw-r--r--   0        0        0     1456 2022-11-05 17:21:11.401611 django_pgpubsub-1.0.4/LICENSE
--rw-r--r--   0        0        0    25976 2023-04-10 14:46:46.455426 django_pgpubsub-1.0.4/README.md
--rw-r--r--   0        0        0      390 2022-11-05 17:21:11.403909 django_pgpubsub-1.0.4/pgpubsub/__init__.py
--rw-r--r--   0        0        0     5843 2023-04-09 15:03:50.911492 django_pgpubsub-1.0.4/pgpubsub/channel.py
--rw-r--r--   0        0        0     4980 2023-02-02 16:18:56.082239 django_pgpubsub-1.0.4/pgpubsub/listen.py
--rw-r--r--   0        0        0     2647 2023-01-10 17:48:32.840212 django_pgpubsub-1.0.4/pgpubsub/listeners.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404451 django_pgpubsub-1.0.4/pgpubsub/management/__init__.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404567 django_pgpubsub-1.0.4/pgpubsub/management/commands/__init__.py
--rw-r--r--   0        0        0     1288 2023-02-02 16:18:56.082808 django_pgpubsub-1.0.4/pgpubsub/management/commands/listen.py
--rw-r--r--   0        0        0      751 2023-04-09 15:03:50.912029 django_pgpubsub-1.0.4/pgpubsub/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405068 django_pgpubsub-1.0.4/pgpubsub/migrations/__init__.py
--rw-r--r--   0        0        0      690 2023-04-09 15:03:50.912484 django_pgpubsub-1.0.4/pgpubsub/models.py
--rw-r--r--   0        0        0     2130 2022-11-05 17:21:11.405511 django_pgpubsub-1.0.4/pgpubsub/notify.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405631 django_pgpubsub-1.0.4/pgpubsub/tests/__init__.py
--rw-r--r--   0        0        0      164 2022-11-05 17:21:11.405752 django_pgpubsub-1.0.4/pgpubsub/tests/apps.py
--rw-r--r--   0        0        0      640 2023-02-01 14:09:57.717907 django_pgpubsub-1.0.4/pgpubsub/tests/channels.py
--rw-r--r--   0        0        0     1938 2023-04-09 15:03:50.912969 django_pgpubsub-1.0.4/pgpubsub/tests/listeners.py
--rw-r--r--   0        0        0     2734 2022-11-05 17:21:11.406152 django_pgpubsub-1.0.4/pgpubsub/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.406217 django_pgpubsub-1.0.4/pgpubsub/tests/migrations/__init__.py
--rw-r--r--   0        0        0     1209 2023-02-02 13:52:43.296803 django_pgpubsub-1.0.4/pgpubsub/tests/models.py
--rw-r--r--   0        0        0     8890 2023-04-09 15:03:50.913480 django_pgpubsub-1.0.4/pgpubsub/tests/test_core.py
--rw-r--r--   0        0        0     1040 2023-04-09 15:03:50.913993 django_pgpubsub-1.0.4/pgpubsub/triggers.py
--rw-r--r--   0        0        0     2082 2023-04-10 14:46:01.186583 django_pgpubsub-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    27299 1970-01-01 00:00:00.000000 django_pgpubsub-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1456 2022-11-05 17:21:11.401611 django_pgpubsub-1.0.5/LICENSE
+-rw-r--r--   0        0        0    25976 2023-04-10 16:26:51.399667 django_pgpubsub-1.0.5/README.md
+-rw-r--r--   0        0        0      390 2022-11-05 17:21:11.403909 django_pgpubsub-1.0.5/pgpubsub/__init__.py
+-rw-r--r--   0        0        0     7341 2023-04-11 13:37:33.189103 django_pgpubsub-1.0.5/pgpubsub/channel.py
+-rw-r--r--   0        0        0     4980 2023-02-02 16:18:56.082239 django_pgpubsub-1.0.5/pgpubsub/listen.py
+-rw-r--r--   0        0        0     2647 2023-01-10 17:48:32.840212 django_pgpubsub-1.0.5/pgpubsub/listeners.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404451 django_pgpubsub-1.0.5/pgpubsub/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404567 django_pgpubsub-1.0.5/pgpubsub/management/commands/__init__.py
+-rw-r--r--   0        0        0     1288 2023-02-02 16:18:56.082808 django_pgpubsub-1.0.5/pgpubsub/management/commands/listen.py
+-rw-r--r--   0        0        0      751 2023-04-10 16:26:51.407699 django_pgpubsub-1.0.5/pgpubsub/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405068 django_pgpubsub-1.0.5/pgpubsub/migrations/__init__.py
+-rw-r--r--   0        0        0      690 2023-04-10 16:26:51.408192 django_pgpubsub-1.0.5/pgpubsub/models.py
+-rw-r--r--   0        0        0     2130 2022-11-05 17:21:11.405511 django_pgpubsub-1.0.5/pgpubsub/notify.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405631 django_pgpubsub-1.0.5/pgpubsub/tests/__init__.py
+-rw-r--r--   0        0        0      164 2022-11-05 17:21:11.405752 django_pgpubsub-1.0.5/pgpubsub/tests/apps.py
+-rw-r--r--   0        0        0      640 2023-04-11 08:28:49.364826 django_pgpubsub-1.0.5/pgpubsub/tests/channels.py
+-rw-r--r--   0        0        0     1938 2023-04-11 08:32:09.955989 django_pgpubsub-1.0.5/pgpubsub/tests/listeners.py
+-rw-r--r--   0        0        0     2734 2022-11-05 17:21:11.406152 django_pgpubsub-1.0.5/pgpubsub/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0      673 2023-04-11 13:37:33.190988 django_pgpubsub-1.0.5/pgpubsub/tests/migrations/0002_auto_20230411_0829.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.406217 django_pgpubsub-1.0.5/pgpubsub/tests/migrations/__init__.py
+-rw-r--r--   0        0        0     1348 2023-04-11 13:37:33.192550 django_pgpubsub-1.0.5/pgpubsub/tests/models.py
+-rw-r--r--   0        0        0     5876 2023-04-11 13:37:33.193462 django_pgpubsub-1.0.5/pgpubsub/tests/test_core.py
+-rw-r--r--   0        0        0     2199 2023-04-11 13:37:33.194348 django_pgpubsub-1.0.5/pgpubsub/tests/test_deserialize.py
+-rw-r--r--   0        0        0     4286 2023-04-11 13:37:33.194866 django_pgpubsub-1.0.5/pgpubsub/tests/test_trigger_deserialize.py
+-rw-r--r--   0        0        0     1040 2023-04-10 16:26:51.410131 django_pgpubsub-1.0.5/pgpubsub/triggers.py
+-rw-r--r--   0        0        0     2082 2023-04-11 13:37:57.567950 django_pgpubsub-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    27299 1970-01-01 00:00:00.000000 django_pgpubsub-1.0.5/PKG-INFO
```

### Comparing `django_pgpubsub-1.0.4/LICENSE` & `django_pgpubsub-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.4/README.md` & `django_pgpubsub-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.4/pgpubsub/listen.py` & `django_pgpubsub-1.0.5/pgpubsub/listen.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.4/pgpubsub/listeners.py` & `django_pgpubsub-1.0.5/pgpubsub/listeners.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.4/pgpubsub/management/commands/listen.py` & `django_pgpubsub-1.0.5/pgpubsub/management/commands/listen.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.4/pgpubsub/migrations/0001_initial.py` & `django_pgpubsub-1.0.5/pgpubsub/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.4/pgpubsub/models.py` & `django_pgpubsub-1.0.5/pgpubsub/models.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.4/pgpubsub/notify.py` & `django_pgpubsub-1.0.5/pgpubsub/notify.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.4/pgpubsub/tests/channels.py` & `django_pgpubsub-1.0.5/pgpubsub/tests/channels.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.4/pgpubsub/tests/listeners.py` & `django_pgpubsub-1.0.5/pgpubsub/tests/listeners.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.4/pgpubsub/tests/migrations/0001_initial.py` & `django_pgpubsub-1.0.5/pgpubsub/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.4/pgpubsub/tests/models.py` & `django_pgpubsub-1.0.5/pgpubsub/tests/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,19 +11,26 @@
 class Media(models.Model):
     name = models.TextField()
     content_type = models.TextField(null=True)
     size = models.BigIntegerField(null=True)
 
 
 class Author(models.Model):
-    user = models.ForeignKey(User, on_delete=models.PROTECT, null=True)
+    user = models.ForeignKey(
+        User, on_delete=models.PROTECT, null=True)
     name = models.TextField()
     age = models.IntegerField(null=True)
     active = models.BooleanField(default=True)
-    profile_picture = models.ForeignKey(Media, null=True, on_delete=models.PROTECT)
+    profile_picture = models.ForeignKey(
+        Media,
+        null=True,
+        on_delete=models.PROTECT,
+        db_column='picture',
+    )
+    alternative_name = models.TextField(db_column='other', null=True)
 
 
 class Post(models.Model):
     content = models.TextField()
     date = models.DateTimeField()
     author = models.ForeignKey(
         Author, null=True, on_delete=models.SET_NULL, related_name='entries'
```

### Comparing `django_pgpubsub-1.0.4/pgpubsub/triggers.py` & `django_pgpubsub-1.0.5/pgpubsub/triggers.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.4/pyproject.toml` & `django_pgpubsub-1.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 fail_under = 100
 
 [tool.poetry]
 name = "django-pgpubsub"
 packages = [
   { include = "pgpubsub" }
 ]
-version = "1.0.4"
+version = "1.0.5"
 description = "A distributed task processing framework for Django built on top of the Postgres NOTIFY/LISTEN protocol."
 authors = ["Opus 10 Engineering"]
 classifiers = [
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
```

### Comparing `django_pgpubsub-1.0.4/PKG-INFO` & `django_pgpubsub-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgpubsub
-Version: 1.0.4
+Version: 1.0.5
 Summary: A distributed task processing framework for Django built on top of the Postgres NOTIFY/LISTEN protocol.
 Home-page: https://github.com/Opus10/django-pgpubsub
 License: BSD-3-Clause
 Author: Opus 10 Engineering
 Requires-Python: >=3.7.0,<4
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

