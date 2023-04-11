# Comparing `tmp/xpypact-0.2.1.tar.gz` & `tmp/xpypact-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpypact-0.2.1.tar", max compression
+gzip compressed data, was "xpypact-0.3.0.tar", max compression
```

## Comparing `xpypact-0.2.1.tar` & `xpypact-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2023-04-03 06:46:35.689982 xpypact-0.2.1/LICENSE
--rw-r--r--   0        0        0     3201 2023-04-03 06:46:35.689982 xpypact-0.2.1/README.rst
--rw-r--r--   0        0        0    14963 2023-04-03 06:46:49.409964 xpypact-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1199 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/__init__.py
--rw-r--r--   0        0        0      174 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/dao/__init__.py
--rw-r--r--   0        0        0     2110 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/dao/api.py
--rw-r--r--   0        0        0      136 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/dao/duckdb/__init__.py
--rw-r--r--   0        0        0     2868 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/dao/duckdb/create_schema.sql
--rw-r--r--   0        0        0     5637 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/dao/duckdb/implementation.py
--rw-r--r--   0        0        0    14157 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/data_arrays.py
--rw-r--r--   0        0        0     5307 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/data_frames.py
--rw-r--r--   0        0        0    12337 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/fluxes.py
--rw-r--r--   0        0        0     5863 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/inventory.py
--rw-r--r--   0        0        0     1965 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/nuclide.py
--rw-r--r--   0        0        0        0 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/py.typed
--rw-r--r--   0        0        0      515 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/run_data.py
--rw-r--r--   0        0        0     4924 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/time_step.py
--rw-r--r--   0        0        0       29 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/utils/__init__.py
--rw-r--r--   0        0        0      809 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/utils/io.py
--rw-r--r--   0        0        0        0 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/utils/py.typed
--rw-r--r--   0        0        0      768 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/utils/resource.py
--rw-r--r--   0        0        0      270 2023-04-03 06:46:35.693982 xpypact-0.2.1/src/xpypact/utils/types.py
--rw-r--r--   0        0        0     4679 1970-01-01 00:00:00.000000 xpypact-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-11 10:08:01.831799 xpypact-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3296 2023-04-11 10:08:01.831799 xpypact-0.3.0/README.rst
+-rw-r--r--   0        0        0    17326 2023-04-11 10:08:14.379796 xpypact-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1199 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/__init__.py
+-rw-r--r--   0        0        0      174 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/dao/__init__.py
+-rw-r--r--   0        0        0     2241 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/dao/api.py
+-rw-r--r--   0        0        0      168 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/dao/duckdb/__init__.py
+-rw-r--r--   0        0        0     2870 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/dao/duckdb/create_schema.sql
+-rw-r--r--   0        0        0     7790 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/dao/duckdb/implementation.py
+-rw-r--r--   0        0        0    14156 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/data_arrays.py
+-rw-r--r--   0        0        0     5307 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/data_frames.py
+-rw-r--r--   0        0        0    12337 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/fluxes.py
+-rw-r--r--   0        0        0     5862 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/inventory.py
+-rw-r--r--   0        0        0     1965 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/nuclide.py
+-rw-r--r--   0        0        0        0 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/py.typed
+-rw-r--r--   0        0        0      515 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/run_data.py
+-rw-r--r--   0        0        0     4924 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/time_step.py
+-rw-r--r--   0        0        0       29 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/utils/__init__.py
+-rw-r--r--   0        0        0      809 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/utils/io.py
+-rw-r--r--   0        0        0        0 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/utils/py.typed
+-rw-r--r--   0        0        0      768 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/utils/resource.py
+-rw-r--r--   0        0        0      270 2023-04-11 10:08:01.839799 xpypact-0.3.0/src/xpypact/utils/types.py
+-rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 xpypact-0.3.0/PKG-INFO
```

### Comparing `xpypact-0.2.1/LICENSE` & `xpypact-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xpypact-0.2.1/README.rst` & `xpypact-0.3.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 
 Description
 -----------
 
 The module loads FISPACT JSON output as xarray dataset.
 This allows efficient data extraction and aggregation.
 
+Implemented functionality
+-------------------------
+
+- export to DuckDB
+- export to parquet files
+
 .. configures and runs FISPACT, converts FISPACT output to xarray datasets.
 
 .. note::
 
     Currently available FISPACT v.5 API uses rather old python version (3.6).
     That prevents direct use of their API in our package (>=3.8).
     Check if own python integration with FISPACT is reasonable and feasible.
@@ -71,17 +77,17 @@
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
    :target: https://pycqa.github.io/isort/
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
-.. image:: https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black
-   :target: https://github.com/guilatrova/tryceratops
-   :alt: try/except style: tryceratops
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+   :target: https://github.com/charliermarsh/ruff
+   :alt: linter
 
 Just follow ordinary practice:
 
     - `Commit message <https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines>`_
     - `Conventional commits <https://www.conventionalcommits.org/en/v1.0.0/#summary>`_
```

### Comparing `xpypact-0.2.1/pyproject.toml` & `xpypact-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "xpypact"
-version = "0.2.1"
+version = "0.3.0"
 description = "\"Python tools to work with elements and isotopes\""
 authors = ["dvp <dmitri_portnov@yahoo.com>"]
 license = "MIT"
 homepage = "https://github.com/MC-kit/xpypact"
 repository = "https://github.com/MC-kit/xpypact"
 documentation = "https://xpypact.readthedocs.io"
 keywords = [
     "element",
     "nuclide",
     "isotope",
     "abundance",
     "FISPACT",
-    "activation"
+    "activation",
+    "duckdb",
+    "parquet"
 ]
 readme = "README.rst"
 packages = [
     { include = "xpypact", from = "src" },
 ]
 # Select from PyPI classifiers: https://pypi.org/classifiers/
 classifiers = [
@@ -46,15 +48,15 @@
 python = ">=3.8.1,<4.0"
 duckdb = ">=0.7.1"
 h5netcdf = ">=0.13.1"
 mckit-nuclides = {version = ">=0.1.1", allow-prereleases = true}
 numpy = ">=1.24.2"
 openpyxl = ">=3.0.9"
 orjson = ">=3.6.7"
-pandas = ">=1.4.1"
+pandas = ">=2.0.0"
 xarray = ">=2022.3.0"
 multipledispatch = ">=0.6.0"
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 nox = ">=2022.1.7"
 tomli = { version = ">=2.0.1", python="<3.11" }
@@ -62,48 +64,47 @@
 #[tool.poetry.group.profile]
 #optional = true
 
 #[tool.poetry.group.profile.dependencies]
 # TODO dvp: apply yappi: https://coderzcolumn.com/tutorials/python/yappi-yet-another-python-profiler
 #yappi = ">=1.3.2"
 
-[tool.poetry.group.safety.dependencies]
-safety = ">=2.3.5"
-
 [tool.poetry.group.pre_commit.dependencies]
 pre-commit = ">=2.15.0"
 rstcheck = ">=3.3.1"
 pydocstringformatter = "^0.7.3"
 
 [tool.poetry.group.black.dependencies]
 black = ">=22.8.0"  #TODO dvp: update with safety and packaging
 
 [tool.poetry.group.isort.dependencies]
 isort = ">=5.9.3"
 pycln = {version = "^2.1.1", extras = ["click"]}
 
 [tool.poetry.group.test.dependencies]
-pytest = ">=7.0.1"
+pytest = ">=7.1"
 pytest-cache = ">=1.0"
-pytest-cov = ">=3.0.0"
-pytest-mock = ">=3.6.1"
+pytest-cov = ">=4.0"
+pytest-mock = ">=3.9"
+pytest-randomly = ">=3.12"
 coverage = { version = ">=6.1.2", extras = ["toml"] }
 pytest-benchmark = "^4.0.0"
 
 [tool.poetry.group.coverage.dependencies]
 coverage = { version = ">=6.1.2", extras = ["toml"] }
 
 [tool.poetry.group.xdoctest.dependencies]
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 
 [tool.poetry.group.typeguard.dependencies]
-typeguard = ">=2.13.0"
+typeguard = ">=2.13.3"
+# typeguard = ">=3.0.2"  - pygls, which is required by ruff-lsp, doesn't allow newer version
 
 [tool.poetry.group.mypy.dependencies]
-mypy = ">=0.931"
+mypy = ">=1.2.0"
 pep8-naming = ">=0.12.1"
 types-setuptools = ">=57.4.2"
 numpy = ">=1.23.2"
 
 [tool.poetry.group.flake8.dependencies]
 darglint = ">=1.8.1"
 flake8 = ">=6.0.0"
@@ -153,14 +154,27 @@
 pyls-memestra = ">=0.0.16"
 pylsp-rope = ">=0.1.11"
 ruff-lsp = "^0.0.24"
 
 [tool.poetry.group.ruff.dependencies]
 ruff = ">=0.0.259"
 
+
+[tool.poetry.group.adhoc]
+optional = true
+
+[tool.poetry.group.adhoc.dependencies]
+pyarrow = "^11.0.0"
+
+[tool.poetry.group.analysis]
+optional = true
+
+[tool.poetry.group.analysis.dependencies]
+jupyterlab = "^3.6.3"  # don't use >= - installs development version 4.0...
+
 [tool.isort]
 atomic = true
 ensure_newline_before_comments = true
 known_first_party = "src"
 known_third_party = "mpl_toolkits,matplotlib,numpy,scipy"
 known_typing = "typing,types,typing_extensions,mypy,mypy_extensions"
 sections = "FUTURE,TYPING,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
@@ -222,15 +236,16 @@
 # xfail tests that pass should fail the test suite
 xfail_strict = true
 filterwarnings = [
     "error",
     'ignore:Implementing implicit namespace packages \(as specified in PEP 420\) is preferred to `pkg_resources.declare_namespace`',
     "ignore:.*not typechecking multipledispatch.dispatcher.*UserWarning",
     'ignore:.*io.FileIO \[closed\]',
-    'ignore:.*Deprecated call to `pkg_resources.declare_namespace'
+    'ignore:.*Deprecated call to `pkg_resources.declare_namespace',
+    'ignore:.*DeprecationWarning.*Implicit None on return values'
 ]
 log_format = "%(asctime)s %(levelname)s %(message)s"
 log_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.xdoctest]
 quiet = true
 options = ""
@@ -268,14 +283,15 @@
 sort = "Cover"
 
 
 # MyPy config
 # See https://mypy.readthedocs.io/en/stable/config_file.html#using-a-pyproject-toml-file
 #     https://dev.to/tusharsadhwani/the-comprehensive-guide-to-mypy-561m
 [tool.mypy]
+python_version = "3.11"
 # strict = true     # TODO dvp: uncomment this to get strict control
 follow_imports = "silent"
 # namespace_packages = true
 warn_return_any = true
 warn_unused_configs = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
@@ -299,16 +315,16 @@
     "multipledispatch",
     "nox",
     "numpy.testing",
     "orjson",
     "pandas",
     "pytest",
     "scipy.constants",
-    "tomllib",
     "tomli",
+    "tomllib",
     "xarray.*"
 ]
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = [
     "tomllib",
@@ -375,14 +391,15 @@
 good-names-rgxs=["."]  # a single character variable is okay
 logging-format-style="new"   # use {} in logging messages
 deprecated-modules=["six"]
 
 [tool.ruff]
 target-version = "py38"
 #see full list: https://beta.ruff.rs/docs/rules/#pyflakes-f
+#or run 'ruff linter' to see a brief list
 select= [
     "A", # flake8-builtins
     "ANN", # flake8-annotations
     "ARG", # flake8-unused-arguments
     "B", # flake8-bugbear
     "BLE", # flake8-blind-except
     "C4", # flake8-comprehensions
@@ -430,20 +447,36 @@
 
 # Ignore rules that currently fail on the codebase
 ignore = [
     "ANN001", # ANN001 Missing type annotation for function argument: doesn't allow to use functools dispatching
     "ANN002", # ANN002 Missing type annotation for *drop_items: ... as above
     "ANN101", # ANN101 Missing type annotation for self in method
     "ANN102", # ANN102 Missing type annotation for cls in classmethod
+    # "ANN201", # Missing return type annotation for public function `mesh2com`
     "ANN202", # ANN202 Missing return type annotation for protected function: ... dispatching
     "ANN204", # ANN204 Missing return type annotation for special method
+
+    # "ARG001", # Unused function argument: `expected`
+
     "B905",   # B905 `zip()` without an explicit `strict=` parameter - ignore while support 3.8, 3.9
+
     # "C812",   # C812 Missing trailing comma: black compatibility
+    # "C901",   # too complex - ...
+
+    # "D100",   # Missing docstring in public module
+    # "D101",   # Missing docstring in public class
+    # "D102",   # Missing docstring in public method
+    # "D103",   # Missing docstring in public function
     "D105",   # D105 Missing docstring in magic method (__hash__, __eq__)
+    # "D104",   # Missing docstring in public package
+    # "D106",   # Missing docstring in public nested class
     "D107",   # Missing docstring in __init__
+    # "D417",   # Missing argument descriptions in the docstring: `config`, `ebins`, - TODO
+
+
     # "E203",   # E203: Whitespace before ‘:'
     # "E401",  # Multiple imports on one line
     # "E402",  # Module level import not at top of file
     # "E501",  # Line too long (<LENGTH> > 100 characters)
     # "E701",  # Multiple statements on one line (colon)
     # "E702",  # Multiple statements on one line (semicolon)
     # "E703",  # Statement ends with an unnecessary semicolon
@@ -453,35 +486,65 @@
     # "E713",  # Test for membership should be `not in`
     # "E714",  # Test for object identity should be `is not`
     # "E721",  # Do not compare types, use `isinstance()`
     # "E722",  # Do not use bare `except`
     # "E731",  # Do not assign a `lambda` expression, use a `def`
     # "E741",  # Ambiguous variable name: `<VARIABLE>`
     # "E743",  # Ambiguous function name: `<FUNCTION>`
+
+    # "EM101",   # Exception must not use a string literal, assign to variable first
+    # "EM102",   # Exception must not use an f-string literal, assign to variable first
+
+    # "N803",    # Argument name `R` should be lowercase
+    # "N806",    # Variable `D` in function should be lowercase
+
     # "F401",  # `<TYPE>` imported but unused
     # "F403",  # `from <MODULE> import *` used; unable to detect undefined names
     # "F405",  # `<TYPE>` may be undefined, or defined from star imports: `<MODULE>`
     # "F523",  # `.format` call has unused arguments at position(s): <INDEX>
     # "F601",  # Dictionary key literal `'<KEY>'` repeated
     # "F811",  # Redefinition of unused `<VARIABLE>` from line <LINE>
     # "F821",  # Undefined name `VARIABLE`
     # "F823",  # Local variable `VARIABLE` referenced before assignment
     # "F841",  # Local variable `VARIABLE` is assigned to but never used
 
-    "I001",  # import order is controlled by isort
+    # "FBT001",  # Boolean positional arg in function definition (TODO!)
+    # "FBT002",  # Boolean default value in function definition (TODO!)
+    # "FBT003",  # Boolean positional value in function call
+
+    "I001",    # import order is controlled by isort
     # "I101",
     # "I201",
     # "I202",
+    # "INP001",  # File `tools/clear-prev-dist-info.py` is part of an implicit namespace package.
 
 # ignore some questionable pandas-vet warnings
     # "PD005", # use operator instead of method
     # "PD008", # We use at() to access single values
     # "PD009", # And we use iat()
+
+    "PLE1205", # logging-too-many-args - with use logure with '{' style of placeholders
+
+    # "PLR0912", # Too many branches (15 > 12)
+    # "PLR0913", # Too many arguments to function call (6 > 5)
+    # "PLR0915", # Too many statements (65 > 50)
+    "PLR2004", # magic number - don't want declare 0.0 as constant
+    # "PLR5501", # Consider using `elif` instead of `else` then `if` to remove one indentation level
+
     "PT019",   # Fixture `_bin` without value is injected as parameter (false positive?)
 
+    # "S101",    # Use of `assert` detected
+    # "S301",    # `pickle` and modules that wrap... - TODO - use sql instead of pickle
+
+    # "SLF001",  # Private member accessed: `_geometry_spec`
+
+    # "TCH001",  # Move application import `mckit.utils.named` into a type-checking block
+
+    # "TRY003",  #  Avoid specifying long messages outside the exception class
+
     # "W503",  # Line break before binary operator: for compatibility with black settings
 ]
 
 # Same as Black.
 line-length = 100
 
 # show an enumeration of all autofixed lint violations
@@ -512,18 +575,15 @@
 "src/xpypact/fluxes.py" = ["F811"]
 "benchmarks/*" = ["S101"]
 "noxfile.py" = ["ANN"]
 "tests/*" = ["ANN", "D100", "D101", "D102", "D103", "D104",  "PLR2004", "S101"]
 "src/xpypact/inventory.py" = ["F811"]
 "src/xpypact/data_arrays.py" = ["ANN401", "PD011"]
 "src/xpypact/utils/resource.py" = ["ANN202"]
-"tools/*" = [
-    "T201",
-    "INP001",  # file ... is part of implicit namespace ... add __init__.py - there are no modules in tools
-]
+"tools/*" = ["T201", "INP001"]
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.ruff.flake8-type-checking]
 strict = true
```

### Comparing `xpypact-0.2.1/src/xpypact/__init__.py` & `xpypact-0.3.0/src/xpypact/__init__.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.2.1/src/xpypact/dao/api.py` & `xpypact-0.3.0/src/xpypact/dao/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,29 +7,31 @@
 
 if TYPE_CHECKING:
     import pandas as pd
     import xarray as xr
 
 
 class DataAccessInterface(ABC):
-    """Abstract DAO."""
+    """Abstract DAO for to save/load xpypact dataset.
 
-    @abstractmethod
-    def __enter__(self):
-        """Use DAO as context manager."""
+    The subclasses implement methods to save/load xpypact dataset to/from
+    database or filesystem.
 
-    @abstractmethod
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        """Use DAO as context manager."""
+    A caller is to provide connection or whatever resource to subclasses.
+    """
 
     @abstractmethod
     def get_tables_info(self) -> pd.DataFrame:
         """Get information on tables in schema."""
 
     @abstractmethod
+    def has_schema(self) -> bool:
+        """Check if the schema is available in a database."""
+
+    @abstractmethod
     def create_schema(self) -> None:
         """Create tables to store xpypact dataset.
 
         Retain existing tables.
         """
 
     @abstractmethod
```

### Comparing `xpypact-0.2.1/src/xpypact/dao/duckdb/create_schema.sql` & `xpypact-0.3.0/src/xpypact/dao/duckdb/create_schema.sql`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 CREATE TABLE IF NOT EXISTS rundata (
     material_id uinteger not null,
-    case_id varchar not null,
+    case_id     uinteger not null,
     timestamp timestamp not null,
     run_name varchar not null,
     flux_name varchar NOT NULL,
     dose_rate_type varchar NOT NULL,
     dose_rate_distance real NOT NULL,
     primary key(material_id, case_id)
 );
 
 CREATE TABLE IF NOT EXISTS timestep(
-    material_id  uinteger not null,
-    case_id      varchar not null,
+    material_id uinteger not null,
+    case_id     uinteger not null,
     time_step_number uinteger not null,
     elapsed_time float4 not null,
     irradiation_time float4 not null,
     cooling_time float4 not null,
     duration float4 not null,
     flux float4 not null,
     atoms float4 not null,
@@ -42,16 +42,16 @@
     state varchar(1) not null,
     zai integer not null check(10010 <= zai) unique,
     half_life float4 not null check(0 <= half_life),
     primary key(element, mass_number, state)
 );
 
 CREATE TABLE IF NOT EXISTS timestep_nuclide(
-    material_id  uinteger not null,
-    case_id      varchar not null,
+    material_id uinteger not null,
+    case_id     uinteger not null,
     time_step_number uinteger not null,
     element varchar(2) not null,
     mass_number usmallint not null,
 
     state varchar(1) not null,
     atoms float4 not null,
     grams float4 not null,
@@ -71,15 +71,15 @@
 
     primary key(material_id, case_id, time_step_number, element, mass_number, state),
     foreign key(material_id, case_id, time_step_number) references timestep(material_id, case_id, time_step_number),
     foreign key(element, mass_number, state) references nuclide(element, mass_number, state)
 );
 
 CREATE TABLE IF NOT EXISTS timestep_gamma(
-    material_id  uinteger not null,
-    case_id      varchar not null,
+    material_id uinteger not null,
+    case_id     uinteger not null,
     time_step_number uinteger not null,
     boundary real not null check(0 <= boundary),
     rate real not null,
     primary key(material_id, case_id, time_step_number, boundary),
     foreign key(material_id, case_id, time_step_number) references timestep(material_id, case_id, time_step_number),
 );
```

### Comparing `xpypact-0.2.1/src/xpypact/data_arrays.py` & `xpypact-0.3.0/src/xpypact/data_arrays.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     dtype=float,
 ) -> tuple[tuple[str, str], ArrayLike]:
     _data = np.fromiter(map(getter, nuclides), dtype=dtype)
     return ("time_step_number", "nuclide"), _data.reshape(1, _data.size)
 
 
 def _add_time_step_record(_ds: xr.Dataset, ts: TimeStep) -> xr.Dataset:
-
     data_vars = {
         "irradiation_time": _make_var(ts.irradiation_time),
         "cooling_time": _make_var(ts.cooling_time),
         "duration": _make_var(ts.duration),
         "flux": _make_var(ts.flux),
         "total_atoms": _make_var(ts.total_atoms),
         "total_activity": _make_var(ts.total_activity),
```

### Comparing `xpypact-0.2.1/src/xpypact/data_frames.py` & `xpypact-0.3.0/src/xpypact/data_frames.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.2.1/src/xpypact/fluxes.py` & `xpypact-0.3.0/src/xpypact/fluxes.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.2.1/src/xpypact/inventory.py` & `xpypact-0.3.0/src/xpypact/inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 import orjson as json
 
 from xpypact.run_data import RunData
 from xpypact.time_step import TimeStep
 
 if TYPE_CHECKING:
-
     from collections.abc import Callable, Iterable
 
     from xpypact.utils.types import NDArrayFloat
 
 FLOAT_ZERO = 0.0
```

### Comparing `xpypact-0.2.1/src/xpypact/nuclide.py` & `xpypact-0.3.0/src/xpypact/nuclide.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.2.1/src/xpypact/run_data.py` & `xpypact-0.3.0/src/xpypact/run_data.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.2.1/src/xpypact/time_step.py` & `xpypact-0.3.0/src/xpypact/time_step.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.2.1/src/xpypact/utils/io.py` & `xpypact-0.3.0/src/xpypact/utils/io.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.2.1/src/xpypact/utils/resource.py` & `xpypact-0.3.0/src/xpypact/utils/resource.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.2.1/PKG-INFO` & `xpypact-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: xpypact
-Version: 0.2.1
+Version: 0.3.0
 Summary: "Python tools to work with elements and isotopes"
 Home-page: https://github.com/MC-kit/xpypact
 License: MIT
-Keywords: element,nuclide,isotope,abundance,FISPACT,activation
+Keywords: element,nuclide,isotope,abundance,FISPACT,activation,duckdb,parquet
 Author: dvp
 Author-email: dmitri_portnov@yahoo.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -23,15 +23,15 @@
 Requires-Dist: duckdb (>=0.7.1)
 Requires-Dist: h5netcdf (>=0.13.1)
 Requires-Dist: mckit-nuclides (>=0.1.1)
 Requires-Dist: multipledispatch (>=0.6.0)
 Requires-Dist: numpy (>=1.24.2)
 Requires-Dist: openpyxl (>=3.0.9)
 Requires-Dist: orjson (>=3.6.7)
-Requires-Dist: pandas (>=1.4.1)
+Requires-Dist: pandas (>=2.0.0)
 Requires-Dist: xarray (>=2022.3.0)
 Project-URL: Changelog, https://github.com/MC-kit/xpypact/releases
 Project-URL: Documentation, https://xpypact.readthedocs.io
 Project-URL: Repository, https://github.com/MC-kit/xpypact
 Project-URL: documentation, https://xpypact.readthedocs.io
 Description-Content-Type: text/x-rst
 
@@ -52,14 +52,20 @@
 
 Description
 -----------
 
 The module loads FISPACT JSON output as xarray dataset.
 This allows efficient data extraction and aggregation.
 
+Implemented functionality
+-------------------------
+
+- export to DuckDB
+- export to parquet files
+
 .. configures and runs FISPACT, converts FISPACT output to xarray datasets.
 
 .. note::
 
     Currently available FISPACT v.5 API uses rather old python version (3.6).
     That prevents direct use of their API in our package (>=3.8).
     Check if own python integration with FISPACT is reasonable and feasible.
@@ -108,17 +114,17 @@
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
    :target: https://pycqa.github.io/isort/
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
-.. image:: https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black
-   :target: https://github.com/guilatrova/tryceratops
-   :alt: try/except style: tryceratops
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+   :target: https://github.com/charliermarsh/ruff
+   :alt: linter
 
 Just follow ordinary practice:
 
     - `Commit message <https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines>`_
     - `Conventional commits <https://www.conventionalcommits.org/en/v1.0.0/#summary>`_
```

