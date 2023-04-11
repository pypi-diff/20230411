# Comparing `tmp/sqlalchemy-firebird-0.7.6.tar.gz` & `tmp/sqlalchemy-firebird-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-firebird-0.7.6.tar", last modified: Wed Sep 28 01:03:11 2022, max compression
+gzip compressed data, was "sqlalchemy-firebird-0.8.0.tar", last modified: Tue Apr 11 05:50:23 2023, max compression
```

## Comparing `sqlalchemy-firebird-0.7.6.tar` & `sqlalchemy-firebird-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-09-28 01:03:11.936772 sqlalchemy-firebird-0.7.6/
--rw-rw-rw-   0        0        0     1117 2022-08-15 03:21:49.000000 sqlalchemy-firebird-0.7.6/LICENSE
--rw-rw-rw-   0        0        0     2294 2022-09-28 01:03:11.937273 sqlalchemy-firebird-0.7.6/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2022-08-15 03:21:49.000000 sqlalchemy-firebird-0.7.6/README.rst
--rw-rw-rw-   0        0        0      359 2022-09-27 23:12:18.000000 sqlalchemy-firebird-0.7.6/pyproject.toml
--rw-rw-rw-   0        0        0      388 2022-09-28 01:03:11.938774 sqlalchemy-firebird-0.7.6/setup.cfg
--rw-rw-rw-   0        0        0     1875 2022-09-27 23:18:50.000000 sqlalchemy-firebird-0.7.6/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-28 01:03:11.909772 sqlalchemy-firebird-0.7.6/sqlalchemy_firebird/
--rw-rw-rw-   0        0        0     1109 2022-09-27 23:21:53.000000 sqlalchemy-firebird-0.7.6/sqlalchemy_firebird/__init__.py
--rw-rw-rw-   0        0        0    34948 2022-09-27 23:18:50.000000 sqlalchemy-firebird-0.7.6/sqlalchemy_firebird/base.py
--rw-rw-rw-   0        0        0     4000 2022-09-25 20:27:46.000000 sqlalchemy-firebird-0.7.6/sqlalchemy_firebird/fdb.py
--rw-rw-rw-   0        0        0     6415 2022-09-25 20:27:46.000000 sqlalchemy-firebird-0.7.6/sqlalchemy_firebird/kinterbasdb.py
--rw-rw-rw-   0        0        0      277 2022-08-15 03:21:49.000000 sqlalchemy-firebird-0.7.6/sqlalchemy_firebird/provision.py
--rw-rw-rw-   0        0        0     2824 2022-08-15 03:21:49.000000 sqlalchemy-firebird-0.7.6/sqlalchemy_firebird/requirements.py
-drwxrwxrwx   0        0        0        0 2022-09-28 01:03:11.927273 sqlalchemy-firebird-0.7.6/sqlalchemy_firebird.egg-info/
--rw-rw-rw-   0        0        0     2294 2022-09-28 01:03:11.000000 sqlalchemy-firebird-0.7.6/sqlalchemy_firebird.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      564 2022-09-28 01:03:11.000000 sqlalchemy-firebird-0.7.6/sqlalchemy_firebird.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-28 01:03:11.000000 sqlalchemy-firebird-0.7.6/sqlalchemy_firebird.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2022-09-28 01:03:11.000000 sqlalchemy-firebird-0.7.6/sqlalchemy_firebird.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-08-15 03:25:58.000000 sqlalchemy-firebird-0.7.6/sqlalchemy_firebird.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       22 2022-09-28 01:03:11.000000 sqlalchemy-firebird-0.7.6/sqlalchemy_firebird.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2022-09-28 01:03:11.000000 sqlalchemy-firebird-0.7.6/sqlalchemy_firebird.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-09-28 01:03:11.934273 sqlalchemy-firebird-0.7.6/test/
--rw-rw-rw-   0        0        0    19593 2022-08-15 03:21:49.000000 sqlalchemy-firebird-0.7.6/test/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:50:23.479142 sqlalchemy-firebird-0.8.0/
+-rw-rw-rw-   0        0        0     1117 2023-01-02 01:08:06.000000 sqlalchemy-firebird-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0     2271 2023-04-11 05:50:23.479642 sqlalchemy-firebird-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2023-01-02 01:08:06.000000 sqlalchemy-firebird-0.8.0/README.rst
+-rw-rw-rw-   0        0        0      896 2023-04-11 05:26:28.000000 sqlalchemy-firebird-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0      374 2023-04-11 05:50:23.482142 sqlalchemy-firebird-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1944 2023-04-11 05:26:28.000000 sqlalchemy-firebird-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:50:23.449643 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/
+-rw-rw-rw-   0        0        0     1109 2023-04-11 05:34:11.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/__init__.py
+-rw-rw-rw-   0        0        0    35223 2023-04-02 20:53:51.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/base.py
+-rw-rw-rw-   0        0        0     4082 2023-04-11 05:26:28.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/fdb.py
+-rw-rw-rw-   0        0        0     6415 2023-01-16 16:40:52.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/kinterbasdb.py
+-rw-rw-rw-   0        0        0      348 2023-04-11 05:26:28.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/provision.py
+-rw-rw-rw-   0        0        0     2984 2023-04-11 05:26:28.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/requirements.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:50:23.464145 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/
+-rw-rw-rw-   0        0        0     2271 2023-04-11 05:50:23.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      687 2023-04-11 05:50:23.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 05:50:23.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2023-04-11 05:50:23.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-01-14 23:50:33.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       22 2023-04-11 05:50:23.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-11 05:50:23.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 05:50:23.477144 sqlalchemy-firebird-0.8.0/test/
+-rw-rw-rw-   0        0        0     4463 2023-01-16 16:40:52.000000 sqlalchemy-firebird-0.8.0/test/test_domain_reflection.py
+-rw-rw-rw-   0        0        0     1629 2023-01-02 01:08:06.000000 sqlalchemy-firebird-0.8.0/test/test_fb_argument.py
+-rw-rw-rw-   0        0        0     7646 2023-01-16 16:40:52.000000 sqlalchemy-firebird-0.8.0/test/test_fb_compile.py
+-rw-rw-rw-   0        0        0     4094 2023-01-16 16:40:52.000000 sqlalchemy-firebird-0.8.0/test/test_fb_misc.py
+-rw-rw-rw-   0        0        0      624 2023-01-02 01:08:06.000000 sqlalchemy-firebird-0.8.0/test/test_fb_types.py
+-rw-rw-rw-   0        0        0     9471 2023-04-11 05:26:28.000000 sqlalchemy-firebird-0.8.0/test/test_suite.py
```

### Comparing `sqlalchemy-firebird-0.7.6/LICENSE` & `sqlalchemy-firebird-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-firebird-0.7.6/PKG-INFO` & `sqlalchemy-firebird-0.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-firebird
-Version: 0.7.6
+Version: 0.8.0
 Summary: Firebird for SQLAlchemy
 Home-page: https://github.com/pauldex/sqlalchemy-firebird
 Author: Paul Graves-DesLauriers
 Author-email: paul@dexmicro.com
 License: MIT
 Project-URL: Documentation, https://github.com/pauldex/sqlalchemy-firebird/wiki
 Project-URL: Source, https://github.com/pauldex/sqlalchemy-firebird
 Project-URL: Tracker, https://github.com/pauldex/sqlalchemy-firebird/issues
 Keywords: SQLAlchemy Firebird
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database :: Front-Ends
@@ -65,9 +64,7 @@
 
 ----
 
 **License**
 
 sqlalchemy-firebird is distributed under the `MIT license
 <http://www.opensource.org/licenses/mit-license.php>`_.
-
-
```

### Comparing `sqlalchemy-firebird-0.7.6/README.rst` & `sqlalchemy-firebird-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqlalchemy-firebird-0.7.6/setup.py` & `sqlalchemy-firebird-0.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,10 +46,11 @@
     packages=find_packages(include=["sqlalchemy_firebird"]),
     include_package_data=True,
     install_requires=["SQLAlchemy>1.3.16", "fdb"],
     zip_safe=False,
     entry_points={
         "sqlalchemy.dialects": [
             "firebird = sqlalchemy_firebird.fdb:FBDialect_fdb",
+            "firebird.fdb = sqlalchemy_firebird.fdb:FBDialect_fdb",
         ]
     },
 )
```

### Comparing `sqlalchemy-firebird-0.7.6/sqlalchemy_firebird/__init__.py` & `sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from . import base  # noqa
 from . import fdb  # noqa
 from . import provision  # noqa
 
 # Not supporting kinterbase
 # from . import kinterbasdb  # noqa
 
-__version__ = "0.7.6"
+__version__ = "0.8.0"
 
 base.dialect = dialect = fdb.dialect
 
 _registry.register("firebird", "sqlalchemy_firebird.fdb", "FBDialect_fdb")
 
 __all__ = (
     "SMALLINT",
```

### Comparing `sqlalchemy-firebird-0.7.6/sqlalchemy_firebird/base.py` & `sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -660,14 +660,15 @@
         63 characters character set UTF8 (252 bytes).  Prior versions have a
         maximum identifier length of 31 bytes.
 
     max_identifier_length = 31
 
     """
 
+    supports_schemas = False
     supports_sequences = True
     sequences_optional = False
     supports_default_values = True
     postfetch_lastrowid = False
 
     supports_comments = True
     inline_comments = True
@@ -751,15 +752,17 @@
         """Return ``True`` if the given sequence (generator) exists."""
         genqry = """
         SELECT 1 AS has_sequence FROM rdb$database
         WHERE EXISTS (SELECT rdb$generator_name
                       FROM rdb$generators
                       WHERE rdb$generator_name=?)
         """
-        c = connection.execute(genqry, [self.denormalize_name(sequence_name)])
+        c = connection.exec_driver_sql(
+            genqry, (self.denormalize_name(sequence_name),)
+        )
         return c.first() is not None
 
     @reflection.cache
     def get_table_names(self, connection, schema=None, **kw):
         # there are two queries commonly mentioned for this.
         # this one, using view_blr, is at the Firebird FAQ among other places:
         # http://www.firebirdfaq.org/faq174/
@@ -775,74 +778,88 @@
         # any difference between these two.  This link:
         # http://www.alberton.info/firebird_sql_meta_info.html#.Ur3vXfZGni8
         # states them as interchangeable.  Some discussion at [ticket:2898]
         # SELECT DISTINCT rdb$relation_name
         # FROM rdb$relation_fields
         # WHERE rdb$system_flag=0 AND rdb$view_context IS NULL
 
-        return [self.normalize_name(row[0]) for row in connection.execute(s)]
+        return [
+            self.normalize_name(row.relation_name)
+            for row in connection.exec_driver_sql(s)
+        ]
 
     @reflection.cache
     def get_temp_table_names(self, connection, schema=None, **kw):
         s = """
         select TRIM(rdb$relation_name) AS relation_name
         from rdb$relations
         where rdb$view_blr is null
         and (rdb$system_flag is null or rdb$system_flag = 0)
         and rdb$relation_type in (4, 5);
         """
-        return [self.normalize_name(row[0]) for row in connection.execute(s)]
+        return [
+            self.normalize_name(row.relation_name)
+            for row in connection.exec_driver_sql(s)
+        ]
 
     @reflection.cache
     def get_sequence_names(self, connection, schema=None, **kw):
         s = """
-        select TRIM(rdb$generator_name)
+        select TRIM(rdb$generator_name) AS generator_name
         from rdb$generators
         where (rdb$system_flag is null or rdb$system_flag = 0);
         """
-        return [self.normalize_name(row[0]) for row in connection.execute(s)]
+        return [
+            self.normalize_name(row.generator_name)
+            for row in connection.exec_driver_sql(s)
+        ]
 
     @reflection.cache
     def get_view_names(self, connection, schema=None, **kw):
         # see http://www.firebirdfaq.org/faq174/
         s = """
-        select TRIM(rdb$relation_name)
+        select TRIM(rdb$relation_name) AS relation_name
         from rdb$relations
         where rdb$view_blr is not null
         and (rdb$system_flag is null or rdb$system_flag = 0);
         """
-        return [self.normalize_name(row[0]) for row in connection.execute(s)]
+        return [
+            self.normalize_name(row.relation_name)
+            for row in connection.exec_driver_sql(s)
+        ]
 
     @reflection.cache
     def get_view_definition(self, connection, view_name, schema=None, **kw):
         qry = """
         SELECT rdb$view_source AS view_source
         FROM rdb$relations
         WHERE rdb$relation_name=?
         """
-        rp = connection.execute(qry, [self.denormalize_name(view_name)])
+        rp = connection.exec_driver_sql(
+            qry, (self.denormalize_name(view_name),)
+        )
         row = rp.first()
         if row:
-            return row["view_source"]
+            return row.view_source
         else:
             return None
 
     @reflection.cache
     def get_pk_constraint(self, connection, table_name, schema=None, **kw):
         # Query to extract the PK/FK constrained fields of the given table
         keyqry = """
         SELECT TRIM(se.rdb$field_name) AS fname
         FROM rdb$relation_constraints rc
              JOIN rdb$index_segments se ON rc.rdb$index_name=se.rdb$index_name
         WHERE rc.rdb$constraint_type=? AND rc.rdb$relation_name=?
         """
         tablename = self.denormalize_name(table_name)
         # get primary key fields
-        c = connection.execute(keyqry, ["PRIMARY KEY", tablename])
-        pkfields = [self.normalize_name(r["fname"]) for r in c.fetchall()]
+        c = connection.exec_driver_sql(keyqry, ("PRIMARY KEY", tablename))
+        pkfields = [self.normalize_name(r.fname) for r in c.fetchall()]
         return {"constrained_columns": pkfields, "name": None}
 
     @reflection.cache
     def get_column_sequence(
         self, connection, table_name, column_name, schema=None, **kw
     ):
         tablename = self.denormalize_name(table_name)
@@ -861,17 +878,17 @@
           AND tabdep.rdb$depended_on_type=0
           AND trig.rdb$trigger_type=1
           AND tabdep.rdb$field_name=?
           AND (SELECT count(*)
            FROM rdb$dependencies trigdep2
            WHERE trigdep2.rdb$dependent_name = trigdep.rdb$dependent_name) = 2
         """
-        genr = connection.execute(genqry, [tablename, colname]).first()
+        genr = connection.exec_driver_sql(genqry, (tablename, colname)).first()
         if genr is not None:
-            return dict(name=self.normalize_name(genr["fgenerator"]))
+            return dict(name=self.normalize_name(genr.fgenerator))
 
     @reflection.cache
     def get_columns(  # noqa: C901
         self, connection, table_name, schema=None, **kw
     ):
         # Query to extract the details of all the fields of the given table
         tblqry = """
@@ -898,73 +915,71 @@
         """
         # get the PK, used to determine the eventual associated sequence
         pk_constraint = self.get_pk_constraint(connection, table_name)
         pkey_cols = pk_constraint["constrained_columns"]
 
         tablename = self.denormalize_name(table_name)
         # get all of the fields for this table
-        c = [row for row in connection.execute(tblqry, [tablename])]
+        c = [row for row in connection.exec_driver_sql(tblqry, (tablename,))]
         cols = []
         for row in c:
-            name = self.normalize_name(row["fname"])
-            orig_colname = row["fname"]
+            name = self.normalize_name(row.fname)
+            orig_colname = row.fname
 
             # get the data type
-            colspec = row["ftype"].rstrip()
+            colspec = row.ftype.rstrip()
             coltype = self.ischema_names.get(colspec)
             if coltype is None:
                 util.warn(
                     "Did not recognize type '%s' of column '%s'"
                     % (colspec, name)
                 )
                 coltype = sqltypes.NULLTYPE
-            elif issubclass(coltype, Integer) and row["fprec"] != 0:
-                coltype = NUMERIC(
-                    precision=row["fprec"], scale=row["fscale"] * -1
-                )
+            elif issubclass(coltype, Integer) and row.fprec != 0:
+                coltype = NUMERIC(precision=row.fprec, scale=row.fscale * -1)
             elif colspec in ("VARYING", "CSTRING"):
-                coltype = coltype(row["flen"])
+                coltype = coltype(row.flen)
             elif colspec == "TEXT":
-                coltype = TEXT(row["flen"])
+                coltype = TEXT(row.flen)
             elif colspec == "BLOB":
-                if row["stype"] == 1:
+                if row.stype == 1:
                     coltype = TEXT()
                 else:
                     coltype = BLOB()
             else:
                 coltype = coltype()
 
             # does it have a default value?
             defvalue = None
-            if row["fdefault"] is not None:
+            if row.fdefault is not None:
                 # the value comes down as "DEFAULT 'value'": there may be
                 # more than one whitespace around the "DEFAULT" keyword
                 # and it may also be lower case
                 # (see also http://tracker.firebirdsql.org/browse/CORE-356)
-                defexpr = row["fdefault"].lstrip()
+                defexpr = row.fdefault.lstrip()
                 assert defexpr[:8].rstrip().upper() == "DEFAULT", (
                     "Unrecognized default value: %s" % defexpr
                 )
                 defvalue = defexpr[8:].strip()
                 if defvalue == "NULL":
                     # Redundant
                     defvalue = None
             col_d = {
                 "name": name,
                 "type": coltype,
-                "nullable": not bool(row["null_flag"]),
+                "nullable": not bool(row.null_flag),
                 "default": defvalue,
                 "autoincrement": "auto",
             }
 
             if orig_colname.lower() == orig_colname:
                 col_d["quote"] = True
 
-            if row["computed_source"] is not None:
-                col_d["computed"] = {"sqltext": row["computed_source"]}
+            if row.computed_source is not None:
+                col_d["computed"] = {"sqltext": row.computed_source}
 
             # if the PK is a single field, try to see if its linked to
             # a sequence thru a trigger
             if len(pkey_cols) == 1 and name == pkey_cols[0]:
                 seq_d = self.get_column_sequence(connection, tablename, name)
                 if seq_d is not None:
                     col_d["sequence"] = seq_d
@@ -989,35 +1004,33 @@
                   ON se.rdb$index_name=ix2.rdb$index_name
                      AND se.rdb$field_position=cse.rdb$field_position
         WHERE rc.rdb$constraint_type=? AND rc.rdb$relation_name=?
         ORDER BY se.rdb$index_name, se.rdb$field_position
         """
         tablename = self.denormalize_name(table_name)
 
-        c = connection.execute(fkqry, ["FOREIGN KEY", tablename])
+        c = connection.exec_driver_sql(fkqry, ("FOREIGN KEY", tablename))
         fks = util.defaultdict(
             lambda: {
                 "name": None,
                 "constrained_columns": [],
                 "referred_schema": None,
                 "referred_table": None,
                 "referred_columns": [],
             }
         )
 
         for row in c:
-            cname = self.normalize_name(row["cname"])
+            cname = self.normalize_name(row.cname)
             fk = fks[cname]
             if not fk["name"]:
                 fk["name"] = cname
-                fk["referred_table"] = self.normalize_name(row["targetrname"])
-            fk["constrained_columns"].append(self.normalize_name(row["fname"]))
-            fk["referred_columns"].append(
-                self.normalize_name(row["targetfname"])
-            )
+                fk["referred_table"] = self.normalize_name(row.targetrname)
+            fk["constrained_columns"].append(self.normalize_name(row.fname))
+            fk["referred_columns"].append(self.normalize_name(row.targetfname))
         return list(fks.values())
 
     @reflection.cache
     def get_indexes(self, connection, table_name, schema=None, **kw):
         qry = """
         SELECT TRIM(ix.rdb$index_name) AS index_name,
                ix.rdb$unique_flag AS unique_flag,
@@ -1028,26 +1041,28 @@
              LEFT OUTER JOIN rdb$relation_constraints
                   ON rdb$relation_constraints.rdb$index_name =
                         ic.rdb$index_name
         WHERE ix.rdb$relation_name=? AND ix.rdb$foreign_key IS NULL
           AND rdb$relation_constraints.rdb$constraint_type IS NULL
         ORDER BY index_name, ic.rdb$field_position
         """
-        c = connection.execute(qry, [self.denormalize_name(table_name)])
+        c = connection.exec_driver_sql(
+            qry, (self.denormalize_name(table_name),)
+        )
 
         indexes = util.defaultdict(dict)
         for row in c:
-            indexrec = indexes[row["index_name"]]
+            indexrec = indexes[row.index_name]
             if "name" not in indexrec:
-                indexrec["name"] = self.normalize_name(row["index_name"])
+                indexrec["name"] = self.normalize_name(row.index_name)
                 indexrec["column_names"] = []
-                indexrec["unique"] = bool(row["unique_flag"])
+                indexrec["unique"] = bool(row.unique_flag)
 
             indexrec["column_names"].append(
-                self.normalize_name(row["field_name"])
+                self.normalize_name(row.field_name)
             )
 
         return list(indexes.values())
 
     @reflection.cache
     def get_table_comment(self, connection, table_name, schema=None, **kw):
         qry = text(
```

### Comparing `sqlalchemy-firebird-0.7.6/sqlalchemy_firebird/fdb.py` & `sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/fdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,18 @@
             enable_rowcount=enable_rowcount, retaining=retaining, **kwargs
         )
 
     @classmethod
     def dbapi(cls):
         return __import__("fdb")
 
+    @classmethod
+    def import_dbapi(cls):
+        return __import__("fdb")
+
     def create_connect_args(self, url):
         opts = url.translate_connect_args(username="user")
         if opts.get("port"):
             opts["host"] = "%s/%s" % (opts["host"], opts["port"])
             del opts["port"]
         opts.update(url.query)
```

### Comparing `sqlalchemy-firebird-0.7.6/sqlalchemy_firebird/kinterbasdb.py` & `sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/kinterbasdb.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-firebird-0.7.6/sqlalchemy_firebird/requirements.py` & `sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/requirements.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from sqlalchemy.testing.requirements import SuiteRequirements
 from sqlalchemy.testing import exclusions
 
 
 class Requirements(SuiteRequirements):
     @property
+    def array_type(self):
+        return exclusions.open()
+
+    @property
+    def uuid_data_type(self):
+        return exclusions.open()
+
+    @property
     def autoincrement_insert(self):
         return exclusions.closed()
 
     @property
     def computed_columns(self):
         """Supports computed columns"""
         return exclusions.open()
```

### Comparing `sqlalchemy-firebird-0.7.6/sqlalchemy_firebird.egg-info/PKG-INFO` & `sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-firebird
-Version: 0.7.6
+Version: 0.8.0
 Summary: Firebird for SQLAlchemy
 Home-page: https://github.com/pauldex/sqlalchemy-firebird
 Author: Paul Graves-DesLauriers
 Author-email: paul@dexmicro.com
 License: MIT
 Project-URL: Documentation, https://github.com/pauldex/sqlalchemy-firebird/wiki
 Project-URL: Source, https://github.com/pauldex/sqlalchemy-firebird
 Project-URL: Tracker, https://github.com/pauldex/sqlalchemy-firebird/issues
 Keywords: SQLAlchemy Firebird
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database :: Front-Ends
@@ -65,9 +64,7 @@
 
 ----
 
 **License**
 
 sqlalchemy-firebird is distributed under the `MIT license
 <http://www.opensource.org/licenses/mit-license.php>`_.
-
-
```

