# Comparing `tmp/goodcrap-0.2.1.tar.gz` & `tmp/goodcrap-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodcrap-0.2.1.tar", last modified: Sun Apr  9 16:31:20 2023, max compression
+gzip compressed data, was "goodcrap-0.2.2.tar", last modified: Tue Apr 11 04:43:02 2023, max compression
```

## Comparing `goodcrap-0.2.1.tar` & `goodcrap-0.2.2.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.443144 goodcrap-0.2.1/
--rw-rw-rw-   0        0        0       66 2023-03-29 13:09:13.000000 goodcrap-0.2.1/.gitattributes
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.371122 goodcrap-0.2.1/.github/
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.392992 goodcrap-0.2.1/.github/workflows/
--rw-rw-rw-   0        0        0      576 2023-04-05 03:09:29.000000 goodcrap-0.2.1/.github/workflows/pylint.yml
--rw-rw-rw-   0        0        0       54 2023-04-09 16:29:54.000000 goodcrap-0.2.1/.gitignore
--rw-rw-rw-   0        0        0      332 2023-04-07 02:10:51.000000 goodcrap-0.2.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1574 2023-04-05 01:05:21.000000 goodcrap-0.2.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0    35802 2023-03-29 13:09:13.000000 goodcrap-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      193 2023-04-07 02:11:43.000000 goodcrap-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0    11178 2023-04-09 16:31:20.443144 goodcrap-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    10544 2023-04-09 16:30:52.000000 goodcrap-0.2.1/README.md
--rw-rw-rw-   0        0        0        5 2023-04-08 02:20:55.000000 goodcrap-0.2.1/VERSION
--rw-rw-rw-   0        0        0    72291 2023-04-07 05:50:59.000000 goodcrap-0.2.1/customers.parquet
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.393124 goodcrap-0.2.1/examples/
--rw-rw-rw-   0        0        0      139 2023-04-04 14:07:32.000000 goodcrap-0.2.1/examples/mysql_config.json
--rw-rw-rw-   0        0        0       59 2023-04-05 01:09:16.000000 goodcrap-0.2.1/examples/sqlite_config.json
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.393124 goodcrap-0.2.1/goodcrap/
--rw-rw-rw-   0        0        0       87 2023-04-08 02:21:05.000000 goodcrap-0.2.1/goodcrap/__init__.py
--rw-rw-rw-   0        0        0       72 2023-04-04 00:49:25.000000 goodcrap-0.2.1/goodcrap/__main__.py
--rw-rw-rw-   0        0        0     5755 2023-04-09 15:59:05.000000 goodcrap-0.2.1/goodcrap/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.409045 goodcrap-0.2.1/goodcrap/crappers/
--rw-rw-rw-   0        0        0     1019 2023-04-08 15:25:53.000000 goodcrap-0.2.1/goodcrap/crappers/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-04-09 16:23:36.000000 goodcrap-0.2.1/goodcrap/crappers/queries.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.409045 goodcrap-0.2.1/goodcrap/data_warehouses/
--rw-rw-rw-   0        0        0        0 2023-04-05 14:10:31.000000 goodcrap-0.2.1/goodcrap/data_warehouses/__init__.py
--rw-rw-rw-   0        0        0     2283 2023-04-08 15:13:42.000000 goodcrap-0.2.1/goodcrap/data_warehouses/dimension_featurizer.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.426149 goodcrap-0.2.1/goodcrap/databases/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:02:02.000000 goodcrap-0.2.1/goodcrap/databases/__init__.py
--rw-rw-rw-   0        0        0     3184 2023-04-09 16:30:44.000000 goodcrap-0.2.1/goodcrap/databases/database.py
--rw-rw-rw-   0        0        0      532 2023-04-07 06:19:36.000000 goodcrap-0.2.1/goodcrap/databases/mysql.py
--rw-rw-rw-   0        0        0      194 2023-04-07 06:53:45.000000 goodcrap-0.2.1/goodcrap/databases/queries.py
--rw-rw-rw-   0        0        0      379 2023-04-07 06:19:48.000000 goodcrap-0.2.1/goodcrap/databases/sqlite.py
--rw-rw-rw-   0        0        0    13362 2023-04-09 15:54:21.000000 goodcrap-0.2.1/goodcrap/goodcrap.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.426149 goodcrap-0.2.1/goodcrap/pipelines/
--rw-rw-rw-   0        0        0      560 2023-04-05 15:59:55.000000 goodcrap-0.2.1/goodcrap/pipelines/README.md
--rw-rw-rw-   0        0        0        0 2023-04-05 15:01:30.000000 goodcrap-0.2.1/goodcrap/pipelines/__init__.py
--rw-rw-rw-   0        0        0     3608 2023-04-07 06:10:04.000000 goodcrap-0.2.1/goodcrap/pipelines/mage.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.426149 goodcrap-0.2.1/goodcrap/pipelines/templates/
--rw-rw-rw-   0        0        0        0 2023-04-05 15:01:30.000000 goodcrap-0.2.1/goodcrap/pipelines/templates/__init__.py
--rw-rw-rw-   0        0        0     1122 2023-04-07 06:20:36.000000 goodcrap-0.2.1/goodcrap/pipelines/templates/data_exporter_mysql.py
--rw-rw-rw-   0        0        0      683 2023-04-07 06:10:42.000000 goodcrap-0.2.1/goodcrap/pipelines/templates/data_loader.py
--rw-rw-rw-   0        0        0      832 2023-04-06 06:10:32.000000 goodcrap-0.2.1/goodcrap/pipelines/templates/metadata.yaml
--rw-rw-rw-   0        0        0     2525 2023-04-09 16:25:30.000000 goodcrap-0.2.1/goodcrap/random_mapper.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.426149 goodcrap-0.2.1/goodcrap/templates/
--rw-rw-rw-   0        0        0        0 2023-03-31 13:15:48.000000 goodcrap-0.2.1/goodcrap/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.426149 goodcrap-0.2.1/goodcrap/templates/__pycache__/
--rw-rw-rw-   0        0        0      143 2023-03-31 13:16:56.000000 goodcrap-0.2.1/goodcrap/templates/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.438887 goodcrap-0.2.1/goodcrap/templates/data_warehouses/
--rw-rw-rw-   0        0        0     3459 2023-04-08 14:48:01.000000 goodcrap-0.2.1/goodcrap/templates/data_warehouses/sales.sql
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.376597 goodcrap-0.2.1/goodcrap/templates/databases/
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.441068 goodcrap-0.2.1/goodcrap/templates/databases/customers_orders/
--rw-rw-rw-   0        0        0      751 2023-04-04 05:53:19.000000 goodcrap-0.2.1/goodcrap/templates/databases/customers_orders/customers_orders.crap_labels.json
--rw-rw-rw-   0        0        0     1148 2023-04-06 15:06:31.000000 goodcrap-0.2.1/goodcrap/templates/databases/customers_orders/customers_orders.sql
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.377596 goodcrap-0.2.1/goodcrap/templates/tables/
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.441068 goodcrap-0.2.1/goodcrap/templates/tables/customers/
--rw-rw-rw-   0        0        0      562 2023-04-04 23:45:49.000000 goodcrap-0.2.1/goodcrap/templates/tables/customers/customers.crap_labels.json
--rw-rw-rw-   0        0        0      547 2023-04-02 16:03:37.000000 goodcrap-0.2.1/goodcrap/templates/tables/customers/customers.sql
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.443144 goodcrap-0.2.1/goodcrap/templates/tables/orders/
--rw-rw-rw-   0        0        0      244 2023-04-04 04:00:46.000000 goodcrap-0.2.1/goodcrap/templates/tables/orders/orders.crap_labels.json
--rw-rw-rw-   0        0        0      599 2023-04-04 03:59:42.000000 goodcrap-0.2.1/goodcrap/templates/tables/orders/orders.sql
-drwxrwxrwx   0        0        0        0 2023-04-09 16:31:20.409045 goodcrap-0.2.1/goodcrap.egg-info/
--rw-rw-rw-   0        0        0    11178 2023-04-09 16:31:20.000000 goodcrap-0.2.1/goodcrap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1567 2023-04-09 16:31:20.000000 goodcrap-0.2.1/goodcrap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 16:31:20.000000 goodcrap-0.2.1/goodcrap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-04-09 16:31:20.000000 goodcrap-0.2.1/goodcrap.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-04-09 16:31:20.000000 goodcrap-0.2.1/goodcrap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-09 16:31:20.000000 goodcrap-0.2.1/goodcrap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      215 2023-04-09 16:31:20.443144 goodcrap-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-04-06 16:31:50.000000 goodcrap-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.540344 goodcrap-0.2.2/
+-rw-rw-rw-   0        0        0       66 2023-03-29 13:09:13.000000 goodcrap-0.2.2/.gitattributes
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.486710 goodcrap-0.2.2/.github/
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.493219 goodcrap-0.2.2/.github/workflows/
+-rw-rw-rw-   0        0        0      576 2023-04-05 03:09:29.000000 goodcrap-0.2.2/.github/workflows/pylint.yml
+-rw-rw-rw-   0        0        0       54 2023-04-09 16:29:54.000000 goodcrap-0.2.2/.gitignore
+-rw-rw-rw-   0        0        0      332 2023-04-07 02:10:51.000000 goodcrap-0.2.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1574 2023-04-05 01:05:21.000000 goodcrap-0.2.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0    35802 2023-03-29 13:09:13.000000 goodcrap-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      193 2023-04-07 02:11:43.000000 goodcrap-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    12091 2023-04-11 04:43:02.540344 goodcrap-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11426 2023-04-11 04:41:17.000000 goodcrap-0.2.2/README.md
+-rw-rw-rw-   0        0        0        5 2023-04-11 04:41:26.000000 goodcrap-0.2.2/VERSION
+-rw-rw-rw-   0        0        0    72291 2023-04-07 05:50:59.000000 goodcrap-0.2.2/customers.parquet
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.493219 goodcrap-0.2.2/examples/
+-rw-rw-rw-   0        0        0      139 2023-04-04 14:07:32.000000 goodcrap-0.2.2/examples/mysql_config.json
+-rw-rw-rw-   0        0        0       59 2023-04-05 01:09:16.000000 goodcrap-0.2.2/examples/sqlite_config.json
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.508862 goodcrap-0.2.2/goodcrap/
+-rw-rw-rw-   0        0        0       87 2023-04-11 04:41:48.000000 goodcrap-0.2.2/goodcrap/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-04-04 00:49:25.000000 goodcrap-0.2.2/goodcrap/__main__.py
+-rw-rw-rw-   0        0        0     6033 2023-04-11 02:45:35.000000 goodcrap-0.2.2/goodcrap/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.525333 goodcrap-0.2.2/goodcrap/crappers/
+-rw-rw-rw-   0        0        0     1019 2023-04-08 15:25:53.000000 goodcrap-0.2.2/goodcrap/crappers/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-04-11 03:30:28.000000 goodcrap-0.2.2/goodcrap/crappers/queries.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.525333 goodcrap-0.2.2/goodcrap/data_warehouses/
+-rw-rw-rw-   0        0        0        0 2023-04-05 14:10:31.000000 goodcrap-0.2.2/goodcrap/data_warehouses/__init__.py
+-rw-rw-rw-   0        0        0     2283 2023-04-08 15:13:42.000000 goodcrap-0.2.2/goodcrap/data_warehouses/dimension_featurizer.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.525333 goodcrap-0.2.2/goodcrap/databases/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:02:02.000000 goodcrap-0.2.2/goodcrap/databases/__init__.py
+-rw-rw-rw-   0        0        0     4136 2023-04-11 04:37:36.000000 goodcrap-0.2.2/goodcrap/databases/database.py
+-rw-rw-rw-   0        0        0      532 2023-04-07 06:19:36.000000 goodcrap-0.2.2/goodcrap/databases/mysql.py
+-rw-rw-rw-   0        0        0      194 2023-04-07 06:53:45.000000 goodcrap-0.2.2/goodcrap/databases/queries.py
+-rw-rw-rw-   0        0        0     3915 2023-04-11 03:54:27.000000 goodcrap-0.2.2/goodcrap/databases/snowflake.py
+-rw-rw-rw-   0        0        0      379 2023-04-07 06:19:48.000000 goodcrap-0.2.2/goodcrap/databases/sqlite.py
+-rw-rw-rw-   0        0        0    13742 2023-04-11 04:21:40.000000 goodcrap-0.2.2/goodcrap/goodcrap.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.525333 goodcrap-0.2.2/goodcrap/pipelines/
+-rw-rw-rw-   0        0        0      560 2023-04-05 15:59:55.000000 goodcrap-0.2.2/goodcrap/pipelines/README.md
+-rw-rw-rw-   0        0        0        0 2023-04-05 15:01:30.000000 goodcrap-0.2.2/goodcrap/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     3608 2023-04-07 06:10:04.000000 goodcrap-0.2.2/goodcrap/pipelines/mage.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.540344 goodcrap-0.2.2/goodcrap/pipelines/templates/
+-rw-rw-rw-   0        0        0        0 2023-04-05 15:01:30.000000 goodcrap-0.2.2/goodcrap/pipelines/templates/__init__.py
+-rw-rw-rw-   0        0        0     1122 2023-04-07 06:20:36.000000 goodcrap-0.2.2/goodcrap/pipelines/templates/data_exporter_mysql.py
+-rw-rw-rw-   0        0        0      683 2023-04-07 06:10:42.000000 goodcrap-0.2.2/goodcrap/pipelines/templates/data_loader.py
+-rw-rw-rw-   0        0        0      832 2023-04-06 06:10:32.000000 goodcrap-0.2.2/goodcrap/pipelines/templates/metadata.yaml
+-rw-rw-rw-   0        0        0     2525 2023-04-09 16:25:30.000000 goodcrap-0.2.2/goodcrap/random_mapper.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.540344 goodcrap-0.2.2/goodcrap/templates/
+-rw-rw-rw-   0        0        0        0 2023-03-31 13:15:48.000000 goodcrap-0.2.2/goodcrap/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.540344 goodcrap-0.2.2/goodcrap/templates/__pycache__/
+-rw-rw-rw-   0        0        0      143 2023-03-31 13:16:56.000000 goodcrap-0.2.2/goodcrap/templates/__pycache__/__init__.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.540344 goodcrap-0.2.2/goodcrap/templates/data_warehouses/
+-rw-rw-rw-   0        0        0     3459 2023-04-08 14:48:01.000000 goodcrap-0.2.2/goodcrap/templates/data_warehouses/sales.sql
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.493219 goodcrap-0.2.2/goodcrap/templates/databases/
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.540344 goodcrap-0.2.2/goodcrap/templates/databases/customers_orders/
+-rw-rw-rw-   0        0        0      751 2023-04-04 05:53:19.000000 goodcrap-0.2.2/goodcrap/templates/databases/customers_orders/customers_orders.crap_labels.json
+-rw-rw-rw-   0        0        0      912 2023-04-11 04:27:42.000000 goodcrap-0.2.2/goodcrap/templates/databases/customers_orders/customers_orders.sql
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.493219 goodcrap-0.2.2/goodcrap/templates/tables/
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.540344 goodcrap-0.2.2/goodcrap/templates/tables/customers/
+-rw-rw-rw-   0        0        0      562 2023-04-04 23:45:49.000000 goodcrap-0.2.2/goodcrap/templates/tables/customers/customers.crap_labels.json
+-rw-rw-rw-   0        0        0      457 2023-04-11 04:27:37.000000 goodcrap-0.2.2/goodcrap/templates/tables/customers/customers.sql
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.540344 goodcrap-0.2.2/goodcrap/templates/tables/orders/
+-rw-rw-rw-   0        0        0      244 2023-04-04 04:00:46.000000 goodcrap-0.2.2/goodcrap/templates/tables/orders/orders.crap_labels.json
+-rw-rw-rw-   0        0        0      451 2023-04-11 04:27:31.000000 goodcrap-0.2.2/goodcrap/templates/tables/orders/orders.sql
+drwxrwxrwx   0        0        0        0 2023-04-11 04:43:02.525333 goodcrap-0.2.2/goodcrap.egg-info/
+-rw-rw-rw-   0        0        0    12091 2023-04-11 04:43:02.000000 goodcrap-0.2.2/goodcrap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1599 2023-04-11 04:43:02.000000 goodcrap-0.2.2/goodcrap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 04:43:02.000000 goodcrap-0.2.2/goodcrap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-11 04:43:02.000000 goodcrap-0.2.2/goodcrap.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       58 2023-04-11 04:43:02.000000 goodcrap-0.2.2/goodcrap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-11 04:43:02.000000 goodcrap-0.2.2/goodcrap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      215 2023-04-11 04:43:02.555995 goodcrap-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2023-04-10 13:23:32.000000 goodcrap-0.2.2/setup.py
```

### Comparing `goodcrap-0.2.1/.github/workflows/pylint.yml` & `goodcrap-0.2.2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/CONTRIBUTING.rst` & `goodcrap-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/LICENSE` & `goodcrap-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/PKG-INFO` & `goodcrap-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: goodcrap
-Version: 0.2.1
+Version: 0.2.2
 Summary: goodcrap creates tables, databases and csv files and fill them with random data
 Home-page: https://github.com/goodcrap/goodcrap
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: gpl-3.0
 Keywords: ai,data engineering,fake data,data science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `goodcrap`
 
-`goodcrap` is a python package that generates data structures (tables, databases and `csv` files) and fill them with random data, generates [`Mage`](https://github.com/mage-ai/mage-ai) pipelines that the user can use to orchestrate filling the data structures, and generate random SQL queries.
+`goodcrap` is a python package that generates random data stuff: creates and fills data structures (tables, databases and `csv` files) with random data, generates [`Mage`](https://github.com/mage-ai/mage-ai) pipelines that the user can use to orchestrate filling the data structures, and generate random SQL queries.
 
 ## Motivation
 
 This software enables data engineers to replicate the database schemas at their organisations, and then generate fake data that resemble a random sample of the actual data in their organisation. It also enables them to generate any number of random SQL queries that they can use for testing their analytics pipelines, as well as benchmark their data platforms.
 
 While public datasets, such as those hosted at Google or Kaggle, is a common starting point for people interested in learning data analytics and machine learning, many of these datasets require extensive data cleaning so that they can be usable in analytics pipelines. This makes the use of these datasets difficult for AI learners and practitioners.
 
@@ -69,14 +69,24 @@
 
 where `mysql_config` is the name of the configuration `json` file (`mysql_config.json`).
 
 For every table `mytable` you want to fill with random values, you must provide either:
 - a file `mytable.crap_labels.json`: this file tells `goodcrap` what sort of random values to generate for each record
 - a sample database table or `csv` file with matching structure and with some values: `goodcrap` will learn how to generate new random values based on the sample values
 
+### Supported destinations
+
+Currently, `goodcrap` can write data to the following destinations:
+- MySQL
+- SQLite
+- Snowflake
+- `csv` file
+- `json` file
+- `parquet` file
+
 ### Template data structures
 
 `goodcrap` has a number of template tables and databases that you can use. They are in the `templates/` directory.
 
 ## The `crap_labels.json` settings file
 
 For every table you want to generate, you have to provide the `crap_labels.json` file. If you are using the python library, then you can pass the `crap_label` dictionary instead - as is explained below.
@@ -209,14 +219,35 @@
 
 `Mage` python files are generated using `Jinja` templates. Given that Mage will always be backwards compatible (according to communication with its authors), files and folders generated by `goodcrap` will always be valid. Here is an example command to generate pipelines for each of the tables in the template database `customers_orders`:
 
 `goodcrap --size 1000 --seed 3 --database_config examples\mysql_config --template_database customers_orders --mage_pipeline`
 
 Note that `goodcrap` currently will only generate `Mage` projects if the database configurations are defined.
 
+## Writing to Snowflake
+
+`goodcrap` supports writing your random table to Snowflake using two methods:
+- row-by-row, which can be done by setting Snowflake as your database in the database configuration file
+- bulk upload of the generated `pandas DataFrame`, which is enabled by the command line argument `--bulk_upload`.
+
+The bulk upload is obviously preferred. Below is an example configuration settings file:
+
+```json
+{
+    "db_type": "snowflake",
+    "snowflake_database":"GOODCRAP",
+    "snowflake_warehouse":"WH",
+    "snowflake_user":"user",
+    "snowflake_password":"password",
+    "snowflake_account":"account",
+    "snowflake_schema":"public",
+    "snowflake_role":"role"
+}
+```
+
 ## Data warehouses
 
 Some dimensions in data warehouses will required to be filled as part of the testing exercise, but should not be filled with random data. These are the *conformed* dimensions with rigid data, such as the Date, Countries, and Cities dimensions. `goodcrap` will be able to fill these dimensions using the `DimensionFiller` class by providing several options for featurization. Filling these tables will be performed before any other table is populated.
 
 ## Guessing the `crap_labels.json` settings
 
 *in progress*
```

### Comparing `goodcrap-0.2.1/README.md` & `goodcrap-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # `goodcrap`
 
-`goodcrap` is a python package that generates data structures (tables, databases and `csv` files) and fill them with random data, generates [`Mage`](https://github.com/mage-ai/mage-ai) pipelines that the user can use to orchestrate filling the data structures, and generate random SQL queries.
+`goodcrap` is a python package that generates random data stuff: creates and fills data structures (tables, databases and `csv` files) with random data, generates [`Mage`](https://github.com/mage-ai/mage-ai) pipelines that the user can use to orchestrate filling the data structures, and generate random SQL queries.
 
 ## Motivation
 
 This software enables data engineers to replicate the database schemas at their organisations, and then generate fake data that resemble a random sample of the actual data in their organisation. It also enables them to generate any number of random SQL queries that they can use for testing their analytics pipelines, as well as benchmark their data platforms.
 
 While public datasets, such as those hosted at Google or Kaggle, is a common starting point for people interested in learning data analytics and machine learning, many of these datasets require extensive data cleaning so that they can be usable in analytics pipelines. This makes the use of these datasets difficult for AI learners and practitioners.
 
@@ -57,14 +57,24 @@
 
 where `mysql_config` is the name of the configuration `json` file (`mysql_config.json`).
 
 For every table `mytable` you want to fill with random values, you must provide either:
 - a file `mytable.crap_labels.json`: this file tells `goodcrap` what sort of random values to generate for each record
 - a sample database table or `csv` file with matching structure and with some values: `goodcrap` will learn how to generate new random values based on the sample values
 
+### Supported destinations
+
+Currently, `goodcrap` can write data to the following destinations:
+- MySQL
+- SQLite
+- Snowflake
+- `csv` file
+- `json` file
+- `parquet` file
+
 ### Template data structures
 
 `goodcrap` has a number of template tables and databases that you can use. They are in the `templates/` directory.
 
 ## The `crap_labels.json` settings file
 
 For every table you want to generate, you have to provide the `crap_labels.json` file. If you are using the python library, then you can pass the `crap_label` dictionary instead - as is explained below.
@@ -197,14 +207,35 @@
 
 `Mage` python files are generated using `Jinja` templates. Given that Mage will always be backwards compatible (according to communication with its authors), files and folders generated by `goodcrap` will always be valid. Here is an example command to generate pipelines for each of the tables in the template database `customers_orders`:
 
 `goodcrap --size 1000 --seed 3 --database_config examples\mysql_config --template_database customers_orders --mage_pipeline`
 
 Note that `goodcrap` currently will only generate `Mage` projects if the database configurations are defined.
 
+## Writing to Snowflake
+
+`goodcrap` supports writing your random table to Snowflake using two methods:
+- row-by-row, which can be done by setting Snowflake as your database in the database configuration file
+- bulk upload of the generated `pandas DataFrame`, which is enabled by the command line argument `--bulk_upload`.
+
+The bulk upload is obviously preferred. Below is an example configuration settings file:
+
+```json
+{
+    "db_type": "snowflake",
+    "snowflake_database":"GOODCRAP",
+    "snowflake_warehouse":"WH",
+    "snowflake_user":"user",
+    "snowflake_password":"password",
+    "snowflake_account":"account",
+    "snowflake_schema":"public",
+    "snowflake_role":"role"
+}
+```
+
 ## Data warehouses
 
 Some dimensions in data warehouses will required to be filled as part of the testing exercise, but should not be filled with random data. These are the *conformed* dimensions with rigid data, such as the Date, Countries, and Cities dimensions. `goodcrap` will be able to fill these dimensions using the `DimensionFiller` class by providing several options for featurization. Filling these tables will be performed before any other table is populated.
 
 ## Guessing the `crap_labels.json` settings
 
 *in progress*
```

### Comparing `goodcrap-0.2.1/customers.parquet` & `goodcrap-0.2.2/customers.parquet`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/goodcrap/cli.py` & `goodcrap-0.2.2/goodcrap/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -155,14 +155,22 @@
         parser.add_argument(
             "--queries",
             default=0,
             type=int,
             help="generate random SQL queries",
         )
 
+        parser.add_argument(
+            "--bulk_upload",
+            action="store_const",
+            default=False,
+            const=True,
+            help="upload to the database in bulk",
+        )
+
         arguments = parser.parse_args(self.argv[1:])
         random.seed(arguments.seed)
 
         from .goodcrap import GoodCrap
         good_crap = GoodCrap(size=arguments.size,
                              seed=arguments.seed,
                              to_csv=arguments.to_csv,
@@ -173,15 +181,16 @@
                              database_config=arguments.database_config,
                              table_sql=arguments.table_sql,
                              table_crap_labels=arguments.table_crap_labels,
                              database_sql=arguments.database_sql,
                              database_crap_labels=arguments.database_crap_labels,
                              mage_project_name=arguments.mage_project,
                              mage_pipeline=arguments.mage_pipeline,
-                             queries=arguments.queries
+                             queries=arguments.queries,
+                             bulk_upload=arguments.bulk_upload
                              )
 
         good_crap.run()
 
 
 def execute_cli(argv: Optional[str] = None) -> None:
     cli = CLI()
```

### Comparing `goodcrap-0.2.1/goodcrap/crappers/__init__.py` & `goodcrap-0.2.2/goodcrap/crappers/__init__.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/goodcrap/crappers/queries.py` & `goodcrap-0.2.2/goodcrap/crappers/queries.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/goodcrap/data_warehouses/dimension_featurizer.py` & `goodcrap-0.2.2/goodcrap/data_warehouses/dimension_featurizer.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/goodcrap/databases/database.py` & `goodcrap-0.2.2/goodcrap/databases/database.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,55 +4,74 @@
 import sqlalchemy
 from sqlalchemy import MetaData, Table, Column, Integer, String
 from sqlalchemy.sql import text
 
 from ..random_mapper import RandomMapper
 from ..crappers import queries
 
+
 class DataBase:
     def __init__(self,
                  database_config) -> None:
         self.database_config = database_config
         self.size = 1000
         self.connection = None
         self.engine = None
+        self.native = False
+        
 
     def set_size(self, size):
         self.size = size
 
     def set_seed(self, seed):
         self.seed = seed
 
+    def insert(self, table_name: str, row, table: Table = None):
+        if table is not None:
+            ins = table.insert().values(row)
+            self.engine.execute(ins)
+
+    def execute_sql(self, table_sql):
+        self.connection.execute(table_sql)
+
     def run(self, table_sql=None, table_crap_labels=None,
             database_sql=None, database_crap_labels=None):
         if table_sql is not None and table_crap_labels is not None:
             table_name = os.path.basename(table_sql).split('.')[0]
             with open(table_sql, 'r') as f:
                 self.table_sql = f.read()
                 f.close()
-            self.connection.execute(self.table_sql)
-            metadata = MetaData(bind=self.engine)
+            
+            # sqlalchemy.inspect(self.engine).has_table(table_name)
+
+            self.execute_sql(self.table_sql)
 
+            metadata = MetaData(bind=self.engine)
             table = Table(table_name, metadata, autoload=True)
 
-            fm = RandomMapper(self.seed, self.table_crap_labels,
+            fm = RandomMapper(self.seed, table_crap_labels,
                               table, engine=self.engine)
-
             data_csv = []
             for i in range(self.size):
                 row = fm.get_crap()
-                ins = table.insert().values(row)
-                self.engine.execute(ins)
-                if self.database_config['to_csv']:
+                if not self.database_config['bulk_upload']:
+                    self.insert(table_name=table_name, row=row, table=table)
+                if self.database_config['to_csv'] or self.database_config['bulk_upload']:
                     data_csv += [row]
-            if self.database_config['to_csv']:
-                df = pd.DataFrame(data_csv, columns=table.columns)
+            if self.database_config['to_csv'] or self.database_config['bulk_upload']:
+                df = pd.DataFrame(data_csv, columns=table_crap_labels.keys())
                 df.to_csv(table_name+'.csv')
+            if self.database_config['bulk_upload']:
+                self.bulk_upload(df, table_name)
 
         elif database_sql is not None and database_crap_labels is not None:
+            if self.database_config['bulk_upload']:
+                import sys
+                sys.exit('Write a database to Snowflake is not yet supported.')
+
             with open(database_sql, 'r') as f:
                 self.database_sql = f.read()
                 f.close()
             self.connection.execute(self.database_sql)
             metadata = MetaData(bind=self.engine)
             rounds = 10
             for i in range(rounds):
@@ -61,21 +80,25 @@
 
                     fm = RandomMapper(
                         self.seed, database_crap_labels[table_name], table, self.engine)
 
                     data_csv = []
                     for i in range(int(self.size/rounds)):
                         row = fm.get_crap()
-                        ins = table.insert().values(row)
-                        self.engine.execute(ins)
+                        self.insert(table_name=table_name, row=row, table=table)
                         if self.database_config['to_csv']:
                             data_csv += [row]
                     if self.database_config['to_csv']:
                         df = pd.DataFrame(data_csv, columns=table.columns)
                         df.to_csv(table_name+'.csv')
         if 'queries' in self.database_config.keys():
-            with open('queries.sql','a') as f:
+            with open('queries.sql', 'w') as f:
                 for i in range(self.database_config['queries']):
                     f.write(str(queries.crapper(self.engine))+'\n')
+                    f.flush()
+                f.close()
+
+    def bulk_upload(self, df, table_name):
+        print('Bulk upload is not implemented yet for', self.database_config['db_type'])
 
     def execute(self, sql):
         return self.engine.execute(sql)
```

### Comparing `goodcrap-0.2.1/goodcrap/databases/mysql.py` & `goodcrap-0.2.2/goodcrap/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/goodcrap/goodcrap.py` & `goodcrap-0.2.2/goodcrap/goodcrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
 import os
 from .databases.sqlite import SQLite
 from .databases.mysql import MySQL
+from .databases.snowflake import Snowflake
 from .random_mapper import RandomMapper
 from .pipelines.mage import MageProject
 from . import templates
 
+
 class GoodCrap:
     seed = None
 
     def __init__(
         self,
         size,
         seed,
@@ -21,15 +23,16 @@
         template_database=None,
         table_sql=None,
         table_crap_labels=None,
         database_sql=None,
         database_crap_labels=None,
         mage_project_name=None,
         mage_pipeline=None,
-        queries=False
+        queries=False,
+        bulk_upload=False
     ) -> None:
         GoodCrap.seed = seed
         self.size = size
         self.to_csv = to_csv
         self.to_json = to_json
         self.to_parquet = to_parquet
         self.template_table = template_table
@@ -37,14 +40,15 @@
         self.table_sql = table_sql
         self.table_crap_labels = table_crap_labels
         self.database_sql = database_sql
         self.database_crap_labels = database_crap_labels
         self.mage_project_name = mage_project_name
         self.mage_pipeline = mage_pipeline
         self.queries = queries
+        self.bulk_upload = bulk_upload
 
         self.templates_path = os.path.dirname(templates.__file__)
 
         if self.table_crap_labels:
             with open(self.table_crap_labels, 'r') as f:
                 self.table_crap_labels = json.load(f)
                 f.close()
@@ -63,19 +67,22 @@
                 fdatabase_config = open(database_config+'.json', 'r')
                 database_config = json.load(fdatabase_config)
                 fdatabase_config.close()
             database_config['to_csv'] = self.to_csv
             database_config['to_json'] = self.to_json
             database_config['to_parquet'] = self.to_parquet
             database_config['queries'] = self.queries
+            database_config['bulk_upload'] = self.bulk_upload
             self.database_config = database_config
             if database_config['db_type'] == 'sqlite':
                 self.database_instance = SQLite(database_config)
             elif database_config['db_type'] == 'mysql':
                 self.database_instance = MySQL(database_config)
+            elif database_config['db_type'] == 'snowflake':
+                self.database_instance = Snowflake(database_config)
 
             if self.database_instance is not None:
                 self.database_instance.set_size(self.size)
                 self.database_instance.set_seed(self.seed)
 
     def run(self):
         '''
@@ -210,17 +217,16 @@
                 self.database_instance.execute(database_sql)
                 for table_name in database_crap_labels.keys():
                     self.create_mage_pipeline(
                         table_name, database_crap_labels[table_name])
 
         else:
             # Set the project name as the database name plus a random string
-            import uuid
             self.mage_project_name = self.database_config['database']
-            self.mage_project_name += '-' + str(uuid.uuid4())[:8]
+            self.mage_project_name += '-' + self.get_random_filename()
             self.create_mage_project()
             if table_sql is not None and table_crap_labels is not None:
                 table_name = os.path.basename(
                     table_sql).replace('.sql', '')
                 with open(table_sql, 'r') as f:
                     table_sql = f.read()
                     f.close()
@@ -231,14 +237,18 @@
                     database_sql = f.read()
                     f.close()
                 self.database_instance.execute(database_sql)
                 for table_name in database_crap_labels.keys():
                     self.create_mage_pipeline(
                         table_name, database_crap_labels[table_name])
 
+    def get_random_filename():
+        import uuid
+        return str(uuid.uuid4())[:8]
+
     def _is_run_with_mage(self):
         return self.mage_pipeline is not None
 
     def write_file(self, table_name=None,
                    table_crap_labels=None,
                    database_crap_labels=None):
         import pandas as pd
```

### Comparing `goodcrap-0.2.1/goodcrap/pipelines/README.md` & `goodcrap-0.2.2/goodcrap/pipelines/README.md`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/goodcrap/pipelines/mage.py` & `goodcrap-0.2.2/goodcrap/pipelines/mage.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/goodcrap/pipelines/templates/data_exporter_mysql.py` & `goodcrap-0.2.2/goodcrap/pipelines/templates/data_exporter_mysql.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/goodcrap/pipelines/templates/data_loader.py` & `goodcrap-0.2.2/goodcrap/pipelines/templates/data_loader.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/goodcrap/pipelines/templates/metadata.yaml` & `goodcrap-0.2.2/goodcrap/pipelines/templates/metadata.yaml`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/goodcrap/random_mapper.py` & `goodcrap-0.2.2/goodcrap/random_mapper.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/goodcrap/templates/data_warehouses/sales.sql` & `goodcrap-0.2.2/goodcrap/templates/data_warehouses/sales.sql`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/goodcrap/templates/databases/customers_orders/customers_orders.crap_labels.json` & `goodcrap-0.2.2/goodcrap/templates/databases/customers_orders/customers_orders.crap_labels.json`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/goodcrap/templates/tables/customers/customers.crap_labels.json` & `goodcrap-0.2.2/goodcrap/templates/tables/customers/customers.crap_labels.json`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.1/goodcrap.egg-info/PKG-INFO` & `goodcrap-0.2.2/goodcrap.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: goodcrap
-Version: 0.2.1
+Version: 0.2.2
 Summary: goodcrap creates tables, databases and csv files and fill them with random data
 Home-page: https://github.com/goodcrap/goodcrap
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: gpl-3.0
 Keywords: ai,data engineering,fake data,data science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `goodcrap`
 
-`goodcrap` is a python package that generates data structures (tables, databases and `csv` files) and fill them with random data, generates [`Mage`](https://github.com/mage-ai/mage-ai) pipelines that the user can use to orchestrate filling the data structures, and generate random SQL queries.
+`goodcrap` is a python package that generates random data stuff: creates and fills data structures (tables, databases and `csv` files) with random data, generates [`Mage`](https://github.com/mage-ai/mage-ai) pipelines that the user can use to orchestrate filling the data structures, and generate random SQL queries.
 
 ## Motivation
 
 This software enables data engineers to replicate the database schemas at their organisations, and then generate fake data that resemble a random sample of the actual data in their organisation. It also enables them to generate any number of random SQL queries that they can use for testing their analytics pipelines, as well as benchmark their data platforms.
 
 While public datasets, such as those hosted at Google or Kaggle, is a common starting point for people interested in learning data analytics and machine learning, many of these datasets require extensive data cleaning so that they can be usable in analytics pipelines. This makes the use of these datasets difficult for AI learners and practitioners.
 
@@ -69,14 +69,24 @@
 
 where `mysql_config` is the name of the configuration `json` file (`mysql_config.json`).
 
 For every table `mytable` you want to fill with random values, you must provide either:
 - a file `mytable.crap_labels.json`: this file tells `goodcrap` what sort of random values to generate for each record
 - a sample database table or `csv` file with matching structure and with some values: `goodcrap` will learn how to generate new random values based on the sample values
 
+### Supported destinations
+
+Currently, `goodcrap` can write data to the following destinations:
+- MySQL
+- SQLite
+- Snowflake
+- `csv` file
+- `json` file
+- `parquet` file
+
 ### Template data structures
 
 `goodcrap` has a number of template tables and databases that you can use. They are in the `templates/` directory.
 
 ## The `crap_labels.json` settings file
 
 For every table you want to generate, you have to provide the `crap_labels.json` file. If you are using the python library, then you can pass the `crap_label` dictionary instead - as is explained below.
@@ -209,14 +219,35 @@
 
 `Mage` python files are generated using `Jinja` templates. Given that Mage will always be backwards compatible (according to communication with its authors), files and folders generated by `goodcrap` will always be valid. Here is an example command to generate pipelines for each of the tables in the template database `customers_orders`:
 
 `goodcrap --size 1000 --seed 3 --database_config examples\mysql_config --template_database customers_orders --mage_pipeline`
 
 Note that `goodcrap` currently will only generate `Mage` projects if the database configurations are defined.
 
+## Writing to Snowflake
+
+`goodcrap` supports writing your random table to Snowflake using two methods:
+- row-by-row, which can be done by setting Snowflake as your database in the database configuration file
+- bulk upload of the generated `pandas DataFrame`, which is enabled by the command line argument `--bulk_upload`.
+
+The bulk upload is obviously preferred. Below is an example configuration settings file:
+
+```json
+{
+    "db_type": "snowflake",
+    "snowflake_database":"GOODCRAP",
+    "snowflake_warehouse":"WH",
+    "snowflake_user":"user",
+    "snowflake_password":"password",
+    "snowflake_account":"account",
+    "snowflake_schema":"public",
+    "snowflake_role":"role"
+}
+```
+
 ## Data warehouses
 
 Some dimensions in data warehouses will required to be filled as part of the testing exercise, but should not be filled with random data. These are the *conformed* dimensions with rigid data, such as the Date, Countries, and Cities dimensions. `goodcrap` will be able to fill these dimensions using the `DimensionFiller` class by providing several options for featurization. Filling these tables will be performed before any other table is populated.
 
 ## Guessing the `crap_labels.json` settings
 
 *in progress*
```

### Comparing `goodcrap-0.2.1/goodcrap.egg-info/SOURCES.txt` & `goodcrap-0.2.2/goodcrap.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 goodcrap/crappers/queries.py
 goodcrap/data_warehouses/__init__.py
 goodcrap/data_warehouses/dimension_featurizer.py
 goodcrap/databases/__init__.py
 goodcrap/databases/database.py
 goodcrap/databases/mysql.py
 goodcrap/databases/queries.py
+goodcrap/databases/snowflake.py
 goodcrap/databases/sqlite.py
 goodcrap/pipelines/README.md
 goodcrap/pipelines/__init__.py
 goodcrap/pipelines/mage.py
 goodcrap/pipelines/templates/__init__.py
 goodcrap/pipelines/templates/data_exporter_mysql.py
 goodcrap/pipelines/templates/data_loader.py
```

### Comparing `goodcrap-0.2.1/setup.py` & `goodcrap-0.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,10 +19,15 @@
     long_description=README,
     long_description_content_type='text/markdown',
     author='Sherif Abdulkader Tawfik Abbas',
     author_email='sherif.tawfic@gmail.com',
     url='https://github.com/goodcrap/goodcrap',
     keywords=['ai', 'data engineering', 'fake data',
               'data science'],
-    install_requires=['sqlalchemy', 'faker', 'pandas', 'numpy', 'jinja2'],
+    install_requires=['sqlalchemy',
+                      'faker',
+                      'pandas',
+                      'numpy',
+                      'jinja2',
+                      'snowflake-sqlalchemy'],
 
 )
```

