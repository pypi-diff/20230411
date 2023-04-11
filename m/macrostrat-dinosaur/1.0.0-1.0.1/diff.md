# Comparing `tmp/macrostrat_dinosaur-1.0.0.tar.gz` & `tmp/macrostrat_dinosaur-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrostrat_dinosaur-1.0.0.tar", max compression
+gzip compressed data, was "macrostrat_dinosaur-1.0.1.tar", max compression
```

## Comparing `macrostrat_dinosaur-1.0.0.tar` & `macrostrat_dinosaur-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10121 2023-04-11 05:06:58.497729 macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/__init__.py
--rw-r--r--   0        0        0     3836 2023-04-11 05:06:58.498297 macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/upgrade_cluster/__init__.py
--rw-r--r--   0        0        0     1711 2023-04-11 05:06:58.498793 macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/upgrade_cluster/describe.py
--rw-r--r--   0        0        0     1796 2023-04-11 05:06:58.498985 macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/upgrade_cluster/restore.py
--rw-r--r--   0        0        0     3328 2023-04-11 05:06:58.499169 macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/upgrade_cluster/utils.py
--rw-r--r--   0        0        0      705 2023-04-11 05:10:29.158461 macrostrat_dinosaur-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 macrostrat_dinosaur-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    10121 2023-04-11 05:06:58.497729 macrostrat_dinosaur-1.0.1/macrostrat/dinosaur/__init__.py
+-rw-r--r--   0        0        0     3836 2023-04-11 05:06:58.498297 macrostrat_dinosaur-1.0.1/macrostrat/dinosaur/upgrade_cluster/__init__.py
+-rw-r--r--   0        0        0     1711 2023-04-11 05:06:58.498793 macrostrat_dinosaur-1.0.1/macrostrat/dinosaur/upgrade_cluster/describe.py
+-rw-r--r--   0        0        0     1796 2023-04-11 05:06:58.498985 macrostrat_dinosaur-1.0.1/macrostrat/dinosaur/upgrade_cluster/restore.py
+-rw-r--r--   0        0        0     3328 2023-04-11 05:06:58.499169 macrostrat_dinosaur-1.0.1/macrostrat/dinosaur/upgrade_cluster/utils.py
+-rw-r--r--   0        0        0      723 2023-04-11 19:50:54.664232 macrostrat_dinosaur-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 macrostrat_dinosaur-1.0.1/PKG-INFO
```

### Comparing `macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/__init__.py` & `macrostrat_dinosaur-1.0.1/macrostrat/dinosaur/__init__.py`

 * *Files identical despite different names*

### Comparing `macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/upgrade_cluster/__init__.py` & `macrostrat_dinosaur-1.0.1/macrostrat/dinosaur/upgrade_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/upgrade_cluster/describe.py` & `macrostrat_dinosaur-1.0.1/macrostrat/dinosaur/upgrade_cluster/describe.py`

 * *Files identical despite different names*

### Comparing `macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/upgrade_cluster/restore.py` & `macrostrat_dinosaur-1.0.1/macrostrat/dinosaur/upgrade_cluster/restore.py`

 * *Files identical despite different names*

### Comparing `macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/upgrade_cluster/utils.py` & `macrostrat_dinosaur-1.0.1/macrostrat/dinosaur/upgrade_cluster/utils.py`

 * *Files identical despite different names*

### Comparing `macrostrat_dinosaur-1.0.0/pyproject.toml` & `macrostrat_dinosaur-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 authors = ["Daven Quinn <dev@davenquinn.com>"]
 description = "Diff-based database migrations"
 name = "macrostrat.dinosaur"
 packages = [
   {include = "macrostrat"},
 ]
-version = "1.0.0"
+version = "1.0.1"
 
 [tool.poetry.dependencies]
 GeoAlchemy2 = "^0.9.4"
 SQLAlchemy = "^1.4.26"
 SQLAlchemy-Utils = "^0.37.0"
 "macrostrat.database" = "^2.0.0"
 "macrostrat.utils" = "^1.0.0"
 psycopg2-binary = "^2.9.1"
 python = "^3.8"
 schemainspect = "^3.0.1616029793"
 sqlparse = "^0.4.0"
+docker = "^6.0.1"
 
 [tool.poetry.dev-dependencies]
 "macrostrat.database" = {path = "../database", develop = true}
 "macrostrat.utils" = {path = "../utils", develop = true}
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `macrostrat_dinosaur-1.0.0/PKG-INFO` & `macrostrat_dinosaur-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: macrostrat-dinosaur
-Version: 1.0.0
+Version: 1.0.1
 Summary: Diff-based database migrations
 Author: Daven Quinn
 Author-email: dev@davenquinn.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GeoAlchemy2 (>=0.9.4,<0.10.0)
 Requires-Dist: SQLAlchemy (>=1.4.26,<2.0.0)
 Requires-Dist: SQLAlchemy-Utils (>=0.37.0,<0.38.0)
+Requires-Dist: docker (>=6.0.1,<7.0.0)
 Requires-Dist: macrostrat.database (>=2.0.0,<3.0.0)
 Requires-Dist: macrostrat.utils (>=1.0.0,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.1,<3.0.0)
 Requires-Dist: schemainspect (>=3.0.1616029793,<4.0.0)
 Requires-Dist: sqlparse (>=0.4.0,<0.5.0)
```

