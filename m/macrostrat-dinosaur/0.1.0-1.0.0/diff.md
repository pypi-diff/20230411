# Comparing `tmp/macrostrat.dinosaur-0.1.0.tar.gz` & `tmp/macrostrat_dinosaur-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrostrat.dinosaur-0.1.0.tar", max compression
+gzip compressed data, was "macrostrat_dinosaur-1.0.0.tar", max compression
```

## Comparing `macrostrat.dinosaur-0.1.0.tar` & `macrostrat_dinosaur-1.0.0.tar`

### file list

```diff
@@ -1,4 +1,7 @@
--rw-r--r--   0        0        0     9123 2022-05-25 21:38:52.237421 macrostrat.dinosaur-0.1.0/macrostrat/dinosaur/__init__.py
--rw-r--r--   0        0        0      705 2022-05-25 21:44:38.555114 macrostrat.dinosaur-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      897 2022-05-25 22:40:23.609155 macrostrat.dinosaur-0.1.0/setup.py
--rw-r--r--   0        0        0      768 2022-05-25 22:40:23.609427 macrostrat.dinosaur-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10121 2023-04-11 05:06:58.497729 macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/__init__.py
+-rw-r--r--   0        0        0     3836 2023-04-11 05:06:58.498297 macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/upgrade_cluster/__init__.py
+-rw-r--r--   0        0        0     1711 2023-04-11 05:06:58.498793 macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/upgrade_cluster/describe.py
+-rw-r--r--   0        0        0     1796 2023-04-11 05:06:58.498985 macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/upgrade_cluster/restore.py
+-rw-r--r--   0        0        0     3328 2023-04-11 05:06:58.499169 macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/upgrade_cluster/utils.py
+-rw-r--r--   0        0        0      705 2023-04-11 05:10:29.158461 macrostrat_dinosaur-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 macrostrat_dinosaur-1.0.0/PKG-INFO
```

### Comparing `macrostrat.dinosaur-0.1.0/macrostrat/dinosaur/__init__.py` & `macrostrat_dinosaur-1.0.0/macrostrat/dinosaur/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 import os
 import sys
 from contextlib import contextmanager, redirect_stdout
 
-from sqlalchemy.exc import ProgrammingError, IntegrityError
+from sqlalchemy.exc import ProgrammingError, IntegrityError, DataError
 from schemainspect import get_inspector
 from migra import Migration
 from migra.statements import check_for_drop
 from sqlalchemy import text
 from rich import print
+from typing import Callable
 
 from macrostrat.utils import get_logger, cmd
 from macrostrat.database import Database
 from macrostrat.database.utils import (
-    _exec_raw_sql,
     run_sql,
     temp_database,
     connection_args,
 )
 
 
 log = get_logger(__name__)
 
+DatabaseInitializer = Callable[[Database], None]
+
 
 class AutoMigration(Migration):
     def changes_omitting_views(self):
         nsel_drops = self.changes.non_table_selectable_drops()
         nsel_creations = self.changes.non_table_selectable_creations()
         # Warning: this also may omit changes to functions etc. We need to test this.
         for stmt in self.statements:
             if stmt in nsel_drops or stmt in nsel_creations:
                 continue
             yield stmt
 
     def _exec(self, sql, quiet=False):
         """Execute SQL unsafely on an sqlalchemy Engine"""
-        if not quiet:
-            return _exec_raw_sql(self.s_from, sql)
-        try:
-            self.s_from.execute(text(sql))
-        except (ProgrammingError, IntegrityError) as err:
-            log.debug(err)
+        run_sql(self.s_from, sql)
 
     def apply(self, quiet=False):
         n = len(self.statements)
         log.debug(f"Applying migration with {n} operations")
         for stmt in self.statements:
             self._exec(stmt, quiet=quiet)
         self.changes.i_from = get_inspector(
@@ -74,63 +71,83 @@
         statements = "\n".join(self.statements)
         print(statements, file=sys.stderr)
 
 
 def _create_migration(db_engine, target, safe=True, **kwargs):
     # For some reason we need to patch this...
     log.info("Creating an automatic migration")
-    target.dialect.server_version_info = db_engine.dialect.server_version_info
-    m = AutoMigration(db_engine, target, **kwargs)  # , exclude_schema="core_view")
 
-    m.set_safety(safe)
+    # Populate server_version_info if it's not already populated
+    if db_engine.dialect.server_version_info is None:
+        db_engine.connect()
+    if target.dialect.server_version_info is None:
+        target.connect()
+
+    migration = AutoMigration(
+        db_engine, target, **kwargs
+    )  # , exclude_schema="core_view")
+
+    migration.set_safety(safe)
     # Not sure what this does
-    m.add_all_changes()
-    return m
+    migration.add_all_changes()
+    return migration
 
 
 @contextmanager
-def _target_db(url, initialize, quiet=False, redirect=sys.stderr):
-    from . import Database
-
+def _target_db(
+    url: str, initializer: DatabaseInitializer, quiet: bool = False, redirect=sys.stderr
+):
     if quiet:
         redirect = open(os.devnull, "w")
 
     log.debug("Creating migration target")
     with temp_database(url) as engine:
-        db = Database(url)
+        database = Database(url)
         with redirect_stdout(redirect):
-            initialize(db)
+            initializer(database)
         yield engine
 
 
-def create_migration(db, initialize, safe=True, redirect=sys.stderr):
-    url = "postgresql://postgres@db:5432/sparrow_temp_migration"
-    with _target_db(url, initialize, redirect=redirect) as target, redirect_stdout(
-        redirect
-    ):
-        return _create_migration(db.engine, target)
+def create_migration(
+    database: Database,
+    initializer: DatabaseInitializer,
+    target_url: str = "postgresql://postgres@db:5432/sparrow_temp_migration",
+    safe: bool = True,
+    redirect=sys.stderr,
+    **kwargs,
+):
+    with _target_db(
+        target_url, initializer, redirect=redirect
+    ) as target, redirect_stdout(redirect):
+        return _create_migration(database.engine, target, safe=safe, **kwargs)
 
 
-def needs_migration(db):
-    migration = create_migration(db)
+def needs_migration(database: Database, initializer: DatabaseInitializer):
+    migration = create_migration(database, initializer)
     return len(migration.statements) == 0
 
 
-def db_migration(db, initialize, safe=True, apply=False, hide_view_changes=False):
+def db_migration(
+    database: Database,
+    initializer: DatabaseInitializer,
+    safe=True,
+    apply=False,
+    hide_view_changes=False,
+):
     """Create a database migration against the idealized schema"""
-    m = create_migration(db, initialize, safe=safe, redirect=sys.stderr)
+    m = create_migration(database, initializer, safe=safe, redirect=sys.stderr)
     stmts = m.statements
     if hide_view_changes:
         stmts = m.changes_omitting_views()
     print("===MIGRATION BELOW THIS LINE===", file=sys.stderr)
-    for s in stmts:
+    for stmt in stmts:
         if apply:
-            run_sql(db.session, s)
+            run_sql(database.session, stmt)
         else:
-            print(s, file=sys.stdout)
+            print(stmt, file=sys.stdout)
 
 
 def dump_schema(engine):
     flags, dbname = connection_args(engine)
     res = cmd("pg_dump", "--schema-only", flags, dbname, capture_output=True)
     return res.stdout
 
@@ -181,77 +198,87 @@
 
 
 class MigrationManager:
     target_url = "postgresql://postgres@db:5432/sparrow_temp_migration"
     dry_run_url = "postgresql://postgres@db:5432/sparrow_schema_clone"
     schema = None
 
-    def __init__(self, db, _init_function, migrations=[], schema=None):
-        self.db = db
+    def __init__(self, database, _init_function, migrations=None, schema=None):
+        self.db = database
 
         self._init_function = _init_function
-        self._migrations = migrations
+        self._migrations = migrations or []
         self.schema = schema
 
     def add_migration(self, migration):
-        assert issubclass(migration, SparrowMigration)
+        assert issubclass(migration, SchemaMigration)
         self._migrations.append(migration())
 
     def add_module(self, module):
         for _, obj in module.__dict__.items():
             try:
-                assert issubclass(obj, SparrowMigration)
+                assert issubclass(obj, SchemaMigration)
             except (TypeError, AssertionError):
                 continue
-            if obj is SparrowMigration:
+            if obj is SchemaMigration:
                 continue
             self.add_migration(obj)
 
     def apply_migrations(self, engine, target):
         """This is the magic function where an ordered changeset gets
         generated and applied"""
         migrations = [
             m for m in self._migrations if m.should_apply(engine, target, self)
         ]
         log.info("Applying manual migrations")
         if len(migrations) == 0:
-            log.info(f"Found no migrations to apply")
+            log.info("Found no migrations to apply")
         while len(migrations) > 0:
             n = len(migrations)
             log.info(f"Found {n} migrations to apply")
             for m in migrations:
-                log.info(f"Applying migration {m.name}")
+                log.info(f"Applying manual migration {m.name}")
                 m.apply(engine)
                 # We have applied this migration and should not do it again.
                 migrations.remove(m)
             migrations = [m for m in migrations if m.should_apply(engine, target, self)]
 
+    def _pre_auto_migration(self, engine, target):
+        """This is a hook for subclasses to do things before the automatic migration"""
+        pass
+
     def _run_migration(self, engine, target, check=False):
-        m = _create_migration(engine, target, schema=self.schema)
-        if len(m.statements) == 0:
-            log.info("No automatic migration necessary")
-            return
-
-        if m.is_safe:
-            log.info("Applying automatic migration")
-            m.apply(quiet=True)
-            return
+        try:
+            # First, try an automatic migration
+            m = _create_migration(engine, target, schema=self.schema)
+            if len(m.statements) == 0:
+                log.info("No automatic migration necessary")
+                return
+
+            if m.is_safe:
+                log.info("Applying automatic migration")
+                m.apply(quiet=True)
+                return
+        except Exception as exc:
+            log.warning(f"Automatic migration failed: {exc}")
 
         self.apply_migrations(engine, target)
 
-        # Migrating to the new version should now be "safe"
-        m = _create_migration(engine, target)
+        log.info("Running scripts before automatic migrations")
+        self._pre_auto_migration(engine, target)
 
-        for s in m.statements:
-            print(s, file=sys.stderr)
+        # Migrating to the new version should now be possible using a "safe" automatic migration
+        m = _create_migration(engine, target)
 
         try:
             assert m.is_safe
         except AssertionError as err:
-            print("[bold red]Manual migration needed! Unsafe changes:[/bold red]")
+            print("[bold red]Manual migration needed!")
+            print("Run [bold cyan]sparrow db migration[/bold cyan] to see the changes")
+            print("[bold red]Unsafe changes:[/bold red]")
             for s in m.unsafe_changes():
                 print(s, file=sys.stderr)
             raise err
 
         m.apply(quiet=True)
         # Re-add changes (this is time-consuming)
         # m.add_all_changes()
@@ -260,14 +287,15 @@
     def dry_run_migration(self, target):
         log.info("Running dry-run migration")
         with create_schema_clone(self.db.engine, db_url=self.dry_run_url) as src:
             self._run_migration(src, target)
         log.info("Migration dry run successful")
 
     def run_migration(self, dry_run=True, apply=True):
+        log.info("Setting up target database")
         with _target_db(self.target_url, self._init_function) as target:
             if dry_run:
                 self.dry_run_migration(target)
             if not apply:
                 return
             log.info("Running migration")
             self._run_migration(self.db.engine, target)
```

### Comparing `macrostrat.dinosaur-0.1.0/pyproject.toml` & `macrostrat_dinosaur-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 authors = ["Daven Quinn <dev@davenquinn.com>"]
 description = "Diff-based database migrations"
 name = "macrostrat.dinosaur"
 packages = [
   {include = "macrostrat"},
 ]
-version = "0.1.0"
+version = "1.0.0"
 
 [tool.poetry.dependencies]
 GeoAlchemy2 = "^0.9.4"
 SQLAlchemy = "^1.4.26"
 SQLAlchemy-Utils = "^0.37.0"
-"macrostrat.database" = "^1.0.0"
+"macrostrat.database" = "^2.0.0"
 "macrostrat.utils" = "^1.0.0"
 psycopg2-binary = "^2.9.1"
 python = "^3.8"
 schemainspect = "^3.0.1616029793"
 sqlparse = "^0.4.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `macrostrat.dinosaur-0.1.0/PKG-INFO` & `macrostrat_dinosaur-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
-Name: macrostrat.dinosaur
-Version: 0.1.0
+Name: macrostrat-dinosaur
+Version: 1.0.0
 Summary: Diff-based database migrations
 Author: Daven Quinn
 Author-email: dev@davenquinn.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GeoAlchemy2 (>=0.9.4,<0.10.0)
 Requires-Dist: SQLAlchemy (>=1.4.26,<2.0.0)
 Requires-Dist: SQLAlchemy-Utils (>=0.37.0,<0.38.0)
-Requires-Dist: macrostrat.database (>=1.0.0,<2.0.0)
+Requires-Dist: macrostrat.database (>=2.0.0,<3.0.0)
 Requires-Dist: macrostrat.utils (>=1.0.0,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.1,<3.0.0)
 Requires-Dist: schemainspect (>=3.0.1616029793,<4.0.0)
 Requires-Dist: sqlparse (>=0.4.0,<0.5.0)
```

