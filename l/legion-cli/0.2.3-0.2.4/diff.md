# Comparing `tmp/legion-cli-0.2.3.tar.gz` & `tmp/legion-cli-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legion-cli-0.2.3.tar", max compression
+gzip compressed data, was "legion-cli-0.2.4.tar", last modified: Mon Apr 10 23:25:55 2023, max compression
```

## Comparing `legion-cli-0.2.3.tar` & `legion-cli-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,50 @@
--rw-r--r--   0        0        0    34500 2021-06-29 22:18:00.000000 legion-cli-0.2.3/LICENSE
--rw-r--r--   0        0        0     2472 2021-06-29 22:18:00.000000 legion-cli-0.2.3/README.md
--rw-r--r--   0        0        0        0 2021-06-29 22:18:00.000000 legion-cli-0.2.3/legion_cli/__init__.py
--rw-r--r--   0        0        0     4459 2021-09-01 15:13:33.404707 legion-cli-0.2.3/legion_cli/alerts_manager.py
--rw-r--r--   0        0        0     7023 2021-09-01 15:13:33.404707 legion-cli-0.2.3/legion_cli/cli.py
--rw-r--r--   0        0        0      214 2021-06-29 22:18:00.000000 legion-cli-0.2.3/legion_cli/config.py
--rw-r--r--   0        0        0     1451 2021-09-01 15:13:33.404707 legion-cli-0.2.3/legion_cli/log.py
--rw-r--r--   0        0        0        0 2021-09-01 15:13:33.404707 legion-cli-0.2.3/legion_cli/tui/__init__.py
--rw-r--r--   0        0        0     8393 2021-09-01 15:13:33.404707 legion-cli-0.2.3/legion_cli/tui/alerts_monitor.py
--rw-r--r--   0        0        0     8180 2021-09-01 15:13:33.404707 legion-cli-0.2.3/legion_cli/tui/detail_list.py
--rw-r--r--   0        0        0      897 2021-09-01 15:13:33.404707 legion-cli-0.2.3/legion_cli/tui/keyboard.py
--rw-r--r--   0        0        0     1130 2022-01-17 20:28:50.342806 legion-cli-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3461 2022-01-17 20:29:01.321182 legion-cli-0.2.3/setup.py
--rw-r--r--   0        0        0     3568 2022-01-17 20:29:01.321468 legion-cli-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    34500 2022-11-16 02:41:53.005895 legion-cli-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2472 2022-11-16 02:41:53.005895 legion-cli-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.4/legion_cli/__init__.py
+-rw-r--r--   0        0        0     4459 2022-11-16 02:41:53.005895 legion-cli-0.2.4/legion_cli/alerts_manager.py
+-rw-r--r--   0        0        0     7023 2022-11-16 02:41:53.005895 legion-cli-0.2.4/legion_cli/cli.py
+-rw-r--r--   0        0        0      214 2022-11-16 02:41:53.005895 legion-cli-0.2.4/legion_cli/config.py
+-rw-r--r--   0        0        0     1451 2022-11-16 02:41:53.005895 legion-cli-0.2.4/legion_cli/log.py
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.4/legion_cli/tui/__init__.py
+-rw-r--r--   0        0        0     8393 2022-11-16 02:41:53.005895 legion-cli-0.2.4/legion_cli/tui/alerts_monitor.py
+-rw-r--r--   0        0        0     8180 2022-11-16 02:41:53.005895 legion-cli-0.2.4/legion_cli/tui/detail_list.py
+-rw-r--r--   0        0        0      897 2022-11-16 02:41:53.005895 legion-cli-0.2.4/legion_cli/tui/keyboard.py
+-rw-r--r--   0        0        0      956 2023-04-10 23:21:10.468487 legion-cli-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1119 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/test_watch.py
+-rw-r--r--   0        0        0     1103 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/utils.py
+-rw-r--r--   0        0        0     1184 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/host_files/rabbitmq-vm/legiond/legiond.conf
+-rw-r--r--   0        0        0      556 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/host_files/rabbitmq-vm/robotnikmq/robotnikmq.yaml
+-rw-r--r--   0        0        0    13754 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/library/ca.py
+-rw-r--r--   0        0        0    12451 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/library/cert.py
+-rw-r--r--   0        0        0      907 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/provision.yaml
+-rw-r--r--   0        0        0      234 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/robotnikmq.yaml
+-rw-r--r--   0        0        0       26 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/legion-cli/meta/main.yaml
+-rw-r--r--   0        0        0     1064 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/legion-cli/tasks/main.yaml
+-rw-r--r--   0        0        0       43 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/legiond/meta/main.yaml
+-rw-r--r--   0        0        0     2173 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/legiond/tasks/main.yaml
+-rw-r--r--   0        0        0      339 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/legiond/templates/legiond.conf.j2
+-rw-r--r--   0        0        0       84 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/rabbitmq/handlers/main.yaml
+-rw-r--r--   0        0        0       19 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/rabbitmq/meta/main.yaml
+-rw-r--r--   0        0        0      102 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/rabbitmq/tasks/main.yaml
+-rw-r--r--   0        0        0     1609 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq-cluster.yaml
+-rw-r--r--   0        0        0     4907 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq.yaml
+-rwxr-xr-x   0        0        0      588 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/rabbitmq/tasks/vhosts.yaml
+-rw-r--r--   0        0        0     1236 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq-env.conf.j2
+-rw-r--r--   0        0        0     1012 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq.conf.j2
+-rw-r--r--   0        0        0     2602 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/robotnikmq/files/dk_legion_robotnik_id_rsa
+-rw-r--r--   0        0        0      552 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/robotnikmq/files/dk_legion_robotnik_id_rsa.pub
+-rw-r--r--   0        0        0       21 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/robotnikmq/meta/main.yaml
+-rw-r--r--   0        0        0     1212 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/robotnikmq/tasks/main.yaml
+-rw-r--r--   0        0        0       78 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/supervisor/handlers/main.yaml
+-rw-r--r--   0        0        0       36 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/supervisor/tasks/main.yaml
+-rw-r--r--   0        0        0      385 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/supervisor/tasks/supervisor.yaml
+-rw-r--r--   0        0        0       29 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/tls/tasks/main.yaml
+-rw-r--r--   0        0        0     2526 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/roles/tls/tasks/tls.yaml
+-rw-r--r--   0        0        0      172 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/integration/vagrant/testing
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/unit/__init__.py
+-rw-r--r--   0        0        0     8670 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/unit/test_alerts_manager.py
+-rw-r--r--   0        0        0      863 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/unit/test_config.py
+-rw-r--r--   0        0        0    11550 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/unit/test_detail_list.py
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.4/tests/unit/test_keyboard.py
+-rw-r--r--   0        0        0     2755 1970-01-01 00:00:00.000000 legion-cli-0.2.4/PKG-INFO
```

### Comparing `legion-cli-0.2.3/LICENSE` & `legion-cli-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.3/README.md` & `legion-cli-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.3/legion_cli/alerts_manager.py` & `legion-cli-0.2.4/legion_cli/alerts_manager.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.3/legion_cli/cli.py` & `legion-cli-0.2.4/legion_cli/cli.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.3/legion_cli/log.py` & `legion-cli-0.2.4/legion_cli/log.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.3/legion_cli/tui/alerts_monitor.py` & `legion-cli-0.2.4/legion_cli/tui/alerts_monitor.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.3/legion_cli/tui/detail_list.py` & `legion-cli-0.2.4/legion_cli/tui/detail_list.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.3/legion_cli/tui/keyboard.py` & `legion-cli-0.2.4/legion_cli/tui/keyboard.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.3/setup.py` & `legion-cli-0.2.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,98 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: legion-cli
+Version: 0.2.4
+Summary: Commandline Utilities for the Legion Alerting and Monitoring System
+License: GPL-3.0-or-later
+Author-email: Eugene Kovalev <eugene@kovalev.systems>
+Requires-Python: >=3.8.3,<4.0
+Description-Content-Type: text/markdown
 
-packages = \
-['legion_cli', 'legion_cli.tui']
+# Legion CLI
 
-package_data = \
-{'': ['*']}
+Commandline Utilities for the Legion Alerting and Monitoring System
 
-install_requires = \
-['click>=8.0,<9.0',
- 'legion-utils>=0.2.10,<0.3.0',
- 'rich>=10.8.0,<11.0.0',
- 'termcolor>=1.1,<2.0']
-
-entry_points = \
-{'console_scripts': ['legion = legion_cli.cli:cli']}
-
-setup_kwargs = {
-    'name': 'legion-cli',
-    'version': '0.2.3',
-    'description': 'Commandline Utilities for the Legion Alerting and Monitoring System',
-    'long_description': '# Legion CLI\n\nCommandline Utilities for the Legion Alerting and Monitoring System\n\n## Setup & Usage\n\n### Installation\n\nTODO\n\n### Configuration\n\nTODO\n\n### Usage\n\nThe key reference for using `legion-cli` is:\n\n```bash\nlegion-cli --help\n```\n\n## Development\n\n### Standards\n\n- Be excellent to each other\n- Code coverage must be at 100% for all new code, or a good reason must be provided for why a given bit of code is not covered.\n  - Example of an acceptable reason: "There is a bug in the code coverage tool and it says its missing this, but its not".\n  - Example of unacceptable reason: "This is just exception handling, its too annoying to cover it".\n- The code must pass the following analytics tools. Similar exceptions are allowable as in rule 2.\n  - `pylint --disable=C0111,W1203,R0903 --max-line-length=100 ...`\n  - `flake8 --max-line-length=100 ...`\n  - `mypy --ignore-missing-imports --follow-imports=skip --strict-optional ...`\n- All incoming information from users, clients, and configurations should be validated.\n- All internal arguments passing should be typechecked whenever possible with `typeguard.typechecked`\n\n### Development Setup\n\nUsing [poetry](https://python-poetry.org/) install from inside the repo directory:\n\n```bash\npoetry install\n```\n\nThis will set up a virtualenv which you can always activate with either `poetry shell` or run specific commands with `poetry run`. All instructions below that are meant to be run in the virtualenv will be prefaced with `(legion-cli)$ `\n\n#### IDE Setup\n\n**Sublime Text 3**\n\n```bash\ncurl -sSL https://gitlab.com/-/snippets/2066312/raw/master/poetry.sublime-project.py | poetry run python\n```\n\n#### Development\n\n### Testing\n\nAll testing should be done with `pytest` which is installed with the `dev` requirements.\n\nTo run all the unit tests, execute the following from the repo directory:\n\n```bash\n(legion-cli)$  pytest\n```\n\nThis should produce a coverage report in `/path/to/dewey-api/htmlcov/`\n\nWhile developing, you can use [`watchexec`](https://github.com/watchexec/watchexec) to monitor the file system for changes and re-run the tests:\n\n```bash\n(legion-cli)$ watchexec -r -e py,yaml pytest\n```\n\nTo run a specific test file:\n\n```bash\n(legion-cli)$ pytest tests/unit/test_cli.py\n```\n\nTo run a specific test:\n\n```bash\n(legion-cli)$ pytest tests/unit/test_cli.py::test_cli_basics\n```\n\nFor more information on testing, see the `pytest.ini` file as well as the [documentation](https://docs.pytest.org/en/stable/).\n',
-    'author': 'Eugene Kovalev',
-    'author_email': 'eugene@kovalev.systems',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://gitlab.com/legion-robotnik/legion-cli',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+## Setup & Usage
 
+### Installation
+
+TODO
+
+### Configuration
+
+TODO
+
+### Usage
+
+The key reference for using `legion-cli` is:
+
+```bash
+legion-cli --help
+```
+
+## Development
+
+### Standards
+
+- Be excellent to each other
+- Code coverage must be at 100% for all new code, or a good reason must be provided for why a given bit of code is not covered.
+  - Example of an acceptable reason: "There is a bug in the code coverage tool and it says its missing this, but its not".
+  - Example of unacceptable reason: "This is just exception handling, its too annoying to cover it".
+- The code must pass the following analytics tools. Similar exceptions are allowable as in rule 2.
+  - `pylint --disable=C0111,W1203,R0903 --max-line-length=100 ...`
+  - `flake8 --max-line-length=100 ...`
+  - `mypy --ignore-missing-imports --follow-imports=skip --strict-optional ...`
+- All incoming information from users, clients, and configurations should be validated.
+- All internal arguments passing should be typechecked whenever possible with `typeguard.typechecked`
+
+### Development Setup
+
+Using [poetry](https://python-poetry.org/) install from inside the repo directory:
+
+```bash
+poetry install
+```
+
+This will set up a virtualenv which you can always activate with either `poetry shell` or run specific commands with `poetry run`. All instructions below that are meant to be run in the virtualenv will be prefaced with `(legion-cli)$ `
+
+#### IDE Setup
+
+**Sublime Text 3**
+
+```bash
+curl -sSL https://gitlab.com/-/snippets/2066312/raw/master/poetry.sublime-project.py | poetry run python
+```
+
+#### Development
+
+### Testing
+
+All testing should be done with `pytest` which is installed with the `dev` requirements.
+
+To run all the unit tests, execute the following from the repo directory:
+
+```bash
+(legion-cli)$  pytest
+```
+
+This should produce a coverage report in `/path/to/dewey-api/htmlcov/`
+
+While developing, you can use [`watchexec`](https://github.com/watchexec/watchexec) to monitor the file system for changes and re-run the tests:
+
+```bash
+(legion-cli)$ watchexec -r -e py,yaml pytest
+```
+
+To run a specific test file:
+
+```bash
+(legion-cli)$ pytest tests/unit/test_cli.py
+```
+
+To run a specific test:
+
+```bash
+(legion-cli)$ pytest tests/unit/test_cli.py::test_cli_basics
+```
+
+For more information on testing, see the `pytest.ini` file as well as the [documentation](https://docs.pytest.org/en/stable/).
 
-setup(**setup_kwargs)
```

