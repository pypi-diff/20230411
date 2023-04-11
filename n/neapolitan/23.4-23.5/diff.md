# Comparing `tmp/neapolitan-23.4.tar.gz` & `tmp/neapolitan-23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neapolitan-23.4.tar", last modified: Mon Apr 10 10:08:31 2023, max compression
+gzip compressed data, was "neapolitan-23.5.tar", last modified: Tue Apr 11 14:14:04 2023, max compression
```

## Comparing `neapolitan-23.4.tar` & `neapolitan-23.5.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0       59 2023-04-08 15:53:57.994299 neapolitan-23.4/.gitignore
--rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.4/LICENSE
--rw-r--r--   0        0        0      837 2023-04-10 08:57:02.274208 neapolitan-23.4/Notes.txt
--rw-r--r--   0        0        0      942 2023-04-08 15:11:04.794396 neapolitan-23.4/README.rst
--rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.4/docs/Makefile
--rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.4/docs/make.bat
--rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.4/docs/source/conf.py
--rw-r--r--   0        0        0     1162 2023-04-08 15:11:01.258471 neapolitan-23.4/docs/source/index.rst
--rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-23.4/justfile
--rw-r--r--   0        0        0      653 2023-04-10 09:35:41.106347 neapolitan-23.4/pyproject.toml
--rw-r--r--   0        0        0      948 2023-04-10 10:07:28.363677 neapolitan-23.4/src/neapolitan/__init__.py
--rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.4/src/neapolitan/templates/neapolitan/object_confirm_delete.html
--rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.4/src/neapolitan/templates/neapolitan/object_detail.html
--rw-r--r--   0        0        0      349 2023-01-30 14:23:01.301967 neapolitan-23.4/src/neapolitan/templates/neapolitan/object_form.html
--rw-r--r--   0        0        0      264 2023-04-08 14:09:43.805065 neapolitan-23.4/src/neapolitan/templates/neapolitan/object_list.html
--rw-r--r--   0        0        0      131 2023-01-30 15:27:46.386717 neapolitan-23.4/src/neapolitan/templates/neapolitan/partial/detail.html
--rw-r--r--   0        0        0      313 2023-01-30 19:42:10.115831 neapolitan-23.4/src/neapolitan/templates/neapolitan/partial/list.html
--rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.4/src/neapolitan/templatetags/__init__.py
--rw-r--r--   0        0        0     1263 2023-04-08 14:11:26.730590 neapolitan-23.4/src/neapolitan/templatetags/neapolitan.py
--rw-r--r--   0        0        0    16787 2023-04-10 10:04:43.015907 neapolitan-23.4/src/neapolitan/views.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.4/tests/__init__.py
--rw-r--r--   0        0        0      840 2023-04-10 09:00:23.657242 neapolitan-23.4/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.4/tests/migrations/__init__.py
--rw-r--r--   0        0        0      236 2023-04-10 08:59:09.860534 neapolitan-23.4/tests/models.py
--rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-23.4/tests/settings.py
--rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-23.4/tests/templates/base.html
--rw-r--r--   0        0        0     3850 2023-04-10 09:49:22.975379 neapolitan-23.4/tests/tests.py
--rw-r--r--   0        0        0     1517 1970-01-01 00:00:00.000000 neapolitan-23.4/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-04-08 15:53:57.994299 neapolitan-23.5/.gitignore
+-rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.5/LICENSE
+-rw-r--r--   0        0        0     1128 2023-04-11 13:44:05.034404 neapolitan-23.5/Notes.txt
+-rw-r--r--   0        0        0     1621 2023-04-10 13:12:58.659109 neapolitan-23.5/README.rst
+-rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.5/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.5/docs/make.bat
+-rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.5/docs/source/conf.py
+-rw-r--r--   0        0        0      160 2023-04-11 14:07:29.272376 neapolitan-23.5/docs/source/crud-view.rst
+-rw-r--r--   0        0        0     1169 2023-04-11 14:06:03.118807 neapolitan-23.5/docs/source/index.rst
+-rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-23.5/justfile
+-rw-r--r--   0        0        0      653 2023-04-10 09:35:41.106347 neapolitan-23.5/pyproject.toml
+-rw-r--r--   0        0        0      948 2023-04-11 14:13:17.268344 neapolitan-23.5/src/neapolitan/__init__.py
+-rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.5/src/neapolitan/templates/neapolitan/object_confirm_delete.html
+-rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.5/src/neapolitan/templates/neapolitan/object_detail.html
+-rw-r--r--   0        0        0      349 2023-01-30 14:23:01.301967 neapolitan-23.5/src/neapolitan/templates/neapolitan/object_form.html
+-rw-r--r--   0        0        0      259 2023-04-11 13:59:14.152085 neapolitan-23.5/src/neapolitan/templates/neapolitan/object_list.html
+-rw-r--r--   0        0        0      131 2023-01-30 15:27:46.386717 neapolitan-23.5/src/neapolitan/templates/neapolitan/partial/detail.html
+-rw-r--r--   0        0        0      313 2023-01-30 19:42:10.115831 neapolitan-23.5/src/neapolitan/templates/neapolitan/partial/list.html
+-rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.5/src/neapolitan/templatetags/__init__.py
+-rw-r--r--   0        0        0     1263 2023-04-08 14:11:26.730590 neapolitan-23.5/src/neapolitan/templatetags/neapolitan.py
+-rw-r--r--   0        0        0    17002 2023-04-11 14:10:32.822513 neapolitan-23.5/src/neapolitan/views.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.5/tests/__init__.py
+-rw-r--r--   0        0        0      840 2023-04-10 09:00:23.657242 neapolitan-23.5/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.5/tests/migrations/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-10 08:59:09.860534 neapolitan-23.5/tests/models.py
+-rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-23.5/tests/settings.py
+-rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-23.5/tests/templates/base.html
+-rw-r--r--   0        0        0     3972 2023-04-11 13:56:54.581398 neapolitan-23.5/tests/tests.py
+-rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 neapolitan-23.5/PKG-INFO
```

### Comparing `neapolitan-23.4/LICENSE` & `neapolitan-23.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neapolitan-23.4/README.rst` & `neapolitan-23.5/src/neapolitan/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-==========
+"""
 Neapolitan
-==========
 
 I have a Django model::
 
     from django.db import models
 
     class Bookmark(models.Model):
         url = models.URLField(unique=True)
@@ -19,18 +18,21 @@
     class BookmarkView(CRUDView):
         model = Bookmark
         fields = ["url", "title", "note"]
 
 
     urlpatterns = [ ... ] + BookmarkView.get_urls()
 
-Neapolitan's ``CRUDView`` provides the standard list, detail,
+Neapolitan's `CRUDView` provides the standard list, detail,
 create, edit, and delete views for a model, as well as the hooks you need to
 be able to customise any part of that.
 
 Neapolitan provides base templates and re-usable template tags to make getting
 your model on the page as easy as possible.
 
 Where you take your app after that is up to you. But Neapolitan will get you
 started.
 
 Let's go! 🚀
+"""
+
+__version__ = "23.5"
```

### Comparing `neapolitan-23.4/docs/Makefile` & `neapolitan-23.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `neapolitan-23.4/docs/make.bat` & `neapolitan-23.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `neapolitan-23.4/docs/source/conf.py` & `neapolitan-23.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.4/docs/source/index.rst` & `neapolitan-23.5/docs/source/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -30,18 +30,21 @@
 Neapolitan provides base templates and re-usable template tags to make getting
 your model on the page as easy as possible.
 
 Where you take your app after that is up to you. But Neapolitan will get you
 started.
 
 Let's go! 🚀
-..
-   .. toctree::
-      :maxdepth: 2
-      :caption: Contents:
+
+
+.. toctree::
+    :maxdepth: 1
+    :caption: Contents:
+
+    crud-view
 
 ..
    Indices and tables
    ==================
 
    * :ref:`genindex`
    * :ref:`modindex`
```

### Comparing `neapolitan-23.4/pyproject.toml` & `neapolitan-23.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neapolitan-23.4/src/neapolitan/__init__.py` & `neapolitan-23.5/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,65 @@
-"""
+==========
 Neapolitan
+==========
 
 I have a Django model::
 
     from django.db import models
 
     class Bookmark(models.Model):
         url = models.URLField(unique=True)
         title = models.CharField(max_length=255)
         note = models.TextField(blank=True)
+        favourite = models.BooleanField(default=False)
 
 I want easy CRUD views for it, without it taking all day::
 
     # urls.py
     from neapolitan.views import CRUDView
 
     class BookmarkView(CRUDView):
         model = Bookmark
         fields = ["url", "title", "note"]
-
+        filterset_fields = [
+            "favourite",
+        ]
 
     urlpatterns = [ ... ] + BookmarkView.get_urls()
 
-Neapolitan's `CRUDView` provides the standard list, detail,
+Neapolitan's ``CRUDView`` provides the standard list, detail,
 create, edit, and delete views for a model, as well as the hooks you need to
 be able to customise any part of that.
 
 Neapolitan provides base templates and re-usable template tags to make getting
 your model on the page as easy as possible.
 
 Where you take your app after that is up to you. But Neapolitan will get you
 started.
 
 Let's go! 🚀
-"""
 
-__version__ = "23.4"
+Status
+------
+
+This is alpha software. I'm still working out the details of the API, and I've
+not written the docs.
+
+**But**: You could just read `neapolitan.views.CRUDView` and see what it does.
+Up to you. 😜
+
+Installation
+------------
+
+Install with pip::
+
+    pip install neapolitan
+
+Add ``neapolitan`` to your ``INSTALLED_APPS``::
+
+    INSTALLED_APPS = [
+        ...
+        "neapolitan",
+    ]
+
+Templates expect a ``base.html`` template to exist and for that to defined a
+``content`` block. (Refs <https://github.com/carltongibson/neapolitan/issues/6>.)
```

### Comparing `neapolitan-23.4/src/neapolitan/templatetags/neapolitan.py` & `neapolitan-23.5/src/neapolitan/templatetags/neapolitan.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.4/src/neapolitan/views.py` & `neapolitan-23.5/src/neapolitan/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,23 +232,26 @@
     def get_context_data(self, **kwargs):
         """
         Returns a dictionary to use as the context of the response.
 
         Takes a set of keyword arguments to use as the base context,
         and adds the following keys:
 
-        * 'view'
-        * 'object_verbose_name' and 'object_verbose_name_plural'
-        * Optionally, 'object' or 'object_list'
-        * Optionally, '{context_object_name}' or '{context_object_name}_list'
+        * ``view``: A reference to the view object itself.
+        * The ``object_verbose_name`` and ``object_verbose_name_plural`` of the
+          model.
+        * ``object`` or ``object_list``: The object or list of objects being
+          displayed, plus more user-friendly versions using the model, such as
+          ``bookmark`` or ``bookmark_list``.
+        * ``create_view_url``: The URL of the create view
         """
         kwargs["view"] = self
         kwargs["object_verbose_name"] = self.model._meta.verbose_name
         kwargs["object_verbose_name_plural"] = self.model._meta.verbose_name_plural
-        kwargs["create_view_name"] = f"{self.model._meta.model_name}-create"
+        kwargs["create_view_url"] = reverse(f"{self.model._meta.model_name}-create")
 
         if getattr(self, "object", None) is not None:
             kwargs["object"] = self.object
             context_object_name = self.get_context_object_name()
             if context_object_name:
                 kwargs[context_object_name] = self.object
```

### Comparing `neapolitan-23.4/tests/migrations/0001_initial.py` & `neapolitan-23.5/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.4/tests/settings.py` & `neapolitan-23.5/tests/settings.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.4/tests/tests.py` & `neapolitan-23.5/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 
     def test_list(self):
         response = self.client.get("/bookmark/")
         self.assertEqual(response.status_code, 200)
         self.assertContains(response, self.homepage.title)
         self.assertContains(response, self.github.title)
         self.assertContains(response, self.fosstodon.title)
+        self.assertContains(
+            response, '<a href="/bookmark/new/">Add a new bookmark</a>', html=True
+        )
 
     def test_detail(self):
         response = self.client.get(f"/bookmark/{self.homepage.pk}/")
         self.assertEqual(response.status_code, 200)
         self.assertContains(response, self.homepage.title)
         self.assertContains(response, escape(self.homepage.note))
```

