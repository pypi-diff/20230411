# Comparing `tmp/fractal-specifications-2.3.0.tar.gz` & `tmp/fractal-specifications-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal-specifications-2.3.0.tar", last modified: Tue Mar  7 14:58:19 2023, max compression
+gzip compressed data, was "fractal-specifications-3.0.0.tar", last modified: Tue Apr 11 07:19:26 2023, max compression
```

## Comparing `fractal-specifications-2.3.0.tar` & `fractal-specifications-3.0.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0      187 2023-03-07 14:58:05.613916 fractal-specifications-2.3.0/.coveragerc
--rw-r--r--   0        0        0      100 2023-03-07 14:58:05.613916 fractal-specifications-2.3.0/.flake8
--rw-r--r--   0        0        0      965 2023-03-07 14:58:05.613916 fractal-specifications-2.3.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-03-07 14:58:05.613916 fractal-specifications-2.3.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-03-07 14:58:05.613916 fractal-specifications-2.3.0/.gitignore
--rw-r--r--   0        0        0      161 2023-03-07 14:58:05.613916 fractal-specifications-2.3.0/.isort.cfg
--rw-r--r--   0        0        0     1716 2023-03-07 14:58:05.613916 fractal-specifications-2.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/LICENSE
--rw-r--r--   0        0        0     1431 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/Makefile
--rw-r--r--   0        0        0    12347 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/README.md
--rw-r--r--   0        0        0      780 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/align_version.py
--rw-r--r--   0        0        0      157 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/contrib/django/__init__.py
--rw-r--r--   0        0        0     2679 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/contrib/django/specifications.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/contrib/elasticsearch/__init__.py
--rw-r--r--   0        0        0     3167 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/contrib/elasticsearch/specifications.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/contrib/google_firestore/__init__.py
--rw-r--r--   0        0        0     2381 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/contrib/google_firestore/specifications.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     2814 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/contrib/mongo/specifications.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/contrib/pandas/__init__.py
--rw-r--r--   0        0        0     4014 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/contrib/pandas/specifications.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1599 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/contrib/sqlalchemy/specifications.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/generic/__init__.py
--rw-r--r--   0        0        0     1968 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/generic/collections.py
--rw-r--r--   0        0        0     3665 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/generic/operators.py
--rw-r--r--   0        0        0     4129 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/fractal_specifications/generic/specification.py
--rw-r--r--   0        0        0     1661 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/setup.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/contrib/django/__init__.py
--rw-r--r--   0        0        0     2761 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/contrib/django/test_specifications.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/contrib/elasticsearch/__init__.py
--rw-r--r--   0        0        0     2447 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/contrib/elasticsearch/test_specifications.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/contrib/google_firestore/__init__.py
--rw-r--r--   0        0        0     1724 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/contrib/google_firestore/test_specifications.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     2205 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/contrib/mongo/test_specifications.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/contrib/pandas/__init__.py
--rw-r--r--   0        0        0     4709 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/contrib/pandas/test_specifications.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1153 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/contrib/sqlalchemy/test_specifications.py
--rw-r--r--   0        0        0       52 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     4032 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/fixtures/specifications.py
--rw-r--r--   0        0        0        0 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/generic/__init__.py
--rw-r--r--   0        0        0     3730 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/generic/test_collections.py
--rw-r--r--   0        0        0     2775 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/generic/test_operators.py
--rw-r--r--   0        0        0     1243 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/generic/test_serialization.py
--rw-r--r--   0        0        0     3721 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tests/generic/test_specification.py
--rw-r--r--   0        0        0      696 2023-03-07 14:58:05.617916 fractal-specifications-2.3.0/tox.ini
--rw-r--r--   0        0        0    13219 1970-01-01 00:00:00.000000 fractal-specifications-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/.coveragerc
+-rw-r--r--   0        0        0      100 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/.flake8
+-rw-r--r--   0        0        0      965 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/.gitignore
+-rw-r--r--   0        0        0      161 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/.isort.cfg
+-rw-r--r--   0        0        0     1716 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/LICENSE
+-rw-r--r--   0        0        0     1436 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/Makefile
+-rw-r--r--   0        0        0    14107 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/README.md
+-rw-r--r--   0        0        0      780 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/align_version.py
+-rw-r--r--   0        0        0      157 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/django/__init__.py
+-rw-r--r--   0        0        0     2679 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/django/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     3167 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/elasticsearch/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/google_firestore/__init__.py
+-rw-r--r--   0        0        0     2381 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/google_firestore/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     2814 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/mongo/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/pandas/__init__.py
+-rw-r--r--   0        0        0     4014 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/pandas/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1599 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/sqlalchemy/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/generic/__init__.py
+-rw-r--r--   0        0        0     1968 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/generic/collections.py
+-rw-r--r--   0        0        0     4863 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/generic/dsl_parser.py
+-rw-r--r--   0        0        0     4069 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/generic/operators.py
+-rw-r--r--   0        0        0     6528 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/generic/specification.py
+-rw-r--r--   0        0        0     1713 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/setup.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/django/__init__.py
+-rw-r--r--   0        0        0     2761 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/django/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     2447 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/elasticsearch/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/google_firestore/__init__.py
+-rw-r--r--   0        0        0     1724 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/google_firestore/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     2205 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/mongo/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/pandas/__init__.py
+-rw-r--r--   0        0        0     4709 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/pandas/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1153 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/sqlalchemy/test_specifications.py
+-rw-r--r--   0        0        0       52 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     4254 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/fixtures/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/generic/__init__.py
+-rw-r--r--   0        0        0     3730 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/generic/test_collections.py
+-rw-r--r--   0        0        0     3435 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/generic/test_operators.py
+-rw-r--r--   0        0        0     5601 2023-04-11 07:19:07.829229 fractal-specifications-3.0.0/tests/generic/test_serialization.py
+-rw-r--r--   0        0        0     3854 2023-04-11 07:19:07.829229 fractal-specifications-3.0.0/tests/generic/test_specification.py
+-rw-r--r--   0        0        0      705 2023-04-11 07:19:07.829229 fractal-specifications-3.0.0/tox.ini
+-rw-r--r--   0        0        0    14999 1970-01-01 00:00:00.000000 fractal-specifications-3.0.0/PKG-INFO
```

### Comparing `fractal-specifications-2.3.0/.github/workflows/build.yml` & `fractal-specifications-3.0.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/.github/workflows/publish.yml` & `fractal-specifications-3.0.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/.gitignore` & `fractal-specifications-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/.pre-commit-config.yaml` & `fractal-specifications-3.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/LICENSE` & `fractal-specifications-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/Makefile` & `fractal-specifications-3.0.0/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 coverage:  ## Run tests with coverage
 	rm .coverage ||:
 	rm coverage.xml ||:
 	pytest --cov fractal_specifications --cov-report=xml
 
 deps:  ## Install dependencies
 	python -m pip install --upgrade pip
-	python -m pip install black coverage flake8 flit isort mccabe mypy pylint pytest pytest-cov pytest-asyncio pytest-lazy-fixture tox tox-gh-actions pre-commit autoflake
+	python -m pip install black coverage flake8 flit isort lark mccabe mypy pylint pytest pytest-cov pytest-asyncio pytest-lazy-fixture tox tox-gh-actions pre-commit autoflake
 	pre-commit install
 
 lint:  ## Lint and static-check
 	pre-commit run --all-files
 
 publish:  ## Publish to PyPi
 	python -m flit publish
```

### Comparing `fractal-specifications-2.3.0/README.md` & `fractal-specifications-3.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -120,14 +120,61 @@
 
 Specifications can also be exported to JSON via `spec.dumps()`. This essentially is a `json.dumps()` call around `spec.to_dict()`.
 
 JSON specification strings can be loaded directly as Specification object via `Specification.loads(s)`.
 
 Via this mechanism, specifications can be used outside the application runtime environment. For example, in a database or sent via API.
 
+### Domain Specific Language (DSL)
+
+Apart from basic JSON serialization, Fractal Specifications also comes with a DSL.
+
+Example specifications DSL strings:
+
+- `field_name == 10`
+  - This is a simple comparison expression with a numerical value.
+- `name != 'John'`
+  - This is another comparison expression with a string value.
+- `age >= 18 && is_student == True`
+  - This is a logical AND operation between two comparison expressions and a boolean value.
+- `roles contains "admin" || roles contains "editor"`
+  - This is a logical OR operation between two values of a list field.
+- `!(active == True)`
+  - This is a negation of an expression.
+- `name in ['John', 'Jane']`
+  - This is an in_expression that checks if a field value is present in a list of values.
+- `email matches \"[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}\"`
+  - This is a regex match_expression that checks if a field value matches a given pattern.
+- `items contains "element"`
+  - This is a contains_expression that checks if a list field contains a given value
+    - Contains can sometimes also be used with substrings, e.g, when using `is_satisfied_by`.
+- `salary is None`
+  - This is an is_none_expression that checks if a field value is None.
+- `#`
+  - This is an empty_expression that represents an empty expression.
+
+Specifications can be loaded from a DSL string with `spec = Specification.load_dsl(dsl_string)`.\
+Specifications can be serialized to a DSL string using `spec.dump_dsl()`.
+
+Example:
+```python
+from dataclasses import dataclass
+
+from fractal_specifications.generic.specification import Specification
+
+
+@dataclass
+class Demo:
+    field: str
+
+
+spec = Specification.load_dsl("field matches 'f.{20}s'")
+spec.is_satisfied_by(Demo("fractal_specifications"))  # True
+```
+
 ## Contrib
 
 This library also comes with some additional helpers to integrate the specifications easier with existing backends,
 such as the Django ORM.
 
 ### Django
```

### Comparing `fractal-specifications-2.3.0/align_version.py` & `fractal-specifications-3.0.0/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/fractal_specifications/contrib/django/specifications.py` & `fractal-specifications-3.0.0/fractal_specifications/contrib/django/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/fractal_specifications/contrib/elasticsearch/specifications.py` & `fractal-specifications-3.0.0/fractal_specifications/contrib/elasticsearch/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/fractal_specifications/contrib/google_firestore/specifications.py` & `fractal-specifications-3.0.0/fractal_specifications/contrib/google_firestore/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/fractal_specifications/contrib/mongo/specifications.py` & `fractal-specifications-3.0.0/fractal_specifications/contrib/mongo/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/fractal_specifications/contrib/pandas/specifications.py` & `fractal-specifications-3.0.0/fractal_specifications/contrib/pandas/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/fractal_specifications/contrib/sqlalchemy/specifications.py` & `fractal-specifications-3.0.0/fractal_specifications/contrib/sqlalchemy/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/fractal_specifications/generic/collections.py` & `fractal-specifications-3.0.0/fractal_specifications/generic/collections.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/fractal_specifications/generic/operators.py` & `fractal-specifications-3.0.0/fractal_specifications/generic/operators.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,14 +67,27 @@
         return cls(field=d["field"], values=d["value"])
 
 
 class EqualsSpecification(FieldValueSpecification):
     def is_satisfied_by(self, obj: Any) -> bool:
         return getattr(obj, self.field) == self.value
 
+    @classmethod
+    def name(cls):
+        return "eq"
+
+
+class NotEqualsSpecification(FieldValueSpecification):
+    def is_satisfied_by(self, obj: Any) -> bool:
+        return getattr(obj, self.field) != self.value
+
+    @classmethod
+    def name(cls):
+        return "neq"
+
 
 class LessThanSpecification(FieldValueSpecification):
     def is_satisfied_by(self, obj: Any) -> bool:
         return getattr(obj, self.field) < self.value
 
     @classmethod
     def name(cls):
@@ -110,19 +123,22 @@
 
 class ContainsSpecification(FieldValueSpecification):
     def is_satisfied_by(self, obj: Any) -> bool:
         return self.value in getattr(obj, self.field)
 
 
 class RegexStringMatchSpecification(ContainsSpecification):
-    pass
+    def is_satisfied_by(self, obj: Any) -> bool:
+        import re
+
+        return bool(re.match(self.value, getattr(obj, self.field)))
 
     @classmethod
     def name(cls):
-        return "regex"
+        return "matches"
 
 
 class IsNoneSpecification(FieldValueSpecification):
     def __init__(self, field: str):
         super(IsNoneSpecification, self).__init__(field, None)
 
     def __str__(self):
```

### Comparing `fractal-specifications-2.3.0/pyproject.toml` & `fractal-specifications-3.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 [tool.poetry]
 name = "fractal-specifications"
-version = "2.3.0"
+version = "3.0.0"
 description = "Fractal Specifications is an implementation of the specification pattern for building SOLID logic for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
+[tool.poetry.dependencies]
+lark = "*"
+
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
 
 [tool.flit.metadata]
 module = "fractal_specifications"
 dist-name = "fractal-specifications"
@@ -20,15 +23,17 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python",
 ]
 description-file = "README.md"
-requires = []
+requires = [
+    "lark",
+]
 requires-python=">=3.8"
 
 [tool.flit.metadata.requires-extra]
 test = [
     "black",
     "flake8",
     "isort",
```

### Comparing `fractal-specifications-2.3.0/tests/contrib/django/test_specifications.py` & `fractal-specifications-3.0.0/tests/contrib/django/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/tests/contrib/elasticsearch/test_specifications.py` & `fractal-specifications-3.0.0/tests/contrib/elasticsearch/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/tests/contrib/google_firestore/test_specifications.py` & `fractal-specifications-3.0.0/tests/contrib/google_firestore/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/tests/contrib/mongo/test_specifications.py` & `fractal-specifications-3.0.0/tests/contrib/mongo/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/tests/contrib/pandas/test_specifications.py` & `fractal-specifications-3.0.0/tests/contrib/pandas/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/tests/contrib/sqlalchemy/test_specifications.py` & `fractal-specifications-3.0.0/tests/contrib/sqlalchemy/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/tests/fixtures/specifications.py` & `fractal-specifications-3.0.0/tests/fixtures/specifications.py`

 * *Files 7% similar despite different names*

```diff
@@ -125,26 +125,24 @@
 
 
 @pytest.fixture
 def complex_specification():
     from fractal_specifications.generic import operators
     from fractal_specifications.generic.specification import EmptySpecification
 
-    return operators.EqualsSpecification("id", 1) & operators.GreaterThanSpecification(
-        "price", 25
-    ) & operators.GreaterThanEqualSpecification(
-        "price", 25
-    ) & operators.LessThanSpecification(
-        "price", 25
-    ) & operators.LessThanEqualSpecification(
-        "price", 25
-    ) & operators.NotSpecification(
-        operators.IsNoneSpecification("name")
-    ) & operators.ContainsSpecification(
-        "field", "y"
-    ) & operators.InSpecification(
-        "field", [1, 2, 3]
-    ) & operators.RegexStringMatchSpecification(
-        "field", ".*abc.*"
-    ) | (
-        EmptySpecification() & EmptySpecification()
+    return (
+        operators.EqualsSpecification("id", 1)
+        & operators.EqualsSpecification("id", 1.5)
+        & operators.EqualsSpecification("id", False)
+        & operators.EqualsSpecification("id", True)
+        & operators.EqualsSpecification("id", None)
+        & operators.GreaterThanSpecification("price", 25)
+        & operators.GreaterThanEqualSpecification("price", 25)
+        & operators.LessThanSpecification("price", 25)
+        & operators.LessThanEqualSpecification("price", 25)
+        & operators.NotSpecification(operators.IsNoneSpecification("name"))
+        & operators.ContainsSpecification("field", "y")
+        | operators.NotEqualsSpecification("id", 1)
+        & operators.InSpecification("field", [1, 2, 3])
+        & operators.RegexStringMatchSpecification("field", ".*abc.*")
+        | (EmptySpecification() & EmptySpecification())
     )
```

### Comparing `fractal-specifications-2.3.0/tests/generic/test_collections.py` & `fractal-specifications-3.0.0/tests/generic/test_collections.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-2.3.0/tests/generic/test_operators.py` & `fractal-specifications-3.0.0/tests/generic/test_operators.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,17 @@
     FieldValueSpecification,
     GreaterThanEqualSpecification,
     GreaterThanSpecification,
     InSpecification,
     IsNoneSpecification,
     LessThanEqualSpecification,
     LessThanSpecification,
+    NotEqualsSpecification,
     NotSpecification,
+    RegexStringMatchSpecification,
 )
 
 
 def test_not_specification():
     spec = NotSpecification(EqualsSpecification("id", 2))
     DC = make_dataclass("DC", [("id", int)])
     assert spec.is_satisfied_by(DC(**dict(id=1)))
@@ -49,14 +51,20 @@
 
 def test_equals_specification():
     spec = EqualsSpecification("id", 1)
     DC = make_dataclass("DC", [("id", int)])
     assert spec.is_satisfied_by(DC(**dict(id=1)))
 
 
+def test_not_equals_specification():
+    spec = NotEqualsSpecification("id", 1)
+    DC = make_dataclass("DC", [("id", int)])
+    assert spec.is_satisfied_by(DC(**dict(id=2)))
+
+
 def test_less_than_specification():
     spec = LessThanSpecification("id", 2)
     DC = make_dataclass("DC", [("id", int)])
     assert spec.is_satisfied_by(DC(**dict(id=1)))
 
 
 def test_less_than_equal_specification():
@@ -79,14 +87,26 @@
 
 def test_contains_specification():
     spec = ContainsSpecification("name", "a")
     DC = make_dataclass("DC", [("name", str)])
     assert spec.is_satisfied_by(DC(**dict(name="fractal")))
 
 
+def test_list_contains_specification():
+    spec = ContainsSpecification("names", "fractal")
+    DC = make_dataclass("DC", [("names", list)])
+    assert spec.is_satisfied_by(DC(**dict(names=["fractal"])))
+
+
+def test_regex_string_match_specification():
+    spec = RegexStringMatchSpecification("name", "^f.*l$")
+    DC = make_dataclass("DC", [("name", str)])
+    assert spec.is_satisfied_by(DC(**dict(name="fractal")))
+
+
 def test_is_none_specification():
     spec = IsNoneSpecification("name")
     DC = make_dataclass("DC", [("name", str)])
     assert spec.is_satisfied_by(DC(**dict(name=None)))
 
 
 def test_is_none_specification_str():
```

### Comparing `fractal-specifications-2.3.0/tests/generic/test_specification.py` & `fractal-specifications-3.0.0/tests/generic/test_specification.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,42 +5,46 @@
     ContainsSpecification,
     EqualsSpecification,
     GreaterThanEqualSpecification,
     GreaterThanSpecification,
     InSpecification,
     LessThanEqualSpecification,
     LessThanSpecification,
+    RegexStringMatchSpecification,
 )
 from fractal_specifications.generic.specification import (
     EmptySpecification,
     Specification,
 )
 
 
 def test_parse():
     assert Specification.parse(id=1) == EqualsSpecification("id", 1)
     assert Specification.parse(id_x=1) == EqualsSpecification("id_x", 1)
     assert not Specification.parse(id__x=1)
-    assert Specification.parse(id__equals=1) == EqualsSpecification("id", 1)
+    assert Specification.parse(id__eq=1) == EqualsSpecification("id", 1)
     assert Specification.parse(id__in=[1]) == InSpecification("id", [1])
     assert Specification.parse(id__contains="a") == ContainsSpecification("id", "a")
+    assert Specification.parse(name__matches=r"^.*$") == RegexStringMatchSpecification(
+        "name", r"^.*$"
+    )
     assert Specification.parse(id__lt=1) == LessThanSpecification("id", 1)
     assert Specification.parse(id__lte=1) == LessThanEqualSpecification("id", 1)
     assert Specification.parse(id__gt=1) == GreaterThanSpecification("id", 1)
     assert Specification.parse(id__gte=1) == GreaterThanEqualSpecification("id", 1)
     assert Specification.parse(id=1, name="a") == AndSpecification(
         [EqualsSpecification("id", 1), EqualsSpecification("name", "a")]
     )
-    assert Specification.parse(id__equals=1, name__equals="a") == AndSpecification(
+    assert Specification.parse(id__eq=1, name__eq="a") == AndSpecification(
         [EqualsSpecification("id", 1), EqualsSpecification("name", "a")]
     )
-    assert Specification.parse(id__equals=1, name="a") == AndSpecification(
+    assert Specification.parse(id__eq=1, name="a") == AndSpecification(
         [EqualsSpecification("id", 1), EqualsSpecification("name", "a")]
     )
-    assert Specification.parse(id=1, name__equals="a") == AndSpecification(
+    assert Specification.parse(id=1, name__eq="a") == AndSpecification(
         [EqualsSpecification("id", 1), EqualsSpecification("name", "a")]
     )
     assert Specification.parse(id__gt=1, name__contains="a") == AndSpecification(
         [GreaterThanSpecification("id", 1), ContainsSpecification("name", "a")]
     )
```

### Comparing `fractal-specifications-2.3.0/tox.ini` & `fractal-specifications-3.0.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 [testenv]
 deps =
     black
     coverage
     flake8
     flit
     isort
+    lark
     mccabe
     mypy
     pylint
     pytest
     pytest-cov
     pytest-asyncio
     pytest-lazy-fixture
```

### Comparing `fractal-specifications-2.3.0/PKG-INFO` & `fractal-specifications-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: fractal-specifications
-Version: 2.3.0
+Version: 3.0.0
 Summary: Fractal Specifications is an implementation of the specification pattern for building SOLID logic for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal-specifications
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
+Requires-Dist: lark
 Requires-Dist: black ; extra == "test"
 Requires-Dist: flake8 ; extra == "test"
 Requires-Dist: isort ; extra == "test"
 Provides-Extra: test
 
 # Fractal Specifications
 
@@ -141,14 +142,61 @@
 
 Specifications can also be exported to JSON via `spec.dumps()`. This essentially is a `json.dumps()` call around `spec.to_dict()`.
 
 JSON specification strings can be loaded directly as Specification object via `Specification.loads(s)`.
 
 Via this mechanism, specifications can be used outside the application runtime environment. For example, in a database or sent via API.
 
+### Domain Specific Language (DSL)
+
+Apart from basic JSON serialization, Fractal Specifications also comes with a DSL.
+
+Example specifications DSL strings:
+
+- `field_name == 10`
+  - This is a simple comparison expression with a numerical value.
+- `name != 'John'`
+  - This is another comparison expression with a string value.
+- `age >= 18 && is_student == True`
+  - This is a logical AND operation between two comparison expressions and a boolean value.
+- `roles contains "admin" || roles contains "editor"`
+  - This is a logical OR operation between two values of a list field.
+- `!(active == True)`
+  - This is a negation of an expression.
+- `name in ['John', 'Jane']`
+  - This is an in_expression that checks if a field value is present in a list of values.
+- `email matches \"[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}\"`
+  - This is a regex match_expression that checks if a field value matches a given pattern.
+- `items contains "element"`
+  - This is a contains_expression that checks if a list field contains a given value
+    - Contains can sometimes also be used with substrings, e.g, when using `is_satisfied_by`.
+- `salary is None`
+  - This is an is_none_expression that checks if a field value is None.
+- `#`
+  - This is an empty_expression that represents an empty expression.
+
+Specifications can be loaded from a DSL string with `spec = Specification.load_dsl(dsl_string)`.\
+Specifications can be serialized to a DSL string using `spec.dump_dsl()`.
+
+Example:
+```python
+from dataclasses import dataclass
+
+from fractal_specifications.generic.specification import Specification
+
+
+@dataclass
+class Demo:
+    field: str
+
+
+spec = Specification.load_dsl("field matches 'f.{20}s'")
+spec.is_satisfied_by(Demo("fractal_specifications"))  # True
+```
+
 ## Contrib
 
 This library also comes with some additional helpers to integrate the specifications easier with existing backends,
 such as the Django ORM.
 
 ### Django
```

