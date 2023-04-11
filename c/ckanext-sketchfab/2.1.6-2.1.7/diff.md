# Comparing `tmp/ckanext-sketchfab-2.1.6.tar.gz` & `tmp/ckanext-sketchfab-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-sketchfab-2.1.6.tar", last modified: Mon Feb 20 11:04:36 2023, max compression
+gzip compressed data, was "ckanext-sketchfab-2.1.7.tar", last modified: Tue Apr 11 08:26:02 2023, max compression
```

## Comparing `ckanext-sketchfab-2.1.6.tar` & `ckanext-sketchfab-2.1.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:04:36.937737 ckanext-sketchfab-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-20 11:04:22.000000 ckanext-sketchfab-2.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-02-20 11:04:36.937737 ckanext-sketchfab-2.1.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3772 2023-02-20 11:04:22.000000 ckanext-sketchfab-2.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:04:36.933737 ckanext-sketchfab-2.1.6/ckanext/
--rwxr-xr-x   0 runner    (1001) docker     (123)      310 2023-02-20 11:04:22.000000 ckanext-sketchfab-2.1.6/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:04:36.933737 ckanext-sketchfab-2.1.6/ckanext/sketchfab/
--rwxr-xr-x   0 runner    (1001) docker     (123)      310 2023-02-20 11:04:22.000000 ckanext-sketchfab-2.1.6/ckanext/sketchfab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:04:36.933737 ckanext-sketchfab-2.1.6/ckanext/sketchfab/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 11:04:22.000000 ckanext-sketchfab-2.1.6/ckanext/sketchfab/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-20 11:04:22.000000 ckanext-sketchfab-2.1.6/ckanext/sketchfab/logic/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-02-20 11:04:22.000000 ckanext-sketchfab-2.1.6/ckanext/sketchfab/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:04:36.933737 ckanext-sketchfab-2.1.6/ckanext/sketchfab/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:04:36.933737 ckanext-sketchfab-2.1.6/ckanext/sketchfab/theme/templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)      571 2023-02-20 11:04:22.000000 ckanext-sketchfab-2.1.6/ckanext/sketchfab/theme/templates/sketchfab_form.html
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-02-20 11:04:22.000000 ckanext-sketchfab-2.1.6/ckanext/sketchfab/theme/templates/sketchfab_view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:04:36.937737 ckanext-sketchfab-2.1.6/ckanext_sketchfab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-02-20 11:04:36.000000 ckanext-sketchfab-2.1.6/ckanext_sketchfab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-02-20 11:04:36.000000 ckanext-sketchfab-2.1.6/ckanext_sketchfab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 11:04:36.000000 ckanext-sketchfab-2.1.6/ckanext_sketchfab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-20 11:04:36.000000 ckanext-sketchfab-2.1.6/ckanext_sketchfab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 11:04:36.000000 ckanext-sketchfab-2.1.6/ckanext_sketchfab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-20 11:04:36.000000 ckanext-sketchfab-2.1.6/ckanext_sketchfab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 11:04:36.000000 ckanext-sketchfab-2.1.6/ckanext_sketchfab.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:04:36.933737 ckanext-sketchfab-2.1.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:04:36.937737 ckanext-sketchfab-2.1.6/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-02-20 11:04:22.000000 ckanext-sketchfab-2.1.6/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-02-20 11:04:22.000000 ckanext-sketchfab-2.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 11:04:36.937737 ckanext-sketchfab-2.1.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-02-20 11:04:22.000000 ckanext-sketchfab-2.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:04:36.937737 ckanext-sketchfab-2.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-20 11:04:22.000000 ckanext-sketchfab-2.1.6/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-02-20 11:04:22.000000 ckanext-sketchfab-2.1.6/tests/test_sketchfab_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-02-20 11:04:22.000000 ckanext-sketchfab-2.1.6/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.684827 ckanext-sketchfab-2.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-04-11 08:26:02.684827 ckanext-sketchfab-2.1.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3772 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.676828 ckanext-sketchfab-2.1.7/ckanext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      310 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.676828 ckanext-sketchfab-2.1.7/ckanext/sketchfab/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      310 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/ckanext/sketchfab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.676828 ckanext-sketchfab-2.1.7/ckanext/sketchfab/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/ckanext/sketchfab/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/ckanext/sketchfab/logic/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/ckanext/sketchfab/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.672827 ckanext-sketchfab-2.1.7/ckanext/sketchfab/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.676828 ckanext-sketchfab-2.1.7/ckanext/sketchfab/theme/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      571 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/ckanext/sketchfab/theme/templates/sketchfab_form.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/ckanext/sketchfab/theme/templates/sketchfab_view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.680827 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-04-11 08:26:02.000000 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-11 08:26:02.000000 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:26:02.000000 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 08:26:02.000000 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:26:02.000000 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 08:26:02.000000 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:26:02.000000 ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.672827 ckanext-sketchfab-2.1.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.680827 ckanext-sketchfab-2.1.7/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:26:02.684827 ckanext-sketchfab-2.1.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:02.684827 ckanext-sketchfab-2.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/tests/test_sketchfab_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-11 08:25:44.000000 ckanext-sketchfab-2.1.7/tests/test_validators.py
```

### Comparing `ckanext-sketchfab-2.1.6/LICENSE` & `ckanext-sketchfab-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-sketchfab-2.1.6/PKG-INFO` & `ckanext-sketchfab-2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-sketchfab
-Version: 2.1.6
+Version: 2.1.7
 Summary: A CKAN extension for embedding Sketchfab models as views.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-sketchfab
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-sketchfab/blob/main/CHANGELOG.md
 Keywords: CKAN,data,sketchfab
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-sketchfab-2.1.6/README.md` & `ckanext-sketchfab-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-sketchfab-2.1.6/ckanext/sketchfab/logic/validators.py` & `ckanext-sketchfab-2.1.7/ckanext/sketchfab/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-sketchfab-2.1.6/ckanext/sketchfab/plugin.py` & `ckanext-sketchfab-2.1.7/ckanext/sketchfab/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-sketchfab-2.1.6/ckanext/sketchfab/theme/templates/sketchfab_form.html` & `ckanext-sketchfab-2.1.7/ckanext/sketchfab/theme/templates/sketchfab_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-sketchfab-2.1.6/ckanext_sketchfab.egg-info/PKG-INFO` & `ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-sketchfab
-Version: 2.1.6
+Version: 2.1.7
 Summary: A CKAN extension for embedding Sketchfab models as views.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-sketchfab
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-sketchfab/blob/main/CHANGELOG.md
 Keywords: CKAN,data,sketchfab
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-sketchfab-2.1.6/ckanext_sketchfab.egg-info/SOURCES.txt` & `ckanext-sketchfab-2.1.7/ckanext_sketchfab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-sketchfab-2.1.6/docs/_scripts/gen_api_pages.py` & `ckanext-sketchfab-2.1.7/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-sketchfab-2.1.6/pyproject.toml` & `ckanext-sketchfab-2.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-sketchfab"
-version = "2.1.6"
+version = "2.1.7"
 description = "A CKAN extension for embedding Sketchfab models as views."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -51,15 +51,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.sketchfab.theme" = ["*", "**/*"]
 
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

### Comparing `ckanext-sketchfab-2.1.6/tests/test_sketchfab_view.py` & `ckanext-sketchfab-2.1.7/tests/test_sketchfab_view.py`

 * *Files identical despite different names*

### Comparing `ckanext-sketchfab-2.1.6/tests/test_validators.py` & `ckanext-sketchfab-2.1.7/tests/test_validators.py`

 * *Files identical despite different names*

