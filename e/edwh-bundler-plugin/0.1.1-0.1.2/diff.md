# Comparing `tmp/edwh_bundler_plugin-0.1.1.tar.gz` & `tmp/edwh_bundler_plugin-0.1.2.tar.gz`

## Comparing `edwh_bundler_plugin-0.1.1.tar` & `edwh_bundler_plugin-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.1/src/edwh_bundler_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.1/src/edwh_bundler_plugin/__init__.py
--rw-r--r--   0        0        0    19877 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.1/src/edwh_bundler_plugin/bundler_plugin.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.1/src/edwh_bundler_plugin/css.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.1/src/edwh_bundler_plugin/js.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.1/src/edwh_bundler_plugin/lazy.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.1/src/edwh_bundler_plugin/shared.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.1/README.md
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/requirements-dev.in
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/__init__.py
+-rw-r--r--   0        0        0    19160 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/bundler_plugin.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/css.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/js.py
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/shared.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/README.md
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.2/PKG-INFO
```

### Comparing `edwh_bundler_plugin-0.1.1/src/edwh_bundler_plugin/bundler_plugin.py` & `edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/bundler_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,32 +13,30 @@
 
 import invoke
 import yaml
 from invoke import task
 
 from .css import extract_contents_for_css
 from .js import extract_contents_for_js
-from .lazy import JIT
 from .shared import truthy
+from dotenv import load_dotenv
 
 now = datetime.utcnow
 
 # prgram is created in __init__
 
 # defaults/consts
 DEFAULT_INPUT = "bundle.yaml"
 DEFAULT_INPUT_LTS = "bundle-lts.yaml"
 DEFAULT_OUTPUT_JS = "bundle.js"
 DEFAULT_OUTPUT_CSS = "bundle.css"
 TEMP_OUTPUT_DIR = "/tmp/bundle-build/"
 TEMP_OUTPUT = ".bundle_tmp"
 DEFAULT_ASSETS_DB = "py4web/apps/lts/databases/lts_assets.db"
 
-load_dotenv = JIT("dotenv", "load_dotenv")
-
 
 def load_config(fname: str = DEFAULT_INPUT, strict=False) -> dict:
     """
     Load yaml config from file name, default to empty or error if strict
     """
     if os.path.exists(fname):
         with open(fname) as f:
@@ -177,47 +175,15 @@
         os.rename(bufferf.name, output)
     if verbose:
         print(f"Written final bundle to {output}", file=sys.stderr)
 
     return output
 
 
-@task
-def require_jsmin(c):
-    try:
-        import rjsmin
-    except ImportError:
-        c.run("pip install rjsmin")
-
-
-@task
-def require_httpx(c):
-    try:
-        import httpx
-    except ImportError:
-        c.run("pip install httpx")
-
-
-@task
-def require_sass(c):
-    try:
-        import sass
-    except ImportError:
-        c.run("pip install pysass")
-
-
-@task
-def require_dotenv(c):
-    try:
-        import dotenv
-    except ImportError:
-        c.run("pip install python-dotenv")
-
-
-@task(iterable=["files"], pre=[require_jsmin, require_httpx])
+@task(iterable=["files"])
 def build_js(
     c,
     files=None,
     input=DEFAULT_INPUT,
     verbose=False,
     # overrule config:
     output=None,  # DEFAULT_OUTPUT_JS
@@ -242,15 +208,15 @@
 
     minify = cli_or_config(minify, settings, "minify")
     cache = cli_or_config(cache, settings, "cache", default=True)
     output = (
         sys.stdout
         if stdout
         else cli_or_config(output, settings, "output_js", bool=False)
-        or DEFAULT_OUTPUT_JS
+             or DEFAULT_OUTPUT_JS
     )
 
     settings["version"] = cli_or_config(
         version, settings, "version", bool=False, default="latest"
     )
 
     return _handle_files(
@@ -302,15 +268,15 @@
     if isinstance(output, io.StringIO):
         output.seek(0)
         return output.read()
     else:
         return output
 
 
-@task(iterable=["files"], pre=[require_sass, require_httpx])
+@task(iterable=["files"])
 def build_css(
     c,
     files=None,
     input=DEFAULT_INPUT,
     verbose=False,
     # overrule config:
     output=None,  # DEFAULT_OUTPUT_CSS
@@ -332,15 +298,15 @@
         version, settings, "version", bool=False, default="latest"
     )
 
     output = (
         sys.stdout
         if stdout
         else cli_or_config(output, settings, "output_css", bool=False)
-        or DEFAULT_OUTPUT_CSS
+             or DEFAULT_OUTPUT_CSS
     )
 
     files = files or config.get("css")
 
     if not files:
         raise ValueError(
             "Please specify either --files or the css key in a config yaml (e.g. bundle.yaml)"
@@ -395,15 +361,15 @@
     if isinstance(output, io.StringIO):
         output.seek(0)
         return output.read()
     else:
         return output
 
 
-@task(iterable=["files"], pre=[require_sass, require_jsmin, require_httpx])
+@task(iterable=["files"])
 def build(
     c,
     input=DEFAULT_INPUT,
     verbose=False,
     # defaults from config, can be overwritten:
     output_js=None,  # DEFAULT_OUTPUT_JS
     output_css=None,  # DEFAULT_OUTPUT_CSS
@@ -534,25 +500,25 @@
     idx = row["id"]
 
     hostingdomain = os.environ.get("HOSTINGDOMAIN", "your.domain")
 
     print(f"https://py4web.{hostingdomain}/lts/manage_versions/edit/{idx}")
 
 
-@task(pre=[require_dotenv])
+@task()
 def show_changelog_url(c, filetype, version):
     db = setup_db(c)
     prompt_changelog(db, filetype, version)
 
 
 def confirm(prompt: str, force=False) -> bool:
     return force or truthy(input(prompt))
 
 
-@task(pre=[require_dotenv, require_jsmin, require_sass, require_httpx])
+@task()
 def publish(
     c,
     version=None,
     major=False,
     minor=False,
     patch=False,
     filename=None,
@@ -718,17 +684,16 @@
 
     db.execute("DELETE FROM bundle_version;")
     db.commit()
     _update_assets_sql(c)
 
     assert db.execute("SELECT COUNT(*) as c FROM bundle_version;").fetchone()["c"] == 0
 
-
 # DEV:
 
 #
 # @task
 # def update_dependencies(c):
 #     # invoke update-dependencies
 #     c.run("pip-compile requirements.in")
 #     c.run("pip-compile requirements-dev.in")
-#     c.run("pip-sync *.txt")
+#     c.run("pip-sync *.txt")
```

### Comparing `edwh_bundler_plugin-0.1.1/src/edwh_bundler_plugin/css.py` & `edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/css.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 # methods for converting CSS files
 from __future__ import annotations
 
 from functools import singledispatch
 
-from .lazy import JIT
-
-# libsass
-# will be installed by pre=[require_sass]
-
-sass = JIT("sass")
+import sass
 
 from .shared import (
     extract_contents_cdn,
     extract_contents_local,
     truthy,
     _del_whitespace,
 )
```

### Comparing `edwh_bundler_plugin-0.1.1/src/edwh_bundler_plugin/js.py` & `edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/js.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 # methods for converting JS and hyperscript files
 
 from __future__ import annotations
 
 from functools import singledispatch
 
-from .lazy import JIT
-
-# will be installed by pre=[require_jsmin]
-jsmin = JIT("rjsmin", "jsmin")
-
+from rjsmin import jsmin
 
 from .shared import (
     extract_contents_cdn,
     extract_contents_local,
     HS_COMMENT_RE,
     DOUBLE_SPACE_RE,
     _del_whitespace,
@@ -122,8 +118,8 @@
     # " \n " -> "   " -> " "
     return DOUBLE_SPACE_RE.sub(
         " ",
         # -- at the first line will not be caught by HS_COMMENT_RE, so prefix with newline
         HS_COMMENT_RE.sub(" ", "\n" + contents)
         # replace every newline with space for minification
         .replace("\n", " "),
-    )
+    )
```

### Comparing `edwh_bundler_plugin-0.1.1/src/edwh_bundler_plugin/shared.py` & `edwh_bundler_plugin-0.1.2/src/edwh_bundler_plugin/shared.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 from __future__ import annotations
 
 import hashlib
 import os
 import re
 from functools import singledispatch
 from pathlib import Path
-
-from .lazy import JIT
-
-httpx = JIT("httpx")
+import httpx
 
 _CACHE_DIR = ".cdn_cache"
 CACHE_DIR = Path(_CACHE_DIR)
 
 # https://stackoverflow.com/questions/70064025/regex-pattern-to-match-comments-but-not-urls
 HS_COMMENT_RE = re.compile(r"(?<=[^:])(//|--).+$", re.MULTILINE)
 DOUBLE_SPACE_RE = re.compile(" {2,}")
```

### Comparing `edwh_bundler_plugin-0.1.1/LICENSE.txt` & `edwh_bundler_plugin-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.1/README.md` & `edwh_bundler_plugin-0.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
+- [Changelog](#changelog)
 
 ## Installation
 
 ```console
 pip install edwh-bundler-plugin
 ```
 
@@ -23,7 +24,11 @@
 # or
 pipx install edwh[plugins,omgeving]
 ```
 
 ## License
 
 `edwh-bundler-plugin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+
+## Changelog 
+
+[See CHANGELOG.md](CHANGELOG.md)
```

### Comparing `edwh_bundler_plugin-0.1.1/pyproject.toml` & `edwh_bundler_plugin-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ['invoke', 'python-dotenv', 'pysass', 'rjsmin']
+dependencies = ['invoke', 'python-dotenv', 'pysass', 'rjsmin', 'httpx', 'pyyaml']
 
 [project.urls]
 Documentation = "https://github.com/educationwarehouse/edwh-bundler-plugin#readme"
 Issues = "https://github.com/educationwarehouse/edwh-bundler-plugin/issues"
 Source = "https://github.com/educationwarehouse/edwh-bundler-plugin"
 
 # https://packaging.python.org/en/latest/guides/creating-and-discovering-plugins/#using-package-metadata
```

### Comparing `edwh_bundler_plugin-0.1.1/PKG-INFO` & `edwh_bundler_plugin-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-bundler-plugin
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python-only static file (js, css) bundler for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-bundler-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-bundler-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-bundler-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -14,31 +14,34 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: httpx
 Requires-Dist: invoke
 Requires-Dist: pysass
 Requires-Dist: python-dotenv
+Requires-Dist: pyyaml
 Requires-Dist: rjsmin
 Description-Content-Type: text/markdown
 
 # edwh-bundler-plugin
 
 [![PyPI - Version](https://img.shields.io/pypi/v/edwh-bundler-plugin.svg)](https://pypi.org/project/edwh-bundler-plugin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-bundler-plugin.svg)](https://pypi.org/project/edwh-bundler-plugin)
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
+- [Changelog](#changelog)
 
 ## Installation
 
 ```console
 pip install edwh-bundler-plugin
 ```
 
@@ -49,7 +52,11 @@
 # or
 pipx install edwh[plugins,omgeving]
 ```
 
 ## License
 
 `edwh-bundler-plugin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+
+## Changelog 
+
+[See CHANGELOG.md](CHANGELOG.md)
```

