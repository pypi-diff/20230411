# Comparing `tmp/serious-scaffold-0.0.8.tar.gz` & `tmp/serious-scaffold-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serious-scaffold-0.0.8.tar", last modified: Wed Jan 11 07:22:43 2023, max compression
+gzip compressed data, was "serious-scaffold-0.0.9.tar", last modified: Tue Apr 11 13:03:48 2023, max compression
```

## Comparing `serious-scaffold-0.0.8.tar` & `serious-scaffold-0.0.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.818744 serious-scaffold-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.814743 serious-scaffold-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/.github/FUNDING.yml.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.814743 serious-scaffold-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/.github/workflows/package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/.github/workflows/readthedocs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/.github/workflows/readthedocs-preview.yml.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/.gitignore.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.814743 serious-scaffold-0.0.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/Makefile.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-01-11 07:22:43.818744 serious-scaffold-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/README.md.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.814743 serious-scaffold-0.0.8/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/constraints/default.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/copier.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.814743 serious-scaffold-0.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.810743 serious-scaffold-0.0.8/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.814743 serious-scaffold-0.0.8/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/docs/_static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.814743 serious-scaffold-0.0.8/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/docs/cli/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/docs/cli/index.rst.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/docs/conf.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/docs/index.rst.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.814743 serious-scaffold-0.0.8/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/docs/modules/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/docs/modules/index.rst.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/docs/modules/serious_scaffold.settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/docs/modules/{{ module_name }}.settings.rst.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/pyproject.toml.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.814743 serious-scaffold-0.0.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/requirements/package.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 07:22:43.818744 serious-scaffold-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.810743 serious-scaffold-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.814743 serious-scaffold-0.0.8/src/serious_scaffold/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/src/serious_scaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/src/serious_scaffold/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/src/serious_scaffold/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.814743 serious-scaffold-0.0.8/src/serious_scaffold.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-01-11 07:22:43.000000 serious-scaffold-0.0.8/src/serious_scaffold.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-01-11 07:22:43.000000 serious-scaffold-0.0.8/src/serious_scaffold.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 07:22:43.000000 serious-scaffold-0.0.8/src/serious_scaffold.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-11 07:22:43.000000 serious-scaffold-0.0.8/src/serious_scaffold.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-01-11 07:22:43.000000 serious-scaffold-0.0.8/src/serious_scaffold.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-11 07:22:43.000000 serious-scaffold-0.0.8/src/serious_scaffold.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.818744 serious-scaffold-0.0.8/src/{{ module_name }}/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/src/{{ module_name }}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/src/{{ module_name }}/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/src/{{ module_name }}/settings.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 07:22:43.818744 serious-scaffold-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/tests/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/tests/cli_test.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/tests/pkg_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/tests/pkg_test.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/tests/settings_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/tests/settings_test.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-11 07:22:13.000000 serious-scaffold-0.0.8/{{_copier_conf.answers_file}}.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.681902 serious-scaffold-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.677902 serious-scaffold-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/.github/FUNDING.yml.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.677902 serious-scaffold-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/.github/workflows/package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/.github/workflows/readthedocs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/.github/workflows/readthedocs-preview.yml.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/.gitignore.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.677902 serious-scaffold-0.0.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/Makefile.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-11 13:03:48.681902 serious-scaffold-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/README.md.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.677902 serious-scaffold-0.0.9/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/constraints/default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/copier.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.677902 serious-scaffold-0.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.673902 serious-scaffold-0.0.9/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.677902 serious-scaffold-0.0.9/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/docs/_static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.677902 serious-scaffold-0.0.9/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/docs/cli/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/docs/cli/index.rst.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/docs/conf.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/docs/index.rst.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.677902 serious-scaffold-0.0.9/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/docs/modules/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/docs/modules/index.rst.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/docs/modules/serious_scaffold.settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/docs/modules/{{ module_name }}.settings.rst.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/pyproject.toml.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.677902 serious-scaffold-0.0.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/requirements/package.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:03:48.681902 serious-scaffold-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.673902 serious-scaffold-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.681902 serious-scaffold-0.0.9/src/serious_scaffold/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/src/serious_scaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/src/serious_scaffold/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/src/serious_scaffold/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.681902 serious-scaffold-0.0.9/src/serious_scaffold.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-11 13:03:48.000000 serious-scaffold-0.0.9/src/serious_scaffold.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-11 13:03:48.000000 serious-scaffold-0.0.9/src/serious_scaffold.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:03:48.000000 serious-scaffold-0.0.9/src/serious_scaffold.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-11 13:03:48.000000 serious-scaffold-0.0.9/src/serious_scaffold.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-11 13:03:48.000000 serious-scaffold-0.0.9/src/serious_scaffold.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 13:03:48.000000 serious-scaffold-0.0.9/src/serious_scaffold.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.681902 serious-scaffold-0.0.9/src/{{ module_name }}/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/src/{{ module_name }}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/src/{{ module_name }}/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/src/{{ module_name }}/settings.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:48.681902 serious-scaffold-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/tests/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/tests/cli_test.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/tests/pkg_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/tests/pkg_test.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/tests/settings_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/tests/settings_test.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-11 13:03:21.000000 serious-scaffold-0.0.9/{{_copier_conf.answers_file}}.jinja
```

### Comparing `serious-scaffold-0.0.8/.github/workflows/ci.yml` & `serious-scaffold-0.0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `serious-scaffold-0.0.8/.github/workflows/package.yml` & `serious-scaffold-0.0.9/.github/workflows/package.yml`

 * *Files identical despite different names*

### Comparing `serious-scaffold-0.0.8/.gitignore` & `serious-scaffold-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `serious-scaffold-0.0.8/.gitignore.jinja` & `serious-scaffold-0.0.9/.gitignore.jinja`

 * *Files identical despite different names*

### Comparing `serious-scaffold-0.0.8/.pre-commit-config.yaml` & `serious-scaffold-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `serious-scaffold-0.0.8/.vscode/settings.json` & `serious-scaffold-0.0.9/.vscode/settings.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8260869565217391%*

 * *Differences: {"'vscode-yaml-sort.useArrayProcessor'": 'False',*

 * * "'vscode-yaml-sort.useBlockProcessor'": 'False',*

 * * "'vscode-yaml-sort.useHelmProcessor'": 'False',*

 * * 'delete': "['vscode-yaml-sort.useAsFormatter']"}*

```diff
@@ -71,10 +71,12 @@
         "author_email",
         "repo_name",
         "package_name",
         "module_name"
     ],
     "vscode-yaml-sort.noCompatMode": true,
     "vscode-yaml-sort.sortOnSave": 2,
-    "vscode-yaml-sort.useAsFormatter": true,
+    "vscode-yaml-sort.useArrayProcessor": false,
+    "vscode-yaml-sort.useBlockProcessor": false,
+    "vscode-yaml-sort.useHelmProcessor": false,
     "vscode-yaml-sort.useLeadingDashes": false
 }
```

### Comparing `serious-scaffold-0.0.8/LICENSE` & `serious-scaffold-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `serious-scaffold-0.0.8/Makefile` & `serious-scaffold-0.0.9/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 		Pipfile* \
 		coverage.xml \
 		dist \
 		docs/_build
 	find . -name '*.egg-info' -print0 | xargs -0 rm -rf
 	find . -name '*.pyc' -print0 | xargs -0 rm -f
 	find . -name '*.swp' -print0 | xargs -0 rm -f
-	find . -name '.DS_Store' -print0 | xargs -0 rm -r
+	find . -name '.DS_Store' -print0 | xargs -0 rm -f
 	find . -name '__pycache__' -print0 | xargs -0 rm -rf
 
 deepclean: clean
 	-pre-commit uninstall --hook-type pre-push
 	-pipenv --venv >/dev/null 2>&1 && pipenv --rm
 
 install:
```

### Comparing `serious-scaffold-0.0.8/Makefile.jinja` & `serious-scaffold-0.0.9/Makefile.jinja`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 		Pipfile* \
 		coverage.xml \
 		dist \
 		docs/_build
 	find . -name '*.egg-info' -print0 | xargs -0 rm -rf
 	find . -name '*.pyc' -print0 | xargs -0 rm -f
 	find . -name '*.swp' -print0 | xargs -0 rm -f
-	find . -name '.DS_Store' -print0 | xargs -0 rm -r
+	find . -name '.DS_Store' -print0 | xargs -0 rm -f
 	find . -name '__pycache__' -print0 | xargs -0 rm -rf
 
 deepclean: clean
 	-pre-commit uninstall --hook-type pre-push
 	-pipenv --venv >/dev/null 2>&1 && pipenv --rm
 
 install:
```

### Comparing `serious-scaffold-0.0.8/PKG-INFO` & `serious-scaffold-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serious-scaffold
-Version: 0.0.8
+Version: 0.0.9
 Summary: A serious Python project template for out-of-box and production usage.
 Author-email: huxuan <i@huxuan.org>
 Project-URL: homepage, https://github.com/huxuan/serious-scaffold-python/
 Project-URL: issue, https://github.com/huxuan/serious-scaffold-python/issues
 Keywords: out-of-box,production,project template,template
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: serious-scaffold Version: 0.0.8 Summary: A serious
+Metadata-Version: 2.1 Name: serious-scaffold Version: 0.0.9 Summary: A serious
 Python project template for out-of-box and production usage. Author-email:
 huxuan
 huxuan.org> Project-URL: homepage, https://github.com/huxuan/serious-scaffold-
 python/ Project-URL: issue, https://github.com/huxuan/serious-scaffold-python/
 issues Keywords: out-of-box,production,project template,template Classifier:
 Development Status :: 4 - Beta Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
```

### Comparing `serious-scaffold-0.0.8/README.md` & `serious-scaffold-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `serious-scaffold-0.0.8/README.md.jinja` & `serious-scaffold-0.0.9/README.md.jinja`

 * *Files identical despite different names*

### Comparing `serious-scaffold-0.0.8/constraints/default.txt` & `serious-scaffold-0.0.9/constraints/default.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,68 @@
-alabaster==0.7.12
-attrs==22.2.0
+alabaster==0.7.13
 autodoc-pydantic==1.8.0
-Babel==2.11.0
-beautifulsoup4==4.11.1
-black==22.12.0
-bleach==5.0.1
-build==0.9.0
+Babel==2.12.1
+beautifulsoup4==4.12.2
+black==23.3.0
+bleach==6.0.0
+build==0.10.0
 certifi==2022.12.7
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
 click==8.1.3
 colorama==0.4.6
 commonmark==0.9.1
-coverage==7.0.3
+coverage==7.2.3
 docutils==0.19
-exceptiongroup==1.1.0
-furo==2022.12.7
+furo==2023.3.27
 idna==3.4
 imagesize==1.4.1
-importlib-metadata==6.0.0
-iniconfig==1.1.1
-isort==5.11.4
+importlib-metadata==6.3.0
+iniconfig==2.0.0
+isort==5.12.0
 jaraco.classes==3.2.3
 Jinja2==3.1.2
 keyring==23.13.1
 livereload==2.6.3
-MarkupSafe==2.1.1
-more-itertools==9.0.0
-mypy==0.991
-mypy-extensions==0.4.3
-packaging==22.0
-pathspec==0.10.3
-pep517==0.13.0
-pkginfo==1.9.3
-platformdirs==2.6.2
+MarkupSafe==2.1.2
+more-itertools==9.1.0
+mypy==1.2.0
+mypy-extensions==1.0.0
+packaging==23.0
+pathspec==0.11.1
+pkginfo==1.9.6
+platformdirs==3.2.0
 pluggy==1.0.0
-pydantic==1.10.4
-Pygments==2.14.0
-pytest==7.2.0
+pydantic==1.10.7
+Pygments==2.15.0
+pyproject_hooks==1.0.0
+pytest==7.3.0
 pytest-cov==4.0.0
-pytz==2022.7
 readme-renderer==37.3
-requests==2.28.1
+requests==2.28.2
 requests-toolbelt==0.10.1
 rfc3986==2.0.0
 rich==12.6.0
-ruff==0.0.209
+ruff==0.0.261
 setuptools-scm==7.1.0
 shellingham==1.5.0.post1
 six==1.16.0
 snowballstemmer==2.2.0
-soupsieve==2.3.2.post1
-Sphinx==6.0.0
+soupsieve==2.4
+Sphinx==6.1.3
 sphinx-autobuild==2021.3.14
 sphinx-basic-ng==1.0.0b1
 sphinx-click==4.4.0
-sphinxcontrib-applehelp==1.0.2
+sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-toml-sort==0.22.1
-tomli==2.0.1
-tomlkit==0.11.6
+toml-sort==0.23.0
+tomlkit==0.11.7
 tornado==6.2
 twine==4.0.2
 typer==0.7.0
-typing_extensions==4.4.0
-urllib3==1.26.13
+typing_extensions==4.5.0
+urllib3==1.26.15
 webencodings==0.5.1
-zipp==3.11.0
+zipp==3.15.0
```

### Comparing `serious-scaffold-0.0.8/copier.yaml` & `serious-scaffold-0.0.9/copier.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -26,18 +26,18 @@
   help: 'Author name:'
   type: str
 author_email:
   default: i@{{ author_name }}.org
   help: 'Author email:'
   type: str
 repo_name:
-  default: '{{ project_name|lower|replace('' '', ''-'') }}'
+  default: '{{ project_name|lower|replace(" ", "-") }}'
   help: 'Repo name:'
   type: str
 package_name:
-  default: '{{ repo_name|regex_replace(''-python$'','''') }}'
+  default: '{{ repo_name|regex_replace("-python$", "") }}'
   help: 'Package name:'
   type: str
 module_name:
-  default: '{{ package_name|lower|replace(''-'', ''_'') }}'
+  default: '{{ package_name|lower|replace("-", "_") }}'
   help: 'Module name:'
   type: str
```

### Comparing `serious-scaffold-0.0.8/docs/_static/images/logo.png` & `serious-scaffold-0.0.9/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `serious-scaffold-0.0.8/docs/conf.py` & `serious-scaffold-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `serious-scaffold-0.0.8/docs/conf.py.jinja` & `serious-scaffold-0.0.9/docs/conf.py.jinja`

 * *Files identical despite different names*

### Comparing `serious-scaffold-0.0.8/pyproject.toml` & `serious-scaffold-0.0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -87,18 +87,21 @@
   "D406",
   "D407",
   "D408",
   "D409",
   "D413",
 ]
 fix = true
-per-file-ignores = {"tests/*" = ["S101"]}
 select = ["ALL"]
 src = ["src"]
-target-version = "py38"
+
+[tool.ruff.per-file-ignores]
+"docs/conf.py" = ["INP001"]
+"src/\\{\\{ module_name \\}\\}/__init__.py" = ["N999"]
+"tests/*" = ["S101"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [tool.setuptools.dynamic.optional-dependencies]
 docs = {file = ["requirements/docs.txt"]}
 lint = {file = ["requirements/lint.txt"]}
```

### Comparing `serious-scaffold-0.0.8/pyproject.toml.jinja` & `serious-scaffold-0.0.9/pyproject.toml.jinja`

 * *Files identical despite different names*

### Comparing `serious-scaffold-0.0.8/src/serious_scaffold/settings.py` & `serious-scaffold-0.0.9/src/serious_scaffold/settings.py`

 * *Files identical despite different names*

### Comparing `serious-scaffold-0.0.8/src/serious_scaffold.egg-info/PKG-INFO` & `serious-scaffold-0.0.9/src/serious_scaffold.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serious-scaffold
-Version: 0.0.8
+Version: 0.0.9
 Summary: A serious Python project template for out-of-box and production usage.
 Author-email: huxuan <i@huxuan.org>
 Project-URL: homepage, https://github.com/huxuan/serious-scaffold-python/
 Project-URL: issue, https://github.com/huxuan/serious-scaffold-python/issues
 Keywords: out-of-box,production,project template,template
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: serious-scaffold Version: 0.0.8 Summary: A serious
+Metadata-Version: 2.1 Name: serious-scaffold Version: 0.0.9 Summary: A serious
 Python project template for out-of-box and production usage. Author-email:
 huxuan
 huxuan.org> Project-URL: homepage, https://github.com/huxuan/serious-scaffold-
 python/ Project-URL: issue, https://github.com/huxuan/serious-scaffold-python/
 issues Keywords: out-of-box,production,project template,template Classifier:
 Development Status :: 4 - Beta Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
```

### Comparing `serious-scaffold-0.0.8/src/serious_scaffold.egg-info/SOURCES.txt` & `serious-scaffold-0.0.9/src/serious_scaffold.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serious-scaffold-0.0.8/src/{{ module_name }}/settings.py.jinja` & `serious-scaffold-0.0.9/src/{{ module_name }}/settings.py.jinja`

 * *Files identical despite different names*

