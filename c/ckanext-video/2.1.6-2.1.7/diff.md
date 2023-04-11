# Comparing `tmp/ckanext-video-2.1.6.tar.gz` & `tmp/ckanext-video-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-video-2.1.6.tar", last modified: Mon Feb 20 11:12:32 2023, max compression
+gzip compressed data, was "ckanext-video-2.1.7.tar", last modified: Tue Apr 11 08:44:22 2023, max compression
```

## Comparing `ckanext-video-2.1.6.tar` & `ckanext-video-2.1.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:12:32.758154 ckanext-video-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-20 11:12:21.000000 ckanext-video-2.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-02-20 11:12:32.758154 ckanext-video-2.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-02-20 11:12:21.000000 ckanext-video-2.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:12:32.754154 ckanext-video-2.1.6/ckanext/
--rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-02-20 11:12:21.000000 ckanext-video-2.1.6/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:12:32.754154 ckanext-video-2.1.6/ckanext/video/
--rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-02-20 11:12:21.000000 ckanext-video-2.1.6/ckanext/video/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:12:32.754154 ckanext-video-2.1.6/ckanext/video/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 11:12:21.000000 ckanext-video-2.1.6/ckanext/video/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-20 11:12:21.000000 ckanext-video-2.1.6/ckanext/video/logic/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-02-20 11:12:21.000000 ckanext-video-2.1.6/ckanext/video/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-02-20 11:12:21.000000 ckanext-video-2.1.6/ckanext/video/providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:12:32.754154 ckanext-video-2.1.6/ckanext/video/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:12:32.754154 ckanext-video-2.1.6/ckanext/video/theme/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-20 11:12:21.000000 ckanext-video-2.1.6/ckanext/video/theme/templates/video_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-20 11:12:21.000000 ckanext-video-2.1.6/ckanext/video/theme/templates/video_view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:12:32.758154 ckanext-video-2.1.6/ckanext_video.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-02-20 11:12:32.000000 ckanext-video-2.1.6/ckanext_video.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-02-20 11:12:32.000000 ckanext-video-2.1.6/ckanext_video.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 11:12:32.000000 ckanext-video-2.1.6/ckanext_video.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-20 11:12:32.000000 ckanext-video-2.1.6/ckanext_video.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 11:12:32.000000 ckanext-video-2.1.6/ckanext_video.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-20 11:12:32.000000 ckanext-video-2.1.6/ckanext_video.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 11:12:32.000000 ckanext-video-2.1.6/ckanext_video.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:12:32.754154 ckanext-video-2.1.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:12:32.758154 ckanext-video-2.1.6/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-20 11:12:21.000000 ckanext-video-2.1.6/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-02-20 11:12:21.000000 ckanext-video-2.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 11:12:32.758154 ckanext-video-2.1.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-02-20 11:12:21.000000 ckanext-video-2.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:12:32.758154 ckanext-video-2.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-02-20 11:12:21.000000 ckanext-video-2.1.6/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-02-20 11:12:21.000000 ckanext-video-2.1.6/tests/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.398120 ckanext-video-2.1.7/ckanext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.398120 ckanext-video-2.1.7/ckanext/video/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/video/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/ckanext/video/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/video/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/video/logic/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/video/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/video/providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.398120 ckanext-video-2.1.7/ckanext/video/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/ckanext/video/theme/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/video/theme/templates/video_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/ckanext/video/theme/templates/video_view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/ckanext_video.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-11 08:44:22.000000 ckanext-video-2.1.7/ckanext_video.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-11 08:44:22.000000 ckanext-video-2.1.7/ckanext_video.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:44:22.000000 ckanext-video-2.1.7/ckanext_video.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-11 08:44:22.000000 ckanext-video-2.1.7/ckanext_video.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:44:22.000000 ckanext-video-2.1.7/ckanext_video.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 08:44:22.000000 ckanext-video-2.1.7/ckanext_video.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:44:22.000000 ckanext-video-2.1.7/ckanext_video.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.398120 ckanext-video-2.1.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:44:22.402120 ckanext-video-2.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-11 08:44:11.000000 ckanext-video-2.1.7/tests/test_view.py
```

### Comparing `ckanext-video-2.1.6/LICENSE` & `ckanext-video-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-video-2.1.6/PKG-INFO` & `ckanext-video-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-video
-Version: 2.1.6
+Version: 2.1.7
 Summary: A CKAN extension for embedding Youtube or Vimeo videos as views.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-video
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-video/blob/main/CHANGELOG.md
 Keywords: CKAN,data,video
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-video-2.1.6/README.md` & `ckanext-video-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-video-2.1.6/ckanext/video/logic/validators.py` & `ckanext-video-2.1.7/ckanext/video/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-video-2.1.6/ckanext/video/plugin.py` & `ckanext-video-2.1.7/ckanext/video/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-video-2.1.6/ckanext/video/theme/templates/video_form.html` & `ckanext-video-2.1.7/ckanext/video/theme/templates/video_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-video-2.1.6/ckanext_video.egg-info/PKG-INFO` & `ckanext-video-2.1.7/ckanext_video.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-video
-Version: 2.1.6
+Version: 2.1.7
 Summary: A CKAN extension for embedding Youtube or Vimeo videos as views.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-video
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-video/blob/main/CHANGELOG.md
 Keywords: CKAN,data,video
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-video-2.1.6/ckanext_video.egg-info/SOURCES.txt` & `ckanext-video-2.1.7/ckanext_video.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-video-2.1.6/docs/_scripts/gen_api_pages.py` & `ckanext-video-2.1.7/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-video-2.1.6/pyproject.toml` & `ckanext-video-2.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-video"
-version = "2.1.6"
+version = "2.1.7"
 description = "A CKAN extension for embedding Youtube or Vimeo videos as views."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -51,15 +51,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.video.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "2.1.6"
+version = "2.1.7"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-video-2.1.6/tests/test_validators.py` & `ckanext-video-2.1.7/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-video-2.1.6/tests/test_view.py` & `ckanext-video-2.1.7/tests/test_view.py`

 * *Files identical despite different names*

