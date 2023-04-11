# Comparing `tmp/django_browser_reload-1.7.0.tar.gz` & `tmp/django_browser_reload-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_browser_reload-1.7.0.tar", last modified: Sat Feb 25 07:19:49 2023, max compression
+gzip compressed data, was "django_browser_reload-1.8.0.tar", last modified: Tue Apr 11 18:26:02 2023, max compression
```

## Comparing `django_browser_reload-1.7.0.tar` & `django_browser_reload-1.8.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:19:49.605929 django_browser_reload-1.7.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1688 2023-02-25 07:19:42.000000 django_browser_reload-1.7.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:58:23.000000 django_browser_reload-1.7.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      130 2023-01-20 12:09:56.000000 django_browser_reload-1.7.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     9832 2023-02-25 07:19:49.606029 django_browser_reload-1.7.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8425 2023-01-20 11:36:46.000000 django_browser_reload-1.7.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      460 2023-02-15 21:55:44.000000 django_browser_reload-1.7.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1681 2023-02-25 07:19:49.606390 django_browser_reload-1.7.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:19:49.597774 django_browser_reload-1.7.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:19:49.603361 django_browser_reload-1.7.0/src/django_browser_reload/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:28.000000 django_browser_reload-1.7.0/src/django_browser_reload/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      324 2022-06-03 11:58:28.000000 django_browser_reload-1.7.0/src/django_browser_reload/apps.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      646 2022-06-03 11:58:28.000000 django_browser_reload-1.7.0/src/django_browser_reload/jinja.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2770 2022-11-08 22:26:11.000000 django_browser_reload-1.7.0/src/django_browser_reload/middleware.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:28.000000 django_browser_reload-1.7.0/src/django_browser_reload/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:19:49.597891 django_browser_reload-1.7.0/src/django_browser_reload/static/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:19:49.604716 django_browser_reload-1.7.0/src/django_browser_reload/static/django-browser-reload/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      623 2022-06-03 11:58:28.000000 django_browser_reload-1.7.0/src/django_browser_reload/static/django-browser-reload/reload-listener.js
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2711 2022-06-03 11:58:28.000000 django_browser_reload-1.7.0/src/django_browser_reload/static/django-browser-reload/reload-worker.js
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:19:49.605015 django_browser_reload-1.7.0/src/django_browser_reload/templatetags/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:28.000000 django_browser_reload-1.7.0/src/django_browser_reload/templatetags/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      215 2022-11-04 10:25:47.000000 django_browser_reload-1.7.0/src/django_browser_reload/templatetags/django_browser_reload.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      211 2022-11-04 10:25:47.000000 django_browser_reload-1.7.0/src/django_browser_reload/urls.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5020 2022-11-04 10:30:45.000000 django_browser_reload-1.7.0/src/django_browser_reload/views.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:19:49.604380 django_browser_reload-1.7.0/src/django_browser_reload.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     9832 2023-02-25 07:19:49.000000 django_browser_reload-1.7.0/src/django_browser_reload.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      938 2023-02-25 07:19:49.000000 django_browser_reload-1.7.0/src/django_browser_reload.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-02-25 07:19:49.000000 django_browser_reload-1.7.0/src/django_browser_reload.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-02-25 07:19:49.000000 django_browser_reload-1.7.0/src/django_browser_reload.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-02-25 07:19:49.000000 django_browser_reload-1.7.0/src/django_browser_reload.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       22 2023-02-25 07:19:49.000000 django_browser_reload-1.7.0/src/django_browser_reload.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:19:49.605779 django_browser_reload-1.7.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      781 2022-11-04 10:30:45.000000 django_browser_reload-1.7.0/tests/test_jinja.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5179 2022-11-04 10:30:45.000000 django_browser_reload-1.7.0/tests/test_middleware.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4107 2022-11-04 10:30:45.000000 django_browser_reload-1.7.0/tests/test_views.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.496020 django_browser_reload-1.8.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1812 2023-04-11 18:25:59.000000 django_browser_reload-1.8.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:58:23.000000 django_browser_reload-1.8.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      130 2023-01-20 12:09:56.000000 django_browser_reload-1.8.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     9832 2023-04-11 18:26:02.496102 django_browser_reload-1.8.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8425 2023-01-20 11:36:46.000000 django_browser_reload-1.8.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      500 2023-02-28 09:05:51.000000 django_browser_reload-1.8.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1681 2023-04-11 18:26:02.496419 django_browser_reload-1.8.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.492169 django_browser_reload-1.8.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.494168 django_browser_reload-1.8.0/src/django_browser_reload/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:28.000000 django_browser_reload-1.8.0/src/django_browser_reload/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      324 2022-06-03 11:58:28.000000 django_browser_reload-1.8.0/src/django_browser_reload/apps.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      646 2022-06-03 11:58:28.000000 django_browser_reload-1.8.0/src/django_browser_reload/jinja.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2770 2022-11-08 22:26:11.000000 django_browser_reload-1.8.0/src/django_browser_reload/middleware.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:28.000000 django_browser_reload-1.8.0/src/django_browser_reload/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.492292 django_browser_reload-1.8.0/src/django_browser_reload/static/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.495281 django_browser_reload-1.8.0/src/django_browser_reload/static/django-browser-reload/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      623 2022-06-03 11:58:28.000000 django_browser_reload-1.8.0/src/django_browser_reload/static/django-browser-reload/reload-listener.js
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2711 2023-04-11 18:15:57.000000 django_browser_reload-1.8.0/src/django_browser_reload/static/django-browser-reload/reload-worker.js
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.495540 django_browser_reload-1.8.0/src/django_browser_reload/templatetags/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:28.000000 django_browser_reload-1.8.0/src/django_browser_reload/templatetags/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      215 2022-11-04 10:25:47.000000 django_browser_reload-1.8.0/src/django_browser_reload/templatetags/django_browser_reload.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      211 2022-11-04 10:25:47.000000 django_browser_reload-1.8.0/src/django_browser_reload/urls.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5141 2023-04-11 18:20:55.000000 django_browser_reload-1.8.0/src/django_browser_reload/views.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.494995 django_browser_reload-1.8.0/src/django_browser_reload.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     9832 2023-04-11 18:26:02.000000 django_browser_reload-1.8.0/src/django_browser_reload.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      938 2023-04-11 18:26:02.000000 django_browser_reload-1.8.0/src/django_browser_reload.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-04-11 18:26:02.000000 django_browser_reload-1.8.0/src/django_browser_reload.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-04-11 18:26:02.000000 django_browser_reload-1.8.0/src/django_browser_reload.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-04-11 18:26:02.000000 django_browser_reload-1.8.0/src/django_browser_reload.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       22 2023-04-11 18:26:02.000000 django_browser_reload-1.8.0/src/django_browser_reload.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-11 18:26:02.495916 django_browser_reload-1.8.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      781 2022-11-04 10:30:45.000000 django_browser_reload-1.8.0/tests/test_jinja.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5179 2022-11-04 10:30:45.000000 django_browser_reload-1.8.0/tests/test_middleware.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5001 2023-04-11 18:20:55.000000 django_browser_reload-1.8.0/tests/test_views.py
```

### Comparing `django_browser_reload-1.7.0/CHANGELOG.rst` & `django_browser_reload-1.8.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+1.8.0 (2023-04-11)
+------------------
+
+* Support use with `GzipMiddleware`, or other middleware that encodes the response.
+
 1.7.0 (2023-02-25)
 ------------------
 
 * Support Django 4.2.
 
 1.6.0 (2022-06-05)
 ------------------
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_1qctnbbl_/tmpvsxm7ueq_TarContainer/0/1.rst", line 69, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_1qctnbbl_/tmpvsxm7ueq_TarContainer/0/1.rst", line 69, column 0: CDATA terminal not found*

```diff
@@ -1,14 +1,16 @@
-========= Changelog ========= 1.7.0 (2023-02-25) ------------------ * Support
-Django 4.2. 1.6.0 (2022-06-05) ------------------ * Support Python 3.11. *
-Support Django 4.1. 1.5.0 (2022-05-18) ------------------ * Add async support
-to the middleware, to reduce overhead on async projects. * Disable middleware
-at Django startup when ``DEBUG`` is ``False``. 1.4.0 (2022-05-10) -------------
------ * Drop support for Django 2.2, 3.0, and 3.1. 1.3.0 (2022-01-13) ---------
---------- * âDebounceâ reload events with a 50 millisecond window. This
-fixes an issue with repeat triggers of the same reload event. It should also
-help workflows where several files change in quick succession. 1.2.0 (2022-01-
-10) ------------------ * Drop Python 3.6 support. 1.1.1 (2022-01-10) ----------
--------- * Prevent restarting the server when static assets change. Thanks to
-Tim Kamanin for the report in `Issue #46
+========= Changelog ========= 1.8.0 (2023-04-11) ------------------ * Support
+use with `GzipMiddleware`, or other middleware that encodes the response. 1.7.0
+(2023-02-25) ------------------ * Support Django 4.2. 1.6.0 (2022-06-05) ------
+------------ * Support Python 3.11. * Support Django 4.1. 1.5.0 (2022-05-18) --
+---------------- * Add async support to the middleware, to reduce overhead on
+async projects. * Disable middleware at Django startup when ``DEBUG`` is
+``False``. 1.4.0 (2022-05-10) ------------------ * Drop support for Django 2.2,
+3.0, and 3.1. 1.3.0 (2022-01-13) ------------------ * âDebounceâ reload
+events with a 50 millisecond window. This fixes an issue with repeat triggers
+of the same reload event. It should also help workflows where several files
+change in quick succession. 1.2.0 (2022-01-10) ------------------ * Drop Python
+3.6 support. 1.1.1 (2022-01-10) ------------------ * Prevent restarting the
+server when static assets change. Thanks to Tim Kamanin for the report in
+`Issue #46
 github.com/adamchainz/django-browser-reload/issues/46>`__. * Use 'defer' in the
 ``
```

### Comparing `django_browser_reload-1.7.0/LICENSE` & `django_browser_reload-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.7.0/PKG-INFO` & `django_browser_reload-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_browser_reload
-Version: 1.7.0
+Version: 1.8.0
 Summary: Automatically reload your browser in development.
 Home-page: https://github.com/adamchainz/django-browser-reload
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-browser-reload/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
```

### Comparing `django_browser_reload-1.7.0/README.rst` & `django_browser_reload-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.7.0/setup.cfg` & `django_browser_reload-1.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_browser_reload
-version = 1.7.0
+version = 1.8.0
 description = Automatically reload your browser in development.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/django-browser-reload
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
```

### Comparing `django_browser_reload-1.7.0/src/django_browser_reload/jinja.py` & `django_browser_reload-1.8.0/src/django_browser_reload/jinja.py`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.7.0/src/django_browser_reload/middleware.py` & `django_browser_reload-1.8.0/src/django_browser_reload/middleware.py`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.7.0/src/django_browser_reload/static/django-browser-reload/reload-listener.js` & `django_browser_reload-1.8.0/src/django_browser_reload/static/django-browser-reload/reload-listener.js`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.7.0/src/django_browser_reload/static/django-browser-reload/reload-worker.js` & `django_browser_reload-1.8.0/src/django_browser_reload/static/django-browser-reload/reload-worker.js`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.7.0/src/django_browser_reload/views.py` & `django_browser_reload-1.8.0/src/django_browser_reload/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,11 +150,14 @@
             yield message("ping", versionId=version_id)
 
             should_reload = should_reload_event.wait(timeout=PING_DELAY)
             if should_reload:
                 should_reload_event.clear()
                 yield message("reload")
 
-    return StreamingHttpResponse(
+    response = StreamingHttpResponse(
         event_stream(),
         content_type="text/event-stream",
     )
+    # Set a content-encoding to bypass GzipMiddleware etc.
+    response["content-encoding"] = ""
+    return response
```

### Comparing `django_browser_reload-1.7.0/src/django_browser_reload.egg-info/PKG-INFO` & `django_browser_reload-1.8.0/src/django_browser_reload.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-browser-reload
-Version: 1.7.0
+Version: 1.8.0
 Summary: Automatically reload your browser in development.
 Home-page: https://github.com/adamchainz/django-browser-reload
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-browser-reload/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
```

### Comparing `django_browser_reload-1.7.0/src/django_browser_reload.egg-info/SOURCES.txt` & `django_browser_reload-1.8.0/src/django_browser_reload.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.7.0/tests/test_jinja.py` & `django_browser_reload-1.8.0/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.7.0/tests/test_middleware.py` & `django_browser_reload-1.8.0/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django_browser_reload-1.7.0/tests/test_views.py` & `django_browser_reload-1.8.0/tests/test_views.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import time
 from http import HTTPStatus
 from pathlib import Path
 from unittest import mock
 
 from django.conf import settings
 from django.http import StreamingHttpResponse
+from django.middleware.gzip import GZipMiddleware
 from django.test import override_settings
+from django.test import RequestFactory
 from django.test import SimpleTestCase
 
 import django_browser_reload
 from django_browser_reload import views
 
 
 class OnAutoreloadStartedTests(SimpleTestCase):
@@ -116,7 +118,24 @@
         assert response.status_code == HTTPStatus.OK
         assert response["Content-Type"] == "text/event-stream"
         # Skip version ID message
         next(response.streaming_content)
         event = next(response.streaming_content)
         assert event == b'data: {"type": "reload"}\n\n'
         assert not views.should_reload_event.is_set()
+
+    def test_success_template_change_with_gzip(self):
+        # https://github.com/typeddjango/django-stubs/pull/1421
+        middleware = GZipMiddleware(views.events)  # type: ignore[arg-type]
+        request = RequestFactory(HTTP_ACCEPT_ENCODING="gzip").get("/")
+        response = middleware(request)
+        assert isinstance(response, StreamingHttpResponse)
+        views.should_reload_event.set()
+
+        assert response.status_code == HTTPStatus.OK
+        assert response["Content-Type"] == "text/event-stream"
+        assert response["Content-Encoding"] == ""
+        # Skip version ID message
+        next(response.streaming_content)
+        event = next(response.streaming_content)
+        assert event == b'data: {"type": "reload"}\n\n'
+        assert not views.should_reload_event.is_set()
```

