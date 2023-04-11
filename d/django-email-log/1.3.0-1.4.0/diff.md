# Comparing `tmp/django-email-log-1.3.0.tar.gz` & `tmp/django-email-log-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-email-log-1.3.0.tar", last modified: Thu Feb 16 15:34:57 2023, max compression
+gzip compressed data, was "dist\django-email-log-1.4.0.tar", last modified: Tue Apr 11 08:32:30 2023, max compression
```

## Comparing `django-email-log-1.3.0.tar` & `django-email-log-1.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2023-02-16 15:34:57.568572 django-email-log-1.3.0/
--rw-rw-r--   0 trey      (1001) trey      (1001)      273 2023-02-16 15:31:04.000000 django-email-log-1.3.0/AUTHORS.rst
--rw-rw-r--   0 trey      (1001) trey      (1001)     1282 2023-02-16 15:31:40.000000 django-email-log-1.3.0/CHANGES.rst
--rw-rw-r--   0 trey      (1001) trey      (1001)     1992 2022-02-07 18:38:42.000000 django-email-log-1.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 trey      (1001) trey      (1001)     1084 2022-01-27 19:27:50.000000 django-email-log-1.3.0/LICENSE
--rw-rw-r--   0 trey      (1001) trey      (1001)       77 2022-01-27 19:27:50.000000 django-email-log-1.3.0/MANIFEST.in
--rw-rw-r--   0 trey      (1001) trey      (1001)     4450 2023-02-16 15:34:57.568572 django-email-log-1.3.0/PKG-INFO
--rw-rw-r--   0 trey      (1001) trey      (1001)     2080 2023-02-16 15:31:04.000000 django-email-log-1.3.0/README.rst
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2023-02-16 15:34:57.568572 django-email-log-1.3.0/django_email_log.egg-info/
--rw-rw-r--   0 trey      (1001) trey      (1001)     4450 2023-02-16 15:34:57.000000 django-email-log-1.3.0/django_email_log.egg-info/PKG-INFO
--rw-rw-r--   0 trey      (1001) trey      (1001)      723 2023-02-16 15:34:57.000000 django-email-log-1.3.0/django_email_log.egg-info/SOURCES.txt
--rw-rw-r--   0 trey      (1001) trey      (1001)        1 2023-02-16 15:34:57.000000 django-email-log-1.3.0/django_email_log.egg-info/dependency_links.txt
--rw-rw-r--   0 trey      (1001) trey      (1001)       14 2023-02-16 15:34:57.000000 django-email-log-1.3.0/django_email_log.egg-info/requires.txt
--rw-rw-r--   0 trey      (1001) trey      (1001)       10 2023-02-16 15:34:57.000000 django-email-log-1.3.0/django_email_log.egg-info/top_level.txt
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2023-02-16 15:34:57.568572 django-email-log-1.3.0/docs/
--rw-rw-r--   0 trey      (1001) trey      (1001)      756 2022-01-27 19:27:50.000000 django-email-log-1.3.0/docs/index.rst
--rw-rw-r--   0 trey      (1001) trey      (1001)     1594 2023-02-16 15:31:04.000000 django-email-log-1.3.0/docs/usage.rst
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2023-02-16 15:34:57.568572 django-email-log-1.3.0/email_log/
--rw-rw-r--   0 trey      (1001) trey      (1001)       77 2023-02-16 15:31:04.000000 django-email-log-1.3.0/email_log/__init__.py
--rw-rw-r--   0 trey      (1001) trey      (1001)     1382 2023-02-16 15:31:04.000000 django-email-log-1.3.0/email_log/admin.py
--rw-rw-r--   0 trey      (1001) trey      (1001)      177 2022-02-07 18:38:42.000000 django-email-log-1.3.0/email_log/apps.py
--rw-rw-r--   0 trey      (1001) trey      (1001)     3864 2023-02-16 15:31:04.000000 django-email-log-1.3.0/email_log/backends.py
--rw-rw-r--   0 trey      (1001) trey      (1001)      494 2022-01-27 19:27:50.000000 django-email-log-1.3.0/email_log/conf.py
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2023-02-16 15:34:57.568572 django-email-log-1.3.0/email_log/migrations/
--rw-rw-r--   0 trey      (1001) trey      (1001)     1463 2022-02-07 18:38:42.000000 django-email-log-1.3.0/email_log/migrations/0001_initial.py
--rw-rw-r--   0 trey      (1001) trey      (1001)      590 2022-02-07 18:38:42.000000 django-email-log-1.3.0/email_log/migrations/0002_email.py
--rw-rw-r--   0 trey      (1001) trey      (1001)     1693 2023-02-16 15:31:04.000000 django-email-log-1.3.0/email_log/migrations/0003_email_html_message_attachment.py
--rw-rw-r--   0 trey      (1001) trey      (1001)        0 2022-01-27 19:27:50.000000 django-email-log-1.3.0/email_log/migrations/__init__.py
--rw-rw-r--   0 trey      (1001) trey      (1001)     1376 2023-02-16 15:31:04.000000 django-email-log-1.3.0/email_log/models.py
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2023-02-16 15:34:57.568572 django-email-log-1.3.0/email_log/tests/
--rw-rw-r--   0 trey      (1001) trey      (1001)        0 2022-01-27 19:27:50.000000 django-email-log-1.3.0/email_log/tests/__init__.py
--rw-rw-r--   0 trey      (1001) trey      (1001)      417 2022-01-27 19:27:50.000000 django-email-log-1.3.0/email_log/tests/backends.py
--rw-rw-r--   0 trey      (1001) trey      (1001)        0 2022-01-27 19:27:50.000000 django-email-log-1.3.0/email_log/tests/models.py
--rw-rw-r--   0 trey      (1001) trey      (1001)    12891 2023-02-16 15:31:04.000000 django-email-log-1.3.0/email_log/tests/tests.py
--rw-rw-r--   0 trey      (1001) trey      (1001)      141 2022-02-07 18:38:42.000000 django-email-log-1.3.0/email_log/tests/urls.py
--rw-rw-r--   0 trey      (1001) trey      (1001)       38 2023-02-16 15:34:57.568572 django-email-log-1.3.0/setup.cfg
--rw-rw-r--   0 trey      (1001) trey      (1001)     1478 2023-02-16 15:31:04.000000 django-email-log-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:32:30.911181 django-email-log-1.4.0/
+-rw-rw-rw-   0        0        0      273 2023-04-11 08:29:42.000000 django-email-log-1.4.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1417 2023-04-11 08:30:48.000000 django-email-log-1.4.0/CHANGES.rst
+-rw-rw-rw-   0        0        0     1992 2023-01-30 08:18:42.000000 django-email-log-1.4.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       77 2022-01-17 12:14:50.000000 django-email-log-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5716 2023-04-11 08:32:30.910184 django-email-log-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2080 2023-04-11 08:30:48.000000 django-email-log-1.4.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 08:32:30.765328 django-email-log-1.4.0/django_email_log.egg-info/
+-rw-rw-rw-   0        0        0     5716 2023-04-11 08:32:30.000000 django-email-log-1.4.0/django_email_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      766 2023-04-11 08:32:30.000000 django-email-log-1.4.0/django_email_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 08:32:30.000000 django-email-log-1.4.0/django_email_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-11 08:32:30.000000 django-email-log-1.4.0/django_email_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-11 08:32:30.000000 django-email-log-1.4.0/django_email_log.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 08:32:30.785523 django-email-log-1.4.0/docs/
+-rw-rw-rw-   0        0        0      756 2022-01-17 12:14:50.000000 django-email-log-1.4.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1895 2023-04-11 08:29:42.000000 django-email-log-1.4.0/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 08:32:30.835489 django-email-log-1.4.0/email_log/
+-rw-rw-rw-   0        0        0       77 2023-04-11 08:30:48.000000 django-email-log-1.4.0/email_log/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-02-16 09:25:45.000000 django-email-log-1.4.0/email_log/admin.py
+-rw-rw-rw-   0        0        0      177 2023-01-30 08:18:42.000000 django-email-log-1.4.0/email_log/apps.py
+-rw-rw-rw-   0        0        0     3583 2023-04-11 08:29:42.000000 django-email-log-1.4.0/email_log/backends.py
+-rw-rw-rw-   0        0        0      577 2023-04-11 08:29:42.000000 django-email-log-1.4.0/email_log/conf.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:32:30.873418 django-email-log-1.4.0/email_log/migrations/
+-rw-rw-rw-   0        0        0     1463 2023-01-30 08:18:42.000000 django-email-log-1.4.0/email_log/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      590 2023-01-30 08:18:42.000000 django-email-log-1.4.0/email_log/migrations/0002_email.py
+-rw-rw-rw-   0        0        0     1693 2023-02-16 09:25:45.000000 django-email-log-1.4.0/email_log/migrations/0003_email_html_message_attachment.py
+-rw-rw-rw-   0        0        0      509 2023-04-11 08:29:42.000000 django-email-log-1.4.0/email_log/migrations/0004_alter_attachment_file.py
+-rw-rw-rw-   0        0        0        0 2022-01-17 12:14:50.000000 django-email-log-1.4.0/email_log/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1875 2023-04-11 08:29:42.000000 django-email-log-1.4.0/email_log/models.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:32:30.907182 django-email-log-1.4.0/email_log/tests/
+-rw-rw-rw-   0        0        0        0 2022-01-17 12:14:50.000000 django-email-log-1.4.0/email_log/tests/__init__.py
+-rw-rw-rw-   0        0        0      417 2022-01-17 12:14:50.000000 django-email-log-1.4.0/email_log/tests/backends.py
+-rw-rw-rw-   0        0        0        0 2022-01-17 12:14:50.000000 django-email-log-1.4.0/email_log/tests/models.py
+-rw-rw-rw-   0        0        0    13236 2023-04-11 08:29:42.000000 django-email-log-1.4.0/email_log/tests/tests.py
+-rw-rw-rw-   0        0        0      141 2023-01-30 08:18:42.000000 django-email-log-1.4.0/email_log/tests/urls.py
+-rw-rw-rw-   0        0        0       42 2023-04-11 08:32:30.912184 django-email-log-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1516 2023-04-11 08:30:48.000000 django-email-log-1.4.0/setup.py
```

### Comparing `django-email-log-1.3.0/CHANGES.rst` & `django-email-log-1.4.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+1.4.0 (2023-04-06)
+------------------
+
+- Added ability to assign callable to `EMAIL_LOG_ATTACHMENTS_PATH`
+- Added Django 4.2 support
+
+
 1.3.0 (2023-02-10)
 ------------------
 
 - Added Django 4.1 support
 - Remove Python 3.6 support
 - Add saving of e-mail attachemnts to database
 - Add saving of html alternatives to database
```

### Comparing `django-email-log-1.3.0/CONTRIBUTING.rst` & `django-email-log-1.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-email-log-1.3.0/README.rst` & `django-email-log-1.4.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
    :alt: Tests
 .. image:: https://codecov.io/gh/treyhunner/django-email-log/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/treyhunner/django-email-log
    :alt: Codecov
 
 Django email backend that logs all sent emails to a database using a Django model.
 
-This app works with Django 2.2 to 4.1
+This app works with Django 2.2 to 4.2
 
 This app requires Python 3.7+.
 
 Getting Help
 ------------
 
 Documentation for django-email-log is available at https://django-email-log.readthedocs.org/
```

### Comparing `django-email-log-1.3.0/django_email_log.egg-info/SOURCES.txt` & `django-email-log-1.4.0/django_email_log.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 AUTHORS.rst
 CHANGES.rst
 CONTRIBUTING.rst
-LICENSE
 MANIFEST.in
 README.rst
 setup.py
 django_email_log.egg-info/PKG-INFO
 django_email_log.egg-info/SOURCES.txt
 django_email_log.egg-info/dependency_links.txt
 django_email_log.egg-info/requires.txt
@@ -17,13 +16,14 @@
 email_log/apps.py
 email_log/backends.py
 email_log/conf.py
 email_log/models.py
 email_log/migrations/0001_initial.py
 email_log/migrations/0002_email.py
 email_log/migrations/0003_email_html_message_attachment.py
+email_log/migrations/0004_alter_attachment_file.py
 email_log/migrations/__init__.py
 email_log/tests/__init__.py
 email_log/tests/backends.py
 email_log/tests/models.py
 email_log/tests/tests.py
 email_log/tests/urls.py
```

### Comparing `django-email-log-1.3.0/docs/index.rst` & `django-email-log-1.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-email-log-1.3.0/docs/usage.rst` & `django-email-log-1.4.0/docs/usage.rst`

 * *Files 22% similar despite different names*

```diff
@@ -40,14 +40,24 @@
 
 And using this setting you can configure path to your attachments:
 
 .. code-block:: python
 
     EMAIL_LOG_ATTACHMENTS_PATH = "path/to/attachments"
 
+Or you can even provide callable object just like for `FileField.upload_to`
+
+.. code-block:: python
+
+    def get_path(instance, filename):
+        date_sent = email.date_sent.strftime('%m-%d-%Y')
+        return f"path/to/attachments/{date_sent}/{filename}"
+
+    EMAIL_LOG_ATTACHMENTS_PATH = get_path
+
 
 
 Using with other email backends
 -------------------------------
 
 By default django-email-log uses Django's SMTP backend to send emails.  The
 ``EMAIL_LOG_BACKEND`` setting should be specified if you are using a custom
```

### Comparing `django-email-log-1.3.0/email_log/admin.py` & `django-email-log-1.4.0/email_log/admin.py`

 * *Files identical despite different names*

### Comparing `django-email-log-1.3.0/email_log/backends.py` & `django-email-log-1.4.0/email_log/backends.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,15 @@
                     html_message=html_message,
                 )
             except Exception:
                 logging.error(
                     "Failed to save email to database (create)", exc_info=True
                 )
 
-            has_setting = hasattr(settings, "EMAIL_LOG_SAVE_ATTACHMENTS")
-            if has_setting and settings.EMAIL_LOG_SAVE_ATTACHMENTS is True:
+            if settings.EMAIL_LOG_SAVE_ATTACHMENTS:
                 self._log_attachments(email, message)
 
             message.connection = self.connection
             num_sent += message.send()
             if num_sent > 0 and email:
                 email.ok = True
                 try:
@@ -77,25 +76,22 @@
                     attachment_files[name].update({"mimetype": type})
 
         if attachment_files:
             self._create_attachments(email, attachment_files)
 
     def _create_attachments(self, email: Email, files: dict):
         """Create attachments and save it to database."""
-        attachment_path = ""
-        if hasattr(settings, "EMAIL_LOG_ATTACHMENTS_PATH"):
-            attachment_path = f"{settings.EMAIL_LOG_ATTACHMENTS_PATH}/"
-
         for filename, filedata in files.items():
             content = filedata.get("file", None)
             mimetype = filedata.get("mimetype", None)
-
             attachment = Attachment()
-            if mimetype:
-                attachment.mimetype = mimetype
+
             attachment.name = filename
             attachment.email = email
+            if mimetype:
+                attachment.mimetype = mimetype
+
             attachment.file.save(
-                f"{attachment_path}{filename}",
+                filename,
                 content=content,
                 save=True,
             )
```

### Comparing `django-email-log-1.3.0/email_log/migrations/0001_initial.py` & `django-email-log-1.4.0/email_log/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-email-log-1.3.0/email_log/migrations/0002_email.py` & `django-email-log-1.4.0/email_log/migrations/0002_email.py`

 * *Files identical despite different names*

### Comparing `django-email-log-1.3.0/email_log/migrations/0003_email_html_message_attachment.py` & `django-email-log-1.4.0/email_log/migrations/0003_email_html_message_attachment.py`

 * *Files identical despite different names*

### Comparing `django-email-log-1.3.0/email_log/tests/tests.py` & `django-email-log-1.4.0/email_log/tests/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,14 +81,19 @@
 
 @override_settings(EMAIL_BACKEND="email_log.backends.EmailBackend")
 class EmailBackendTests(TestCase):
     @classmethod
     def setUpClass(cls):
         # Create test folder
         os.mkdir(ATTACHMENTS_TEST_FOLDER)
+        cls.attachment_data = {
+            "filename": "test.txt",
+            "content": b"test",
+            "mimetype": "text/plain",
+        }
         return super().setUpClass()
 
     @classmethod
     def tearDownClass(cls):
         # Remove test folder
         shutil.rmtree(ATTACHMENTS_TEST_FOLDER)
         return super().tearDownClass()
@@ -155,25 +160,31 @@
     @override_settings(EMAIL_LOG_SAVE_ATTACHMENTS=True)
     def test_send_messages_with_attachment(self):
         attachment_data = {
             "filename": f"{ATTACHMENTS_TEST_FOLDER}/test.txt",
             "content": b"test",
             "mimetype": "text/plain",
         }
-        self.assertAttachmentOK(attachment_data, expected_data=attachment_data)
+        self.assertAttachmentOK(attachment_data)
 
-    @override_settings(EMAIL_LOG_ATTACHMENTS_PATH=ATTACHMENTS_TEST_FOLDER)
-    @override_settings(EMAIL_LOG_SAVE_ATTACHMENTS=True)
+    @override_settings(
+        EMAIL_LOG_SAVE_ATTACHMENTS=True,
+        EMAIL_LOG_ATTACHMENTS_PATH=ATTACHMENTS_TEST_FOLDER,
+    )
     def test_send_messages_with_attachment_with_path_specified(self):
-        attachment_data = {
-            "filename": "test.txt",
-            "content": b"test",
-            "mimetype": "text/plain",
-        }
-        self.assertAttachmentOK(attachment_data, expected_data=attachment_data)
+        self.assertAttachmentOK(self.attachment_data)
+
+    @override_settings(
+        EMAIL_LOG_ATTACHMENTS_PATH=(
+            lambda email, name: f"{ATTACHMENTS_TEST_FOLDER}/{name}"
+        )
+    )
+    @override_settings(EMAIL_LOG_SAVE_ATTACHMENTS=True)
+    def test_send_messages_with_attachments_path_callable_specified(self):
+        self.assertAttachmentOK(self.attachment_data)
 
     @override_settings(EMAIL_LOG_SAVE_ATTACHMENTS=True)
     def test_send_messages_with_mime_base_attachment(self):
         mime_base_message = MIMEText("Test message")
         mime_base_message.add_header(
             "Content-ID",
             f"{ATTACHMENTS_TEST_FOLDER}/<{{test.txt}}>",
@@ -186,23 +197,23 @@
         attachment_data = {
             "filename": mime_base_message,
         }
         expected_data = {
             "filename": f"{ATTACHMENTS_TEST_FOLDER}/test.txt",
             "content": b"Test message",
         }
-        self.assertAttachmentOK(attachment_data, expected_data)
+        self.assertAttachmentOK(attachment_data, expected_data=expected_data)
 
     @override_settings(EMAIL_LOG_SAVE_ATTACHMENTS=True)
     def test_send_messages_with_attachment_without_type(self):
         attachment_data = {
             "filename": f"{ATTACHMENTS_TEST_FOLDER}/test",
             "content": b"test",
         }
-        self.assertAttachmentOK(attachment_data, expected_data=attachment_data)
+        self.assertAttachmentOK(attachment_data)
 
     def test_send_html_message(self):
         html_message = "<strong>Test html</strong><br>"
         args = {
             **self.plain_args,
             "to": self.plain_args["recipients"],
         }
@@ -291,15 +302,18 @@
         self.assertEqual(email.recipients, self.plain_args["recipients"][0])
         self.assertSequenceEqual(mail.outbox[0].to, self.plain_args["recipients"])
         for message in (email, mail.outbox[0]):
             self.assertEqual(message.from_email, self.plain_args["from_email"])
             self.assertEqual(message.subject, self.plain_args["subject"])
             self.assertEqual(message.body, self.plain_args["body"])
 
-    def assertAttachmentOK(self, attachment_data: dict, expected_data):
+    def assertAttachmentOK(self, attachment_data: dict, expected_data=None):
+        if expected_data is None:
+            expected_data = attachment_data
+
         number_of_attachments = self.get_number_of_test_files()
         sent = self.send_mail_with_attachment(attachment_data)
 
         self.assertEqual(sent, 1)
         self.assertEqual(len(mail.outbox), 1)
         self.assertEqual(self.get_number_of_test_files(), number_of_attachments + 1)
```

### Comparing `django-email-log-1.3.0/setup.py` & `django-email-log-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,12 +33,13 @@
         "Programming Language :: Python :: 3.10",
         "Framework :: Django",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
     ],
     tests_require=["Django >= 2.2.0"],
     include_package_data=True,
     test_suite="runtests.runtests",
 )
```

