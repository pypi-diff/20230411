# Comparing `tmp/pydbbackups-0.0.3.tar.gz` & `tmp/pydbbackups-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbbackups-0.0.3.tar", max compression
+gzip compressed data, was "pydbbackups-0.0.4.tar", max compression
```

## Comparing `pydbbackups-0.0.3.tar` & `pydbbackups-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1074 2023-04-10 18:04:15.039262 pydbbackups-0.0.3/LICENSE
--rw-r--r--   0        0        0      761 2023-04-10 17:17:51.024476 pydbbackups-0.0.3/README.md
--rw-r--r--   0        0        0      394 2023-04-09 16:37:42.039199 pydbbackups-0.0.3/pydbbackups/__init__.py
--rw-r--r--   0        0        0       85 2023-03-26 16:35:39.235013 pydbbackups-0.0.3/pydbbackups/backups/__init__.py
--rw-r--r--   0        0        0     1474 2023-04-09 16:37:28.839768 pydbbackups-0.0.3/pydbbackups/backups/base.py
--rw-r--r--   0        0        0      776 2023-04-04 15:17:50.157968 pydbbackups-0.0.3/pydbbackups/backups/mongodb.py
--rw-r--r--   0        0        0     1201 2023-04-10 14:23:53.741447 pydbbackups-0.0.3/pydbbackups/backups/postgres.py
--rw-r--r--   0        0        0        0 2023-04-09 16:28:12.507897 pydbbackups-0.0.3/pydbbackups/cli/__init__.py
--rw-r--r--   0        0        0      475 2023-04-04 15:26:47.389488 pydbbackups-0.0.3/pydbbackups/cli/config.py
--rw-r--r--   0        0        0     1680 2023-04-10 16:43:42.903888 pydbbackups-0.0.3/pydbbackups/cli/main.py
--rw-r--r--   0        0        0       27 2023-04-04 15:31:15.953085 pydbbackups-0.0.3/pydbbackups/cli/models/__init__.py
--rw-r--r--   0        0        0      325 2023-04-09 16:07:03.941354 pydbbackups-0.0.3/pydbbackups/cli/models/backup_data.py
--rw-r--r--   0        0        0       36 2023-04-09 18:03:20.321476 pydbbackups-0.0.3/pydbbackups/cli/services/__init__.py
--rw-r--r--   0        0        0     1715 2023-04-10 14:38:28.130620 pydbbackups-0.0.3/pydbbackups/cli/services/backups.py
--rw-r--r--   0        0        0     1453 2023-04-10 16:49:51.999547 pydbbackups-0.0.3/pydbbackups/cli/utils/__init__.py
--rw-r--r--   0        0        0      526 2023-04-09 16:37:14.487168 pydbbackups-0.0.3/pydbbackups/errors.py
--rw-r--r--   0        0        0      654 2023-04-10 18:01:31.897934 pydbbackups-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 pydbbackups-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-10 18:04:15.039262 pydbbackups-0.0.4/LICENSE
+-rw-r--r--   0        0        0      762 2023-04-11 15:50:15.989646 pydbbackups-0.0.4/README.md
+-rw-r--r--   0        0        0      394 2023-04-11 16:03:17.287223 pydbbackups-0.0.4/pydbbackups/__init__.py
+-rw-r--r--   0        0        0       85 2023-03-26 16:35:39.235013 pydbbackups-0.0.4/pydbbackups/backups/__init__.py
+-rw-r--r--   0        0        0     1443 2023-04-11 14:59:10.375930 pydbbackups-0.0.4/pydbbackups/backups/base.py
+-rw-r--r--   0        0        0      776 2023-04-04 15:17:50.157968 pydbbackups-0.0.4/pydbbackups/backups/mongodb.py
+-rw-r--r--   0        0        0     1201 2023-04-10 14:23:53.741447 pydbbackups-0.0.4/pydbbackups/backups/postgres.py
+-rw-r--r--   0        0        0        0 2023-04-09 16:28:12.507897 pydbbackups-0.0.4/pydbbackups/cli/__init__.py
+-rw-r--r--   0        0        0      475 2023-04-04 15:26:47.389488 pydbbackups-0.0.4/pydbbackups/cli/config.py
+-rw-r--r--   0        0        0     1854 2023-04-11 16:10:46.105655 pydbbackups-0.0.4/pydbbackups/cli/main.py
+-rw-r--r--   0        0        0       27 2023-04-04 15:31:15.953085 pydbbackups-0.0.4/pydbbackups/cli/models/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-09 16:07:03.941354 pydbbackups-0.0.4/pydbbackups/cli/models/backup_data.py
+-rw-r--r--   0        0        0       36 2023-04-09 18:03:20.321476 pydbbackups-0.0.4/pydbbackups/cli/services/__init__.py
+-rw-r--r--   0        0        0     1715 2023-04-11 15:52:37.888137 pydbbackups-0.0.4/pydbbackups/cli/services/backups.py
+-rw-r--r--   0        0        0     1453 2023-04-10 16:49:51.999547 pydbbackups-0.0.4/pydbbackups/cli/utils/__init__.py
+-rw-r--r--   0        0        0      526 2023-04-09 16:37:14.487168 pydbbackups-0.0.4/pydbbackups/errors.py
+-rw-r--r--   0        0        0      654 2023-04-11 16:10:38.665692 pydbbackups-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 pydbbackups-0.0.4/PKG-INFO
```

### Comparing `pydbbackups-0.0.3/LICENSE` & `pydbbackups-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydbbackups-0.0.3/README.md` & `pydbbackups-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ```bash
 pip install pydbbackups
 ```
 
 ## CLI example
 
 ```bash
-dbbackups run \
+dbbackups dump \
     --name backup-example \
     --database-type postgres \
     --host localhost \
     --database test \
     --username postgres \
     --port 5432
```

### Comparing `pydbbackups-0.0.3/pydbbackups/backups/base.py` & `pydbbackups-0.0.4/pydbbackups/backups/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 @dataclass
 class Backup:
     host: str
     username: str
     database: str
 
     uri: Optional[str] = None
-    name: Optional[str] = None
     password: Optional[str] = None
     port: Optional[int] = None
 
     compress: Optional[bool] = False
 
     CMDS_TO_CHECK: Optional[Sequence[Tuple[str, Optional[str]] | str]] = None
```

### Comparing `pydbbackups-0.0.3/pydbbackups/backups/mongodb.py` & `pydbbackups-0.0.4/pydbbackups/backups/mongodb.py`

 * *Files identical despite different names*

### Comparing `pydbbackups-0.0.3/pydbbackups/backups/postgres.py` & `pydbbackups-0.0.4/pydbbackups/backups/postgres.py`

 * *Files identical despite different names*

### Comparing `pydbbackups-0.0.3/pydbbackups/cli/main.py` & `pydbbackups-0.0.4/pydbbackups/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 from rich.table import Table
 from rich.console import Console
 from pydbbackups.cli.config import build_config
 from pydbbackups.cli.services import BackupsService
 
 
-@click.group()
+@click.group(invoke_without_command=True, no_args_is_help=True)
+@click.version_option('0.0.4', prog_name='dbbackups')
 def app():
     """ Awesome APP """
 
 
 @app.command(name='list')
 def get_backups():
     table = Table()
@@ -23,15 +24,15 @@
     for bfile, bdata in BackupsService.list_backups():
         table.add_row(bfile.name, bdata.database_name, bfile.date)
 
     console = Console()
     console.print(table)
 
 
-@app.command(name='run')
+@app.command(name='dump')
 @click.option('--name', required=True)
 @click.option('--database-type', required=True, type=click.Choice(['postgres', 'mongodb']))
 @click.option('--host', required=True)
 @click.option('--database', required=True)
 @click.option('--username', default=None)
 @click.option('--password', default=None)
 @click.option('--without-password', default=False)
@@ -44,23 +45,24 @@
         password = getpass.getpass('Password: ')
 
     if without_password is True:
         password = None
 
     service = BackupsService.build(
         database_type,
-        name=name,
         host=host,
         database=database,
         username=username,
         password=password,
         port=port,
         compress=compress)
 
-    service.dump(name)
+    console = Console()
+    with console.status("[bold green]Dumping database ..."):
+        service.dump(name)
 
 
 def main():
     build_config()
     app()
```

### Comparing `pydbbackups-0.0.3/pydbbackups/cli/services/backups.py` & `pydbbackups-0.0.4/pydbbackups/cli/services/backups.py`

 * *Files identical despite different names*

### Comparing `pydbbackups-0.0.3/pydbbackups/cli/utils/__init__.py` & `pydbbackups-0.0.4/pydbbackups/cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pydbbackups-0.0.3/pydbbackups/errors.py` & `pydbbackups-0.0.4/pydbbackups/errors.py`

 * *Files identical despite different names*

### Comparing `pydbbackups-0.0.3/pyproject.toml` & `pydbbackups-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydbbackups"
-version = "0.0.3"
+version = "0.0.4"
 description = "DB backups handler"
 authors = ["jbuendia1y <jgamer669@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jbuendia1y/pydbbackups"
 repository = "https://github.com/jbuendia1y/pydbbackups"
 keywords = ["backups", "databases", "handler", "library", "cli"]
```

### Comparing `pydbbackups-0.0.3/PKG-INFO` & `pydbbackups-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbbackups
-Version: 0.0.3
+Version: 0.0.4
 Summary: DB backups handler
 Home-page: https://github.com/jbuendia1y/pydbbackups
 License: MIT
 Keywords: backups,databases,handler,library,cli
 Author: jbuendia1y
 Author-email: jgamer669@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -27,15 +27,15 @@
 ```bash
 pip install pydbbackups
 ```
 
 ## CLI example
 
 ```bash
-dbbackups run \
+dbbackups dump \
     --name backup-example \
     --database-type postgres \
     --host localhost \
     --database test \
     --username postgres \
     --port 5432
```

