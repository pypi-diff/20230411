# Comparing `tmp/mkdocs-coverage-0.2.6.tar.gz` & `tmp/mkdocs_coverage-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-coverage-0.2.6.tar", last modified: Sun Nov 13 13:59:30 2022, max compression
+gzip compressed data, was "mkdocs_coverage-0.2.7.tar", last modified: Tue Apr 11 09:43:17 2023, max compression
```

## Comparing `mkdocs-coverage-0.2.6.tar` & `mkdocs_coverage-0.2.7.tar`

### file list

```diff
@@ -1,11 +1,17 @@
--rw-r--r--   0 pawamoy   (1000) users      (985)      754 2022-11-13 12:56:42.129598 mkdocs-coverage-0.2.6/LICENSE
--rw-r--r--   0 pawamoy   (1000) users      (985)     1447 2022-11-13 12:56:42.209598 mkdocs-coverage-0.2.6/README.md
--rw-r--r--   0 pawamoy   (1000) users      (985)     3169 2022-11-13 12:58:31.286450 mkdocs-coverage-0.2.6/pyproject.toml
--rw-r--r--   0 pawamoy   (1000) users      (985)      218 2022-11-13 13:07:16.906015 mkdocs-coverage-0.2.6/src/mkdocs_coverage/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     1319 2022-11-13 13:08:03.266762 mkdocs-coverage-0.2.6/src/mkdocs_coverage/loggers.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     4829 2022-11-13 13:56:15.057285 mkdocs-coverage-0.2.6/src/mkdocs_coverage/plugin.py
--rw-r--r--   0 pawamoy   (1000) users      (985)        0 2022-11-13 12:56:42.029598 mkdocs-coverage-0.2.6/src/mkdocs_coverage/py.typed
--rw-r--r--   0 pawamoy   (1000) users      (985)      168 2022-11-13 12:56:42.026264 mkdocs-coverage-0.2.6/tests/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)       47 2022-11-13 12:56:42.022931 mkdocs-coverage-0.2.6/tests/conftest.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      636 2022-11-12 19:40:00.876841 mkdocs-coverage-0.2.6/tests/test_plugin.py
--rw-------   0 pawamoy   (1000) users      (985)     2950 2022-11-13 13:59:30.098058 mkdocs-coverage-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-04-11 09:21:19.888457 mkdocs_coverage-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1447 2023-04-11 09:21:22.561805 mkdocs_coverage-0.2.7/README.md
+-rw-r--r--   0        0        0     2439 2023-04-11 09:43:17.543348 mkdocs_coverage-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-04-11 09:21:19.791790 mkdocs_coverage-0.2.7/src/mkdocs_coverage/__init__.py
+-rw-r--r--   0        0        0     1289 2023-04-11 09:22:19.352160 mkdocs_coverage-0.2.7/src/mkdocs_coverage/loggers.py
+-rw-r--r--   0        0        0     4739 2023-04-11 09:34:18.910852 mkdocs_coverage-0.2.7/src/mkdocs_coverage/plugin.py
+-rw-r--r--   0        0        0        0 2023-04-11 09:21:19.785123 mkdocs_coverage-0.2.7/src/mkdocs_coverage/py.typed
+-rw-r--r--   0        0        0       37 2021-12-16 22:27:12.259244 mkdocs_coverage-0.2.7/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      194 2021-12-16 22:27:12.259244 mkdocs_coverage-0.2.7/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      295 2021-12-16 22:27:12.259244 mkdocs_coverage-0.2.7/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2021-12-16 22:27:34.598920 mkdocs_coverage-0.2.7/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2021-12-16 22:27:34.598920 mkdocs_coverage-0.2.7/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       10 2021-12-16 22:27:32.335620 mkdocs_coverage-0.2.7/tests/.pytest_cache/v/randomly_seed
+-rw-r--r--   0        0        0      168 2023-04-11 09:21:19.781790 mkdocs_coverage-0.2.7/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-11 09:21:19.778456 mkdocs_coverage-0.2.7/tests/conftest.py
+-rw-r--r--   0        0        0      791 2023-04-11 09:37:31.333365 mkdocs_coverage-0.2.7/tests/test_plugin.py
+-rw-r--r--   0        0        0     2976 1970-01-01 00:00:00.000000 mkdocs_coverage-0.2.7/PKG-INFO
```

### Comparing `mkdocs-coverage-0.2.6/LICENSE` & `mkdocs_coverage-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-coverage-0.2.6/README.md` & `mkdocs_coverage-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-coverage-0.2.6/pyproject.toml` & `mkdocs_coverage-0.2.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [project]
 name = "mkdocs-coverage"
 description = "MkDocs plugin to integrate your coverage HTML report into your site."
 authors = [
     { name = "Timothée Mazzucotelli", email = "pawamoy@pm.me" },
 ]
-license = "ISC"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = []
 dynamic = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -31,15 +30,18 @@
     "Topic :: Software Development :: Documentation",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "mkdocs>=1.2",
 ]
-version = "0.2.6"
+version = "0.2.7"
+
+[project.license]
+text = "ISC"
 
 [project.urls]
 Homepage = "https://pawamoy.github.io/mkdocs-coverage"
 Documentation = "https://pawamoy.github.io/mkdocs-coverage"
 Changelog = "https://pawamoy.github.io/mkdocs-coverage/changelog"
 Repository = "https://github.com/pawamoy/mkdocs-coverage"
 Issues = "https://github.com/pawamoy/mkdocs-coverage/issues"
@@ -55,51 +57,35 @@
 
 [tool.pdm.build]
 package-dir = "src"
 editable-backend = "editables"
 
 [tool.pdm.dev-dependencies]
 duty = [
-    "duty>=0.7",
+    "duty>=0.10",
 ]
 docs = [
+    "black>=23.1",
     "mkdocs>=1.3",
     "mkdocs-gen-files>=0.3",
     "mkdocs-literate-nav>=0.4",
     "mkdocs-material>=7.3",
     "mkdocs-section-index>=0.3",
     "mkdocstrings[python]>=0.18",
     "markdown-callouts>=0.2",
     "markdown-exec>=0.5",
     "toml>=0.10",
 ]
-format = [
-    "autoflake>=1.4",
-    "black>=21.10b0",
-    "isort>=5.10",
-]
 maintain = [
-    "git-changelog>=0.4",
+    "black>=23.1",
+    "blacken-docs>=1.13",
+    "git-changelog>=1.0",
 ]
 quality = [
-    "importlib-metadata<5; python_version < '3.8'",
-    "flake8>=4; python_version >= '3.8'",
-    "darglint>=1.8",
-    "flake8-bandit>=2.1",
-    "flake8-black>=0.2",
-    "flake8-bugbear>=21.9",
-    "flake8-builtins>=1.5",
-    "flake8-comprehensions>=3.7",
-    "flake8-docstrings>=1.6",
-    "flake8-pytest-style>=1.5",
-    "flake8-string-format>=0.3",
-    "flake8-tidy-imports>=4.5",
-    "flake8-variables-names>=0.0",
-    "pep8-naming>=0.12",
-    "wps-light>=0.15",
+    "ruff>=0.0.246",
 ]
 tests = [
     "pytest>=6.2",
     "pytest-cov>=3.0",
     "pytest-randomly>=3.10",
     "pytest-xdist>=2.4",
 ]
@@ -107,21 +93,7 @@
     "mypy>=0.910",
     "types-markdown>=3.3",
     "types-toml>=0.10",
 ]
 security = [
     "safety>=2",
 ]
-
-[tool.black]
-line-length = 120
-exclude = "tests/fixtures"
-
-[tool.isort]
-line_length = 120
-not_skip = "__init__.py"
-multi_line_output = 3
-force_single_line = false
-balanced_wrapping = true
-default_section = "THIRDPARTY"
-known_first_party = "mkdocs_coverage"
-include_trailing_comma = true
```

### Comparing `mkdocs-coverage-0.2.6/src/mkdocs_coverage/loggers.py` & `mkdocs_coverage-0.2.7/src/mkdocs_coverage/loggers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 """Logging functions."""
 
 from __future__ import annotations
 
 import logging
-from typing import Any, MutableMapping, Tuple
+from typing import Any, MutableMapping
 
 from mkdocs.utils import warning_filter
 
 
 class LoggerAdapter(logging.LoggerAdapter):
     """A logger adapter to prefix messages."""
 
     def __init__(self, prefix: str, logger: logging.Logger):
-        """
-        Initialize the object.
+        """Initialize the object.
 
         Arguments:
             prefix: The string to insert in front of every message.
             logger: The logger instance.
         """
         super().__init__(logger, {})
         self.prefix = prefix
 
-    def process(self, msg: str, kwargs: MutableMapping[str, Any]) -> Tuple[Any, MutableMapping[str, Any]]:
-        """
-        Process the message.
+    def process(self, msg: str, kwargs: MutableMapping[str, Any]) -> tuple[Any, MutableMapping[str, Any]]:
+        """Process the message.
 
         Arguments:
             msg: The message:
             kwargs: Remaining arguments.
 
         Returns:
             The processed message, and the remaining arguments.
         """
         return f"{self.prefix}: {msg}", kwargs
 
 
 def get_logger(name: str) -> LoggerAdapter:
-    """
-    Return a pre-configured logger.
+    """Return a pre-configured logger.
 
     Arguments:
         name: The name to use with `logging.getLogger`.
 
     Returns:
         A logger configured to work well in MkDocs.
     """
```

### Comparing `mkdocs-coverage-0.2.6/src/mkdocs_coverage/plugin.py` & `mkdocs_coverage-0.2.7/src/mkdocs_coverage/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,78 @@
 """This module contains the `mkdocs_coverage` plugin."""
 
 from __future__ import annotations
 
 import re
 import shutil
 import textwrap
-from distutils.dir_util import copy_tree
-from distutils.errors import DistutilsFileError
 from pathlib import Path
 from tempfile import mkdtemp
-from typing import Any, Sequence, Tuple
+from typing import TYPE_CHECKING, Any, Sequence
 
-from mkdocs.config import Config
 from mkdocs.config.config_options import Type as MkType
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure.files import File, Files
 
 from mkdocs_coverage.loggers import get_logger
 
+if TYPE_CHECKING:
+    from mkdocs.config import Config
+
 log = get_logger(__name__)
 
 
 class MkDocsCoveragePlugin(BasePlugin):
     """The MkDocs plugin to integrate the coverage HTML report in the site."""
 
-    config_scheme: Sequence[Tuple[str, MkType]] = (
+    config_scheme: Sequence[tuple[str, MkType]] = (
         ("page_name", MkType(str, default="coverage")),
         ("html_report_dir", MkType(str, default="htmlcov")),
     )
 
-    def on_files(self, files: Files, config: Config, **kwargs: Any) -> Files:
-        """
-        Add the coverage page to the navigation.
+    def on_files(self, files: Files, config: Config, **kwargs: Any) -> Files:  # noqa: ARG002
+        """Add the coverage page to the navigation.
 
         Hook for the [`on_files` event](https://www.mkdocs.org/user-guide/plugins/#on_files).
         This hook is used to add the coverage page to the navigation, using a temporary file.
 
         Arguments:
             files: The files collection.
             config: The MkDocs config object.
             **kwargs: Additional arguments passed by MkDocs.
 
         Returns:
             The modified files collection.
         """
-        if config["use_directory_urls"]:
-            covindex = "covindex.html"
-        else:
-            covindex = f"{self.config['page_name']}/covindex.html"
+        covindex = "covindex.html" if config["use_directory_urls"] else f"{self.config['page_name']}/covindex.html"
 
-        style = textwrap.dedent(  # noqa: WPS462
+        style = textwrap.dedent(
             """
             <style>
             article h1, article > a, .md-sidebar--secondary {
                 display: none !important;
             }
             </style>
-            """
+            """,
         )
 
-        iframe = textwrap.dedent(  # noqa: WPS462
+        iframe = textwrap.dedent(
             f"""
             <iframe
                 id="coviframe"
                 src="{covindex}"
                 frameborder="0"
                 scrolling="no"
                 onload="resizeIframe();"
                 width="100%">
             </iframe>
-            """
+            """,
         )
 
-        script = textwrap.dedent(  # noqa: WPS462
+        script = textwrap.dedent(
             """
             <script>
             var coviframe = document.getElementById("coviframe");
 
             function resizeIframe() {
                 coviframe.style.height = coviframe.contentWindow.document.documentElement.offsetHeight + 'px';
             }
@@ -100,17 +96,16 @@
                 str(tempfile.parent),
                 config["site_dir"],
                 config["use_directory_urls"],
             ),
         )
         return files
 
-    def on_post_build(self, config: Config, **kwargs: Any) -> None:  # noqa: W0613,R0201
-        """
-        Copy the coverage HTML report into the site directory.
+    def on_post_build(self, config: Config, **kwargs: Any) -> None:  # noqa: ARG002
+        """Copy the coverage HTML report into the site directory.
 
         Hook for the [`on_post_build` event](https://www.mkdocs.org/user-guide/plugins/#on_post_build).
 
         Rename `index.html` into `covindex.html`.
         Replace every occurrence of `index.html` by `covindex.html` in the HTML files.
 
         Arguments:
@@ -122,18 +117,19 @@
         tmp_index = site_dir / ".coverage-tmp.html"
 
         if config["use_directory_urls"]:
             shutil.move(coverage_dir / "index.html", tmp_index)
         else:
             shutil.move(coverage_dir.with_suffix(".html"), tmp_index)
 
+        shutil.rmtree(str(coverage_dir), ignore_errors=True)
         try:
-            copy_tree(self.config["html_report_dir"], str(coverage_dir))
-        except DistutilsFileError:
-            log.warning("No such HTML report directory: " + self.config["html_report_dir"])
+            shutil.copytree(self.config["html_report_dir"], str(coverage_dir))
+        except FileNotFoundError:
+            log.warning(f"No such HTML report directory: {self.config['html_report_dir']}")
             return
 
         shutil.move(coverage_dir / "index.html", coverage_dir / "covindex.html")
 
         if config["use_directory_urls"]:
             shutil.move(str(tmp_index), coverage_dir / "index.html")
         else:
```

### Comparing `mkdocs-coverage-0.2.6/tests/test_plugin.py` & `mkdocs_coverage-0.2.7/tests/test_plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,21 @@
 import re
 from pathlib import Path
 
 from mkdocs.commands.build import build
 from mkdocs.config.base import load_config
 
 
-def test_plugin():
+def test_plugin() -> None:
     """Build our own documentation."""
     config = load_config()
-    build(config)
+    config["plugins"].run_event("startup", command="build", dirty=False)
+    try:
+        build(config)
+    finally:
+        config["plugins"].run_event("shutdown")
     site_coverage_dir = Path(config["site_dir"]) / "coverage"
     for html_file in site_coverage_dir.iterdir():
         if html_file.suffix == ".html" and html_file.name != "index.html" and "tests" not in html_file.name:
             text = html_file.read_text()
             assert not re.search("covcovindex", text)
             assert not re.search('href="index.html"', text)
```

### Comparing `mkdocs-coverage-0.2.6/PKG-INFO` & `mkdocs_coverage-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: mkdocs-coverage
-Version: 0.2.6
+Version: 0.2.7
 Summary: MkDocs plugin to integrate your coverage HTML report into your site.
+Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
-Author-email: Timothée Mazzucotelli <pawamoy@pm.me>
-Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
+Project-URL: Homepage, https://pawamoy.github.io/mkdocs-coverage
+Project-URL: Documentation, https://pawamoy.github.io/mkdocs-coverage
 Project-URL: Changelog, https://pawamoy.github.io/mkdocs-coverage/changelog
+Project-URL: Repository, https://github.com/pawamoy/mkdocs-coverage
+Project-URL: Issues, https://github.com/pawamoy/mkdocs-coverage/issues
 Project-URL: Discussions, https://github.com/pawamoy/mkdocs-coverage/discussions
-Project-URL: Documentation, https://pawamoy.github.io/mkdocs-coverage
-Project-URL: Funding, https://github.com/sponsors/pawamoy
 Project-URL: Gitter, https://gitter.im/mkdocs-coverage/community
-Project-URL: Homepage, https://pawamoy.github.io/mkdocs-coverage
-Project-URL: Issues, https://github.com/pawamoy/mkdocs-coverage/issues
-Project-URL: Repository, https://github.com/pawamoy/mkdocs-coverage
+Project-URL: Funding, https://github.com/sponsors/pawamoy
+Requires-Python: >=3.7
+Requires-Dist: mkdocs>=1.2
 Description-Content-Type: text/markdown
 
 # MkDocs Coverage Plugin
 
 [![ci](https://github.com/pawamoy/mkdocs-coverage/workflows/ci/badge.svg)](https://github.com/pawamoy/mkdocs-coverage/actions?query=workflow%3Aci)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/mkdocs-coverage/)
 [![pypi version](https://img.shields.io/pypi/v/mkdocs-coverage.svg)](https://pypi.org/project/mkdocs-coverage/)
@@ -69,8 +70,7 @@
 
 Now serve your documentation,
 and go to http://localhost:8000/coverage/
 to see your coverage report!
 
 ![coverage index](https://user-images.githubusercontent.com/3999221/106802970-f4376a80-6663-11eb-8665-e9e09f0f4ac0.png)
 ![coverage module](https://user-images.githubusercontent.com/3999221/106803017-fe596900-6663-11eb-9df9-973755c5b63e.png)
-
```

