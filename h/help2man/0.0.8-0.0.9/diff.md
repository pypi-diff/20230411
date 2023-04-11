# Comparing `tmp/help2man-0.0.8.tar.gz` & `tmp/help2man-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "help2man-0.0.8.tar", last modified: Tue Apr 11 17:01:27 2023, max compression
+gzip compressed data, was "help2man-0.0.9.tar", last modified: Tue Apr 11 17:09:45 2023, max compression
```

## Comparing `help2man-0.0.8.tar` & `help2man-0.0.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.684364 help2man-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.680364 help2man-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-11 17:01:15.000000 help2man-0.0.8/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.680364 help2man-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-11 17:01:15.000000 help2man-0.0.8/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-11 17:01:15.000000 help2man-0.0.8/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-04-11 17:01:15.000000 help2man-0.0.8/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-11 17:01:15.000000 help2man-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-11 17:01:15.000000 help2man-0.0.8/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-11 17:01:15.000000 help2man-0.0.8/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-11 17:01:15.000000 help2man-0.0.8/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 17:01:15.000000 help2man-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-11 17:01:27.684364 help2man-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-04-11 17:01:15.000000 help2man-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.680364 help2man-0.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.680364 help2man-0.0.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 17:01:15.000000 help2man-0.0.8/docs/api/external.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-11 17:01:15.000000 help2man-0.0.8/docs/api/help2man.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 17:01:15.000000 help2man-0.0.8/docs/api/ui.md
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-11 17:01:15.000000 help2man-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-11 17:01:15.000000 help2man-0.0.8/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-11 17:01:15.000000 help2man-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.680364 help2man-0.0.8/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 17:01:15.000000 help2man-0.0.8/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 17:01:15.000000 help2man-0.0.8/docs/resources/man.md
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-11 17:01:15.000000 help2man-0.0.8/flake.lock
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-11 17:01:15.000000 help2man-0.0.8/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-11 17:01:15.000000 help2man-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.680364 help2man-0.0.8/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)      113 2023-04-11 17:01:15.000000 help2man-0.0.8/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-11 17:01:15.000000 help2man-0.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.680364 help2man-0.0.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-11 17:01:15.000000 help2man-0.0.8/scripts/generate-api.md.pl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.680364 help2man-0.0.8/sdist/
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-11 17:01:27.000000 help2man-0.0.8/sdist/_help2man
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-11 17:01:27.000000 help2man-0.0.8/sdist/help2man
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-11 17:01:27.000000 help2man-0.0.8/sdist/help2man.1
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:01:27.684364 help2man-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2521 2023-04-11 17:01:15.000000 help2man-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.676364 help2man-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.680364 help2man-0.0.8/src/help2man/
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-04-11 17:01:15.000000 help2man-0.0.8/src/help2man/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3420 2023-04-11 17:01:15.000000 help2man-0.0.8/src/help2man/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 17:01:27.000000 help2man-0.0.8/src/help2man/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.676364 help2man-0.0.8/src/help2man/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.684364 help2man-0.0.8/src/help2man/assets/jinja2/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-11 17:01:15.000000 help2man-0.0.8/src/help2man/assets/jinja2/template.man.j2
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-11 17:01:15.000000 help2man-0.0.8/src/help2man/assets/jinja2/template.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.684364 help2man-0.0.8/src/help2man/assets/txt/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 17:01:27.000000 help2man-0.0.8/src/help2man/assets/txt/description.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-11 17:01:27.000000 help2man-0.0.8/src/help2man/assets/txt/epilog.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 17:01:27.000000 help2man-0.0.8/src/help2man/assets/txt/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.684364 help2man-0.0.8/src/help2man/external/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-11 17:01:15.000000 help2man-0.0.8/src/help2man/external/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-04-11 17:01:15.000000 help2man-0.0.8/src/help2man/external/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.684364 help2man-0.0.8/src/help2man/external/shtab/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-11 17:01:15.000000 help2man-0.0.8/src/help2man/external/shtab/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1746 2023-04-11 17:01:15.000000 help2man-0.0.8/src/help2man/external/shtab/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:15.000000 help2man-0.0.8/src/help2man/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.684364 help2man-0.0.8/src/help2man/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-11 17:01:15.000000 help2man-0.0.8/src/help2man/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-11 17:01:15.000000 help2man-0.0.8/src/help2man/ui/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.684364 help2man-0.0.8/src/help2man.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-11 17:01:27.000000 help2man-0.0.8/src/help2man.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-11 17:01:27.000000 help2man-0.0.8/src/help2man.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:01:27.000000 help2man-0.0.8/src/help2man.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 17:01:27.000000 help2man-0.0.8/src/help2man.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 17:01:27.000000 help2man-0.0.8/src/help2man.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 17:01:27.000000 help2man-0.0.8/src/help2man.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.684364 help2man-0.0.8/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 17:01:15.000000 help2man-0.0.8/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-11 17:01:15.000000 help2man-0.0.8/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 17:01:15.000000 help2man-0.0.8/templates/epilog.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 17:01:15.000000 help2man-0.0.8/templates/noarg.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 17:01:15.000000 help2man-0.0.8/templates/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.684364 help2man-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-11 17:01:15.000000 help2man-0.0.8/tests/__init___test.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-11 17:01:15.000000 help2man-0.0.8/tests/cmd_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:01:27.684364 help2man-0.0.8/tests/txt/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-11 17:01:15.000000 help2man-0.0.8/tests/txt/options.txt
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-11 17:01:15.000000 help2man-0.0.8/tests/txt/test.man
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-11 17:01:15.000000 help2man-0.0.8/tests/txt/usage.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.463607 help2man-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.451607 help2man-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-11 17:09:32.000000 help2man-0.0.9/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.451607 help2man-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-11 17:09:32.000000 help2man-0.0.9/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-11 17:09:32.000000 help2man-0.0.9/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-04-11 17:09:32.000000 help2man-0.0.9/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-11 17:09:32.000000 help2man-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-11 17:09:32.000000 help2man-0.0.9/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-11 17:09:32.000000 help2man-0.0.9/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-11 17:09:32.000000 help2man-0.0.9/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 17:09:32.000000 help2man-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-11 17:09:45.463607 help2man-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-04-11 17:09:32.000000 help2man-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.451607 help2man-0.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.451607 help2man-0.0.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 17:09:32.000000 help2man-0.0.9/docs/api/external.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-11 17:09:32.000000 help2man-0.0.9/docs/api/help2man.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 17:09:32.000000 help2man-0.0.9/docs/api/ui.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-11 17:09:32.000000 help2man-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-11 17:09:32.000000 help2man-0.0.9/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-11 17:09:32.000000 help2man-0.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.455607 help2man-0.0.9/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 17:09:32.000000 help2man-0.0.9/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 17:09:32.000000 help2man-0.0.9/docs/resources/man.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-11 17:09:32.000000 help2man-0.0.9/flake.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-11 17:09:32.000000 help2man-0.0.9/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-11 17:09:32.000000 help2man-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.455607 help2man-0.0.9/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      113 2023-04-11 17:09:32.000000 help2man-0.0.9/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-11 17:09:32.000000 help2man-0.0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.455607 help2man-0.0.9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-11 17:09:32.000000 help2man-0.0.9/scripts/generate-api.md.pl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.455607 help2man-0.0.9/sdist/
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-11 17:09:45.000000 help2man-0.0.9/sdist/_help2man
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-11 17:09:45.000000 help2man-0.0.9/sdist/help2man
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-11 17:09:45.000000 help2man-0.0.9/sdist/help2man.1
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:09:45.463607 help2man-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2521 2023-04-11 17:09:32.000000 help2man-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.443607 help2man-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.459607 help2man-0.0.9/src/help2man/
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-04-11 17:09:32.000000 help2man-0.0.9/src/help2man/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3420 2023-04-11 17:09:32.000000 help2man-0.0.9/src/help2man/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 17:09:45.000000 help2man-0.0.9/src/help2man/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.443607 help2man-0.0.9/src/help2man/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.459607 help2man-0.0.9/src/help2man/assets/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-11 17:09:32.000000 help2man-0.0.9/src/help2man/assets/jinja2/template.man.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-11 17:09:32.000000 help2man-0.0.9/src/help2man/assets/jinja2/template.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.459607 help2man-0.0.9/src/help2man/assets/txt/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 17:09:45.000000 help2man-0.0.9/src/help2man/assets/txt/description.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-11 17:09:45.000000 help2man-0.0.9/src/help2man/assets/txt/epilog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 17:09:45.000000 help2man-0.0.9/src/help2man/assets/txt/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.459607 help2man-0.0.9/src/help2man/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-11 17:09:32.000000 help2man-0.0.9/src/help2man/external/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-04-11 17:09:32.000000 help2man-0.0.9/src/help2man/external/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.459607 help2man-0.0.9/src/help2man/external/shtab/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-11 17:09:32.000000 help2man-0.0.9/src/help2man/external/shtab/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1746 2023-04-11 17:09:32.000000 help2man-0.0.9/src/help2man/external/shtab/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:32.000000 help2man-0.0.9/src/help2man/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.459607 help2man-0.0.9/src/help2man/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-11 17:09:32.000000 help2man-0.0.9/src/help2man/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-11 17:09:32.000000 help2man-0.0.9/src/help2man/ui/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.459607 help2man-0.0.9/src/help2man.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-11 17:09:45.000000 help2man-0.0.9/src/help2man.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-11 17:09:45.000000 help2man-0.0.9/src/help2man.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:09:45.000000 help2man-0.0.9/src/help2man.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 17:09:45.000000 help2man-0.0.9/src/help2man.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 17:09:45.000000 help2man-0.0.9/src/help2man.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 17:09:45.000000 help2man-0.0.9/src/help2man.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.463607 help2man-0.0.9/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 17:09:32.000000 help2man-0.0.9/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-11 17:09:32.000000 help2man-0.0.9/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 17:09:32.000000 help2man-0.0.9/templates/epilog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 17:09:32.000000 help2man-0.0.9/templates/noarg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 17:09:32.000000 help2man-0.0.9/templates/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.463607 help2man-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-11 17:09:32.000000 help2man-0.0.9/tests/__init___test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-11 17:09:32.000000 help2man-0.0.9/tests/cmd_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:09:45.463607 help2man-0.0.9/tests/txt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-11 17:09:32.000000 help2man-0.0.9/tests/txt/options.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-11 17:09:32.000000 help2man-0.0.9/tests/txt/test.man
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-11 17:09:32.000000 help2man-0.0.9/tests/txt/usage.txt
```

### Comparing `help2man-0.0.8/.github/workflows/main.yml` & `help2man-0.0.9/.github/workflows/main.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -60,28 +60,28 @@
           cache: ${{ env.cache }}
       - name: Install dependencies
         run: |
           pip install build
       - name: Build
         run: |
           python -m build
-      - uses: pypa/gh-action-pypi-publish@release/v1
-        if: startsWith(github.ref, 'refs/tags/') && runner.os == 'Linux'
-        with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
       - uses: actions/upload-artifact@v3
         if: ${{ ! startsWith(github.ref, 'refs/tags/') }}
         with:
           path: |
             dist/*
       - uses: softprops/action-gh-release@v1
         if: startsWith(github.ref, 'refs/tags/') && runner.os != 'Windows'
         with:
           files: |
             dist/*
+      - uses: pypa/gh-action-pypi-publish@release/v1
+        if: startsWith(github.ref, 'refs/tags/') && runner.os == 'Linux'
+        with:
+          password: ${{ secrets.PYPI_API_TOKEN }}
       - uses: Freed-Wu/update-aur-package@v1.0.6
         if: startsWith(github.ref, 'refs/tags/') && runner.os == 'Linux'
         with:
           tag_version_prefix: ""
           package_name: python-help2man
           commit_username: github-action[bot]
           commit_email: 41898282+github-actions[bot]@users.noreply.github.com
```

### Comparing `help2man-0.0.8/.gitignore` & `help2man-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/.pre-commit-config.yaml` & `help2man-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/LICENSE` & `help2man-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/PKG-INFO` & `help2man-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: help2man
-Version: 0.0.8
+Version: 0.0.9
 Summary: Convert --help and --version to man page.
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://help2man.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/help2man/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/help2man/issues
 Project-URL: Source, https://github.com/Freed-Wu/help2man
```

### Comparing `help2man-0.0.8/README.md` & `help2man-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/docs/conf.py` & `help2man-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/docs/resources/install.md` & `help2man-0.0.9/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/flake.lock` & `help2man-0.0.9/flake.lock`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/flake.nix` & `help2man-0.0.9/flake.nix`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/pyproject.toml` & `help2man-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/sdist/_help2man` & `help2man-0.0.9/sdist/_help2man`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/sdist/help2man` & `help2man-0.0.9/sdist/help2man`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/sdist/help2man.1` & `help2man-0.0.9/sdist/help2man.1`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-.\" DO NOT MODIFY THIS FILE!  It was generated by help2man 0.0.8.
-.TH HELP2MAN "1" "2023-04-11" "help2man 0.0.8" "User Commands"
+.\" DO NOT MODIFY THIS FILE!  It was generated by help2man 0.0.9.
+.TH HELP2MAN "1" "2023-04-11" "help2man 0.0.9" "User Commands"
 .SH NAME
 help2man \- Convert --help and --version to man page.
 .SH SYNOPSIS
 \&help2man [-h] [-V] [--print-completion {bash,zsh,tcsh}] [-n NAME]
          [-s SECTION] [-m MANUAL] [-S SOURCE] [-p INFO_PAGE]
          [-i INCLUDE] [-o OUTPUT] [--template {man,markdown}]
          [--template-file TEMPLATE_FILE] [--help-option HELP_OPTION]
```

### Comparing `help2man-0.0.8/setup.py` & `help2man-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/src/help2man/__init__.py` & `help2man-0.0.9/src/help2man/__init__.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/src/help2man/__main__.py` & `help2man-0.0.9/src/help2man/__main__.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/src/help2man/assets/jinja2/template.man.j2` & `help2man-0.0.9/src/help2man/assets/jinja2/template.man.j2`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/src/help2man/assets/jinja2/template.md.j2` & `help2man-0.0.9/src/help2man/assets/jinja2/template.md.j2`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/src/help2man/external/__main__.py` & `help2man-0.0.9/src/help2man/external/__main__.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/src/help2man/external/shtab/__main__.py` & `help2man-0.0.9/src/help2man/external/shtab/__main__.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/src/help2man/ui/__init__.py` & `help2man-0.0.9/src/help2man/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/src/help2man/ui/cli.py` & `help2man-0.0.9/src/help2man/ui/cli.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/src/help2man.egg-info/PKG-INFO` & `help2man-0.0.9/src/help2man.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: help2man
-Version: 0.0.8
+Version: 0.0.9
 Summary: Convert --help and --version to man page.
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://help2man.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/help2man/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/help2man/issues
 Project-URL: Source, https://github.com/Freed-Wu/help2man
```

### Comparing `help2man-0.0.8/src/help2man.egg-info/SOURCES.txt` & `help2man-0.0.9/src/help2man.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/tests/__init___test.py` & `help2man-0.0.9/tests/__init___test.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/tests/cmd_test.py` & `help2man-0.0.9/tests/cmd_test.py`

 * *Files identical despite different names*

### Comparing `help2man-0.0.8/tests/txt/options.txt` & `help2man-0.0.9/tests/txt/options.txt`

 * *Files identical despite different names*

