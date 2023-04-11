# Comparing `tmp/creosote-2.5.0-py3-none-any.whl.zip` & `tmp/creosote-2.6.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 14112 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 creosote/__about__.py
+Zip file size: 14152 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       25 b- defN 20-Feb-02 00:00 creosote/__about__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 creosote/__init__.py
--rw-r--r--  2.0 unx     6574 b- defN 20-Feb-02 00:00 creosote/cli.py
--rw-r--r--  2.0 unx      882 b- defN 20-Feb-02 00:00 creosote/formatters.py
--rw-r--r--  2.0 unx      520 b- defN 20-Feb-02 00:00 creosote/models.py
+-rw-r--r--  2.0 unx     6597 b- defN 20-Feb-02 00:00 creosote/cli.py
+-rw-r--r--  2.0 unx     1109 b- defN 20-Feb-02 00:00 creosote/formatters.py
+-rw-r--r--  2.0 unx      523 b- defN 20-Feb-02 00:00 creosote/models.py
 -rw-r--r--  2.0 unx     8558 b- defN 20-Feb-02 00:00 creosote/parsers.py
--rw-r--r--  2.0 unx     8827 b- defN 20-Feb-02 00:00 creosote/resolvers.py
-?rw-r--r--  2.0 unx    13037 b- defN 20-Feb-02 00:00 creosote-2.5.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 creosote-2.5.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 creosote-2.5.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 creosote-2.5.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      932 b- defN 20-Feb-02 00:00 creosote-2.5.0.dist-info/RECORD
-12 files, 40558 bytes uncompressed, 12554 bytes compressed:  69.0%
+-rw-r--r--  2.0 unx     9413 b- defN 20-Feb-02 00:00 creosote/resolvers.py
+?rw-r--r--  2.0 unx    13016 b- defN 20-Feb-02 00:00 creosote-2.6.0rc1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 creosote-2.6.0rc1.dist-info/WHEEL
+?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 creosote-2.6.0rc1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 creosote-2.6.0rc1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      948 b- defN 20-Feb-02 00:00 creosote-2.6.0rc1.dist-info/RECORD
+12 files, 41395 bytes uncompressed, 12564 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: creosote/parsers.py
 Comment: 
 
 Filename: creosote/resolvers.py
 Comment: 
 
-Filename: creosote-2.5.0.dist-info/METADATA
+Filename: creosote-2.6.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: creosote-2.5.0.dist-info/WHEEL
+Filename: creosote-2.6.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: creosote-2.5.0.dist-info/entry_points.txt
+Filename: creosote-2.6.0rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: creosote-2.5.0.dist-info/licenses/LICENSE
+Filename: creosote-2.6.0rc1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: creosote-2.5.0.dist-info/RECORD
+Filename: creosote-2.6.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## creosote/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "2.5.0"
+__version__ = "2.6.0rc1"
```

## creosote/cli.py

```diff
@@ -68,15 +68,15 @@
         help="increase output verbosity",
     )
     parser.add_argument(
         "-f",
         "--format",
         dest="format",
         default="default",
-        choices=["default", "porcelain"],
+        choices=["default", "no-color", "porcelain"],
         help="output format",
     )
 
     if Features.ARGS_CAN_BE_SPECIFIED_MULTIPLE_TIMES.value in sys.argv:
         # v3.0 behavior
         parser.add_argument(
             "-p",
@@ -143,15 +143,15 @@
     parser.add_argument(
         "-v",
         "--venv",
         dest="venvs",
         metavar="PATH",
         action=CustomAppendAction,
         default=[".venv"],
-        help="path(s) to the virtual environment to scan",
+        help="path(s) to the virtual environment (or site-packages)",
     )
     parser.add_argument(
         "--use-feature",
         dest="features",
         metavar="FEATURE",
         action="append",
         choices=[v.value for v in Features.__members__.values()],
```

## creosote/formatters.py

```diff
@@ -6,15 +6,23 @@
 
 def configure_logger(verbose: bool, format_: str) -> None:
     logger.remove()
 
     if format_ == "porcelain":
         logger.add(sys.stderr, level="CRITICAL")
         return
+    if format_ == "no-color":
+        logger.add(
+            sys.stderr,
+            level="DEBUG" if verbose else "INFO",
+            colorize=False,
+            format="<level>{message}</level>",
+        )
     else:
+        # default
         logger.add(
             sys.stderr,
             level="DEBUG" if verbose else "INFO",
             colorize=True,
             format="<level>{message}</level>",
         )
```

## creosote/models.py

```diff
@@ -9,10 +9,10 @@
     alias: Optional[str] = None
 
 
 @dataclasses.dataclass
 class DependencyInfo:
     name: str  # as defined in the dependencies specification file
     top_level_import_names: Optional[List[str]] = None
-    distlib_db_import_name: Optional[str] = None
+    record_import_names: Optional[List[str]] = None
     canonicalized_dep_name: Optional[str] = None
     associated_imports: List[ImportInfo] = dataclasses.field(default_factory=list)
```

## creosote/resolvers.py

```diff
@@ -1,14 +1,13 @@
 import os
 import pathlib
 import re
 from pathlib import Path
 from typing import List
 
-from distlib import database
 from loguru import logger
 
 from creosote.models import DependencyInfo, ImportInfo
 
 
 class DepsResolver:
     def __init__(
@@ -22,52 +21,59 @@
             DependencyInfo(name=dep) for dep in dependency_names
         ]
         self.venvs: List[str] = venvs
 
         self.top_level_txt_pattern = re.compile(
             r"\/([\w]*).[\d\.]*.dist-info\/top_level.txt"
         )
+        self.record_pattern = re.compile(r"\/([\w]*).[\d\.]*.dist-info\/RECORD")
 
         self.top_level_filepaths: List[pathlib.Path] = []
+        self.record_filepaths: List[pathlib.Path] = []
         self.unused_deps: List[DependencyInfo] = []
 
     @staticmethod
     def canonicalize_module_name(module_name: str) -> str:
         return module_name.replace("-", "_").replace(".", "_").strip()
 
     def is_importable(self, module_name: str) -> bool:
         try:
             __import__(self.canonicalize_module_name(module_name))
             return True
         except ImportError:
             return False
 
+    def gather_filepaths(self, venv: str, glob_str: str) -> List[Path]:
+        logger.debug(f"Gathering all top_level.txt files in venv {venv}...")
+        venv_path = pathlib.Path(venv)
+        filepaths = list(venv_path.glob(glob_str))
+        for filepath in filepaths:
+            logger.debug(f"Found {filepath}")
+        return sorted(set(filepaths))
+
     def gather_top_level_filepaths(self, venv: str) -> None:
         """Gathers all top_level.txt filepaths in the venv.
 
         Note:
             The path may contain case sensitive variations of the
             dependency name, like e.g. GitPython for gitpython.
         """
 
-        venv_exists = Path(venv).exists()
-        if not venv_exists:
-            logger.warning(
-                f"Virtual environment(s) '{', '.join(self.venvs)}' does not exist, "
-                "cannot resolve top-level names. This may lead to incorrect results."
-            )
-
-        logger.debug("Gathering all top_level.txt files in venv...")
-        venv_path = pathlib.Path(venv)
         glob_str = "**/*.dist-info/top_level.txt"
-        top_level_filepaths = venv_path.glob(glob_str)
-        self.top_level_filepaths.extend(top_level_filepaths)
-        self.top_level_filepaths = sorted(set(self.top_level_filepaths))
-        for top_level_filepath in self.top_level_filepaths:
-            logger.debug(f"Found {top_level_filepath}")
+        self.top_level_filepaths = self.gather_filepaths(venv=venv, glob_str=glob_str)
+
+    def gather_record_filepaths(self, venv: str) -> None:
+        """Gathers all RECORD filepaths in the venv.
+
+        Note:
+            The path may contain case sensitive variations of the
+            dependency name, like e.g. GitPython for gitpython.
+        """
+        glob_str = "**/*.dist-info/RECORD"
+        self.record_filepaths = self.gather_filepaths(venv=venv, glob_str=glob_str)
 
     def map_dep_to_import_via_top_level_txt_file(
         self, dep_info: DependencyInfo
     ) -> bool:
         """Map dependency to import via top_level.txt file.
 
         Return True if import name was found in the top_level.txt,
@@ -79,92 +85,84 @@
             normalized_top_level_filepath = top_level_filepath.as_posix()
             matches = self.top_level_txt_pattern.findall(normalized_top_level_filepath)
             for import_name_from_top_level in matches:
                 if import_name_from_top_level.lower() == dep_name.lower():
                     with open(top_level_filepath, "r", encoding="utf-8") as infile:
                         lines = infile.readlines()
                     dep_info.top_level_import_names = [line.strip() for line in lines]
-                    import_names = ",".join(dep_info.top_level_import_names)
+                    import_names = ", ".join(dep_info.top_level_import_names)
                     logger.debug(
-                        f"[{dep_info.name}] found import name "
+                        f"[{dep_info.name}] found import name(s) "
                         f"via top_level.txt: {import_names} ⭐️"
                     )
                     return True
         logger.debug(f"[{dep_info.name}] did not find top_level.txt in venv")
         return False
 
-    def map_dep_to_module_via_distlib(self, dep_info: DependencyInfo) -> bool:
-        """Fallback to distlib if we can't find the top_level.txt file.
+    def map_dep_to_import_via_record_file(self, dep_info: DependencyInfo) -> bool:
+        dep_name = self.canonicalize_module_name(dep_info.name)
 
-        Return True if import name was found in the distlib database,
-        otherwise return False.
+        for record_filepath in self.record_filepaths:
+            normalized_record_filepath = record_filepath.as_posix()
+            matches = self.record_pattern.findall(normalized_record_filepath)
+            for import_name_from_record in matches:
+                if import_name_from_record.lower() == dep_name.lower():
+                    with open(record_filepath, "r", encoding="utf-8") as infile:
+                        lines = infile.readlines()
 
-        It seems this brings very little value right now, but I'll
-        leave it in for now...
-        """
-        dp = database.DistributionPath(include_egg=True)
-        dist = dp.get_distribution(dep_info.name)
-        found_module_name = None
-
-        if dist is None:
-            logger.debug(
-                f"[{dep_info.name}] did not find dependency in distlib.database"
-            )
-            return False
+                    import_names_found = []
+                    for line in lines:
+                        candidate, _hash, _size = line.split(",")
+                        if candidate.endswith(".py") and "__init__" in candidate:
+                            import_name = candidate.split(os.sep)[0]
+                            if import_name not in import_names_found:
+                                import_names_found.append(import_name)
+
+                            dep_info.record_import_names = import_names_found
+
+                            import_names = ",".join(dep_info.record_import_names)
+                            logger.debug(
+                                f"[{dep_info.name}] found import name "
+                                f"via RECORD: {import_names} ⭐️"
+                            )
+                            return True
 
-        for filename, _, _ in dist.list_installed_files():  # TODO: #125
-            if filename.endswith((".py")):
-                parts = os.path.splitext(filename)[0].split(os.sep)
-                if len(parts) == 1:  # windows sep varies with distribution type
-                    parts = os.path.splitext(filename)[0].split("/")
-                if parts[-1].startswith("_") and not parts[-1].startswith("__"):
-                    continue  # ignore internals
-                elif filename.endswith(".py") and parts[-1] == "__init__":
-                    found_module_name = parts[-2]
-                    break
-
-        if found_module_name:
-            logger.debug(
-                f"[{dep_info.name}] found import name "
-                f"via distlib.database: {found_module_name} 🤞"
-            )
-            dep_info.distlib_db_import_name = found_module_name
-            return True
+        logger.debug(f"[{dep_info.name}] did not find RECORD in venv")
         return False
 
     def map_dep_to_canonical_name(self, dep_info: DependencyInfo) -> str:
         return self.canonicalize_module_name(dep_info.name)
 
-    def gather_import_info(self):
+    def populate_dependency_info(self):
         """Populate DependencyInfo object with import naming info.
 
         There are three strategies from where the import name can be
         found:
             1. In the top_level.txt file in the venv.
-            2. From the distlib database.
+            2. From the RECORD file in the venv.
             3. Guess the import name by canonicalizing the dep name.
 
         Later, these gathered import names will be compared against the
         imports found in the source code by the AST parser.
         """
         logger.debug("Attempting to find import names...")
-        found_import_name = False
 
         for dep_info in self.dependencies:
-            # best chance to get the import name
-            found_import_name = self.map_dep_to_import_via_top_level_txt_file(dep_info)
+            # find the import name in the top_level.txt file
+            found_via_top_level_txt = self.map_dep_to_import_via_top_level_txt_file(
+                dep_info
+            )
 
-            if not found_import_name:
-                # fallback to distlib
-                found_import_name = self.map_dep_to_module_via_distlib(dep_info)
+            # find the import name in the RECORD file
+            found_via_record = self.map_dep_to_import_via_record_file(dep_info)
 
             # this is really just guessing, but it's better than nothing
             dep_info.canonicalized_dep_name = self.map_dep_to_canonical_name(dep_info)
 
-            if not found_import_name:
+            if not found_via_top_level_txt and not found_via_record:
                 logger.debug(
                     f"[{dep_info.name}] relying on canonicalization "
                     f"fallback: {dep_info.canonicalized_dep_name } 🤞"
                 )
 
     def associate_dep_with_import(self, dep_info: DependencyInfo, import_name: str):
         for imp in self.imports.copy():
@@ -172,47 +170,54 @@
                 # import <imp.name>
                 dep_info.associated_imports.append(imp)
 
             elif imp.name and import_name in imp.module:
                 # from <imp.name> import ...
                 dep_info.associated_imports.append(imp)
 
-    def associate_dep_info_with_imports(self):
+    def resolve(self):
         """Associate dependency name with import (module) name.
 
         The AST has found imports from the source code. This function
         will now attempt to associate these imports with the
-        DependencyInfo data, gathered from the venv, distlib, or
-        canonicalization.
+        DependencyInfo data, gathered from the venv's top_level.txt,
+        the RECORD and a best-guess.
         """
         for dep_info in self.dependencies:
             if dep_info.top_level_import_names:
                 for top_level_import_name in dep_info.top_level_import_names:
                     self.associate_dep_with_import(dep_info, top_level_import_name)
-            elif dep_info.distlib_db_import_name:
-                self.associate_dep_with_import(
-                    dep_info, dep_info.distlib_db_import_name
-                )
-            elif dep_info.canonicalized_dep_name:
+            if dep_info.record_import_names:
+                for record_import_name in dep_info.record_import_names:
+                    self.associate_dep_with_import(dep_info, record_import_name)
+            if dep_info.canonicalized_dep_name:
                 self.associate_dep_with_import(
                     dep_info, dep_info.canonicalized_dep_name
                 )
 
     def get_unused_dependencies(self) -> None:
         self.unused_deps = [
             dep_info
             for dep_info in self.dependencies
             if not dep_info.associated_imports
         ]
 
     def resolve_unused_dependency_names(self) -> List[str]:
         for venv in self.venvs:
+            if not Path(venv).exists():
+                logger.warning(
+                    f"Virtual environment(s) '{', '.join(self.venvs)}' does not exist, "
+                    "cannot resolve top-level names. "
+                    "This may lead to incorrect results."
+                )
             self.gather_top_level_filepaths(venv=venv)
-        self.gather_import_info()
-        self.associate_dep_info_with_imports()
+            self.gather_record_filepaths(venv=venv)
+
+        self.populate_dependency_info()
+        self.resolve()
         self.get_unused_dependencies()
 
         logger.debug(
             "Dependencies with populated 'associated_import' attribute are used in "
             "code. End result of resolve:"
         )
         for dep_info in self.dependencies:
```

## Comparing `creosote-2.5.0.dist-info/METADATA` & `creosote-2.6.0rc1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creosote
-Version: 2.5.0
+Version: 2.6.0rc1
 Summary: Identify unused dependencies and avoid a bloated virtual environment.
 Project-URL: Source, https://github.com/fredrikaverpil/creosote
 Project-URL: Tracker, https://github.com/fredrikaverpil/creosote/issues
 Author-email: Fredrik Averpil <fredrik.averpil@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -13,25 +13,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Requires-Dist: distlib<0.4,>=0.3.4
 Requires-Dist: dotty-dict<1.4,>=1.3.1
 Requires-Dist: loguru<0.7,>=0.6.0
 Requires-Dist: pip-requirements-parser<33.1,>=32.0.1
 Requires-Dist: toml<0.11,>=0.10.2
 Provides-Extra: dev
 Requires-Dist: creosote[lint,test,types]; extra == 'dev'
 Provides-Extra: lint
 Requires-Dist: black; extra == 'lint'
 Requires-Dist: ruff; extra == 'lint'
 Provides-Extra: test
+Requires-Dist: coverage; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-mock; extra == 'test'
 Provides-Extra: types
 Requires-Dist: loguru-mypy; extra == 'types'
 Requires-Dist: mypy; extra == 'types'
 Requires-Dist: types-toml; extra == 'types'
 Description-Content-Type: text/markdown
@@ -47,29 +47,29 @@
 
 Install creosote in separate virtual environment (using e.g. [`pipx`](https://github.com/pypa/pipx)):
 
 ```bash
 pipx install creosote
 ```
 
-Scan virtual environment for unused dependencies ([PEP-621](https://peps.python.org/pep-0621/) example below, but [Poetry](https://python-poetry.org/), [Pipenv](https://github.com/pypa/pipenv) and `requirements.txt` files are also supported, [see this table](#which-dependency-specification-toolingstandards-are-supported)):
+Scan virtual environment for unused dependencies ([PEP-621](https://peps.python.org/pep-0621/) example below, but [Poetry](https://python-poetry.org/), [Pipenv](https://github.com/pypa/pipenv), [PDM](https://pdm.fming.dev/latest/) and `requirements.txt` files are also supported, [see this table](#which-dependency-specification-toolingstandards-are-supported)):
 
 
 ```
 $ creosote
-Found dependencies in pyproject.toml: distlib, dotty-dict, loguru, pip-requirements-parser, requests, toml
+Found dependencies in pyproject.toml: dotty-dict, loguru, pip-requirements-parser, requests, toml
 Oh no, bloated venv! 🤢 🪣
 Unused dependencies found: requests
 ```
 
 And after having removed/uninstalled `requests`:
 
 ```
 $ creosote
-Found dependencies in pyproject.toml: distlib, dotty-dict, loguru, pip-requirements-parser, toml
+Found dependencies in pyproject.toml: dotty-dict, loguru, pip-requirements-parser, toml
 No unused dependencies found! ✨
 ```
 
 Get help:
 
 ```bash
 creosote --help
@@ -77,50 +77,42 @@
 
 ## 🤔 How this works
 
 ### ☘️ Required arguments
 
 | Argument      | Default value          | Description                                                                                            |
 | ------------- | ---------------------- | ------------------------------------------------------------------------------------------------------ |
-| `--venv`      | `.venv`                | The path to your virtual environment.                                                                  |
+| `--venv`      | `.venv`                | The path to your virtual environment or site-packages folder.                                          |
 | `--paths`     | `src`                  | The path to your source code, one or more files/folders.                                               |
 | `--deps-file` | `pyproject.toml`       | The path to the file specifying your dependencies, like `pyproject.toml`, `requirements_*.txt \| .in`. |
 | `--sections`  | `project.dependencies` | One or more toml sections to parse, e.g. `project.dependencies`.                                       |
 
 
 The creosote tool will first scan the given python file(s) for all its imports. Then it fetches all dependency names (from the dependencies spec file). Finally, all imports are associated with their corresponding dependency name (requires the virtual environment for resolving). If a dependency does not have any imports associated, it is considered unused.
 
 See the `main` function in [`cli.py`](https://github.com/fredrikaverpil/creosote/blob/main/src/creosote/cli.py) for a terse overview of the logic.
 
 ### 🌶️ Features
 
-These optional features enable new/experimental functionality, that may be backward incompatible and may be removed at any time. Use at your own risk!
+These optional features enable new/experimental functionality, that may be backward incompatible and may be removed/changed at any time. Some features may become mandatory for a target release version e.g. the next major release. Enable using `--use-feature <FEATURE>`. Use at your own risk!
 
-| Feature                           | Description                                                                                                                                                                                                                                                                                                                                                                          |
-| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
-| `fail-excluded-and-not-installed` | When excluding a dependency from the scan (using `--exclude-deps`) and if the dependency is removed from the dependency specification file (e.g. `pyproject.toml`), return with exit code 1.                                                                                                                                                                                         |
-| `v3-args`                         | Use the new arguments, which will be used in creosote version 3.0.0. In version 2.x, the argument is specified once and then space-separated values, like `-p <path1> <path2>`. This will change in version 3.0.0, where you will have to define the argument for each value, like `-p <path1> -p <path2>`. I believe this is more common and caters better for different use cases. |
+| Feature                           | Description                                                                                                                                                                                                                                                                                                                          | Target version |
+| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------- |
+| `fail-excluded-and-not-installed` | When excluding a dependency from the scan (using `--exclude-deps`) and if the dependency is removed from the dependency specification file (e.g. `pyproject.toml`), return with exit code 1.                                                                                                                                         | N/A            |
+| `v3-args`                         | In version 2.x, some arguments are specified once and then takes space-separated values, like `-p <path1> <path2>`. This is proposed to change with version 3.0.0, where you will have to define the argument for each value, like `-p <path1> -p <path2>`. I believe this is more common and caters better for different use cases. | 3.0.0          |
 
 ### 😤 Known limitations
 
 - `importlib` imports are not detected by the AST parser (a great first contribution for anyone inclined 😄, reach out or start [here](https://github.com/fredrikaverpil/creosote/blob/72d4ce0a8a983725a704decce9083702aa2312cc/src/creosote/parsers.py#L138-L156)).
 
 ## 🥧 History and ambition
 
-The idea of a project like this was hatched from having security vulnerability
-reports about production dependencies (shipped into production) which turned out to not not
-even be in use.
+This project was inspired by security vulnerability reports about production dependencies that were shipped into production but turned out to be unused. Creosote aims to help prevent such occurrences and reduce noise from bots like [Dependabot](https://github.com/dependabot) or [Renovate](https://github.com/renovatebot/renovate) for simply unused dependencies.
 
-This can also help avoiding noise from bots like [Dependabot](https://github.com/dependabot) or [Renovate](https://github.com/renovatebot/renovate)
-for dependencies you don't even need.
-
-The goal of this project is to run the `creosote` tool in CI, which will catch cases where the developer
-forgets to remove unused dependencies. An example of such a case could be when doing refactorings.
-
-Note: Creosote supports identifying both unused production dependencies and developer dependencies. It all depends on what you would like to achieve.
+The intent is to run Creosote in CI (or with [pre-commit](https://pre-commit.com)) to detect cases where developers forget to remove unused dependencies, especially during refactorings. Creosote can identify both unused production dependencies and developer dependencies, depending on your objectives.
 
 ## 🤨 FAQ
 
 ### Which dependency specification tooling/standards are supported?
 
 | Tool/standard                                                                                                               | Supported | `--deps-file` value | Example `--sections` values                                                                                         |
 | --------------------------------------------------------------------------------------------------------------------------- | :-------: | ------------------- | ------------------------------------------------------------------------------------------------------------------- |
@@ -146,15 +138,15 @@
 ### Can I exclude dependencies from the scan?
 
 Yes, you can use the `--exclude-deps` argument to specify one or more dependencies you do not wish to get warnings for.
 
 This feature is intended for dependencies you must specify in your dependencies spec file, but which you don't import in your source code. An example of such a dependency are database drivers, which are commonly only defined in connection strings and will signal to the ORM which driver to use.
 
 ```bash
-$ creosote --exclude-deps pyodbc starlette
+$ creosote --exclude-deps pyodbc pg8000
 ```
 
 ### Can I run Creosote in a GitHub Action workflow?
 
 Yes, please see the `action` job example in [`.github/workflows/test.yml`](https://github.com/fredrikaverpil/creosote/blob/main/.github/workflows/test.yml).
 
 ### Can I run Creosote with [pre-commit](https://pre-commit.com)?
```

## Comparing `creosote-2.5.0.dist-info/licenses/LICENSE` & `creosote-2.6.0rc1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

