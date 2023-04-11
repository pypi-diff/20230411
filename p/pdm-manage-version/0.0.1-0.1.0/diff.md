# Comparing `tmp/pdm_manage_version-0.0.1.tar.gz` & `tmp/pdm_manage_version-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_manage_version-0.0.1.tar", last modified: Tue Apr 11 12:18:18 2023, max compression
+gzip compressed data, was "pdm_manage_version-0.1.0.tar", last modified: Tue Apr 11 12:21:35 2023, max compression
```

## Comparing `pdm_manage_version-0.0.1.tar` & `pdm_manage_version-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      252 2023-04-11 12:17:36.676681 pdm_manage_version-0.0.1/README.md
--rw-r--r--   0        0        0     1382 2023-04-11 12:15:45.127988 pdm_manage_version-0.0.1/plugin.py
--rw-r--r--   0        0        0      515 2023-04-11 12:18:18.067453 pdm_manage_version-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 pdm_manage_version-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      297 2023-04-11 12:19:23.905505 pdm_manage_version-0.1.0/README.md
+-rw-r--r--   0        0        0     1382 2023-04-11 12:15:45.127988 pdm_manage_version-0.1.0/plugin.py
+-rw-r--r--   0        0        0      514 2023-04-11 12:21:35.385621 pdm_manage_version-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 pdm_manage_version-0.1.0/PKG-INFO
```

### Comparing `pdm_manage_version-0.0.1/plugin.py` & `pdm_manage_version-0.1.0/plugin.py`

 * *Files identical despite different names*

### Comparing `pdm_manage_version-0.0.1/pyproject.toml` & `pdm_manage_version-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pdm>=2.5.2",
 ]
 
 [project]
 name = "pdm-manage-version"
-version = "0.0.1"
+version = "0.1.0"
 description = "`pdm version` working like `poetry version`"
 authors = [
     { name = "Marco Acierno", email = "marcoaciernoemail@gmail.com" },
 ]
 dependencies = [
     "packaging>=23.0",
 ]
-requires-python = ">=3.11"
+requires-python = ">=3.9"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points.pdm]
 version = "plugin:version"
```

### Comparing `pdm_manage_version-0.0.1/PKG-INFO` & `pdm_manage_version-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: pdm-manage-version
-Version: 0.0.1
+Version: 0.1.0
 Summary: `pdm version` working like `poetry version`
 Author-Email: Marco Acierno <marcoaciernoemail@gmail.com>
 License: MIT
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Requires-Dist: packaging>=23.0
 Description-Content-Type: text/markdown
 
 # pdm-manage-version
 
 Wanted something like `poetry version` in `pdm`
 
 ## Alternatives
 
 I found [https://github.com/abersheeran/pdm-version/](https://github.com/abersheeran/pdm-version/) but
 it doesn't really behave like `poetry version` unfortunately
+
+## ToDo:
+
+- [] Tests
+- [] Better bump logic
```

