# Comparing `tmp/thermoextrap-0.2.2.tar.gz` & `tmp/thermoextrap-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thermoextrap-0.2.2.tar", last modified: Thu Apr  6 00:53:08 2023, max compression
+gzip compressed data, was "thermoextrap-0.2.3.tar", last modified: Tue Apr 11 03:03:46 2023, max compression
```

## Comparing `thermoextrap-0.2.2.tar` & `thermoextrap-0.2.3.tar`

### file list

```diff
@@ -1,88 +1,86 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:53:08.780643 thermoextrap-0.2.2/
--rw-r--r--   0 wpk      (42033)    36681     1381 2023-04-06 00:51:43.000000 thermoextrap-0.2.2/.cruft.json
--rw-r--r--   0 wpk      (42033)    36681     1346 2023-03-29 02:34:47.000000 thermoextrap-0.2.2/.gitignore
--rw-r--r--   0 wpk      (42033)    36681     2891 2023-04-06 00:51:43.000000 thermoextrap-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681      163 2023-03-29 02:34:47.000000 thermoextrap-0.2.2/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681     6773 2023-03-31 00:02:24.000000 thermoextrap-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681       59 2023-03-29 02:34:47.000000 thermoextrap-0.2.2/HISTORY.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2023-03-29 02:34:47.000000 thermoextrap-0.2.2/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      267 2023-03-29 02:34:47.000000 thermoextrap-0.2.2/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681     8464 2023-04-06 00:51:43.000000 thermoextrap-0.2.2/Makefile
--rw-r--r--   0 wpk      (42033)    36681     8070 2023-04-06 00:53:08.781024 thermoextrap-0.2.2/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     5160 2023-03-31 00:02:24.000000 thermoextrap-0.2.2/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:53:08.734924 thermoextrap-0.2.2/environment/
--rw-r--r--   0 wpk      (42033)    36681       11 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/environment/conda-spec.txt
--rw-r--r--   0 wpk      (42033)    36681     1095 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      339 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/environment/dev.yaml
--rw-r--r--   0 wpk      (42033)    36681      120 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681       76 2023-04-06 00:51:43.000000 thermoextrap-0.2.2/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      692 2023-04-06 00:51:43.000000 thermoextrap-0.2.2/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      470 2023-04-06 00:51:43.000000 thermoextrap-0.2.2/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681       40 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      256 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      337 2023-02-15 21:32:10.000000 thermoextrap-0.2.2/environment.yaml
--rw-r--r--   0 wpk      (42033)    36681     4808 2023-04-06 00:51:43.000000 thermoextrap-0.2.2/pyproject.toml
--rw-r--r--   0 wpk      (42033)    36681      398 2023-04-06 00:53:08.782269 thermoextrap-0.2.2/setup.cfg
--rw-r--r--   0 wpk      (42033)    36681      323 2023-04-06 00:51:43.000000 thermoextrap-0.2.2/setup.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:53:08.720146 thermoextrap-0.2.2/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:53:08.740377 thermoextrap-0.2.2/src/thermoextrap/
--rw-r--r--   0 wpk      (42033)    36681     1560 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/__init__.py
--rw-r--r--   0 wpk      (42033)    36681    18793 2023-03-31 00:02:24.000000 thermoextrap-0.2.2/src/thermoextrap/adaptive_interp.py
--rw-r--r--   0 wpk      (42033)    36681    17305 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/beta.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:53:08.749404 thermoextrap-0.2.2/src/thermoextrap/core/
--rw-r--r--   0 wpk      (42033)    36681      134 2023-03-30 11:25:22.000000 thermoextrap-0.2.2/src/thermoextrap/core/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     4998 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/core/_attrs_utils.py
--rw-r--r--   0 wpk      (42033)    36681    12107 2023-03-31 00:02:24.000000 thermoextrap-0.2.2/src/thermoextrap/core/_deprecate.py
--rw-r--r--   0 wpk      (42033)    36681     8229 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/core/_docstrings.py
--rw-r--r--   0 wpk      (42033)    36681     5672 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/core/cached_decorators.py
--rw-r--r--   0 wpk      (42033)    36681    52841 2023-03-31 00:02:24.000000 thermoextrap-0.2.2/src/thermoextrap/core/data.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:53:08.751428 thermoextrap-0.2.2/src/thermoextrap/core/external/
--rw-r--r--   0 wpk      (42033)    36681       23 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/core/external/__init__.py
--rw-r--r--   0 wpk      (42033)    36681    19656 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/core/external/docfiller.py
--rw-r--r--   0 wpk      (42033)    36681    23537 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/core/external/docscrape.py
--rw-r--r--   0 wpk      (42033)    36681    10298 2023-03-31 00:02:24.000000 thermoextrap-0.2.2/src/thermoextrap/core/idealgas.py
--rw-r--r--   0 wpk      (42033)    36681    32148 2023-03-31 00:02:24.000000 thermoextrap-0.2.2/src/thermoextrap/core/models.py
--rw-r--r--   0 wpk      (42033)    36681      322 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/core/sputils.py
--rw-r--r--   0 wpk      (42033)    36681    18816 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/core/stack.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:53:08.753083 thermoextrap-0.2.2/src/thermoextrap/core/tmp/
--rw-r--r--   0 wpk      (42033)    36681     5676 2022-10-28 20:31:54.000000 thermoextrap-0.2.2/src/thermoextrap/core/tmp/_docfiller.py
--rw-r--r--   0 wpk      (42033)    36681    10332 2023-02-13 21:54:21.000000 thermoextrap-0.2.2/src/thermoextrap/core/tmp/_docstrings.py
--rw-r--r--   0 wpk      (42033)    36681     3159 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/core/xrutils.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:53:08.757472 thermoextrap-0.2.2/src/thermoextrap/gpr_active/
--rw-r--r--   0 wpk      (42033)    36681      717 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/gpr_active/__init__.py
--rw-r--r--   0 wpk      (42033)    36681    88989 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/gpr_active/active_utils.py
--rw-r--r--   0 wpk      (42033)    36681    56361 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/gpr_active/gp_models.py
--rw-r--r--   0 wpk      (42033)    36681     3386 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/gpr_active/ig_active.py
--rw-r--r--   0 wpk      (42033)    36681     3003 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/gpr_active/sine_active.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:53:08.766287 thermoextrap-0.2.2/src/thermoextrap/legacy/
--rw-r--r--   0 wpk      (42033)    36681      629 2023-02-14 18:08:06.000000 thermoextrap-0.2.2/src/thermoextrap/legacy/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     9563 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/legacy/extrap.py
--rw-r--r--   0 wpk      (42033)    36681    18316 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/legacy/gpr.py
--rw-r--r--   0 wpk      (42033)    36681    16856 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/legacy/gpr_stack.py
--rw-r--r--   0 wpk      (42033)    36681     5547 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/legacy/ig.py
--rw-r--r--   0 wpk      (42033)    36681    16626 2023-02-14 18:08:06.000000 thermoextrap-0.2.2/src/thermoextrap/legacy/interp.py
--rw-r--r--   0 wpk      (42033)    36681     9580 2023-02-14 18:08:06.000000 thermoextrap-0.2.2/src/thermoextrap/legacy/old_scripts.py
--rw-r--r--   0 wpk      (42033)    36681    21063 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/legacy/recursive_interp.py
--rw-r--r--   0 wpk      (42033)    36681     8609 2023-02-14 18:08:06.000000 thermoextrap-0.2.2/src/thermoextrap/legacy/reweight.py
--rw-r--r--   0 wpk      (42033)    36681    10983 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/legacy/utilities.py
--rw-r--r--   0 wpk      (42033)    36681    13021 2023-03-31 00:02:24.000000 thermoextrap-0.2.2/src/thermoextrap/lnpi.py
--rw-r--r--   0 wpk      (42033)    36681    21936 2023-03-31 00:02:24.000000 thermoextrap-0.2.2/src/thermoextrap/recursive_interp.py
--rw-r--r--   0 wpk      (42033)    36681     5855 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/volume.py
--rw-r--r--   0 wpk      (42033)    36681     4391 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/src/thermoextrap/volume_idealgas.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:53:08.780143 thermoextrap-0.2.2/src/thermoextrap.egg-info/
--rw-r--r--   0 wpk      (42033)    36681     2048 2023-04-06 00:53:08.000000 thermoextrap-0.2.2/src/thermoextrap.egg-info/SOURCES.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:53:08.775968 thermoextrap-0.2.2/tests/
--rw-r--r--   0 wpk      (42033)    36681     9121 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/tests/conftest.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 00:53:08.776856 thermoextrap-0.2.2/tests/lnpi_data/
--rw-r--r--   0 wpk      (42033)    36681   667972 2023-02-14 18:08:06.000000 thermoextrap-0.2.2/tests/lnpi_data/sample_data.json
--rw-r--r--   0 wpk      (42033)    36681    23103 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/tests/test_GPs.py
--rw-r--r--   0 wpk      (42033)    36681    25332 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/tests/test_active.py
--rw-r--r--   0 wpk      (42033)    36681    32495 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/tests/test_beta.py
--rw-r--r--   0 wpk      (42033)    36681     2259 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/tests/test_data.py
--rw-r--r--   0 wpk      (42033)    36681     1421 2023-02-14 18:08:06.000000 thermoextrap-0.2.2/tests/test_idealgas.py
--rw-r--r--   0 wpk      (42033)    36681     3437 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/tests/test_lnPi.py
--rw-r--r--   0 wpk      (42033)    36681     2099 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/tests/test_stack.py
--rw-r--r--   0 wpk      (42033)    36681     7641 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/tests/test_u_data.py
--rw-r--r--   0 wpk      (42033)    36681     2051 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/tests/test_u_equations.py
--rw-r--r--   0 wpk      (42033)    36681     2703 2023-03-29 02:34:48.000000 thermoextrap-0.2.2/tests/test_volume.py
--rw-r--r--   0 wpk      (42033)    36681     4193 2023-03-31 00:02:24.000000 thermoextrap-0.2.2/tox.ini
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.944791 thermoextrap-0.2.3/
+-rw-r--r--   0 wpk      (42033)    36681     1869 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/.cruft.json
+-rw-r--r--   0 wpk      (42033)    36681     1373 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/.gitignore
+-rw-r--r--   0 wpk      (42033)    36681      104 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/.gitmodules
+-rw-r--r--   0 wpk      (42033)    36681     2901 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033)    36681      163 2023-04-10 21:01:10.000000 thermoextrap-0.2.3/AUTHORS.md
+-rw-r--r--   0 wpk      (42033)    36681     6909 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033)    36681       59 2023-04-10 21:01:10.000000 thermoextrap-0.2.3/HISTORY.md
+-rw-r--r--   0 wpk      (42033)    36681     1645 2023-04-10 21:01:10.000000 thermoextrap-0.2.3/LICENSE
+-rw-r--r--   0 wpk      (42033)    36681      266 2023-04-11 03:00:42.000000 thermoextrap-0.2.3/MANIFEST.in
+-rw-r--r--   0 wpk      (42033)    36681     8464 2023-04-10 21:01:10.000000 thermoextrap-0.2.3/Makefile
+-rw-r--r--   0 wpk      (42033)    36681     8307 2023-04-11 03:03:46.945126 thermoextrap-0.2.3/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     5401 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.912608 thermoextrap-0.2.3/environment/
+-rw-r--r--   0 wpk      (42033)    36681       11 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/environment/conda-spec.txt
+-rw-r--r--   0 wpk      (42033)    36681     1095 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      345 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033)    36681      120 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033)    36681       87 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033)    36681      692 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      476 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033)    36681       40 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      262 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/environment/test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      343 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/environment.yaml
+-rw-r--r--   0 wpk      (42033)    36681     4872 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/pyproject.toml
+-rw-r--r--   0 wpk      (42033)    36681      397 2023-04-11 03:03:46.946361 thermoextrap-0.2.3/setup.cfg
+-rw-r--r--   0 wpk      (42033)    36681      323 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/setup.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.901302 thermoextrap-0.2.3/src/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.915495 thermoextrap-0.2.3/src/thermoextrap/
+-rw-r--r--   0 wpk      (42033)    36681     1560 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681    18804 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/src/thermoextrap/adaptive_interp.py
+-rw-r--r--   0 wpk      (42033)    36681    17305 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/beta.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.921839 thermoextrap-0.2.3/src/thermoextrap/core/
+-rw-r--r--   0 wpk      (42033)    36681      134 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     4998 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/_attrs_utils.py
+-rw-r--r--   0 wpk      (42033)    36681    12082 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/src/thermoextrap/core/_deprecate.py
+-rw-r--r--   0 wpk      (42033)    36681     8229 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/_docstrings.py
+-rw-r--r--   0 wpk      (42033)    36681     5672 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/cached_decorators.py
+-rw-r--r--   0 wpk      (42033)    36681    52840 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/src/thermoextrap/core/data.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.923918 thermoextrap-0.2.3/src/thermoextrap/core/external/
+-rw-r--r--   0 wpk      (42033)    36681       23 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/external/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681    19656 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/external/docfiller.py
+-rw-r--r--   0 wpk      (42033)    36681    23537 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/external/docscrape.py
+-rw-r--r--   0 wpk      (42033)    36681    10298 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/idealgas.py
+-rw-r--r--   0 wpk      (42033)    36681    32148 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/models.py
+-rw-r--r--   0 wpk      (42033)    36681      322 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/sputils.py
+-rw-r--r--   0 wpk      (42033)    36681    18816 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/stack.py
+-rw-r--r--   0 wpk      (42033)    36681     3159 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/xrutils.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.927418 thermoextrap-0.2.3/src/thermoextrap/gpr_active/
+-rw-r--r--   0 wpk      (42033)    36681      717 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/gpr_active/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681    88989 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/gpr_active/active_utils.py
+-rw-r--r--   0 wpk      (42033)    36681    56361 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/gpr_active/gp_models.py
+-rw-r--r--   0 wpk      (42033)    36681     3386 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/gpr_active/ig_active.py
+-rw-r--r--   0 wpk      (42033)    36681     3003 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/gpr_active/sine_active.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.934091 thermoextrap-0.2.3/src/thermoextrap/legacy/
+-rw-r--r--   0 wpk      (42033)    36681      629 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     9563 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/extrap.py
+-rw-r--r--   0 wpk      (42033)    36681    18316 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/gpr.py
+-rw-r--r--   0 wpk      (42033)    36681    16856 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/gpr_stack.py
+-rw-r--r--   0 wpk      (42033)    36681     5547 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/ig.py
+-rw-r--r--   0 wpk      (42033)    36681    16626 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/interp.py
+-rw-r--r--   0 wpk      (42033)    36681     9580 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/old_scripts.py
+-rw-r--r--   0 wpk      (42033)    36681    21063 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/recursive_interp.py
+-rw-r--r--   0 wpk      (42033)    36681     8609 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/reweight.py
+-rw-r--r--   0 wpk      (42033)    36681    10983 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/utilities.py
+-rw-r--r--   0 wpk      (42033)    36681    13032 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/src/thermoextrap/lnpi.py
+-rw-r--r--   0 wpk      (42033)    36681    21947 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/src/thermoextrap/recursive_interp.py
+-rw-r--r--   0 wpk      (42033)    36681     5855 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/volume.py
+-rw-r--r--   0 wpk      (42033)    36681     4391 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/volume_idealgas.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.944403 thermoextrap-0.2.3/src/thermoextrap.egg-info/
+-rw-r--r--   0 wpk      (42033)    36681     1979 2023-04-11 03:03:46.000000 thermoextrap-0.2.3/src/thermoextrap.egg-info/SOURCES.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.941969 thermoextrap-0.2.3/tests/
+-rw-r--r--   0 wpk      (42033)    36681     9121 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/conftest.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.942599 thermoextrap-0.2.3/tests/lnpi_data/
+-rw-r--r--   0 wpk      (42033)    36681   667972 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/lnpi_data/sample_data.json
+-rw-r--r--   0 wpk      (42033)    36681    23103 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_GPs.py
+-rw-r--r--   0 wpk      (42033)    36681    25332 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_active.py
+-rw-r--r--   0 wpk      (42033)    36681    32495 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_beta.py
+-rw-r--r--   0 wpk      (42033)    36681     2259 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_data.py
+-rw-r--r--   0 wpk      (42033)    36681     1421 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_idealgas.py
+-rw-r--r--   0 wpk      (42033)    36681     3437 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_lnPi.py
+-rw-r--r--   0 wpk      (42033)    36681     2099 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_stack.py
+-rw-r--r--   0 wpk      (42033)    36681     7641 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_u_data.py
+-rw-r--r--   0 wpk      (42033)    36681     2051 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_u_equations.py
+-rw-r--r--   0 wpk      (42033)    36681     2703 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_volume.py
+-rw-r--r--   0 wpk      (42033)    36681     4245 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/tox.ini
```

### Comparing `thermoextrap-0.2.2/.cruft.json` & `thermoextrap-0.2.3/.cruft.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8734335839598998%*

 * *Differences: {"'commit'": "'be1b9cec709f862f8de5132e517a42db90758f04'",*

 * * "'context'": "{'cookiecutter': {'project_name': 'thermoextrap', '_copy_without_render': {insert: "*

 * *              "[(4, 'docs/_static/*'), (5, 'docs/_static/css/*'), (6, 'docs/_static/js/*')]}}}",*

 * * "'skip'": "{insert: [(7, 'environment/dev-extras.yaml'), (8, 'environment/docs-extras.yaml'), (9, "*

 * *           "'environment/test-extras.yaml'), (10, 'docs/index.md'), (11, 'docs/installation.md'), "*

 * *           "(12, '.gitignore')], delete: [7]}"}*

```diff
@@ -1,27 +1,30 @@
 {
     "checkout": "feature/markdown",
-    "commit": "c209d4c07a6142de87d6b1600f7319ebc69729cd",
+    "commit": "be1b9cec709f862f8de5132e517a42db90758f04",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
                 "docs/_templates/autosummary/*.rst",
-                "docs/_templates/autodocsumm/*.rst"
+                "docs/_templates/autodocsumm/*.rst",
+                "docs/_static/*",
+                "docs/_static/css/*",
+                "docs/_static/js/*"
             ],
             "_template": "https://github.com/wpk-nist-gov/cookiecutter-pypackage.git",
             "command_line_interface": "No command-line interface",
             "conda_channel": "wpk-nist",
             "create_author_file": "y",
             "email": "wpk@nist.gov",
             "full_name": "William P. Krekelberg",
             "github_username": "usnistgov",
             "open_source_license": "NIST license",
-            "project_name": "thermo-extrap",
+            "project_name": "thermoextrap",
             "project_short_description": "Thermodynamic extrapolation",
             "project_slug": "thermoextrap",
             "pypi_username": "wpk-nist",
             "sphinx_auto": "autosummary",
             "sphinx_theme": "sphinx_book_theme",
             "sphinx_use_autodocsumm": "y",
             "use_pypi_deployment_with_travis": "n",
@@ -34,11 +37,16 @@
         "src/thermoextrap/__init__.py",
         "environment.yaml",
         "HISTORY.md",
         "AUTHORS.md",
         "MANIFEST.in",
         "README.md",
         "docs/spelling_wordlist.txt",
-        "environment/"
+        "environment/dev-extras.yaml",
+        "environment/docs-extras.yaml",
+        "environment/test-extras.yaml",
+        "docs/index.md",
+        "docs/installation.md",
+        ".gitignore"
     ],
     "template": "https://github.com/wpk-nist-gov/cookiecutter-pypackage.git"
 }
```

### Comparing `thermoextrap-0.2.2/.gitignore` & `thermoextrap-0.2.3/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -108,7 +108,8 @@
 .autoenv.zsh
 .autoenv_leave.zsh
 /docs/generated/
 /monkeytype.sqlite3
 /dist-conda/
 /cruft.patch
 /docs/jupyter_execute/
+/docs/reference/generated/
```

### Comparing `thermoextrap-0.2.2/.pre-commit-config.yaml` & `thermoextrap-0.2.3/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
   #       args: [--in-place]
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         stages: [manual]
         additional_dependencies: [flake8-docstrings]
-        exclude: ^tests/|docs/notebooks/gpr/|src/thermoextrap/legacy/|^docs/conf.py|^setup.py
+        exclude: ^tests/|examples/gpr_active_learning/|src/thermoextrap/legacy/|^docs/conf.py|^setup.py
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.1.1
     hooks:
       - id: mypy
         # `properies` & `asv_bench` are copied from setup.cfg.
         # `_typed_ops.py` is added since otherwise mypy will complain (but notably only in pre-commit)
         exclude: properties|asv_bench|_typed_ops.py|conf.py
```

### Comparing `thermoextrap-0.2.2/CONTRIBUTING.md` & `thermoextrap-0.2.3/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 You can contribute in many ways:
 
 ## Types of Contributions
 
 ### Report Bugs
 
-Report bugs at <https://github.com/usnistgov/thermo-extrap/issues>.
+Report bugs at <https://github.com/usnistgov/thermoextrap/issues>.
 
 If you are reporting a bug, please include:
 
 - Your operating system name and version.
 - Any details about your local setup that might be helpful in troubleshooting.
 - Detailed steps to reproduce the bug.
 
@@ -25,21 +25,21 @@
 ### Implement Features
 
 Look through the GitHub issues for features. Anything tagged with "enhancement"
 and "help wanted" is open to whoever wants to implement it.
 
 ### Write Documentation
 
-`thermo-extrap` could always use more documentation, whether as part of the
-official `thermo-extrap` docs, in docstrings, or even on the web in blog posts,
+`thermoextrap` could always use more documentation, whether as part of the
+official `thermoextrap` docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 ### Submit Feedback
 
-The best way to send feedback is to file an issue at <https://github.com/usnistgov/thermo-extrap/issues>.
+The best way to send feedback is to file an issue at <https://github.com/usnistgov/thermoextrap/issues>.
 
 If you are proposing a feature:
 
 - Explain in detail how it would work.
 - Keep the scope as narrow as possible, to make it easier to implement.
 - Remember that this is a volunteer-driven project, and that contributions
   are welcome :)
@@ -90,15 +90,21 @@
 
 2. Clone your fork locally:
 
     ```bash
     git clone git@github.com:your_name_here/thermoextrap.git
     ```
 
-3. Create development environment.  Using the makefile will install a development version using mamba.
+    The example notebooks require the `examples/data` submodule to be loaded.
+
+    ```bash
+    git submodule update --init --recursive
+    ```
+
+3. Create development environment.  Using the `make` will install a development version using mamba.
 
     ```bash
     make mamba-dev
     ```
 
 4. Initiate pre-commit with:
 
@@ -147,15 +153,15 @@
 
     To test against multiple python versions, use tox:
 
     ```bash
     tox
     ```
 
-    or using the makefile:
+    or using the `make`:
 
     ```bash
     make test-all
     ```
 
 
 09. Commit your changes and push your branch to GitHub:
```

### Comparing `thermoextrap-0.2.2/LICENSE` & `thermoextrap-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/Makefile` & `thermoextrap-0.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/PKG-INFO` & `thermoextrap-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: thermoextrap
-Version: 0.2.2
+Version: 0.2.3
 Summary: Thermodynamic extrapolation
-Home-page: https://github.com/usnistgov/thermo-extrap
+Home-page: https://github.com/usnistgov/thermoextrap
 Author-email: Jacob Monroe <jacob.monroe@nist.gov>, William Krekelberg <wpk@nist.gov>
 License: "NIST license https://www.nist.gov/director/licensing"
-Project-URL: homepage, https://github.com/usnistgov/thermo-extrap
-Project-URL: documentation, https://pages.nist.gov/thermo-extrap/
-Keywords: thermo-extrap
+Project-URL: homepage, https://github.com/usnistgov/thermoextrap
+Project-URL: documentation, https://pages.nist.gov/thermoextrap/
+Keywords: thermoextrap
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -38,33 +38,33 @@
 [![Conda (channel only)][conda-badge]][conda-link]
 [![Code style: black][black-badge]][black-link]
 
 
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]: https://github.com/ambv/black
 [pypi-badge]: https://img.shields.io/pypi/v/thermoextrap
-<!-- [pypi-badge]: https://badge.fury.io/py/thermo-extrap -->
+<!-- [pypi-badge]: https://badge.fury.io/py/thermoextrap -->
 [pypi-link]: https://pypi.org/project/thermoextrap
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
-[docs-link]: https://pages.nist.gov/thermo-extrap/
+[docs-link]: https://pages.nist.gov/thermoextrap/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
-[repo-link]: https://github.com/usnistgov/thermo-extrap
+[repo-link]: https://github.com/usnistgov/thermoextrap
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/thermoextrap
 [conda-link]: https://anaconda.org/wpk-nist/thermoextrap
 <!-- Use total link so works from anywhere -->
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
-[license-link]: https://github.com/usnistgov/thermo-extrap/blob/master/LICENSE
+[license-link]: https://github.com/usnistgov/thermoextrap/blob/master/LICENSE
 <!-- For more badges, see https://shields.io/category/other and https://naereen.github.io/badges/ -->
 
 [numpy]: https://numpy.org
 [Numba]: https://numba.pydata.org/
 [xarray]: https://docs.xarray.dev/en/stable/
 [cmomy]: https://github.com/usnistgov/cmomy
-[gpr-link]: https://github.com/usnistgov/thermo-extrap/tree/master/docs/notebooks/gpr
-[notebook-link]: https://github.com/usnistgov/thermo-extrap/tree/master/docs/notebooks
+[gpr-link]: https://github.com/usnistgov/thermoextrap/tree/master/examples/gpr_active_learning
+[notebook-link]: https://github.com/usnistgov/thermoextrap/tree/master/examples/usage
 
 
 
 # `thermoextrap`: Thermodynamic Extrapolation/Interpolation Library
 
 This repository contains code used and described in references [^fn1] [^fn2].
 
@@ -121,35 +121,46 @@
 ```
 
 If you install `thermoextrap` with conda, there are additional optional dependencies that take some care for installation.  We recommend installing the following via `pip`, as the versions on the conda/conda-forge channels are often a bit old.
 ```bash
 pip install tensorflow tensorflow-probability gpflow
 ```
 
+To install from source do the following:
+```bash
+git clone git@github.com:usnistgov/thermoextrap.git
+cd thermoextrap
+pip install . [-e]
+```
+
+To (optionally) include the example data do the following:
+```bash
+git submodule update --init  --recursive
+```
+
+
 ## Example usage
 
 ```python
 import thermoextrap
 
 ```
 
 <!-- end-docs -->
 
 ## Documentation
 
-See the [documentation][docs-link] for a look at `thermo-extrap` in action.
+See the [documentation][docs-link] for a look at `thermoextrap` in action.
 
-To have a look at using `thermo-extrap` with Gaussian process regression, look in the [gpr][docs/notebooks/gpr] directory.
+To have a look at using `thermoextrap` with Gaussian process regression, look in the [gpr][docs/notebooks/gpr] directory.
 
 ## License
 
 This is free software.  See [LICENSE][license-link].
 
-## Related wor
-
 ## Related work
 
 This package extensively uses the [cmomy] package to handle central comoments.
 
 
 # Contact
 Questions may be addressed to Bill Krekelberg at william.krekelberg@nist.gov or Jacob Monroe at jacob.monroe@uark.edu.
```

### Comparing `thermoextrap-0.2.2/README.md` & `thermoextrap-0.2.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 [![Conda (channel only)][conda-badge]][conda-link]
 [![Code style: black][black-badge]][black-link]
 
 
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]: https://github.com/ambv/black
 [pypi-badge]: https://img.shields.io/pypi/v/thermoextrap
-<!-- [pypi-badge]: https://badge.fury.io/py/thermo-extrap -->
+<!-- [pypi-badge]: https://badge.fury.io/py/thermoextrap -->
 [pypi-link]: https://pypi.org/project/thermoextrap
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
-[docs-link]: https://pages.nist.gov/thermo-extrap/
+[docs-link]: https://pages.nist.gov/thermoextrap/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
-[repo-link]: https://github.com/usnistgov/thermo-extrap
+[repo-link]: https://github.com/usnistgov/thermoextrap
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/thermoextrap
 [conda-link]: https://anaconda.org/wpk-nist/thermoextrap
 <!-- Use total link so works from anywhere -->
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
-[license-link]: https://github.com/usnistgov/thermo-extrap/blob/master/LICENSE
+[license-link]: https://github.com/usnistgov/thermoextrap/blob/master/LICENSE
 <!-- For more badges, see https://shields.io/category/other and https://naereen.github.io/badges/ -->
 
 [numpy]: https://numpy.org
 [Numba]: https://numba.pydata.org/
 [xarray]: https://docs.xarray.dev/en/stable/
 [cmomy]: https://github.com/usnistgov/cmomy
-[gpr-link]: https://github.com/usnistgov/thermo-extrap/tree/master/docs/notebooks/gpr
-[notebook-link]: https://github.com/usnistgov/thermo-extrap/tree/master/docs/notebooks
+[gpr-link]: https://github.com/usnistgov/thermoextrap/tree/master/examples/gpr_active_learning
+[notebook-link]: https://github.com/usnistgov/thermoextrap/tree/master/examples/usage
 
 
 
 # `thermoextrap`: Thermodynamic Extrapolation/Interpolation Library
 
 This repository contains code used and described in references [^fn1] [^fn2].
 
@@ -88,35 +88,46 @@
 ```
 
 If you install `thermoextrap` with conda, there are additional optional dependencies that take some care for installation.  We recommend installing the following via `pip`, as the versions on the conda/conda-forge channels are often a bit old.
 ```bash
 pip install tensorflow tensorflow-probability gpflow
 ```
 
+To install from source do the following:
+```bash
+git clone git@github.com:usnistgov/thermoextrap.git
+cd thermoextrap
+pip install . [-e]
+```
+
+To (optionally) include the example data do the following:
+```bash
+git submodule update --init  --recursive
+```
+
+
 ## Example usage
 
 ```python
 import thermoextrap
 
 ```
 
 <!-- end-docs -->
 
 ## Documentation
 
-See the [documentation][docs-link] for a look at `thermo-extrap` in action.
+See the [documentation][docs-link] for a look at `thermoextrap` in action.
 
-To have a look at using `thermo-extrap` with Gaussian process regression, look in the [gpr][docs/notebooks/gpr] directory.
+To have a look at using `thermoextrap` with Gaussian process regression, look in the [gpr][docs/notebooks/gpr] directory.
 
 ## License
 
 This is free software.  See [LICENSE][license-link].
 
-## Related wor
-
 ## Related work
 
 This package extensively uses the [cmomy] package to handle central comoments.
 
 
 # Contact
 Questions may be addressed to Bill Krekelberg at william.krekelberg@nist.gov or Jacob Monroe at jacob.monroe@uark.edu.
```

### Comparing `thermoextrap-0.2.2/environment/dev-extras.yaml` & `thermoextrap-0.2.3/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/environment/docs-extras.yaml` & `thermoextrap-0.2.3/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/pyproject.toml` & `thermoextrap-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = [
     "setuptools>=61.2",
-    "setuptools_scm[toml]>=3.4",
+    "setuptools_scm[toml]>=7.0",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "thermoextrap"
 authors = [{name = "Jacob Monroe", email = "jacob.monroe@nist.gov"}, {name = "William Krekelberg", email="wpk@nist.gov"}]
 license = {text = '"NIST license https://www.nist.gov/director/licensing"'}
 description = "Thermodynamic extrapolation"
 # if using markdown
 # long_description_content_type = text/markdown
-keywords = ["thermo-extrap"]
+keywords = ["thermoextrap"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: Public Domain",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -36,16 +36,16 @@
     "cmomy >= 0.1.9",
     "custom-inherit",
     "attrs",
 ]
 
 
 [project.urls]
-homepage = "https://github.com/usnistgov/thermo-extrap"
-documentation = "https://pages.nist.gov/thermo-extrap/"
+homepage = "https://github.com/usnistgov/thermoextrap"
+documentation = "https://pages.nist.gov/thermoextrap/"
 
 [project.optional-dependencies]
 accel = ["bottleneck"]
 parallel = ["dask[complete]"]
 viz = ["matplotlib"]
 mbar = ["pymbar<4.0"]
 gpr = [
@@ -67,21 +67,23 @@
 # dev = []
 # docs = []
 
 ## Defer this to setup.cfg
 ## Will transition when everything works (grayskull in particular)
 ## and will remove setup.py
 # [tool.setuptools]
-# zip-safe = true
+# zip-safe = true # if using mypy, must be False
 # include-package-data = true
 # license-files = ["LICENSE"]
 
 # [tool.setuptools.packages.find]
 # namespaces = true
 # where = ["src"]
+## include = []
+## exclude = []
 
 [tool.setuptools.dynamic]
 readme = {file = ["README.md", "HISTORY.md", "LICENSE"], content-type = "text/markdown"}
 
 [tool.setuptools_scm]
 fallback_version = "999"
 
@@ -110,15 +112,15 @@
   "E",
   "W",
   # isort
   "I",
   # pyupgrade
   "UP",
   # pydocstyle
-  "D"
+  "D",
   # # flake8-2020
   # "YTT",
   # # flake8-bugbear
   # "B",
   # # flake8-quotes
   # "Q",
   # # pylint
@@ -132,15 +134,15 @@
   # # type-checking imports
   # "TCH",
 ]
 
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 # fixable = ["A", "B", "C", "D", "E", "F", "..."]
-unfixable = ["D"]
+unfixable = []
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
@@ -160,16 +162,15 @@
     "dist",
     "node_modules",
     "venv",
     "docs/conf.py",
     "src/thermoextrap/tests",
     "tests/",
     "src/thermoextrap/legacy/",
-    "docs/notebooks/gpr/",
-
+    "examples/gpr_active_learning/",
 ]
 
 
 ignore = [
     # # whitespace before ':' - doesn't work well with black
     # "E203",
     # module level import not at top of file
@@ -193,21 +194,18 @@
     "D103",
     # these are useful, but too many errors
     # due to use of docfiller
     "D417",
     "D107",
     "D203",
     "D212",
-
 ]
 
 per-file-ignores = {}
 
-
-
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 [tool.ruff.isort]
 known-first-party = ["thermoextrap"]
 
 [tool.ruff.mccabe]
```

### Comparing `thermoextrap-0.2.2/src/thermoextrap/__init__.py` & `thermoextrap-0.2.3/src/thermoextrap/__init__.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/adaptive_interp.py` & `thermoextrap-0.2.3/src/thermoextrap/adaptive_interp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Adaptive interpolation (:mod:`~thermoextrap.adaptive_interp`)
 =============================================================
 
 Holds recursive interpolation class.
 This includes the recursive training algorithm and consistency checks.
 
-See :ref:`notebooks/temperature_interp:adaptive interpolation` for example usage.
+See :ref:`examples/usage/basic/temperature_interp:adaptive interpolation` for example usage.
 
 """
 
 
 from itertools import chain, islice
 
 import numpy as np
```

### Comparing `thermoextrap-0.2.2/src/thermoextrap/beta.py` & `thermoextrap-0.2.3/src/thermoextrap/beta.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/core/_attrs_utils.py` & `thermoextrap-0.2.3/src/thermoextrap/core/_attrs_utils.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/core/_deprecate.py` & `thermoextrap-0.2.3/src/thermoextrap/core/_deprecate.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,15 @@
 """
 from __future__ import annotations
 
 import inspect
 import warnings
 from functools import wraps
 from textwrap import dedent
-from typing import (
-    Any,
-    Callable,
-    Mapping,
-    TypeVar,
-    cast,
-)
+from typing import Any, Callable, Mapping, TypeVar, cast
 
 # to maintain type information across generic functions and parametrization
 T = TypeVar("T")
 
 # used in decorators to preserve the signature of the function it decorates
 # see https://mypy.readthedocs.io/en/stable/generics.html#declaring-decorators
 FuncType = Callable[..., Any]
```

### Comparing `thermoextrap-0.2.2/src/thermoextrap/core/_docstrings.py` & `thermoextrap-0.2.3/src/thermoextrap/core/_docstrings.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/core/cached_decorators.py` & `thermoextrap-0.2.3/src/thermoextrap/core/cached_decorators.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/core/data.py` & `thermoextrap-0.2.3/src/thermoextrap/core/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1932,15 +1932,15 @@
     )
     #: Expansion order
     order: int | None = kw_only_field(
         default=None, validator=attv.optional(attv.instance_of(int))
     )
     #: Stored weights
     w: Sequence | None = kw_only_field(default=None)
-    #: Optional parameteres to :meth:`cmomy.xCentralMoments.from_vals`
+    #: Optional parameters to :meth:`cmomy.xCentralMoments.from_vals`
     from_vals_kws: Mapping | None = kw_only_field(default=None)
     #: :class:`cmomy.xCentralMoments` object
     dxduave: xCentralMoments | None = kw_only_field(
         default=None,
         validator=attv.optional(attv.instance_of(xCentralMoments)),
     )
```

### Comparing `thermoextrap-0.2.2/src/thermoextrap/core/external/docfiller.py` & `thermoextrap-0.2.3/src/thermoextrap/core/external/docfiller.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/core/external/docscrape.py` & `thermoextrap-0.2.3/src/thermoextrap/core/external/docscrape.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/core/idealgas.py` & `thermoextrap-0.2.3/src/thermoextrap/core/idealgas.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/core/models.py` & `thermoextrap-0.2.3/src/thermoextrap/core/models.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/core/stack.py` & `thermoextrap-0.2.3/src/thermoextrap/core/stack.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/core/xrutils.py` & `thermoextrap-0.2.3/src/thermoextrap/core/xrutils.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/gpr_active/__init__.py` & `thermoextrap-0.2.3/src/thermoextrap/gpr_active/__init__.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/gpr_active/active_utils.py` & `thermoextrap-0.2.3/src/thermoextrap/gpr_active/active_utils.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/gpr_active/gp_models.py` & `thermoextrap-0.2.3/src/thermoextrap/gpr_active/gp_models.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/gpr_active/ig_active.py` & `thermoextrap-0.2.3/src/thermoextrap/gpr_active/ig_active.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/gpr_active/sine_active.py` & `thermoextrap-0.2.3/src/thermoextrap/gpr_active/sine_active.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/legacy/__init__.py` & `thermoextrap-0.2.3/src/thermoextrap/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/legacy/extrap.py` & `thermoextrap-0.2.3/src/thermoextrap/legacy/extrap.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/legacy/gpr.py` & `thermoextrap-0.2.3/src/thermoextrap/legacy/gpr.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/legacy/gpr_stack.py` & `thermoextrap-0.2.3/src/thermoextrap/legacy/gpr_stack.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/legacy/ig.py` & `thermoextrap-0.2.3/src/thermoextrap/legacy/ig.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/legacy/interp.py` & `thermoextrap-0.2.3/src/thermoextrap/legacy/interp.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/legacy/old_scripts.py` & `thermoextrap-0.2.3/src/thermoextrap/legacy/old_scripts.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/legacy/recursive_interp.py` & `thermoextrap-0.2.3/src/thermoextrap/legacy/recursive_interp.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/legacy/reweight.py` & `thermoextrap-0.2.3/src/thermoextrap/legacy/reweight.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/legacy/utilities.py` & `thermoextrap-0.2.3/src/thermoextrap/legacy/utilities.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/lnpi.py` & `thermoextrap-0.2.3/src/thermoextrap/lnpi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 r"""
 Inverse temperature expansion of macrostate distribution (:mod:`~thermoextrap.lnpi`)
 ====================================================================================
 
 This is used to extrapolate, in inverse temperature :math:`\beta = (k_{\rm B} T)^{-1}`, the macrostate distribution function :math:`\ln\Pi` from transition matrix Monte Carlo simulations.
 
-See :ref:`notebooks/macrostate_dist_extrap:macrostate distribution extrapolation` for example usage.
+See :ref:`examples/usage/basic/macrostate_dist_extrap:macrostate distribution extrapolation` for example usage.
 """
 
 from __future__ import annotations
 
 import warnings
 from functools import lru_cache
 from typing import Hashable, Sequence
```

### Comparing `thermoextrap-0.2.2/src/thermoextrap/recursive_interp.py` & `thermoextrap-0.2.3/src/thermoextrap/recursive_interp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Recursive interpolation (:mod:`~thermoextrap.recursive_interp`)
 ===============================================================
 
 Holds recursive interpolation class.
 This includes the recursive training algorithm and consistency checks.
 
-See :ref:`notebooks/temperature_interp:recursive interpolation` for example usage.
+See :ref:`examples/usage/basic/temperature_interp:recursive interpolation` for example usage.
 """
 
 
 import numpy as np
 
 # import xarray as xr
 from scipy import stats
```

### Comparing `thermoextrap-0.2.2/src/thermoextrap/volume.py` & `thermoextrap-0.2.3/src/thermoextrap/volume.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap/volume_idealgas.py` & `thermoextrap-0.2.3/src/thermoextrap/volume_idealgas.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/src/thermoextrap.egg-info/SOURCES.txt` & `thermoextrap-0.2.3/src/thermoextrap.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .cruft.json
 .gitignore
+.gitmodules
 .pre-commit-config.yaml
 AUTHORS.md
 CONTRIBUTING.md
 HISTORY.md
 LICENSE
 MANIFEST.in
 Makefile
@@ -39,16 +40,14 @@
 src/thermoextrap/core/models.py
 src/thermoextrap/core/sputils.py
 src/thermoextrap/core/stack.py
 src/thermoextrap/core/xrutils.py
 src/thermoextrap/core/external/__init__.py
 src/thermoextrap/core/external/docfiller.py
 src/thermoextrap/core/external/docscrape.py
-src/thermoextrap/core/tmp/_docfiller.py
-src/thermoextrap/core/tmp/_docstrings.py
 src/thermoextrap/gpr_active/__init__.py
 src/thermoextrap/gpr_active/active_utils.py
 src/thermoextrap/gpr_active/gp_models.py
 src/thermoextrap/gpr_active/ig_active.py
 src/thermoextrap/gpr_active/sine_active.py
 src/thermoextrap/legacy/__init__.py
 src/thermoextrap/legacy/extrap.py
```

### Comparing `thermoextrap-0.2.2/tests/conftest.py` & `thermoextrap-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/tests/lnpi_data/sample_data.json` & `thermoextrap-0.2.3/tests/lnpi_data/sample_data.json`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/tests/test_GPs.py` & `thermoextrap-0.2.3/tests/test_GPs.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/tests/test_active.py` & `thermoextrap-0.2.3/tests/test_active.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/tests/test_beta.py` & `thermoextrap-0.2.3/tests/test_beta.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/tests/test_data.py` & `thermoextrap-0.2.3/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/tests/test_idealgas.py` & `thermoextrap-0.2.3/tests/test_idealgas.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/tests/test_lnPi.py` & `thermoextrap-0.2.3/tests/test_lnPi.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/tests/test_stack.py` & `thermoextrap-0.2.3/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/tests/test_u_data.py` & `thermoextrap-0.2.3/tests/test_u_data.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/tests/test_u_equations.py` & `thermoextrap-0.2.3/tests/test_u_equations.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/tests/test_volume.py` & `thermoextrap-0.2.3/tests/test_volume.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.2/tox.ini` & `thermoextrap-0.2.3/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-skipsdist=True
+isolated_build = True
 requires = tox-conda
 envlist =
         # test
         py3{8, 9, 10}-tests
 
 
 [base]
@@ -71,15 +71,14 @@
     release: ghp-import -n {posargs:-m 'update docs'} -b nist-pages {toxinidir}/docs/_build/html
     clean: make allclean
     spelling: make spelling
     command: {posargs}
     live: make livehtml
     make: make {posargs}
 
-
 # create pypi dist
 [testenv:dist-pypi-{build, testrelease, release}]
 description  =
     build: build distribution.
     testrelease: upload to testpypi
     release: upload to pypi
 skip_install = True
@@ -94,25 +93,25 @@
     testrelease: twine upload --repository testpypi {toxinidir}/dist/*
     release: twine upload {toxinidir}/dist/*
 
 
 # create conda dist
 [testenv:dist-conda-{recipe, build, command}]
 description  =
-    recipe: build conda recipe using grayskull
+    recipe: build conda recipe using grayskull (can optionally pass a local sdist)
     build: build conda distribution
     command: run arbitrary command
 skip_install = True
 envdir       = {toxworkdir}/dist-conda
 basepython   = {[base]build_python}
 conda_env    = {[base]conda_env_dist_conda}
 changedir    = {toxinidir}/dist-conda
 commands     =
     recipe: rm -rf {toxinidir}/dist-conda/{[base]package_name}
-    recipe: grayskull pypi {[base]package_name}
+    recipe: grayskull pypi {posargs:{[base]package_name}}
     recipe: cat {[base]package_name}/meta.yaml
 
     build: rm -rf build
     build: mkdir -p build
     build: conda mambabuild --output-folder=build --no-anaconda-upload .
     command: {posargs:python}
```

