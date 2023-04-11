# Comparing `tmp/peewee_migrate-1.7.0.tar.gz` & `tmp/peewee_migrate-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_migrate-1.7.0.tar", max compression
+gzip compressed data, was "peewee_migrate-1.7.1.tar", max compression
```

## Comparing `peewee_migrate-1.7.0.tar` & `peewee_migrate-1.7.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4453 2023-03-22 19:35:27.034475 peewee_migrate-1.7.0/README.rst
--rw-r--r--   0        0        0      146 2023-03-22 19:35:27.034475 peewee_migrate-1.7.0/peewee_migrate/__init__.py
--rw-r--r--   0        0        0       78 2023-03-22 19:35:27.034475 peewee_migrate-1.7.0/peewee_migrate/__main__.py
--rw-r--r--   0        0        0    11993 2023-03-22 19:35:27.034475 peewee_migrate-1.7.0/peewee_migrate/auto.py
--rw-r--r--   0        0        0     6591 2023-03-22 19:35:27.034475 peewee_migrate-1.7.0/peewee_migrate/cli.py
--rw-r--r--   0        0        0      146 2023-03-22 19:35:27.034475 peewee_migrate-1.7.0/peewee_migrate/logs.py
--rw-r--r--   0        0        0    15604 2023-03-22 19:35:27.034475 peewee_migrate-1.7.0/peewee_migrate/migrator.py
--rw-r--r--   0        0        0      465 2023-03-22 19:35:27.034475 peewee_migrate-1.7.0/peewee_migrate/models.py
--rw-r--r--   0        0        0        0 2023-03-22 19:35:27.034475 peewee_migrate-1.7.0/peewee_migrate/py.typed
--rw-r--r--   0        0        0    12203 2023-03-22 19:35:27.034475 peewee_migrate-1.7.0/peewee_migrate/router.py
--rw-r--r--   0        0        0     1681 2023-03-22 19:35:27.034475 peewee_migrate-1.7.0/peewee_migrate/template.py
--rw-r--r--   0        0        0      255 2023-03-22 19:35:27.034475 peewee_migrate-1.7.0/peewee_migrate/types.py
--rw-r--r--   0        0        0     1496 2023-03-22 19:35:27.034475 peewee_migrate-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     5687 1970-01-01 00:00:00.000000 peewee_migrate-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     4456 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/README.rst
+-rw-r--r--   0        0        0      146 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/__init__.py
+-rw-r--r--   0        0        0       78 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/__main__.py
+-rw-r--r--   0        0        0    11993 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/auto.py
+-rw-r--r--   0        0        0     6597 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/cli.py
+-rw-r--r--   0        0        0      146 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/logs.py
+-rw-r--r--   0        0        0    15733 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/migrator.py
+-rw-r--r--   0        0        0      465 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/models.py
+-rw-r--r--   0        0        0        0 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/py.typed
+-rw-r--r--   0        0        0    12194 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/router.py
+-rw-r--r--   0        0        0     1681 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/template.py
+-rw-r--r--   0        0        0      255 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/types.py
+-rw-r--r--   0        0        0     1600 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     5690 1970-01-01 00:00:00.000000 peewee_migrate-1.7.1/PKG-INFO
```

### Comparing `peewee_migrate-1.7.0/README.rst` & `peewee_migrate-1.7.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 =============
 
 - peewee >= 3.8
 
 Dependency Note
 ---------------
 
-For ``Peewee<3.0`` please use ``Peewee-Migrate==0.14.0``.
-For ``Python 3.0-3.6`` please use ``Peewee-Migrate==1.1.6``.
-For ``Python 3.7`` please use ``Peewee-Migrate==1.6.6``.
+- For ``Peewee<3.0`` please use ``Peewee-Migrate==0.14.0``
+- For ``Python 3.0-3.6`` please use ``Peewee-Migrate==1.1.6``
+- For ``Python 3.7`` please use ``Peewee-Migrate==1.6.6``
 
 .. _installation:
 
 Installation
 =============
 
 **Peewee Migrate** should be installed using pip: ::
```

### Comparing `peewee_migrate-1.7.0/peewee_migrate/auto.py` & `peewee_migrate-1.7.1/peewee_migrate/auto.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.0/peewee_migrate/cli.py` & `peewee_migrate-1.7.1/peewee_migrate/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ignore = schema = None
 
     if directory:
         directory = Path(directory)
         try:
             with directory.joinpath("conf.py").open() as cfg:
                 code = compile(cfg.read(), "<string>", "exec", dont_inherit=True)
-                exec(code, config, config)  # noqa: S102
+                exec(code, config, config)
                 database = config.get("DATABASE", database)
                 ignore = config.get("IGNORE", ignore)
                 schema = config.get("SCHEMA", schema)
                 migratetable = config.get("MIGRATE_TABLE", migratetable)
                 logging_level = config.get("LOGGING_LEVEL", logging_level).upper()
 
         except IOError:
@@ -67,15 +67,15 @@
     except RuntimeError:
         logger.exception("Failed to initialize router")
         return sys.exit(1)
 
 
 @click.group()
 def cli():
-    """Just a group."""
+    """Migrate database with Peewee ORM."""
     logging.basicConfig(level=logging.INFO)
 
 
 @cli.command()
 @click.option("--name", default=None, help="Select migration")
 @click.option("--database", default=None, help="Database connection")
 @click.option("--directory", default="migrations", help="Directory where migrations are stored")
```

### Comparing `peewee_migrate-1.7.0/peewee_migrate/migrator.py` & `peewee_migrate-1.7.1/peewee_migrate/migrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,21 @@
 
     def drop_table(self, model: pw.Model, *, cascade: bool = True) -> Callable:
         """Sqlite doesnt support cascade syntax by default."""
         return lambda: model.drop_table(cascade=False)
 
     def alter_change_column(self, table: str, column: str, field: pw.Field) -> Operation:
         """Support change columns."""
-        return self._update_column(table, column, lambda a, b: b)  # type: ignore[]
+
+        def fn(c_name, c_def):
+            ctx = self.make_context()
+            ctx.sql(field.ddl(ctx))
+            return ctx.query()[0]
+
+        return self._update_column(table, column, fn)  # type: ignore[]
 
 
 class ORM:
     __slots__ = ("__tables__", "__models__")
 
     def __init__(self):
         self.__tables__ = {}
```

### Comparing `peewee_migrate-1.7.0/peewee_migrate/router.py` & `peewee_migrate-1.7.1/peewee_migrate/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
     def read(self, name):
         """Read migration from file."""
         path = self.migrate_dir / (name + ".py")
         with path.open("r") as f:
             code = f.read()
             scope = {}
             code = compile(code, "<string>", "exec", dont_inherit=True)
-            exec(code, scope, None)  # noqa:
+            exec(code, scope, None)
             return scope.get("migrate", void), scope.get("rollback", void)
 
     def clear(self):
         """Remove migrations from fs."""
         super(Router, self).clear()
         for name in self.todo:
             path = self.migrate_dir / (name + ".py")
```

### Comparing `peewee_migrate-1.7.0/peewee_migrate/template.py` & `peewee_migrate-1.7.1/peewee_migrate/template.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.0/pyproject.toml` & `peewee_migrate-1.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-migrate"
-version = "1.7.0"
+version = "1.7.1"
 homepage = "https://github.com/klen/peewee_migrate"
 repository = "https://github.com/klen/peewee_migrate"
 description = "Support for migrations in Peewee ORM"
 readme = "README.rst"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["peewee", "migrations", "orm"]
@@ -18,14 +18,18 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
 
+[tool.poetry.scripts]
+pw_migrate = "peewee_migrate.cli:cli"
+pw-migrate = "peewee_migrate.cli:cli"
+
 [tool.poetry.dependencies]
 python = "^3.8"
 peewee = "^3"
 click = "*"
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
@@ -35,15 +39,15 @@
 pytest-mypy = "*"
 ruff = "*"
 
 [tool.ruff]
 line-length = 100
 target-version = "py38"
 select = ["ALL"]
-ignore = ["ANN", "ARG", "COM", "D", "N", "UP", "SLF", "INP001"]
+ignore = ["ANN", "ARG", "COM", "D", "N", "UP", "S", "SLF", "INP001"]
 
 [tool.pytest.ini_options]
 addopts = "-svx --mypy"
 
 [tool.mypy]
 packages = ["peewee_migrate"]
 ignore_missing_imports = true
```

### Comparing `peewee_migrate-1.7.0/PKG-INFO` & `peewee_migrate-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-migrate
-Version: 1.7.0
+Version: 1.7.1
 Summary: Support for migrations in Peewee ORM
 Home-page: https://github.com/klen/peewee_migrate
 License: MIT
 Keywords: peewee,migrations,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -64,17 +64,17 @@
 =============
 
 - peewee >= 3.8
 
 Dependency Note
 ---------------
 
-For ``Peewee<3.0`` please use ``Peewee-Migrate==0.14.0``.
-For ``Python 3.0-3.6`` please use ``Peewee-Migrate==1.1.6``.
-For ``Python 3.7`` please use ``Peewee-Migrate==1.6.6``.
+- For ``Peewee<3.0`` please use ``Peewee-Migrate==0.14.0``
+- For ``Python 3.0-3.6`` please use ``Peewee-Migrate==1.1.6``
+- For ``Python 3.7`` please use ``Peewee-Migrate==1.6.6``
 
 .. _installation:
 
 Installation
 =============
 
 **Peewee Migrate** should be installed using pip: ::
```

