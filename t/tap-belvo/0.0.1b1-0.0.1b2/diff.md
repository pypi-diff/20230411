# Comparing `tmp/tap_belvo-0.0.1b1.tar.gz` & `tmp/tap_belvo-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_belvo-0.0.1b1.tar", max compression
+gzip compressed data, was "tap_belvo-0.0.1b2.tar", max compression
```

## Comparing `tap_belvo-0.0.1b1.tar` & `tap_belvo-0.0.1b2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1068 2022-12-08 22:41:28.908862 tap_belvo-0.0.1b1/LICENSE
--rw-r--r--   0        0        0     3135 2022-12-08 22:41:28.908862 tap_belvo-0.0.1b1/README.md
--rw-r--r--   0        0        0     3020 2022-12-08 22:41:47.816880 tap_belvo-0.0.1b1/pyproject.toml
--rw-r--r--   0        0        0       80 2022-12-08 22:41:28.908862 tap_belvo-0.0.1b1/tap_belvo/__init__.py
--rw-r--r--   0        0        0      110 2022-12-08 22:41:28.908862 tap_belvo-0.0.1b1/tap_belvo/__main__.py
--rw-r--r--   0        0        0     5028 2022-12-08 22:41:28.908862 tap_belvo-0.0.1b1/tap_belvo/client.py
--rw-r--r--   0        0        0  1025531 2022-12-08 22:41:28.912862 tap_belvo-0.0.1b1/tap_belvo/openapi/BelvoOpenFinanceApiSpec.json
--rw-r--r--   0        0        0       89 2022-12-08 22:41:28.912862 tap_belvo-0.0.1b1/tap_belvo/openapi/__init__.py
--rw-r--r--   0        0        0      936 2022-12-08 22:41:28.912862 tap_belvo-0.0.1b1/tap_belvo/streams/__init__.py
--rw-r--r--   0        0        0     2400 2022-12-08 22:41:28.912862 tap_belvo-0.0.1b1/tap_belvo/streams/banking.py
--rw-r--r--   0        0        0      758 2022-12-08 22:41:28.912862 tap_belvo-0.0.1b1/tap_belvo/streams/enrichment.py
--rw-r--r--   0        0        0     1591 2022-12-08 22:41:28.912862 tap_belvo-0.0.1b1/tap_belvo/streams/fiscal.py
--rw-r--r--   0        0        0      903 2022-12-08 22:41:28.912862 tap_belvo-0.0.1b1/tap_belvo/streams/links.py
--rw-r--r--   0        0        0     1888 2022-12-08 22:41:28.912862 tap_belvo-0.0.1b1/tap_belvo/tap.py
--rw-r--r--   0        0        0     4195 1970-01-01 00:00:00.000000 tap_belvo-0.0.1b1/setup.py
--rw-r--r--   0        0        0     4111 1970-01-01 00:00:00.000000 tap_belvo-0.0.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-11 06:32:45.211947 tap_belvo-0.0.1b2/LICENSE
+-rw-r--r--   0        0        0     3135 2023-04-11 06:32:45.211947 tap_belvo-0.0.1b2/README.md
+-rw-r--r--   0        0        0     2171 2023-04-11 06:33:06.220157 tap_belvo-0.0.1b2/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-11 06:32:45.211947 tap_belvo-0.0.1b2/tap_belvo/__init__.py
+-rw-r--r--   0        0        0      110 2023-04-11 06:32:45.211947 tap_belvo-0.0.1b2/tap_belvo/__main__.py
+-rw-r--r--   0        0        0     4417 2023-04-11 06:32:45.211947 tap_belvo-0.0.1b2/tap_belvo/client.py
+-rw-r--r--   0        0        0  1025531 2023-04-11 06:32:45.215947 tap_belvo-0.0.1b2/tap_belvo/openapi/BelvoOpenFinanceApiSpec.json
+-rw-r--r--   0        0        0      739 2023-04-11 06:32:45.215947 tap_belvo-0.0.1b2/tap_belvo/openapi/__init__.py
+-rw-r--r--   0        0        0      936 2023-04-11 06:32:45.215947 tap_belvo-0.0.1b2/tap_belvo/streams/__init__.py
+-rw-r--r--   0        0        0     2438 2023-04-11 06:32:45.215947 tap_belvo-0.0.1b2/tap_belvo/streams/banking.py
+-rw-r--r--   0        0        0      758 2023-04-11 06:32:45.215947 tap_belvo-0.0.1b2/tap_belvo/streams/enrichment.py
+-rw-r--r--   0        0        0     1591 2023-04-11 06:32:45.215947 tap_belvo-0.0.1b2/tap_belvo/streams/fiscal.py
+-rw-r--r--   0        0        0      903 2023-04-11 06:32:45.215947 tap_belvo-0.0.1b2/tap_belvo/streams/links.py
+-rw-r--r--   0        0        0     1924 2023-04-11 06:32:45.215947 tap_belvo-0.0.1b2/tap_belvo/tap.py
+-rw-r--r--   0        0        0     4063 1970-01-01 00:00:00.000000 tap_belvo-0.0.1b2/PKG-INFO
```

### Comparing `tap_belvo-0.0.1b1/LICENSE` & `tap_belvo-0.0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b1/README.md` & `tap_belvo-0.0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b1/pyproject.toml` & `tap_belvo-0.0.1b2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-belvo"
-version = "0.0.1b1"
+version = "0.0.1b2"
 description = "`tap-belvo` is a Singer tap for Belvo, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 keywords = [
   "ELT",
   "singer.io",
   "Belvo",
 ]
@@ -12,22 +12,19 @@
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-belvo"
 repository = "https://github.com/edgarrmondragon/tap-belvo"
 documentation = "https://github.com/edgarrmondragon/tap-belvo#readme"
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
-singer-sdk = "0.15.0"
-belvo-python = "^0.35.0"
-requests-cache = "^0.9.7"
+singer-sdk = "0.23.0"
+requests-cache = ">=0.9.7,<1.1.0"
 
 [tool.poetry.dev-dependencies]
-mypy = ">=0.991"
-pytest = "^7.2.0"
-types-requests = ">=2.28.11"
+pytest = "^7.3.0"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3 # Vertical Hanging Indent
 use_parentheses = true
 include_trailing_comma = true
 src_paths = "tap_belvo"
@@ -67,69 +64,29 @@
     {%- endif -%}
 """
 metadata = true
 style = "pep440"
 vcs = "git"
 
 [tool.ruff]
-extend-ignore = [
-  # equivalent to `--docstring-convention=google`
-  "D203",
-  "D204",
-  "D213",
-  "D215",
-  "D400",
-  "D404",
-  "D406",
-  "D407",
-  "D408",
-  "D409",
-  "D413",
-]
 ignore = [
-  "ANN101",
+  "ANN101", # missing-type-self
+  "DJ", # flake8-django
 ]
 line-length = 88
-select = [
-  "F", # Pyflakes
-  "E", # pycodestyle (error)
-  "W", # pycodestyle (warning)
-  "C9", # mccabe
-  "I0", # isort
-  "D", # pydocstyle (with google style docstring convention)
-  "UP", # pyupgrade
-  "N8", # pep8-naming
-  "YTT", # flake8-2020
-  "ANN", # flake8-annotations
-  "S", # flake8-bandit
-  "BLE", # flake8-blind-except
-  "FBT", # flake8-boolean-trap
-  "B0", # flake8-bugbear
-  "A0", # flake8-builtins
-  "C4", # flake8-comprehensions
-  "T1", # flake8-debugger
-  "ICN", # flake8-import-conventions
-  "T2", # flake8-print
-  "Q", # flake8-quotes
-  "RET", # flake8-return
-  "TID", # flake8-tidy-imports
-  "ARG", # flake8-unused-arguments
-  "ERA", # eradicate
-  "PGH", # pygrep-hooks
-  "PLC", # Pylint
-  "PLE", # Pylint
-  "PLR", # Pylint
-  "PLW", # Pylint
-  "RUF", # Ruff-specific rules
-]
+select = ["ALL"]
 src = ["tap_belvo", "tests"]
 target-version = "py37"
 
 [tool.ruff.per-file-ignores]
 "noxfile.py" = ["ANN"]
 "tests/*" = [
-  "ANN201",
-  "S101",
+  "ANN201", # missing-return-type-public-function
+  "S101", # assert
+  "SLF001", # private-member-access
 ]
 
 [tool.ruff.isort]
 known-first-party = ["tap_belvo"]
+
+[tool.ruff.pydocstyle]
+convention = "google"
```

### Comparing `tap_belvo-0.0.1b1/tap_belvo/client.py` & `tap_belvo-0.0.1b2/tap_belvo/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,31 @@
 """REST client handling, including BelvoStream base class."""
 
 from __future__ import annotations
 
-import json
-import logging
-import sys
 from abc import ABCMeta, abstractmethod
-from functools import lru_cache
 from typing import TYPE_CHECKING, Any
 from urllib.parse import ParseResult, parse_qsl
 
 from requests_cache import install_cache
 from singer_sdk import RESTStream
 from singer_sdk._singerlib import resolve_schema_references
 from singer_sdk.authenticators import BasicAuthenticator
 from singer_sdk.helpers._typing import is_date_or_datetime_type
 from singer_sdk.pagination import BaseHATEOASPaginator
 
-from tap_belvo import openapi
-
-if sys.version_info >= (3, 9):
-    import importlib.resources as importlib_resources
-else:
-    import importlib_resources
-
+from tap_belvo.openapi import load_openapi
 
 if TYPE_CHECKING:
     from requests import Response
 
 
-OPENAPI_FILENAME = "BelvoOpenFinanceApiSpec.json"
 PAGE_SIZE = 1000
 
 install_cache("tap_belvo_cache", backend="sqlite", expire_after=3600)
-logger = logging.getLogger(__name__)
-
-
-@lru_cache(maxsize=None)
-def load_openapi() -> dict[str, Any]:
-    """Load the OpenAPI specification from the package.
-
-    Returns:
-        The OpenAPI specification as a dict.
-    """
-    logger.info("Loading OpenAPI spec from package")
-    with importlib_resources.files(openapi).joinpath(OPENAPI_FILENAME).open() as f:
-        return json.load(f)
 
 
 class BelvoPaginator(BaseHATEOASPaginator):
     """Belvo API paginator class."""
 
     def get_next_url(self, response: Response) -> str | None:
         """Get the next URL from the response.
@@ -122,15 +98,15 @@
         Args:
             context: Stream sync context.
             next_page_token: Next offset.
 
         Returns:
             Mapping of URL query parameters.
         """
-        params: dict = {
+        params: dict[str, Any] = {
             "page": 1,
             "page_size": PAGE_SIZE,
         }
 
         if next_page_token:
             params.update(parse_qsl(next_page_token.query))
```

### Comparing `tap_belvo-0.0.1b1/tap_belvo/openapi/BelvoOpenFinanceApiSpec.json` & `tap_belvo-0.0.1b2/tap_belvo/openapi/BelvoOpenFinanceApiSpec.json`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b1/tap_belvo/streams/__init__.py` & `tap_belvo-0.0.1b2/tap_belvo/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b1/tap_belvo/streams/banking.py` & `tap_belvo-0.0.1b2/tap_belvo/streams/banking.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Stream type classes for tap-belvo."""
 
 from __future__ import annotations
 
-from typing import Any
-from urllib.parse import ParseResult
+from typing import TYPE_CHECKING, Any
 
 from tap_belvo.client import BelvoStream
 from tap_belvo.streams.links import Links
 
+if TYPE_CHECKING:
+    from urllib.parse import ParseResult
+
 
 class Accounts(BelvoStream):
     """Accounts stream."""
 
     name = "banking_accounts"
     path = "/api/accounts"
     primary_keys = ["id"]
```

### Comparing `tap_belvo-0.0.1b1/tap_belvo/streams/enrichment.py` & `tap_belvo-0.0.1b2/tap_belvo/streams/enrichment.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b1/tap_belvo/streams/fiscal.py` & `tap_belvo-0.0.1b2/tap_belvo/streams/fiscal.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b1/tap_belvo/streams/links.py` & `tap_belvo-0.0.1b2/tap_belvo/streams/links.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b1/tap_belvo/tap.py` & `tap_belvo-0.0.1b2/tap_belvo/tap.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,16 +51,16 @@
         return [
             links.Links(self),
             links.Institutions(self),
             banking.Accounts(self),
             banking.Transactions(self),
             banking.Balances(self),
             banking.Owners(self),
-            banking.InvestmentPortfolios(self),
-            banking.ReceivableTransactions(self),
+            # banking.InvestmentPortfolios(self),  # noqa: ERA001
+            # banking.ReceivableTransactions(self),  # noqa: ERA001
             enrichment.Incomes(self),
             enrichment.RecurringExpenses(self),
             enrichment.RiskInsights(self),
             fiscal.Invoices(self),
             fiscal.TaxComplianceStatuses(self),
             fiscal.TaxRetentions(self),
             fiscal.TaxStatuses(self),
```

### Comparing `tap_belvo-0.0.1b1/setup.py` & `tap_belvo-0.0.1b2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,125 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tap-belvo
+Version: 0.0.1b2
+Summary: `tap-belvo` is a Singer tap for Belvo, built with the Meltano SDK for Singer Taps.
+Home-page: https://github.com/edgarrmondragon/tap-belvo
+License: Apache 2.0
+Keywords: ELT,singer.io,Belvo
+Author: Edgar Ramírez-Mondragón
+Author-email: edgarrm358@gmail.com
+Requires-Python: >=3.7.1,<3.12
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests-cache (>=0.9.7,<1.1.0)
+Requires-Dist: singer-sdk (==0.23.0)
+Project-URL: Documentation, https://github.com/edgarrmondragon/tap-belvo#readme
+Project-URL: Repository, https://github.com/edgarrmondragon/tap-belvo
+Description-Content-Type: text/markdown
 
-packages = \
-['tap_belvo', 'tap_belvo.openapi', 'tap_belvo.streams']
+# `tap-belvo`
 
-package_data = \
-{'': ['*']}
+Singer tap for Belvo.
 
-install_requires = \
-['belvo-python>=0.35.0,<0.36.0',
- 'requests-cache>=0.9.7,<0.10.0',
- 'singer-sdk==0.15.0']
-
-entry_points = \
-{'console_scripts': ['tap-belvo = tap_belvo.tap:TapBelvo.cli']}
-
-setup_kwargs = {
-    'name': 'tap-belvo',
-    'version': '0.0.1b1',
-    'description': '`tap-belvo` is a Singer tap for Belvo, built with the Meltano SDK for Singer Taps.',
-    'long_description': '# `tap-belvo`\n\nSinger tap for Belvo.\n\nBuilt with the [Meltano Singer SDK](https://sdk.meltano.com).\n\n## Capabilities\n\n* `catalog`\n* `state`\n* `discover`\n* `about`\n* `stream-maps`\n* `schema-flattening`\n\n## Settings\n\n| Setting             | Required | Default | Description |\n|:--------------------|:--------:|:-------:|:------------|\n| secret_id           | True     | None    | Belvo API secret ID. |\n| password            | True     | None    | Belvo API password. |\n| start_date          | False    | None    | Earliest datetime to get data from |\n| base_url            | False    | https://development.belvo.com | Base URL for the Belvo API |\n| stream_maps         | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |\n| stream_map_config   | False    | None    | User-defined config values to be used within map expressions. |\n| flattening_enabled  | False    | None    | \'True\' to enable schema flattening and automatically expand nested properties. |\n| flattening_max_depth| False    | None    | The max depth to flatten schemas. |\n\nA full list of supported settings and capabilities is available by running: `tap-belvo --about`\n\n### Source Authentication and Authorization\n\n- [ ] `Developer TODO:` If your tap requires special access on the source system, or any special authentication requirements, provide those here.\n\n## Usage\n\nYou can easily run `tap-belvo` by itself or in a pipeline using [Meltano](https://meltano.com/).\n\n### Executing the Tap Directly\n\n```bash\ntap-belvo --version\ntap-belvo --help\ntap-belvo --config CONFIG --discover > ./catalog.json\n```\n\n## Developer Resources\n\n- [ ] `Developer TODO:` As a first step, scan the entire project for the text "`TODO:`" and complete any recommended steps, deleting the "TODO" references once completed.\n\n### Initialize your Development Environment\n\n```bash\npipx install poetry\npoetry install\n```\n\n### Create and Run Tests\n\nCreate tests within the `tests` subfolder and then run:\n\n```bash\npoetry run pytest\n```\n\nYou can also test the `tap-belvo` CLI interface directly using `poetry run`:\n\n```bash\npoetry run tap-belvo --help\n```\n\n### Testing with [Meltano](https://www.meltano.com)\n\n_**Note:** This tap will work in any Singer environment and does not require Meltano.\nExamples here are for convenience and to streamline end-to-end orchestration scenarios._\n\nYour project comes with a custom `meltano.yml` project file already created. Open the `meltano.yml` and follow any _"TODO"_ items listed in\nthe file.\n\nNext, install Meltano (if you haven\'t already) and any needed plugins:\n\n```bash\n# Install meltano\npipx install meltano\n# Initialize meltano within this directory\ncd tap-belvo\nmeltano install\n```\n\nNow you can test and orchestrate using Meltano:\n\n```bash\n# Test invocation:\nmeltano invoke tap-belvo --version\n# OR run a test `elt` pipeline:\nmeltano elt tap-belvo target-jsonl\n```\n\n### SDK Dev Guide\n\nSee the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the SDK to\ndevelop your own taps and targets.\n',
-    'author': 'Edgar Ramírez-Mondragón',
-    'author_email': 'edgarrm358@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/edgarrmondragon/tap-belvo',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<3.12',
-}
+Built with the [Meltano Singer SDK](https://sdk.meltano.com).
 
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
+| secret_id           | True     | None    | Belvo API secret ID. |
+| password            | True     | None    | Belvo API password. |
+| start_date          | False    | None    | Earliest datetime to get data from |
+| base_url            | False    | https://development.belvo.com | Base URL for the Belvo API |
+| stream_maps         | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |
+| stream_map_config   | False    | None    | User-defined config values to be used within map expressions. |
+| flattening_enabled  | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |
+| flattening_max_depth| False    | None    | The max depth to flatten schemas. |
+
+A full list of supported settings and capabilities is available by running: `tap-belvo --about`
+
+### Source Authentication and Authorization
+
+- [ ] `Developer TODO:` If your tap requires special access on the source system, or any special authentication requirements, provide those here.
+
+## Usage
+
+You can easily run `tap-belvo` by itself or in a pipeline using [Meltano](https://meltano.com/).
+
+### Executing the Tap Directly
+
+```bash
+tap-belvo --version
+tap-belvo --help
+tap-belvo --config CONFIG --discover > ./catalog.json
+```
+
+## Developer Resources
+
+- [ ] `Developer TODO:` As a first step, scan the entire project for the text "`TODO:`" and complete any recommended steps, deleting the "TODO" references once completed.
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
+You can also test the `tap-belvo` CLI interface directly using `poetry run`:
+
+```bash
+poetry run tap-belvo --help
+```
+
+### Testing with [Meltano](https://www.meltano.com)
+
+_**Note:** This tap will work in any Singer environment and does not require Meltano.
+Examples here are for convenience and to streamline end-to-end orchestration scenarios._
+
+Your project comes with a custom `meltano.yml` project file already created. Open the `meltano.yml` and follow any _"TODO"_ items listed in
+the file.
+
+Next, install Meltano (if you haven't already) and any needed plugins:
+
+```bash
+# Install meltano
+pipx install meltano
+# Initialize meltano within this directory
+cd tap-belvo
+meltano install
+```
+
+Now you can test and orchestrate using Meltano:
+
+```bash
+# Test invocation:
+meltano invoke tap-belvo --version
+# OR run a test `elt` pipeline:
+meltano elt tap-belvo target-jsonl
+```
+
+### SDK Dev Guide
+
+See the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the SDK to
+develop your own taps and targets.
 
-setup(**setup_kwargs)
```

