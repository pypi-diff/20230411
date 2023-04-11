# Comparing `tmp/ckanext-doi-3.1.6.tar.gz` & `tmp/ckanext-doi-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-doi-3.1.6.tar", last modified: Mon Feb 20 10:47:22 2023, max compression
+gzip compressed data, was "ckanext-doi-3.1.7.tar", last modified: Tue Apr 11 08:17:38 2023, max compression
```

## Comparing `ckanext-doi-3.1.6.tar` & `ckanext-doi-3.1.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.470656 ckanext-doi-3.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-02-20 10:47:22.470656 ckanext-doi-3.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.466657 ckanext-doi-3.1.6/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.466657 ckanext-doi-3.1.6/ckanext/doi/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.470656 ckanext-doi-3.1.6/ckanext/doi/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/lib/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/lib/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/lib/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/lib/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/lib/xml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.470656 ckanext-doi-3.1.6/ckanext/doi/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/model/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/model/doi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.466657 ckanext-doi-3.1.6/ckanext/doi/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.466657 ckanext-doi-3.1.6/ckanext/doi/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.466657 ckanext-doi-3.1.6/ckanext/doi/theme/templates/doi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.470656 ckanext-doi-3.1.6/ckanext/doi/theme/templates/doi/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/theme/templates/doi/snippets/package_citation.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/theme/templates/doi/snippets/resource_citation.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.470656 ckanext-doi-3.1.6/ckanext/doi/theme/templates/package/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/theme/templates/package/read.html
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/theme/templates/package/read_base.html
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/theme/templates/package/resource_read.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.470656 ckanext-doi-3.1.6/ckanext/doi/theme/templates/package/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/theme/templates/package/snippets/package_basic_fields.html
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/ckanext/doi/theme/templates/package/snippets/package_metadata_fields.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.470656 ckanext-doi-3.1.6/ckanext_doi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-02-20 10:47:22.000000 ckanext-doi-3.1.6/ckanext_doi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-02-20 10:47:22.000000 ckanext-doi-3.1.6/ckanext_doi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 10:47:22.000000 ckanext-doi-3.1.6/ckanext_doi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-20 10:47:22.000000 ckanext-doi-3.1.6/ckanext_doi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 10:47:22.000000 ckanext-doi-3.1.6/ckanext_doi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-20 10:47:22.000000 ckanext-doi-3.1.6/ckanext_doi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-20 10:47:22.000000 ckanext-doi-3.1.6/ckanext_doi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.466657 ckanext-doi-3.1.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.470656 ckanext-doi-3.1.6/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 10:47:22.470656 ckanext-doi-3.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.470656 ckanext-doi-3.1.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:22.470656 ckanext-doi-3.1.6/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/tests/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-02-20 10:47:11.000000 ckanext-doi-3.1.6/tests/test_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.561735 ckanext-doi-3.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-04-11 08:17:38.561735 ckanext-doi-3.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.557735 ckanext-doi-3.1.7/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.557735 ckanext-doi-3.1.7/ckanext/doi/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.557735 ckanext-doi-3.1.7/ckanext/doi/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/lib/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/lib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/lib/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/lib/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/lib/xml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.557735 ckanext-doi-3.1.7/ckanext/doi/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/model/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/model/doi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.553735 ckanext-doi-3.1.7/ckanext/doi/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.553735 ckanext-doi-3.1.7/ckanext/doi/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.553735 ckanext-doi-3.1.7/ckanext/doi/theme/templates/doi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.557735 ckanext-doi-3.1.7/ckanext/doi/theme/templates/doi/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/theme/templates/doi/snippets/package_citation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/theme/templates/doi/snippets/resource_citation.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.561735 ckanext-doi-3.1.7/ckanext/doi/theme/templates/package/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/theme/templates/package/read.html
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/theme/templates/package/read_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/theme/templates/package/resource_read.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.561735 ckanext-doi-3.1.7/ckanext/doi/theme/templates/package/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/theme/templates/package/snippets/package_basic_fields.html
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/ckanext/doi/theme/templates/package/snippets/package_metadata_fields.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.561735 ckanext-doi-3.1.7/ckanext_doi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-04-11 08:17:38.000000 ckanext-doi-3.1.7/ckanext_doi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-11 08:17:38.000000 ckanext-doi-3.1.7/ckanext_doi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:17:38.000000 ckanext-doi-3.1.7/ckanext_doi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-11 08:17:38.000000 ckanext-doi-3.1.7/ckanext_doi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:17:38.000000 ckanext-doi-3.1.7/ckanext_doi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-11 08:17:38.000000 ckanext-doi-3.1.7/ckanext_doi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-11 08:17:38.000000 ckanext-doi-3.1.7/ckanext_doi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.553735 ckanext-doi-3.1.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.561735 ckanext-doi-3.1.7/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:17:38.561735 ckanext-doi-3.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.561735 ckanext-doi-3.1.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:17:38.561735 ckanext-doi-3.1.7/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/tests/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-11 08:17:09.000000 ckanext-doi-3.1.7/tests/test_generate.py
```

### Comparing `ckanext-doi-3.1.6/LICENSE` & `ckanext-doi-3.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/PKG-INFO` & `ckanext-doi-3.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-doi
-Version: 3.1.6
+Version: 3.1.7
 Summary: A CKAN extension for assigning a digital object identifier (DOI) to datasets, using the DataCite DOI service.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-doi
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-doi/blob/main/CHANGELOG.md
 Keywords: CKAN,data,doi
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-doi-3.1.6/README.md` & `ckanext-doi-3.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/ckanext/doi/cli.py` & `ckanext-doi-3.1.7/ckanext/doi/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/ckanext/doi/interfaces.py` & `ckanext-doi-3.1.7/ckanext/doi/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/ckanext/doi/lib/api.py` & `ckanext-doi-3.1.7/ckanext/doi/lib/api.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/ckanext/doi/lib/helpers.py` & `ckanext-doi-3.1.7/ckanext/doi/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/ckanext/doi/lib/metadata.py` & `ckanext-doi-3.1.7/ckanext/doi/lib/metadata.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/ckanext/doi/lib/xml_utils.py` & `ckanext-doi-3.1.7/ckanext/doi/lib/xml_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/ckanext/doi/model/crud.py` & `ckanext-doi-3.1.7/ckanext/doi/model/crud.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/ckanext/doi/model/doi.py` & `ckanext-doi-3.1.7/ckanext/doi/model/doi.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/ckanext/doi/plugin.py` & `ckanext-doi-3.1.7/ckanext/doi/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/ckanext/doi/theme/templates/doi/snippets/package_citation.html` & `ckanext-doi-3.1.7/ckanext/doi/theme/templates/doi/snippets/package_citation.html`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/ckanext/doi/theme/templates/doi/snippets/resource_citation.html` & `ckanext-doi-3.1.7/ckanext/doi/theme/templates/doi/snippets/resource_citation.html`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/ckanext/doi/theme/templates/package/read.html` & `ckanext-doi-3.1.7/ckanext/doi/theme/templates/package/read.html`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/ckanext/doi/theme/templates/package/snippets/package_metadata_fields.html` & `ckanext-doi-3.1.7/ckanext/doi/theme/templates/package/snippets/package_metadata_fields.html`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/ckanext_doi.egg-info/PKG-INFO` & `ckanext-doi-3.1.7/ckanext_doi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-doi
-Version: 3.1.6
+Version: 3.1.7
 Summary: A CKAN extension for assigning a digital object identifier (DOI) to datasets, using the DataCite DOI service.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-doi
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-doi/blob/main/CHANGELOG.md
 Keywords: CKAN,data,doi
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-doi-3.1.6/ckanext_doi.egg-info/SOURCES.txt` & `ckanext-doi-3.1.7/ckanext_doi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/docs/_scripts/gen_api_pages.py` & `ckanext-doi-3.1.7/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/pyproject.toml` & `ckanext-doi-3.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-doi"
-version = "3.1.6"
+version = "3.1.7"
 description = "A CKAN extension for assigning a digital object identifier (DOI) to datasets, using the DataCite DOI service."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -54,15 +54,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.doi.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "3.1.6"
+version = "3.1.7"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-doi-3.1.6/tests/helpers/constants.py` & `ckanext-doi-3.1.7/tests/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/tests/test_api.py` & `ckanext-doi-3.1.7/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/tests/test_db.py` & `ckanext-doi-3.1.7/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `ckanext-doi-3.1.6/tests/test_generate.py` & `ckanext-doi-3.1.7/tests/test_generate.py`

 * *Files identical despite different names*

