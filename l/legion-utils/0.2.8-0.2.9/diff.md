# Comparing `tmp/legion-utils-0.2.8.tar.gz` & `tmp/legion-utils-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legion-utils-0.2.8.tar", max compression
+gzip compressed data, was "legion-utils-0.2.9.tar", max compression
```

## Comparing `legion-utils-0.2.8.tar` & `legion-utils-0.2.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34500 2021-07-04 19:28:00.000000 legion-utils-0.2.8/LICENSE
--rw-r--r--   0        0        0     2573 2021-07-04 19:28:00.000000 legion-utils-0.2.8/README.md
--rw-r--r--   0        0        0      671 2021-09-01 15:13:35.284697 legion-utils-0.2.8/legion_utils/__init__.py
--rw-r--r--   0        0        0    12427 2021-09-01 15:13:35.284697 legion-utils-0.2.8/legion_utils/core.py
--rw-r--r--   0        0        0     1054 2021-12-30 04:42:29.121573 legion-utils-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     3372 2021-12-30 06:05:59.002115 legion-utils-0.2.8/setup.py
--rw-r--r--   0        0        0     3582 2021-12-30 06:05:59.002419 legion-utils-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    34500 2021-07-04 19:28:00.000000 legion-utils-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2573 2021-07-04 19:28:00.000000 legion-utils-0.2.9/README.md
+-rw-r--r--   0        0        0      671 2021-09-01 15:13:35.284697 legion-utils-0.2.9/legion_utils/__init__.py
+-rw-r--r--   0        0        0    12427 2021-09-01 15:13:35.284697 legion-utils-0.2.9/legion_utils/core.py
+-rw-r--r--   0        0        0     1054 2022-01-17 17:10:47.572775 legion-utils-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     3372 2022-01-17 17:14:46.313467 legion-utils-0.2.9/setup.py
+-rw-r--r--   0        0        0     3582 2022-01-17 17:14:46.313776 legion-utils-0.2.9/PKG-INFO
```

### Comparing `legion-utils-0.2.8/LICENSE` & `legion-utils-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `legion-utils-0.2.8/README.md` & `legion-utils-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `legion-utils-0.2.8/legion_utils/__init__.py` & `legion-utils-0.2.9/legion_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `legion-utils-0.2.8/legion_utils/core.py` & `legion-utils-0.2.9/legion_utils/core.py`

 * *Files identical despite different names*

### Comparing `legion-utils-0.2.8/pyproject.toml` & `legion-utils-0.2.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "legion-utils"
-version = "0.2.8"
+version = "0.2.9"
 description = "Utilities for Legion Reporters and Monitors"
 authors = ["Eugene Kovalev <eugene@kovalev.systems>"]
 classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
@@ -17,15 +17,15 @@
 repository="https://gitlab.com/legion-robotnik/legion-utils"
 readme="README.md"
 license="GPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typeguard = "^2.13.3"
-robotnikmq = "^0.3.2"
+robotnikmq = "^0.3.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 pylint = "^2.12.2"
 mypy = "^0.930"
 flake8 = "^4.0.1"
```

### Comparing `legion-utils-0.2.8/setup.py` & `legion-utils-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['legion_utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['robotnikmq>=0.3.2,<0.4.0', 'typeguard>=2.13.3,<3.0.0']
+['robotnikmq>=0.3.3,<0.4.0', 'typeguard>=2.13.3,<3.0.0']
 
 setup_kwargs = {
     'name': 'legion-utils',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Utilities for Legion Reporters and Monitors',
     'long_description': '# Legion Utils\n\nUtilities for Legion Reporters and Monitors\n\n## Usage\n\nTODO\n\n## Installation & Setup\n\nTo install legion-utils with [`pip`](https://pip.pypa.io/en/stable/) execute the following:\n\n```bash\npip install /path/to/repo/legion-utils\n```\n\nIf you don\'t want to re-install every time there is an update, and prefer to just pull from the git repository, then use the `-e` flag.\n\n## Development\n\n### Standards\n\n- Be excellent to each other\n- Code coverage must be at 100% for all new code, or a good reason must be provided for why a given bit of code is not covered.\n  - Example of an acceptable reason: "There is a bug in the code coverage tool and it says its missing this, but its not".\n  - Example of unacceptable reason: "This is just exception handling, its too annoying to cover it".\n- The code must pass the following analytics tools. Similar exceptions are allowable as in rule 2.\n  - `pylint --disable=C0111,W1203,R0903 --max-line-length=100 ...`\n  - `flake8 --max-line-length=100 ...`\n  - `mypy --ignore-missing-imports --follow-imports=skip --strict-optional ...`\n- All incoming information from users, clients, and configurations should be validated.\n- All internal arguments passing should be typechecked whenever possible with `typeguard.typechecked`\n\n### Development Setup\n\nUsing [poetry](https://python-poetry.org/) install from inside the repo directory:\n\n```bash\npoetry install\n```\n\nThis will set up a virtualenv which you can always activate with either `poetry shell` or run specific commands with `poetry run`. All instructions below that are meant to be run in the virtualenv will be prefaced with `(legion-utils)$ `\n\n#### IDE Setup\n\n**Sublime Text 3**\n\n```bash\ncurl -sSL https://gitlab.com/-/snippets/2066312/raw/master/poetry.sublime-project.py | poetry run python\n```\n\n## Testing\n\nAll testing should be done with `pytest` which is installed with the `dev` requirements.\n\nTo run all the unit tests, execute the following from the repo directory:\n\n```bash\n(legion-utils)$ pytest\n```\n\nThis should produce a coverage report in `/path/to/dewey-api/htmlcov/`\n\nWhile developing, you can use [`watchexec`](https://github.com/watchexec/watchexec) to monitor the file system for changes and re-run the tests:\n\n```bash\n(legion-utils)$ watchexec -r -e py,yaml pytest\n```\n\nTo run a specific test file:\n\n```bash\npytest tests/unit/test_core.py\n```\n\nTo run a specific test:\n\n```bash\npytest tests/unit/test_core.py::test_hello\n```\n\nFor more information on testing, see the `pytest.ini` file as well as the [documentation](https://docs.pytest.org/en/stable/).\n',
     'author': 'Eugene Kovalev',
     'author_email': 'eugene@kovalev.systems',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/legion-robotnik/legion-utils',
```

### Comparing `legion-utils-0.2.8/PKG-INFO` & `legion-utils-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legion-utils
-Version: 0.2.8
+Version: 0.2.9
 Summary: Utilities for Legion Reporters and Monitors
 Home-page: https://gitlab.com/legion-robotnik/legion-utils
 License: GPL-3.0-only
 Author: Eugene Kovalev
 Author-email: eugene@kovalev.systems
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: robotnikmq (>=0.3.2,<0.4.0)
+Requires-Dist: robotnikmq (>=0.3.3,<0.4.0)
 Requires-Dist: typeguard (>=2.13.3,<3.0.0)
 Project-URL: Documentation, https://gitlab.com/legion-robotnik/legion-utils
 Project-URL: Repository, https://gitlab.com/legion-robotnik/legion-utils
 Description-Content-Type: text/markdown
 
 # Legion Utils
```

