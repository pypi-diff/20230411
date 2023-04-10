# Comparing `tmp/wring-0.0.2.tar.gz` & `tmp/wring-0.0.4.tar.gz`

## Comparing `wring-0.0.2.tar` & `wring-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 wring-0.0.2/mkdocs.yml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 wring-0.0.2/src/wring/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wring-0.0.2/src/wring/_version.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 wring-0.0.2/src/wring/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wring-0.0.2/src/wring/py.typed
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 wring-0.0.2/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 wring-0.0.2/LICENSE
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 wring-0.0.2/README.md
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 wring-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 wring-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 wring-0.0.4/mkdocs.yml
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 wring-0.0.4/src/wring/__init__.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 wring-0.0.4/src/wring/_app.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wring-0.0.4/src/wring/_version.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 wring-0.0.4/src/wring/csv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wring-0.0.4/src/wring/py.typed
+-rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 wring-0.0.4/src/wring/tar_zst.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 wring-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 wring-0.0.4/LICENSE
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 wring-0.0.4/README.md
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 wring-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 wring-0.0.4/PKG-INFO
```

### Comparing `wring-0.0.2/mkdocs.yml` & `wring-0.0.4/mkdocs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -8,30 +8,35 @@
 
 copyright: Copyright (c) 2023-present Jeff Newman <jeff@newman.me>
 
 theme:
   name: material
   palette:
     - scheme: default
+      primary: blue
       toggle:
         icon: material/brightness-7
         name: Switch to dark mode
     - scheme: slate
+      primary: indigo
       toggle:
         icon: material/brightness-4
         name: Switch to light mode
   font:
     text: Roboto
     code: Roboto Mono
+  icon:
+    logo: material/water-opacity
 
 markdown_extensions:
   - pymdownx.highlight:
       anchor_linenums: true
   - pymdownx.superfences
   - mkdocs-click
+  - mkdocs-typer
 
 plugins:
   - search:
   - git-revision-date-localized:
       type: timeago
       enable_creation_date: true
   - mkdocstrings:
```

### Comparing `wring-0.0.2/src/wring/main.py` & `wring-0.0.4/src/wring/csv.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 import os
+from pathlib import Path
 
-import click
 import pyarrow.csv as pc
 import pyarrow.parquet as pq
+import typer
+from rich import print
 
+from ._app import app
 
-@click.command()
-@click.argument("directory", type=click.Path(exists=True))
-@click.option("--compression", default="zstd", help="compression algorithm")
-@click.option("--compression-level", default=9, help="compression level")
-@click.option(
-    "--clean/--no-clean",
-    default=False,
-    help="remove uncompressed files after successful wringing",
-)
-def wring(directory, compression, compression_level, clean):
+
+@app.command()
+def csv(
+    directory: Path,
+    compression: str = typer.Option("zstd", help="compression algorithm"),
+    compression_level: int = typer.Option(9, help="compression level"),
+    clean: bool = typer.Option(
+        False, help="remove uncompressed files after successful wringing"
+    ),
+):
     """Crawl a directory and compress csv files into parquet."""
-    click.echo(f"wringing {directory} [{compression=}, {compression_level=}]")
-    click.echo(f"[{compression=}, {compression_level=}]")
+    if not directory.exists():
+        raise FileNotFoundError(directory)
+    print(f"wringing {directory} [{compression=}, {compression_level=}]")
+    print(f"[{compression=}, {compression_level=}]")
     for dirpath, _dirnames, filenames in os.walk(directory):
         for f in filenames:
             source = os.path.join(dirpath, f)
             target = None
             if source.endswith(".csv"):
                 target = source[:-4] + ".parquet"
             elif source.endswith(".csv.gz"):
                 target = source[:-7] + ".parquet"
             if target is not None:
                 if not os.path.exists(target):
-                    click.echo(click.style("converting ", fg="green") + source)
+                    print(f"[green]converting[/green] {source}")
                     try:
                         t = pc.read_csv(source)
                         pq.write_table(
                             t,
                             target,
                             compression=compression,
                             compression_level=compression_level,
                         )
                     except Exception as err:
-                        click.echo(click.style(str(err), fg="red", bold=True))
+                        print(f"[bold red]{err}[/bold red]")
                     else:
                         if clean and os.path.exists(target):
                             if pq.read_table(target).equals(t, check_metadata=True):
                                 os.unlink(source)
                 else:
-                    click.echo(
-                        click.style("not converting ", fg="red")
-                        + source
-                        + click.style(" (parquet already exists)", fg="red")
+                    print(
+                        f"[red]not converting[/red] {source} "
+                        "[red](parquet already exists)[/red]"
                     )
-
-
-if __name__ == "__main__":
-    wring()
```

### Comparing `wring-0.0.2/.gitignore` & `wring-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `wring-0.0.2/LICENSE` & `wring-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wring-0.0.2/pyproject.toml` & `wring-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,28 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "pyarrow",
+  "rich",
+  "typer",
+  "zstandard",
 ]
 description = "A tool to compress multiple CSV data files into parquet"
 dynamic = ["version"]
 keywords = []
 license = "MIT"
 name = "wring"
 readme = "README.md"
 requires-python = ">=3.10"
 
 [project.scripts]
-wring = "wring.main:wring"
+wring = "wring:app"
 
 [project.urls]
 Documentation = "https://jpn--.github.io/wring"
 Issues = "https://github.com/jpn--/wring/issues"
 Source = "https://github.com/jpn--/wring"
 
 [tool.hatch.version]
@@ -36,14 +39,15 @@
 [project.optional-dependencies]
 docs = [
   "mkdocs~=1.4.0",
   "mkdocs-material~=8.5.4",
   "mkdocs-git-revision-date-localized-plugin~=1.1.0",
   "mkdocstrings[python]~=0.19.0",
   "mkdocs-click",
+  "mkdocs-typer",
 ]
 quality = [
   "black~=22.10.0",
   "ruff",
   "pre-commit~=2.20.0",
 ]
 tests = [
```

### Comparing `wring-0.0.2/PKG-INFO` & `wring-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: wring
-Version: 0.0.2
+Version: 0.0.4
 Summary: A tool to compress multiple CSV data files into parquet
 Project-URL: Documentation, https://jpn--.github.io/wring
 Project-URL: Issues, https://github.com/jpn--/wring/issues
 Project-URL: Source, https://github.com/jpn--/wring
 Author: Jeff Newman
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: pyarrow
+Requires-Dist: rich
+Requires-Dist: typer
+Requires-Dist: zstandard
 Provides-Extra: docs
 Requires-Dist: mkdocs-click; extra == 'docs'
 Requires-Dist: mkdocs-git-revision-date-localized-plugin~=1.1.0; extra == 'docs'
 Requires-Dist: mkdocs-material~=8.5.4; extra == 'docs'
+Requires-Dist: mkdocs-typer; extra == 'docs'
 Requires-Dist: mkdocstrings[python]~=0.19.0; extra == 'docs'
 Requires-Dist: mkdocs~=1.4.0; extra == 'docs'
 Provides-Extra: quality
 Requires-Dist: black~=22.10.0; extra == 'quality'
 Requires-Dist: pre-commit~=2.20.0; extra == 'quality'
 Requires-Dist: ruff; extra == 'quality'
 Provides-Extra: tests
```

