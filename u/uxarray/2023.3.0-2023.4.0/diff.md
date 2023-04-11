# Comparing `tmp/uxarray-2023.3.0.tar.gz` & `tmp/uxarray-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uxarray-2023.3.0.tar", last modified: Fri Mar 24 17:33:00 2023, max compression
+gzip compressed data, was "uxarray-2023.4.0.tar", last modified: Tue Apr 11 21:51:59 2023, max compression
```

## Comparing `uxarray-2023.3.0.tar` & `uxarray-2023.4.0.tar`

### file list

```diff
@@ -1,29 +1,141 @@
-drwxr-xr-x   0 hcraker  (1042954360) 1202617992        0 2023-03-24 17:33:00.699991 uxarray-2023.3.0/
--rw-r--r--   0 hcraker  (1042954360) 1202617992    11377 2023-03-24 17:29:34.000000 uxarray-2023.3.0/LICENSE
--rw-r--r--   0 hcraker  (1042954360) 1202617992     7865 2023-03-24 17:33:00.699471 uxarray-2023.3.0/PKG-INFO
--rw-r--r--   0 hcraker  (1042954360) 1202617992     7068 2023-03-24 17:29:34.000000 uxarray-2023.3.0/README.md
--rw-r--r--   0 hcraker  (1042954360) 1202617992       38 2023-03-24 17:33:00.700138 uxarray-2023.3.0/setup.cfg
--rw-r--r--   0 hcraker  (1042954360) 1202617992     1687 2023-03-24 17:29:34.000000 uxarray-2023.3.0/setup.py
-drwxr-xr-x   0 hcraker  (1042954360) 1202617992        0 2023-03-24 17:33:00.688582 uxarray-2023.3.0/test/
--rw-r--r--   0 hcraker  (1042954360) 1202617992     1324 2023-03-24 17:29:35.000000 uxarray-2023.3.0/test/test_exodus.py
--rw-r--r--   0 hcraker  (1042954360) 1202617992    12113 2023-03-24 17:29:35.000000 uxarray-2023.3.0/test/test_grid.py
--rw-r--r--   0 hcraker  (1042954360) 1202617992     4816 2023-03-24 17:29:35.000000 uxarray-2023.3.0/test/test_helpers.py
--rw-r--r--   0 hcraker  (1042954360) 1202617992      309 2023-03-24 17:29:35.000000 uxarray-2023.3.0/test/test_placeholder.py
--rw-r--r--   0 hcraker  (1042954360) 1202617992     4618 2023-03-24 17:29:35.000000 uxarray-2023.3.0/test/test_scrip.py
--rw-r--r--   0 hcraker  (1042954360) 1202617992     2307 2023-03-24 17:29:35.000000 uxarray-2023.3.0/test/test_ugrid.py
-drwxr-xr-x   0 hcraker  (1042954360) 1202617992        0 2023-03-24 17:33:00.694190 uxarray-2023.3.0/uxarray/
--rw-r--r--   0 hcraker  (1042954360) 1202617992       43 2023-03-24 17:29:35.000000 uxarray-2023.3.0/uxarray/__init__.py
--rw-r--r--   0 hcraker  (1042954360) 1202617992    12478 2023-03-24 17:29:35.000000 uxarray-2023.3.0/uxarray/_exodus.py
--rw-r--r--   0 hcraker  (1042954360) 1202617992     8292 2023-03-24 17:29:35.000000 uxarray-2023.3.0/uxarray/_scrip.py
--rw-r--r--   0 hcraker  (1042954360) 1202617992      258 2023-03-24 17:29:35.000000 uxarray-2023.3.0/uxarray/_shapefile.py
--rw-r--r--   0 hcraker  (1042954360) 1202617992     2123 2023-03-24 17:29:35.000000 uxarray-2023.3.0/uxarray/_ugrid.py
--rw-r--r--   0 hcraker  (1042954360) 1202617992    13193 2023-03-24 17:29:35.000000 uxarray-2023.3.0/uxarray/get_quadratureDG.py
--rw-r--r--   0 hcraker  (1042954360) 1202617992    18169 2023-03-24 17:29:35.000000 uxarray-2023.3.0/uxarray/grid.py
--rw-r--r--   0 hcraker  (1042954360) 1202617992    17426 2023-03-24 17:29:35.000000 uxarray-2023.3.0/uxarray/helpers.py
-drwxr-xr-x   0 hcraker  (1042954360) 1202617992        0 2023-03-24 17:33:00.698537 uxarray-2023.3.0/uxarray.egg-info/
--rw-r--r--   0 hcraker  (1042954360) 1202617992     7865 2023-03-24 17:33:00.000000 uxarray-2023.3.0/uxarray.egg-info/PKG-INFO
--rw-r--r--   0 hcraker  (1042954360) 1202617992      492 2023-03-24 17:33:00.000000 uxarray-2023.3.0/uxarray.egg-info/SOURCES.txt
--rw-r--r--   0 hcraker  (1042954360) 1202617992        1 2023-03-24 17:33:00.000000 uxarray-2023.3.0/uxarray.egg-info/dependency_links.txt
--rw-r--r--   0 hcraker  (1042954360) 1202617992        1 2023-03-24 17:33:00.000000 uxarray-2023.3.0/uxarray.egg-info/not-zip-safe
--rw-r--r--   0 hcraker  (1042954360) 1202617992       18 2023-03-24 17:33:00.000000 uxarray-2023.3.0/uxarray.egg-info/requires.txt
--rw-r--r--   0 hcraker  (1042954360) 1202617992        8 2023-03-24 17:33:00.000000 uxarray-2023.3.0/uxarray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.036582 uxarray-2023.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:58.996580 uxarray-2023.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:58.996580 uxarray-2023.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.000581 uxarray-2023.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.github/workflows/upstream-dev-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-11 21:51:48.000000 uxarray-2023.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-11 21:51:48.000000 uxarray-2023.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-11 21:51:48.000000 uxarray-2023.4.0/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-11 21:51:48.000000 uxarray-2023.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-11 21:51:59.036582 uxarray-2023.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-04-11 21:51:48.000000 uxarray-2023.4.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-04-11 21:51:48.000000 uxarray-2023.4.0/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.000581 uxarray-2023.4.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-11 21:51:48.000000 uxarray-2023.4.0/ci/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-11 21:51:48.000000 uxarray-2023.4.0/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 21:51:48.000000 uxarray-2023.4.0/ci/upstream-dev-environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.000581 uxarray-2023.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.004581 uxarray-2023.4.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.004581 uxarray-2023.4.0/docs/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.004581 uxarray-2023.4.0/docs/_static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/icons/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/icons/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/icons/science.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/icons/tips.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.004581 uxarray-2023.4.0/docs/_static/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)   348960 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/logos/DOE_vertical.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44028 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/logos/EarthCube_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   210002 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/logos/NSF_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/logos/PANGEO_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   241224 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/logos/uxarray_temp_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/images/nsf.png
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.004581 uxarray-2023.4.0/docs/_static/thumbnails/
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_static/thumbnails/default.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.004581 uxarray-2023.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/_templates/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30865 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/examples/000-template.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    65555 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/examples/001-read-grid-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/examples/002-access-grid-info.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/gallery.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/docs/internal_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/internal_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/docs/user_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/user_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-11 21:51:48.000000 uxarray-2023.4.0/docs/user_api/uxarray_api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 21:51:48.000000 uxarray-2023.4.0/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 21:51:48.000000 uxarray-2023.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 21:51:59.036582 uxarray-2023.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-11 21:51:48.000000 uxarray-2023.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:58.992581 uxarray-2023.4.0/test/meshfiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:58.992581 uxarray-2023.4.0/test/meshfiles/exodus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/test/meshfiles/exodus/mixed/
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/exodus/mixed/mixed.exo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/test/meshfiles/exodus/outCSne8/
+-rw-r--r--   0 runner    (1001) docker     (123)    42627 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/exodus/outCSne8/outCSne8.g
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:58.992581 uxarray-2023.4.0/test/meshfiles/mpas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/test/meshfiles/mpas/QU/
+-rw-r--r--   0 runner    (1001) docker     (123)   178192 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/mpas/QU/mesh.QU.1920km.151026.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:58.992581 uxarray-2023.4.0/test/meshfiles/scrip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/test/meshfiles/scrip/outCSne8/
+-rw-r--r--   0 runner    (1001) docker     (123)    48890 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/scrip/outCSne8/outCSne8.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.008581 uxarray-2023.4.0/test/meshfiles/shp/
+-rw-r--r--   0 runner    (1001) docker     (123)   162187 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/shp/grid_fire.shp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:58.992581 uxarray-2023.4.0/test/meshfiles/ugrid/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.024581 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    46371 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/a_ice.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  2510328 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/fesom.mesh.diag.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1203548 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/salt.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    46383 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/sst.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1203552 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/temp.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50983 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/test_scrip_outfile.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  2218394 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/u.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/uice.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  2218394 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/v.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/fesom/vice.fesom.1948.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.028581 uxarray-2023.4.0/test/meshfiles/ugrid/geoflow-small/
+-rw-r--r--   0 runner    (1001) docker     (123)  1130591 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/geoflow-small/grid.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/geoflow-small/v1.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/geoflow-small/v2.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/geoflow-small/v3.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.028581 uxarray-2023.4.0/test/meshfiles/ugrid/outCSne30/
+-rw-r--r--   0 runner    (1001) docker     (123)   181767 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/outCSne30/outCSne30.ug
+-rw-r--r--   0 runner    (1001) docker     (123)    49344 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/outCSne30/outCSne30_var2.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    43280 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/outCSne30/outCSne30_vortex.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.032581 uxarray-2023.4.0/test/meshfiles/ugrid/outRLL1deg/
+-rw-r--r--   0 runner    (1001) docker     (123)  2076807 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg.ug
+-rw-r--r--   0 runner    (1001) docker     (123)   518496 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg_vortex.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.032581 uxarray-2023.4.0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/
+-rw-r--r--   0 runner    (1001) docker     (123)    36983 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4.ug
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4_vortex.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/test_exodus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/test_mpas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/test_placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/test_scrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-11 21:51:48.000000 uxarray-2023.4.0/test/test_ugrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.036582 uxarray-2023.4.0/uxarray/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/_exodus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/_mpas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/_scrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/_shapefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/_ugrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/get_quadratureDG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20707 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19769 2023-04-11 21:51:48.000000 uxarray-2023.4.0/uxarray/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:59.036582 uxarray-2023.4.0/uxarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-11 21:51:58.000000 uxarray-2023.4.0/uxarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-11 21:51:58.000000 uxarray-2023.4.0/uxarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:51:58.000000 uxarray-2023.4.0/uxarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:51:58.000000 uxarray-2023.4.0/uxarray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 21:51:58.000000 uxarray-2023.4.0/uxarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 21:51:58.000000 uxarray-2023.4.0/uxarray.egg-info/top_level.txt
```

### Comparing `uxarray-2023.3.0/LICENSE` & `uxarray-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uxarray-2023.3.0/PKG-INFO` & `uxarray-2023.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uxarray
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: Unstructured grid model reading and recognizing with xarray.
 Home-page: https://github.com/UXARRAY/uxarray
 Maintainer: UXARRAY
 Maintainer-email: 
 Project-URL: Source, https://github.com/UXARRAY/uxarray
 Project-URL: Tracker, https://github.com/UXARRAY/uxarray/issues
 Classifier: Operating System :: OS Independent
```

### Comparing `uxarray-2023.3.0/README.md` & `uxarray-2023.4.0/README.md`

 * *Files identical despite different names*

### Comparing `uxarray-2023.3.0/setup.py` & `uxarray-2023.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.3.0/test/test_exodus.py` & `uxarray-2023.4.0/test/test_exodus.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import numpy as np
 
 from unittest import TestCase
 from pathlib import Path
 
 import xarray as xr
 import uxarray as ux
+from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
 
 current_path = Path(os.path.dirname(os.path.realpath(__file__)))
 
 
 class TestExodus(TestCase):
 
     def test_read_exodus(self):
@@ -18,15 +19,15 @@
         exo2_filename = current_path / "meshfiles" / "exodus" / "outCSne8" / "outCSne8.g"
         xr_exo_ds = xr.open_dataset(exo2_filename)
         tgrid = ux.Grid(xr_exo_ds)
 
     def test_init_verts(self):
         """Create a uxarray grid from vertices and saves a 1 face exodus
         file."""
-        verts = np.array([[0, 0], [2, 0], [0, 2], [2, 2]])
+        verts = [[[0, 0], [2, 0], [0, 2], [2, 2]]]
         vgrid = ux.Grid(verts)
 
     def test_encode_exodus(self):
         """Read a UGRID dataset and encode that as an Exodus format."""
 
     def test_mixed_exodus(self):
         """Read/write an exodus file with two types of faces (triangle and
@@ -35,7 +36,18 @@
         exo2_filename = current_path / "meshfiles" / "exodus" / "mixed" / "mixed.exo"
         xr_exo_ds = xr.open_dataset(exo2_filename)
         tgrid = ux.Grid(xr_exo_ds)
         outfile = current_path / "write_test_mixed.ug"
         tgrid.encode_as("ugrid")
         outfile = current_path / "write_test_mixed.exo"
         tgrid.encode_as("exodus")
+
+    def test_standardized_dtype_and_fill(self):
+        """Test to see if Mesh2_Face_Nodes uses the expected integer datatype
+        and expected fill value as set in constants.py."""
+
+        exo2_filename = current_path / "meshfiles" / "exodus" / "mixed" / "mixed.exo"
+        xr_exo_ds = xr.open_dataset(exo2_filename)
+        ux_grid = ux.Grid(xr_exo_ds)
+
+        assert ux_grid.Mesh2_face_nodes.dtype == INT_DTYPE
+        assert ux_grid.Mesh2_face_nodes._FillValue == INT_FILL_VALUE
```

### Comparing `uxarray-2023.3.0/test/test_helpers.py` & `uxarray-2023.4.0/test/test_helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 import xarray as xr
 
 from unittest import TestCase
 from pathlib import Path
 
 import uxarray as ux
 
+from uxarray.helpers import _replace_fill_values
+from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
+
 try:
     import constants
 except ImportError:
     from . import constants
 
 # Data files
 current_path = Path(os.path.dirname(os.path.realpath(__file__)))
@@ -26,15 +29,15 @@
 
     def test_face_area_coords(self):
         """Test function for helper function get_all_face_area_from_coords."""
         # Note: currently only testing one face, but this can be used to get area of multiple faces
         x = np.array([0.57735027, 0.57735027, -0.57735027])
         y = np.array([-5.77350269e-01, 5.77350269e-01, 5.77350269e-01])
         z = np.array([-0.57735027, -0.57735027, -0.57735027])
-        face_nodes = np.array([[0, 1, 2]]).astype(constants.int_dtype)
+        face_nodes = np.array([[0, 1, 2]]).astype(INT_DTYPE)
         area = ux.get_all_face_area_from_coords(x,
                                                 y,
                                                 z,
                                                 face_nodes,
                                                 3,
                                                 coords_type="cartesian")
         nt.assert_almost_equal(area, constants.TRI_AREA, decimal=1)
@@ -115,7 +118,50 @@
             random.uniform(-0.5 * np.pi, 0.5 * np.pi)
         ]
         [x, y, z] = ux.helpers._convert_node_lonlat_rad_to_xyz([lon, lat])
         [new_lon,
          new_lat] = ux.helpers._convert_node_xyz_to_lonlat_rad([x, y, z])
         self.assertLessEqual(np.absolute(new_lon - lon), err_tolerance)
         self.assertLessEqual(np.absolute(new_lat - lat), err_tolerance)
+
+
+class TestConstants(TestCase):
+    # DTYPE as set in constants.py
+    expected_int_dtype = INT_DTYPE
+
+    # INT_FILL_VALUE as set in constants.py
+    fv = INT_FILL_VALUE
+
+    def test_replace_fill_values(self):
+        """Tests _replace_fill_values() helper function across multiple
+        different dtype arrays used as face_nodes."""
+
+        # expected output from _replace_fill_values()
+        face_nodes_gold = np.array(
+            [[1, 2, self.fv], [self.fv, self.fv, self.fv]], dtype=INT_DTYPE)
+
+        # test different datatypes for face_nodes
+        dtypes = [np.int32, np.int64, np.float32, np.float64]
+        for dtype in dtypes:
+            # test face nodes with set dtype
+            face_nodes = np.array([[1, 2, -1], [-1, -1, -1]], dtype=dtype)
+
+            # output of _replace_fill_values()
+            face_nodes_test = _replace_fill_values(grid_var=face_nodes,
+                                                   original_fill=-1,
+                                                   new_fill=INT_FILL_VALUE,
+                                                   new_dtype=INT_DTYPE)
+
+            assert np.array_equal(face_nodes_test, face_nodes_gold)
+
+    def test_replace_fill_values_invalid(self):
+        """Tests _replace_fill_values() helper function attempting to use a
+        fill value that is not representable by the current dtype."""
+
+        face_nodes = np.array([[1, 2, -1], [-1, -1, -1]], dtype=np.uint32)
+        # invalid fill value with dtype should raise a valueError
+        with self.assertRaises(ValueError):
+            # INT_FILL_VALUE (max(uint32) not representable by int16)
+            face_nodes_test = _replace_fill_values(grid_var=face_nodes,
+                                                   original_fill=-1,
+                                                   new_fill=INT_FILL_VALUE,
+                                                   new_dtype=np.int16)
```

### Comparing `uxarray-2023.3.0/test/test_scrip.py` & `uxarray-2023.4.0/test/test_scrip.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from uxarray._scrip import _read_scrip, _encode_scrip
+from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
 import uxarray as ux
 import xarray as xr
 from unittest import TestCase
 import numpy as np
 
 import os
 from pathlib import Path
@@ -106,7 +107,22 @@
 
         # Create a flattened and unique array for comparisons
         corner_lon = ds_ne8['grid_corner_lon'].values
         corner_lon = corner_lon.flatten()
         strip_lon = np.unique(corner_lon)
 
         assert strip_lon.all() == mesh08['Mesh2_node_x'].all()
+
+    def test_standardized_dtype_and_fill(self):
+        """Test to see if Mesh2_Face_Nodes uses the expected integer datatype
+        and expected fill value as set in constants.py."""
+
+        xr_ne30 = xr.open_dataset(ne30)
+        ux_grid_01 = ux.Grid(xr_ne30)
+
+        xr_ne8 = xr.open_dataset(ne8)
+        ux_grid_02 = ux.Grid(xr_ne8)
+
+        grids = [ux_grid_01, ux_grid_02]
+        for grid in grids:
+            assert grid.Mesh2_face_nodes.dtype == INT_DTYPE
+            assert grid.Mesh2_face_nodes._FillValue == INT_FILL_VALUE
```

### Comparing `uxarray-2023.3.0/uxarray/_exodus.py` & `uxarray-2023.4.0/uxarray/_exodus.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import xarray as xr
 import numpy as np
 from pathlib import PurePath
 from datetime import datetime
 
-int_dtype = np.uint32
+from uxarray.helpers import _replace_fill_values
+from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
 
 
 # Exodus Number is one-based.
 def _read_exodus(ext_ds, ds_var_names):
     """Exodus file reader.
 
     Parameters: xarray.Dataset, required
@@ -43,15 +44,15 @@
     conn = np.empty((0, max_face_nodes))
 
     for key, value in ext_ds.variables.items():
         if key == "qa_records":
             # TODO: Use the data here for Mesh2 construct, if required.
             pass
         elif key == "coord":
-            ds.Mesh2.attrs['topology_dimension'] = int_dtype(
+            ds.Mesh2.attrs['topology_dimension'] = INT_DTYPE(
                 ext_ds.dims['num_dim'])
             ds["Mesh2_node_x"] = xr.DataArray(
                 data=ext_ds.coord[0],
                 dims=["nMesh2_node"],
                 attrs={
                     "standard_name": "longitude",
                     "long_name": "longitude of mesh nodes",
@@ -116,24 +117,31 @@
             for k, v in value.attrs.items():
                 if k == "elem_type":
                     # TODO: etype if not used now, remove if it'll never be required
                     etype = v
 
     # outside the k,v for loop
     # set the face nodes data compiled in "connect" section
+
+    # standardize fill values and data type face nodes
+    face_nodes = _replace_fill_values(grid_var=conn[:] - 1,
+                                      original_fill=-1,
+                                      new_fill=INT_FILL_VALUE,
+                                      new_dtype=INT_DTYPE)
+
     ds["Mesh2_face_nodes"] = xr.DataArray(
-        data=(conn[:] - 1),
+        data=face_nodes,
         dims=["nMesh2_face", "nMaxMesh2_face_nodes"],
         attrs={
             "cf_role":
                 "face_node_connectivity",
             "_FillValue":
-                -1,
+                INT_FILL_VALUE,
             "start_index":
-                int_dtype(
+                INT_DTYPE(
                     0)  # NOTE: This might cause an error if numbering has holes
         })
     print("Finished reading exodus file.")
 
     if ext_ds.dims['num_dim'] > 2:
         # set coordinates
         ds = ds.set_coords(["Mesh2_node_x", "Mesh2_node_y", "Mesh2_node_z"])
@@ -164,15 +172,15 @@
     # Note this is 1-based unlike native Mesh2 construct
 
     exo_ds = xr.Dataset()
 
     now = datetime.now()
     date = now.strftime("%Y:%m:%d")
     time = now.strftime("%H:%M:%S")
-    fp_word = int_dtype(8)
+    fp_word = INT_DTYPE(8)
     exo_version = np.float32(5.0)
     api_version = np.float32(5.0)
 
     exo_ds.attrs = {
         "api_version": api_version,
         "version": exo_version,
         "floating_point_word_size": fp_word,
@@ -224,15 +232,15 @@
     # eg num_el_all_blks = [0, 0, 6, 12] signifies 6 TRI and 12 SHELL elements
     num_el_all_blks = np.zeros(ds[ds_var_names["nMaxMesh2_face_nodes"]].size,
                                "i8")
     # this list stores connectivity without filling
     conn_nofill = []
 
     # store the number of faces in an array
-    for row in ds[ds_var_names["Mesh2_face_nodes"]].astype(int_dtype).data:
+    for row in ds[ds_var_names["Mesh2_face_nodes"]].astype(INT_DTYPE).data:
 
         # find out -1 in each row, this indicates lower than max face nodes
         arr = np.where(row == -1)
         # arr[0].size returns the location of first -1 in the conn list
         # if > 0, arr[0][0] is the num_nodes forming the face
         if arr[0].size > 0:
             # increment the number of faces at the corresponding location
@@ -279,22 +287,23 @@
         element_type = _get_element_type(num_nodes)
 
         # get number of faces for this block
         num_faces = num_el_all_blks[nonzero_el_index_blks[0][blk]]
         # assign Data variables
         # convert list to np.array, sorted list guarantees we have the correct info
         conn_blk = conn_nofill[start:start + num_faces]
-        conn_np = np.array([np.array(xi, dtype="i8") for xi in conn_blk])
+        conn_np = np.array([np.array(xi, dtype=INT_DTYPE) for xi in conn_blk])
         exo_ds[str_connect] = xr.DataArray(data=xr.DataArray((conn_np[:] + 1)),
                                            dims=[str_el_in_blk, str_nod_per_el],
                                            attrs={"elem_type": element_type})
 
         # edge type
         exo_ds[str_edge_type] = xr.DataArray(
-            data=xr.DataArray(np.zeros((num_faces, num_nodes), "i8")),
+            data=xr.DataArray(np.zeros((num_faces, num_nodes),
+                                       dtype=INT_DTYPE)),
             dims=[str_el_in_blk, str_nod_per_el])
 
         # global id
         gid = np.arange(start + 1, start + num_faces + 1, 1)
         exo_ds[str_global_id] = xr.DataArray(data=(gid), dims=[str_el_in_blk])
 
         # attrib
@@ -311,15 +320,15 @@
     # eb_prop1
     prop1_vals = np.arange(1, num_blks + 1, 1)
     exo_ds["eb_prop1"] = xr.DataArray(data=prop1_vals,
                                       dims=["num_el_blk"],
                                       attrs={"name": "ID"})
     # eb_status
     exo_ds["eb_status"] = xr.DataArray(data=xr.DataArray(
-        np.ones([num_blks], dtype="i8")),
+        np.ones([num_blks], dtype=INT_DTYPE)),
                                        dims=["num_el_blk"])
 
     # eb_names
     eb_names = np.empty(num_blks, dtype='str')
     exo_ds["eb_names"] = xr.DataArray(data=xr.DataArray(eb_names),
                                       dims=["num_el_blk"])
     if dim == 2:
```

### Comparing `uxarray-2023.3.0/uxarray/_scrip.py` & `uxarray-2023.4.0/uxarray/_scrip.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import xarray as xr
 import numpy as np
 
-from .helpers import grid_center_lat_lon
+from uxarray.helpers import grid_center_lat_lon
 
-int_dtype = np.uint32
+from uxarray.helpers import _replace_fill_values
+from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
 
 
 def _to_ugrid(in_ds, out_ds):
     """If input dataset (``in_ds``) file is an unstructured SCRIP file,
     function will reassign SCRIP variables to UGRID conventions in output file
     (``out_ds``).
 
@@ -66,25 +67,31 @@
                 "units": "degrees_north",
             })
 
         # Create Mesh2_face_x/y from grid_center_lat/lon
         out_ds['Mesh2_face_x'] = in_ds['grid_center_lon']
         out_ds['Mesh2_face_y'] = in_ds['grid_center_lat']
 
+        # standardize fill values and data type face nodes
+        face_nodes = _replace_fill_values(unq_inv,
+                                          original_fill=-1,
+                                          new_fill=INT_FILL_VALUE,
+                                          new_dtype=INT_DTYPE)
+
         # set the face nodes data compiled in "connect" section
         out_ds["Mesh2_face_nodes"] = xr.DataArray(
-            data=unq_inv,
+            data=face_nodes,
             dims=["nMesh2_face", "nMaxMesh2_face_nodes"],
             attrs={
                 "cf_role":
                     "face_node_connectivity",
                 "_FillValue":
-                    -1,
+                    INT_FILL_VALUE,
                 "start_index":
-                    int_dtype(
+                    INT_DTYPE(
                         0
                     )  # NOTE: This might cause an error if numbering has holes
             })
 
     else:
         raise Exception("Structured scrip files are not yet supported")
 
@@ -180,15 +187,15 @@
         Dataset to be returned by ``_encode_scrip``. The function returns
         the output dataset in SCRIP format for immediate use.
     """
     # Create empty dataset to put new scrip format data into
     ds = xr.Dataset()
 
     # Make grid corner lat/lon
-    f_nodes = mesh2_face_nodes.values.astype(int_dtype).ravel()
+    f_nodes = mesh2_face_nodes.values.astype(INT_DTYPE).ravel()
 
     # Create arrays to hold lat/lon data
     lat_nodes = mesh2_node_y[f_nodes].values
     lon_nodes = mesh2_node_x[f_nodes].values
 
     # Reshape arrays to be 2D instead of 1D
     reshp_lat = np.reshape(
```

### Comparing `uxarray-2023.3.0/uxarray/get_quadratureDG.py` & `uxarray-2023.4.0/uxarray/get_quadratureDG.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.3.0/uxarray/grid.py` & `uxarray-2023.4.0/uxarray/grid.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import numpy as np
 
 # reader and writer imports
 from ._exodus import _read_exodus, _encode_exodus
 from ._ugrid import _read_ugrid, _encode_ugrid
 from ._shapefile import _read_shpfile
 from ._scrip import _read_scrip, _encode_scrip
+from ._mpas import _read_mpas
 from .helpers import get_all_face_area_from_coords, parse_grid_type, _convert_node_xyz_to_lonlat_rad, _convert_node_lonlat_rad_to_xyz
-
-int_dtype = np.uint32
+from .constants import INT_DTYPE, INT_FILL_VALUE
 
 
 class Grid:
     """
     Examples
     ----------
 
@@ -42,16 +42,17 @@
         islatlon : bool, optional
             Specify if the grid is lat/lon based
         concave: bool, optional
             Specify if this grid has concave elements (internal checks for this are possible)
         gridspec: bool, optional
             Specifies gridspec
         mesh_type: str, optional
-            Specify the mesh file type, eg. exo, ugrid, shp, etc
-
+            Specify the mesh file type, eg. exo, ugrid, shp, mpas, etc
+        use_dual: bool, optional
+            Specify whether to use the primal (use_dual=False) or dual (use_dual=True) mesh if the file type is mpas
         Raises
         ------
             RuntimeError
                 If specified file not found
         """
         # initialize internal variable names
         self.__init_ds_var_names__()
@@ -60,24 +61,37 @@
         self._face_areas = None
 
         # TODO: fix when adding/exercising gridspec
 
         # unpack kwargs
         # sets default values for all kwargs to None
         kwargs_list = [
-            'gridspec', 'vertices', 'islatlon', 'concave', 'source_grid'
+            'gridspec', 'vertices', 'islatlon', 'concave', 'source_grid',
+            'use_dual'
         ]
         for key in kwargs_list:
             setattr(self, key, kwargs.get(key, None))
 
         # check if initializing from verts:
         if isinstance(dataset, (list, tuple, np.ndarray)):
-            self.vertices = dataset
-            self.__from_vert__()
-            self.source_grid = "From vertices"
+            dataset = np.asarray(dataset)
+            # grid with multiple faces
+            if dataset.ndim == 3:
+                self.__from_vert__(dataset)
+                self.source_grid = "From vertices"
+            # grid with a single face
+            elif dataset.ndim == 2:
+                dataset = np.array([dataset])
+                self.__from_vert__(dataset)
+                self.source_grid = "From vertices"
+            else:
+                raise RuntimeError(
+                    f"Invalid Input Dimension: {dataset.ndim}. Expected dimension should be "
+                    f"3: [nMesh2_face, nMesh2_node, Two/Three] or 2 when only "
+                    f"one face is passed in.")
         # check if initializing from string
         # TODO: re-add gridspec initialization when implemented
         elif isinstance(dataset, xr.Dataset):
             self.mesh_type = parse_grid_type(dataset)
             self.__from_ds__(dataset=dataset)
         else:
             raise RuntimeError("Dataset is not a valid input type.")
@@ -135,66 +149,97 @@
                     setattr(self, key, self.ds[value])
 
             # Set Attributes for Dimensions
             if self.ds.dims is not None:
                 if value in self.ds.dims:
                     setattr(self, key, len(self.ds[value]))
 
-    def __from_vert__(self):
-        """Create a grid with one face with vertices specified by the given
-        argument.
+    def __from_vert__(self, dataset):
+        """Create a grid with faces constructed from vertices specified by the
+        given argument.
 
-        Called by :func:`__init__`.
+        Parameters
+        ----------
+        dataset : ndarray, list, tuple, required
+            Input vertex coordinates that form our face(s)
         """
         self.ds = xr.Dataset()
         self.ds["Mesh2"] = xr.DataArray(
             attrs={
                 "cf_role": "mesh_topology",
                 "long_name": "Topology data of unstructured mesh",
                 "topology_dimension": -1,
                 "node_coordinates": "Mesh2_node_x Mesh2_node_y Mesh2_node_z",
                 "node_dimension": "nMesh2_node",
                 "face_node_connectivity": "Mesh2_face_nodes",
                 "face_dimension": "nMesh2_face"
             })
-        self.ds.Mesh2.attrs['topology_dimension'] = self.vertices[0].size
+        self.ds.Mesh2.attrs['topology_dimension'] = dataset.ndim
 
         # set default coordinate units to spherical coordinates
         # users can change to cartesian if using cartesian for initialization
         x_units = "degrees_east"
         y_units = "degrees_north"
-        if self.vertices[0].size > 2:
+        if dataset[0][0].size > 2:
             z_units = "elevation"
+        x_coord = dataset[:, :, 0].flatten()
+        y_coord = dataset[:, :, 1].flatten()
+        if dataset[0][0].size > 2:
+            z_coord = dataset[:, :, 2].flatten()
+
+        # Identify unique vertices and their indices
+        unique_verts, indices = np.unique(dataset.reshape(
+            -1, dataset.shape[-1]),
+                                          axis=0,
+                                          return_inverse=True)
+
+        # Nodes index that contain a fill value
+        fill_value_mask = np.logical_or(unique_verts[:, 0] == INT_FILL_VALUE,
+                                        unique_verts[:, 1] == INT_FILL_VALUE)
+        if dataset[0][0].size > 2:
+            fill_value_mask = np.logical_or(
+                unique_verts[:, 0] == INT_FILL_VALUE,
+                unique_verts[:, 1] == INT_FILL_VALUE,
+                unique_verts[:, 2] == INT_FILL_VALUE)
+
+        # Get the indices of all the False values in fill_value_mask
+        false_indices = np.where(fill_value_mask == True)[0]
+
+        # Check if any False values were found
+        indices = indices.astype(INT_DTYPE)
+        if false_indices.size > 0:
+
+            # Remove the rows corresponding to False values in unique_verts
+            unique_verts = np.delete(unique_verts, false_indices, axis=0)
+
+            # Update indices accordingly
+            for i, idx in enumerate(false_indices):
+                indices[indices == idx] = INT_FILL_VALUE
+                indices[indices > idx] -= 1
 
-        x_coord = self.vertices.transpose()[0]
-        y_coord = self.vertices.transpose()[1]
-        if self.vertices[0].size > 2:
-            z_coord = self.vertices.transpose()[2]
-
-        # single face with all nodes
-        num_nodes = x_coord.size
-        connectivity = [list(range(0, num_nodes))]
-
-        self.ds["Mesh2_node_x"] = xr.DataArray(data=xr.DataArray(x_coord),
+        # Create coordinate DataArrays
+        self.ds["Mesh2_node_x"] = xr.DataArray(data=unique_verts[:, 0],
                                                dims=["nMesh2_node"],
                                                attrs={"units": x_units})
-        self.ds["Mesh2_node_y"] = xr.DataArray(data=xr.DataArray(y_coord),
+        self.ds["Mesh2_node_y"] = xr.DataArray(data=unique_verts[:, 1],
                                                dims=["nMesh2_node"],
                                                attrs={"units": y_units})
-        if self.vertices[0].size > 2:
-            self.ds["Mesh2_node_z"] = xr.DataArray(data=xr.DataArray(z_coord),
+        if dataset.shape[-1] > 2:
+            self.ds["Mesh2_node_z"] = xr.DataArray(data=unique_verts[:, 2],
                                                    dims=["nMesh2_node"],
                                                    attrs={"units": z_units})
 
+        # Create connectivity array using indices of unique vertices
+        connectivity = indices.reshape(dataset.shape[:-1])
         self.ds["Mesh2_face_nodes"] = xr.DataArray(
-            data=xr.DataArray(connectivity),
+            data=xr.DataArray(connectivity).astype(INT_DTYPE),
             dims=["nMesh2_face", "nMaxMesh2_face_nodes"],
             attrs={
                 "cf_role": "face_node_connectivity",
-                "_FillValue": -1,
+                "_FillValue": INT_FILL_VALUE,
                 "start_index": 0
             })
 
     # load mesh from a file
     def __from_ds__(self, dataset):
         """Loads a mesh dataset."""
         # call reader as per mesh_type
@@ -202,14 +247,20 @@
             self.ds = _read_exodus(dataset, self.ds_var_names)
         elif self.mesh_type == "scrip":
             self.ds = _read_scrip(dataset)
         elif self.mesh_type == "ugrid":
             self.ds, self.ds_var_names = _read_ugrid(dataset, self.ds_var_names)
         elif self.mesh_type == "shp":
             self.ds = _read_shpfile(dataset)
+        elif self.mesh_type == "mpas":
+            # select whether to use the dual mesh
+            if self.use_dual is not None:
+                self.ds = _read_mpas(dataset, self.use_dual)
+            else:
+                self.ds = _read_mpas(dataset)
         else:
             raise RuntimeError("unknown mesh type")
 
         dataset.close()
 
     def encode_as(self, grid_type):
         """Encodes the grid as a new `xarray.Dataset` per grid format supplied
@@ -296,15 +347,15 @@
         """
         if self._face_areas is None:
             # area of a face call needs the units for coordinate conversion if spherical grid is used
             coords_type = "spherical"
             if not "degree" in self.Mesh2_node_x.units:
                 coords_type = "cartesian"
 
-            face_nodes = self.Mesh2_face_nodes.data.astype(int_dtype)
+            face_nodes = self.Mesh2_face_nodes.data
             dim = self.Mesh2.attrs['topology_dimension']
 
             # initialize z
             z = np.zeros((self.nMesh2_node))
 
             # call func to cal face area of all nodes
             x = self.Mesh2_node_x.data
```

### Comparing `uxarray-2023.3.0/uxarray/helpers.py` & `uxarray-2023.4.0/uxarray/helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 import xarray as xr
 from pathlib import PurePath
 from .get_quadratureDG import get_gauss_quadratureDG, get_tri_quadratureDG
 from numba import njit, config
 import math
 
+from .constants import INT_DTYPE
+
 config.DISABLE_JIT = False
-int_dtype = np.uint32
 
 
 def parse_grid_type(dataset):
     """Checks input and contents to determine grid type. Supports detection of
     UGrid, SCRIP, Exodus and shape file.
 
     Parameters
@@ -37,14 +38,16 @@
         mesh_type = "exo"
     # scrip with grid_center_lon
     elif "grid_center_lon" in dataset:
         mesh_type = "scrip"
     # ugrid topology
     elif _is_ugrid(dataset):
         mesh_type = "ugrid"
+    elif "verticesOnCell" in dataset:
+        mesh_type = "mpas"
     else:
         raise RuntimeError(f"Could not recognize dataset format.")
     return mesh_type
 
     # check mesh topology and dimension
     try:
         standard_name = lambda v: v is not None
@@ -222,15 +225,15 @@
     Returns
     -------
     area of all faces : ndarray
     """
     num_faces = face_nodes.shape[0]
     area = np.zeros(num_faces)  # set area of each face to 0
 
-    face_nodes = face_nodes[:].astype(int_dtype)
+    face_nodes = face_nodes[:].astype(INT_DTYPE)
 
     for i in range(num_faces):
         face_z = np.zeros(len(face_nodes[i]))
 
         face_x = x[face_nodes[i]]
         face_y = y[face_nodes[i]]
         # check if z dimension
@@ -552,7 +555,66 @@
     RuntimeError
         The input array doesn't have the size of 3.
     """
     if len(node) != 3:
         raise RuntimeError("Input array should have a length of 3: [x, y, z]")
 
     return list(np.array(node) / np.linalg.norm(np.array(node), ord=2))
+
+
+def _replace_fill_values(grid_var, original_fill, new_fill, new_dtype=None):
+    """Replaces all instances of the the current fill value (``original_fill``)
+    in (``grid_var``) with (``new_fill``) and converts to the dtype defined by
+    (``new_dtype``)
+
+    Parameters
+    ----------
+    grid_var : np.ndarray
+        grid variable to be modified
+    original_fill : constant
+        original fill value used in (``grid_var``)
+    new_fill : constant
+        new fill value to be used in (``grid_var``)
+    new_dtype : np.dtype, optional
+        new data type to convert (``grid_var``) to
+
+    Returns
+    ----------
+    grid_var : xarray.Dataset
+        Input Dataset with correct fill value and dtype
+    """
+
+    # locations of fill values
+    if original_fill is not None and np.isnan(original_fill):
+        fill_val_idx = np.isnan(grid_var)
+    else:
+        fill_val_idx = grid_var == original_fill
+
+    # convert to new data type
+    if new_dtype != grid_var.dtype and new_dtype is not None:
+        grid_var = grid_var.astype(new_dtype)
+
+    # ensure fill value can be represented with current integer data type
+    if np.issubdtype(new_dtype, np.integer):
+        int_min = np.iinfo(grid_var.dtype).min
+        int_max = np.iinfo(grid_var.dtype).max
+        # ensure new_fill is in range [int_min, int_max]
+        if new_fill < int_min or new_fill > int_max:
+            raise ValueError(f'New fill value: {new_fill} not representable by'
+                             f' integer dtype: {grid_var.dtype}')
+
+    # ensure non-nan fill value can be represented with current float data type
+    elif np.issubdtype(new_dtype, np.floating) and not np.isnan(new_fill):
+        float_min = np.finfo(grid_var.dtype).min
+        float_max = np.finfo(grid_var.dtype).max
+        # ensure new_fill is in range [float_min, float_max]
+        if new_fill < float_min or new_fill > float_max:
+            raise ValueError(f'New fill value: {new_fill} not representable by'
+                             f' float dtype: {grid_var.dtype}')
+    else:
+        raise ValueError(f'Data type {grid_var.dtype} not supported'
+                         f'for grid variables')
+
+    # replace all zeros with a fill value
+    grid_var[fill_val_idx] = new_fill
+
+    return grid_var
```

### Comparing `uxarray-2023.3.0/uxarray.egg-info/PKG-INFO` & `uxarray-2023.4.0/uxarray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uxarray
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: Unstructured grid model reading and recognizing with xarray.
 Home-page: https://github.com/UXARRAY/uxarray
 Maintainer: UXARRAY
 Maintainer-email: 
 Project-URL: Source, https://github.com/UXARRAY/uxarray
 Project-URL: Tracker, https://github.com/UXARRAY/uxarray/issues
 Classifier: Operating System :: OS Independent
```

