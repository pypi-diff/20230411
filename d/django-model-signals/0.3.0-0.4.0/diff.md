# Comparing `tmp/django_model_signals-0.3.0.tar.gz` & `tmp/django_model_signals-0.4.0.tar.gz`

## Comparing `django_model_signals-0.3.0.tar` & `django_model_signals-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 django_model_signals-0.3.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_model_signals-0.3.0/django_model_signals/__init__.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_model_signals-0.3.0/django_model_signals/apps.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 django_model_signals-0.3.0/django_model_signals/dispatcher.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 django_model_signals-0.3.0/django_model_signals/manager.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 django_model_signals-0.3.0/django_model_signals/signals.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 django_model_signals-0.3.0/django_model_signals/transceiver.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 django_model_signals-0.3.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 django_model_signals-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 django_model_signals-0.3.0/README.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 django_model_signals-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 django_model_signals-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/django_model_signals/__init__.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/django_model_signals/apps.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/django_model_signals/dispatcher.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/django_model_signals/manager.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/django_model_signals/signals.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/django_model_signals/transceiver.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/README.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/PKG-INFO
```

### Comparing `django_model_signals-0.3.0/.github/workflows/publish-to-pypi.yml` & `django_model_signals-0.4.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.3.0/django_model_signals/apps.py` & `django_model_signals-0.4.0/django_model_signals/apps.py`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.3.0/django_model_signals/dispatcher.py` & `django_model_signals-0.4.0/django_model_signals/dispatcher.py`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.3.0/django_model_signals/manager.py` & `django_model_signals-0.4.0/django_model_signals/manager.py`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.3.0/django_model_signals/signals.py` & `django_model_signals-0.4.0/django_model_signals/signals.py`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.3.0/LICENSE.md` & `django_model_signals-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.3.0/README.md` & `django_model_signals-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -50,20 +50,26 @@
 
     def pre_full_clean(self, **kwargs):
         pass
 
     def post_full_clean(self, **kwargs):
         pass
 
+    def post_full_clean_error(self, **kwargs):
+        raise kwargs['error']
+
     def pre_save(self, **kwargs):
         pass
 
     def post_save(self, **kwargs):
         pass
 
+    def post_save_error(self, **kwargs):
+        raise kwargs['error']
+
     def pre_delete(self, **kwargs):
         pass
 
     def post_delete(self, **kwargs):
         pass
 
     def m2m_changed(self, **kwargs):
@@ -94,27 +100,39 @@
             'post_bulk_save'
         ]
 ```
 
 ## Notes
 
 - The following actions are supported for triggering the implemented signals:
-  - Creating or loading an model instance from the database will trigger the `pre_init` and `post_init` signals.
-  - Calling `Model.full_clean` will trigger the `pre_full_clean` and `post_full_clean` signals.
+  - Creating or loading an model instance from the database will trigger the
+    `pre_init` and `post_init` signals.
+  - Calling `Model.full_clean` will trigger the `pre_full_clean` and
+    `post_full_clean` signals.
+  - An error during `Model.full_clean` will trigger the `post_full_clean_error`
+    signal.
   - Calling `Model.save` will trigger the `pre_save` and `post_save` signals.
-  - Calling `Model.delete` will trigger the `pre_delete` and `post_delete` signals.
-  - Calling `Model.objects.create` will trigger the `pre_save` and `post_save` signals.
-  - Calling `Model.objects.get_or_create` will trigger the `pre_save` and `post_save` signals.
-  - Calling `Model.objects.update_or_create` will trigger the `pre_save` and `post_save` signals.
-  - Calling `Model.objects.bulk_create` will trigger the `pre_bulk_save` and `post_bulk_save` signals.
-  - Calling `Model.objects.bulk_update` will trigger the `pre_bulk_save` and `post_bulk_save` signals.
-  - Calling `QuerySet.delete` will trigger the `pre_delete` and `post_delete` signals.
-
-- To implement the `pre_full_clean` and `post_full_clean` signals, this library
-  overrides the `full_clean` method of Django models and calls the original
-  method in a backwards compatible way. However, make sure the order of the
-  classes inherited from is the same as the above example to ensure the proper
-  method resolution order.
+  - An error during `Model.save` will trigger the `post_save_error` signal.
+  - Calling `Model.delete` will trigger the `pre_delete` and `post_delete`
+    signals.
+  - Calling `Model.objects.create` will trigger the `pre_save` and `post_save`
+    signals.
+  - Calling `Model.objects.get_or_create` will trigger the `pre_save` and
+    `post_save` signals.
+  - Calling `Model.objects.update_or_create` will trigger the `pre_save` and
+    `post_save` signals.
+  - Calling `Model.objects.bulk_create` will trigger the `pre_bulk_save` and
+    `post_bulk_save` signals.
+  - Calling `Model.objects.bulk_update` will trigger the `pre_bulk_save` and
+    `post_bulk_save` signals.
+  - Calling `QuerySet.delete` will trigger the `pre_delete` and `post_delete`
+    signals.
+- To implement the `pre_full_clean` and `post_full_clean`,
+  `post_full_clean_error` and `post_save_errors` signals, this library
+  overrides the `full_clean` and `save` methods of Django models and calls the
+  original method in a backwards compatible way. However, make sure the order
+  of the classes inherited from is the same as the above example to ensure the
+  proper method resolution order.
 
 ## Resources
 
 - Django: https://www.djangoproject.com/
```

### Comparing `django_model_signals-0.3.0/pyproject.toml` & `django_model_signals-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-model-signals"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="Digital Valley", email="techteam@digitalvalley.nl" }
 ]
 description = "Django Model Signals makes it easier to keep model related business logic in your Django models by allowing them to become transceivers of their own signals, including bulk signals."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django_model_signals-0.3.0/PKG-INFO` & `django_model_signals-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-signals
-Version: 0.3.0
+Version: 0.4.0
 Summary: Django Model Signals makes it easier to keep model related business logic in your Django models by allowing them to become transceivers of their own signals, including bulk signals.
 Author-email: Digital Valley <techteam@digitalvalley.nl>
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -64,20 +64,26 @@
 
     def pre_full_clean(self, **kwargs):
         pass
 
     def post_full_clean(self, **kwargs):
         pass
 
+    def post_full_clean_error(self, **kwargs):
+        raise kwargs['error']
+
     def pre_save(self, **kwargs):
         pass
 
     def post_save(self, **kwargs):
         pass
 
+    def post_save_error(self, **kwargs):
+        raise kwargs['error']
+
     def pre_delete(self, **kwargs):
         pass
 
     def post_delete(self, **kwargs):
         pass
 
     def m2m_changed(self, **kwargs):
@@ -108,27 +114,39 @@
             'post_bulk_save'
         ]
 ```
 
 ## Notes
 
 - The following actions are supported for triggering the implemented signals:
-  - Creating or loading an model instance from the database will trigger the `pre_init` and `post_init` signals.
-  - Calling `Model.full_clean` will trigger the `pre_full_clean` and `post_full_clean` signals.
+  - Creating or loading an model instance from the database will trigger the
+    `pre_init` and `post_init` signals.
+  - Calling `Model.full_clean` will trigger the `pre_full_clean` and
+    `post_full_clean` signals.
+  - An error during `Model.full_clean` will trigger the `post_full_clean_error`
+    signal.
   - Calling `Model.save` will trigger the `pre_save` and `post_save` signals.
-  - Calling `Model.delete` will trigger the `pre_delete` and `post_delete` signals.
-  - Calling `Model.objects.create` will trigger the `pre_save` and `post_save` signals.
-  - Calling `Model.objects.get_or_create` will trigger the `pre_save` and `post_save` signals.
-  - Calling `Model.objects.update_or_create` will trigger the `pre_save` and `post_save` signals.
-  - Calling `Model.objects.bulk_create` will trigger the `pre_bulk_save` and `post_bulk_save` signals.
-  - Calling `Model.objects.bulk_update` will trigger the `pre_bulk_save` and `post_bulk_save` signals.
-  - Calling `QuerySet.delete` will trigger the `pre_delete` and `post_delete` signals.
-
-- To implement the `pre_full_clean` and `post_full_clean` signals, this library
-  overrides the `full_clean` method of Django models and calls the original
-  method in a backwards compatible way. However, make sure the order of the
-  classes inherited from is the same as the above example to ensure the proper
-  method resolution order.
+  - An error during `Model.save` will trigger the `post_save_error` signal.
+  - Calling `Model.delete` will trigger the `pre_delete` and `post_delete`
+    signals.
+  - Calling `Model.objects.create` will trigger the `pre_save` and `post_save`
+    signals.
+  - Calling `Model.objects.get_or_create` will trigger the `pre_save` and
+    `post_save` signals.
+  - Calling `Model.objects.update_or_create` will trigger the `pre_save` and
+    `post_save` signals.
+  - Calling `Model.objects.bulk_create` will trigger the `pre_bulk_save` and
+    `post_bulk_save` signals.
+  - Calling `Model.objects.bulk_update` will trigger the `pre_bulk_save` and
+    `post_bulk_save` signals.
+  - Calling `QuerySet.delete` will trigger the `pre_delete` and `post_delete`
+    signals.
+- To implement the `pre_full_clean` and `post_full_clean`,
+  `post_full_clean_error` and `post_save_errors` signals, this library
+  overrides the `full_clean` and `save` methods of Django models and calls the
+  original method in a backwards compatible way. However, make sure the order
+  of the classes inherited from is the same as the above example to ensure the
+  proper method resolution order.
 
 ## Resources
 
 - Django: https://www.djangoproject.com/
```

