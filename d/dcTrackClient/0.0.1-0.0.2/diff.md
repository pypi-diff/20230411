# Comparing `tmp/dctrackclient-0.0.1.tar.gz` & `tmp/dctrackclient-0.0.2.tar.gz`

## Comparing `dctrackclient-0.0.1.tar` & `dctrackclient-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dctrackclient-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 dctrackclient-0.0.1/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 dctrackclient-0.0.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.0.1/LICENSE
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 dctrackclient-0.0.1/README.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dctrackclient-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 dctrackclient-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 dctrackclient-0.0.2/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 dctrackclient-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.0.2/LICENSE
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dctrackclient-0.0.2/README.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dctrackclient-0.0.2/PKG-INFO
```

### Comparing `dctrackclient-0.0.1/.github/workflows/python-publish.yml` & `dctrackclient-0.0.2/.github/workflows/python-publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -29,11 +29,11 @@
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
     - name: Publish package
-      uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+      uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `dctrackclient-0.0.1/.gitignore` & `dctrackclient-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.0.1/LICENSE` & `dctrackclient-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.0.1/pyproject.toml` & `dctrackclient-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

