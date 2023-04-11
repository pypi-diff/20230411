# Comparing `tmp/ckanext-webview-1.1.6.tar.gz` & `tmp/ckanext-webview-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-webview-1.1.6.tar", last modified: Mon Feb 20 11:13:59 2023, max compression
+gzip compressed data, was "ckanext-webview-1.1.7.tar", last modified: Tue Apr 11 08:47:00 2023, max compression
```

## Comparing `ckanext-webview-1.1.6.tar` & `ckanext-webview-1.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:13:59.701033 ckanext-webview-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-20 11:13:45.000000 ckanext-webview-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-02-20 11:13:59.701033 ckanext-webview-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-02-20 11:13:45.000000 ckanext-webview-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:13:59.697033 ckanext-webview-1.1.6/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-20 11:13:45.000000 ckanext-webview-1.1.6/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:13:59.697033 ckanext-webview-1.1.6/ckanext/webview/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-20 11:13:45.000000 ckanext-webview-1.1.6/ckanext/webview/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:13:59.697033 ckanext-webview-1.1.6/ckanext/webview/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 11:13:45.000000 ckanext-webview-1.1.6/ckanext/webview/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-02-20 11:13:45.000000 ckanext-webview-1.1.6/ckanext/webview/logic/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-02-20 11:13:45.000000 ckanext-webview-1.1.6/ckanext/webview/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:13:59.697033 ckanext-webview-1.1.6/ckanext/webview/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:13:59.697033 ckanext-webview-1.1.6/ckanext/webview/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:13:59.697033 ckanext-webview-1.1.6/ckanext/webview/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-20 11:13:45.000000 ckanext-webview-1.1.6/ckanext/webview/theme/assets/less/webview.less
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-20 11:13:45.000000 ckanext-webview-1.1.6/ckanext/webview/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:13:59.697033 ckanext-webview-1.1.6/ckanext/webview/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:13:59.701033 ckanext-webview-1.1.6/ckanext/webview/theme/templates/views/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-20 11:13:45.000000 ckanext-webview-1.1.6/ckanext/webview/theme/templates/views/web_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-20 11:13:45.000000 ckanext-webview-1.1.6/ckanext/webview/theme/templates/views/web_view_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:13:59.701033 ckanext-webview-1.1.6/ckanext_webview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-02-20 11:13:59.000000 ckanext-webview-1.1.6/ckanext_webview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-02-20 11:13:59.000000 ckanext-webview-1.1.6/ckanext_webview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 11:13:59.000000 ckanext-webview-1.1.6/ckanext_webview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-20 11:13:59.000000 ckanext-webview-1.1.6/ckanext_webview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 11:13:59.000000 ckanext-webview-1.1.6/ckanext_webview.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-20 11:13:59.000000 ckanext-webview-1.1.6/ckanext_webview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 11:13:59.000000 ckanext-webview-1.1.6/ckanext_webview.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:13:59.697033 ckanext-webview-1.1.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:13:59.701033 ckanext-webview-1.1.6/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-20 11:13:45.000000 ckanext-webview-1.1.6/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-02-20 11:13:45.000000 ckanext-webview-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 11:13:59.701033 ckanext-webview-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-20 11:13:45.000000 ckanext-webview-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:13:59.701033 ckanext-webview-1.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-02-20 11:13:45.000000 ckanext-webview-1.1.6/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.416164 ckanext-webview-1.1.7/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.416164 ckanext-webview-1.1.7/ckanext/webview/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/ckanext/webview/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/logic/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.416164 ckanext-webview-1.1.7/ckanext/webview/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/ckanext/webview/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/ckanext/webview/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/theme/assets/less/webview.less
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.416164 ckanext-webview-1.1.7/ckanext/webview/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/ckanext/webview/theme/templates/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/theme/templates/views/web_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/ckanext/webview/theme/templates/views/web_view_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/ckanext_webview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-11 08:47:00.000000 ckanext-webview-1.1.7/ckanext_webview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-11 08:47:00.000000 ckanext-webview-1.1.7/ckanext_webview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:47:00.000000 ckanext-webview-1.1.7/ckanext_webview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-11 08:47:00.000000 ckanext-webview-1.1.7/ckanext_webview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:47:00.000000 ckanext-webview-1.1.7/ckanext_webview.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 08:47:00.000000 ckanext-webview-1.1.7/ckanext_webview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:47:00.000000 ckanext-webview-1.1.7/ckanext_webview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.416164 ckanext-webview-1.1.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:47:00.420163 ckanext-webview-1.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-11 08:46:44.000000 ckanext-webview-1.1.7/tests/test_validators.py
```

### Comparing `ckanext-webview-1.1.6/LICENSE` & `ckanext-webview-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-webview-1.1.6/PKG-INFO` & `ckanext-webview-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-webview
-Version: 1.1.6
+Version: 1.1.7
 Summary: A CKAN extension that adds a view for displaying generic/arbitrary URLs.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-webview
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-webview/blob/main/CHANGELOG.md
 Keywords: CKAN,data,webview
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-webview-1.1.6/README.md` & `ckanext-webview-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-webview-1.1.6/ckanext/webview/logic/validators.py` & `ckanext-webview-1.1.7/ckanext/webview/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-webview-1.1.6/ckanext/webview/plugin.py` & `ckanext-webview-1.1.7/ckanext/webview/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-webview-1.1.6/ckanext_webview.egg-info/PKG-INFO` & `ckanext-webview-1.1.7/ckanext_webview.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-webview
-Version: 1.1.6
+Version: 1.1.7
 Summary: A CKAN extension that adds a view for displaying generic/arbitrary URLs.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-webview
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-webview/blob/main/CHANGELOG.md
 Keywords: CKAN,data,webview
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-webview-1.1.6/ckanext_webview.egg-info/SOURCES.txt` & `ckanext-webview-1.1.7/ckanext_webview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-webview-1.1.6/docs/_scripts/gen_api_pages.py` & `ckanext-webview-1.1.7/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-webview-1.1.6/pyproject.toml` & `ckanext-webview-1.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-webview"
-version = "1.1.6"
+version = "1.1.7"
 description = "A CKAN extension that adds a view for displaying generic/arbitrary URLs."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -51,15 +51,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.webview.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "1.1.6"
+version = "1.1.7"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-webview-1.1.6/tests/test_validators.py` & `ckanext-webview-1.1.7/tests/test_validators.py`

 * *Files identical despite different names*

