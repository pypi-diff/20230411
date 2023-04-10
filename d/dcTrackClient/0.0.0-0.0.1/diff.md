# Comparing `tmp/dctrackclient-0.0.0.tar.gz` & `tmp/dctrackclient-0.0.1.tar.gz`

## Comparing `dctrackclient-0.0.0.tar` & `dctrackclient-0.0.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 dctrackclient-0.0.0/dcTrackAPI.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 dctrackclient-0.0.0/token.txt
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dctrackclient-0.0.0/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 dctrackclient-0.0.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.0.0/LICENSE
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 dctrackclient-0.0.0/README.md
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 dctrackclient-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 dctrackclient-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dctrackclient-0.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 dctrackclient-0.0.1/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 dctrackclient-0.0.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.0.1/LICENSE
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 dctrackclient-0.0.1/README.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dctrackclient-0.0.1/PKG-INFO
```

### Comparing `dctrackclient-0.0.0/.gitignore` & `dctrackclient-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.0.0/LICENSE` & `dctrackclient-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.0.0/pyproject.toml` & `dctrackclient-0.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
-description = "A small example package"
+description = "Sunbird dcTrack API client in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `dctrackclient-0.0.0/PKG-INFO` & `dctrackclient-0.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.0.0
-Summary: A small example package
+Version: 0.0.1
+Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

