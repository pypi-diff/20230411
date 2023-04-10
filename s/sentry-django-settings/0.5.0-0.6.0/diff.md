# Comparing `tmp/sentry_django_settings-0.5.0.tar.gz` & `tmp/sentry_django_settings-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/aaronc/Coding/enervee/sentry-django-settings/dist/tmpnf5q7ro3/sentry_django_settings-0.5.0.tar", last modified: Tue Mar  8 00:20:15 2022, max compression
+gzip compressed data, was "sentry_django_settings-0.6.0.tar", max compression
```

## Comparing `sentry_django_settings-0.5.0.tar` & `sentry_django_settings-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,5 @@
-drwxr-xr-x   0 aaronc     (501) staff       (20)        0 2022-03-08 00:20:15.000000 sentry_django_settings-0.5.0/
--rw-r--r--   0 aaronc     (501) staff       (20)     2487 2022-03-08 00:20:15.000000 sentry_django_settings-0.5.0/PKG-INFO
--rw-r--r--   0 aaronc     (501) staff       (20)     1487 2022-02-25 21:51:49.000000 sentry_django_settings-0.5.0/LICENSE
--rw-r--r--   0 aaronc     (501) staff       (20)      439 2022-03-07 18:42:33.000000 sentry_django_settings-0.5.0/pyproject.toml
-drwxr-xr-x   0 aaronc     (501) staff       (20)        0 2022-03-08 00:20:15.000000 sentry_django_settings-0.5.0/sentry_django_settings/
--rw-r--r--   0 aaronc     (501) staff       (20)      489 2022-02-25 21:51:49.000000 sentry_django_settings-0.5.0/sentry_django_settings/git_sha.py
--rw-r--r--   0 aaronc     (501) staff       (20)        0 2022-02-25 21:51:49.000000 sentry_django_settings-0.5.0/sentry_django_settings/__init__.py
--rw-r--r--   0 aaronc     (501) staff       (20)     2267 2022-03-07 18:37:20.000000 sentry_django_settings-0.5.0/sentry_django_settings/apps.py
--rw-r--r--   0 aaronc     (501) staff       (20)       34 2022-02-25 21:51:49.000000 sentry_django_settings-0.5.0/MANIFEST.in
--rw-r--r--   0 aaronc     (501) staff       (20)     1655 2022-03-07 18:55:59.000000 sentry_django_settings-0.5.0/README.md
--rw-r--r--   0 aaronc     (501) staff       (20)     1270 2022-03-08 00:19:55.000000 sentry_django_settings-0.5.0/setup.py
-drwxr-xr-x   0 aaronc     (501) staff       (20)        0 2022-03-08 00:20:15.000000 sentry_django_settings-0.5.0/sentry_django_settings.egg-info/
--rw-r--r--   0 aaronc     (501) staff       (20)     2487 2022-03-08 00:20:15.000000 sentry_django_settings-0.5.0/sentry_django_settings.egg-info/PKG-INFO
--rw-r--r--   0 aaronc     (501) staff       (20)      382 2022-03-08 00:20:15.000000 sentry_django_settings-0.5.0/sentry_django_settings.egg-info/SOURCES.txt
--rw-r--r--   0 aaronc     (501) staff       (20)       21 2022-03-08 00:20:15.000000 sentry_django_settings-0.5.0/sentry_django_settings.egg-info/requires.txt
--rw-r--r--   0 aaronc     (501) staff       (20)       23 2022-03-08 00:20:15.000000 sentry_django_settings-0.5.0/sentry_django_settings.egg-info/top_level.txt
--rw-r--r--   0 aaronc     (501) staff       (20)        1 2022-03-08 00:20:15.000000 sentry_django_settings-0.5.0/sentry_django_settings.egg-info/dependency_links.txt
--rw-r--r--   0 aaronc     (501) staff       (20)       38 2022-03-08 00:20:15.000000 sentry_django_settings-0.5.0/setup.cfg
+-rw-r--r--   0        0        0     1487 2022-02-25 21:51:49.124961 sentry_django_settings-0.6.0/LICENSE
+-rw-r--r--   0        0        0      423 2023-04-10 22:56:22.589817 sentry_django_settings-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-02-25 21:51:49.125929 sentry_django_settings-0.6.0/sentry_django_settings/__init__.py
+-rw-r--r--   0        0        0     2402 2023-04-10 22:23:23.223916 sentry_django_settings-0.6.0/sentry_django_settings/apps.py
+-rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 sentry_django_settings-0.6.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sentry_django_settings-0.5.0/LICENSE` & `sentry_django_settings-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_django_settings-0.5.0/sentry_django_settings/apps.py` & `sentry_django_settings-0.6.0/sentry_django_settings/apps.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 """
 This is the Django configuration file for Sentry.
 """
-from __future__ import unicode_literals
 import logging
+import warnings
 
 from django.apps import AppConfig
 from django.conf import settings
 
 import sentry_sdk
 from sentry_sdk.integrations.django import DjangoIntegration
 
-from sentry_django_settings.git_sha import get_from_repo, get_from_file
-
 logger = logging.getLogger("django.sentry_django_settings")
 
 
 class Sentry(AppConfig):
     name = "sentry_django_settings"
 
     extra_config_options = {"enabled", "git_sha_path"}
 
     def ready(self):
+        warnings.warn(
+            "sentry_django_settings is no longer supported. See "
+            "https://github.com/enervee/sentry-django-settings/issues/12 for more information.",
+            FutureWarning,
+            stacklevel=2,
+        )
         sentry_setting = getattr(settings, "SENTRY", None)
         if not sentry_setting:
             logger.warning("No SENTRY settings found.")
             return
 
         sentry_django_config = SentryDjangoConfig(sentry_setting)
 
@@ -47,33 +51,29 @@
         in the settings.
 
         Returns:
             dict: a collection of Sentry configuration options
         """
         config = self.default_config()
         config.update(self.config)
-        config["release"] = self.get_release()
         self.remove_extra_options(config)
         return config
 
-    def get_release(self):
-        """Gets the "release" value. If one isn't given, it tries to get it
-        from the project."""
-        release = self.config.get("release")
-        if not release:
-            release = get_from_repo()
-        if not release and self.config.get("git_sha_path"):
-            release = get_from_file(self.config.get("git_sha_path"))
-
-        return release
-
     def enabled(self):
         return self.config.get("enabled", False)
 
     @staticmethod
     def default_config():
         return {"integrations": [DjangoIntegration()]}
 
     @classmethod
     def remove_extra_options(cls, config):
         for extra_key in cls.EXTRA_CONFIG_OPTIONS:
+            if extra_key == "git_sha_path" and extra_key in config:
+                warnings.warn(
+                    "`git_sha_path` is no longer supported and has no effect. "
+                    "See https://docs.sentry.io/platforms/python/configuration/options/#release"
+                    " on how to set the release directly.",
+                    FutureWarning,
+                    stacklevel=4,
+                )
             config.pop(extra_key, None)
```

