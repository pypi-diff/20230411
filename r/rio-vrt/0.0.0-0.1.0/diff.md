# Comparing `tmp/rio-vrt-0.0.0.tar.gz` & `tmp/rio-vrt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio-vrt-0.0.0.tar", last modified: Sun Apr  9 19:16:43 2023, max compression
+gzip compressed data, was "rio-vrt-0.1.0.tar", last modified: Tue Apr 11 06:09:06 2023, max compression
```

## Comparing `rio-vrt-0.0.0.tar` & `rio-vrt-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 borntobealive  (1000) borntobealive  (1000)        0 2023-04-09 19:16:43.322961 rio-vrt-0.0.0/
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)     2728 2023-04-09 19:16:43.322961 rio-vrt-0.0.0/PKG-INFO
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)     1958 2023-04-09 19:08:08.000000 rio-vrt-0.0.0/README.rst
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)     2171 2023-04-09 19:08:08.000000 rio-vrt-0.0.0/pyproject.toml
-drwxr-xr-x   0 borntobealive  (1000) borntobealive  (1000)        0 2023-04-09 19:16:43.322961 rio-vrt-0.0.0/rio_vrt/
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)      274 2023-04-09 19:08:08.000000 rio-vrt-0.0.0/rio_vrt/__init__.py
-drwxr-xr-x   0 borntobealive  (1000) borntobealive  (1000)        0 2023-04-09 19:16:43.322961 rio-vrt-0.0.0/rio_vrt.egg-info/
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)     2728 2023-04-09 19:16:43.000000 rio-vrt-0.0.0/rio_vrt.egg-info/PKG-INFO
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)      226 2023-04-09 19:16:43.000000 rio-vrt-0.0.0/rio_vrt.egg-info/SOURCES.txt
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)        1 2023-04-09 19:16:43.000000 rio-vrt-0.0.0/rio_vrt.egg-info/dependency_links.txt
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)      186 2023-04-09 19:16:43.000000 rio-vrt-0.0.0/rio_vrt.egg-info/requires.txt
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)        8 2023-04-09 19:16:43.000000 rio-vrt-0.0.0/rio_vrt.egg-info/top_level.txt
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)       38 2023-04-09 19:16:43.322961 rio-vrt-0.0.0/setup.cfg
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)       66 2023-04-09 19:08:08.000000 rio-vrt-0.0.0/setup.py
-drwxr-xr-x   0 borntobealive  (1000) borntobealive  (1000)        0 2023-04-09 19:16:43.322961 rio-vrt-0.0.0/tests/
--rw-r--r--   0 borntobealive  (1000) borntobealive  (1000)      154 2023-04-09 19:08:08.000000 rio-vrt-0.0.0/tests/test_src.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:09:06.460069 rio-vrt-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-11 06:09:06.460069 rio-vrt-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-11 06:08:50.000000 rio-vrt-0.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-11 06:08:50.000000 rio-vrt-0.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:09:06.456069 rio-vrt-0.1.0/rio_vrt/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-11 06:08:50.000000 rio-vrt-0.1.0/rio_vrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-11 06:08:50.000000 rio-vrt-0.1.0/rio_vrt/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-11 06:08:50.000000 rio-vrt-0.1.0/rio_vrt/vrt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:09:06.460069 rio-vrt-0.1.0/rio_vrt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-11 06:09:06.000000 rio-vrt-0.1.0/rio_vrt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-11 06:09:06.000000 rio-vrt-0.1.0/rio_vrt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:09:06.000000 rio-vrt-0.1.0/rio_vrt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-11 06:09:06.000000 rio-vrt-0.1.0/rio_vrt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 06:09:06.000000 rio-vrt-0.1.0/rio_vrt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 06:09:06.460069 rio-vrt-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-11 06:08:50.000000 rio-vrt-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:09:06.460069 rio-vrt-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-11 06:08:51.000000 rio-vrt-0.1.0/tests/test_rio_vrt.py
```

### Comparing `rio-vrt-0.0.0/PKG-INFO` & `rio-vrt-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-vrt
-Version: 0.0.0
+Version: 0.1.0
 Summary: A simple librairy to build a vrt from multiple raster source relying only on rasterio
 Author-email: pierrick rambaud <pierrick.rambaud49@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/12rambau/rio-vrt
 Keywords: skeleton,Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -62,13 +62,20 @@
 .. image:: https://img.shields.io/badge/all_contributors-0-orange.svg
     :alt: All contributors
     :target: AUTHORS.rst
 
 Overview
 --------
 
-A simple librairy to build a vrt from multiple raster source relying only on rasterio
+A simple librairy to build a vrt from multiple raster source relying only on rasterio.
+
+.. code-block:: python
+
+    from rio_vrt import build_vrt
+
+    raster_files = ["example.tif", "example2.tif", "...", "examplen.tif"]
+    vrt_file = build_vrt("example.vrt", raster_files)
 
 Credits
 -------
 
 This package was created with `Cookiecutter <https://github.com/cookiecutter/cookiecutter>`__ and the `12rambau/pypackage <https://github.com/12rambau/pypackage>` project template.
```

### Comparing `rio-vrt-0.0.0/README.rst` & `rio-vrt-0.1.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -41,13 +41,20 @@
 .. image:: https://img.shields.io/badge/all_contributors-0-orange.svg
     :alt: All contributors
     :target: AUTHORS.rst
 
 Overview
 --------
 
-A simple librairy to build a vrt from multiple raster source relying only on rasterio
+A simple librairy to build a vrt from multiple raster source relying only on rasterio.
+
+.. code-block:: python
+
+    from rio_vrt import build_vrt
+
+    raster_files = ["example.tif", "example2.tif", "...", "examplen.tif"]
+    vrt_file = build_vrt("example.vrt", raster_files)
 
 Credits
 -------
 
 This package was created with `Cookiecutter <https://github.com/cookiecutter/cookiecutter>`__ and the `12rambau/pypackage <https://github.com/12rambau/pypackage>` project template.
```

### Comparing `rio-vrt-0.0.0/pyproject.toml` & `rio-vrt-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rio-vrt"
-version = "0.0.0"
+version = "0.1.0"
 description = "A simple librairy to build a vrt from multiple raster source relying only on rasterio"
 keywords = ["skeleton", "Python"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 requires-python = ">=3.6.9"
-dependencies = []
+dependencies = ["rasterio", ]
 
 [[project.authors]]
 name = "pierrick rambaud"
 email = "pierrick.rambaud49@gmail.com"
 
 [project.license]
 text = "MIT"
@@ -31,29 +31,29 @@
 content-type = "text/x-rst"
 
 [project.urls]
 Homepage = "https://github.com/12rambau/rio-vrt"
 
 [project.optional-dependencies]
 dev = ["pre-commit", "commitizen", "nox", "mypy"]
-test = ["pytest", "pytest-sugar", "pytest-cov", "pytest-deadfixtures"]
+test = ["pytest", "pytest-sugar", "pytest-cov", "pytest-deadfixtures", "pytest-regressions", "xmlschema", "natsort", "beautifulsoup4", "lxml"]
 doc = ["sphinx", "pydata-sphinx-theme", "sphinx-copybutton", "sphinx-design", "sphinx-icon", "sphinx-btn"]
 
 [tool.setuptools]
 include-package-data = false
 license-files = ["LICENSE.txt"]
 
 [tool.setuptools.packages.find]
 include = ["rio_vrt*"]
 exclude = ["docs*", "tests*"]
 
 [tool.commitizen]
 tag_format = "v$major.$minor.$patch$prerelease"
 update_changelog_on_bump = false
-version = "0.0.0"
+version = "0.1.0"
 version_files = [
     "pyproject.toml:version",
     "rio_vrt/__init__.py:__version__",
     "docs/conf.py:release"
 ]
 
 [tool.pytest.ini_options]
```

### Comparing `rio-vrt-0.0.0/rio_vrt.egg-info/PKG-INFO` & `rio-vrt-0.1.0/rio_vrt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-vrt
-Version: 0.0.0
+Version: 0.1.0
 Summary: A simple librairy to build a vrt from multiple raster source relying only on rasterio
 Author-email: pierrick rambaud <pierrick.rambaud49@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/12rambau/rio-vrt
 Keywords: skeleton,Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -62,13 +62,20 @@
 .. image:: https://img.shields.io/badge/all_contributors-0-orange.svg
     :alt: All contributors
     :target: AUTHORS.rst
 
 Overview
 --------
 
-A simple librairy to build a vrt from multiple raster source relying only on rasterio
+A simple librairy to build a vrt from multiple raster source relying only on rasterio.
+
+.. code-block:: python
+
+    from rio_vrt import build_vrt
+
+    raster_files = ["example.tif", "example2.tif", "...", "examplen.tif"]
+    vrt_file = build_vrt("example.vrt", raster_files)
 
 Credits
 -------
 
 This package was created with `Cookiecutter <https://github.com/cookiecutter/cookiecutter>`__ and the `12rambau/pypackage <https://github.com/12rambau/pypackage>` project template.
```

