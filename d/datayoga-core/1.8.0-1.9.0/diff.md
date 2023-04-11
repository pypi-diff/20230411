# Comparing `tmp/datayoga_core-1.8.0.tar.gz` & `tmp/datayoga_core-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datayoga_core-1.8.0.tar", max compression
+gzip compressed data, was "datayoga_core-1.9.0.tar", max compression
```

## Comparing `datayoga_core-1.8.0.tar` & `datayoga_core-1.9.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0    10712 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/README.md
--rw-r--r--   0        0        0     1479 2022-11-22 09:04:39.181166 datayoga_core-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     1987 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/__init__.py
--rw-r--r--   0        0        0     2287 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/block.py
--rw-r--r--   0        0        0        0 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/__init__.py
--rw-r--r--   0        0        0        0 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/add_field/__init__.py
--rw-r--r--   0        0        0     1413 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/add_field/block.py
--rw-r--r--   0        0        0     2062 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/add_field/block.schema.json
--rw-r--r--   0        0        0     1826 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py
--rw-r--r--   0        0        0        0 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/files/read_csv/__init__.py
--rw-r--r--   0        0        0     1047 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/files/read_csv/block.py
--rw-r--r--   0        0        0     1494 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/files/read_csv/block.schema.json
--rw-r--r--   0        0        0        0 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/filter/__init__.py
--rw-r--r--   0        0        0      766 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/filter/block.py
--rw-r--r--   0        0        0      464 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/filter/block.schema.json
--rw-r--r--   0        0        0     2572 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/filter/tests/test_filter.py
--rw-r--r--   0        0        0        0 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/map/__init__.py
--rw-r--r--   0        0        0     1077 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/map/block.py
--rw-r--r--   0        0        0      766 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/map/block.schema.json
--rw-r--r--   0        0        0        0 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/redis/read_stream/__init__.py
--rw-r--r--   0        0        0     2703 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/redis/read_stream/block.py
--rw-r--r--   0        0        0      586 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json
--rw-r--r--   0        0        0      493 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/redis/utils.py
--rw-r--r--   0        0        0        0 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/redis/write/__init__.py
--rw-r--r--   0        0        0     1439 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/redis/write/block.py
--rw-r--r--   0        0        0      605 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/redis/write/block.schema.json
--rw-r--r--   0        0        0        0 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/relational/write/__init__.py
--rw-r--r--   0        0        0     1650 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/relational/write/block.py
--rw-r--r--   0        0        0     2485 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/relational/write/block.schema.json
--rw-r--r--   0        0        0        0 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/remove_field/__init__.py
--rw-r--r--   0        0        0     1180 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/remove_field/block.py
--rw-r--r--   0        0        0     1182 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/remove_field/block.schema.json
--rw-r--r--   0        0        0     1907 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py
--rw-r--r--   0        0        0        0 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/rename_field/__init__.py
--rw-r--r--   0        0        0     1972 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/rename_field/block.py
--rw-r--r--   0        0        0     1716 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/rename_field/block.schema.json
--rw-r--r--   0        0        0     2282 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py
--rw-r--r--   0        0        0        0 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/sequence/__init__.py
--rw-r--r--   0        0        0      347 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/sequence/block.py
--rw-r--r--   0        0        0      517 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/sequence/block.schema.json
--rw-r--r--   0        0        0        0 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/std/read/__init__.py
--rw-r--r--   0        0        0     1263 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/std/read/block.py
--rw-r--r--   0        0        0       75 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/std/read/block.schema.json
--rw-r--r--   0        0        0        0 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/std/write/__init__.py
--rw-r--r--   0        0        0      862 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/std/write/block.py
--rw-r--r--   0        0        0       76 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/blocks/std/write/block.schema.json
--rw-r--r--   0        0        0      633 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/context.py
--rw-r--r--   0        0        0     5473 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/expression.py
--rw-r--r--   0        0        0     4546 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/jmespath_custom_functions.py
--rw-r--r--   0        0        0     4408 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/job.py
--rw-r--r--   0        0        0      712 2022-11-22 09:04:13.877360 datayoga_core-1.8.0/src/datayoga_core/producer.py
--rw-r--r--   0        0        0       23 2022-11-22 09:04:13.881360 datayoga_core-1.8.0/src/datayoga_core/resources/scaffold/.gitignore
--rw-r--r--   0        0        0      955 2022-11-22 09:04:13.881360 datayoga_core-1.8.0/src/datayoga_core/resources/scaffold/README.md
--rw-r--r--   0        0        0      154 2022-11-22 09:04:13.881360 datayoga_core-1.8.0/src/datayoga_core/resources/scaffold/connections.yaml
--rw-r--r--   0        0        0      188 2022-11-22 09:04:13.881360 datayoga_core-1.8.0/src/datayoga_core/resources/scaffold/data/sample.csv
--rw-r--r--   0        0        0      445 2022-11-22 09:04:13.881360 datayoga_core-1.8.0/src/datayoga_core/resources/scaffold/jobs/sample/hello.yaml
--rw-r--r--   0        0        0     2169 2022-11-22 09:04:13.881360 datayoga_core-1.8.0/src/datayoga_core/resources/schemas/connections.schema.json
--rw-r--r--   0        0        0     1757 2022-11-22 09:04:13.881360 datayoga_core-1.8.0/src/datayoga_core/resources/schemas/job.schema.json
--rw-r--r--   0        0        0     4378 2022-11-22 09:04:13.881360 datayoga_core-1.8.0/src/datayoga_core/step.py
--rw-r--r--   0        0        0     2356 2022-11-22 09:04:13.881360 datayoga_core-1.8.0/src/datayoga_core/utils.py
--rw-r--r--   0        0        0    13032 1970-01-01 00:00:00.000000 datayoga_core-1.8.0/setup.py
--rw-r--r--   0        0        0    12379 1970-01-01 00:00:00.000000 datayoga_core-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    10712 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/README.md
+-rw-r--r--   0        0        0     1479 2022-11-23 19:29:20.562231 datayoga_core-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1987 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/__init__.py
+-rw-r--r--   0        0        0     2287 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/block.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/__init__.py
+-rw-r--r--   0        0        0     1413 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/block.py
+-rw-r--r--   0        0        0     2062 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/block.schema.json
+-rw-r--r--   0        0        0     1826 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/files/read_csv/__init__.py
+-rw-r--r--   0        0        0     1047 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/files/read_csv/block.py
+-rw-r--r--   0        0        0     1494 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/files/read_csv/block.schema.json
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/filter/__init__.py
+-rw-r--r--   0        0        0      766 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/filter/block.py
+-rw-r--r--   0        0        0      464 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/filter/block.schema.json
+-rw-r--r--   0        0        0     2572 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/filter/tests/test_filter.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/map/__init__.py
+-rw-r--r--   0        0        0     1077 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/map/block.py
+-rw-r--r--   0        0        0      766 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/map/block.schema.json
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/read_stream/__init__.py
+-rw-r--r--   0        0        0     2703 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/read_stream/block.py
+-rw-r--r--   0        0        0      586 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json
+-rw-r--r--   0        0        0      493 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/utils.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/write/__init__.py
+-rw-r--r--   0        0        0     1439 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/write/block.py
+-rw-r--r--   0        0        0      605 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/redis/write/block.schema.json
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/relational/write/__init__.py
+-rw-r--r--   0        0        0     1650 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/relational/write/block.py
+-rw-r--r--   0        0        0     2485 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/relational/write/block.schema.json
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/__init__.py
+-rw-r--r--   0        0        0     1180 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/block.py
+-rw-r--r--   0        0        0     1182 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/block.schema.json
+-rw-r--r--   0        0        0     1907 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/__init__.py
+-rw-r--r--   0        0        0     1972 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/block.py
+-rw-r--r--   0        0        0     1716 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/block.schema.json
+-rw-r--r--   0        0        0     2282 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/sequence/__init__.py
+-rw-r--r--   0        0        0      347 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/sequence/block.py
+-rw-r--r--   0        0        0      517 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/sequence/block.schema.json
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/read/__init__.py
+-rw-r--r--   0        0        0     1263 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/read/block.py
+-rw-r--r--   0        0        0       75 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/read/block.schema.json
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/write/__init__.py
+-rw-r--r--   0        0        0      862 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/write/block.py
+-rw-r--r--   0        0        0       76 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/blocks/std/write/block.schema.json
+-rw-r--r--   0        0        0      633 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/context.py
+-rw-r--r--   0        0        0     5473 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/expression.py
+-rw-r--r--   0        0        0     4546 2022-11-23 19:28:55.950277 datayoga_core-1.9.0/src/datayoga_core/jmespath_custom_functions.py
+-rw-r--r--   0        0        0     4408 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/job.py
+-rw-r--r--   0        0        0      712 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/producer.py
+-rw-r--r--   0        0        0       23 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/.gitignore
+-rw-r--r--   0        0        0      955 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/README.md
+-rw-r--r--   0        0        0      154 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/connections.yaml
+-rw-r--r--   0        0        0      188 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/data/sample.csv
+-rw-r--r--   0        0        0      445 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/jobs/sample/hello.yaml
+-rw-r--r--   0        0        0     2226 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/schemas/connections.schema.json
+-rw-r--r--   0        0        0     1757 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/resources/schemas/job.schema.json
+-rw-r--r--   0        0        0     4378 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/step.py
+-rw-r--r--   0        0        0     2317 2022-11-23 19:28:55.954277 datayoga_core-1.9.0/src/datayoga_core/utils.py
+-rw-r--r--   0        0        0    13032 1970-01-01 00:00:00.000000 datayoga_core-1.9.0/setup.py
+-rw-r--r--   0        0        0    12379 1970-01-01 00:00:00.000000 datayoga_core-1.9.0/PKG-INFO
```

### Comparing `datayoga_core-1.8.0/README.md` & `datayoga_core-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/pyproject.toml` & `datayoga_core-1.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datayoga-core"
-version = "1.8.0"
+version = "1.9.0"
 description = "DataYoga for Python"
 authors = ["DataYoga <admin@datayoga.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 include = [
 ]
```

### Comparing `datayoga_core-1.8.0/src/datayoga_core/__init__.py` & `datayoga_core-1.9.0/src/datayoga_core/__init__.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/block.py` & `datayoga_core-1.9.0/src/datayoga_core/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/add_field/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/add_field/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/files/read_csv/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/files/read_csv/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/files/read_csv/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/files/read_csv/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/filter/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/filter/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/filter/tests/test_filter.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/filter/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/map/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/map/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/map/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/map/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/redis/read_stream/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/redis/read_stream/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/redis/write/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/redis/write/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/redis/write/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/redis/write/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/relational/write/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/relational/write/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/relational/write/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/relational/write/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/remove_field/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/remove_field/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/rename_field/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/rename_field/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/sequence/block.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/blocks/sequence/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/std/read/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/std/read/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/blocks/std/write/block.py` & `datayoga_core-1.9.0/src/datayoga_core/blocks/std/write/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/context.py` & `datayoga_core-1.9.0/src/datayoga_core/context.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/expression.py` & `datayoga_core-1.9.0/src/datayoga_core/expression.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/jmespath_custom_functions.py` & `datayoga_core-1.9.0/src/datayoga_core/jmespath_custom_functions.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/job.py` & `datayoga_core-1.9.0/src/datayoga_core/job.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/producer.py` & `datayoga_core-1.9.0/src/datayoga_core/producer.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/resources/scaffold/README.md` & `datayoga_core-1.9.0/src/datayoga_core/resources/scaffold/README.md`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/resources/schemas/connections.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/resources/schemas/connections.schema.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4444444444444444%*

 * *Differences: {"'additionalProperties'": 'False',*

 * * "'patternProperties'": "OrderedDict([('.', OrderedDict([('type', 'object'), ('anyOf', "*

 * *                        "[OrderedDict([('description', 'SQL database'), ('properties', "*

 * *                        "OrderedDict([('type', OrderedDict([('description', 'DB type'), ('type', "*

 * *                        "'string'), ('pattern', '^(?!redis$)')])), ('host', "*

 * *                        "OrderedDict([('description', 'DB host'), ('type', 'string')])), ('port', "*

 * *                      […]*

```diff
@@ -1,112 +1,107 @@
 {
+    "additionalProperties": false,
     "description": "Connection catalog",
-    "items": {
-        "anyOf": [
-            {
-                "additionalProperties": false,
-                "description": "SQL database",
-                "examples": [
-                    {
-                        "database": "postgres",
-                        "host": "localhost",
-                        "name": "hr",
-                        "password": "postgres",
-                        "port": 5432,
-                        "type": "postgresql",
-                        "user": "postgres"
-                    }
-                ],
-                "properties": {
-                    "database": {
-                        "description": "DB name",
-                        "type": "string"
-                    },
-                    "host": {
-                        "description": "DB host",
-                        "type": "string"
-                    },
-                    "name": {
-                        "description": "Connection name",
-                        "type": "string"
-                    },
-                    "password": {
-                        "description": "DB password",
-                        "type": "string"
-                    },
-                    "port": {
-                        "description": "DB port",
-                        "maximum": 65535,
-                        "minimum": 1,
-                        "type": "integer"
-                    },
-                    "type": {
-                        "description": "DB type",
-                        "pattern": "^(?!redis$)",
-                        "type": "string"
-                    },
-                    "user": {
-                        "description": "DB user",
-                        "type": "string"
-                    }
-                },
-                "required": [
-                    "type",
-                    "host",
-                    "database",
-                    "user"
-                ]
-            },
-            {
-                "additionalProperties": false,
-                "description": "Redis",
-                "examples": [
-                    {
-                        "host": "localhost",
-                        "name": "cache",
-                        "port": 6379,
-                        "type": "redis"
-                    }
-                ],
-                "properties": {
-                    "host": {
-                        "description": "Redis DB host",
-                        "type": "string"
-                    },
-                    "name": {
-                        "description": "Connection name",
-                        "type": "string"
-                    },
-                    "password": {
-                        "description": "Redis DB password",
-                        "type": "string"
-                    },
-                    "port": {
-                        "description": "Redis DB port",
-                        "maximum": 65535,
-                        "minimum": 1,
-                        "type": "integer"
-                    },
-                    "type": {
-                        "description": "DB type",
-                        "enum": [
-                            "redis"
-                        ],
-                        "type": "string"
-                    }
+    "patternProperties": {
+        ".": {
+            "anyOf": [
+                {
+                    "additionalProperties": false,
+                    "description": "SQL database",
+                    "examples": [
+                        {
+                            "database": "postgres",
+                            "host": "localhost",
+                            "name": "hr",
+                            "password": "postgres",
+                            "port": 5432,
+                            "type": "postgresql",
+                            "user": "postgres"
+                        }
+                    ],
+                    "properties": {
+                        "database": {
+                            "description": "DB name",
+                            "type": "string"
+                        },
+                        "host": {
+                            "description": "DB host",
+                            "type": "string"
+                        },
+                        "password": {
+                            "description": "DB password",
+                            "type": "string"
+                        },
+                        "port": {
+                            "description": "DB port",
+                            "maximum": 65535,
+                            "minimum": 1,
+                            "type": "integer"
+                        },
+                        "type": {
+                            "description": "DB type",
+                            "pattern": "^(?!redis$)",
+                            "type": "string"
+                        },
+                        "user": {
+                            "description": "DB user",
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "type",
+                        "host",
+                        "database",
+                        "user"
+                    ]
                 },
-                "required": [
-                    "name",
-                    "type",
-                    "host",
-                    "port"
-                ]
-            }
-        ],
-        "type": "object"
+                {
+                    "additionalProperties": false,
+                    "description": "Redis",
+                    "examples": [
+                        {
+                            "cache": {
+                                "host": "localhost",
+                                "port": 6379,
+                                "type": "redis"
+                            }
+                        }
+                    ],
+                    "properties": {
+                        "host": {
+                            "description": "Redis DB host",
+                            "type": "string"
+                        },
+                        "password": {
+                            "description": "Redis DB password",
+                            "type": "string"
+                        },
+                        "port": {
+                            "description": "Redis DB port",
+                            "maximum": 65535,
+                            "minimum": 1,
+                            "type": "integer"
+                        },
+                        "type": {
+                            "description": "DB type",
+                            "enum": [
+                                "redis"
+                            ],
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "type",
+                        "host",
+                        "port"
+                    ]
+                }
+            ],
+            "type": "object"
+        }
     },
     "title": "Connections",
     "type": [
-        "array",
+        "object",
         "null"
     ]
 }
```

### Comparing `datayoga_core-1.8.0/src/datayoga_core/resources/schemas/job.schema.json` & `datayoga_core-1.9.0/src/datayoga_core/resources/schemas/job.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/step.py` & `datayoga_core-1.9.0/src/datayoga_core/step.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.8.0/src/datayoga_core/utils.py` & `datayoga_core-1.9.0/src/datayoga_core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,12 +79,12 @@
 
 def unescape_field(field: str) -> str:
     return field.replace("\\.", ".")
 
 
 def get_connection_details(connection_name: str, context: Context) -> Dict[str, Any]:
     if context:
-        connection = next(filter(lambda x: x["name"] == connection_name, context.properties.get("connections")), None)
+        connection = context.properties.get("connections").get(connection_name)
         if connection:
             return connection
 
     raise ValueError(f"{connection_name} connection not found")
```

### Comparing `datayoga_core-1.8.0/setup.py` & `datayoga_core-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
           'testcontainers>=3.7.0,<4.0.0',
           'psycopg2>=2.9.3,<3.0.0',
           'redis>=4.1.4,<5.0.0',
           'SQLAlchemy>=1.4.41,<2.0.0']}
 
 setup_kwargs = {
     'name': 'datayoga-core',
-    'version': '1.8.0',
+    'version': '1.9.0',
     'description': 'DataYoga for Python',
     'long_description': '# DataYoga Core\n\n## Introduction\n\n`datayoga-core` is the transformation engine used in `DataYoga`, a framework for building and generating data pipelines.\n\n## Installation\n\n```bash\npip install datayoga-core\n```\n\n## Quick Start\n\nThis demonstrates how to transform data using a DataYoga job.\n\n### Create a Job\n\nUse this `example.yaml`:\n\n```yaml\n- steps:\n    - uses: add_field\n      with:\n        fields:\n          - field: full_name\n            language: jmespath\n            expression: concat([fname, \' \' , lname])\n          - field: country\n            language: sql\n            expression: country_code || \' - \' || UPPER(country_name)\n    - uses: rename_field\n      with:\n        fields:\n          - from_field: fname\n            to_field: first_name\n          - from_field: lname\n            to_field: last_name\n    - uses: remove_field\n      with:\n        fields:\n          - field: credit_card\n          - field: country_name\n          - field: country_code\n    - uses: map\n      with:\n        expression:\n          {\n            first_name: first_name,\n            last_name: last_name,\n            greeting: "\'Hello \' || CASE WHEN gender = \'F\' THEN \'Ms.\' WHEN gender = \'M\' THEN \'Mr.\' ELSE \'N/A\' END || \' \' || full_name",\n            country: country,\n            full_name: full_name,\n          }\n        language: sql\n```\n\n### Transform Data Using `datayoga-core`\n\nUse this code snippet to transform a data record using the job defined [above](#create-a-job):\n\n```python\nimport datayoga_core as dy\nfrom datayoga_core.job import Job\nfrom datayoga_core.utils import read_yaml\n\njob_settings = read_yaml("example.yaml")\njob = dy.compile(job_settings)\n\nassert job.transform({"fname": "jane", "lname": "smith", "country_code": 1, "country_name": "usa", "credit_card": "1234-5678-0000-9999", "gender": "F"}) == {"first_name": "jane", "last_name": "smith", "country": "1 - USA", "full_name": "jane smith", "greeting": "Hello Ms. jane smith"}\n```\n\nAs can be seen, the record has been transformed based on the job:\n\n- `fname` field renamed to `first_name`.\n- `lname` field renamed to `last_name`.\n- `country` field added based on an SQL expression.\n- `full_name` field added based on a [JMESPath](https://jmespath.org/) expression.\n- `greeting` field added based on an SQL expression.\n\n### Examples\n\n- Add a new field `country` out of an SQL expression that concatenates `country_code` and `country_name` fields after upper case the later:\n\n  ```yaml\n  uses: add_field\n  with:\n    field: country\n    language: sql\n    expression: country_code || \' - \' || UPPER(country_name)\n  ```\n\n- Rename `fname` field to `first_name` and `lname` field to `last_name`:\n\n  ```yaml\n  uses: rename_field\n  with:\n    fields:\n      - from_field: fname\n        to_field: first_name\n      - from_field: lname\n        to_field: last_name\n  ```\n\n- Remove `credit_card` field:\n\n  ```yaml\n  uses: remove_field\n  with:\n    field: credit_card\n  ```\n\nFor a full list of supported block types [see reference](https://datayoga-io.github.io/datayoga-py/).\n\n## Expression Language\n\nDataYoga supports both SQL and [JMESPath](https://jmespath.org/) expressions. JMESPath are especially useful to handle nested JSON data, while SQL is more suited to flat row-like structures.\n\n### Notes\n\n- Dot notation in expression represents nesting fields in the object, for example `name.first_name` refers to `{ "name": { "first_name": "John" } }`.\n- In order to refer to a field that contains a dot in its name, escape it, for example `name\\.first_name` refers to `{ "name.first_name": "John" }`.\n\n### JMESPath Custom Functions\n\nDataYoga adds the following custom functions to the standard JMESPath library:\n\n| Function             | Description                                                                                                                         | Example                                                                                                                                           | Comments                                                                                                                                                         |\n| -------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| `capitalize`         | Capitalizes all the words in the string                                                                                             | Input: `{"name": "john doe"}` <br /> Expression: `capitalize(name)` <br /> Output: `John Doe`                                                     |                                                                                                                                                                  |\n| `concat`             | Concatenates an array of variables or literals                                                                                      | Input: `{"fname": "john", "lname": "doe"}` <br /> Expression: `concat([fname, \' \' ,lname])` <br /> Output: `john doe`                             | This is equivalent to the more verbose built-in expression: `\' \'.join([fname,lname])`                                                                            |\n| `hash`               | Calculates a hash using the `hash_name` hash function and returns its hexadecimal representation                                    | Input: `{"some_str": "some_value"}` <br /> Expression: `hash(some_str, &#96;sha1&#96;)` <br /> Output: `8c818171573b03feeae08b0b4ffeb6999e3afc05` | Supported algorithms: sha1 (default), sha256, md5, sha384, sha3_384, blake2b, sha512, sha3_224, sha224, sha3_256, sha3_512, blake2s                              |\n| `left`               | Returns a specified number of characters from the start of a given text string                                                      | Input: `{"greeting": "hello world!"}` <br /> Expression: `` left(greeting, `5`) `` <br /> Output: `hello`                                         |                                                                                                                                                                  |\n| `lower`              | Converts all uppercase characters in a string into lowercase characters                                                             | Input: `{"fname": "John"}` <br /> Expression: `lower(fname)` <br /> Output: `john`                                                                |                                                                                                                                                                  |\n| `mid `               | Returns a specified number of characters from the middle of a given text string                                                     | Input: `{"greeting": "hello world!"}` <br /> Expression: `` mid(greeting, `4`, `3`) `` <br /> Output: `o w`                                       |                                                                                                                                                                  |\n| `replace`            | Replaces all the occurrences of a substring with a new one                                                                          | Input: `{"sentence": "one four three four!"}` <br /> Expression: `replace(sentence, \'four\', \'two\')` <br /> Output: `one two three two!`           |                                                                                                                                                                  |\n| `right`              | Returns a specified number of characters from the end of a given text string                                                        | Input: `{"greeting": "hello world!"}` <br /> Expression: `` right(greeting, `6`) `` <br /> Output: `world!`                                       |                                                                                                                                                                  |\n| `split`              | Splits a string into a list of strings after breaking the given string by the specified delimiter (comma by default)                | Input: `{"departments": "finance,hr,r&d"}` <br /> Expression: `split(departments)` <br /> Output: `[\'finance\', \'hr\', \'r&d\']`                      | Default delimiter is comma - a different delimiter can be passed to the function as the second argument, for example: `split(departments, \';\')`                  |\n| `time_delta_days`    | Returns the number of days between a given `dt` and now (positive) or the number of days that have passed from now (negative)       | Input: `{"dt": \'2021-10-06T18:56:16.701670+00:00\'}` <br /> Expression: `time_delta_days(dt)` <br /> Output: `365`                                 | If `dt` is a string, ISO datetime (2011-11-04T00:05:23+04:00, for example) is assumed. If `dt` is a number, Unix timestamp (1320365123, for example) is assumed. |\n| `time_delta_seconds` | Returns the number of seconds between a given `dt` and now (positive) or the number of seconds that have passed from now (negative) | Input: `{"dt": \'2021-10-06T18:56:16.701670+00:00\'}` <br /> Expression: `time_delta_days(dt)` <br /> Output: `31557600`                            | If `dt` is a string, ISO datetime (2011-11-04T00:05:23+04:00, for example) is assumed. If `dt` is a number, Unix timestamp (1320365123, for example) is assumed. |\n| `upper`              | Converts all lowercase characters in a string into uppercase characters                                                             | Input: `{"fname": "john"}` <br /> Expression: `upper(fname)` <br /> Output: `JOHN`                                                                |                                                                                                                                                                  |\n| `uuid`               | Generates a random UUID4 and returns it as a string in standard format                                                              | Input: None <br /> Expression: `uuid()` <br /> Output: `3264b35c-ff5d-44a8-8bc7-9be409dac2b7`                                                     |                                                                                                                                                                  |\n',
     'author': 'DataYoga',
     'author_email': 'admin@datayoga.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `datayoga_core-1.8.0/PKG-INFO` & `datayoga_core-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datayoga-core
-Version: 1.8.0
+Version: 1.9.0
 Summary: DataYoga for Python
 License: Apache-2.0
 Author: DataYoga
 Author-email: admin@datayoga.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

