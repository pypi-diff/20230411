# Comparing `tmp/rozklad_ontu_parser_makisukurisu-0.0.3.tar.gz` & `tmp/rozklad_ontu_parser_makisukurisu-0.0.3.1.tar.gz`

## Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.tar` & `rozklad_ontu_parser_makisukurisu-0.0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/requirements.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/run_lint.bat
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/run_lint.sh
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/__init__.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/example.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/__init__.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/base.py
--rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/dataclasses.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/enums.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/parser.py
--rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/sender.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/.gitignore
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/LICENSE
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/readme.md
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/requirements.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/run_lint.bat
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/run_lint.sh
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/ontu_parser/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/ontu_parser/example.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/ontu_parser/classes/__init__.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/ontu_parser/classes/base.py
+-rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/ontu_parser/classes/dataclasses.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/ontu_parser/classes/enums.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/ontu_parser/classes/parser.py
+-rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/ontu_parser/classes/sender.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/.gitignore
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/LICENSE
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/readme.md
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.1/PKG-INFO
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md` & `rozklad_ontu_parser_makisukurisu-0.0.3.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3/.github/workflows/pylint.yml` & `rozklad_ontu_parser_makisukurisu-0.0.3.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3/.github/workflows/python-publish.yml` & `rozklad_ontu_parser_makisukurisu-0.0.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/example.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.1/ontu_parser/example.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/base.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.1/ontu_parser/classes/base.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/dataclasses.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.1/ontu_parser/classes/dataclasses.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/enums.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.1/ontu_parser/classes/enums.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3/ontu_parser/classes/parser.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.1/ontu_parser/classes/parser.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3/LICENSE` & `rozklad_ontu_parser_makisukurisu-0.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3/pyproject.toml` & `rozklad_ontu_parser_makisukurisu-0.0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rozklad_ontu_parser_MakisuKurisu"
-version = "0.0.3"
+version = "0.0.3.1"
 authors = [
   {  name="Pavlo Pohorieltsev", email="667strets@gmail.com"  },
 ]
 description = "Package for parsing data from rozklad.ontu.edu.ua"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3/readme.md` & `rozklad_ontu_parser_makisukurisu-0.0.3.1/readme.md`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3/PKG-INFO` & `rozklad_ontu_parser_makisukurisu-0.0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rozklad_ontu_parser_MakisuKurisu
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: Package for parsing data from rozklad.ontu.edu.ua
 Project-URL: Homepage, https://github.com/makisukurisu/rozklad-ontu-parser
 Project-URL: Bug Tracker, https://github.com/makisukurisu/rozklad-ontu-parser/issues
 Author-email: Pavlo Pohorieltsev <667strets@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
```

