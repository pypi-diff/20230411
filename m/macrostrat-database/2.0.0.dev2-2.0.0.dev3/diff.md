# Comparing `tmp/macrostrat_database-2.0.0.dev2.tar.gz` & `tmp/macrostrat_database-2.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrostrat_database-2.0.0.dev2.tar", max compression
+gzip compressed data, was "macrostrat_database-2.0.0.dev3.tar", max compression
```

## Comparing `macrostrat_database-2.0.0.dev2.tar` & `macrostrat_database-2.0.0.dev3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     5630 2022-10-28 09:04:41.302050 macrostrat_database-2.0.0.dev2/macrostrat/database/__init__.py
--rw-r--r--   0        0        0     4665 2022-10-28 06:36:46.591730 macrostrat_database-2.0.0.dev2/macrostrat/database/mapper/__init__.py
--rw-r--r--   0        0        0      686 2022-05-26 00:55:15.936699 macrostrat_database-2.0.0.dev2/macrostrat/database/mapper/base.py
--rw-r--r--   0        0        0     2272 2022-05-26 05:21:07.121385 macrostrat_database-2.0.0.dev2/macrostrat/database/mapper/cache.py
--rw-r--r--   0        0        0     3070 2022-10-28 06:26:55.575375 macrostrat_database-2.0.0.dev2/macrostrat/database/mapper/utils.py
--rw-r--r--   0        0        0     1630 2022-05-26 00:55:15.936016 macrostrat_database-2.0.0.dev2/macrostrat/database/postgresql.py
--rw-r--r--   0        0        0     8063 2022-10-28 08:24:36.711469 macrostrat_database-2.0.0.dev2/macrostrat/database/utils.py
--rw-r--r--   0        0        0      700 2022-10-28 09:06:02.004674 macrostrat_database-2.0.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 macrostrat_database-2.0.0.dev2/setup.py
--rw-r--r--   0        0        0      900 1970-01-01 00:00:00.000000 macrostrat_database-2.0.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0     5630 2022-10-28 09:04:41.302050 macrostrat_database-2.0.0.dev3/macrostrat/database/__init__.py
+-rw-r--r--   0        0        0     4665 2022-10-28 06:36:46.591730 macrostrat_database-2.0.0.dev3/macrostrat/database/mapper/__init__.py
+-rw-r--r--   0        0        0      686 2022-05-26 00:55:15.936699 macrostrat_database-2.0.0.dev3/macrostrat/database/mapper/base.py
+-rw-r--r--   0        0        0     2272 2022-05-26 05:21:07.121385 macrostrat_database-2.0.0.dev3/macrostrat/database/mapper/cache.py
+-rw-r--r--   0        0        0     3070 2022-10-28 06:26:55.575375 macrostrat_database-2.0.0.dev3/macrostrat/database/mapper/utils.py
+-rw-r--r--   0        0        0     1630 2022-05-26 00:55:15.936016 macrostrat_database-2.0.0.dev3/macrostrat/database/postgresql.py
+-rw-r--r--   0        0        0     8332 2022-10-28 18:22:02.012812 macrostrat_database-2.0.0.dev3/macrostrat/database/utils.py
+-rw-r--r--   0        0        0      700 2022-10-28 18:22:13.985170 macrostrat_database-2.0.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 macrostrat_database-2.0.0.dev3/setup.py
+-rw-r--r--   0        0        0      900 1970-01-01 00:00:00.000000 macrostrat_database-2.0.0.dev3/PKG-INFO
```

### Comparing `macrostrat_database-2.0.0.dev2/macrostrat/database/__init__.py` & `macrostrat_database-2.0.0.dev3/macrostrat/database/__init__.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.0.0.dev2/macrostrat/database/mapper/__init__.py` & `macrostrat_database-2.0.0.dev3/macrostrat/database/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.0.0.dev2/macrostrat/database/mapper/base.py` & `macrostrat_database-2.0.0.dev3/macrostrat/database/mapper/base.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.0.0.dev2/macrostrat/database/mapper/cache.py` & `macrostrat_database-2.0.0.dev3/macrostrat/database/mapper/cache.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.0.0.dev2/macrostrat/database/mapper/utils.py` & `macrostrat_database-2.0.0.dev3/macrostrat/database/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.0.0.dev2/macrostrat/database/postgresql.py` & `macrostrat_database-2.0.0.dev3/macrostrat/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.0.0.dev2/macrostrat/database/utils.py` & `macrostrat_database-2.0.0.dev3/macrostrat/database/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,25 +89,29 @@
 
 def run_sql(
     connectable,
     sql,
     params=None,
     stop_on_error=False,
     interpret_as_file=None,
+    yield_results=False,
 ):
     if isinstance(connectable, Engine):
         with connectable.connect() as conn:
-            yield from run_sql(
+            res = run_sql(
                 conn,
                 sql,
                 params=params,
                 stop_on_error=stop_on_error,
                 interpret_as_file=interpret_as_file,
             )
-            return
+            if yield_results:
+                yield from res
+            else:
+                return res
 
     if interpret_as_file:
         sql = Path(sql).read_text()
     elif interpret_as_file is None:
         sql = canonicalize_query(sql)
 
     if isinstance(sql, Path):
@@ -121,15 +125,17 @@
 
     for query, params in zip(queries, params):
         sql = format(query, strip_comments=True).strip()
         if sql == "":
             continue
         try:
             connectable.begin()
-            yield connectable.execute(text(sql), params=params)
+            res = connectable.execute(text(sql), params=params)
+            if yield_results:
+                yield res
             if hasattr(connectable, "commit"):
                 connectable.commit()
             pretty_print(sql, dim=True)
         except (ProgrammingError, IntegrityError) as err:
             err = str(err.orig).strip()
             dim = "already exists" in err
             if hasattr(connectable, "rollback"):
@@ -139,14 +145,17 @@
                 err = "  " + err
             secho(err, fg="red", dim=dim)
             if stop_on_error:
                 return
         finally:
             if hasattr(connectable, "close"):
                 connectable.close()
+    # Return the last result if a generator wasn't requested
+    if not yield_results:
+        return res
 
 
 def execute(connectable, sql, params=None, stop_on_error=False):
     sql = format(sql, strip_comments=True).strip()
     if sql == "":
         return
     try:
```

### Comparing `macrostrat_database-2.0.0.dev2/pyproject.toml` & `macrostrat_database-2.0.0.dev3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Daven Quinn <dev@davenquinn.com>"]
 description = "A small library based on SQLAlchemy to assist with common database tasks."
 name = "macrostrat.database"
 packages = [
   {include = "macrostrat"},
 ]
-version = "2.0.0.dev2"
+version = "2.0.0.dev3"
 
 [tool.poetry.dependencies]
 GeoAlchemy2 = "^0.9.4"
 SQLAlchemy = "^1.4.26"
 SQLAlchemy-Utils = "^0.37.0"
 click = "^8.1.3"
 "macrostrat.utils" = "^1.0.0"
```

### Comparing `macrostrat_database-2.0.0.dev2/setup.py` & `macrostrat_database-2.0.0.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'migra>=3.0.1621480950,<4.0.0',
  'psycopg2-binary>=2.9.1,<3.0.0',
  'schemainspect>=3.0.1616029793,<4.0.0',
  'sqlparse>=0.4.0,<0.5.0']
 
 setup_kwargs = {
     'name': 'macrostrat-database',
-    'version': '2.0.0.dev2',
+    'version': '2.0.0.dev3',
     'description': 'A small library based on SQLAlchemy to assist with common database tasks.',
     'long_description': 'None',
     'author': 'Daven Quinn',
     'author_email': 'dev@davenquinn.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrostrat_database-2.0.0.dev2/PKG-INFO` & `macrostrat_database-2.0.0.dev3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrostrat-database
-Version: 2.0.0.dev2
+Version: 2.0.0.dev3
 Summary: A small library based on SQLAlchemy to assist with common database tasks.
 Author: Daven Quinn
 Author-email: dev@davenquinn.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

