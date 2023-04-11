# Comparing `tmp/arraytex-0.0.6.tar.gz` & `tmp/arraytex-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraytex-0.0.6.tar", max compression
+gzip compressed data, was "arraytex-0.0.7.tar", max compression
```

## Comparing `arraytex-0.0.6.tar` & `arraytex-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-04-08 16:33:14.959418 arraytex-0.0.6/LICENSE
--rw-r--r--   0        0        0     2978 2023-04-08 16:33:14.959418 arraytex-0.0.6/README.md
--rw-r--r--   0        0        0     2398 2023-04-08 16:33:31.887712 arraytex-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      112 2023-04-08 16:33:14.959418 arraytex-0.0.6/src/arraytex/__init__.py
--rw-r--r--   0        0        0      206 2023-04-08 16:33:14.959418 arraytex-0.0.6/src/arraytex/__main__.py
--rw-r--r--   0        0        0     3927 2023-04-08 16:33:31.887712 arraytex-0.0.6/src/arraytex/api.py
--rw-r--r--   0        0        0      243 2023-04-08 16:33:14.959418 arraytex-0.0.6/src/arraytex/errors.py
--rw-r--r--   0        0        0        0 2023-04-08 16:33:14.959418 arraytex-0.0.6/src/arraytex/py.typed
--rw-r--r--   0        0        0     1772 2023-04-08 16:33:14.959418 arraytex-0.0.6/src/arraytex/utils.py
--rw-r--r--   0        0        0     3966 1970-01-01 00:00:00.000000 arraytex-0.0.6/setup.py
--rw-r--r--   0        0        0     3941 1970-01-01 00:00:00.000000 arraytex-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-11 16:41:58.785130 arraytex-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2982 2023-04-11 16:41:58.785130 arraytex-0.0.7/README.md
+-rw-r--r--   0        0        0     2389 2023-04-11 16:42:15.609325 arraytex-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-04-11 16:41:58.789131 arraytex-0.0.7/src/arraytex/__init__.py
+-rw-r--r--   0        0        0      206 2023-04-11 16:41:58.789131 arraytex-0.0.7/src/arraytex/__main__.py
+-rw-r--r--   0        0        0     4983 2023-04-11 16:42:15.609325 arraytex-0.0.7/src/arraytex/api.py
+-rw-r--r--   0        0        0      243 2023-04-11 16:41:58.789131 arraytex-0.0.7/src/arraytex/errors.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:41:58.789131 arraytex-0.0.7/src/arraytex/py.typed
+-rw-r--r--   0        0        0     1772 2023-04-11 16:41:58.789131 arraytex-0.0.7/src/arraytex/utils.py
+-rw-r--r--   0        0        0     3970 1970-01-01 00:00:00.000000 arraytex-0.0.7/setup.py
+-rw-r--r--   0        0        0     3945 1970-01-01 00:00:00.000000 arraytex-0.0.7/PKG-INFO
```

### Comparing `arraytex-0.0.6/LICENSE` & `arraytex-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `arraytex-0.0.6/README.md` & `arraytex-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ```
 
 Inspired by [@josephcslater](https://github.com/josephcslater)'s
 [array_to_latex](https://github.com/josephcslater/array_to_latex).
 
 ## Features
 
-- Support for different matrix environment delimiters (`bmatrix` or `pmatrix`).
+- Support for different matrix environment delimiters, (`bmatrix`, `pmatrix`, etc.)
 - Support for tabular environments.
 - Support for builtin number formats (`:.2f`, `:.3e`, etc.).
 - Fully tested and typed.
 
 ## Requirements
 
 - `python >= 3.8`
```

### Comparing `arraytex-0.0.6/pyproject.toml` & `arraytex-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arraytex"
-version = "0.0.6"
+version = "0.0.7"
 description = "ArrayTeX"
 authors = ["Dom Batten <dominic.batten@googlemail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dbatten5/arraytex"
 repository = "https://github.com/dbatten5/arraytex"
 documentation = "https://arraytex.readthedocs.io"
@@ -102,15 +102,14 @@
   'D413',
   'E501'
 ]
 line-length = 80
 select = [
     'B',
     'B9',
-    'C',
     'D',
     'E',
     'F',
     'N',
     'S',
     'W',
 ]
```

### Comparing `arraytex-0.0.6/src/arraytex/api.py` & `arraytex-0.0.7/src/arraytex/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -54,29 +54,31 @@
 
 @use_clipboard
 def to_tabular(
     arr: NDArray[Any],
     num_format: Optional[str] = None,
     scientific_notation: bool = False,
     col_align: Union[List[str], str] = "c",
-    cols: Optional[List[str]] = None,
+    col_names: Optional[List[str]] = None,
+    col_index: Optional[List[str]] = None,
     to_clp: bool = False,
 ) -> str:
     """Convert a numpy.NDArray to LaTeX tabular environment.
 
     Args:
         arr: the array to be converted
         num_format: a number formatter string, e.g. ".2f"
         scientific_notation: a flag to determine whether 1 x 10^3 should be used,
             otherwise e-notation is used (1e3)
         col_align: set the alignment of the columns, usually "c", "r" or "l". If a
             single character is provided then it will be broadcast to all columns. If a list
             is provided then each item will be assigned to each column, list size and
             number of columns must match
-        cols: an optional list of column names, otherwise generic names will be assigned
+        col_names: an optional list of column names, otherwise generic names will be assigned
+        col_index: an optional list of column indices, i.e. row identifiers
         to_clp: copy the output to the system clipboard
 
     Returns:
         the LaTeX tabular string representation of the array
 
     Raises:
         TooManyDimensionsError: when the supplied array has more than 2 dimensions
@@ -90,36 +92,64 @@
     elif n_dims == 1:
         n_cols = arr.shape[0]
     elif n_dims == 2:
         n_cols = arr.shape[1]
     else:
         raise TooManyDimensionsError
 
-    if isinstance(col_align, list) and len(col_align) != n_cols:
+    if not col_index:
+        if isinstance(col_align, list) and len(col_align) != n_cols:
+            raise DimensionMismatchError(
+                f"Number of `col_align` items ({len(col_align)}) "
+                + f"doesn't match number of columns ({n_cols})"
+            )
+
+        if col_names and len(col_names) != n_cols:
+            raise DimensionMismatchError(
+                f"Number of `col_names` items ({len(col_names)}) "
+                + f"doesn't match number of columns ({n_cols})"
+            )
+
+    if (
+        col_index
+        and col_names
+        and isinstance(col_align, list)
+        and len(col_names) != len(col_align)
+    ):
         raise DimensionMismatchError(
             f"Number of `col_align` items ({len(col_align)}) "
-            + f"doesn't match number of columns ({n_cols})"
+            + f"doesn't match number of columns ({len(col_names)})"
         )
 
     if isinstance(col_align, str):
         col_align = [col_align for _ in range(n_cols)]
 
-    if cols and len(cols) != n_cols:
-        raise DimensionMismatchError(
-            f"Number of `cols` items ({len(cols)}) "
-            + f"doesn't match number of columns ({n_cols})"
-        )
-
-    if not cols:
-        cols = [f"Col {i + 1}" for i in range(n_cols)]
+    if not col_names:
+        col_names = [f"Col {i + 1}" for i in range(n_cols)]
 
     lines = _parse_lines(arr, num_format, scientific_notation)
 
+    if col_index:
+        if len(col_index) != len(lines):
+            raise DimensionMismatchError(
+                f"Number of `col_index` items ({len(col_index)}) "
+                + f"doesn't match number of rows ({len(lines)})"
+            )
+
+        if len(col_align) == n_cols:
+            col_align.insert(0, "l")
+
+        if len(col_names) == n_cols:
+            col_names.insert(0, "Index")
+
+        for idx, line in enumerate(lines):
+            lines[idx] = f"{col_index[idx]} & " + line.strip()
+
     rv = [f"\\begin{{tabular}}{{{' '.join(col_align)}}}"]
     rv += [r"\toprule"]
-    rv += [" & ".join(cols) + r" \\"]
+    rv += [" & ".join(col_names) + r" \\"]
     rv += [r"\midrule"]
     rv += [line.strip() + r" \\" for line in lines]
     rv += [r"\bottomrule"]
     rv += [r"\end{tabular}"]
 
     return "\n".join(rv)
```

### Comparing `arraytex-0.0.6/src/arraytex/utils.py` & `arraytex-0.0.7/src/arraytex/utils.py`

 * *Files identical despite different names*

### Comparing `arraytex-0.0.6/setup.py` & `arraytex-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
  'typing-extensions>=4.5.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['arraytex = arraytex.__main__:main']}
 
 setup_kwargs = {
     'name': 'arraytex',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'ArrayTeX',
-    'long_description': "# ArrayTeX\n\n[![PyPI](https://img.shields.io/pypi/v/arraytex.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/arraytex.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/arraytex)][python version]\n[![License](https://img.shields.io/pypi/l/arraytex)][license]\n\n[![Read the documentation at https://arraytex.readthedocs.io/](https://img.shields.io/readthedocs/arraytex/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/dbatten5/arraytex/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/dbatten5/arraytex/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/arraytex/\n[status]: https://pypi.org/project/arraytex/\n[python version]: https://pypi.org/project/arraytex\n[read the docs]: https://arraytex.readthedocs.io/\n[tests]: https://github.com/dbatten5/arraytex/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/dbatten5/arraytex\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\nConvert a `numpy.NDArray` to various LaTeX forms.\n\n```python\n>>> import numpy as np\n>>> import arraytex as atx\n>>> A = np.array([[1, 2, 3], [4, 5, 6]])\n>>> print(atx.to_matrix(A))\n\\begin{bmatrix}\n1 & 2 & 3 \\\\\n4 & 5 & 6 \\\\\n\\end{bmatrix}\n```\n\nInspired by [@josephcslater](https://github.com/josephcslater)'s\n[array_to_latex](https://github.com/josephcslater/array_to_latex).\n\n## Features\n\n- Support for different matrix environment delimiters (`bmatrix` or `pmatrix`).\n- Support for tabular environments.\n- Support for builtin number formats (`:.2f`, `:.3e`, etc.).\n- Fully tested and typed.\n\n## Requirements\n\n- `python >= 3.8`\n\n## Installation\n\nYou can install _ArrayTeX_ via [pip] from [PyPI]:\n\n```console\n$ pip install arraytex\n```\n\n## Usage\n\nPlease see the [docs](https://arraytex.readthedocs.io/) for more information.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_ArrayTeX_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/dbatten5/arraytex/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/dbatten5/arraytex/blob/main/LICENSE\n[contributor guide]: https://github.com/dbatten5/arraytex/blob/main/CONTRIBUTING.md\n[command-line reference]: https://arraytex.readthedocs.io/en/latest/usage.html\n",
+    'long_description': "# ArrayTeX\n\n[![PyPI](https://img.shields.io/pypi/v/arraytex.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/arraytex.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/arraytex)][python version]\n[![License](https://img.shields.io/pypi/l/arraytex)][license]\n\n[![Read the documentation at https://arraytex.readthedocs.io/](https://img.shields.io/readthedocs/arraytex/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/dbatten5/arraytex/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/dbatten5/arraytex/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/arraytex/\n[status]: https://pypi.org/project/arraytex/\n[python version]: https://pypi.org/project/arraytex\n[read the docs]: https://arraytex.readthedocs.io/\n[tests]: https://github.com/dbatten5/arraytex/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/dbatten5/arraytex\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\nConvert a `numpy.NDArray` to various LaTeX forms.\n\n```python\n>>> import numpy as np\n>>> import arraytex as atx\n>>> A = np.array([[1, 2, 3], [4, 5, 6]])\n>>> print(atx.to_matrix(A))\n\\begin{bmatrix}\n1 & 2 & 3 \\\\\n4 & 5 & 6 \\\\\n\\end{bmatrix}\n```\n\nInspired by [@josephcslater](https://github.com/josephcslater)'s\n[array_to_latex](https://github.com/josephcslater/array_to_latex).\n\n## Features\n\n- Support for different matrix environment delimiters, (`bmatrix`, `pmatrix`, etc.)\n- Support for tabular environments.\n- Support for builtin number formats (`:.2f`, `:.3e`, etc.).\n- Fully tested and typed.\n\n## Requirements\n\n- `python >= 3.8`\n\n## Installation\n\nYou can install _ArrayTeX_ via [pip] from [PyPI]:\n\n```console\n$ pip install arraytex\n```\n\n## Usage\n\nPlease see the [docs](https://arraytex.readthedocs.io/) for more information.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_ArrayTeX_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/dbatten5/arraytex/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/dbatten5/arraytex/blob/main/LICENSE\n[contributor guide]: https://github.com/dbatten5/arraytex/blob/main/CONTRIBUTING.md\n[command-line reference]: https://arraytex.readthedocs.io/en/latest/usage.html\n",
     'author': 'Dom Batten',
     'author_email': 'dominic.batten@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dbatten5/arraytex',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `arraytex-0.0.6/PKG-INFO` & `arraytex-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arraytex
-Version: 0.0.6
+Version: 0.0.7
 Summary: ArrayTeX
 Home-page: https://github.com/dbatten5/arraytex
 License: MIT
 Author: Dom Batten
 Author-email: dominic.batten@googlemail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -60,15 +60,15 @@
 ```
 
 Inspired by [@josephcslater](https://github.com/josephcslater)'s
 [array_to_latex](https://github.com/josephcslater/array_to_latex).
 
 ## Features
 
-- Support for different matrix environment delimiters (`bmatrix` or `pmatrix`).
+- Support for different matrix environment delimiters, (`bmatrix`, `pmatrix`, etc.)
 - Support for tabular environments.
 - Support for builtin number formats (`:.2f`, `:.3e`, etc.).
 - Fully tested and typed.
 
 ## Requirements
 
 - `python >= 3.8`
```

