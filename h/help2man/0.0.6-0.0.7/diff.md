# Comparing `tmp/help2man-0.0.6.tar.gz` & `tmp/help2man-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "help2man-0.0.6.tar", last modified: Tue Apr 11 16:37:24 2023, max compression
+gzip compressed data, was "help2man-0.0.7.tar", last modified: Tue Apr 11 16:57:05 2023, max compression
```

## Comparing `help2man-0.0.6.tar` & `help2man-0.0.7.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.941069 help2man-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.925068 help2man-0.0.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-11 16:37:03.000000 help2man-0.0.6/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.925068 help2man-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-11 16:37:03.000000 help2man-0.0.6/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-11 16:37:03.000000 help2man-0.0.6/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-04-11 16:37:03.000000 help2man-0.0.6/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-11 16:37:03.000000 help2man-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-11 16:37:03.000000 help2man-0.0.6/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-11 16:37:03.000000 help2man-0.0.6/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-11 16:37:03.000000 help2man-0.0.6/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 16:37:03.000000 help2man-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-11 16:37:24.941069 help2man-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-04-11 16:37:03.000000 help2man-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.929069 help2man-0.0.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.929069 help2man-0.0.6/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 16:37:03.000000 help2man-0.0.6/docs/api/external.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-11 16:37:03.000000 help2man-0.0.6/docs/api/help2man.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 16:37:03.000000 help2man-0.0.6/docs/api/ui.md
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-11 16:37:03.000000 help2man-0.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-11 16:37:03.000000 help2man-0.0.6/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-11 16:37:03.000000 help2man-0.0.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.929069 help2man-0.0.6/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 16:37:03.000000 help2man-0.0.6/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 16:37:03.000000 help2man-0.0.6/docs/resources/man.md
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-11 16:37:03.000000 help2man-0.0.6/flake.lock
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-11 16:37:03.000000 help2man-0.0.6/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-11 16:37:03.000000 help2man-0.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.929069 help2man-0.0.6/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)      113 2023-04-11 16:37:03.000000 help2man-0.0.6/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-11 16:37:03.000000 help2man-0.0.6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.929069 help2man-0.0.6/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-11 16:37:03.000000 help2man-0.0.6/scripts/generate-api.md.pl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.929069 help2man-0.0.6/sdist/
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-11 16:37:24.000000 help2man-0.0.6/sdist/_help2man
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-11 16:37:24.000000 help2man-0.0.6/sdist/help2man
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-11 16:37:24.000000 help2man-0.0.6/sdist/help2man.1
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 16:37:24.941069 help2man-0.0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2521 2023-04-11 16:37:03.000000 help2man-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.921069 help2man-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.933069 help2man-0.0.6/src/help2man/
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-04-11 16:37:03.000000 help2man-0.0.6/src/help2man/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3420 2023-04-11 16:37:03.000000 help2man-0.0.6/src/help2man/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 16:37:24.000000 help2man-0.0.6/src/help2man/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.921069 help2man-0.0.6/src/help2man/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.933069 help2man-0.0.6/src/help2man/assets/jinja2/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-11 16:37:03.000000 help2man-0.0.6/src/help2man/assets/jinja2/template.man.j2
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-11 16:37:03.000000 help2man-0.0.6/src/help2man/assets/jinja2/template.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.937069 help2man-0.0.6/src/help2man/assets/txt/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 16:37:24.000000 help2man-0.0.6/src/help2man/assets/txt/description.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-11 16:37:24.000000 help2man-0.0.6/src/help2man/assets/txt/epilog.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 16:37:24.000000 help2man-0.0.6/src/help2man/assets/txt/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.937069 help2man-0.0.6/src/help2man/external/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-11 16:37:03.000000 help2man-0.0.6/src/help2man/external/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-04-11 16:37:03.000000 help2man-0.0.6/src/help2man/external/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.937069 help2man-0.0.6/src/help2man/external/shtab/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-11 16:37:03.000000 help2man-0.0.6/src/help2man/external/shtab/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1746 2023-04-11 16:37:03.000000 help2man-0.0.6/src/help2man/external/shtab/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:03.000000 help2man-0.0.6/src/help2man/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.937069 help2man-0.0.6/src/help2man/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-11 16:37:03.000000 help2man-0.0.6/src/help2man/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-11 16:37:03.000000 help2man-0.0.6/src/help2man/ui/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.933069 help2man-0.0.6/src/help2man.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-11 16:37:24.000000 help2man-0.0.6/src/help2man.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-11 16:37:24.000000 help2man-0.0.6/src/help2man.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:37:24.000000 help2man-0.0.6/src/help2man.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 16:37:24.000000 help2man-0.0.6/src/help2man.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 16:37:24.000000 help2man-0.0.6/src/help2man.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 16:37:24.000000 help2man-0.0.6/src/help2man.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.941069 help2man-0.0.6/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 16:37:03.000000 help2man-0.0.6/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-11 16:37:03.000000 help2man-0.0.6/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 16:37:03.000000 help2man-0.0.6/templates/epilog.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 16:37:03.000000 help2man-0.0.6/templates/noarg.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 16:37:03.000000 help2man-0.0.6/templates/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.941069 help2man-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-11 16:37:03.000000 help2man-0.0.6/tests/__init___test.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-11 16:37:03.000000 help2man-0.0.6/tests/cmd_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:37:24.941069 help2man-0.0.6/tests/txt/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-11 16:37:03.000000 help2man-0.0.6/tests/txt/options.txt
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-11 16:37:03.000000 help2man-0.0.6/tests/txt/test.man
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-11 16:37:03.000000 help2man-0.0.6/tests/txt/usage.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.270597 help2man-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.266597 help2man-0.0.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-11 16:56:53.000000 help2man-0.0.7/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.266597 help2man-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-11 16:56:53.000000 help2man-0.0.7/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-11 16:56:53.000000 help2man-0.0.7/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-04-11 16:56:53.000000 help2man-0.0.7/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-11 16:56:53.000000 help2man-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-11 16:56:53.000000 help2man-0.0.7/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-11 16:56:53.000000 help2man-0.0.7/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-11 16:56:53.000000 help2man-0.0.7/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 16:56:53.000000 help2man-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-11 16:57:05.270597 help2man-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-04-11 16:56:53.000000 help2man-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.266597 help2man-0.0.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.266597 help2man-0.0.7/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 16:56:53.000000 help2man-0.0.7/docs/api/external.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-11 16:56:53.000000 help2man-0.0.7/docs/api/help2man.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 16:56:53.000000 help2man-0.0.7/docs/api/ui.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-11 16:56:53.000000 help2man-0.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-11 16:56:53.000000 help2man-0.0.7/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-11 16:56:53.000000 help2man-0.0.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.266597 help2man-0.0.7/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 16:56:53.000000 help2man-0.0.7/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 16:56:53.000000 help2man-0.0.7/docs/resources/man.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-11 16:56:53.000000 help2man-0.0.7/flake.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-11 16:56:53.000000 help2man-0.0.7/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-11 16:56:53.000000 help2man-0.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.266597 help2man-0.0.7/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      113 2023-04-11 16:56:53.000000 help2man-0.0.7/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-11 16:56:53.000000 help2man-0.0.7/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.266597 help2man-0.0.7/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-11 16:56:53.000000 help2man-0.0.7/scripts/generate-api.md.pl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.270597 help2man-0.0.7/sdist/
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-11 16:57:05.000000 help2man-0.0.7/sdist/_help2man
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-11 16:57:05.000000 help2man-0.0.7/sdist/help2man
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-11 16:57:05.000000 help2man-0.0.7/sdist/help2man.1
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 16:57:05.270597 help2man-0.0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2521 2023-04-11 16:56:53.000000 help2man-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.266597 help2man-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.270597 help2man-0.0.7/src/help2man/
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-04-11 16:56:53.000000 help2man-0.0.7/src/help2man/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3420 2023-04-11 16:56:53.000000 help2man-0.0.7/src/help2man/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 16:57:05.000000 help2man-0.0.7/src/help2man/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.266597 help2man-0.0.7/src/help2man/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.270597 help2man-0.0.7/src/help2man/assets/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-11 16:56:53.000000 help2man-0.0.7/src/help2man/assets/jinja2/template.man.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-11 16:56:53.000000 help2man-0.0.7/src/help2man/assets/jinja2/template.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.270597 help2man-0.0.7/src/help2man/assets/txt/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 16:57:05.000000 help2man-0.0.7/src/help2man/assets/txt/description.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-11 16:57:05.000000 help2man-0.0.7/src/help2man/assets/txt/epilog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 16:57:05.000000 help2man-0.0.7/src/help2man/assets/txt/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.270597 help2man-0.0.7/src/help2man/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-11 16:56:53.000000 help2man-0.0.7/src/help2man/external/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-04-11 16:56:53.000000 help2man-0.0.7/src/help2man/external/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.270597 help2man-0.0.7/src/help2man/external/shtab/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-11 16:56:53.000000 help2man-0.0.7/src/help2man/external/shtab/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1746 2023-04-11 16:56:53.000000 help2man-0.0.7/src/help2man/external/shtab/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:56:53.000000 help2man-0.0.7/src/help2man/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.270597 help2man-0.0.7/src/help2man/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-11 16:56:53.000000 help2man-0.0.7/src/help2man/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-11 16:56:53.000000 help2man-0.0.7/src/help2man/ui/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.270597 help2man-0.0.7/src/help2man.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-11 16:57:05.000000 help2man-0.0.7/src/help2man.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-11 16:57:05.000000 help2man-0.0.7/src/help2man.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:57:05.000000 help2man-0.0.7/src/help2man.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 16:57:05.000000 help2man-0.0.7/src/help2man.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 16:57:05.000000 help2man-0.0.7/src/help2man.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 16:57:05.000000 help2man-0.0.7/src/help2man.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.270597 help2man-0.0.7/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 16:56:53.000000 help2man-0.0.7/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-11 16:56:53.000000 help2man-0.0.7/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 16:56:53.000000 help2man-0.0.7/templates/epilog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 16:56:53.000000 help2man-0.0.7/templates/noarg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 16:56:53.000000 help2man-0.0.7/templates/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.270597 help2man-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-11 16:56:53.000000 help2man-0.0.7/tests/__init___test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-11 16:56:53.000000 help2man-0.0.7/tests/cmd_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:57:05.270597 help2man-0.0.7/tests/txt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-11 16:56:53.000000 help2man-0.0.7/tests/txt/options.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-11 16:56:53.000000 help2man-0.0.7/tests/txt/test.man
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-11 16:56:53.000000 help2man-0.0.7/tests/txt/usage.txt
```

### Comparing `help2man-0.0.6/.github/workflows/main.yml` & `help2man-0.0.7/.github/workflows/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         with:
           files: |
             dist/*
       - uses: pypa/gh-action-pypi-publish@release/v1
         if: startsWith(github.ref, 'refs/tags/') && runner.os == 'Linux'
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
-      - uses: aksh1618/update-aur-package@v1.0.5
+      - uses: Freed-Wu/update-aur-package@v1.0.6
         if: startsWith(github.ref, 'refs/tags/') && runner.os == 'Linux'
         with:
           tag_version_prefix: ""
           package_name: python-help2man
           commit_username: github-action[bot]
           commit_email: 41898282+github-actions[bot]@users.noreply.github.com
           ssh_private_key: ${{ secrets.AUR_SSH_PRIVATE_KEY }}
```

### Comparing `help2man-0.0.6/.gitignore` & `help2man-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/.pre-commit-config.yaml` & `help2man-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/LICENSE` & `help2man-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/PKG-INFO` & `help2man-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: help2man
-Version: 0.0.6
+Version: 0.0.7
 Summary: Convert --help and --version to man page.
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://help2man.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/help2man/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/help2man/issues
 Project-URL: Source, https://github.com/Freed-Wu/help2man
```

### Comparing `help2man-0.0.6/README.md` & `help2man-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/docs/conf.py` & `help2man-0.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/docs/resources/install.md` & `help2man-0.0.7/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/flake.lock` & `help2man-0.0.7/flake.lock`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/flake.nix` & `help2man-0.0.7/flake.nix`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/pyproject.toml` & `help2man-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/sdist/_help2man` & `help2man-0.0.7/sdist/_help2man`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/sdist/help2man` & `help2man-0.0.7/sdist/help2man`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/sdist/help2man.1` & `help2man-0.0.7/sdist/help2man.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-.\" DO NOT MODIFY THIS FILE!  It was generated by help2man 0.0.6.
-.TH HELP2MAN "1" "2023-04-11" "help2man 0.0.6" "User Commands"
+.\" DO NOT MODIFY THIS FILE!  It was generated by help2man 0.0.7.
+.TH HELP2MAN "1" "2023-04-11" "help2man 0.0.7" "User Commands"
 .SH NAME
 help2man \- Convert --help and --version to man page.
 .SH SYNOPSIS
 \&help2man [-h] [-V] [--print-completion {bash,zsh,tcsh}] [-n NAME]
          [-s SECTION] [-m MANUAL] [-S SOURCE] [-p INFO_PAGE]
          [-i INCLUDE] [-o OUTPUT] [--template {man,markdown}]
          [--template-file TEMPLATE_FILE] [--help-option HELP_OPTION]
```

### Comparing `help2man-0.0.6/setup.py` & `help2man-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/src/help2man/__init__.py` & `help2man-0.0.7/src/help2man/__init__.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/src/help2man/__main__.py` & `help2man-0.0.7/src/help2man/__main__.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/src/help2man/assets/jinja2/template.man.j2` & `help2man-0.0.7/src/help2man/assets/jinja2/template.man.j2`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/src/help2man/assets/jinja2/template.md.j2` & `help2man-0.0.7/src/help2man/assets/jinja2/template.md.j2`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/src/help2man/external/__main__.py` & `help2man-0.0.7/src/help2man/external/__main__.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/src/help2man/external/shtab/__main__.py` & `help2man-0.0.7/src/help2man/external/shtab/__main__.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/src/help2man/ui/__init__.py` & `help2man-0.0.7/src/help2man/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/src/help2man/ui/cli.py` & `help2man-0.0.7/src/help2man/ui/cli.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/src/help2man.egg-info/PKG-INFO` & `help2man-0.0.7/src/help2man.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: help2man
-Version: 0.0.6
+Version: 0.0.7
 Summary: Convert --help and --version to man page.
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://help2man.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/help2man/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/help2man/issues
 Project-URL: Source, https://github.com/Freed-Wu/help2man
```

### Comparing `help2man-0.0.6/src/help2man.egg-info/SOURCES.txt` & `help2man-0.0.7/src/help2man.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/tests/__init___test.py` & `help2man-0.0.7/tests/__init___test.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/tests/cmd_test.py` & `help2man-0.0.7/tests/cmd_test.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.6/tests/txt/options.txt` & `help2man-0.0.7/tests/txt/options.txt`

 * *Files identical despite different names*

