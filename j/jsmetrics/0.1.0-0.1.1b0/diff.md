# Comparing `tmp/jsmetrics-0.1.0.tar.gz` & `tmp/jsmetrics-0.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsmetrics-0.1.0.tar", last modified: Sun Jan 22 17:10:07 2023, max compression
+gzip compressed data, was "jsmetrics-0.1.1b0.tar", last modified: Tue Apr 11 16:09:24 2023, max compression
```

## Comparing `jsmetrics-0.1.0.tar` & `jsmetrics-0.1.1b0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:07.375585 jsmetrics-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-01-22 17:10:07.375585 jsmetrics-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:07.367585 jsmetrics-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:07.363585 jsmetrics-0.1.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:07.371585 jsmetrics-0.1.0/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)  1519071 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png
--rw-r--r--   0 runner    (1001) docker     (123)   788211 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/docs/_static/images/jet_shift_violin.png
--rw-r--r--   0 runner    (1001) docker     (123)    87261 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/docs/_static/images/kuang_jet_centers.png
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/docs/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/docs/statement.rst
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:07.371585 jsmetrics-0.1.0/jsmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/jsmetrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:07.371585 jsmetrics-0.1.0/jsmetrics/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/jsmetrics/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/jsmetrics/core/check_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/jsmetrics/details_for_all_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:07.371585 jsmetrics-0.1.0/jsmetrics/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/jsmetrics/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/jsmetrics/metrics/jet_core_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    26250 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/jsmetrics/metrics/jet_core_algorithms_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    19197 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/jsmetrics/metrics/jet_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    39171 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/jsmetrics/metrics/jet_metrics_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/jsmetrics/metrics/waviness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/jsmetrics/metrics/waviness_metrics_components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:07.371585 jsmetrics-0.1.0/jsmetrics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/jsmetrics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/jsmetrics/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/jsmetrics/utils/spatial_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/jsmetrics/utils/windspeed_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:07.371585 jsmetrics-0.1.0/jsmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-01-22 17:10:07.000000 jsmetrics-0.1.0/jsmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-01-22 17:10:07.000000 jsmetrics-0.1.0/jsmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-22 17:10:07.000000 jsmetrics-0.1.0/jsmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-22 17:10:07.000000 jsmetrics-0.1.0/jsmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-01-22 17:10:07.000000 jsmetrics-0.1.0/jsmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-22 17:10:07.000000 jsmetrics-0.1.0/jsmetrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-01-22 17:10:07.379586 jsmetrics-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:07.371585 jsmetrics-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:07.375585 jsmetrics-0.1.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1262096 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1260860 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1104721 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:07.375585 jsmetrics-0.1.0/tests/metric_verification/
--rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/tests/metric_verification/metric_verification.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 17:10:07.375585 jsmetrics-0.1.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/tests/unit/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/tests/unit/test_jet_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    12642 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/tests/unit/test_jet_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/tests/unit/test_spatial_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/tests/unit/test_waviness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-01-22 17:10:05.000000 jsmetrics-0.1.0/tests/unit/test_windspeed_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.548435 jsmetrics-0.1.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-04-11 16:09:24.548435 jsmetrics-0.1.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.540434 jsmetrics-0.1.1b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.536434 jsmetrics-0.1.1b0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.540434 jsmetrics-0.1.1b0/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  1519071 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png
+-rw-r--r--   0 runner    (1001) docker     (123)   788211 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/_static/images/jet_shift_violin.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87261 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/_static/images/kuang_jet_centers.png
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/statement.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.540434 jsmetrics-0.1.1b0/jsmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.544435 jsmetrics-0.1.1b0/jsmetrics/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/core/check_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/details_for_all_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.544435 jsmetrics-0.1.1b0/jsmetrics/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/metrics/jet_core_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26250 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/metrics/jet_core_algorithms_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22290 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/metrics/jet_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39836 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/metrics/jet_statistics_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/metrics/waviness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/metrics/waviness_metrics_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.544435 jsmetrics-0.1.1b0/jsmetrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/utils/spatial_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/utils/windspeed_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.544435 jsmetrics-0.1.1b0/jsmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-04-11 16:09:24.000000 jsmetrics-0.1.1b0/jsmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-11 16:09:24.000000 jsmetrics-0.1.1b0/jsmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:09:24.000000 jsmetrics-0.1.1b0/jsmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:09:24.000000 jsmetrics-0.1.1b0/jsmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-11 16:09:24.000000 jsmetrics-0.1.1b0/jsmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 16:09:24.000000 jsmetrics-0.1.1b0/jsmetrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-11 16:09:24.552435 jsmetrics-0.1.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.544435 jsmetrics-0.1.1b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.548435 jsmetrics-0.1.1b0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1262096 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1260860 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1104721 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.548435 jsmetrics-0.1.1b0/tests/metric_verification/
+-rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/metric_verification/metric_verification.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.548435 jsmetrics-0.1.1b0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/unit/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/unit/test_jet_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/unit/test_jet_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/unit/test_spatial_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/unit/test_waviness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/unit/test_windspeed_utils.py
```

### Comparing `jsmetrics-0.1.0/CONTRIBUTING.rst` & `jsmetrics-0.1.1b0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/HISTORY.rst` & `jsmetrics-0.1.1b0/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 =======
 History
 =======
 
+0.1.1-beta (2023-04-07)
+-------------------------
+* add parameter for Kerr et al. 2020
+* Add Ceppi et al jet speed adaptation from Screen et al. 2022
+* Add fix for sort_xarray_data_coords so it works when only one coord value in coordinate (i.e. so each metric can work when only one longitude)
+* Supress warning for quadratic func
+
+
+0.1.1-alpha (2023-03-31)
+-------------------------
+* Add fix for Kuang to run when there is no time dim
+* Add fix for BP15 to except errors where all nan data
+* Add warning for BS17 when more than 10 days resolution
+
 
 0.1.0 (2023-01-22)
 -------------------------
 * MAJOR UPDATE: re-organise the structure of the package into core, metrics and utils
-* rename jet metrics, waviness and jet core algorithm files
+* rename jet statistics, waviness metrics and jet core algorithm files
 * add wrappers to check data is xarray and is sorted in descending order (in core/check_data.py)
 * move waviness metrics to new file
 * Update appropriate tests
 
 
 0.0.19-alpha (2022-12-21)
 -------------------------
```

### Comparing `jsmetrics-0.1.0/LICENSE` & `jsmetrics-0.1.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/PKG-INFO` & `jsmetrics-0.1.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsmetrics
-Version: 0.1.0
+Version: 0.1.1b0
 Summary: Library of algorithms and metrics used to characterise and/or identify jet-streams, based on xarray.
 Home-page: https://github.com/Thomasjkeel/jsmetrics
 Author: Thomas Keel
 Author-email: thomas.keel.18@ucl.ac.uk
 License: MIT License
 Keywords: jet-stream climate metrics algorithms xarray
 Platform: UNKNOWN
@@ -74,16 +74,19 @@
 
     import xarray as xr
     import jsmetrics
 
     # load windspeed data with u- and v- component wind.
     uv_data = xr.open_dataset(filename)
 
+   # run Woollings et al. 2010 metric 
+    w10 = jsmetrics.jet_metrics.woolling_et_al_2010(uv_data)
+
     # run Kuang et al. 2014 metric 
-    k14 = jsmetrics.jetstream_algorithms.kuang_et_al_2014(uv_data)
+    k14 = jsmetrics.jet_core_algorithms.kuang_et_al_2014(uv_data)
 
 .. image:: docs/_static/images/kuang_jet_centers.png
   :width: 360
   :align: center
   :alt: Kuang et al. 2014 Jet-core algorithm
 
 DISCLAIMER
@@ -220,19 +223,33 @@
 ..         :alt: Conda-forge Build Version
 
 
 =======
 History
 =======
 
+0.1.1-beta (2023-04-07)
+-------------------------
+* add parameter for Kerr et al. 2020
+* Add Ceppi et al jet speed adaptation from Screen et al. 2022
+* Add fix for sort_xarray_data_coords so it works when only one coord value in coordinate (i.e. so each metric can work when only one longitude)
+* Supress warning for quadratic func
+
+
+0.1.1-alpha (2023-03-31)
+-------------------------
+* Add fix for Kuang to run when there is no time dim
+* Add fix for BP15 to except errors where all nan data
+* Add warning for BS17 when more than 10 days resolution
+
 
 0.1.0 (2023-01-22)
 -------------------------
 * MAJOR UPDATE: re-organise the structure of the package into core, metrics and utils
-* rename jet metrics, waviness and jet core algorithm files
+* rename jet statistics, waviness metrics and jet core algorithm files
 * add wrappers to check data is xarray and is sorted in descending order (in core/check_data.py)
 * move waviness metrics to new file
 * Update appropriate tests
 
 
 0.0.19-alpha (2022-12-21)
 -------------------------
```

### Comparing `jsmetrics-0.1.0/README.rst` & `jsmetrics-0.1.1b0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,19 @@
 
     import xarray as xr
     import jsmetrics
 
     # load windspeed data with u- and v- component wind.
     uv_data = xr.open_dataset(filename)
 
+   # run Woollings et al. 2010 metric 
+    w10 = jsmetrics.jet_metrics.woolling_et_al_2010(uv_data)
+
     # run Kuang et al. 2014 metric 
-    k14 = jsmetrics.jetstream_algorithms.kuang_et_al_2014(uv_data)
+    k14 = jsmetrics.jet_core_algorithms.kuang_et_al_2014(uv_data)
 
 .. image:: docs/_static/images/kuang_jet_centers.png
   :width: 360
   :align: center
   :alt: Kuang et al. 2014 Jet-core algorithm
 
 DISCLAIMER
```

### Comparing `jsmetrics-0.1.0/docs/Makefile` & `jsmetrics-0.1.1b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png` & `jsmetrics-0.1.1b0/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/docs/_static/images/jet_shift_violin.png` & `jsmetrics-0.1.1b0/docs/_static/images/jet_shift_violin.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/docs/_static/images/kuang_jet_centers.png` & `jsmetrics-0.1.1b0/docs/_static/images/kuang_jet_centers.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/docs/conf.py` & `jsmetrics-0.1.1b0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/docs/index.rst` & `jsmetrics-0.1.1b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/docs/installation.rst` & `jsmetrics-0.1.1b0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/docs/make.bat` & `jsmetrics-0.1.1b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/docs/metrics.rst` & `jsmetrics-0.1.1b0/docs/metrics.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/jsmetrics/core/check_data.py` & `jsmetrics-0.1.1b0/jsmetrics/core/check_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,18 @@
             else:
                 return func(*args, **kwargs)
             check_data_is_xarray(data)
             for coord in coords:
                 assert (
                     coord in data.coords
                 ), f"'{coord}' is not in data. Please check your data and the variable names. Should be like: 'lat', 'lon', 'plev', etc."
+                if data[coord].size == 1 and not data[coord].shape == (1,):
+                    data = data.expand_dims(
+                        coord
+                    )  # expand dimensions so the sortby function works if only one in dim
                 data = data.sortby(coord, ascending=ascending)
             return func(data, *args[1:], **kwargs)
 
         return wrapped_func
 
     return wrap
```

### Comparing `jsmetrics-0.1.0/jsmetrics/details_for_all_metrics.py` & `jsmetrics-0.1.1b0/jsmetrics/details_for_all_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from jsmetrics.metrics import jet_core_algorithms, jet_metrics, waviness_metrics
+from jsmetrics.metrics import jet_core_algorithms, jet_statistics, waviness_metrics
 
 
 # RULES for METRIC_DETAILS dictionary:
 # 1. must have the keys: 'variables', 'coords' 'metric', 'plev_units', 'metric', 'name', 'description, and 'doi'
 # 2. 'variables' will contain the required variable names in the data conforming to the CMIP Controlled Vocabulary (Taylor et al. 2011)
 # 3. 'coords' will contain the required conforming to the CMIP Controlled Vocabulary
 #       and each coord will provide a list of 2 integer values: a minimum and maximum value
@@ -24,15 +24,15 @@
         "description": "",
         "doi": "https://doi.org/10.1002/joc.1255",
     },
     "ArcherCaldeira2008": {
         "variables": ["ua", "va"],
         "coords": {"plev": [10000, 40000]},
         "plev_units": "Pa",
-        "metric": jet_metrics.archer_caldeira_2008,
+        "metric": jet_statistics.archer_caldeira_2008,
         "name": "Archer & Caldeira 2008",
         "description": "",
         "doi": "https://doi.org/10.1029/2008GL033614",
     },
     "Schiemann2009": {
         "variables": ["ua", "va"],
         "coords": {"plev": [10000, 50000]},
@@ -42,15 +42,15 @@
         "description": "",
         "doi": "https://doi.org/10.1175/2008JCLI2625.1",
     },
     "Woollings2010_NorthAtlantic": {
         "variables": ["ua"],
         "coords": {"plev": [70000, 92500], "lat": [15, 75], "lon": [120, 180]},
         "plev_units": "Pa",
-        "metric": jet_metrics.woollings_et_al_2010,
+        "metric": jet_statistics.woollings_et_al_2010,
         "name": "Woollings et al. 2010 North Atlantic",
         "description": "exact coords for metric are: [92500, 85000, 77500, 70000]",
         "doi": "https://onlinelibrary.wiley.com/doi/10.1002/qj.625",
     },
     "Manney2011": {
         "variables": ["ua", "va"],
         "coords": {"plev": [10000, 40000]},
@@ -60,33 +60,33 @@
         "description": "",
         "doi": "https://doi.org/10.5194/acp-11-6115-2011",
     },
     "BarnesPolvani2013_NorthAtlantic": {
         "variables": ["ua"],
         "coords": {"plev": [70000, 85000], "lat": [0, 90], "lon": [300, 360]},
         "plev_units": "Pa",
-        "metric": jet_metrics.barnes_polvani_2013,
+        "metric": jet_statistics.barnes_polvani_2013,
         "name": "Barnes & Polvani 2013 North Atlantic",
         "description": "",
         "doi": "https://doi.org/10.1175/JCLI-D-12-00536.1",
     },
     "BarnesPolvani2013_NorthPacific": {
         "variables": ["ua"],
         "coords": {"plev": [70000, 85000], "lat": [0, 90], "lon": [135, 235]},
         "plev_units": "Pa",
-        "metric": jet_metrics.barnes_polvani_2013,
+        "metric": jet_statistics.barnes_polvani_2013,
         "name": "Barnes & Polvani 2013 North Pacific",
         "description": "",
         "doi": "https://doi.org/10.1175/JCLI-D-12-00536.1",
     },
     "BarnesPolvani2013_SouthernHemisphere": {
         "variables": ["ua"],
         "coords": {"plev": [70000, 85000], "lat": [-90, 0]},
         "plev_units": "Pa",
-        "metric": jet_metrics.barnes_polvani_2013,
+        "metric": jet_statistics.barnes_polvani_2013,
         "name": "Barnes & Polvani 2013 Southern Hemisphere",
         "description": "",
         "doi": "https://doi.org/10.1175/JCLI-D-12-00536.1",
     },
     "PenaOrtiz2013": {
         "variables": ["ua", "va"],
         "coords": {"plev": [10000, 40000]},
@@ -141,15 +141,15 @@
         "description": "",
         "doi": "https://doi.org/10.1007/s00704-013-0994-x",
     },
     "BarnesPolvani2015_NorthAmerica_NorthAtlantic": {
         "variables": ["ua"],
         "coords": {"plev": [70000, 92500], "lat": [30, 70], "lon": [230, 350]},
         "plev_units": "Pa",
-        "metric": jet_metrics.barnes_polvani_2015,
+        "metric": jet_statistics.barnes_polvani_2015,
         "name": "Barnes & Polvani 2015",
         "description": "",
         "doi": "https://doi.org/10.1175/JCLI-D-14-00589.1",
     },
     "FrancisVavrus2015": {
         "variables": ["ua", "va"],
         "coords": {"plev": [50000, 50000]},
@@ -182,73 +182,73 @@
     #     "description": "",
     #     "doi": "https://doi.org/10.1007/s00382-016-3102-y",
     # },
     "BarnesSimpson2017_NorthAtlantic": {
         "variables": ["ua"],
         "coords": {"plev": [70000, 70000], "lat": [1, 90], "lon": [280, 350]},
         "plev_units": "Pa",
-        "metric": jet_metrics.barnes_simpson_2017,
+        "metric": jet_statistics.barnes_simpson_2017,
         "name": "Barnes & Simpson 2017 North Atlantic",
         "description": "",
         "doi": "https://doi.org/10.1175/JCLI-D-17-0299.1",
     },
     "BarnesSimpson2017_NorthPacific": {
         "variables": ["ua"],
         "coords": {"plev": [70000, 70000], "lat": [1, 90], "lon": [120, 230]},
         "plev_units": "Pa",
-        "metric": jet_metrics.barnes_simpson_2017,
+        "metric": jet_statistics.barnes_simpson_2017,
         "name": "Barnes & Simpson 2017 North Pacific",
         "description": "",
         "doi": "https://doi.org/10.1175/JCLI-D-17-0299.1",
     },
     "GrisePolvani2017": {
         "variables": ["ua"],
         "coords": {"plev": [85000, 85000], "lat": [-65, -30]},
         "plev_units": "Pa",
-        "metric": jet_metrics.grise_polvani_2017,
+        "metric": jet_statistics.grise_polvani_2017,
         "name": "Grise & Polvani 2017",
         "description": "",
         "doi": "https://journals.ametsoc.org/doi/10.1175/JCLI-D-16-0849.1",
     },
     # "Molnos2017":
     #     {"variables": ["ua", "va"], "coords":{"plev":[50000, 15000]},
     #      "metric": jetstream_metrics.molnos_et_al_2017,
     #      "description": "Molnos et al 2017"},
     "Bracegirdle2018_SouthernHemisphere": {
         "variables": ["ua"],
         "coords": {"plev": [85000, 85000], "lat": [-75, -10]},
         "plev_units": "Pa",
-        "metric": jet_metrics.bracegirdle_et_al_2018,
+        "metric": jet_statistics.bracegirdle_et_al_2018,
         "name": " Bracegirdle et al. 2018",
         "description": "",
         "doi": "https://doi.org/10.1175/JCLI-D-17-0320.1",
     },
     "Ceppi2018_NorthAtlantic_Europe": {
         "variables": ["ua"],
         "coords": {"plev": [85000, 85000], "lat": [30, 60], "lon": [300, 60]},
         "plev_units": "Pa",
-        "metric": jet_metrics.ceppi_et_al_2018,
+        "metric": jet_statistics.ceppi_et_al_2018,
         "name": "Ceppi et al. 2018 North Atlantic",
         "description": "",
         "doi": "10.1175/JCLI-D-17-0323.1",
     },
     "Ceppi2018_NorthPacific": {
         "variables": ["ua"],
         "coords": {"plev": [85000, 85000], "lat": [30, 60], "lon": [140, 240]},
         "plev_units": "Pa",
-        "metric": jet_metrics.ceppi_et_al_2018,
+        "metric": jet_statistics.ceppi_et_al_2018,
         "name": "Ceppi et al. 2018 North Pacific",
         "description": "",
         "doi": "10.1175/JCLI-D-17-0323.1",
     },
     "Ceppi2018_SouthernHemisphere": {
         "variables": ["ua"],
         "coords": {"plev": [85000, 85000], "lat": [-60, -30]},
         "plev_units": "Pa",
-        "metric": jet_metrics.ceppi_et_al_2018,
+        "metric": jet_statistics.ceppi_et_al_2018,
         "name": "Ceppi et al. 2018 Southern Hemisphere",
         "description": "",
         "doi": "10.1175/JCLI-D-17-0323.1",
     },
     # "Kern2018":
     #     {"variables": ["ua", "va"], "coords":{"plev": [0, 100000]}, "plev_units": "Pa",
     #      "metric": jetstream_metrics.kern_et_al_2018,
@@ -257,22 +257,22 @@
     #     {"variables": ["ua"], "coords":{"plev": [0, 100000]}, "plev_units": "Pa",
     #      "metric": jetstream_metrics.rikus_2018,
     #      "description": "Rikus 2018"},
     "Kerr2020_NorthernHemisphere": {
         "variables": ["ua"],
         "coords": {"plev": [50000, 50000], "lat": [20, 70]},
         "plev_units": "Pa",
-        "metric": jet_metrics.kerr_et_al_2020,
+        "metric": jet_statistics.kerr_et_al_2020,
         "name": "Kerr et al. 2020",
         "description": "",
         "doi": "10.1029/2020JD032735",
     },
     "BlackportFyfe2022_NorthAtlantic": {
         "variables": ["ua"],
         "coords": {"plev": [70000, 70000], "lat": [15, 75], "lon": [300, 360]},
         "plev_units": "Pa",
-        "metric": jet_metrics.blackport_fyfe_2022,
+        "metric": jet_statistics.blackport_fyfe_2022,
         "name": "Blackport & Fyfe 2022",
         "description": "",
         "doi": "10.1126/sciadv.abn3112",
     },
 }
```

### Comparing `jsmetrics-0.1.0/jsmetrics/metrics/jet_core_algorithms.py` & `jsmetrics-0.1.1b0/jsmetrics/metrics/jet_core_algorithms.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,19 +218,24 @@
     if "plev" in data.dims:
         if data["plev"].count() == 1:
             data = data.isel(plev=0)
         else:
             raise ValueError("Please subset to one plev value for algorithm")
 
     # Step 1. Run Jet-stream Occurence and Centre Algorithm
-    if data["time"].size == 1:
+    if "time" not in data.coords:
         output = (
             jet_core_algorithms_components.run_jet_occurence_and_centre_alg_on_one_day(
                 data, occurence_ws_threshold
             )
         )
     else:
-        output = data.groupby("time").map(
-            jet_core_algorithms_components.run_jet_occurence_and_centre_alg_on_one_day,
-            (occurence_ws_threshold,),
-        )
+        if data["time"].size == 1:
+            output = jet_core_algorithms_components.run_jet_occurence_and_centre_alg_on_one_day(
+                data, occurence_ws_threshold
+            )
+        else:
+            output = data.groupby("time").map(
+                jet_core_algorithms_components.run_jet_occurence_and_centre_alg_on_one_day,
+                (occurence_ws_threshold,),
+            )
     return output
```

### Comparing `jsmetrics-0.1.0/jsmetrics/metrics/jet_core_algorithms_components.py` & `jsmetrics-0.1.1b0/jsmetrics/metrics/jet_core_algorithms_components.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/jsmetrics/metrics/jet_metrics.py` & `jsmetrics-0.1.1b0/jsmetrics/metrics/jet_statistics.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
     Classes and Functions ordered by paper publish year.
 """
 
 # imports
 import numpy as np
 import xarray
-from . import jet_metrics_components
-from jsmetrics.utils import spatial_utils, windspeed_utils
+from . import jet_statistics_components
+from jsmetrics.utils import data_utils, spatial_utils, windspeed_utils
 from jsmetrics.core.check_data import sort_xarray_data_coords
 
 # docs
 __author__ = "Thomas Keel"
 __email__ = "thomas.keel.18@ucl.ac.uk"
 __status__ = "Development"
 
@@ -51,22 +51,24 @@
     else:
         mon_mean = data.groupby("time.month").mean()
 
     #  Step 2. Calculate wind-speed from u and v-component wind
     mon_mean["ws"] = windspeed_utils.get_resultant_wind(mon_mean["ua"], mon_mean["va"])
 
     #  Step 3. Calculate mass weighted average
-    mass_weighted_average = jet_metrics_components.calc_mass_weighted_average(
+    mass_weighted_average = jet_statistics_components.calc_mass_weighted_average(
         mon_mean, ws_col="ws"
     )
     mass_flux_weighted_pressure = (
-        jet_metrics_components.calc_mass_flux_weighted_pressure(mon_mean, ws_col="ws")
+        jet_statistics_components.calc_mass_flux_weighted_pressure(
+            mon_mean, ws_col="ws"
+        )
     )
     mass_flux_weighted_latitude = (
-        jet_metrics_components.calc_mass_flux_weighted_latitude(
+        jet_statistics_components.calc_mass_flux_weighted_latitude(
             mon_mean, lat_min=15, lat_max=75, ws_col="ws"
         )
     )
     output = data.assign(
         {
             "mass_weighted_average_ws": (
                 ("month", "lat", "lon"),
@@ -109,42 +111,42 @@
     """
     if isinstance(data, xarray.DataArray):
         data = data.to_dataset()
     # Step 1: Calculate long and/or plev mean
     zonal_mean = windspeed_utils.get_zonal_mean(data)
 
     # Step 2: Apply n-day lancoz filter
-    lancoz_filtered_mean_data = jet_metrics_components.apply_lanczos_filter(
+    lancoz_filtered_mean_data = jet_statistics_components.apply_lanczos_filter(
         zonal_mean["ua"], filter_freq, window_size
     )
 
     # Step 3: Calculate max windspeed and lat where max ws found
     max_lat_ws = np.array(
         list(
             map(
-                jet_metrics_components.get_latitude_and_speed_where_max_ws,
+                jet_statistics_components.get_latitude_and_speed_where_max_ws,
                 lancoz_filtered_mean_data[:],
             )
         )
     )
-    zonal_mean_lat_ws = jet_metrics_components.assign_jet_lat_and_speed_to_data(
+    zonal_mean_lat_ws = jet_statistics_components.assign_jet_lat_and_speed_to_data(
         zonal_mean, max_lat_ws
     )
     # Step 4: Make seasonal climatology
-    climatology = jet_metrics_components.get_climatology(zonal_mean_lat_ws, "season")
+    climatology = jet_statistics_components.get_climatology(zonal_mean_lat_ws, "season")
 
     # Step 5: Apply low-freq fourier filter to both max lats and max ws
-    fourier_filtered_lats = jet_metrics_components.apply_low_freq_fourier_filter(
+    fourier_filtered_lats = jet_statistics_components.apply_low_freq_fourier_filter(
         climatology["jet_lat"].values, highest_freq_to_keep=2
     )
-    fourier_filtered_ws = jet_metrics_components.apply_low_freq_fourier_filter(
+    fourier_filtered_ws = jet_statistics_components.apply_low_freq_fourier_filter(
         climatology["jet_speed"].values, highest_freq_to_keep=2
     )
     time_dim = climatology["jet_speed"].dims[0]
-    output = jet_metrics_components.assign_filtered_lats_and_ws_to_data(
+    output = jet_statistics_components.assign_filtered_lats_and_ws_to_data(
         zonal_mean_lat_ws,
         fourier_filtered_lats.real,
         fourier_filtered_ws.real,
         dim=time_dim,
     )
 
     # Step 6: Calculate jet latitude and jet speed anomalies from the seasonal cycle
@@ -171,59 +173,59 @@
 
     Returns
     ----------
     output : xarray.Dataset
         Data containing values for z_lat, z_spd, z_width for jet-stream latitude, speed and width
     """
     #  Step 1. Get pressure-weighted u-component wind
-    pressure_weighted_ua = jet_metrics_components.calc_mass_weighted_average(
+    pressure_weighted_ua = jet_statistics_components.calc_mass_weighted_average(
         data, ws_col="ua"
     )
     #  Step 2. Filter pressure-weighted u-component wind with low-pass Lanczos filter
-    filtered_pressure_weighted_ua = jet_metrics_components.apply_lanczos_filter(
+    filtered_pressure_weighted_ua = jet_statistics_components.apply_lanczos_filter(
         pressure_weighted_ua,
         filter_freq=filter_freq,
         window_size=window_size,
     )
     #  Step 3. Turn dataarray into dataset for next part
     filtered_pressure_weighted_ua = filtered_pressure_weighted_ua.to_dataset(name="ua")
 
     #  Step 4.  Get max latitude and wind speed at max
     zonal_mean = windspeed_utils.get_zonal_mean(filtered_pressure_weighted_ua)
     all_max_lats_and_ws = np.array(
         list(
             map(
-                jet_metrics_components.get_3_latitudes_and_speed_around_max_ws,
+                jet_statistics_components.get_3_latitudes_and_speed_around_max_ws,
                 zonal_mean["ua"],
             )
         )
     )
 
     #  Step 5. Scale max latitude to 0.01 degree using quadratic function
     scaled_max_lats = []
     scaled_max_ws = []
     for max_lat_and_ws in all_max_lats_and_ws:
         if not np.isnan(np.min(max_lat_and_ws)):
             (
                 scaled_max_lat,
                 scaled_ws,
-            ) = jet_metrics_components.get_latitude_and_speed_where_max_ws_at_reduced_resolution(
+            ) = jet_statistics_components.get_latitude_and_speed_where_max_ws_at_reduced_resolution(
                 max_lat_and_ws, lat_resolution=0.01
             )
             scaled_max_lats.append(scaled_max_lat)
             scaled_max_ws.append(scaled_ws)
         else:
             scaled_max_lats.append(np.nan)
             scaled_max_ws.append(np.nan)
 
     #  Step 6. Get jet-widths using scaled windspeed and usual jet-lat
     max_lats = all_max_lats_and_ws[::, 0, 1]
     jet_widths = list(
         map(
-            lambda zm, la, wa: jet_metrics_components.calc_jet_width_for_one_day(
+            lambda zm, la, wa: jet_statistics_components.calc_jet_width_for_one_day(
                 zm, la, wa
             ),
             zonal_mean["ua"],
             max_lats,
             scaled_max_ws,
         )
     )
@@ -258,20 +260,20 @@
         Data containing jet-stream position and jet-speed
     """
     # Step 1. Get zonal mean
     zonal_mean = windspeed_utils.get_zonal_mean(data)
 
     # Step 2. Get jet lat and jet speed values
     if zonal_mean["time"].size == 1:
-        output = jet_metrics_components.get_jet_lat_and_speed_using_parabola_by_day(
+        output = jet_statistics_components.get_jet_lat_and_speed_using_parabola_by_day(
             zonal_mean
         )
     else:
         output = zonal_mean.groupby("time").map(
-            jet_metrics_components.get_jet_lat_and_speed_using_parabola_by_day
+            jet_statistics_components.get_jet_lat_and_speed_using_parabola_by_day
         )
     return output
 
 
 @sort_xarray_data_coords(coords=["lat", "lon"])
 def barnes_simpson_2017(data):
     """
@@ -291,25 +293,35 @@
          Data with max latitude and max windspeed for North Atlantic (280.E to 350. E) and North Pacific (120.E to 230. E) sectors
     """
     if "plev" in data.dims:
         if data["plev"].count() == 1:
             data = data.isel(plev=0)
         else:
             print(
-                "this metric was meant to only work on one plev, please subset plev to one value"
+                "this metric was meant to only work on one plev, please subset plev to one value. For now taking the mean..."
             )
             data = data.mean("plev")
     data = data.mean("lon")
     if data["time"].size == 1 and "time" not in data.dims:
         data = data.expand_dims("time")
-    data = data.resample(time="10D").mean()
+    if not data.indexes["time"].is_monotonic:
+        raise IndexError("Data needs to have a montonic index")
+    # Check that data can be resampled into 10 days
+    if not data["time"].size == 1:
+        time_step_in_data = int((data["time"][1] - data["time"][0]).dt.days)
+        if time_step_in_data <= 10:
+            data = data.resample(time="10D").mean()
+            time_step_in_data = 10
+        else:
+            print(
+                f"Warning this method was developed for 10 day average and data has larger time-step than 10 days. Time step is {time_step_in_data} days"
+            )
     #  Drop all NaN slices
     data = data.dropna("time")
-    data = jet_metrics_components.calc_latitude_and_speed_where_max_ws(data)
-    data = data.rename_dims({"time": "10_day_average"})
+    data = jet_statistics_components.calc_latitude_and_speed_where_max_ws(data)
     return data
 
 
 @sort_xarray_data_coords(coords=["lat", "lon"])
 def grise_polvani_2017(data):
     """
     Calculates maximum latitude of jet-stream to 0.01 degree resolution each time unit
@@ -339,29 +351,29 @@
     # Step 1. Calculate zonal-mean
     zonal_mean = windspeed_utils.get_zonal_mean(data)
 
     # Step 2. Get the 3 latitudes and speeds around max zonal wind-speed (e.g. lat-1, lat, lat+1)
     all_max_lats_and_ws = np.array(
         list(
             map(
-                jet_metrics_components.get_3_latitudes_and_speed_around_max_ws,
+                jet_statistics_components.get_3_latitudes_and_speed_around_max_ws,
                 zonal_mean["ua"],
             )
         )
     )
 
     #  Step 3. Apply quadratic function to get max latitude at 0.01 degree resolution
     scaled_max_lats = []
     scaled_max_ws = []
     for max_lat_and_ws in all_max_lats_and_ws:
         try:
             (
                 scaled_max_lat,
                 scaled_ws,
-            ) = jet_metrics_components.get_latitude_and_speed_where_max_ws_at_reduced_resolution(
+            ) = jet_statistics_components.get_latitude_and_speed_where_max_ws_at_reduced_resolution(
                 max_lat_and_ws, lat_resolution=0.01
             )
         except Exception as e:
             print(e)
             scaled_max_lat = np.nan
             scaled_ws = np.nan
         scaled_max_lats.append(scaled_max_lat)
@@ -406,42 +418,42 @@
     if isinstance(data, xarray.DataArray):
         data = data.to_dataset()
     if "plev" in data.dims:
         if data["plev"].count() == 1:
             data = data.isel(plev=0)
         else:
             print(
-                "this metric was meant to only work on one plev, please subset plev to one value"
+                "this metric was meant to only work on one plev, please subset plev to one value. For now taking the mean..."
             )
             data = data.mean("plev")
             # raise ValueError("Please subset to one plev value for this metric")
 
     # Step 0: Expand time dimensions so we can map a function to the dataset properly
     if data["time"].size == 1:
         data = data.expand_dims("time")
 
     #  Step 1. Make seasonal & annual climatologies
-    seasonal_climatology = jet_metrics_components.get_climatology(data, "season")
-    annual_climatology = jet_metrics_components.get_climatology(data, "year")
+    seasonal_climatology = jet_statistics_components.get_climatology(data, "season")
+    annual_climatology = jet_statistics_components.get_climatology(data, "year")
 
     #  Step 2. Get zonal mean from climatologies
     seasonal_zonal_mean = seasonal_climatology.mean("lon")
     annual_zonal_mean = annual_climatology.mean("lon")
 
     #  Step 3. Cubic spline interpolation to each climatology at latitude resolution of 0.075 degrees
     (
         seasonal_max_lats,
         seasonal_max_ws,
-    ) = jet_metrics_components.run_cubic_spline_interpolation_for_each_unit_of_climatology_to_get_max_lat_and_ws(
+    ) = jet_statistics_components.run_cubic_spline_interpolation_for_each_unit_of_climatology_to_get_max_lat_and_ws(
         seasonal_zonal_mean, lat_resolution=0.075, time_col="season"
     )
     (
         annual_max_lats,
         annual_max_ws,
-    ) = jet_metrics_components.run_cubic_spline_interpolation_for_each_unit_of_climatology_to_get_max_lat_and_ws(
+    ) = jet_statistics_components.run_cubic_spline_interpolation_for_each_unit_of_climatology_to_get_max_lat_and_ws(
         annual_zonal_mean, lat_resolution=0.075, time_col="year"
     )
 
     # Step 4. Assign jet-stream position (JPOS) and jet-stream strength (JSTR) back to data
     output = data.assign(
         {
             "seasonal_JPOS": (("season"), seasonal_max_lats),
@@ -450,46 +462,96 @@
             "annual_JSTR": (("year"), annual_max_ws),
         }
     )
     return output
 
 
 @sort_xarray_data_coords(coords=["lat", "lon"])
-def ceppi_et_al_2018(data):
+def ceppi_et_al_2018(data, lon_resolution=None):
     """
-    Calculates the jet latitude per time unit where jet-lat is defined as a centroid of a zonal wind distribution
+    Calculates the jet latitude per time unit where jet-lat is defined as a centroid of a zonal wind distribution.
+    This method has been slightly adapted to include a jet speed extraction (after Screen et al. 2022 and refs therein).
     Method from Ceppi et al (2018) https://doi.org/10.1175/JCLI-D-17-0323.1
-    "similar methods used in: Chen et al. 2008; Ceppi et al. 2014"
+
+    Also used in Zappa et al. 2018, Ayres & Screen, 2019 and Screen et al. 2022. Similar methods used in: Chen et al. 2008; Ceppi et al. 2014.
 
     Parameters
     ----------
     data : xarray.Dataset
         Data containing u-component windspeed
+    lon_resolution : numeric
+        Resolution to use for longitude coord if size 1
 
     Returns
     ----------
     output : xarray.Dataset
         Data containing centroid latitude of u-wind for each time unit (e.g. each day)
     """
     #  Step 1. Get area in m2 by latitude/longitude grid cells
-    total_area_m2 = spatial_utils.grid_cell_areas(data["lon"], data["lat"])
+    if not data["lon"].size == 1 and not data["lat"].size == 1:
+        total_area_m2 = spatial_utils.grid_cell_areas(data["lon"], data["lat"])
+    elif lon_resolution and not data["lat"].size == 1 and data["lon"].size == 1:
+        lons_to_use = [float(data["lon"]), float(data["lon"]) + lon_resolution]
+        total_area_m2 = spatial_utils.grid_cell_areas(lons_to_use, data["lat"])
+        total_area_m2 = total_area_m2.mean(axis=1)
+        total_area_m2 = total_area_m2.reshape(-1, 1)
+        if data["lon"].shape == ():
+            data = data.expand_dims("lon")
+    else:
+        raise ValueError(
+            "For this method, your data needs to have at least 2 'lat' values and 'lon' values needs to be more than one unless you set the 'lon_resolution' parameter"
+        )
+
     data["total_area_m2"] = (("lat", "lon"), total_area_m2)
 
     #  Step 2. calculate zonal mean
     zonal_mean = windspeed_utils.get_zonal_mean(data)
 
     # Step 3: Assign laitude of jet-stream centroids to main data
-    data["jet_lat"] = jet_metrics_components.calc_centroid_jet_lat_from_zonal_mean(
+    data["jet_lat"] = jet_statistics_components.calc_centroid_jet_lat_from_zonal_mean(
         zonal_mean, area_by_lat=zonal_mean["total_area_m2"]
     )
+
+    # Expand time dimension
+    if data["time"].size == 1:
+        data = data.expand_dims("time")
+        zonal_mean = zonal_mean.expand_dims("time")
+
+    # Step 4 (adapted from original methodology): Get nearest latitude actually in data to the one determined by metric
+    nearest_latitudes_to_jet_lat_estimates = np.array(
+        list(
+            map(
+                lambda row: data_utils.find_nearest_value_to_array(
+                    data["lat"], float(row)
+                ),
+                data["jet_lat"],
+            )
+        )
+    )
+
+    # Step 5 (adapted from original methodology): Get speed of associated nearest latitude
+    data["jet_speed"] = (
+        ("time",),
+        np.array(
+            list(
+                map(
+                    lambda data_row, lat_val: jet_statistics_components.get_latitude_value_in_data_row(
+                        data_row, lat_val
+                    ),
+                    zonal_mean["ua"],
+                    nearest_latitudes_to_jet_lat_estimates,
+                )
+            )
+        ),
+    )
     return data
 
 
 @sort_xarray_data_coords(coords=["lat", "lon"])
-def kerr_et_al_2020(data):
+def kerr_et_al_2020(data, width_of_pulse=10):
     """
     Described in section 2.4.2 of paper. Defines the latitude of the jet-stream as where the
     maximum zonal winds occur for each longitude for each time unit (i.e. day) before smoothing
     with a rectangular pulse (of width 10 degrees) to get a moving average.
     Method from Kerr et al. (2020) https://onlinelibrary.wiley.com/doi/10.1029/2020JD032735
 
     Parameters
@@ -498,25 +560,34 @@
         Data containing u-component windspeed at one plev
 
     Returns
     ----------
     output : xarray.Dataset
         Data containing jet-stream latitude by longitude and smoothed jet_latitude
     """
-    if data["plev"].size != 1:
-        raise IndexError("Please subset your data to have one pressure level (plev)")
+    if "plev" in data.dims:
+        if data["plev"].count() == 1:
+            data = data.isel(plev=0)
+        else:
+            print(
+                "this metric was meant to only work on one plev, please subset plev to one value. For now taking the mean..."
+            )
+            data = data.mean("plev")
+            # raise ValueError("Please subset to one plev value for this metric")
+
     if data["time"].size == 1:
         output = (
-            jet_metrics_components.get_moving_averaged_smoothed_jet_lats_for_one_day(
-                data
+            jet_statistics_components.get_moving_averaged_smoothed_jet_lats_for_one_day(
+                data, width_of_pulse
             )
         )
     else:
         output = data.groupby("time").map(
-            jet_metrics_components.get_moving_averaged_smoothed_jet_lats_for_one_day
+            jet_statistics_components.get_moving_averaged_smoothed_jet_lats_for_one_day,
+            (width_of_pulse,),
         )
     return output
 
 
 @sort_xarray_data_coords(coords=["lat", "lon"])
 def blackport_fyfe_2022(data):
     """
```

### Comparing `jsmetrics-0.1.0/jsmetrics/metrics/jet_metrics_components.py` & `jsmetrics-0.1.1b0/jsmetrics/metrics/jet_statistics_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     This file is in order of publish year of the metrics
     (see details_for_all_metrics.py)
 
     Functions and Classes ordered by the year of the paper that uses each metric component first
 """
 
 # imports
+import warnings
 import numpy as np
 import xarray as xr
 import scipy.fftpack
 import scipy.interpolate
 import scipy.optimize
 from jsmetrics.utils import data_utils
 
@@ -888,15 +889,17 @@
     Parameters
     ----------
     x : xr.DataArray or array-like
         Array 1
     y : xr.DataArray or array-like
         Array 2
     """
-    p = np.polyfit(x, y, deg=2)
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", category=np.RankWarning)
+        p = np.polyfit(x, y, deg=2)
     return p
 
 
 def apply_quadratic_func(x, y, vals):
     """
     Apply quadratic function to an array of values (vals).
 
@@ -934,19 +937,20 @@
         Data of single time unit containing u-component wind
 
     Returns
     ----------
     data_row : xarray.DataArray
         Data of single time unit containing jet_lat and jet_speed variables
     """
+
     data_ua = abs(data_row["ua"].dropna(dim="lat"))
     try:
         # Try and fit the parabola
         _, coeff = fit_parabola(data_ua["lat"].data, data_ua.data)
-    except RuntimeError:
+    except (RuntimeError, ValueError):
         coeff = [np.nan, np.nan]
     # Check that the max lat is not above the min or max (problem with using a parabola)
     if coeff[0] < data_row["lat"].min() or coeff[0] > data_row["lat"].max():
         coeff = [np.nan, np.nan]
     data_row["jet_lat"] = float(coeff[0])
     data_row["jet_speed"] = float(coeff[1])
     return data_row
@@ -1134,15 +1138,31 @@
         Information on area in each latitude (i.e. m2 per latitude)
     """
     u_hat_by_lat = zonal_mean["ua"] ** 2 * zonal_mean["lat"] * area_by_lat
     u_hat = zonal_mean["ua"] ** 2 * area_by_lat
     return u_hat_by_lat.sum("lat") / u_hat.sum("lat")
 
 
-def get_moving_averaged_smoothed_jet_lats_for_one_day(data_row):
+def get_latitude_value_in_data_row(data_row, lat_val):
+    """
+    Will return the latitude value of a given data row. Needed to loop through data and external array
+
+    Component of method from Ceppi et al (2018) https://doi.org/10.1175/JCLI-D-17-0323.1
+
+    Parameters
+    ----------
+    data_row : xarray.DataArray
+        Data row to extract variable from using given latitude
+    lat_val : float or int
+        latitude value to extract from data row
+    """
+    return float(data_row.sel(lat=lat_val))
+
+
+def get_moving_averaged_smoothed_jet_lats_for_one_day(data_row, width_of_pulse=10):
     """
     Get moving average of smoothed_jet_lats for one day. Used in combination with a groupby mapping.
 
     Component of method from Kerr et al. (2020) https://onlinelibrary.wiley.com/doi/10.1029/2020JD032735
 
     Parameters
     ----------
@@ -1150,17 +1170,17 @@
         Data containing u-component windspeed of one time unit
 
     Returns
     ----------
     smoothed_jet_lat : xarray.Dataset
         Data containing jet-stream position
     """
-    data_row["jet_lat_by_lon"] = get_jet_lat_by_lon(data_row["ua"])
-    data_row["smoothed_jet_lats"] = smooth_jet_lat_across_lon_with_rectangular_pulse(
-        data_row["jet_lat_by_lon"], width_of_pulse=10
+    data_row["jet_lat"] = get_jet_lat_by_lon(data_row["ua"])
+    data_row["smoothed_jet_lat"] = smooth_jet_lat_across_lon_with_rectangular_pulse(
+        data_row["jet_lat"], width_of_pulse=width_of_pulse
     )
     return data_row
 
 
 def smooth_jet_lat_across_lon_with_rectangular_pulse(jet_lat_data, width_of_pulse):
     """
     Smooth jet position (jet latitude) by carrying out a convolution with a rectangular pulse.
```

### Comparing `jsmetrics-0.1.0/jsmetrics/metrics/waviness_metrics.py` & `jsmetrics-0.1.1b0/jsmetrics/metrics/waviness_metrics.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/jsmetrics/metrics/waviness_metrics_components.py` & `jsmetrics-0.1.1b0/jsmetrics/metrics/waviness_metrics_components.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/jsmetrics/utils/data_utils.py` & `jsmetrics-0.1.1b0/jsmetrics/utils/data_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,14 +98,37 @@
         If variables not in data
     """
     for var in req_variables:
         if var not in data.variables:
             raise KeyError("'%s' is not the data" % (var,))
 
 
+def find_nearest_value_to_array(array, value):
+    """
+    Will find the nearest value to a given array
+    Built for use with xarray
+    adapted from: https://stackoverflow.com/questions/2566412/find-nearest-value-in-numpy-array
+
+    Parameters
+    ----------
+    array : array-like
+        Array to reference
+    value : numeric-like
+        Number to check nearest value in input array
+
+    Returns
+    ----------
+    output : numeric
+        Closest value to input value in input array
+    """
+    array = np.asarray(array)
+    idx = (np.abs(array - value)).argmin()
+    return array[idx]
+
+
 def get_local_maxima(arr, axis=0):
     """
     Uses scipy.signal.argrelextrema to get index location of minimum value in array
 
     Taken from
     https://stackoverflow.com/questions/4624970/finding-local-maxima-minima-with-numpy-in-a-1d-numpy-array
```

### Comparing `jsmetrics-0.1.0/jsmetrics/utils/spatial_utils.py` & `jsmetrics-0.1.1b0/jsmetrics/utils/spatial_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/jsmetrics/utils/windspeed_utils.py` & `jsmetrics-0.1.1b0/jsmetrics/utils/windspeed_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/jsmetrics.egg-info/PKG-INFO` & `jsmetrics-0.1.1b0/jsmetrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsmetrics
-Version: 0.1.0
+Version: 0.1.1b0
 Summary: Library of algorithms and metrics used to characterise and/or identify jet-streams, based on xarray.
 Home-page: https://github.com/Thomasjkeel/jsmetrics
 Author: Thomas Keel
 Author-email: thomas.keel.18@ucl.ac.uk
 License: MIT License
 Keywords: jet-stream climate metrics algorithms xarray
 Platform: UNKNOWN
@@ -74,16 +74,19 @@
 
     import xarray as xr
     import jsmetrics
 
     # load windspeed data with u- and v- component wind.
     uv_data = xr.open_dataset(filename)
 
+   # run Woollings et al. 2010 metric 
+    w10 = jsmetrics.jet_metrics.woolling_et_al_2010(uv_data)
+
     # run Kuang et al. 2014 metric 
-    k14 = jsmetrics.jetstream_algorithms.kuang_et_al_2014(uv_data)
+    k14 = jsmetrics.jet_core_algorithms.kuang_et_al_2014(uv_data)
 
 .. image:: docs/_static/images/kuang_jet_centers.png
   :width: 360
   :align: center
   :alt: Kuang et al. 2014 Jet-core algorithm
 
 DISCLAIMER
@@ -220,19 +223,33 @@
 ..         :alt: Conda-forge Build Version
 
 
 =======
 History
 =======
 
+0.1.1-beta (2023-04-07)
+-------------------------
+* add parameter for Kerr et al. 2020
+* Add Ceppi et al jet speed adaptation from Screen et al. 2022
+* Add fix for sort_xarray_data_coords so it works when only one coord value in coordinate (i.e. so each metric can work when only one longitude)
+* Supress warning for quadratic func
+
+
+0.1.1-alpha (2023-03-31)
+-------------------------
+* Add fix for Kuang to run when there is no time dim
+* Add fix for BP15 to except errors where all nan data
+* Add warning for BS17 when more than 10 days resolution
+
 
 0.1.0 (2023-01-22)
 -------------------------
 * MAJOR UPDATE: re-organise the structure of the package into core, metrics and utils
-* rename jet metrics, waviness and jet core algorithm files
+* rename jet statistics, waviness metrics and jet core algorithm files
 * add wrappers to check data is xarray and is sorted in descending order (in core/check_data.py)
 * move waviness metrics to new file
 * Update appropriate tests
 
 
 0.0.19-alpha (2022-12-21)
 -------------------------
```

### Comparing `jsmetrics-0.1.0/jsmetrics.egg-info/SOURCES.txt` & `jsmetrics-0.1.1b0/jsmetrics.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,27 +29,27 @@
 jsmetrics.egg-info/requires.txt
 jsmetrics.egg-info/top_level.txt
 jsmetrics/core/__init__.py
 jsmetrics/core/check_data.py
 jsmetrics/metrics/__init__.py
 jsmetrics/metrics/jet_core_algorithms.py
 jsmetrics/metrics/jet_core_algorithms_components.py
-jsmetrics/metrics/jet_metrics.py
-jsmetrics/metrics/jet_metrics_components.py
+jsmetrics/metrics/jet_statistics.py
+jsmetrics/metrics/jet_statistics_components.py
 jsmetrics/metrics/waviness_metrics.py
 jsmetrics/metrics/waviness_metrics_components.py
 jsmetrics/utils/__init__.py
 jsmetrics/utils/data_utils.py
 jsmetrics/utils/spatial_utils.py
 jsmetrics/utils/windspeed_utils.py
 tests/__init__.py
 tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
 tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
 tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
 tests/metric_verification/metric_verification.ipynb
 tests/unit/__init__.py
 tests/unit/test_data_utils.py
 tests/unit/test_jet_algorithms.py
-tests/unit/test_jet_metrics.py
+tests/unit/test_jet_statistics.py
 tests/unit/test_spatial_utils.py
 tests/unit/test_waviness_metrics.py
 tests/unit/test_windspeed_utils.py
```

### Comparing `jsmetrics-0.1.0/setup.cfg` & `jsmetrics-0.1.1b0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.0
+current_version = 0.1.1-beta
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+).(?P<patch>\d+)(\-(?P<release>[a-z]+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}
 	{major}.{minor}.{patch}
```

### Comparing `jsmetrics-0.1.0/setup.py` & `jsmetrics-0.1.1b0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 NAME = "jsmetrics"
 DESCRIPTION = "Library of algorithms and metrics used to characterise and/or identify jet-streams, based on xarray."
 URL = "https://github.com/Thomasjkeel/jsmetrics"
 AUTHOR = "Thomas Keel"
 AUTHOR_EMAIL = "thomas.keel.18@ucl.ac.uk"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.1.0"
+VERSION = "0.1.1-beta"
 LICENSE = "MIT License"
 
 KEYWORDS = "jet-stream climate metrics algorithms xarray"
 
 with open("README.rst") as file:
     readme = file.read()
```

### Comparing `jsmetrics-0.1.0/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc` & `jsmetrics-0.1.1b0/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc` & `jsmetrics-0.1.1b0/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc` & `jsmetrics-0.1.1b0/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/tests/metric_verification/metric_verification.ipynb` & `jsmetrics-0.1.1b0/tests/metric_verification/metric_verification.ipynb`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/tests/unit/__init__.py` & `jsmetrics-0.1.1b0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/tests/unit/test_data_utils.py` & `jsmetrics-0.1.1b0/tests/unit/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/tests/unit/test_jet_algorithms.py` & `jsmetrics-0.1.1b0/tests/unit/test_jet_algorithms.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/tests/unit/test_jet_metrics.py` & `jsmetrics-0.1.1b0/tests/unit/test_jet_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     Includes:
         – tests for each metric defined and expected outputs
         – test for each utility function used in the metric
 """
 
 # imports
 import unittest
-from jsmetrics.metrics import jet_metrics, jet_metrics_components
+from jsmetrics.metrics import jet_statistics, jet_statistics_components
 from parameterized import parameterized
 import xarray as xr
 import numpy as np
 from jsmetrics import (
     details_for_all_metrics,
 )
 from . import (
@@ -121,29 +121,29 @@
 
 
 class TestArcherCaldeira2008(unittest.TestCase):
     def setUp(self):
         self.data = set_up_test_uv_data()
 
     def test_metric(self):
-        result = jet_metrics.archer_caldeira_2008(self.data)
+        result = jet_statistics.archer_caldeira_2008(self.data)
         for col in [
             "mass_weighted_average_ws",
             "mass_flux_weighted_pressure",
             "mass_flux_weighted_latitude",
         ]:
             self.assertIn(col, result)
             # self.assertEqual(10, result[col].max())
 
         self.assertEqual(
             float(result["mass_weighted_average_ws"].max()), 23.904821395874023
         )
 
     def test_get_mass_weighted_average_windspeed(self):
-        tested_func = jet_metrics.archer_caldeira_2008
+        tested_func = jet_statistics.archer_caldeira_2008
         test_data = self.data.isel(plev=1)
         # should fail because needs two plevs
         self.assertRaises(ValueError, lambda: tested_func(test_data))
 
 
 class TestWoollings2010(unittest.TestCase):
     def setUp(self):
@@ -160,23 +160,23 @@
         time_vec = np.arange(0, 5, time_step)
         test_sig = np.sin(2 * np.pi / period * time_vec) + 0.5 * np.random.randn(
             time_vec.size
         )
         return test_sig
 
     def test_metric(self):
-        tested_func = jet_metrics.woollings_et_al_2010
+        tested_func = jet_statistics.woollings_et_al_2010
         result = tested_func(self.data, filter_freq=1, window_size=2)
         self.assertIsInstance(result, xr.Dataset)
         self.assertEqual(result["ff_jet_lat"][0], 36.25)
         self.assertEqual(result["ff_jet_speed"][0], 43.365413665771484)
         tested_func(self.data["ua"], filter_freq=1, window_size=2)
 
     def test_apply_lancoz_filter(self):
-        tested_func = jet_metrics_components.apply_lanczos_filter
+        tested_func = jet_statistics_components.apply_lanczos_filter
         test_ua = self.data["ua"]
         self.assertRaises(AssertionError, lambda: tested_func(self.data, 2, 4))
         self.assertRaises(AssertionError, lambda: tested_func(test_ua, -2, 1))
         self.assertRaises(ValueError, lambda: tested_func(test_ua, 2, -1))
         self.assertRaises(ValueError, lambda: tested_func(test_ua, 2, 1))
         self.assertRaises(
             ValueError,
@@ -185,72 +185,72 @@
         self.assertRaises(
             ValueError,
             lambda: tested_func(test_ua, 2, test_ua["time"].count() + 1),
         )
         self.assertEqual(float(tested_func(test_ua, 2, 4).max()), 99.514892578125)
 
     def test_get_latitude_and_speed_where_max_ws(self):
-        tested_func = jet_metrics_components.get_latitude_and_speed_where_max_ws
+        tested_func = jet_statistics_components.get_latitude_and_speed_where_max_ws
         self.assertRaises(AttributeError, lambda: tested_func(["lol"]))
         tested_data = self.data["ua"].isel(plev=0, lon=0, time=0)
         self.assertEqual(tested_func(tested_data)[0], 81.25)
         self.assertEqual(tested_func(tested_data)[1], -9.87109375)
         self.assertRaises(
             KeyError, lambda: tested_func(tested_data.rename({"lat": "lt"}))
         )
         nan_dataset = set_up_nan_dataset()
         self.assertEqual(tested_func(nan_dataset), (np.nan, np.nan))
 
     def test_apply_fourier_filter(self):
-        tested_func = jet_metrics_components.apply_low_freq_fourier_filter
+        tested_func = jet_statistics_components.apply_low_freq_fourier_filter
         res = tested_func(self.test_sig, 2)
         self.assertAlmostEqual(res[10].real, -0.0956296962962675, places=7)
 
 
 class TestBarnesPolvani2013(unittest.TestCase):
     def setUp(self):
         self.data = set_up_test_u_data()
 
     def test_metric(self):
-        result = jet_metrics.barnes_polvani_2013(
+        result = jet_statistics.barnes_polvani_2013(
             self.data, filter_freq=1, window_size=2
         )
         self.assertIsInstance(result, xr.Dataset)
         self.assertEqual(result["jet_lat"][1], 35.85)
         self.assertEqual(round(float(result["jet_speed"][2]), 5), 33.1134)
         self.assertEqual(float(result["jet_width"][1]), 17.5)
 
     def test_calc_jet_width_for_one_day(self):
-        test_func = jet_metrics_components.calc_jet_width_for_one_day
+        test_func = jet_statistics_components.calc_jet_width_for_one_day
         self.assertTrue(
             np.isnan(test_func(self.data["ua"].isel(time=0, plev=0), 25, None))
         )
         self.assertTrue(
             np.isnan(
                 test_func(
                     self.data["ua"].isel(time=0, plev=0, lon=0, lat=slice(2, 5)),
                     0,
                     1,
                 )
             )
         )
 
     def test_get_3_latitudes_and_speed_around_max_ws(self):
-        test_func = jet_metrics_components.get_3_latitudes_and_speed_around_max_ws
+        test_func = jet_statistics_components.get_3_latitudes_and_speed_around_max_ws
         test_data = self.data["ua"].isel(time=0, plev=0, lat=slice(0, 2))
         res = test_func(test_data["lat"])
         self.assertEqual(len(res[0]), 3)
         self.assertTrue(np.isnan(res[0][-1]))
         test_data = self.data["ua"].isel(time=0, plev=0, lat=slice(68, 73))
         res = test_func(test_data["lat"])
         self.assertEqual(len(res[0]), 3)
         self.assertTrue(np.isnan(res[0][-1]))
 
     def test_get_3_neighbouring_coord_values(self):
-        test_func = jet_metrics_components.get_3_neighbouring_coord_values
+        test_func = jet_statistics_components.get_3_neighbouring_coord_values
         res = test_func(45, 1)
         self.assertEqual(list(res), [44.0, 45.0, 46.0])
 
 
 class TestScreenSimmonds2013(unittest.TestCase):
     def setUp(self):
         self.data = set_up_test_zg_data()
@@ -261,59 +261,79 @@
 
 
 class TestBarnesPolvani2015(unittest.TestCase):
     def setUp(self):
         self.data = set_up_test_u_data()
 
     def test_metric(self):
-        result = jet_metrics.barnes_polvani_2015(self.data)
+        result = jet_statistics.barnes_polvani_2015(self.data)
         self.assertEqual(round(float(result["jet_lat"].mean()), 5), 43.19160)
         self.assertEqual(round(float(result["jet_speed"].max()), 5), 14.31844)
         self.assertEqual(round(float(result["jet_speed"].min()), 5), 13.52508)
 
 
 class TestBarnesSimpson2017(unittest.TestCase):
     def setUp(self):
         self.data = set_up_test_u_data()
 
     def test_metric(self):
-        test_func = jet_metrics.barnes_simpson_2017
+        test_func = jet_statistics.barnes_simpson_2017
         result = test_func(self.data)
         self.assertEqual(round(float(result["jet_lat"].mean()), 5), 36.25)
         self.assertEqual(round(float(result["jet_speed"].max()), 5), 22.05004)
 
 
 class TestGrisePolvani2017(unittest.TestCase):
     def setUp(self):
         self.data = set_up_test_u_data()
 
     def test_metric(self):
-        result = jet_metrics.grise_polvani_2017(self.data)
-        jet_metrics.grise_polvani_2017(self.data["ua"])
+        result = jet_statistics.grise_polvani_2017(self.data)
+        jet_statistics.grise_polvani_2017(self.data["ua"])
         self.assertEqual(float(result["jet_lat"].min()), 35.38)
         self.assertEqual(float(result["jet_lat"].max()), 36.41)
         self.assertEqual(round(float(result["jet_speed"].max()), 5), 22.92644)
 
 
 class TestCeppi2018(unittest.TestCase):
     def setUp(self):
         self.data = set_up_test_u_data()
 
     def test_metric(self):
-        result = jet_metrics.ceppi_et_al_2018(self.data)
-        print(result)
+        tested_func = jet_statistics.ceppi_et_al_2018
+        result = tested_func(self.data)
         self.assertEqual(float(result["jet_lat"][0].data), 37.316638365674194)
+        self.assertEqual(float(result["jet_speed"][0].data), 22.341136932373047)
+
+    def test_one_latlon_coord(self):
+        tested_func = jet_statistics.ceppi_et_al_2018
+        self.assertRaises(ValueError, lambda: tested_func(self.data.isel(lon=0)))
+        self.assertRaises(ValueError, lambda: tested_func(self.data.isel(lat=0)))
+        self.assertRaises(
+            ValueError, lambda: tested_func(self.data.sel(lat=slice(0, 0)))
+        )
+        self.assertRaises(
+            ValueError, lambda: tested_func(self.data.sel(lon=slice(0, 0)))
+        )
+        tested_func(self.data.sel(lon=slice(0, 0)), lon_resolution=1.875)
+        tested_func(self.data.sel(lon=0), lon_resolution=1.875)
+        self.assertRaises(
+            ValueError,
+            lambda: tested_func(
+                self.data.sel(lon=slice(0, 0), lat=slice(0, 0)), lon_resolution=1.875
+            ),
+        )
 
 
 class TestBracegirdle2018(unittest.TestCase):
     def setUp(self):
         self.data = set_up_test_u_data()
 
     def test_metric(self):
-        tested_func = jet_metrics.bracegirdle_et_al_2018
+        tested_func = jet_statistics.bracegirdle_et_al_2018
         test_data = self.data.sel(plev=slice(85000, 85000))
         result = tested_func(test_data)
         tested_func(test_data["ua"])
         # self.assertRaises(ValueError, lambda: tested_func(self.data))
         self.assertEqual(float(result["seasonal_JPOS"].max()), 37.725)
         self.assertEqual(float(result["annual_JPOS"].max()), 37.725)
         self.assertEqual(round(float(result["seasonal_JSTR"].max()), 3), 8.589)
@@ -321,22 +341,18 @@
 
 
 class TestKerr2020(unittest.TestCase):
     def setUp(self):
         self.data = set_up_test_uv_data()
 
     def test_metric(self):
-        tested_func = jet_metrics.kerr_et_al_2020
-        # Should raise index error as takes only one plev
-        self.assertRaises(IndexError, lambda: tested_func(self.data))
+        tested_func = jet_statistics.kerr_et_al_2020
         test_data = self.data.sel(plev=50000)
         result = tested_func(test_data)
-        self.assertEqual(result["jet_lat_by_lon"].isel(time=0).dropna("lon").size, 192)
-        self.assertEqual(float(result["jet_lat_by_lon"].max()), 72.5)
-        self.assertEqual(float(result["smoothed_jet_lats"].max()), 65.0)
-        self.assertEqual(
-            result["smoothed_jet_lats"].isel(time=0).dropna("lon").size, 61
-        )
+        self.assertEqual(result["jet_lat"].isel(time=0).dropna("lon").size, 192)
+        self.assertEqual(float(result["jet_lat"].max()), 72.5)
+        self.assertEqual(float(result["smoothed_jet_lat"].max()), 65.0)
+        self.assertEqual(result["smoothed_jet_lat"].isel(time=0).dropna("lon").size, 61)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `jsmetrics-0.1.0/tests/unit/test_spatial_utils.py` & `jsmetrics-0.1.1b0/tests/unit/test_spatial_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/tests/unit/test_waviness_metrics.py` & `jsmetrics-0.1.1b0/tests/unit/test_waviness_metrics.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.0/tests/unit/test_windspeed_utils.py` & `jsmetrics-0.1.1b0/tests/unit/test_windspeed_utils.py`

 * *Files identical despite different names*

