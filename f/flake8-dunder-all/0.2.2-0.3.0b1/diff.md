# Comparing `tmp/flake8_dunder_all-0.2.2.tar.gz` & `tmp/flake8_dunder_all-0.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_dunder_all-0.2.2.tar", last modified: Mon Aug  1 09:05:20 2022, max compression
+gzip compressed data, was "flake8_dunder_all-0.3.0b1.tar", last modified: Tue Apr 11 13:11:49 2023, max compression
```

## Comparing `flake8_dunder_all-0.2.2.tar` & `flake8_dunder_all-0.3.0b1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0 runner    (1001) docker     (121)     4918 2022-08-01 09:05:20.633737 flake8_dunder_all-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     6450 2022-08-01 09:05:20.637737 flake8_dunder_all-0.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8051 2022-08-01 09:05:20.637737 flake8_dunder_all-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-01 09:05:20.625737 flake8_dunder_all-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-01 09:05:20.637737 flake8_dunder_all-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-01 09:04:37.105467 flake8_dunder_all-0.2.2/flake8_dunder_all/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     8407 2022-08-01 09:04:37.105467 flake8_dunder_all-0.2.2/flake8_dunder_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-08-01 09:04:37.105467 flake8_dunder_all-0.2.2/flake8_dunder_all/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3102 2022-08-01 09:04:37.109467 flake8_dunder_all-0.2.2/flake8_dunder_all/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8059 2023-04-11 13:11:49.717365 flake8_dunder_all-0.3.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4919 2023-04-11 13:11:49.713365 flake8_dunder_all-0.3.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1104 2023-04-11 13:11:49.709365 flake8_dunder_all-0.3.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6456 2023-04-11 13:11:49.717365 flake8_dunder_all-0.3.0b1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-11 13:11:49.717365 flake8_dunder_all-0.3.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8630 2023-04-11 13:11:20.712577 flake8_dunder_all-0.3.0b1/flake8_dunder_all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 13:11:20.712577 flake8_dunder_all-0.3.0b1/flake8_dunder_all/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-04-11 13:11:20.712577 flake8_dunder_all-0.3.0b1/flake8_dunder_all/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3102 2023-04-11 13:11:20.712577 flake8_dunder_all-0.3.0b1/flake8_dunder_all/utils.py
```

### Comparing `flake8_dunder_all-0.2.2/pyproject.toml` & `flake8_dunder_all-0.3.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "flake8-dunder-all"
-version = "0.2.2"
+version = "0.3.0b1"
 description = "A Flake8 plugin and pre-commit hook which checks to ensure modules have defined '__all__'."
 readme = "README.rst"
 keywords = [ "flake8",]
 dynamic = []
 dependencies = [
     "astatine>=0.3.1",
     "click>=7.1.2",
@@ -97,15 +97,15 @@
     "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
     "html_section",
     "sphinx_toolbox.pre_commit",
     "sphinx_toolbox.flake8",
     "sphinx_click",
     "sphinx_toolbox.more_autosummary.column_widths",
-    "sphinx-favicon",
+    "sphinx_favicon",
 ]
 sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
 master_doc = "index"
@@ -164,15 +164,15 @@
 directives = [ "code-block",]
 
 [tool.mkrecipe]
 conda-channels = [ "conda-forge", "domdfcoding",]
 extras = "all"
 
 [project.entry-points."flake8.extension"]
-DALL = "flake8_dunder_all:Plugin"
+DAL = "flake8_dunder_all:Plugin"
 
 [tool.dependency-dash."requirements.txt"]
 order = 10
 
 [tool.dependency-dash."tests/requirements.txt"]
 order = 20
 include = false
```

### Comparing `flake8_dunder_all-0.2.2/README.rst` & `flake8_dunder_all-0.3.0b1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 	:target: https://github.com/python-formate/flake8-dunder-all/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/python-formate/flake8-dunder-all/workflows/mypy/badge.svg
 	:target: https://github.com/python-formate/flake8-dunder-all/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/python-formate/flake8-dunder-all/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/python-formate/flake8-dunder-all/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/python-formate/flake8-dunder-all/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/python-formate/flake8-dunder-all/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/python-formate/flake8-dunder-all/master?logo=coveralls
 	:target: https://coveralls.io/github/python-formate/flake8-dunder-all?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/python-formate/flake8-dunder-all?logo=codefactor
@@ -97,23 +97,23 @@
 .. |license| image:: https://img.shields.io/github/license/python-formate/flake8-dunder-all
 	:target: https://github.com/python-formate/flake8-dunder-all/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/python-formate/flake8-dunder-all
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/python-formate/flake8-dunder-all/v0.2.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/python-formate/flake8-dunder-all/v0.3.0b1
 	:target: https://github.com/python-formate/flake8-dunder-all/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/python-formate/flake8-dunder-all
 	:target: https://github.com/python-formate/flake8-dunder-all/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/flake8-dunder-all
 	:target: https://pypi.org/project/flake8-dunder-all/
 	:alt: PyPI - Downloads
 
 .. end shields
@@ -169,15 +169,15 @@
 
 .. code-block:: yaml
 
 	 - repo: https://gitlab.com/pycqa/flake8
 	   rev: 3.8.1
 	   hooks:
 	    - id: flake8
-	      additional_dependencies: [flake8-dunder-all==0.2.2]
+	      additional_dependencies: [flake8-dunder-all==0.3.0b1]
 
 ``ensure-dunder-all`` script
 
 There is also a script which will automatically add __all__ for files which don't have it.
 
 See `the documentation <https://flake8-dunder-all.readthedocs.io/en/latest/usage.html#ensure-dunder-all-script>`_
 for details.
```

### Comparing `flake8_dunder_all-0.2.2/PKG-INFO` & `flake8_dunder_all-0.3.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-dunder-all
-Version: 0.2.2
+Version: 0.3.0b1
 Summary: A Flake8 plugin and pre-commit hook which checks to ensure modules have defined '__all__'.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: flake8
 Home-page: https://github.com/python-formate/flake8-dunder-all
 Project-URL: Issue Tracker, https://github.com/python-formate/flake8-dunder-all/issues
 Project-URL: Source Code, https://github.com/python-formate/flake8-dunder-all
@@ -93,16 +93,16 @@
 	:target: https://github.com/python-formate/flake8-dunder-all/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/python-formate/flake8-dunder-all/workflows/mypy/badge.svg
 	:target: https://github.com/python-formate/flake8-dunder-all/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/python-formate/flake8-dunder-all/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/python-formate/flake8-dunder-all/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/python-formate/flake8-dunder-all/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/python-formate/flake8-dunder-all/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/python-formate/flake8-dunder-all/master?logo=coveralls
 	:target: https://coveralls.io/github/python-formate/flake8-dunder-all?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/python-formate/flake8-dunder-all?logo=codefactor
@@ -136,23 +136,23 @@
 .. |license| image:: https://img.shields.io/github/license/python-formate/flake8-dunder-all
 	:target: https://github.com/python-formate/flake8-dunder-all/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/python-formate/flake8-dunder-all
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/python-formate/flake8-dunder-all/v0.2.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/python-formate/flake8-dunder-all/v0.3.0b1
 	:target: https://github.com/python-formate/flake8-dunder-all/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/python-formate/flake8-dunder-all
 	:target: https://github.com/python-formate/flake8-dunder-all/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/flake8-dunder-all
 	:target: https://pypi.org/project/flake8-dunder-all/
 	:alt: PyPI - Downloads
 
 .. end shields
@@ -208,15 +208,15 @@
 
 .. code-block:: yaml
 
 	 - repo: https://gitlab.com/pycqa/flake8
 	   rev: 3.8.1
 	   hooks:
 	    - id: flake8
-	      additional_dependencies: [flake8-dunder-all==0.2.2]
+	      additional_dependencies: [flake8-dunder-all==0.3.0b1]
 
 ``ensure-dunder-all`` script
 
 There is also a script which will automatically add __all__ for files which don't have it.
 
 See `the documentation <https://flake8-dunder-all.readthedocs.io/en/latest/usage.html#ensure-dunder-all-script>`_
 for details.
```

### Comparing `flake8_dunder_all-0.2.2/LICENSE` & `flake8_dunder_all-0.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_dunder_all-0.2.2/flake8_dunder_all/__init__.py` & `flake8_dunder_all-0.3.0b1/flake8_dunder_all/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 # this package
 from flake8_dunder_all.utils import find_noqa, get_docstring_lineno, mark_text_ranges
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT"
-__version__: str = "0.2.2"
+__version__: str = "0.3.0b1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ("Visitor", "Plugin", "check_and_add_all", "DALL000")
 
 DALL000 = "DALL000 Module lacks __all__."
 
 
@@ -218,36 +218,35 @@
 			return
 		elif not visitor.members:
 			return
 		else:
 			yield 1, 0, DALL000, type(self)
 
 
-def check_and_add_all(filename: PathLike, quote_type: str = '"') -> int:
+def check_and_add_all(filename: PathLike, quote_type: str = '"', use_tuple: bool = False) -> int:
 	"""
 	Check the given filename for the presence of a ``__all__`` declaration, and add one if none is found.
 
 	:param filename: The filename of the Python source file (``.py``) to check.
 	:param quote_type: The type of quote to use for strings.
+	:param use_tuple: Whether to use tuples instead of lists for ``__all__``.
 
 	:returns:
 
 	* ``0`` if the file already contains a ``__all__`` declaration,
 	  has no function or class definitions, or has a ``  # noqa: DALL000  ` comment.
 	* ``1`` If ``__all__`` is absent.
 	* ``4`` if an error was encountered when parsing the file.
 
 	.. versionchanged:: 0.2.0
 
 		Now returns ``0`` and doesn't add ``__all__`` if the file contains a ``noqa: DALL000`` comment.
-	"""
 
-	quotes = {"'", '"'}
-	quotes.remove(quote_type)
-	bad_quote, *_ = tuple(quotes)
+	.. versionchanged:: 0.3.0  Added the ``use_tuple`` argument.
+	"""
 
 	filename = PathPlus(filename)
 
 	try:
 		source = filename.read_text()
 		for line in source.splitlines():
 			noqas = find_noqa(line)
@@ -278,22 +277,25 @@
 		docstring_end = len(docstring.split('\n')) + docstring_start
 
 		insertion_position = max(docstring_end, visitor.last_import) + 1
 
 		if not visitor.members:
 			return 0
 
-		members = repr(sorted(visitor.members)).replace(bad_quote, quote_type)
+		members = f"{quote_type}, {quote_type}".join(sorted(visitor.members))
 
 		lines = filename.read_text().split('\n')
 
 		# Ensure there don't end up too many lines
 		if lines[insertion_position].strip():
 			lines.insert(insertion_position, '\n')
 		else:
 			lines.insert(insertion_position, '')
 
-		lines.insert(insertion_position, f"__all__ = {members}")
+		if use_tuple:
+			lines.insert(insertion_position, f"__all__ = ({quote_type}{members}{quote_type}, )")
+		else:
+			lines.insert(insertion_position, f"__all__ = [{quote_type}{members}{quote_type}]")
 
 		filename.write_clean('\n'.join(lines))
 
 		return 1
```

### Comparing `flake8_dunder_all-0.2.2/flake8_dunder_all/__main__.py` & `flake8_dunder_all-0.3.0b1/flake8_dunder_all/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,26 +30,27 @@
 import sys
 from typing import Iterable
 
 # 3rd party
 import click
 from consolekit import click_command
 from consolekit.commands import MarkdownHelpCommand
-from consolekit.options import auto_default_option
+from consolekit.options import auto_default_option, flag_option
 
 # this package
 from flake8_dunder_all import check_and_add_all
 
 __all__ = ("main", )
 
 
 @click.argument("filenames", type=click.STRING, nargs=-1, metavar="FILENAME")
 @auto_default_option("--quote-type", type=click.STRING, help="The type of quote to use.", show_default=True)
+@flag_option("--use-tuple", help="Use tuples instead of lists for __all__.", default=False)
 @click_command(cls=MarkdownHelpCommand)
-def main(filenames: Iterable[str], quote_type: str = '"') -> None:
+def main(filenames: Iterable[str], quote_type: str = '"', use_tuple: bool = False) -> None:
 	"""
 	Given a list of Python source files, check each file defines ``__all__``.
 
 	Exit codes:
 
 	* 0: The file already contains a ``__all__`` declaration or has no function or class definitions.
 	* 1: A ``__all__`` declaration was added to the file.
@@ -58,14 +59,14 @@
 	"""
 
 	retv = 0
 
 	for filename in filenames:
 		filename = filename.strip()
 		click.echo(f"Checking {filename}")
-		retv |= check_and_add_all(filename=filename, quote_type=quote_type)
+		retv |= check_and_add_all(filename=filename, quote_type=quote_type, use_tuple=use_tuple)
 
 	sys.exit(retv)
 
 
 if __name__ == "__main__":
 	sys.exit(main())
```

### Comparing `flake8_dunder_all-0.2.2/flake8_dunder_all/utils.py` & `flake8_dunder_all-0.3.0b1/flake8_dunder_all/utils.py`

 * *Files identical despite different names*

