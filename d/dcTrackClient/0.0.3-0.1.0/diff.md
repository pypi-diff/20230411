# Comparing `tmp/dctrackclient-0.0.3.tar.gz` & `tmp/dctrackclient-0.1.0.tar.gz`

## Comparing `dctrackclient-0.0.3.tar` & `dctrackclient-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 dctrackclient-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 dctrackclient-0.0.3/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.0.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.0.3/LICENSE
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dctrackclient-0.0.3/README.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dctrackclient-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 dctrackclient-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 dctrackclient-0.1.0/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.1.0/LICENSE
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dctrackclient-0.1.0/README.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dctrackclient-0.1.0/PKG-INFO
```

### Comparing `dctrackclient-0.0.3/.github/workflows/python-publish.yml` & `dctrackclient-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.0.3/LICENSE` & `dctrackclient-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.0.3/pyproject.toml` & `dctrackclient-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.0.3/PKG-INFO` & `dctrackclient-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.0.3
+Version: 0.1.0
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

