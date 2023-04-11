# Comparing `tmp/doveseed-1.1.0a6.tar.gz` & `tmp/doveseed-1.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doveseed-1.1.0a6.tar", max compression
+gzip compressed data, was "doveseed-1.1.0a7.tar", max compression
```

## Comparing `doveseed-1.1.0a6.tar` & `doveseed-1.1.0a7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1068 2023-03-05 13:07:37.994837 doveseed-1.1.0a6/LICENSE
--rw-r--r--   0        0        0     6426 2023-03-05 13:07:37.994837 doveseed-1.1.0a6/README.rst
--rw-r--r--   0        0        0       22 2023-03-05 13:07:37.994837 doveseed-1.1.0a6/doveseed/__init__.py
--rw-r--r--   0        0        0     3313 2023-03-05 13:07:37.998838 doveseed-1.1.0a6/doveseed/app.py
--rw-r--r--   0        0        0     2163 2023-03-05 13:07:37.998838 doveseed-1.1.0a6/doveseed/cli.py
--rw-r--r--   0        0        0      932 2023-03-05 13:07:37.998838 doveseed-1.1.0a6/doveseed/confirmation.py
--rw-r--r--   0        0        0      765 2023-03-05 13:07:37.998838 doveseed-1.1.0a6/doveseed/domain_types.py
--rw-r--r--   0        0        0     1128 2023-03-05 13:07:37.998838 doveseed-1.1.0a6/doveseed/email_notification.py
--rw-r--r--   0        0        0     3060 2023-03-05 13:07:37.998838 doveseed-1.1.0a6/doveseed/email_templating.py
--rw-r--r--   0        0        0     1289 2023-03-05 13:07:37.998838 doveseed-1.1.0a6/doveseed/feed.py
--rw-r--r--   0        0        0     1287 2023-03-05 13:07:37.998838 doveseed-1.1.0a6/doveseed/notifier.py
--rw-r--r--   0        0        0     2173 2023-03-05 13:07:37.998838 doveseed-1.1.0a6/doveseed/recaptcha.py
--rw-r--r--   0        0        0     3843 2023-03-05 13:07:37.998838 doveseed-1.1.0a6/doveseed/registration.py
--rw-r--r--   0        0        0     2047 2023-03-05 13:07:37.998838 doveseed-1.1.0a6/doveseed/smtp.py
--rw-r--r--   0        0        0     3976 2023-03-05 13:07:37.998838 doveseed-1.1.0a6/doveseed/storage.py
--rw-r--r--   0        0        0      121 2023-03-05 13:07:37.998838 doveseed-1.1.0a6/doveseed/token_gen.py
--rw-r--r--   0        0        0     1059 2023-03-05 13:07:37.998838 doveseed-1.1.0a6/pyproject.toml
--rw-r--r--   0        0        0     7684 1970-01-01 00:00:00.000000 doveseed-1.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/LICENSE
+-rw-r--r--   0        0        0     6426 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/README.rst
+-rw-r--r--   0        0        0       22 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/__init__.py
+-rw-r--r--   0        0        0     3313 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/app.py
+-rw-r--r--   0        0        0     2163 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/cli.py
+-rw-r--r--   0        0        0      932 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/confirmation.py
+-rw-r--r--   0        0        0      765 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/domain_types.py
+-rw-r--r--   0        0        0     1128 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/email_notification.py
+-rw-r--r--   0        0        0     3060 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/email_templating.py
+-rw-r--r--   0        0        0     1289 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/feed.py
+-rw-r--r--   0        0        0     1287 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/notifier.py
+-rw-r--r--   0        0        0     2173 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/recaptcha.py
+-rw-r--r--   0        0        0     3843 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/registration.py
+-rw-r--r--   0        0        0     2047 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/smtp.py
+-rw-r--r--   0        0        0     3976 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/storage.py
+-rw-r--r--   0        0        0      121 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/token_gen.py
+-rw-r--r--   0        0        0     1059 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/pyproject.toml
+-rw-r--r--   0        0        0     7684 1970-01-01 00:00:00.000000 doveseed-1.1.0a7/PKG-INFO
```

### Comparing `doveseed-1.1.0a6/LICENSE` & `doveseed-1.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a6/README.rst` & `doveseed-1.1.0a7/README.rst`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a6/doveseed/app.py` & `doveseed-1.1.0a7/doveseed/app.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a6/doveseed/cli.py` & `doveseed-1.1.0a7/doveseed/cli.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a6/doveseed/confirmation.py` & `doveseed-1.1.0a7/doveseed/confirmation.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a6/doveseed/domain_types.py` & `doveseed-1.1.0a7/doveseed/domain_types.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a6/doveseed/email_notification.py` & `doveseed-1.1.0a7/doveseed/email_notification.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a6/doveseed/email_templating.py` & `doveseed-1.1.0a7/doveseed/email_templating.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a6/doveseed/feed.py` & `doveseed-1.1.0a7/doveseed/feed.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a6/doveseed/notifier.py` & `doveseed-1.1.0a7/doveseed/notifier.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a6/doveseed/recaptcha.py` & `doveseed-1.1.0a7/doveseed/recaptcha.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a6/doveseed/registration.py` & `doveseed-1.1.0a7/doveseed/registration.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a6/doveseed/smtp.py` & `doveseed-1.1.0a7/doveseed/smtp.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a6/doveseed/storage.py` & `doveseed-1.1.0a7/doveseed/storage.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a6/pyproject.toml` & `doveseed-1.1.0a7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 description = "Doveseed is a backend service for email subscriptions to RSS feeds."
 keywords = ["email", "rss", "subscriptions"]
 license = "MIT"
 name = "doveseed"
 readme = "README.rst"
 repository = "https://github.com/jgosmann/doveseed/"
-version = "1.1.0a6"
+version = "1.1.0a7"
 
 [tool.poetry.dependencies]
 Werkzeug = "^2.2.2"
 flask = "^2.2.2"
 flask_cors = "^3.0"
 jinja2 = "^3.1.2"
 python = "^3.7.2"
```

### Comparing `doveseed-1.1.0a6/PKG-INFO` & `doveseed-1.1.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doveseed
-Version: 1.1.0a6
+Version: 1.1.0a7
 Summary: Doveseed is a backend service for email subscriptions to RSS feeds.
 Home-page: https://github.com/jgosmann/doveseed/
 License: MIT
 Keywords: email,rss,subscriptions
 Author: Jan Gosmann
 Author-email: jan@hyper-world.de
 Requires-Python: >=3.7.2,<4.0.0
```

