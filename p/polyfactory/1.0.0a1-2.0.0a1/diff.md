# Comparing `tmp/polyfactory-1.0.0a1.tar.gz` & `tmp/polyfactory-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-1.0.0a1.tar", max compression
+gzip compressed data, was "polyfactory-2.0.0a1.tar", max compression
```

## Comparing `polyfactory-1.0.0a1.tar` & `polyfactory-2.0.0a1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1092 2023-04-11 09:49:18.437820 polyfactory-1.0.0a1/LICENSE
--rw-r--r--   0        0        0     4513 2023-04-11 09:49:18.437820 polyfactory-1.0.0a1/README.md
--rw-r--r--   0        0        0      425 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/__init__.py
--rw-r--r--   0        0        0      605 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/constants.py
--rw-r--r--   0        0        0      578 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    26088 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2757 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1603 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     1074 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0     9542 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1471 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     1976 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3328 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/fields.py
--rw-r--r--   0        0        0     1191 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/py.typed
--rw-r--r--   0        0        0     2890 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     2162 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3401 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     3311 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1838 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1069 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13431 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0     3845 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0     3633 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6185 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     5964 2023-04-11 09:49:18.441820 polyfactory-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     6538 1970-01-01 00:00:00.000000 polyfactory-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-11 13:54:46.061917 polyfactory-2.0.0a1/LICENSE
+-rw-r--r--   0        0        0     4513 2023-04-11 13:54:46.061917 polyfactory-2.0.0a1/README.md
+-rw-r--r--   0        0        0      425 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/__init__.py
+-rw-r--r--   0        0        0      605 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/constants.py
+-rw-r--r--   0        0        0      591 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    26088 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2757 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1603 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     1074 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0     9542 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1471 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     1976 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3328 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/fields.py
+-rw-r--r--   0        0        0     1191 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/py.typed
+-rw-r--r--   0        0        0     2890 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     2162 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3401 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     3311 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1838 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1069 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13431 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0     3845 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0     3633 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6185 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     5964 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     6538 1970-01-01 00:00:00.000000 polyfactory-2.0.0a1/PKG-INFO
```

### Comparing `polyfactory-1.0.0a1/LICENSE` & `polyfactory-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/README.md` & `polyfactory-2.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/constants.py` & `polyfactory-2.0.0a1/polyfactory/constants.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/exceptions.py` & `polyfactory-2.0.0a1/polyfactory/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,9 +10,9 @@
     """Parameter exception - used when wrong parameters are used"""
 
 
 class MissingBuildKwargException(FactoryException):
     """Missing Build Kwarg exception - used when a required build kwarg is not provided"""
 
 
-class MissingDependencyException(FactoryException):
+class MissingDependencyException(FactoryException, ImportError):
     """Missing dependency exception - used when a dependency is not installed"""
```

### Comparing `polyfactory-1.0.0a1/polyfactory/factories/base.py` & `polyfactory-2.0.0a1/polyfactory/factories/base.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.0.0a1/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.0.0a1/polyfactory/factories/dataclass_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.0.0a1/polyfactory/factories/odmantic_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.0.0a1/polyfactory/factories/pydantic_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.0.0a1/polyfactory/factories/typed_dict_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/field_meta.py` & `polyfactory-2.0.0a1/polyfactory/field_meta.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/fields.py` & `polyfactory-2.0.0a1/polyfactory/fields.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/persistence.py` & `polyfactory-2.0.0a1/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/pytest_plugin.py` & `polyfactory-2.0.0a1/polyfactory/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/utils/helpers.py` & `polyfactory-2.0.0a1/polyfactory/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/utils/predicates.py` & `polyfactory-2.0.0a1/polyfactory/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/value_generators/complex_types.py` & `polyfactory-2.0.0a1/polyfactory/value_generators/complex_types.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.0.0a1/polyfactory/value_generators/constrained_collections.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.0.0a1/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.0.0a1/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.0.0a1/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/value_generators/primitives.py` & `polyfactory-2.0.0a1/polyfactory/value_generators/primitives.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/polyfactory/value_generators/regex.py` & `polyfactory-2.0.0a1/polyfactory/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `polyfactory-1.0.0a1/pyproject.toml` & `polyfactory-2.0.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyfactory"
-version = "1.0.0alpha1"
+version = "2.0.0alpha1"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
 ]
```

### Comparing `polyfactory-1.0.0a1/PKG-INFO` & `polyfactory-2.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 1.0.0a1
+Version: 2.0.0a1
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
 Keywords: dataclasses,factory,faker,mock,pydantic,pytest,litestar,tdd,testing,typeddict
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
```

