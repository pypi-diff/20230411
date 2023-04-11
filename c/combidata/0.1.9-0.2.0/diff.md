# Comparing `tmp/combidata-0.1.9.tar.gz` & `tmp/combidata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combidata-0.1.9.tar", last modified: Wed Apr  5 09:38:00 2023, max compression
+gzip compressed data, was "combidata-0.2.0.tar", last modified: Tue Apr 11 20:55:05 2023, max compression
```

## Comparing `combidata-0.1.9.tar` & `combidata-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 09:38:00.008717 combidata-0.1.9/
--rw-rw-rw-   0        0        0     1083 2022-11-07 15:57:18.000000 combidata-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     9967 2023-04-05 09:38:00.007722 combidata-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     9185 2023-04-05 09:37:29.000000 combidata-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 09:37:59.957642 combidata-0.1.9/combidata/
--rw-rw-rw-   0        0        0      395 2023-02-10 13:56:29.000000 combidata-0.1.9/combidata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 09:37:59.989640 combidata-0.1.9/combidata/classes/
--rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.1.9/combidata/classes/__init__.py
--rw-rw-rw-   0        0        0     2831 2023-04-01 06:03:08.000000 combidata-0.1.9/combidata/classes/case.py
--rw-rw-rw-   0        0        0     1827 2023-03-02 18:36:48.000000 combidata-0.1.9/combidata/classes/combination.py
--rw-rw-rw-   0        0        0     5584 2023-04-05 09:37:29.000000 combidata-0.1.9/combidata/classes/data_generator.py
--rw-rw-rw-   0        0        0      351 2023-03-02 16:58:22.000000 combidata-0.1.9/combidata/classes/process.py
-drwxrwxrwx   0        0        0        0 2023-04-05 09:38:00.003705 combidata-0.1.9/combidata/processes/
--rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.1.9/combidata/processes/__init__.py
--rw-rw-rw-   0        0        0     5249 2023-04-01 05:47:28.000000 combidata-0.1.9/combidata/processes/combine.py
--rw-rw-rw-   0        0        0      655 2023-02-16 18:09:16.000000 combidata-0.1.9/combidata/processes/form.py
--rw-rw-rw-   0        0        0     1924 2023-04-01 06:30:40.000000 combidata-0.1.9/combidata/processes/genetate.py
-drwxrwxrwx   0        0        0        0 2023-04-05 09:37:59.979459 combidata-0.1.9/combidata.egg-info/
--rw-rw-rw-   0        0        0     9967 2023-04-05 09:37:59.000000 combidata-0.1.9/combidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-04-05 09:37:59.000000 combidata-0.1.9/combidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 09:37:59.000000 combidata-0.1.9/combidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-05 09:37:59.000000 combidata-0.1.9/combidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      553 2023-04-05 09:37:29.000000 combidata-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-05 09:38:00.008717 combidata-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1074 2023-04-05 09:37:29.000000 combidata-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-05 09:38:00.005753 combidata-0.1.9/tests/
--rw-rw-rw-   0        0        0     3111 2023-04-05 09:25:54.000000 combidata-0.1.9/tests/test_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:55:05.039178 combidata-0.2.0/
+-rw-rw-rw-   0        0        0     1083 2022-11-07 15:57:18.000000 combidata-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0    10026 2023-04-11 20:55:05.038179 combidata-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9245 2023-04-11 20:54:40.000000 combidata-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 20:55:05.007179 combidata-0.2.0/combidata/
+-rw-rw-rw-   0        0        0      395 2023-02-10 13:56:29.000000 combidata-0.2.0/combidata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:55:05.031177 combidata-0.2.0/combidata/classes/
+-rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.0/combidata/classes/__init__.py
+-rw-rw-rw-   0        0        0     2831 2023-04-01 06:03:08.000000 combidata-0.2.0/combidata/classes/case.py
+-rw-rw-rw-   0        0        0     1827 2023-03-02 18:36:48.000000 combidata-0.2.0/combidata/classes/combination.py
+-rw-rw-rw-   0        0        0     5780 2023-04-10 17:49:35.000000 combidata-0.2.0/combidata/classes/data_generator.py
+-rw-rw-rw-   0        0        0      351 2023-03-02 16:58:22.000000 combidata-0.2.0/combidata/classes/process.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:55:05.036179 combidata-0.2.0/combidata/processes/
+-rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.0/combidata/processes/__init__.py
+-rw-rw-rw-   0        0        0     5249 2023-04-01 05:47:28.000000 combidata-0.2.0/combidata/processes/combine.py
+-rw-rw-rw-   0        0        0      655 2023-02-16 18:09:16.000000 combidata-0.2.0/combidata/processes/form.py
+-rw-rw-rw-   0        0        0     1924 2023-04-01 06:30:40.000000 combidata-0.2.0/combidata/processes/genetate.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:55:05.025179 combidata-0.2.0/combidata.egg-info/
+-rw-rw-rw-   0        0        0    10026 2023-04-11 20:55:04.000000 combidata-0.2.0/combidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-04-11 20:55:04.000000 combidata-0.2.0/combidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 20:55:04.000000 combidata-0.2.0/combidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-11 20:55:04.000000 combidata-0.2.0/combidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      553 2023-04-11 20:52:22.000000 combidata-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 20:55:05.039178 combidata-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1073 2023-04-11 20:54:40.000000 combidata-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:55:05.037178 combidata-0.2.0/tests/
+-rw-rw-rw-   0        0        0     3111 2023-04-05 09:25:54.000000 combidata-0.2.0/tests/test_generator.py
```

### Comparing `combidata-0.1.9/LICENSE` & `combidata-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `combidata-0.1.9/PKG-INFO` & `combidata-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: combidata
-Version: 0.1.9
+Version: 0.2.0
 Summary: Package for random data generation, combination and data prepare for tests
 Home-page: https://github.com/Warrfie/combidata
 Author: Kuklikov Maxim (Warrfie)
 Author-email: "MaximKuklikov(Warrfie)" <warrfie@gmail.com>
 Project-URL: Homepage, https://github.com/Warrfie/combidata
 Keywords: QA,SET,random data generation,testing API,testing,autotesting
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,18 +27,22 @@
 
 
 The core functionality of the Combidata library is provided by the `DataGenerator` class, which takes in test flags and a dictionary containing all cases, forms, and workflows. 
 The `DataGenerator` creates `Combination` instances from the possible cases. 
 The `run` function in each `Combination` instance processes all steps in the specified workflow.
 
 ## New features
-1.0.9:
+0.2.0:
+1) Ok, now its Beta ;)
+2) Fixed combination bug
+
+0.1.9:
 1) Now you can use 'types_for_generation' in initialisation of 'DataGenerator'
 
-1.0.8:
+0.1.8:
 1) Now you can use multiply symbols modes
 2) Generate any number of data combinations, even if there are only a few cases.
 3) Use the `get_one()` function in the `DataGenerator` class for generating a single Combination object.
 
 ## Structure of input library
 
 ```python
```

### Comparing `combidata-0.1.9/README.md` & `combidata-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,22 @@
 
 
 The core functionality of the Combidata library is provided by the `DataGenerator` class, which takes in test flags and a dictionary containing all cases, forms, and workflows. 
 The `DataGenerator` creates `Combination` instances from the possible cases. 
 The `run` function in each `Combination` instance processes all steps in the specified workflow.
 
 ## New features
-1.0.9:
+0.2.0:
+1) Ok, now its Beta ;)
+2) Fixed combination bug
+
+0.1.9:
 1) Now you can use 'types_for_generation' in initialisation of 'DataGenerator'
 
-1.0.8:
+0.1.8:
 1) Now you can use multiply symbols modes
 2) Generate any number of data combinations, even if there are only a few cases.
 3) Use the `get_one()` function in the `DataGenerator` class for generating a single Combination object.
 
 ## Structure of input library
 
 ```python
```

### Comparing `combidata-0.1.9/combidata/classes/case.py` & `combidata-0.2.0/combidata/classes/case.py`

 * *Files identical despite different names*

### Comparing `combidata-0.1.9/combidata/classes/combination.py` & `combidata-0.2.0/combidata/classes/combination.py`

 * *Files identical despite different names*

### Comparing `combidata-0.1.9/combidata/classes/data_generator.py` & `combidata-0.2.0/combidata/classes/data_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,21 +72,26 @@
                  types_for_generation: None | str | list = None,
                  amount: int = None):
         assert amount is None or (isinstance(amount, int) and amount > 0), "amount must be integer > 0"
         assert banned_fields is None or isinstance(banned_fields, list), "banned_fields must be list instance"
         assert possible_fields is None or isinstance(possible_fields, list), "possible_fields must be list instance"
         assert banned_fields is None or possible_fields is None, "You can't use banned_fields and possible_fields arguments simultaneously"
 
+        if possible_modes is not None:
+            for key, value in possible_modes.items():
+                if isinstance(value, str):
+                    possible_modes[key] = [value]
+
         self.init_lib = {}
         for field_name, field in library["cases"].items():
             self.init_lib[field_name] = {}
             for field_mode, case in field.items():
                 self.init_lib[field_name].update(
                     {field_mode: (case if isinstance(case, Case) else Case(case, field_name, field_mode))})
-                if possible_modes is not None and field_name in possible_modes.keys() and field_mode != possible_modes[
+                if possible_modes is not None and field_name in possible_modes.keys() and field_mode not in possible_modes[
                     field_name]:
                     self.init_lib[field_name][field_mode].type_of_case = "OFF"
 
         if possible_fields is not None or banned_fields is not None:
             banned_fields = banned_fields if possible_fields is None else [field for field in self.init_lib.keys() if
                                                                            field not in possible_fields]
             for field in banned_fields:
```

### Comparing `combidata-0.1.9/combidata/processes/combine.py` & `combidata-0.2.0/combidata/processes/combine.py`

 * *Files identical despite different names*

### Comparing `combidata-0.1.9/combidata/processes/form.py` & `combidata-0.2.0/combidata/processes/form.py`

 * *Files identical despite different names*

### Comparing `combidata-0.1.9/combidata/processes/genetate.py` & `combidata-0.2.0/combidata/processes/genetate.py`

 * *Files identical despite different names*

### Comparing `combidata-0.1.9/combidata.egg-info/PKG-INFO` & `combidata-0.2.0/combidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: combidata
-Version: 0.1.9
+Version: 0.2.0
 Summary: Package for random data generation, combination and data prepare for tests
 Home-page: https://github.com/Warrfie/combidata
 Author: Kuklikov Maxim (Warrfie)
 Author-email: "MaximKuklikov(Warrfie)" <warrfie@gmail.com>
 Project-URL: Homepage, https://github.com/Warrfie/combidata
 Keywords: QA,SET,random data generation,testing API,testing,autotesting
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,18 +27,22 @@
 
 
 The core functionality of the Combidata library is provided by the `DataGenerator` class, which takes in test flags and a dictionary containing all cases, forms, and workflows. 
 The `DataGenerator` creates `Combination` instances from the possible cases. 
 The `run` function in each `Combination` instance processes all steps in the specified workflow.
 
 ## New features
-1.0.9:
+0.2.0:
+1) Ok, now its Beta ;)
+2) Fixed combination bug
+
+0.1.9:
 1) Now you can use 'types_for_generation' in initialisation of 'DataGenerator'
 
-1.0.8:
+0.1.8:
 1) Now you can use multiply symbols modes
 2) Generate any number of data combinations, even if there are only a few cases.
 3) Use the `get_one()` function in the `DataGenerator` class for generating a single Combination object.
 
 ## Structure of input library
 
 ```python
```

### Comparing `combidata-0.1.9/pyproject.toml` & `combidata-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
     "testing API",
     "testing",
     "autotesting"
 ]
 urls = {Homepage = "https://github.com/Warrfie/combidata"}
 authors = [{name = "MaximKuklikov(Warrfie)", email = "warrfie@gmail.com"}]
 requires-python = ">=3.10"
-version="0.1.9"
+version="0.2.0"
```

### Comparing `combidata-0.1.9/setup.py` & `combidata-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="combidata",
-    version="0.1.9",
+    version="0.2.0",
     description="Package for random data generation and combination different cases",
     long_description=long_description,
     url="https://github.com/Warrfie/combidata",
     author="Kuklikov Maxim (Warrfie)",
     author_email="warrfie@gmail.com",
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Information Technology",
         "Topic :: Software Development :: Quality Assurance",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
     ],
     keywords="QA, random data, data generation, testing API, testing, autotesting",
     packages=find_packages(),
```

### Comparing `combidata-0.1.9/tests/test_generator.py` & `combidata-0.2.0/tests/test_generator.py`

 * *Files identical despite different names*

