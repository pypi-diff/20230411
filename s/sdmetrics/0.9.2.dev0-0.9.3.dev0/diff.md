# Comparing `tmp/sdmetrics-0.9.2.dev0.tar.gz` & `tmp/sdmetrics-0.9.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdmetrics-0.9.2.dev0.tar", last modified: Tue Mar  7 18:37:34 2023, max compression
+gzip compressed data, was "sdmetrics-0.9.3.dev0.tar", last modified: Tue Apr 11 17:54:06 2023, max compression
```

## Comparing `sdmetrics-0.9.2.dev0.tar` & `sdmetrics-0.9.3.dev0.tar`

### file list

```diff
@@ -1,211 +1,213 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.089241 sdmetrics-0.9.2.dev0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      142 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8364 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    16585 2023-03-07 18:29:23.000000 sdmetrics-0.9.2.dev0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1077 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      295 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22735 2023-03-07 18:37:34.089394 sdmetrics-0.9.2.dev0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5223 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.049670 sdmetrics-0.9.2.dev0/docs/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.056952 sdmetrics-0.9.2.dev0/docs/images/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   181646 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/docs/images/column_comparison.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   222559 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/docs/images/column_pairs.png
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.059658 sdmetrics-0.9.2.dev0/sdmetrics/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2089 2023-03-07 18:29:23.000000 sdmetrics-0.9.2.dev0/sdmetrics/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3344 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/base.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.061009 sdmetrics-0.9.2.dev0/sdmetrics/column_pairs/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      551 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/column_pairs/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1867 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/column_pairs/base.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.061741 sdmetrics-0.9.2.dev0/sdmetrics/column_pairs/statistical/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      480 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/column_pairs/statistical/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3367 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/column_pairs/statistical/contingency_similarity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4428 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/column_pairs/statistical/correlation_similarity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4418 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/column_pairs/statistical/kl_divergence.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.062362 sdmetrics-0.9.2.dev0/sdmetrics/demos/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8013 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/demos/multi_table.pkl
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    48099 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/demos/single_table.pkl
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    61272 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/demos/timeseries.pkl
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2451 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/demos.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      130 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      300 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/goal.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.062942 sdmetrics-0.9.2.dev0/sdmetrics/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1611 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1447 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/multi_table/base.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.063718 sdmetrics-0.9.2.dev0/sdmetrics/multi_table/detection/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       71 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/multi_table/detection/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2018 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/multi_table/detection/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4619 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/multi_table/detection/parent_child.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9937 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/multi_table/multi_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.064423 sdmetrics-0.9.2.dev0/sdmetrics/multi_table/statistical/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      352 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/multi_table/statistical/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5932 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/multi_table/statistical/cardinality_shape_similarity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8484 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/multi_table/statistical/cardinality_statistic_similarity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.065011 sdmetrics-0.9.2.dev0/sdmetrics/reports/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/reports/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.066195 sdmetrics-0.9.2.dev0/sdmetrics/reports/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      250 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/reports/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11131 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/reports/multi_table/diagnostic_report.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2081 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/reports/multi_table/plot_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14695 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/reports/multi_table/quality_report.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.066999 sdmetrics-0.9.2.dev0/sdmetrics/reports/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      253 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/reports/single_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9062 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/reports/single_table/diagnostic_report.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12880 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/reports/single_table/plot_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9961 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/reports/single_table/quality_report.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21310 2023-03-07 18:29:23.000000 sdmetrics-0.9.2.dev0/sdmetrics/reports/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.067480 sdmetrics-0.9.2.dev0/sdmetrics/single_column/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1011 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_column/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1938 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_column/base.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.069357 sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      878 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2130 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/boundary_adherence.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2805 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/category_coverage.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2120 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/cstest.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2483 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/kscomplement.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2748 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/missing_value_similarity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2332 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/range_coverage.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3694 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/statistic_similarity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2124 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/tv_complement.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.070837 sdmetrics-0.9.2.dev0/sdmetrics/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3636 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7241 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8748 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/bayesian_network.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.071358 sdmetrics-0.9.2.dev0/sdmetrics/single_table/detection/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      213 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/detection/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4297 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/detection/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2355 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/detection/sklearn.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.072357 sdmetrics-0.9.2.dev0/sdmetrics/single_table/efficacy/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1059 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/efficacy/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4848 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/efficacy/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3062 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/efficacy/binary.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3897 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/efficacy/mlefficacy.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1816 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/efficacy/multiclass.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1412 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/efficacy/regression.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6597 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/gaussian_mixture.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9447 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/multi_column_pairs.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9136 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/multi_single_column.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7518 2023-03-07 18:29:23.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/new_row_synthesis.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.074022 sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1021 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13909 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6127 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/cap.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7982 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/categorical_sklearn.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4255 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/ensemble.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2703 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/loss.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4151 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/numerical_sklearn.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4733 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/radius_nearest_neighbor.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3737 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/util.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.074811 sdmetrics-0.9.2.dev0/sdmetrics/timeseries/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      615 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/timeseries/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3048 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/timeseries/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3919 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/timeseries/detection.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.075330 sdmetrics-0.9.2.dev0/sdmetrics/timeseries/efficacy/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      380 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/timeseries/efficacy/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4195 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/timeseries/efficacy/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      526 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/timeseries/efficacy/classification.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2138 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/timeseries/ml_scorers.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8852 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/sdmetrics/warnings.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.060685 sdmetrics-0.9.2.dev0/sdmetrics.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22735 2023-03-07 18:37:33.000000 sdmetrics-0.9.2.dev0/sdmetrics.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7014 2023-03-07 18:37:34.000000 sdmetrics-0.9.2.dev0/sdmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-03-07 18:37:33.000000 sdmetrics-0.9.2.dev0/sdmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-03-07 18:37:33.000000 sdmetrics-0.9.2.dev0/sdmetrics.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1636 2023-03-07 18:37:33.000000 sdmetrics-0.9.2.dev0/sdmetrics.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       10 2023-03-07 18:37:33.000000 sdmetrics-0.9.2.dev0/sdmetrics.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1425 2023-03-07 18:37:34.090074 sdmetrics-0.9.2.dev0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3717 2023-03-07 18:29:23.000000 sdmetrics-0.9.2.dev0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.075697 sdmetrics-0.9.2.dev0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.076156 sdmetrics-0.9.2.dev0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.076449 sdmetrics-0.9.2.dev0/tests/integration/column_pairs/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       65 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/column_pairs/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.076828 sdmetrics-0.9.2.dev0/tests/integration/column_pairs/statistical/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       77 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/column_pairs/statistical/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3736 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/column_pairs/statistical/test_kl_divergence.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.077798 sdmetrics-0.9.2.dev0/tests/integration/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       64 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2732 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/multi_table/test_multi_single_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      581 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/multi_table/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3719 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/multi_table/test_parent_child.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2932 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/multi_table/test_statistical_metrics.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.077979 sdmetrics-0.9.2.dev0/tests/integration/reports/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/reports/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.078344 sdmetrics-0.9.2.dev0/tests/integration/reports/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       72 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/reports/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2578 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/reports/multi_table/test_multi_table_quality_report.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.078730 sdmetrics-0.9.2.dev0/tests/integration/reports/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       73 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/reports/single_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1823 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/reports/single_table/test_single_table_quality_report.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.078910 sdmetrics-0.9.2.dev0/tests/integration/single_column/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       66 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/single_column/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.079541 sdmetrics-0.9.2.dev0/tests/integration/single_column/statistical/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       66 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/single_column/statistical/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1467 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/single_column/statistical/test_cstest.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1509 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/single_column/statistical/test_kscomplement.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.080059 sdmetrics-0.9.2.dev0/tests/integration/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       65 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/single_table/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.080719 sdmetrics-0.9.2.dev0/tests/integration/single_table/efficacy/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2446 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/single_table/efficacy/test_binary.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1283 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/single_table/efficacy/test_detection.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1677 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/single_table/efficacy/test_multiclass.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1898 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/single_table/efficacy/test_regression.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.080880 sdmetrics-0.9.2.dev0/tests/integration/single_table/privacy/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6178 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/single_table/privacy/test_privacy.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1717 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/single_table/test_gaussian_mixture.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4308 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/single_table/test_single_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1261 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/test_base.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.081206 sdmetrics-0.9.2.dev0/tests/integration/timeseries/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       63 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/timeseries/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.081512 sdmetrics-0.9.2.dev0/tests/integration/timeseries/efficacy/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       72 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/timeseries/efficacy/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      778 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/timeseries/efficacy/test_classification.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1354 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/integration/timeseries/test_timeseries.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.082316 sdmetrics-0.9.2.dev0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       38 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.082678 sdmetrics-0.9.2.dev0/tests/unit/column_pairs/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       46 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/column_pairs/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.083244 sdmetrics-0.9.2.dev0/tests/unit/column_pairs/statistical/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       59 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/column_pairs/statistical/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1515 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/column_pairs/statistical/test_contingency_similarity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6305 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/column_pairs/statistical/test_correlation_similarity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      818 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/column_pairs/test_base.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.083451 sdmetrics-0.9.2.dev0/tests/unit/multi_table/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.083860 sdmetrics-0.9.2.dev0/tests/unit/multi_table/statistical/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6089 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/multi_table/statistical/test_cardinality_shape_similarity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8127 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/multi_table/statistical/test_cardinality_statistic_similarity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3642 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/multi_table/test_multi_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.084064 sdmetrics-0.9.2.dev0/tests/unit/reports/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.085209 sdmetrics-0.9.2.dev0/tests/unit/reports/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    24418 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/reports/multi_table/test_multi_table_diagnostic_report.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1881 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/reports/multi_table/test_multi_table_plot_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    44328 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/reports/multi_table/test_multi_table_quality_report.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.086079 sdmetrics-0.9.2.dev0/tests/unit/reports/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19753 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/reports/single_table/test_single_table_diagnostic_report.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8208 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/reports/single_table/test_single_table_plot_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    31054 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/reports/single_table/test_single_table_quality_report.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    33648 2023-03-07 18:29:23.000000 sdmetrics-0.9.2.dev0/tests/unit/reports/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.086607 sdmetrics-0.9.2.dev0/tests/unit/single_column/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       47 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/single_column/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.088025 sdmetrics-0.9.2.dev0/tests/unit/single_column/statistical/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/single_column/statistical/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1361 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/single_column/statistical/test_boundary_adherence.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2848 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/single_column/statistical/test_category_coverage.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2378 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/single_column/statistical/test_missing_value_similarity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2751 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/single_column/statistical/test_range_coverage.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3543 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/single_column/statistical/test_statistic_similarity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1978 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/single_column/statistical/test_tv_complement.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      823 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/single_column/test_base.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.088589 sdmetrics-0.9.2.dev0/tests/unit/single_table/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.088826 sdmetrics-0.9.2.dev0/tests/unit/single_table/detection/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2518 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/single_table/detection/test_detection.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-03-07 18:37:34.089052 sdmetrics-0.9.2.dev0/tests/unit/single_table/privacy/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      749 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/single_table/privacy/test_util.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7987 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/single_table/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6834 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/single_table/test_multi_single_column.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6338 2023-03-07 18:29:23.000000 sdmetrics-0.9.2.dev0/tests/unit/single_table/test_new_row_synthesis.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1789 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1066 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/test_demos.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6412 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/unit/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      735 2023-02-16 22:23:58.000000 sdmetrics-0.9.2.dev0/tests/utils.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.571921 sdmetrics-0.9.3.dev0/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      142 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/AUTHORS.rst
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     8364 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    17346 2023-04-11 17:49:30.000000 sdmetrics-0.9.3.dev0/HISTORY.md
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1077 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/LICENSE
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      295 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/MANIFEST.in
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    23496 2023-04-11 17:54:06.572266 sdmetrics-0.9.3.dev0/PKG-INFO
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     5223 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/README.md
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.519190 sdmetrics-0.9.3.dev0/docs/
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.528219 sdmetrics-0.9.3.dev0/docs/images/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)   181646 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/docs/images/column_comparison.png
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)   222559 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/docs/images/column_pairs.png
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.530396 sdmetrics-0.9.3.dev0/sdmetrics/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2199 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      825 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/_addons.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3344 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/base.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.531965 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      551 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1867 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/base.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.533379 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      480 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3367 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/contingency_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     5256 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/correlation_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4418 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/kl_divergence.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.534079 sdmetrics-0.9.3.dev0/sdmetrics/demos/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     8013 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/demos/multi_table.pkl
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    48099 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/demos/single_table.pkl
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    61272 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/demos/timeseries.pkl
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2451 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/demos.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      130 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/errors.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      300 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/goal.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.535168 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1611 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1447 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/base.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.536255 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/detection/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       71 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/detection/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2018 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/detection/base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4619 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/detection/parent_child.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    10713 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/multi_single_table.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.537179 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      352 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/statistical/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     5932 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/statistical/cardinality_shape_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     8484 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/multi_table/statistical/cardinality_statistic_similarity.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.537651 sdmetrics-0.9.3.dev0/sdmetrics/reports/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      169 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.538609 sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      250 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    11069 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/diagnostic_report.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2081 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/plot_utils.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    14805 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/quality_report.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.539597 sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      253 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     9171 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/diagnostic_report.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    12880 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/plot_utils.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    10073 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/quality_report.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    24960 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/reports/utils.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.540383 sdmetrics-0.9.3.dev0/sdmetrics/single_column/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1011 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1938 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/base.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.543513 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      878 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2130 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/boundary_adherence.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2805 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/category_coverage.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2120 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/cstest.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2483 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/kscomplement.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2748 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/missing_value_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2332 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/range_coverage.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3694 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/statistic_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2124 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/tv_complement.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.546585 sdmetrics-0.9.3.dev0/sdmetrics/single_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3636 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     7241 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     8748 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/bayesian_network.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.547152 sdmetrics-0.9.3.dev0/sdmetrics/single_table/detection/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      213 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/detection/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4297 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/detection/base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2355 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/detection/sklearn.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.548680 sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1059 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4848 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3062 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/binary.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3897 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/mlefficacy.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1816 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/multiclass.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1412 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/regression.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6597 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/gaussian_mixture.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     9447 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/multi_column_pairs.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     9136 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/multi_single_column.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     7518 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/new_row_synthesis.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.551896 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1021 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    13909 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6127 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/cap.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     7982 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/categorical_sklearn.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4255 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/ensemble.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2703 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/loss.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4151 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/numerical_sklearn.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4733 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/radius_nearest_neighbor.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3737 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/util.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.552682 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      615 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3048 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3919 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/detection.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.553977 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/efficacy/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      380 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/efficacy/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4195 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/efficacy/base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      526 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/efficacy/classification.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2138 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/timeseries/ml_scorers.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     8766 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/utils.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      306 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/sdmetrics/warnings.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.531569 sdmetrics-0.9.3.dev0/sdmetrics.egg-info/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    23496 2023-04-11 17:54:06.000000 sdmetrics-0.9.3.dev0/sdmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     7062 2023-04-11 17:54:06.000000 sdmetrics-0.9.3.dev0/sdmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)        1 2023-04-11 17:54:06.000000 sdmetrics-0.9.3.dev0/sdmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)        1 2023-04-11 17:54:06.000000 sdmetrics-0.9.3.dev0/sdmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1636 2023-04-11 17:54:06.000000 sdmetrics-0.9.3.dev0/sdmetrics.egg-info/requires.txt
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       10 2023-04-11 17:54:06.000000 sdmetrics-0.9.3.dev0/sdmetrics.egg-info/top_level.txt
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1425 2023-04-11 17:54:06.572797 sdmetrics-0.9.3.dev0/setup.cfg
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3717 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/setup.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.554422 sdmetrics-0.9.3.dev0/tests/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       33 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.554901 sdmetrics-0.9.3.dev0/tests/integration/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       45 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.555070 sdmetrics-0.9.3.dev0/tests/integration/column_pairs/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       65 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/column_pairs/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.555468 sdmetrics-0.9.3.dev0/tests/integration/column_pairs/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       77 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/column_pairs/statistical/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3736 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/column_pairs/statistical/test_kl_divergence.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.556983 sdmetrics-0.9.3.dev0/tests/integration/multi_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       64 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/multi_table/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2732 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_multi_single_table.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      581 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_multi_table.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3719 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_parent_child.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2932 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_statistical_metrics.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.557182 sdmetrics-0.9.3.dev0/tests/integration/reports/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       60 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/reports/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.557515 sdmetrics-0.9.3.dev0/tests/integration/reports/multi_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       72 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/reports/multi_table/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2578 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/reports/multi_table/test_multi_table_quality_report.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.557910 sdmetrics-0.9.3.dev0/tests/integration/reports/single_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       73 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/reports/single_table/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1823 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/reports/single_table/test_single_table_quality_report.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.558112 sdmetrics-0.9.3.dev0/tests/integration/single_column/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       66 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_column/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.558678 sdmetrics-0.9.3.dev0/tests/integration/single_column/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       66 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_column/statistical/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1467 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_column/statistical/test_cstest.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1509 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_column/statistical/test_kscomplement.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.559237 sdmetrics-0.9.3.dev0/tests/integration/single_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       65 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.560228 sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2446 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_binary.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1283 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_detection.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1677 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_multiclass.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1898 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_regression.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.560494 sdmetrics-0.9.3.dev0/tests/integration/single_table/privacy/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6178 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/privacy/test_privacy.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1717 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/test_gaussian_mixture.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     4308 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/single_table/test_single_table.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1261 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/test_base.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.561300 sdmetrics-0.9.3.dev0/tests/integration/timeseries/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       63 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/timeseries/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.561692 sdmetrics-0.9.3.dev0/tests/integration/timeseries/efficacy/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       72 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/timeseries/efficacy/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      778 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/timeseries/efficacy/test_classification.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1354 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/integration/timeseries/test_timeseries.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.563610 sdmetrics-0.9.3.dev0/tests/unit/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       38 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.564674 sdmetrics-0.9.3.dev0/tests/unit/column_pairs/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       46 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/column_pairs/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.565449 sdmetrics-0.9.3.dev0/tests/unit/column_pairs/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       59 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/column_pairs/statistical/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1515 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/column_pairs/statistical/test_contingency_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6305 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/column_pairs/statistical/test_correlation_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      818 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/column_pairs/test_base.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.565658 sdmetrics-0.9.3.dev0/tests/unit/multi_table/
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.566311 sdmetrics-0.9.3.dev0/tests/unit/multi_table/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6089 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/multi_table/statistical/test_cardinality_shape_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     8127 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/multi_table/statistical/test_cardinality_statistic_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3642 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/multi_table/test_multi_single_table.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.566515 sdmetrics-0.9.3.dev0/tests/unit/reports/
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.567220 sdmetrics-0.9.3.dev0/tests/unit/reports/multi_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    24434 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/reports/multi_table/test_multi_table_diagnostic_report.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1881 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/reports/multi_table/test_multi_table_plot_utils.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    44827 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/reports/multi_table/test_multi_table_quality_report.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.568151 sdmetrics-0.9.3.dev0/tests/unit/reports/single_table/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    19753 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/reports/single_table/test_single_table_diagnostic_report.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     8208 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/reports/single_table/test_single_table_plot_utils.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    31054 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/reports/single_table/test_single_table_quality_report.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)    39408 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/reports/test_utils.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.568602 sdmetrics-0.9.3.dev0/tests/unit/single_column/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       47 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/__init__.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.570045 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)       60 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/__init__.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1361 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_boundary_adherence.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2848 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_category_coverage.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2378 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_missing_value_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2751 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_range_coverage.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     3543 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_statistic_similarity.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1978 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_tv_complement.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      823 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_column/test_base.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.570894 sdmetrics-0.9.3.dev0/tests/unit/single_table/
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.571116 sdmetrics-0.9.3.dev0/tests/unit/single_table/detection/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     2518 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_table/detection/test_detection.py
+drwxr-xr-x   0 romain_datacebo   (501) staff       (20)        0 2023-04-11 17:54:06.571638 sdmetrics-0.9.3.dev0/tests/unit/single_table/privacy/
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      749 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_table/privacy/test_util.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     7987 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_table/test_base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6834 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_table/test_multi_single_column.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6338 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/single_table/test_new_row_synthesis.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1383 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/test__addons.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1789 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/test_base.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     1066 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/test_demos.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)     6412 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/unit/test_utils.py
+-rw-r--r--   0 romain_datacebo   (501) staff       (20)      735 2023-04-11 14:07:52.000000 sdmetrics-0.9.3.dev0/tests/utils.py
```

### Comparing `sdmetrics-0.9.2.dev0/CONTRIBUTING.rst` & `sdmetrics-0.9.3.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/HISTORY.md` & `sdmetrics-0.9.3.dev0/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # History
 
+## v0.9.2 - 2023-03-08
+
+This release fixes bugs in the  `NewRowSynthesis` metric when too many columns were present. It also fixes bugs around datetime columns that are formatted as strings in both `get_column_pair_plot` and `get_column_plot`.
+
+### Bug Fixes
+* Method get_column_pair_plot: Does not plot synthetic data if datetime column is formatted as a string - Issue [#310] (https://github.com/sdv-dev/SDMetrics/issues/310) by @frances-h
+* Method get_column_plot: ValueError if a datetime column is formatted as a string - Issue [#309](https://github.com/sdv-dev/SDMetrics/issues/309) by @frances-h
+* Fix ValueError in the NewRowSynthesis metric (also impacts DiagnosticReport) - Issue [#307](https://github.com/sdv-dev/SDMetrics/issues/307) by @frances-h
+
 ## v0.9.1 - 2023-02-17
 
 This release fixes bugs in the existing metrics and reports.
 
 ### Bug Fixes
 * Fix issue-296 for discrete and continuous columns - Issue [#296](https://github.com/sdv-dev/SDMetrics/issues/296) by @R-Palazzo
 * Support new metadata for datetime_format - Issue [#303](https://github.com/sdv-dev/SDMetrics/issues/303) by @frances-h
```

### Comparing `sdmetrics-0.9.2.dev0/LICENSE` & `sdmetrics-0.9.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/PKG-INFO` & `sdmetrics-0.9.3.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdmetrics
-Version: 0.9.2.dev0
+Version: 0.9.3.dev0
 Summary: Metrics for Synthetic Data Generation Projects
 Home-page: https://github.com/sdv-dev/SDMetrics
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: sdmetrics sdmetrics SDMetrics
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -169,14 +169,23 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
+## v0.9.2 - 2023-03-08
+
+This release fixes bugs in the  `NewRowSynthesis` metric when too many columns were present. It also fixes bugs around datetime columns that are formatted as strings in both `get_column_pair_plot` and `get_column_plot`.
+
+### Bug Fixes
+* Method get_column_pair_plot: Does not plot synthetic data if datetime column is formatted as a string - Issue [#310] (https://github.com/sdv-dev/SDMetrics/issues/310) by @frances-h
+* Method get_column_plot: ValueError if a datetime column is formatted as a string - Issue [#309](https://github.com/sdv-dev/SDMetrics/issues/309) by @frances-h
+* Fix ValueError in the NewRowSynthesis metric (also impacts DiagnosticReport) - Issue [#307](https://github.com/sdv-dev/SDMetrics/issues/307) by @frances-h
+
 ## v0.9.1 - 2023-02-17
 
 This release fixes bugs in the existing metrics and reports.
 
 ### Bug Fixes
 * Fix issue-296 for discrete and continuous columns - Issue [#296](https://github.com/sdv-dev/SDMetrics/issues/296) by @R-Palazzo
 * Support new metadata for datetime_format - Issue [#303](https://github.com/sdv-dev/SDMetrics/issues/303) by @frances-h
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sdmetrics Version: 0.9.2.dev0 Summary: Metrics for
+Metadata-Version: 2.1 Name: sdmetrics Version: 0.9.3.dev0 Summary: Metrics for
 Synthetic Data Generation Projects Home-page: https://github.com/sdv-dev/
 SDMetrics Author: MIT Data To AI Lab Author-email: dailabmit@gmail.com License:
 MIT license Keywords: sdmetrics sdmetrics SDMetrics Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -73,15 +73,25 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## v0.9.1 - 2023-02-17 This release
+libraries for specific needs. # History ## v0.9.2 - 2023-03-08 This release
+fixes bugs in the `NewRowSynthesis` metric when too many columns were present.
+It also fixes bugs around datetime columns that are formatted as strings in
+both `get_column_pair_plot` and `get_column_plot`. ### Bug Fixes * Method
+get_column_pair_plot: Does not plot synthetic data if datetime column is
+formatted as a string - Issue [#310] (https://github.com/sdv-dev/SDMetrics/
+issues/310) by @frances-h * Method get_column_plot: ValueError if a datetime
+column is formatted as a string - Issue [#309](https://github.com/sdv-dev/
+SDMetrics/issues/309) by @frances-h * Fix ValueError in the NewRowSynthesis
+metric (also impacts DiagnosticReport) - Issue [#307](https://github.com/sdv-
+dev/SDMetrics/issues/307) by @frances-h ## v0.9.1 - 2023-02-17 This release
 fixes bugs in the existing metrics and reports. ### Bug Fixes * Fix issue-296
 for discrete and continuous columns - Issue [#296](https://github.com/sdv-dev/
 SDMetrics/issues/296) by @R-Palazzo * Support new metadata for datetime_format
 - Issue [#303](https://github.com/sdv-dev/SDMetrics/issues/303) by @frances-
 h ## v0.9.0 - 2023-01-18 This release supports Python 3.10 and drops support
 for Python 3.6. We also add a verbosity argument to report generation. ### New
 Features * Silent mode when creating reports. - Issue [#269](https://
```

### Comparing `sdmetrics-0.9.2.dev0/README.md` & `sdmetrics-0.9.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/docs/images/column_comparison.png` & `sdmetrics-0.9.3.dev0/docs/images/column_comparison.png`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/docs/images/column_pairs.png` & `sdmetrics-0.9.3.dev0/docs/images/column_pairs.png`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for SDMetrics."""
 
 __author__ = 'MIT Data To AI Lab'
 __email__ = 'dailabmit@gmail.com'
-__version__ = '0.9.2.dev0'
+__version__ = '0.9.3.dev0'
 
 import pandas as pd
 
 from sdmetrics import (
     column_pairs, demos, goal, multi_table, single_column, single_table, timeseries)
+from sdmetrics._addons import _find_addons
 from sdmetrics.demos import load_demo
 
 __all__ = [
     'demos',
     'load_demo',
     'goal',
     'multi_table',
     'column_pairs',
     'single_column',
     'single_table',
     'timeseries',
 ]
 
+_find_addons(group='sdmetrics_modules', parent_globals=globals())
+
 
 def compute_metrics(metrics, real_data, synthetic_data, metadata=None, **kwargs):
     """Compute a collection of metrics on the given data.
 
     Args:
         metrics (list[sdmetrics.base.BaseMetric]):
             Metrics to compute.
```

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/column_pairs/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/column_pairs/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/column_pairs/statistical/contingency_similarity.py` & `sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/contingency_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/column_pairs/statistical/correlation_similarity.py` & `sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/correlation_similarity.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,29 @@
     """
 
     name = 'CorrelationSimilarity'
     goal = Goal.MAXIMIZE
     min_value = 0.0
     max_value = 1.0
 
+    @staticmethod
+    def _generate_warning_msg(columns, prefix, warning_messages):
+        if len(columns) > 1:
+            cols = ', '.join(columns)
+            warning_messages.append(
+                f"The {prefix} in columns '{cols}' contain a constant value. "
+                'Correlation is undefined for constant data.'
+            )
+
+        elif len(columns):
+            warning_messages.append(
+                f"The {prefix} in column '{columns[0]}' contains a constant value. "
+                'Correlation is undefined for constant data.'
+            )
+
     @classmethod
     def compute_breakdown(cls, real_data, synthetic_data, coefficient='Pearson'):
         """Compare the breakdown of correlation similarity of two continuous columns.
 
         Args:
             real_data (Union[numpy.ndarray, pandas.Series]):
                 The values from the real dataset.
@@ -49,19 +64,23 @@
         synthetic_data = synthetic_data.copy()
 
         if not isinstance(real_data, pd.DataFrame):
             real_data = pd.DataFrame(real_data)
             synthetic_data = pd.DataFrame(synthetic_data)
 
         if (real_data.nunique() == 1).any() or (synthetic_data.nunique() == 1).any():
-            msg = (
-                'One or both of the input arrays is constant. '
-                'The CorrelationSimilarity metric is either undefined or infinite.'
-            )
-            warnings.warn(ConstantInputWarning(msg))
+            warning_messages = []
+            real_columns = list(real_data.loc[:, real_data.nunique() == 1].columns)
+            synthetic_columns = list(synthetic_data.loc[:, synthetic_data.nunique() == 1].columns)
+            cls._generate_warning_msg(real_columns, 'real data', warning_messages)
+            cls._generate_warning_msg(synthetic_columns, 'synthetic data', warning_messages)
+
+            for msg in warning_messages:
+                warnings.warn(ConstantInputWarning(msg))
+
             return {'score': np.nan}
 
         real_data = real_data.dropna()
         synthetic_data = synthetic_data.dropna()
         column1, column2 = real_data.columns[:2]
 
         if is_datetime(real_data[column1]):
```

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/column_pairs/statistical/kl_divergence.py` & `sdmetrics-0.9.3.dev0/sdmetrics/column_pairs/statistical/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/demos/multi_table.pkl` & `sdmetrics-0.9.3.dev0/sdmetrics/demos/multi_table.pkl`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/demos/single_table.pkl` & `sdmetrics-0.9.3.dev0/sdmetrics/demos/single_table.pkl`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/demos/timeseries.pkl` & `sdmetrics-0.9.3.dev0/sdmetrics/demos/timeseries.pkl`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/demos.py` & `sdmetrics-0.9.3.dev0/sdmetrics/demos.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/multi_table/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/multi_table/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/multi_table/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/multi_table/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/multi_table/detection/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/multi_table/detection/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/multi_table/detection/parent_child.py` & `sdmetrics-0.9.3.dev0/sdmetrics/multi_table/detection/parent_child.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/multi_table/multi_single_table.py` & `sdmetrics-0.9.3.dev0/sdmetrics/multi_table/multi_single_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """MultiTable metrics based on applying SingleTable metrics on all the tables."""
 
+import warnings
 from collections import defaultdict
 
 import numpy as np
 
 from sdmetrics import single_table
 from sdmetrics.errors import IncomputableMetricError
 from sdmetrics.multi_table.base import MultiTableMetric
 from sdmetrics.utils import nested_attrs_meta
+from sdmetrics.warnings import SDMetricsWarning
 
 
 class MultiSingleTableMetric(MultiTableMetric, metaclass=nested_attrs_meta('single_table_metric')):
     """MultiTableMetric subclass that applies a SingleTableMetric on each table.
 
     This class can either be used by creating a subclass that inherits from it and
     sets the SingleTable Metric as the ``single_table_metric`` attribute,
@@ -33,27 +35,38 @@
 
     single_table_metric = None
 
     def __init__(self, single_table_metric):
         self.single_table_metric = single_table_metric
         self.compute = self._compute
 
+    @staticmethod
+    def _multitable_warning(caught_warnings, table_name):
+        for warning in caught_warnings:
+            if issubclass(warning.category, SDMetricsWarning):
+                prefixes = ['The real data in', 'The synthetic data in']
+                message = str(warning.message)
+                for prefix in prefixes:
+                    message = message.replace(prefix, f"{prefix[:-3]} in table '{table_name}',")
+
+                warnings.warn(warning.category(message))
+
     def _compute(self, real_data, synthetic_data, metadata=None, **kwargs):
         """Compute this metric.
 
         This applies the underlying single table metric to all the tables
         found in the dataset and then returns the average score obtained.
 
         Args:
             real_data (dict[str, pandas.DataFrame]):
                 The tables from the real dataset.
             synthetic_data (dict[str, pandas.DataFrame]):
                 The tables from the synthetic dataset.
             metadata (dict):
-                Multi-table metadata dict. If not passed, it is build based on the
+                Multi-table metadata dict. If not passed, it is built based on the
                 real_data fields and dtypes.
             **kwargs:
                 Any additional keyword arguments will be passed down
                 to the single table metric
 
         Returns:
             Union[float, tuple[float]]:
@@ -69,24 +82,28 @@
 
         scores = {}
         errors = {}
         for table_name, real_table in real_data.items():
             synthetic_table = synthetic_data[table_name]
             table_meta = metadata['tables'][table_name]
 
-            try:
-                score_breakdown = self.single_table_metric.compute_breakdown(
-                    real_table, synthetic_table, table_meta, **kwargs)
-                scores[table_name] = score_breakdown
-            except AttributeError:
-                score = self.single_table_metric.compute(
-                    real_table, synthetic_table, table_meta, **kwargs)
-                scores[table_name] = score
-            except Exception as error:
-                errors[table_name] = error
+            with warnings.catch_warnings(record=True) as caught_warnings:
+                try:
+                    score_breakdown = self.single_table_metric.compute_breakdown(
+                        real_table, synthetic_table, table_meta, **kwargs)
+                    scores[table_name] = score_breakdown
+                except AttributeError:
+                    score = self.single_table_metric.compute(
+                        real_table, synthetic_table, table_meta, **kwargs)
+                    scores[table_name] = score
+                except Exception as error:
+                    errors[table_name] = error
+
+            if caught_warnings:
+                self._multitable_warning(caught_warnings, table_name)
 
         if not scores:
             raise IncomputableMetricError(f'Encountered the following errors: {errors}')
 
         return scores
 
     @classmethod
@@ -98,15 +115,15 @@
 
         Args:
             real_data (dict[str, pandas.DataFrame]):
                 The tables from the real dataset.
             synthetic_data (dict[str, pandas.DataFrame]):
                 The tables from the synthetic dataset.
             metadata (dict):
-                Multi-table metadata dict. If not passed, it is build based on the
+                Multi-table metadata dict. If not passed, it is built based on the
                 real_data fields and dtypes.
             **kwargs:
                 Any additional keyword arguments will be passed down
                 to the single table metric
 
         Returns:
             Union[float, tuple[float]]:
@@ -137,15 +154,15 @@
 
         Args:
             real_data (dict[str, pandas.DataFrame]):
                 The tables from the real dataset.
             synthetic_data (dict[str, pandas.DataFrame]):
                 The tables from the synthetic dataset.
             metadata (dict):
-                Multi-table metadata dict. If not passed, it is build based on the
+                Multi-table metadata dict. If not passed, it is built based on the
                 real_data fields and dtypes.
             **kwargs:
                 Any additional keyword arguments will be passed down
                 to the single table metric
 
         Returns:
             dict[string -> dict[string -> Union[float, tuple[float]]]]:
```

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/multi_table/statistical/cardinality_shape_similarity.py` & `sdmetrics-0.9.3.dev0/sdmetrics/multi_table/statistical/cardinality_shape_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/multi_table/statistical/cardinality_statistic_similarity.py` & `sdmetrics-0.9.3.dev0/sdmetrics/multi_table/statistical/cardinality_statistic_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/reports/multi_table/diagnostic_report.py` & `sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/diagnostic_report.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
 from sdmetrics.errors import IncomputableMetricError
 from sdmetrics.multi_table import (
     BoundaryAdherence, CategoryCoverage, NewRowSynthesis, RangeCoverage)
 from sdmetrics.reports.single_table.plot_utils import (
     get_column_boundaries_plot, get_column_coverage_plot, get_synthesis_plot)
 from sdmetrics.reports.utils import (
-    DIAGNOSTIC_REPORT_RESULT_DETAILS, aggregate_metric_results, print_results_for_level)
+    DIAGNOSTIC_REPORT_RESULT_DETAILS, aggregate_metric_results, print_results_for_level,
+    validate_multi_table_inputs)
 
 
 class DiagnosticReport():
     """Multi table diagnostic report.
 
     This class creates a diagnostic report for multi-table data. It calculates the diagnostic
     score along three properties - synthesis, coverage, and boundaries.
@@ -78,24 +79,23 @@
             synthetic_data (pandas.DataFrame):
                 The synthetic data.
             metadata (dict):
                 The metadata, which contains each column's data type as well as relationships.
             verbose (bool):
                 Whether or not to print report summary and progress.
         """
+        validate_multi_table_inputs(real_data, synthetic_data, metadata)
+
         metadata = metadata.copy()
         if 'relationships' in metadata:
             for rel in metadata['relationships']:
                 table_meta = metadata['tables'][rel['child_table_name']]
                 table_meta['columns'][rel['child_foreign_key']] = {'sdtype': 'id'}
 
         metrics = list(itertools.chain.from_iterable(self.METRICS.values()))
-        self._metric_args['NewRowSynthesis']['synthetic_sample_size'] = min(
-            len(real_data), self._metric_args['NewRowSynthesis']['synthetic_sample_size'])
-
         for metric in tqdm.tqdm(metrics, desc='Creating report', disable=(not verbose)):
             metric_name = metric.__name__
             try:
                 metric_args = self._metric_args.get(metric_name, {})
                 self._metric_results[metric_name] = metric.compute_breakdown(
                     real_data, synthetic_data, metadata, **metric_args)
                 self._metric_averages_by_table[metric_name] = {}
```

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/reports/multi_table/plot_utils.py` & `sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/plot_utils.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/reports/multi_table/quality_report.py` & `sdmetrics-0.9.3.dev0/sdmetrics/reports/multi_table/quality_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
 from sdmetrics.errors import IncomputableMetricError
 from sdmetrics.multi_table import (
     CardinalityShapeSimilarity, ContingencySimilarity, CorrelationSimilarity, KSComplement,
     TVComplement)
 from sdmetrics.reports.multi_table.plot_utils import get_table_relationships_plot
 from sdmetrics.reports.single_table.plot_utils import get_column_pairs_plot, get_column_shapes_plot
-from sdmetrics.reports.utils import aggregate_metric_results, discretize_and_apply_metric
+from sdmetrics.reports.utils import (
+    aggregate_metric_results, discretize_and_apply_metric, validate_multi_table_inputs)
 
 
 class QualityReport():
     """Multi table quality report.
 
     This class creates a quality report for multi-table data. It calculates the quality
     score along three properties - Column Shapes, Column Pair Trends, and Parent Child
@@ -67,14 +68,16 @@
             synthetic_data (pandas.DataFrame):
                 The synthetic data.
             metadata (dict):
                 The metadata, which contains each column's data type as well as relationships.
             verbose (bool):
                 Whether or not to print report summary and progress.
         """
+        validate_multi_table_inputs(real_data, synthetic_data, metadata)
+
         metadata = metadata.copy()
         if 'relationships' in metadata:
             for rel in metadata['relationships']:
                 table_meta = metadata['tables'][rel['child_table_name']]
                 table_meta['columns'][rel['child_foreign_key']] = {'sdtype': 'id'}
 
         metrics = list(itertools.chain.from_iterable(self.METRICS.values()))
```

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/reports/single_table/diagnostic_report.py` & `sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/diagnostic_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 import pkg_resources
 import tqdm
 
 from sdmetrics.errors import IncomputableMetricError
 from sdmetrics.reports.single_table.plot_utils import (
     get_column_boundaries_plot, get_column_coverage_plot, get_synthesis_plot)
 from sdmetrics.reports.utils import (
-    DIAGNOSTIC_REPORT_RESULT_DETAILS, aggregate_metric_results, print_results_for_level)
+    DIAGNOSTIC_REPORT_RESULT_DETAILS, aggregate_metric_results, print_results_for_level,
+    validate_single_table_inputs)
 from sdmetrics.single_table import (
     BoundaryAdherence, CategoryCoverage, NewRowSynthesis, RangeCoverage)
 
 
 class DiagnosticReport():
     """Single table diagnostic report.
 
@@ -76,14 +77,16 @@
             synthetic_data (pandas.DataFrame):
                 The synthetic data.
             metadata (dict):
                 The metadata, which contains each column's data type as well as relationships.
             verbose (bool):
                 Whether or not to print report summary and progress.
         """
+        validate_single_table_inputs(real_data, synthetic_data, metadata)
+
         metrics = list(itertools.chain.from_iterable(self.METRICS.values()))
         self._metric_args['NewRowSynthesis']['synthetic_sample_size'] = min(
             min(len(real_data), len(synthetic_data)),
             self._metric_args['NewRowSynthesis']['synthetic_sample_size'],
         )
 
         for metric in tqdm.tqdm(metrics, desc='Creating report', disable=(not verbose)):
```

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/reports/single_table/plot_utils.py` & `sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/plot_utils.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/reports/single_table/quality_report.py` & `sdmetrics-0.9.3.dev0/sdmetrics/reports/single_table/quality_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import numpy as np
 import pandas as pd
 import pkg_resources
 import tqdm
 
 from sdmetrics.errors import IncomputableMetricError
 from sdmetrics.reports.single_table.plot_utils import get_column_pairs_plot, get_column_shapes_plot
-from sdmetrics.reports.utils import aggregate_metric_results, discretize_and_apply_metric
+from sdmetrics.reports.utils import (
+    aggregate_metric_results, discretize_and_apply_metric, validate_single_table_inputs)
 from sdmetrics.single_table import (
     ContingencySimilarity, CorrelationSimilarity, KSComplement, TVComplement)
 
 
 class QualityReport():
     """Single table quality report.
 
@@ -63,14 +64,16 @@
             synthetic_data (pandas.DataFrame):
                 The synthetic data.
             metadata (dict):
                 The metadata, which contains each column's data type as well as relationships.
             verbose (bool):
                 Whether or not to print report summary and progress.
         """
+        validate_single_table_inputs(real_data, synthetic_data, metadata)
+
         metrics = list(itertools.chain.from_iterable(self.METRICS.values()))
 
         for metric in tqdm.tqdm(metrics, desc='Creating report', disable=(not verbose)):
             try:
                 self._metric_results[metric.__name__] = metric.compute_breakdown(
                     real_data, synthetic_data, metadata)
             except IncomputableMetricError:
```

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/reports/utils.py` & `sdmetrics-0.9.3.dev0/sdmetrics/reports/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Report utility methods."""
 
 import copy
 import itertools
+import warnings
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.figure_factory as ff
 from pandas.core.tools.datetimes import _guess_datetime_format_for_array
 
@@ -620,7 +621,94 @@
     """
     level_marks = {'SUCCESS': '✓', 'WARNING': '!', 'DANGER': 'x'}
 
     if len(results[level]) > 0:
         out.write(f'\n{level}:\n')
         for result in results[level]:
             out.write(f'{level_marks[level]} {result}\n')
+
+
+def _validate_categorical_values(real_data, synthetic_data, metadata, table=None):
+    """Get categorical values found in synthetic data but not real data for all columns.
+
+    Args:
+        real_data (pd.DataFrame):
+            The real data.
+        synthetic_data (pd.DataFrame):
+            The synthetic data.
+        metadata (dict):
+            The metadata.
+        table (str, optional):
+            The name of the current table, if one exists
+    """
+    if table:
+        warning_format = ('Unexpected values ({values}) in column "{column}" '
+                          f'and table "{table}"')
+    else:
+        warning_format = 'Unexpected values ({values}) in column "{column}"'
+
+    columns = get_columns_from_metadata(metadata)
+    for column, column_meta in columns.items():
+        column_type = get_type_from_column_meta(column_meta)
+        if column_type == 'categorical':
+            extra_categories = [
+                value for value in synthetic_data[column].unique()
+                if value not in real_data[column].unique()
+            ]
+            if extra_categories:
+                value_list = '", "'.join(str(value) for value in extra_categories[:5])
+                values = f'"{value_list}" + more' if len(
+                    extra_categories) > 5 else f'"{value_list}"'
+                warnings.warn(warning_format.format(values=values, column=column))
+
+
+def validate_multi_table_inputs(real_data, synthetic_data, metadata):
+    """Validate multi-table inputs for report generation.
+
+    Args:
+        real_data (dict[str, DataFrame]):
+            The real data.
+        synthetic_data (dict[str, DataFrame]):
+            The synthetic data.
+        metadata (dict):
+            The metadata, which contains each column's data type as well as relationships.
+    """
+    if not isinstance(metadata, dict):
+        metadata = metadata.to_dict()
+
+    for table in metadata['tables']:
+        table_metadata = metadata['tables'][table]
+        _validate_categorical_values(real_data[table],
+                                     synthetic_data[table],
+                                     table_metadata,
+                                     table=table)
+
+    for rel in metadata.get('relationships', []):
+        parent_dtype = real_data[rel['parent_table_name']][rel['parent_primary_key']].dtype
+        child_dtype = real_data[rel['child_table_name']][rel['child_foreign_key']].dtype
+        if (parent_dtype == 'object' and child_dtype != 'object') or (
+                parent_dtype != 'object' and child_dtype == 'object'):
+            parent = rel['parent_table_name']
+            parent_key = rel['parent_primary_key']
+            child = rel['child_table_name']
+            child_key = rel['child_foreign_key']
+            error_msg = (f"The '{parent}' table and '{child}' table cannot be merged. Please "
+                         f"make sure the primary key in '{parent}' ('{parent_key}') and the "
+                         f"foreign key in '{child}' ('{child_key}') have the same data type.")
+            raise ValueError(error_msg)
+
+
+def validate_single_table_inputs(real_data, synthetic_data, metadata):
+    """Validate single table inputs for report generation.
+
+    Args:
+        real_data (pandas.DataFrame):
+            The real data.
+        synthetic_data (pandas.DataFrame):
+            The synthetic data.
+        metadata (dict):
+            The metadata, which contains each column's data type as well as relationships.
+    """
+    if not isinstance(metadata, dict):
+        metadata = metadata.to_dict()
+
+    _validate_categorical_values(real_data, synthetic_data, metadata)
```

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_column/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_column/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/boundary_adherence.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/boundary_adherence.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/category_coverage.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/category_coverage.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/cstest.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/cstest.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/kscomplement.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/kscomplement.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/missing_value_similarity.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/missing_value_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/range_coverage.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/range_coverage.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/statistic_similarity.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/statistic_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_column/statistical/tv_complement.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_column/statistical/tv_complement.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/bayesian_network.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/bayesian_network.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/detection/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/detection/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/detection/sklearn.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/detection/sklearn.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/efficacy/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/efficacy/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/efficacy/binary.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/binary.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/efficacy/mlefficacy.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/mlefficacy.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/efficacy/multiclass.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/multiclass.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/efficacy/regression.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/efficacy/regression.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/gaussian_mixture.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/multi_column_pairs.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/multi_column_pairs.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/multi_single_column.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/multi_single_column.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/new_row_synthesis.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/new_row_synthesis.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/cap.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/cap.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/categorical_sklearn.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/categorical_sklearn.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/ensemble.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/ensemble.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/loss.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/loss.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/numerical_sklearn.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/numerical_sklearn.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/radius_nearest_neighbor.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/radius_nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/single_table/privacy/util.py` & `sdmetrics-0.9.3.dev0/sdmetrics/single_table/privacy/util.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/timeseries/__init__.py` & `sdmetrics-0.9.3.dev0/sdmetrics/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/timeseries/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/timeseries/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/timeseries/detection.py` & `sdmetrics-0.9.3.dev0/sdmetrics/timeseries/detection.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/timeseries/efficacy/base.py` & `sdmetrics-0.9.3.dev0/sdmetrics/timeseries/efficacy/base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/timeseries/efficacy/classification.py` & `sdmetrics-0.9.3.dev0/sdmetrics/timeseries/efficacy/classification.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/timeseries/ml_scorers.py` & `sdmetrics-0.9.3.dev0/sdmetrics/timeseries/ml_scorers.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics/utils.py` & `sdmetrics-0.9.3.dev0/sdmetrics/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """SDMetrics utils to be used across all the project."""
 
-import warnings
 from collections import Counter
 from datetime import datetime
 
 import numpy as np
 import pandas as pd
 from sklearn.preprocessing import OneHotEncoder
 
@@ -60,15 +59,14 @@
         tuble[list, list]:
             The observed and expected frequencies (as a percent).
     """
     f_obs, f_exp = [], []
     real, synthetic = Counter(real), Counter(synthetic)
     for value in synthetic:
         if value not in real:
-            warnings.warn(f'Unexpected value {value} in synthetic data.')
             real[value] += 1e-6  # Regularization to prevent NaN.
 
     for value in real:
         f_obs.append(synthetic[value] / sum(synthetic.values()))  # noqa: PD011
         f_exp.append(real[value] / sum(real.values()))  # noqa: PD011
 
     return f_obs, f_exp
@@ -279,13 +277,13 @@
 
     Returns:
         list:
             The list of alternate keys.
     """
     alternate_keys = []
     for alternate_key in metadata.get('alternate_keys', []):
-        if type(alternate_key) is list:
+        if isinstance(alternate_key, list):
             alternate_keys.extend(alternate_key)
         else:
             alternate_keys.append(alternate_key)
 
     return alternate_keys
```

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics.egg-info/PKG-INFO` & `sdmetrics-0.9.3.dev0/sdmetrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdmetrics
-Version: 0.9.2.dev0
+Version: 0.9.3.dev0
 Summary: Metrics for Synthetic Data Generation Projects
 Home-page: https://github.com/sdv-dev/SDMetrics
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: sdmetrics sdmetrics SDMetrics
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -169,14 +169,23 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
+## v0.9.2 - 2023-03-08
+
+This release fixes bugs in the  `NewRowSynthesis` metric when too many columns were present. It also fixes bugs around datetime columns that are formatted as strings in both `get_column_pair_plot` and `get_column_plot`.
+
+### Bug Fixes
+* Method get_column_pair_plot: Does not plot synthetic data if datetime column is formatted as a string - Issue [#310] (https://github.com/sdv-dev/SDMetrics/issues/310) by @frances-h
+* Method get_column_plot: ValueError if a datetime column is formatted as a string - Issue [#309](https://github.com/sdv-dev/SDMetrics/issues/309) by @frances-h
+* Fix ValueError in the NewRowSynthesis metric (also impacts DiagnosticReport) - Issue [#307](https://github.com/sdv-dev/SDMetrics/issues/307) by @frances-h
+
 ## v0.9.1 - 2023-02-17
 
 This release fixes bugs in the existing metrics and reports.
 
 ### Bug Fixes
 * Fix issue-296 for discrete and continuous columns - Issue [#296](https://github.com/sdv-dev/SDMetrics/issues/296) by @R-Palazzo
 * Support new metadata for datetime_format - Issue [#303](https://github.com/sdv-dev/SDMetrics/issues/303) by @frances-h
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sdmetrics Version: 0.9.2.dev0 Summary: Metrics for
+Metadata-Version: 2.1 Name: sdmetrics Version: 0.9.3.dev0 Summary: Metrics for
 Synthetic Data Generation Projects Home-page: https://github.com/sdv-dev/
 SDMetrics Author: MIT Data To AI Lab Author-email: dailabmit@gmail.com License:
 MIT license Keywords: sdmetrics sdmetrics SDMetrics Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -73,15 +73,25 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## v0.9.1 - 2023-02-17 This release
+libraries for specific needs. # History ## v0.9.2 - 2023-03-08 This release
+fixes bugs in the `NewRowSynthesis` metric when too many columns were present.
+It also fixes bugs around datetime columns that are formatted as strings in
+both `get_column_pair_plot` and `get_column_plot`. ### Bug Fixes * Method
+get_column_pair_plot: Does not plot synthetic data if datetime column is
+formatted as a string - Issue [#310] (https://github.com/sdv-dev/SDMetrics/
+issues/310) by @frances-h * Method get_column_plot: ValueError if a datetime
+column is formatted as a string - Issue [#309](https://github.com/sdv-dev/
+SDMetrics/issues/309) by @frances-h * Fix ValueError in the NewRowSynthesis
+metric (also impacts DiagnosticReport) - Issue [#307](https://github.com/sdv-
+dev/SDMetrics/issues/307) by @frances-h ## v0.9.1 - 2023-02-17 This release
 fixes bugs in the existing metrics and reports. ### Bug Fixes * Fix issue-296
 for discrete and continuous columns - Issue [#296](https://github.com/sdv-dev/
 SDMetrics/issues/296) by @R-Palazzo * Support new metadata for datetime_format
 - Issue [#303](https://github.com/sdv-dev/SDMetrics/issues/303) by @frances-
 h ## v0.9.0 - 2023-01-18 This release supports Python 3.10 and drops support
 for Python 3.6. We also add a verbosity argument to report generation. ### New
 Features * Silent mode when creating reports. - Issue [#269](https://
```

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics.egg-info/SOURCES.txt` & `sdmetrics-0.9.3.dev0/sdmetrics.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 docs/images/column_comparison.png
 docs/images/column_pairs.png
 sdmetrics/__init__.py
+sdmetrics/_addons.py
 sdmetrics/base.py
 sdmetrics/demos.py
 sdmetrics/errors.py
 sdmetrics/goal.py
 sdmetrics/utils.py
 sdmetrics/warnings.py
 sdmetrics.egg-info/PKG-INFO
@@ -122,14 +123,15 @@
 tests/integration/single_table/efficacy/test_regression.py
 tests/integration/single_table/privacy/test_privacy.py
 tests/integration/timeseries/__init__.py
 tests/integration/timeseries/test_timeseries.py
 tests/integration/timeseries/efficacy/__init__.py
 tests/integration/timeseries/efficacy/test_classification.py
 tests/unit/__init__.py
+tests/unit/test__addons.py
 tests/unit/test_base.py
 tests/unit/test_demos.py
 tests/unit/test_utils.py
 tests/unit/column_pairs/__init__.py
 tests/unit/column_pairs/test_base.py
 tests/unit/column_pairs/statistical/__init__.py
 tests/unit/column_pairs/statistical/test_contingency_similarity.py
```

### Comparing `sdmetrics-0.9.2.dev0/sdmetrics.egg-info/requires.txt` & `sdmetrics-0.9.3.dev0/sdmetrics.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/setup.cfg` & `sdmetrics-0.9.3.dev0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.2.dev0
+current_version = 0.9.3.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `sdmetrics-0.9.2.dev0/setup.py` & `sdmetrics-0.9.3.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,10 +121,10 @@
     name='sdmetrics',
     packages=find_packages(include=['sdmetrics', 'sdmetrics.*']),
     python_requires='>=3.7,<3.11',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/SDMetrics',
-    version='0.9.2.dev0',
+    version='0.9.3.dev0',
     zip_safe=False,
 )
```

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/column_pairs/statistical/test_kl_divergence.py` & `sdmetrics-0.9.3.dev0/tests/integration/column_pairs/statistical/test_kl_divergence.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/multi_table/test_multi_single_table.py` & `sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_multi_single_table.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/multi_table/test_multi_table.py` & `sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/multi_table/test_parent_child.py` & `sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_parent_child.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/multi_table/test_statistical_metrics.py` & `sdmetrics-0.9.3.dev0/tests/integration/multi_table/test_statistical_metrics.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/reports/multi_table/test_multi_table_quality_report.py` & `sdmetrics-0.9.3.dev0/tests/integration/reports/multi_table/test_multi_table_quality_report.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/reports/single_table/test_single_table_quality_report.py` & `sdmetrics-0.9.3.dev0/tests/integration/reports/single_table/test_single_table_quality_report.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/single_column/statistical/test_cstest.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_column/statistical/test_cstest.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/single_column/statistical/test_kscomplement.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_column/statistical/test_kscomplement.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/single_table/efficacy/test_binary.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_binary.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/single_table/efficacy/test_detection.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_detection.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/single_table/efficacy/test_multiclass.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_multiclass.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/single_table/efficacy/test_regression.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_table/efficacy/test_regression.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/single_table/privacy/test_privacy.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_table/privacy/test_privacy.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/single_table/test_gaussian_mixture.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_table/test_gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/single_table/test_single_table.py` & `sdmetrics-0.9.3.dev0/tests/integration/single_table/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/test_base.py` & `sdmetrics-0.9.3.dev0/tests/integration/test_base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/timeseries/efficacy/test_classification.py` & `sdmetrics-0.9.3.dev0/tests/integration/timeseries/efficacy/test_classification.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/integration/timeseries/test_timeseries.py` & `sdmetrics-0.9.3.dev0/tests/integration/timeseries/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/column_pairs/statistical/test_contingency_similarity.py` & `sdmetrics-0.9.3.dev0/tests/unit/column_pairs/statistical/test_contingency_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/column_pairs/statistical/test_correlation_similarity.py` & `sdmetrics-0.9.3.dev0/tests/unit/column_pairs/statistical/test_correlation_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/column_pairs/test_base.py` & `sdmetrics-0.9.3.dev0/tests/unit/column_pairs/test_base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/multi_table/statistical/test_cardinality_shape_similarity.py` & `sdmetrics-0.9.3.dev0/tests/unit/multi_table/statistical/test_cardinality_shape_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/multi_table/statistical/test_cardinality_statistic_similarity.py` & `sdmetrics-0.9.3.dev0/tests/unit/multi_table/statistical/test_cardinality_statistic_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/multi_table/test_multi_single_table.py` & `sdmetrics-0.9.3.dev0/tests/unit/multi_table/test_multi_single_table.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/reports/multi_table/test_multi_table_diagnostic_report.py` & `sdmetrics-0.9.3.dev0/tests/unit/reports/multi_table/test_multi_table_diagnostic_report.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,20 +22,20 @@
         assert report._metric_results == {}
         assert report._metric_averages == {}
         assert report._results == {}
 
     def test_generate(self):
         """Test that the ``generate`` method calls the expected multi-table metrics."""
         # Setup
-        real_data = pd.DataFrame({
-            'table1': {'col1': [1, 2, 3], 'col2': ['a', 'b', 'c']},
-        })
-        synthetic_data = pd.DataFrame({
-            'table1': {'col1': [2, 2, 3], 'col2': ['b', 'a', 'c']},
-        })
+        real_data = {
+            'table1': pd.DataFrame({'col1': [1, 2, 3], 'col2': ['a', 'b', 'c']}),
+        }
+        synthetic_data = {
+            'table1': pd.DataFrame({'col1': [2, 2, 3], 'col2': ['b', 'a', 'c']}),
+        }
         metadata = {
             'tables': {
                 'table1': {
                     'fields': {'col1': {'type': 'numerical'}, 'col2': {'type': 'categorical'}},
                 },
             },
         }
@@ -88,33 +88,33 @@
 
         # Assert
         range_coverage.compute_breakdown.assert_called_once_with(
             real_data, synthetic_data, metadata)
         category_coverage.compute_breakdown.assert_called_once_with(
             real_data, synthetic_data, metadata)
         new_row_synth.compute_breakdown.assert_called_once_with(
-            real_data, synthetic_data, metadata, synthetic_sample_size=2)
+            real_data, synthetic_data, metadata, synthetic_sample_size=10000)
         boundary_adherence.compute_breakdown.assert_called_once_with(
             real_data, synthetic_data, metadata)
         assert report._metric_averages == {
             'RangeCoverage': 0.15000000000000002,
             'CategoryCoverage': 0.15000000000000002,
             'NewRowSynthesis': 0.1,
             'BoundaryAdherence': 0.15000000000000002,
         }
 
     def test_generate_verbose_false(self):
         """Test the ``generate`` method on silent mode. Expect that nothing is printed."""
         # Setup
-        real_data = pd.DataFrame({
-            'table1': {'col1': [1, 2, 3], 'col2': ['a', 'b', 'c']},
-        })
-        synthetic_data = pd.DataFrame({
-            'table1': {'col1': [2, 2, 3], 'col2': ['b', 'a', 'c']},
-        })
+        real_data = {
+            'table1': pd.DataFrame({'col1': [1, 2, 3], 'col2': ['a', 'b', 'c']}),
+        }
+        synthetic_data = {
+            'table1': pd.DataFrame({'col1': [2, 2, 3], 'col2': ['b', 'a', 'c']}),
+        }
         metadata = {
             'tables': {
                 'table1': {
                     'fields': {'col1': {'type': 'numerical'}, 'col2': {'type': 'categorical'}},
                 },
             },
         }
@@ -168,15 +168,15 @@
 
         # Assert
         range_coverage.compute_breakdown.assert_called_once_with(
             real_data, synthetic_data, metadata)
         category_coverage.compute_breakdown.assert_called_once_with(
             real_data, synthetic_data, metadata)
         new_row_synth.compute_breakdown.assert_called_once_with(
-            real_data, synthetic_data, metadata, synthetic_sample_size=2)
+            real_data, synthetic_data, metadata, synthetic_sample_size=10000)
         boundary_adherence.compute_breakdown.assert_called_once_with(
             real_data, synthetic_data, metadata)
         assert report._metric_averages == {
             'RangeCoverage': 0.15000000000000002,
             'CategoryCoverage': 0.15000000000000002,
             'NewRowSynthesis': 0.1,
             'BoundaryAdherence': 0.15000000000000002,
@@ -186,20 +186,20 @@
     def test_generate_with_errored_metric(self):
         """Test the ``generate`` method when a metric has an error.
 
         Expect that the multi-table metrics are called. Expect that the results are computed
         without the error-ed out metric.
         """
         # Setup
-        real_data = pd.DataFrame({
-            'table1': {'col1': [1, 2, 3], 'col2': ['a', 'b', 'c']},
-        })
-        synthetic_data = pd.DataFrame({
-            'table1': {'col1': [2, 2, 3], 'col2': ['b', 'a', 'c']}
-        })
+        real_data = {
+            'table1': pd.DataFrame({'col1': [1, 2, 3], 'col2': ['a', 'b', 'c']}),
+        }
+        synthetic_data = {
+            'table1': pd.DataFrame({'col1': [2, 2, 3], 'col2': ['b', 'a', 'c']})
+        }
         range_coverage = Mock()
         range_coverage.__name__ = 'RangeCoverage'
         range_coverage.compute_breakdown.return_value = {
             'table1': {
                 'col1': {'score': 0.1},
                 'col2': {'score': 0.2},
             },
@@ -252,30 +252,30 @@
 
         # Assert
         range_coverage.compute_breakdown.assert_called_once_with(
             real_data, synthetic_data, metadata)
         category_coverage.compute_breakdown.assert_called_once_with(
             real_data, synthetic_data, metadata)
         new_row_synth.compute_breakdown.assert_called_once_with(
-            real_data, synthetic_data, metadata, synthetic_sample_size=2)
+            real_data, synthetic_data, metadata, synthetic_sample_size=10000)
         boundary_adherence.compute_breakdown.assert_called_once_with(
             real_data, synthetic_data, metadata)
 
     def test_generate_with_incomputable_metric_error(self):
         """Test the ``generate`` method when a metric throws an error.
 
         Expect that the error is caught and the metric score is set to None.
         """
         # Setup
-        real_data = pd.DataFrame({
-            'table1': {'col1': [1, 2, 3], 'col2': ['a', 'b', 'c']},
-        })
-        synthetic_data = pd.DataFrame({
-            'table1': {'col1': [2, 2, 3], 'col2': ['b', 'a', 'c']}
-        })
+        real_data = {
+            'table1': pd.DataFrame({'col1': [1, 2, 3], 'col2': ['a', 'b', 'c']}),
+        }
+        synthetic_data = {
+            'table1': pd.DataFrame({'col1': [2, 2, 3], 'col2': ['b', 'a', 'c']})
+        }
         range_coverage = Mock()
         range_coverage.__name__ = 'RangeCoverage'
         range_coverage.compute_breakdown.return_value = {
             'table1': {
                 'col1': {'score': 0.1},
                 'col2': {'score': 0.2},
             },
@@ -326,15 +326,15 @@
 
         # Assert
         range_coverage.compute_breakdown.assert_called_once_with(
             real_data, synthetic_data, metadata)
         category_coverage.compute_breakdown.assert_called_once_with(
             real_data, synthetic_data, metadata)
         new_row_synth.compute_breakdown.assert_called_once_with(
-            real_data, synthetic_data, metadata, synthetic_sample_size=2)
+            real_data, synthetic_data, metadata, synthetic_sample_size=10000)
         boundary_adherence.compute_breakdown.assert_called_once_with(
             real_data, synthetic_data, metadata)
         assert np.isnan(report._property_scores['Synthesis'])
 
     def test_get_results(self):
         """Test that the ``get_results`` method returns the overall diagnostic results."""
         # Setup
```

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/reports/multi_table/test_multi_table_plot_utils.py` & `sdmetrics-0.9.3.dev0/tests/unit/reports/multi_table/test_multi_table_plot_utils.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/reports/multi_table/test_multi_table_quality_report.py` & `sdmetrics-0.9.3.dev0/tests/unit/reports/multi_table/test_multi_table_quality_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,22 @@
         }
         synthetic_data = {
             'table1': pd.DataFrame({'col1': [1, 3, 3], 'col2': ['b', 'b', 'c']}),
             'table2': pd.DataFrame({'col1': [3, 1, 3]}),
         }
         metadata = {
             'tables': {
-                'table1': {'col1': {'type': 'numerical'}, 'col2': {'type': 'categorical'}},
-                'table2': {'col1': {'type': 'numerical'}},
+                'table1': {
+                    'fields': {'col1': {'type': 'numerical'}, 'col2': {'type': 'categorical'}}
+                },
+                'table2': {
+                    'fields': {'col1': {'type': 'numerical'}}
+                },
             },
         }
-
         ks_complement_mock = Mock()
         ks_complement_mock.__name__ = 'KSComplement'
         ks_complement_mock.compute_breakdown.return_value = {
             'table1': {
                 'col1': {'score': 0.1},
                 'col2': {'score': 0.2},
             }
@@ -148,16 +151,20 @@
         }
         synthetic_data = {
             'table1': pd.DataFrame({'col1': [1, 3, 3], 'col2': ['b', 'b', 'c']}),
             'table2': pd.DataFrame({'col1': [3, 1, 3]}),
         }
         metadata = {
             'tables': {
-                'table1': {'col1': {'type': 'numerical'}, 'col2': {'type': 'categorical'}},
-                'table2': {'col1': {'type': 'numerical'}},
+                'table1': {
+                    'fields': {'col1': {'type': 'numerical'}, 'col2': {'type': 'categorical'}}
+                },
+                'table2': {
+                    'fields': {'col1': {'type': 'numerical'}}
+                },
             },
         }
 
         ks_complement_mock = Mock()
         ks_complement_mock.__name__ = 'KSComplement'
         ks_complement_mock.compute_breakdown.return_value = {
             'table1': {
@@ -262,16 +269,20 @@
         }
         synthetic_data = {
             'table1': pd.DataFrame({'col1': [1, 3, 3], 'col2': ['b', 'b', 'c']}),
             'table2': pd.DataFrame({'col1': [3, 1, 3]}),
         }
         metadata = {
             'tables': {
-                'table1': {'col1': {'type': 'numerical'}, 'col2': {'type': 'categorical'}},
-                'table2': {'col1': {'type': 'numerical'}},
+                'table1': {
+                    'fields': {'col1': {'type': 'numerical'}, 'col2': {'type': 'categorical'}}
+                },
+                'table2': {
+                    'fields': {'col1': {'type': 'numerical'}}
+                },
             },
         }
 
         ks_complement_mock = Mock()
         ks_complement_mock.__name__ = 'KSComplement'
         ks_complement_mock.compute_breakdown.return_value = {
             'table1': {
@@ -379,16 +390,20 @@
         }
         synthetic_data = {
             'table1': pd.DataFrame({'col1': [1, 3, 3], 'col2': ['b', 'b', 'c']}),
             'table2': pd.DataFrame({'col1': [3, 1, 3]}),
         }
         metadata = {
             'tables': {
-                'table1': {'col1': {'type': 'numerical'}, 'col2': {'type': 'categorical'}},
-                'table2': {'col1': {'type': 'numerical'}},
+                'table1': {
+                    'fields': {'col1': {'type': 'numerical'}, 'col2': {'type': 'categorical'}}
+                },
+                'table2': {
+                    'fields': {'col1': {'type': 'numerical'}}
+                },
             },
         }
 
         ks_complement_mock = Mock()
         ks_complement_mock.__name__ = 'KSComplement'
         ks_complement_mock.compute_breakdown.return_value = {
             'table1': {
@@ -488,16 +503,20 @@
         }
         synthetic_data = {
             'table1': pd.DataFrame({'col1': [1, 3, 3], 'col2': ['b', 'b', 'c']}),
             'table2': pd.DataFrame({'col1': [3, 1, 3]}),
         }
         metadata = {
             'tables': {
-                'table1': {'col1': {'type': 'numerical'}, 'col2': {'type': 'categorical'}},
-                'table2': {'col1': {'type': 'numerical'}},
+                'table1': {
+                    'fields': {'col1': {'type': 'numerical'}, 'col2': {'type': 'categorical'}}
+                },
+                'table2': {
+                    'fields': {'col1': {'type': 'numerical'}}
+                },
             },
         }
 
         ks_complement_mock = Mock()
         ks_complement_mock.__name__ = 'KSComplement'
         ks_complement_mock.compute_breakdown.return_value = {
             'table1': {
```

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/reports/single_table/test_single_table_diagnostic_report.py` & `sdmetrics-0.9.3.dev0/tests/unit/reports/single_table/test_single_table_diagnostic_report.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/reports/single_table/test_single_table_plot_utils.py` & `sdmetrics-0.9.3.dev0/tests/unit/reports/single_table/test_single_table_plot_utils.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/reports/single_table/test_single_table_quality_report.py` & `sdmetrics-0.9.3.dev0/tests/unit/reports/single_table/test_single_table_quality_report.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/reports/test_utils.py` & `sdmetrics-0.9.3.dev0/tests/unit/reports/test_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import re
+import warnings
 from datetime import date, datetime
 from unittest.mock import Mock, call, patch
 
 import pandas as pd
 import pytest
 
 from sdmetrics.reports.utils import (
-    aggregate_metric_results, convert_to_datetime, discretize_and_apply_metric,
-    discretize_table_data, get_column_pair_plot, get_column_plot, make_continuous_column_pair_plot,
-    make_continuous_column_plot, make_discrete_column_pair_plot, make_discrete_column_plot,
-    make_mixed_column_pair_plot)
+    _validate_categorical_values, aggregate_metric_results, convert_to_datetime,
+    discretize_and_apply_metric, discretize_table_data, get_column_pair_plot, get_column_plot,
+    make_continuous_column_pair_plot, make_continuous_column_plot, make_discrete_column_pair_plot,
+    make_discrete_column_plot, make_mixed_column_pair_plot, validate_multi_table_inputs,
+    validate_single_table_inputs)
 from tests.utils import DataFrameMatcher, SeriesMatcher
 
 
 @patch('sdmetrics.reports.utils.ff')
 def test_make_continuous_column_plot(ff_mock):
     """Test the ``make_continuous_column_plot`` method.
 
@@ -1185,7 +1187,168 @@
 
     # Run
     avg_score, num_errors = aggregate_metric_results(metric_results)
 
     # Assert
     assert avg_score == 0.45
     assert num_errors == 1
+
+
+def test__validate_categorical_values():
+    """Test no extra categoricals does not crash."""
+    # Setup
+    sdtype = 'categorical'
+    real_data = pd.DataFrame({'col1': [1, 2, 3, 4]})
+    synthetic_data = pd.DataFrame({'col1': [1, 2, 4, 4]})
+    metadata = {'fields': {'col1': {'type': sdtype}}}
+    warnings.filterwarnings('error', category=UserWarning)
+
+    # Run
+    _validate_categorical_values(real_data, synthetic_data, metadata)
+
+    warnings.resetwarnings()
+
+
+def test__validate_categorical_values_single_table():
+    """Test validating categoricals for single table."""
+    # Setup
+    sdtype = 'categorical'
+    real_data = pd.DataFrame({'col1': [1, 2, 3, 3]})
+    synthetic_data = pd.DataFrame({'col1': [1, 2, 4, 5]})
+    metadata = {'fields': {'col1': {'type': sdtype}}}
+    warning_msg = re.escape('Unexpected values ("4", "5") in column "col1"')
+
+    warnings.filterwarnings('error', category=UserWarning)
+
+    # Run
+    with pytest.raises(UserWarning, match=warning_msg):
+        _validate_categorical_values(real_data, synthetic_data, metadata)
+
+    warnings.resetwarnings()
+
+
+def test__validate_categorical_values_multi_table():
+    """Test validating categoricals with table name."""
+    # Setup
+    sdtype = 'categorical'
+    real_data = pd.DataFrame({'col1': [1, 2, 3, 3]})
+    synthetic_data = pd.DataFrame({'col1': [1, 2, 4, 5]})
+    metadata = {'fields': {'col1': {'type': sdtype}}}
+    warning_msg = re.escape('Unexpected values ("4", "5") in column "col1" and table "table1"')
+
+    warnings.filterwarnings('error', category=UserWarning)
+
+    # Run
+    with pytest.raises(UserWarning, match=warning_msg):
+        _validate_categorical_values(real_data, synthetic_data, metadata, table='table1')
+
+    warnings.resetwarnings()
+
+
+def test__validate_categorical_many_extra_values():
+    """Test validating categoricals with table name."""
+    # Setup
+    sdtype = 'categorical'
+    real_data = pd.DataFrame({'col1': [1, 2, 3, 3, 4, 4]})
+    synthetic_data = pd.DataFrame({'col1': ['a', 'b', 'c', 'd', 'e', 'f']})
+    metadata = {'fields': {'col1': {'type': sdtype}}}
+    warning_msg = re.escape('Unexpected values ("a", "b", "c", "d", "e" + more) in column "col1"')
+
+    warnings.filterwarnings('error', category=UserWarning)
+
+    # Run
+    with pytest.raises(UserWarning, match=warning_msg):
+        _validate_categorical_values(real_data, synthetic_data, metadata)
+
+    warnings.resetwarnings()
+
+
+def test_validate_single_table():
+    """Test validating single table."""
+    # Setup
+    sdtype = 'categorical'
+    real_data = pd.DataFrame({'col1': [1, 2, 3, 4]})
+    synthetic_data = pd.DataFrame({'col1': [1, 1, 1, 3]})
+    extra_value_synthtetic_data = pd.DataFrame({'col1': [1, 1, 1, 5]})
+    metadata = {'fields': {'col1': {'type': sdtype}}}
+
+    warning_msg = re.escape('Unexpected values ("5") in column "col1"')
+    warnings.filterwarnings('error', category=UserWarning)
+
+    # Run
+    validate_single_table_inputs(real_data, synthetic_data, metadata)
+
+    with pytest.raises(UserWarning, match=warning_msg):
+        validate_single_table_inputs(real_data, extra_value_synthtetic_data, metadata)
+
+    warnings.resetwarnings()
+
+
+def test_validate_multi_table():
+    """Test validating categoricals for single table."""
+    # Setup
+    sdtype = 'categorical'
+    real_data = {
+        'table1': pd.DataFrame({'col1': [1, 2, 3, 3]}),
+        'table2': pd.DataFrame({'col2': ['a', 'b', 'c', 'a']})
+    }
+    synthetic_data = {
+        'table1': pd.DataFrame({'col1': [1, 2, 3, 1]}),
+        'table2': pd.DataFrame({'col2': ['a', 'b', 'c', 'c']})
+    }
+    extra_value_synthetic_data = {
+        'table1': pd.DataFrame({'col1': [1, 2, 3, 1]}),
+        'table2': pd.DataFrame({'col2': ['a', 'b', 'c', 'd']})
+    }
+    metadata = {
+        'tables': {
+            'table1': {'fields': {'col1': {'type': sdtype}}},
+            'table2': {'fields': {'col2': {'type': sdtype}}}
+        }
+    }
+    warning_msg = re.escape('Unexpected values ("d") in column "col2" and table "table2"')
+
+    warnings.filterwarnings('error', category=UserWarning)
+
+    # Run
+    validate_multi_table_inputs(real_data, synthetic_data, metadata)
+    with pytest.raises(UserWarning, match=warning_msg):
+        validate_multi_table_inputs(real_data, extra_value_synthetic_data, metadata)
+
+    warnings.resetwarnings()
+
+
+def test_validate_multi_table_parent_child_dtype_mismatch():
+    """Test validating categoricals for single table."""
+    # Setup
+    sdtype = 'numerical'
+    real_data = {
+        'table1': pd.DataFrame({'primary_key': [1, 2, 3, 4]}),
+        'table2': pd.DataFrame({'foreign_key': ['1', '2', '2', '3']})
+    }
+    synthetic_data = {
+        'table1': pd.DataFrame({'primary_key': [1, 2, 3, 1]}),
+        'table2': pd.DataFrame({'foreign_key': ['2', '2', '1', '3']})
+    }
+    metadata = {
+        'tables': {
+            'table1': {'fields': {'primary_key': {'type': sdtype}}},
+            'table2': {'fields': {'foreign_key': {'type': sdtype}}}
+        },
+        'relationships': [
+            {
+                'parent_table_name': 'table1',
+                'child_table_name': 'table2',
+                'parent_primary_key': 'primary_key',
+                'child_foreign_key': 'foreign_key'
+            }
+        ]
+    }
+    error_msg = re.escape(
+        "The 'table1' table and 'table2' table cannot be merged. Please make sure the primary key "
+        "in 'table1' ('primary_key') and the foreign key in 'table2' ('foreign_key') have the same"
+        ' data type.'
+    )
+
+    # Run and Assert
+    with pytest.raises(ValueError, match=error_msg):
+        validate_multi_table_inputs(real_data, synthetic_data, metadata)
```

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/single_column/statistical/test_boundary_adherence.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_boundary_adherence.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/single_column/statistical/test_category_coverage.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_category_coverage.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/single_column/statistical/test_missing_value_similarity.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_missing_value_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/single_column/statistical/test_range_coverage.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_range_coverage.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/single_column/statistical/test_statistic_similarity.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_statistic_similarity.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/single_column/statistical/test_tv_complement.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_column/statistical/test_tv_complement.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/single_column/test_base.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_column/test_base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/single_table/detection/test_detection.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_table/detection/test_detection.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/single_table/privacy/test_util.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_table/privacy/test_util.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/single_table/test_base.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_table/test_base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/single_table/test_multi_single_column.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_table/test_multi_single_column.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/single_table/test_new_row_synthesis.py` & `sdmetrics-0.9.3.dev0/tests/unit/single_table/test_new_row_synthesis.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/test_base.py` & `sdmetrics-0.9.3.dev0/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/test_demos.py` & `sdmetrics-0.9.3.dev0/tests/unit/test_demos.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/unit/test_utils.py` & `sdmetrics-0.9.3.dev0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdmetrics-0.9.2.dev0/tests/utils.py` & `sdmetrics-0.9.3.dev0/tests/utils.py`

 * *Files identical despite different names*

