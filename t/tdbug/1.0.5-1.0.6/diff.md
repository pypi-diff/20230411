# Comparing `tmp/tdbug-1.0.5.tar.gz` & `tmp/tdbug-1.0.6.tar.gz`

## Comparing `tdbug-1.0.5.tar` & `tdbug-1.0.6.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tdbug-1.0.5/MANIFEST.in
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 tdbug-1.0.5/setup.cfg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tdbug-1.0.5/tdbug/__init__.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tdbug-1.0.5/tdbug/main.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tdbug-1.0.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tdbug-1.0.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tdbug-1.0.5/README.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 tdbug-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 tdbug-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tdbug-1.0.6/MANIFEST.in
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 tdbug-1.0.6/setup.cfg
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 tdbug-1.0.6/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tdbug-1.0.6/tdbug/__init__.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tdbug-1.0.6/tdbug/main.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tdbug-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tdbug-1.0.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tdbug-1.0.6/README.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 tdbug-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 tdbug-1.0.6/PKG-INFO
```

### Comparing `tdbug-1.0.5/setup.cfg` & `tdbug-1.0.6/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tdbug
-version = 1.0.5
+version = 1.0.6
 author = Damon Pickett
 author_email = damon.pickett@gmail.com
 description = tdbug is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/damonpickett/tdbug
 classifiers =
```

### Comparing `tdbug-1.0.5/tdbug/main.py` & `tdbug-1.0.6/tdbug/main.py`

 * *Files identical despite different names*

### Comparing `tdbug-1.0.5/LICENSE` & `tdbug-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tdbug-1.0.5/pyproject.toml` & `tdbug-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tdbug"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Damon Pickett", email="damon.pickett@gmail.com" },
 ]
 description = "tdbug is a command-line application that uses the OpenAI API to diagnose bugs when programming."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tdbug-1.0.5/PKG-INFO` & `tdbug-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdbug
-Version: 1.0.5
+Version: 1.0.6
 Summary: tdbug is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 Project-URL: Homepage, https://github.com/damonpickett/tdbug
 Project-URL: Bug Tracker, https://github.com/damonpickett/tdbug/issues
 Author-email: Damon Pickett <damon.pickett@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

