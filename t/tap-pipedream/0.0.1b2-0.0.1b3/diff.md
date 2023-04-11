# Comparing `tmp/tap_pipedream-0.0.1b2.tar.gz` & `tmp/tap_pipedream-0.0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_pipedream-0.0.1b2.tar", max compression
+gzip compressed data, was "tap_pipedream-0.0.1b3.tar", max compression
```

## Comparing `tap_pipedream-0.0.1b2.tar` & `tap_pipedream-0.0.1b3.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     3120 2023-02-09 01:58:48.417662 tap_pipedream-0.0.1b2/README.md
--rw-r--r--   0        0        0     1816 2023-02-09 01:59:14.055526 tap_pipedream-0.0.1b2/pyproject.toml
--rw-r--r--   0        0        0       84 2023-02-09 01:58:48.421662 tap_pipedream-0.0.1b2/tap_pipedream/__init__.py
--rw-r--r--   0        0        0      122 2023-02-09 01:58:48.421662 tap_pipedream-0.0.1b2/tap_pipedream/__main__.py
--rw-r--r--   0        0        0     1543 2023-02-09 01:58:48.421662 tap_pipedream-0.0.1b2/tap_pipedream/client.py
--rw-r--r--   0        0        0     8154 2023-02-09 01:58:48.421662 tap_pipedream-0.0.1b2/tap_pipedream/streams.py
--rw-r--r--   0        0        0     1511 2023-02-09 01:58:48.421662 tap_pipedream-0.0.1b2/tap_pipedream/tap.py
--rw-r--r--   0        0        0     4144 1970-01-01 00:00:00.000000 tap_pipedream-0.0.1b2/setup.py
--rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 tap_pipedream-0.0.1b2/PKG-INFO
+-rw-r--r--   0        0        0     3120 2023-04-11 06:26:38.894223 tap_pipedream-0.0.1b3/README.md
+-rw-r--r--   0        0        0     2266 2023-04-11 06:27:10.854855 tap_pipedream-0.0.1b3/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-04-11 06:26:38.898223 tap_pipedream-0.0.1b3/tap_pipedream/__init__.py
+-rw-r--r--   0        0        0      122 2023-04-11 06:26:38.898223 tap_pipedream-0.0.1b3/tap_pipedream/__main__.py
+-rw-r--r--   0        0        0     1573 2023-04-11 06:26:38.898223 tap_pipedream-0.0.1b3/tap_pipedream/client.py
+-rw-r--r--   0        0        0     8233 2023-04-11 06:26:38.898223 tap_pipedream-0.0.1b3/tap_pipedream/streams.py
+-rw-r--r--   0        0        0     1512 2023-04-11 06:26:38.898223 tap_pipedream-0.0.1b3/tap_pipedream/tap.py
+-rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 tap_pipedream-0.0.1b3/PKG-INFO
```

### Comparing `tap_pipedream-0.0.1b2/README.md` & `tap_pipedream-0.0.1b3/README.md`

 * *Files identical despite different names*

### Comparing `tap_pipedream-0.0.1b2/pyproject.toml` & `tap_pipedream-0.0.1b3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-pipedream"
-version = "0.0.1b2"
+version = "0.0.1b3"
 description = "`tap-pipedream` is a Singer tap for Pipedream, built with the Meltano SDK for Singer Taps."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 maintainers = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-pipedream"
 repository = "https://github.com/edgarrmondragon/tap-pipedream"
@@ -13,15 +13,15 @@
   "ELT",
   "singer.io",
   "Pipedream",
 ]
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
-singer-sdk = "0.19.0"
+singer-sdk = "0.23.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3 # Vertical Hanging Indent
@@ -62,7 +62,31 @@
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
+  "ANN101", # missing-type-self
+  "DJ", # flake8-django
+]
+line-length = 88
+select = ["ALL"]
+src = ["tap_pipedream", "tests"]
+target-version = "py37"
+
+[tool.ruff.per-file-ignores]
+"noxfile.py" = ["ANN"]
+"tests/*" = [
+  "ANN201", # missing-return-type-public-function
+  "S101", # assert
+  "SLF001", # private-member-access
+]
+
+[tool.ruff.isort]
+known-first-party = ["tap_pipedream"]
+
+[tool.ruff.pydocstyle]
+convention = "google"
```

### Comparing `tap_pipedream-0.0.1b2/tap_pipedream/client.py` & `tap_pipedream-0.0.1b3/tap_pipedream/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class PipedreamStream(RESTStream):
     """Pipedream stream class."""
 
     url_base = "https://api.pipedream.com/v1"
     records_jsonpath = "$.data[*]"
-    next_page_token_jsonpath = "$.page_info.end_cursor"
+    next_page_token_jsonpath = "$.page_info.end_cursor"  # noqa: S105
 
     page_size = 100
 
     @property
     def authenticator(self) -> BearerTokenAuthenticator:
         """Get an authenticator object.
 
@@ -39,15 +39,15 @@
         """
         headers = {}
         headers["User-Agent"] = f"{self.tap_name}/{self._tap.plugin_version}"
         return headers
 
     def get_url_params(
         self,
-        context: dict | None,
+        context: dict | None,  # noqa: ARG002
         next_page_token: str | None,
     ) -> dict[str, Any]:
         """Get URL query parameters.
 
         Args:
             context: Stream sync context.
             next_page_token: Next offset.
```

### Comparing `tap_pipedream-0.0.1b2/tap_pipedream/streams.py` & `tap_pipedream-0.0.1b3/tap_pipedream/streams.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,15 +129,19 @@
                     "emitAsArray",
                     th.BooleanType,
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
         """Return a dictionary of child context objects.
 
         Args:
             record: A dictionary representing one record from the API response.
             context: A dictionary of any context objects from the parent stream.
 
         Returns:
@@ -160,16 +164,16 @@
         th.Property("e", th.StringType),
         th.Property("ts", th.IntegerType),
         th.Property("key", th.StringType),
     ).to_dict()
 
     def get_url_params(
         self,
-        context: dict | None,
-        next_page_token: str | None,
+        context: dict | None,  # noqa: ARG002
+        next_page_token: str | None,  # noqa: ARG002
     ) -> dict[str, Any]:
         """Return a dictionary of values to be used in URL parameterization.
 
         Args:
             context: A dictionary of any context objects from the parent stream.
             next_page_token: A string representing the next page of results.
```

### Comparing `tap_pipedream-0.0.1b2/tap_pipedream/tap.py` & `tap_pipedream-0.0.1b3/tap_pipedream/tap.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,11 +47,11 @@
 
         if self.config.get("organizations"):
             tap_streams.extend(
                 [
                     streams.OrganizationSources(self),
                     streams.OrganizationSubscriptions(self),
                     streams.OrganizationSourceEvents(self),
-                ]
+                ],
             )
 
         return tap_streams
```

### Comparing `tap_pipedream-0.0.1b2/setup.py` & `tap_pipedream-0.0.1b3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,130 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tap-pipedream
+Version: 0.0.1b3
+Summary: `tap-pipedream` is a Singer tap for Pipedream, built with the Meltano SDK for Singer Taps.
+Home-page: https://github.com/edgarrmondragon/tap-pipedream
+License: Apache-2.0
+Keywords: ELT,singer.io,Pipedream
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
+Project-URL: Documentation, https://github.com/edgarrmondragon/tap-pipedream#readme
+Project-URL: Repository, https://github.com/edgarrmondragon/tap-pipedream
+Description-Content-Type: text/markdown
+
+<div align="center">
+
+# tap-pipedream
+
+<div>
+  <a href="https://results.pre-commit.ci/latest/github/edgarrmondragon/tap-pipedream/main">
+    <img alt="pre-commit.ci status" src="https://results.pre-commit.ci/badge/github/edgarrmondragon/tap-pipedream/main.svg"/>
+  </a>
+  <a href="https://github.com/edgarrmondragon/tap-pipedream/blob/main/LICENSE">
+    <img alt="License" src="https://img.shields.io/github/license/edgarrmondragon/tap-pipedream"/>
+  </a>
+</div>
+
+Singer tap for Pipedream. Built with the [Meltano Singer SDK](https://sdk.meltano.com).
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
+| token               | True     | None    | API Token for Pipedream |
+| start_date          | False    | None    | Earliest timestamp to get data from |
+| stream_maps         | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |
+| stream_map_config   | False    | None    | User-defined config values to be used within map expressions. |
+| flattening_enabled  | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |
+| flattening_max_depth| False    | None    | The max depth to flatten schemas. |
+
+A full list of supported settings and capabilities is available by running: `tap-pipedream --about`
+
+### Source Authentication and Authorization
+
+To generate an API key, follow the instructions [in the docs](https://pipedream.com/docs/api/auth/#pipedream-api-key).
+
+## Usage
+
+You can easily run `tap-pipedream` by itself or in a pipeline using [Meltano](https://meltano.com/).
+
+### Executing the Tap Directly
+
+```bash
+tap-pipedream --version
+tap-pipedream --help
+tap-pipedream --config CONFIG --discover > ./catalog.json
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
+You can also test the `tap-pipedream` CLI interface directly using `poetry run`:
+
+```bash
+poetry run tap-pipedream --help
+```
+
+### Testing with [Meltano](https://www.meltano.com)
+
+_**Note:** This tap will work in any Singer environment and does not require Meltano.
+Examples here are for convenience and to streamline end-to-end orchestration scenarios._
+
+Install Meltano (if you haven't already) and any needed plugins:
+
+```bash
+# Install meltano
+pipx install meltano
+# Initialize meltano within this directory
+cd tap-pipedream
+meltano install
+```
+
+Now you can test and orchestrate using Meltano:
+
+```bash
+# Test invocation:
+meltano invoke tap-pipedream --version
+# OR run a test `elt` pipeline:
+meltano elt tap-pipedream target-jsonl
+```
 
-packages = \
-['tap_pipedream']
+### SDK Dev Guide
 
-package_data = \
-{'': ['*']}
+See the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the SDK to
+develop your own taps and targets.
 
-install_requires = \
-['singer-sdk==0.19.0']
-
-entry_points = \
-{'console_scripts': ['tap-pipedream = tap_pipedream.tap:TapPipedream.cli']}
-
-setup_kwargs = {
-    'name': 'tap-pipedream',
-    'version': '0.0.1b2',
-    'description': '`tap-pipedream` is a Singer tap for Pipedream, built with the Meltano SDK for Singer Taps.',
-    'long_description': '<div align="center">\n\n# tap-pipedream\n\n<div>\n  <a href="https://results.pre-commit.ci/latest/github/edgarrmondragon/tap-pipedream/main">\n    <img alt="pre-commit.ci status" src="https://results.pre-commit.ci/badge/github/edgarrmondragon/tap-pipedream/main.svg"/>\n  </a>\n  <a href="https://github.com/edgarrmondragon/tap-pipedream/blob/main/LICENSE">\n    <img alt="License" src="https://img.shields.io/github/license/edgarrmondragon/tap-pipedream"/>\n  </a>\n</div>\n\nSinger tap for Pipedream. Built with the [Meltano Singer SDK](https://sdk.meltano.com).\n\n</div>\n\n## Capabilities\n\n* `catalog`\n* `state`\n* `discover`\n* `about`\n* `stream-maps`\n* `schema-flattening`\n\n## Settings\n\n| Setting             | Required | Default | Description |\n|:--------------------|:--------:|:-------:|:------------|\n| token               | True     | None    | API Token for Pipedream |\n| start_date          | False    | None    | Earliest timestamp to get data from |\n| stream_maps         | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |\n| stream_map_config   | False    | None    | User-defined config values to be used within map expressions. |\n| flattening_enabled  | False    | None    | \'True\' to enable schema flattening and automatically expand nested properties. |\n| flattening_max_depth| False    | None    | The max depth to flatten schemas. |\n\nA full list of supported settings and capabilities is available by running: `tap-pipedream --about`\n\n### Source Authentication and Authorization\n\nTo generate an API key, follow the instructions [in the docs](https://pipedream.com/docs/api/auth/#pipedream-api-key).\n\n## Usage\n\nYou can easily run `tap-pipedream` by itself or in a pipeline using [Meltano](https://meltano.com/).\n\n### Executing the Tap Directly\n\n```bash\ntap-pipedream --version\ntap-pipedream --help\ntap-pipedream --config CONFIG --discover > ./catalog.json\n```\n\n## Developer Resources\n\n### Initialize your Development Environment\n\n```bash\npipx install poetry\npoetry install\n```\n\n### Create and Run Tests\n\nCreate tests within the `tests` subfolder and then run:\n\n```bash\npoetry run pytest\n```\n\nYou can also test the `tap-pipedream` CLI interface directly using `poetry run`:\n\n```bash\npoetry run tap-pipedream --help\n```\n\n### Testing with [Meltano](https://www.meltano.com)\n\n_**Note:** This tap will work in any Singer environment and does not require Meltano.\nExamples here are for convenience and to streamline end-to-end orchestration scenarios._\n\nInstall Meltano (if you haven\'t already) and any needed plugins:\n\n```bash\n# Install meltano\npipx install meltano\n# Initialize meltano within this directory\ncd tap-pipedream\nmeltano install\n```\n\nNow you can test and orchestrate using Meltano:\n\n```bash\n# Test invocation:\nmeltano invoke tap-pipedream --version\n# OR run a test `elt` pipeline:\nmeltano elt tap-pipedream target-jsonl\n```\n\n### SDK Dev Guide\n\nSee the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the SDK to\ndevelop your own taps and targets.\n',
-    'author': 'Edgar Ramírez-Mondragón',
-    'author_email': 'edgarrm358@gmail.com',
-    'maintainer': 'Edgar Ramírez-Mondragón',
-    'maintainer_email': 'edgarrm358@gmail.com',
-    'url': 'https://github.com/edgarrmondragon/tap-pipedream',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<3.12',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,50 +1,51 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['tap_pipedream'] package_data = \ {'': ['*']} install_requires = \ ['singer-
-sdk==0.19.0'] entry_points = \ {'console_scripts': ['tap-pipedream =
-tap_pipedream.tap:TapPipedream.cli']} setup_kwargs = { 'name': 'tap-pipedream',
-'version': '0.0.1b2', 'description': '`tap-pipedream` is a Singer tap for
-Pipedream, built with the Meltano SDK for Singer Taps.', 'long_description': '
-                            \n\n# tap-pipedream\n\n
-               \n \n_[pre-commit.ci_status]\n\n \n_[License]\n\n
-  \n\nSinger tap for Pipedream. Built with the [Meltano Singer SDK](https://
-                             sdk.meltano.com).\n\n
-\n\n## Capabilities\n\n* `catalog`\n* `state`\n* `discover`\n* `about`\n*
-`stream-maps`\n* `schema-flattening`\n\n## Settings\n\n| Setting | Required |
-Default | Description |\n|:--------------------|:--------:|:-------:|:---------
----|\n| token | True | None | API Token for Pipedream |\n| start_date | False |
-None | Earliest timestamp to get data from |\n| stream_maps | False | None |
-Config object for stream maps capability. For more information check out
-[Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |\n|
-stream_map_config | False | None | User-defined config values to be used within
-map expressions. |\n| flattening_enabled | False | None | \'True\' to enable
-schema flattening and automatically expand nested properties. |\n|
-flattening_max_depth| False | None | The max depth to flatten schemas. |\n\nA
-full list of supported settings and capabilities is available by running: `tap-
-pipedream --about`\n\n### Source Authentication and Authorization\n\nTo
-generate an API key, follow the instructions [in the docs](https://
-pipedream.com/docs/api/auth/#pipedream-api-key).\n\n## Usage\n\nYou can easily
-run `tap-pipedream` by itself or in a pipeline using [Meltano](https://
-meltano.com/).\n\n### Executing the Tap Directly\n\n```bash\ntap-pipedream --
-version\ntap-pipedream --help\ntap-pipedream --config CONFIG --discover > ./
-catalog.json\n```\n\n## Developer Resources\n\n### Initialize your Development
-Environment\n\n```bash\npipx install poetry\npoetry install\n```\n\n### Create
-and Run Tests\n\nCreate tests within the `tests` subfolder and then run:
-\n\n```bash\npoetry run pytest\n```\n\nYou can also test the `tap-pipedream`
-CLI interface directly using `poetry run`:\n\n```bash\npoetry run tap-pipedream
---help\n```\n\n### Testing with [Meltano](https://www.meltano.com)\n\n_**Note:
-** This tap will work in any Singer environment and does not require
-Meltano.\nExamples here are for convenience and to streamline end-to-end
-orchestration scenarios._\n\nInstall Meltano (if you haven\'t already) and any
-needed plugins:\n\n```bash\n# Install meltano\npipx install meltano\n#
-Initialize meltano within this directory\ncd tap-pipedream\nmeltano
-install\n```\n\nNow you can test and orchestrate using Meltano:\n\n```bash\n#
-Test invocation:\nmeltano invoke tap-pipedream --version\n# OR run a test `elt`
-pipeline:\nmeltano elt tap-pipedream target-jsonl\n```\n\n### SDK Dev
-Guide\n\nSee the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html)
-for more instructions on how to use the SDK to\ndevelop your own taps and
-targets.\n', 'author': 'Edgar RamÃ­rez-MondragÃ³n', 'author_email':
-'edgarrm358@gmail.com', 'maintainer': 'Edgar RamÃ­rez-MondragÃ³n',
-'maintainer_email': 'edgarrm358@gmail.com', 'url': 'https://github.com/
-edgarrmondragon/tap-pipedream', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'entry_points':
-entry_points, 'python_requires': '>=3.7.1,<3.12', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: tap-pipedream Version: 0.0.1b3 Summary: `tap-
+pipedream` is a Singer tap for Pipedream, built with the Meltano SDK for Singer
+Taps. Home-page: https://github.com/edgarrmondragon/tap-pipedream License:
+Apache-2.0 Keywords: ELT,singer.io,Pipedream Author: Edgar RamÃ­rez-MondragÃ³n
+Author-email: edgarrm358@gmail.com Maintainer: Edgar RamÃ­rez-MondragÃ³n
+Maintainer-email: edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Dist: singer-sdk (==0.23.0) Project-URL: Documentation,
+https://github.com/edgarrmondragon/tap-pipedream#readme Project-URL:
+Repository, https://github.com/edgarrmondragon/tap-pipedream Description-
+Content-Type: text/markdown
+                                # tap-pipedream
+                       [pre-commit.ci_status] [License]
+    Singer tap for Pipedream. Built with the [Meltano Singer SDK](https://
+                               sdk.meltano.com).
+## Capabilities * `catalog` * `state` * `discover` * `about` * `stream-maps` *
+`schema-flattening` ## Settings | Setting | Required | Default | Description |
+|:--------------------|:--------:|:-------:|:------------| | token | True |
+None | API Token for Pipedream | | start_date | False | None | Earliest
+timestamp to get data from | | stream_maps | False | None | Config object for
+stream maps capability. For more information check out [Stream Maps](https://
+sdk.meltano.com/en/latest/stream_maps.html). | | stream_map_config | False |
+None | User-defined config values to be used within map expressions. | |
+flattening_enabled | False | None | 'True' to enable schema flattening and
+automatically expand nested properties. | | flattening_max_depth| False | None
+| The max depth to flatten schemas. | A full list of supported settings and
+capabilities is available by running: `tap-pipedream --about` ### Source
+Authentication and Authorization To generate an API key, follow the
+instructions [in the docs](https://pipedream.com/docs/api/auth/#pipedream-api-
+key). ## Usage You can easily run `tap-pipedream` by itself or in a pipeline
+using [Meltano](https://meltano.com/). ### Executing the Tap Directly ```bash
+tap-pipedream --version tap-pipedream --help tap-pipedream --config CONFIG --
+discover > ./catalog.json ``` ## Developer Resources ### Initialize your
+Development Environment ```bash pipx install poetry poetry install ``` ###
+Create and Run Tests Create tests within the `tests` subfolder and then run:
+```bash poetry run pytest ``` You can also test the `tap-pipedream` CLI
+interface directly using `poetry run`: ```bash poetry run tap-pipedream --help
+``` ### Testing with [Meltano](https://www.meltano.com) _**Note:** This tap
+will work in any Singer environment and does not require Meltano. Examples here
+are for convenience and to streamline end-to-end orchestration scenarios._
+Install Meltano (if you haven't already) and any needed plugins: ```bash #
+Install meltano pipx install meltano # Initialize meltano within this directory
+cd tap-pipedream meltano install ``` Now you can test and orchestrate using
+Meltano: ```bash # Test invocation: meltano invoke tap-pipedream --version # OR
+run a test `elt` pipeline: meltano elt tap-pipedream target-jsonl ``` ### SDK
+Dev Guide See the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html)
+for more instructions on how to use the SDK to develop your own taps and
+targets.
```

