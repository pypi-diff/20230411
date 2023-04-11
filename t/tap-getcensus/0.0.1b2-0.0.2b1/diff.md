# Comparing `tmp/tap_getcensus-0.0.1b2.tar.gz` & `tmp/tap_getcensus-0.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_getcensus-0.0.1b2.tar", max compression
+gzip compressed data, was "tap_getcensus-0.0.2b1.tar", max compression
```

## Comparing `tap_getcensus-0.0.1b2.tar` & `tap_getcensus-0.0.2b1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     4470 2022-12-07 23:25:36.659033 tap_getcensus-0.0.1b2/README.md
--rw-r--r--   0        0        0     1861 2022-12-07 23:25:55.903087 tap_getcensus-0.0.1b2/pyproject.toml
--rw-r--r--   0        0        0       84 2022-12-07 23:25:36.659033 tap_getcensus-0.0.1b2/tap_getcensus/__init__.py
--rw-r--r--   0        0        0      116 2022-12-07 23:25:36.659033 tap_getcensus-0.0.1b2/tap_getcensus/__main__.py
--rw-r--r--   0        0        0     2248 2022-12-07 23:25:36.659033 tap_getcensus-0.0.1b2/tap_getcensus/client.py
--rw-r--r--   0        0        0    20432 2022-12-07 23:25:36.659033 tap_getcensus-0.0.1b2/tap_getcensus/streams.py
--rw-r--r--   0        0        0     1034 2022-12-07 23:25:36.659033 tap_getcensus-0.0.1b2/tap_getcensus/tap.py
--rw-r--r--   0        0        0     5519 1970-01-01 00:00:00.000000 tap_getcensus-0.0.1b2/setup.py
--rw-r--r--   0        0        0     5479 1970-01-01 00:00:00.000000 tap_getcensus-0.0.1b2/PKG-INFO
+-rw-r--r--   0        0        0     4270 2023-04-11 06:14:09.011448 tap_getcensus-0.0.2b1/README.md
+-rw-r--r--   0        0        0     2036 2023-04-11 06:14:30.135483 tap_getcensus-0.0.2b1/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-04-11 06:14:09.015448 tap_getcensus-0.0.2b1/tap_getcensus/__init__.py
+-rw-r--r--   0        0        0      116 2023-04-11 06:14:09.015448 tap_getcensus-0.0.2b1/tap_getcensus/__main__.py
+-rw-r--r--   0        0        0     2287 2023-04-11 06:14:09.015448 tap_getcensus-0.0.2b1/tap_getcensus/client.py
+-rw-r--r--   0        0        0    20605 2023-04-11 06:14:09.015448 tap_getcensus-0.0.2b1/tap_getcensus/streams.py
+-rw-r--r--   0        0        0      955 2023-04-11 06:14:09.015448 tap_getcensus-0.0.2b1/tap_getcensus/tap.py
+-rw-r--r--   0        0        0     5279 1970-01-01 00:00:00.000000 tap_getcensus-0.0.2b1/PKG-INFO
```

### Comparing `tap_getcensus-0.0.1b2/README.md` & `tap_getcensus-0.0.2b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -63,16 +63,14 @@
 tap-getcensus --version
 tap-getcensus --help
 tap-getcensus --config CONFIG --discover > ./catalog.json
 ```
 
 ## Developer Resources
 
-- [ ] `Developer TODO:` As a first step, scan the entire project for the text "`TODO:`" and complete any recommended steps, deleting the "TODO" references once completed.
-
 ### Initialize your Development Environment
 
 ```bash
 pipx install poetry
 poetry install
 ```
 
@@ -91,33 +89,35 @@
 ```
 
 ### Testing with [Meltano](https://www.meltano.com)
 
 _**Note:** This tap will work in any Singer environment and does not require Meltano.
 Examples here are for convenience and to streamline end-to-end orchestration scenarios._
 
-Your project comes with a custom `meltano.yml` project file already created. Open the `meltano.yml` and follow any _"TODO"_ items listed in
-the file.
-
-Next, install Meltano (if you haven't already) and any needed plugins:
+Your project comes with a custom `meltano.yml` project file already created. Install Meltano (if you haven't already) and any needed plugins:
 
 ```bash
 # Install meltano
 pipx install meltano
+
+# Update all plugin definitions
+meltano lock --update --all
+
 # Initialize meltano within this directory
 cd tap-getcensus
 meltano install
 ```
 
 Now you can test and orchestrate using Meltano:
 
 ```bash
 # Test invocation:
 meltano invoke tap-getcensus --version
-# OR run a test `elt` pipeline:
-meltano elt tap-getcensus target-jsonl
+
+# OR run a pipeline:
+meltano run tap-getcensus target-jsonl
 ```
 
 ### SDK Dev Guide
 
 See the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the SDK to
 develop your own taps and targets.
```

#### html2text {}

```diff
@@ -26,26 +26,24 @@
 Table | None | id | https://docs.getcensus.com/basics/api/source-objects#get-
 sources-id-objects | The full catalog is available by running: `tap-getcensus -
 -discover` ### Source Authentication and Authorization See the [API docs]
 (https://docs.getcensus.com/basics/api#getting-api-access). ## Usage You can
 easily run `tap-getcensus` by itself or in a pipeline using [Meltano](https://
 meltano.com/). ### Executing the Tap Directly ```bash tap-getcensus --version
 tap-getcensus --help tap-getcensus --config CONFIG --discover > ./catalog.json
-``` ## Developer Resources - [ ] `Developer TODO:` As a first step, scan the
-entire project for the text "`TODO:`" and complete any recommended steps,
-deleting the "TODO" references once completed. ### Initialize your Development
-Environment ```bash pipx install poetry poetry install ``` ### Create and Run
-Tests Create tests within the `tests` subfolder and then run: ```bash poetry
-run pytest ``` You can also test the `tap-getcensus` CLI interface directly
-using `poetry run`: ```bash poetry run tap-getcensus --help ``` ### Testing
-with [Meltano](https://www.meltano.com) _**Note:** This tap will work in any
-Singer environment and does not require Meltano. Examples here are for
-convenience and to streamline end-to-end orchestration scenarios._ Your project
-comes with a custom `meltano.yml` project file already created. Open the
-`meltano.yml` and follow any _"TODO"_ items listed in the file. Next, install
-Meltano (if you haven't already) and any needed plugins: ```bash # Install
-meltano pipx install meltano # Initialize meltano within this directory cd tap-
-getcensus meltano install ``` Now you can test and orchestrate using Meltano:
-```bash # Test invocation: meltano invoke tap-getcensus --version # OR run a
-test `elt` pipeline: meltano elt tap-getcensus target-jsonl ``` ### SDK Dev
-Guide See the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for
-more instructions on how to use the SDK to develop your own taps and targets.
+``` ## Developer Resources ### Initialize your Development Environment ```bash
+pipx install poetry poetry install ``` ### Create and Run Tests Create tests
+within the `tests` subfolder and then run: ```bash poetry run pytest ``` You
+can also test the `tap-getcensus` CLI interface directly using `poetry run`:
+```bash poetry run tap-getcensus --help ``` ### Testing with [Meltano](https://
+www.meltano.com) _**Note:** This tap will work in any Singer environment and
+does not require Meltano. Examples here are for convenience and to streamline
+end-to-end orchestration scenarios._ Your project comes with a custom
+`meltano.yml` project file already created. Install Meltano (if you haven't
+already) and any needed plugins: ```bash # Install meltano pipx install meltano
+# Update all plugin definitions meltano lock --update --all # Initialize
+meltano within this directory cd tap-getcensus meltano install ``` Now you can
+test and orchestrate using Meltano: ```bash # Test invocation: meltano invoke
+tap-getcensus --version # OR run a pipeline: meltano run tap-getcensus target-
+jsonl ``` ### SDK Dev Guide See the [dev guide](https://sdk.meltano.com/en/
+latest/dev_guide.html) for more instructions on how to use the SDK to develop
+your own taps and targets.
```

### Comparing `tap_getcensus-0.0.1b2/pyproject.toml` & `tap_getcensus-0.0.2b1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-getcensus"
-version = "0.0.1b2"
+version = "0.0.2b1"
 description = "Singer tap for the Census Operational Analytics Platform, built with the Meltano SDK for Singer Taps."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 maintainers = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-getcensus"
 repository = "https://github.com/edgarrmondragon/tap-getcensus"
@@ -13,20 +13,18 @@
   "ELT",
   "singer.io",
   "Census",
 ]
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
-singer-sdk = "0.14.0"
+singer-sdk = "0.23.0"
 
 [tool.poetry.dev-dependencies]
-mypy = ">=0.950"
-pytest = "^7.2.0"
-types-requests = "^2.28.11"
+pytest = "^7.3.0"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3 # Vertical Hanging Indent
 use_parentheses = true
 include_trailing_comma = true
 src_paths = "tap_getcensus"
@@ -64,7 +62,21 @@
     {%- else -%}
         {{ serialize_pep440(bump_version(base), stage, revision, dev=distance, metadata=[commit]) }}
     {%- endif -%}
 """
 metadata = true
 style = "pep440"
 vcs = "git"
+
+[tool.ruff]
+ignore = [
+    "ANN101", # missing-type-self
+    "DJ",     # flake8-django
+]
+line-length = 88
+select = ["ALL"]
+
+[tool.ruff.per-file-ignores]
+"tests/*" = ["ANN"]
+
+[tool.ruff.pydocstyle]
+convention = "google"
```

### Comparing `tap_getcensus-0.0.1b2/tap_getcensus/client.py` & `tap_getcensus-0.0.2b1/tap_getcensus/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """REST client handling, including CensusStream base class."""
 
 from __future__ import annotations
 
-from typing import Any
+import typing as t
 from urllib.parse import ParseResult, parse_qsl
 
-import requests
 from singer_sdk import RESTStream
 from singer_sdk.authenticators import BasicAuthenticator
 from singer_sdk.pagination import BaseHATEOASPaginator
 
+if t.TYPE_CHECKING:
+    import requests
+
 
 class CensusPaginator(BaseHATEOASPaginator):
     """Census API pagination class."""
 
     def get_next_url(self, response: requests.Response) -> str | None:
         """Get the next URL.
 
@@ -56,17 +58,17 @@
         """
         headers = {}
         headers["User-Agent"] = f"{self.tap_name}/{self._tap.plugin_version}"
         return headers
 
     def get_url_params(
         self,
-        context: dict | None,
+        context: dict | None,  # noqa: ARG002
         next_page_token: ParseResult | None,
-    ) -> dict[str, Any]:
+    ) -> dict[str, t.Any]:
         """Get URL query parameters.
 
         Args:
             context: Stream sync context.
             next_page_token: Next offset.
 
         Returns:
```

### Comparing `tap_getcensus-0.0.1b2/tap_getcensus/streams.py` & `tap_getcensus-0.0.2b1/tap_getcensus/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,16 +104,16 @@
             "mirror_strategy",
             th.StringType,
             description="The sync's mirror strategy type",
         ),
         # TODO: Add advanced_configuration when Census documentation is updated
         # th.Property(
         #     "advanced_configuration",
-        #     th.ObjectType(),
-        #     description="The sync's advanced configuration",
+        #     th.ObjectType(),  # noqa: ERA001
+        #     description="The sync's advanced configuration",  # noqa: ERA001
         # ),
         th.Property(
             "source_attributes",
             th.ObjectType(
                 th.Property(
                     "connection_id",
                     th.IntegerType,
@@ -220,15 +220,19 @@
                         description="The sync's mapping operation type",
                     ),
                 ),
             ),
         ),
     ).to_dict()
 
-    def get_child_context(self, record: dict, context: dict | None) -> dict:
+    def get_child_context(
+        self,
+        record: dict,
+        context: dict | None,  # noqa: ARG002
+    ) -> dict:
         """Get child context.
 
         Args:
             record: The record.
             context: The context.
 
         Returns:
@@ -367,15 +371,19 @@
         th.Property(
             "connection_details",
             th.ObjectType(),
             description="The destination's connection details",
         ),
     ).to_dict()
 
-    def get_child_context(self, record: dict, context: dict | None) -> dict:
+    def get_child_context(
+        self,
+        record: dict,
+        context: dict | None,  # noqa: ARG002
+    ) -> dict:
         """Get child context.
 
         Args:
             record: The record.
             context: The context.
 
         Returns:
@@ -554,15 +562,19 @@
         th.Property(
             "read_only_connection",
             th.BooleanType,
             description="Whether the source is read-only",
         ),
     ).to_dict()
 
-    def get_child_context(self, record: dict, context: dict | None) -> dict:
+    def get_child_context(
+        self,
+        record: dict,
+        context: dict | None,  # noqa: ARG002
+    ) -> dict:
         """Get child context.
 
         Args:
             record: The record.
             context: The context.
 
         Returns:
```

### Comparing `tap_getcensus-0.0.1b2/setup.py` & `tap_getcensus-0.0.2b1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,147 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tap-getcensus
+Version: 0.0.2b1
+Summary: Singer tap for the Census Operational Analytics Platform, built with the Meltano SDK for Singer Taps.
+Home-page: https://github.com/edgarrmondragon/tap-getcensus
+License: Apache-2.0
+Keywords: ELT,singer.io,Census
+Author: Edgar Ramírez-Mondragón
+Author-email: edgarrm358@gmail.com
+Maintainer: Edgar Ramírez-Mondragón
+Maintainer-email: edgarrm358@gmail.com
+Requires-Python: >=3.7.1,<3.12
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: singer-sdk (==0.23.0)
+Project-URL: Documentation, https://github.com/edgarrmondragon/tap-getcensus/#readme
+Project-URL: Repository, https://github.com/edgarrmondragon/tap-getcensus
+Description-Content-Type: text/markdown
 
-packages = \
-['tap_getcensus']
+<div align="center">
 
-package_data = \
-{'': ['*']}
+# tap-getcensus
 
-install_requires = \
-['singer-sdk==0.14.0']
-
-entry_points = \
-{'console_scripts': ['tap-getcensus = tap_getcensus.tap:TapCensus.cli']}
-
-setup_kwargs = {
-    'name': 'tap-getcensus',
-    'version': '0.0.1b2',
-    'description': 'Singer tap for the Census Operational Analytics Platform, built with the Meltano SDK for Singer Taps.',
-    'long_description': '<div align="center">\n\n# tap-getcensus\n\n<div>\n  <a href="https://results.pre-commit.ci/latest/github/edgarrmondragon/tap-getcensus/main">\n    <img alt="pre-commit.ci status" src="https://results.pre-commit.ci/badge/github/edgarrmondragon/tap-getcensus/main.svg"/>\n  </a>\n  <a href="https://github.com/edgarrmondragon/tap-getcensus/blob/main/LICENSE">\n    <img alt="License" src="https://img.shields.io/github/license/edgarrmondragon/tap-getcensus"/>\n  </a>\n</div>\n\nSinger Tap for the [Census Operational Analytics Platform](https://www.getcensus.com/). Built with the [Meltano Singer SDK](https://sdk.meltano.com).\n\n</div>\n\n## Capabilities\n\n* `catalog`\n* `state`\n* `discover`\n* `about`\n* `stream-maps`\n* `schema-flattening`\n\n## Settings\n\n| Setting             | Required | Default | Description |\n|:--------------------|:--------:|:-------:|:------------|\n| api_token           | True     | None    | Auth token for getcensus.com API |\n| stream_maps         | False    | None    | Config object for stream maps capability. |\n| stream_map_config   | False    | None    | User-defined config values to be used within map expressions. |\n| flattening_enabled  | False    | None    | \'True\' to enable schema flattening and automatically expand nested properties. |\n| flattening_max_depth| False    | None    | The max depth to flatten schemas. |\n\nA full list of supported settings and capabilities is available by running: `tap-getcensus --about`\n\n## Streams\n\n| Stream                | Replication Method | Replication Key | Primary Key | Documentation |\n|:----------------------|:------------------:|:---------------:|:-----------:|:-------------:|\n| `syncs`               | Full Table         | None            | id          | https://docs.getcensus.com/basics/api/syncs#get-syncs |\n| `sync_runs`           | Full Table         | None            | id          | https://docs.getcensus.com/basics/api/sync-runs#get-syncs-id-sync_runs |\n| `destinations`        | Full Table         | None            | id          | https://docs.getcensus.com/basics/api/destinations#get-destinations |\n| `destination_objects` | Full Table         | None            | id          | https://docs.getcensus.com/basics/api/destination-objects#get-destinations-id-objects |\n| `sources`             | Full Table         | None            | id          | https://docs.getcensus.com/basics/api/sources#get-sources |\n| `source_objects`      | Full Table         | None            | id          | https://docs.getcensus.com/basics/api/source-objects#get-sources-id-objects |\n\nThe full catalog is available by running: `tap-getcensus --discover`\n\n### Source Authentication and Authorization\n\nSee the [API docs](https://docs.getcensus.com/basics/api#getting-api-access).\n\n## Usage\n\nYou can easily run `tap-getcensus` by itself or in a pipeline using [Meltano](https://meltano.com/).\n\n### Executing the Tap Directly\n\n```bash\ntap-getcensus --version\ntap-getcensus --help\ntap-getcensus --config CONFIG --discover > ./catalog.json\n```\n\n## Developer Resources\n\n- [ ] `Developer TODO:` As a first step, scan the entire project for the text "`TODO:`" and complete any recommended steps, deleting the "TODO" references once completed.\n\n### Initialize your Development Environment\n\n```bash\npipx install poetry\npoetry install\n```\n\n### Create and Run Tests\n\nCreate tests within the `tests` subfolder and then run:\n\n```bash\npoetry run pytest\n```\n\nYou can also test the `tap-getcensus` CLI interface directly using `poetry run`:\n\n```bash\npoetry run tap-getcensus --help\n```\n\n### Testing with [Meltano](https://www.meltano.com)\n\n_**Note:** This tap will work in any Singer environment and does not require Meltano.\nExamples here are for convenience and to streamline end-to-end orchestration scenarios._\n\nYour project comes with a custom `meltano.yml` project file already created. Open the `meltano.yml` and follow any _"TODO"_ items listed in\nthe file.\n\nNext, install Meltano (if you haven\'t already) and any needed plugins:\n\n```bash\n# Install meltano\npipx install meltano\n# Initialize meltano within this directory\ncd tap-getcensus\nmeltano install\n```\n\nNow you can test and orchestrate using Meltano:\n\n```bash\n# Test invocation:\nmeltano invoke tap-getcensus --version\n# OR run a test `elt` pipeline:\nmeltano elt tap-getcensus target-jsonl\n```\n\n### SDK Dev Guide\n\nSee the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the SDK to\ndevelop your own taps and targets.\n',
-    'author': 'Edgar Ramírez-Mondragón',
-    'author_email': 'edgarrm358@gmail.com',
-    'maintainer': 'Edgar Ramírez-Mondragón',
-    'maintainer_email': 'edgarrm358@gmail.com',
-    'url': 'https://github.com/edgarrmondragon/tap-getcensus',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<3.12',
-}
+<div>
+  <a href="https://results.pre-commit.ci/latest/github/edgarrmondragon/tap-getcensus/main">
+    <img alt="pre-commit.ci status" src="https://results.pre-commit.ci/badge/github/edgarrmondragon/tap-getcensus/main.svg"/>
+  </a>
+  <a href="https://github.com/edgarrmondragon/tap-getcensus/blob/main/LICENSE">
+    <img alt="License" src="https://img.shields.io/github/license/edgarrmondragon/tap-getcensus"/>
+  </a>
+</div>
 
+Singer Tap for the [Census Operational Analytics Platform](https://www.getcensus.com/). Built with the [Meltano Singer SDK](https://sdk.meltano.com).
+
+</div>
+
+## Capabilities
+
+* `catalog`
+* `state`
+* `discover`
+* `about`
+* `stream-maps`
+* `schema-flattening`
+
+## Settings
+
+| Setting             | Required | Default | Description |
+|:--------------------|:--------:|:-------:|:------------|
+| api_token           | True     | None    | Auth token for getcensus.com API |
+| stream_maps         | False    | None    | Config object for stream maps capability. |
+| stream_map_config   | False    | None    | User-defined config values to be used within map expressions. |
+| flattening_enabled  | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |
+| flattening_max_depth| False    | None    | The max depth to flatten schemas. |
+
+A full list of supported settings and capabilities is available by running: `tap-getcensus --about`
+
+## Streams
+
+| Stream                | Replication Method | Replication Key | Primary Key | Documentation |
+|:----------------------|:------------------:|:---------------:|:-----------:|:-------------:|
+| `syncs`               | Full Table         | None            | id          | https://docs.getcensus.com/basics/api/syncs#get-syncs |
+| `sync_runs`           | Full Table         | None            | id          | https://docs.getcensus.com/basics/api/sync-runs#get-syncs-id-sync_runs |
+| `destinations`        | Full Table         | None            | id          | https://docs.getcensus.com/basics/api/destinations#get-destinations |
+| `destination_objects` | Full Table         | None            | id          | https://docs.getcensus.com/basics/api/destination-objects#get-destinations-id-objects |
+| `sources`             | Full Table         | None            | id          | https://docs.getcensus.com/basics/api/sources#get-sources |
+| `source_objects`      | Full Table         | None            | id          | https://docs.getcensus.com/basics/api/source-objects#get-sources-id-objects |
+
+The full catalog is available by running: `tap-getcensus --discover`
+
+### Source Authentication and Authorization
+
+See the [API docs](https://docs.getcensus.com/basics/api#getting-api-access).
+
+## Usage
+
+You can easily run `tap-getcensus` by itself or in a pipeline using [Meltano](https://meltano.com/).
+
+### Executing the Tap Directly
+
+```bash
+tap-getcensus --version
+tap-getcensus --help
+tap-getcensus --config CONFIG --discover > ./catalog.json
+```
+
+## Developer Resources
+
+### Initialize your Development Environment
+
+```bash
+pipx install poetry
+poetry install
+```
+
+### Create and Run Tests
+
+Create tests within the `tests` subfolder and then run:
+
+```bash
+poetry run pytest
+```
+
+You can also test the `tap-getcensus` CLI interface directly using `poetry run`:
+
+```bash
+poetry run tap-getcensus --help
+```
+
+### Testing with [Meltano](https://www.meltano.com)
+
+_**Note:** This tap will work in any Singer environment and does not require Meltano.
+Examples here are for convenience and to streamline end-to-end orchestration scenarios._
+
+Your project comes with a custom `meltano.yml` project file already created. Install Meltano (if you haven't already) and any needed plugins:
+
+```bash
+# Install meltano
+pipx install meltano
+
+# Update all plugin definitions
+meltano lock --update --all
+
+# Initialize meltano within this directory
+cd tap-getcensus
+meltano install
+```
+
+Now you can test and orchestrate using Meltano:
+
+```bash
+# Test invocation:
+meltano invoke tap-getcensus --version
+
+# OR run a pipeline:
+meltano run tap-getcensus target-jsonl
+```
+
+### SDK Dev Guide
+
+See the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the SDK to
+develop your own taps and targets.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,67 +1,63 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['tap_getcensus'] package_data = \ {'': ['*']} install_requires = \ ['singer-
-sdk==0.14.0'] entry_points = \ {'console_scripts': ['tap-getcensus =
-tap_getcensus.tap:TapCensus.cli']} setup_kwargs = { 'name': 'tap-getcensus',
-'version': '0.0.1b2', 'description': 'Singer tap for the Census Operational
-Analytics Platform, built with the Meltano SDK for Singer Taps.',
-'long_description': '
-                            \n\n# tap-getcensus\n\n
-               \n \n_[pre-commit.ci_status]\n\n \n_[License]\n\n
-    \n\nSinger Tap for the [Census Operational Analytics Platform](https://
+Metadata-Version: 2.1 Name: tap-getcensus Version: 0.0.2b1 Summary: Singer tap
+for the Census Operational Analytics Platform, built with the Meltano SDK for
+Singer Taps. Home-page: https://github.com/edgarrmondragon/tap-getcensus
+License: Apache-2.0 Keywords: ELT,singer.io,Census Author: Edgar RamÃ­rez-
+MondragÃ³n Author-email: edgarrm358@gmail.com Maintainer: Edgar RamÃ­rez-
+MondragÃ³n Maintainer-email: edgarrm358@gmail.com Requires-Python:
+>=3.7.1,<3.12 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: singer-sdk (==0.23.0) Project-URL:
+Documentation, https://github.com/edgarrmondragon/tap-getcensus/#readme
+Project-URL: Repository, https://github.com/edgarrmondragon/tap-getcensus
+Description-Content-Type: text/markdown
+                                # tap-getcensus
+                       [pre-commit.ci_status] [License]
+      Singer Tap for the [Census Operational Analytics Platform](https://
        www.getcensus.com/). Built with the [Meltano Singer SDK](https://
-                             sdk.meltano.com).\n\n
-\n\n## Capabilities\n\n* `catalog`\n* `state`\n* `discover`\n* `about`\n*
-`stream-maps`\n* `schema-flattening`\n\n## Settings\n\n| Setting | Required |
-Default | Description |\n|:--------------------|:--------:|:-------:|:---------
----|\n| api_token | True | None | Auth token for getcensus.com API |\n|
-stream_maps | False | None | Config object for stream maps capability. |\n|
-stream_map_config | False | None | User-defined config values to be used within
-map expressions. |\n| flattening_enabled | False | None | \'True\' to enable
-schema flattening and automatically expand nested properties. |\n|
-flattening_max_depth| False | None | The max depth to flatten schemas. |\n\nA
-full list of supported settings and capabilities is available by running: `tap-
-getcensus --about`\n\n## Streams\n\n| Stream | Replication Method | Replication
-Key | Primary Key | Documentation |\n|:----------------------|:----------------
---:|:---------------:|:-----------:|:-------------:|\n| `syncs` | Full Table |
-None | id | https://docs.getcensus.com/basics/api/syncs#get-syncs |\n|
-`sync_runs` | Full Table | None | id | https://docs.getcensus.com/basics/api/
-sync-runs#get-syncs-id-sync_runs |\n| `destinations` | Full Table | None | id |
-https://docs.getcensus.com/basics/api/destinations#get-destinations |\n|
-`destination_objects` | Full Table | None | id | https://docs.getcensus.com/
-basics/api/destination-objects#get-destinations-id-objects |\n| `sources` |
-Full Table | None | id | https://docs.getcensus.com/basics/api/sources#get-
-sources |\n| `source_objects` | Full Table | None | id | https://
-docs.getcensus.com/basics/api/source-objects#get-sources-id-objects |\n\nThe
-full catalog is available by running: `tap-getcensus --discover`\n\n### Source
-Authentication and Authorization\n\nSee the [API docs](https://
-docs.getcensus.com/basics/api#getting-api-access).\n\n## Usage\n\nYou can
+                               sdk.meltano.com).
+## Capabilities * `catalog` * `state` * `discover` * `about` * `stream-maps` *
+`schema-flattening` ## Settings | Setting | Required | Default | Description |
+|:--------------------|:--------:|:-------:|:------------| | api_token | True |
+None | Auth token for getcensus.com API | | stream_maps | False | None | Config
+object for stream maps capability. | | stream_map_config | False | None | User-
+defined config values to be used within map expressions. | | flattening_enabled
+| False | None | 'True' to enable schema flattening and automatically expand
+nested properties. | | flattening_max_depth| False | None | The max depth to
+flatten schemas. | A full list of supported settings and capabilities is
+available by running: `tap-getcensus --about` ## Streams | Stream | Replication
+Method | Replication Key | Primary Key | Documentation | |:--------------------
+--|:------------------:|:---------------:|:-----------:|:-------------:| |
+`syncs` | Full Table | None | id | https://docs.getcensus.com/basics/api/
+syncs#get-syncs | | `sync_runs` | Full Table | None | id | https://
+docs.getcensus.com/basics/api/sync-runs#get-syncs-id-sync_runs | |
+`destinations` | Full Table | None | id | https://docs.getcensus.com/basics/
+api/destinations#get-destinations | | `destination_objects` | Full Table | None
+| id | https://docs.getcensus.com/basics/api/destination-objects#get-
+destinations-id-objects | | `sources` | Full Table | None | id | https://
+docs.getcensus.com/basics/api/sources#get-sources | | `source_objects` | Full
+Table | None | id | https://docs.getcensus.com/basics/api/source-objects#get-
+sources-id-objects | The full catalog is available by running: `tap-getcensus -
+-discover` ### Source Authentication and Authorization See the [API docs]
+(https://docs.getcensus.com/basics/api#getting-api-access). ## Usage You can
 easily run `tap-getcensus` by itself or in a pipeline using [Meltano](https://
-meltano.com/).\n\n### Executing the Tap Directly\n\n```bash\ntap-getcensus --
-version\ntap-getcensus --help\ntap-getcensus --config CONFIG --discover > ./
-catalog.json\n```\n\n## Developer Resources\n\n- [ ] `Developer TODO:` As a
-first step, scan the entire project for the text "`TODO:`" and complete any
-recommended steps, deleting the "TODO" references once completed.\n\n###
-Initialize your Development Environment\n\n```bash\npipx install poetry\npoetry
-install\n```\n\n### Create and Run Tests\n\nCreate tests within the `tests`
-subfolder and then run:\n\n```bash\npoetry run pytest\n```\n\nYou can also test
-the `tap-getcensus` CLI interface directly using `poetry run`:
-\n\n```bash\npoetry run tap-getcensus --help\n```\n\n### Testing with [Meltano]
-(https://www.meltano.com)\n\n_**Note:** This tap will work in any Singer
-environment and does not require Meltano.\nExamples here are for convenience
-and to streamline end-to-end orchestration scenarios._\n\nYour project comes
-with a custom `meltano.yml` project file already created. Open the
-`meltano.yml` and follow any _"TODO"_ items listed in\nthe file.\n\nNext,
-install Meltano (if you haven\'t already) and any needed plugins:\n\n```bash\n#
-Install meltano\npipx install meltano\n# Initialize meltano within this
-directory\ncd tap-getcensus\nmeltano install\n```\n\nNow you can test and
-orchestrate using Meltano:\n\n```bash\n# Test invocation:\nmeltano invoke tap-
-getcensus --version\n# OR run a test `elt` pipeline:\nmeltano elt tap-getcensus
-target-jsonl\n```\n\n### SDK Dev Guide\n\nSee the [dev guide](https://
-sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use
-the SDK to\ndevelop your own taps and targets.\n', 'author': 'Edgar RamÃ­rez-
-MondragÃ³n', 'author_email': 'edgarrm358@gmail.com', 'maintainer': 'Edgar
-RamÃ­rez-MondragÃ³n', 'maintainer_email': 'edgarrm358@gmail.com', 'url':
-'https://github.com/edgarrmondragon/tap-getcensus', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'entry_points': entry_points, 'python_requires': '>=3.7.1,<3.12', } setup
-(**setup_kwargs)
+meltano.com/). ### Executing the Tap Directly ```bash tap-getcensus --version
+tap-getcensus --help tap-getcensus --config CONFIG --discover > ./catalog.json
+``` ## Developer Resources ### Initialize your Development Environment ```bash
+pipx install poetry poetry install ``` ### Create and Run Tests Create tests
+within the `tests` subfolder and then run: ```bash poetry run pytest ``` You
+can also test the `tap-getcensus` CLI interface directly using `poetry run`:
+```bash poetry run tap-getcensus --help ``` ### Testing with [Meltano](https://
+www.meltano.com) _**Note:** This tap will work in any Singer environment and
+does not require Meltano. Examples here are for convenience and to streamline
+end-to-end orchestration scenarios._ Your project comes with a custom
+`meltano.yml` project file already created. Install Meltano (if you haven't
+already) and any needed plugins: ```bash # Install meltano pipx install meltano
+# Update all plugin definitions meltano lock --update --all # Initialize
+meltano within this directory cd tap-getcensus meltano install ``` Now you can
+test and orchestrate using Meltano: ```bash # Test invocation: meltano invoke
+tap-getcensus --version # OR run a pipeline: meltano run tap-getcensus target-
+jsonl ``` ### SDK Dev Guide See the [dev guide](https://sdk.meltano.com/en/
+latest/dev_guide.html) for more instructions on how to use the SDK to develop
+your own taps and targets.
```

