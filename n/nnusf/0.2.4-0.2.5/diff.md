# Comparing `tmp/nnusf-0.2.4.tar.gz` & `tmp/nnusf-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnusf-0.2.4.tar", max compression
+gzip compressed data, was "nnusf-0.2.5.tar", max compression
```

## Comparing `nnusf-0.2.4.tar` & `nnusf-0.2.5.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0    35149 2023-02-27 21:57:05.697499 nnusf-0.2.4/LICENSE
--rw-r--r--   0        0        0     2606 2023-02-27 21:57:05.697499 nnusf-0.2.4/README.md
--rw-r--r--   0        0        0     2282 2023-02-27 21:58:21.249022 nnusf-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       46 2023-02-27 21:58:21.249022 nnusf-0.2.4/src/nnusf/__init__.py
--rw-r--r--   0        0        0      133 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/cli/__init__.py
--rw-r--r--   0        0        0      172 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/cli/base.py
--rw-r--r--   0        0        0     4109 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/cli/data.py
--rw-r--r--   0        0        0     2082 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/cli/extra.py
--rw-r--r--   0        0        0     3414 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/cli/fit.py
--rw-r--r--   0        0        0      201 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/cli/log.py
--rw-r--r--   0        0        0     5284 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/cli/plot.py
--rw-r--r--   0        0        0      879 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/cli/report.py
--rw-r--r--   0        0        0     6815 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/cli/theory.py
--rw-r--r--   0        0        0      277 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/data/__init__.py
--rw-r--r--   0        0        0     2989 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/data/coefficients.py
--rw-r--r--   0        0        0     1002 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/data/combine_tables.py
--rw-r--r--   0        0        0     1439 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/data/filters.py
--rw-r--r--   0        0        0     6470 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/data/loader.py
--rw-r--r--   0        0        0     9416 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/data/matching_grids.py
--rw-r--r--   0        0        0    13188 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/data/utils.py
--rw-r--r--   0        0        0        0 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/export_lhapdf/__init__.py
--rw-r--r--   0        0        0     6001 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/export_lhapdf/dump_grids.py
--rw-r--r--   0        0        0     9503 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/export_lhapdf/utils.py
--rwxr-xr-x   0        0        0     6128 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/filters/filter_bebcwa59.py
--rwxr-xr-x   0        0        0     6675 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/filters/filter_ccfr.py
--rwxr-xr-x   0        0        0    17661 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/filters/filter_cdhsw.py
--rwxr-xr-x   0        0        0    10365 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/filters/filter_charm.py
--rwxr-xr-x   0        0        0    11707 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/filters/filter_chorus.py
--rwxr-xr-x   0        0        0     9449 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/filters/filter_nutev.py
--rw-r--r--   0        0        0      104 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/get/__init__.py
--rw-r--r--   0        0        0      172 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/get/base.py
--rw-r--r--   0        0        0      698 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/get/gettheory.py
--rw-r--r--   0        0        0      201 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/get/log.py
--rw-r--r--   0        0        0        0 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/plot/__init__.py
--rw-r--r--   0        0        0     7303 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/plot/covmat.py
--rw-r--r--   0        0        0    16374 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/plot/fit.py
--rw-r--r--   0        0        0     4344 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/plot/kinematics.py
--rw-r--r--   0        0        0     3559 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/plot/matching.py
--rw-r--r--   0        0        0     2952 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/plot/sf.py
--rw-r--r--   0        0        0     6132 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/plot/th_covmat.py
--rw-r--r--   0        0        0     4291 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/plot/utils.py
--rw-r--r--   0        0        0     1384 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/plotstyle.mplstyle
--rw-r--r--   0        0        0        0 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/reports/__init__.py
--rw-r--r--   0        0        0     7125 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/reports/assets/index.html
--rwxr-xr-x   0        0        0    68365 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/reports/assets/report.css
--rw-r--r--   0        0        0     9969 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/reports/genfiles.py
--rw-r--r--   0        0        0     5641 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/reports/genhtml.py
--rw-r--r--   0        0        0        0 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/scripts/__init__.py
--rw-r--r--   0        0        0     2370 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/scripts/gettheory.py
--rw-r--r--   0        0        0     1369 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/scripts/integrate.py
--rw-r--r--   0        0        0     3329 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/scripts/isoscalar.py
--rw-r--r--   0        0        0        0 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/sffit/__init__.py
--rw-r--r--   0        0        0     5283 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/sffit/callbacks.py
--rw-r--r--   0        0        0     4147 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/sffit/check_gls.py
--rw-r--r--   0        0        0     3339 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/sffit/compute_expchi2.py
--rw-r--r--   0        0        0     2957 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/sffit/layers.py
--rw-r--r--   0        0        0     3926 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/sffit/load_data.py
--rw-r--r--   0        0        0     4238 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/sffit/load_fit_data.py
--rw-r--r--   0        0        0     5351 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/sffit/model_gen.py
--rw-r--r--   0        0        0     2603 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/sffit/postfit.py
--rw-r--r--   0        0        0     3120 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/sffit/run_sffit.py
--rw-r--r--   0        0        0     2241 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/sffit/scaling.py
--rw-r--r--   0        0        0     2728 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/sffit/train_model.py
--rw-r--r--   0        0        0     8001 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/sffit/utils.py
--rw-r--r--   0        0        0        0 2023-02-27 21:57:05.809498 nnusf-0.2.4/src/nnusf/theory/__init__.py
--rw-r--r--   0        0        0  1626320 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/assets/genie.hdf5
--rw-r--r--   0        0        0      649 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/assets/theory_nnusf.yaml
--rw-r--r--   0        0        0     1245 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/bodek_yang/__init__.py
--rw-r--r--   0        0        0      157 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/bodek_yang/cuts.py
--rw-r--r--   0        0        0     1532 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/bodek_yang/load.py
--rw-r--r--   0        0        0      800 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/bodek_yang/runcards.py
--rw-r--r--   0        0        0     4209 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/compare_to_data.py
--rw-r--r--   0        0        0       47 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/data_vs_theory/__init__.py
--rw-r--r--   0        0        0      646 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/data_vs_theory/runcards.py
--rw-r--r--   0        0        0      885 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/defs.py
--rw-r--r--   0        0        0     1991 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/grids.py
--rw-r--r--   0        0        0       47 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/highq/__init__.py
--rw-r--r--   0        0        0     1377 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/highq/load.py
--rw-r--r--   0        0        0     3960 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/highq/runcards.py
--rw-r--r--   0        0        0    12184 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/predictions.py
--rw-r--r--   0        0        0     5969 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/runcards.py
--rw-r--r--   0        0        0       47 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/yadknots/__init__.py
--rw-r--r--   0        0        0     1187 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/theory/yadknots/runcards.py
--rw-r--r--   0        0        0     6366 2023-02-27 21:57:05.821498 nnusf-0.2.4/src/nnusf/utils.py
--rw-r--r--   0        0        0     1610 2023-02-27 21:57:05.821498 nnusf-0.2.4/tests/test_loader.py
--rw-r--r--   0        0        0      156 2023-02-27 21:57:05.825498 nnusf-0.2.4/tests/theory/test_bodek_yang.py
--rw-r--r--   0        0        0     4252 1970-01-01 00:00:00.000000 nnusf-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 21:01:32.595940 nnusf-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2606 2023-04-11 21:01:32.595940 nnusf-0.2.5/README.md
+-rw-r--r--   0        0        0     2282 2023-04-11 21:03:21.526487 nnusf-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-04-11 21:03:21.530488 nnusf-0.2.5/src/nnusf/__init__.py
+-rw-r--r--   0        0        0      133 2023-04-11 21:01:32.719948 nnusf-0.2.5/src/nnusf/cli/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-11 21:01:32.719948 nnusf-0.2.5/src/nnusf/cli/base.py
+-rw-r--r--   0        0        0     4109 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/cli/data.py
+-rw-r--r--   0        0        0     2082 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/cli/extra.py
+-rw-r--r--   0        0        0     3407 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/cli/fit.py
+-rw-r--r--   0        0        0      201 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/cli/log.py
+-rw-r--r--   0        0        0     5284 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/cli/plot.py
+-rw-r--r--   0        0        0      879 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/cli/report.py
+-rw-r--r--   0        0        0     6815 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/cli/theory.py
+-rw-r--r--   0        0        0      277 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/data/__init__.py
+-rw-r--r--   0        0        0     2989 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/data/coefficients.py
+-rw-r--r--   0        0        0     1002 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/data/combine_tables.py
+-rw-r--r--   0        0        0     1439 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/data/filters.py
+-rw-r--r--   0        0        0     6470 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/data/loader.py
+-rw-r--r--   0        0        0     9416 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/data/matching_grids.py
+-rw-r--r--   0        0        0    13188 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/data/utils.py
+-rwxr-xr-x   0        0        0     6128 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/filters/filter_bebcwa59.py
+-rwxr-xr-x   0        0        0     6675 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/filters/filter_ccfr.py
+-rwxr-xr-x   0        0        0    17661 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/filters/filter_cdhsw.py
+-rwxr-xr-x   0        0        0    10365 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/filters/filter_charm.py
+-rwxr-xr-x   0        0        0    11707 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/filters/filter_chorus.py
+-rwxr-xr-x   0        0        0     9449 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/filters/filter_nutev.py
+-rw-r--r--   0        0        0      104 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/get/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/get/base.py
+-rw-r--r--   0        0        0      698 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/get/gettheory.py
+-rw-r--r--   0        0        0      201 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/get/log.py
+-rw-r--r--   0        0        0        0 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/lhapdf/__init__.py
+-rw-r--r--   0        0        0     6001 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/lhapdf/dump_grids.py
+-rw-r--r--   0        0        0     9503 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/lhapdf/utils.py
+-rw-r--r--   0        0        0        0 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/__init__.py
+-rw-r--r--   0        0        0     7303 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/covmat.py
+-rw-r--r--   0        0        0    17946 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/fit.py
+-rw-r--r--   0        0        0     4344 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/kinematics.py
+-rw-r--r--   0        0        0     3559 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/matching.py
+-rw-r--r--   0        0        0     2952 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/sf.py
+-rw-r--r--   0        0        0     6132 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/th_covmat.py
+-rw-r--r--   0        0        0     7191 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plot/utils.py
+-rw-r--r--   0        0        0     1384 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/plotstyle.mplstyle
+-rw-r--r--   0        0        0        0 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/reports/__init__.py
+-rw-r--r--   0        0        0     7125 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/reports/assets/index.html
+-rwxr-xr-x   0        0        0    68365 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/reports/assets/report.css
+-rw-r--r--   0        0        0     9969 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/reports/genfiles.py
+-rw-r--r--   0        0        0     5641 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/reports/genhtml.py
+-rw-r--r--   0        0        0        0 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/scripts/__init__.py
+-rw-r--r--   0        0        0     2370 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/scripts/gettheory.py
+-rw-r--r--   0        0        0     1369 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/scripts/integrate.py
+-rw-r--r--   0        0        0     3315 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/scripts/isoscalar.py
+-rw-r--r--   0        0        0        0 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/__init__.py
+-rw-r--r--   0        0        0     5283 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/callbacks.py
+-rw-r--r--   0        0        0     3339 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/compute_expchi2.py
+-rw-r--r--   0        0        0     2957 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/layers.py
+-rw-r--r--   0        0        0     3926 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/load_data.py
+-rw-r--r--   0        0        0     4238 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/load_fit_data.py
+-rw-r--r--   0        0        0     5351 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/model_gen.py
+-rw-r--r--   0        0        0     2603 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/postfit.py
+-rw-r--r--   0        0        0     3120 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/run_sffit.py
+-rw-r--r--   0        0        0     2241 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/scaling.py
+-rw-r--r--   0        0        0    11423 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/sum_rules.py
+-rw-r--r--   0        0        0     2728 2023-04-11 21:01:32.723948 nnusf-0.2.5/src/nnusf/sffit/train_model.py
+-rw-r--r--   0        0        0     8001 2023-04-11 21:01:32.727949 nnusf-0.2.5/src/nnusf/sffit/utils.py
+-rw-r--r--   0        0        0        0 2023-04-11 21:01:32.727949 nnusf-0.2.5/src/nnusf/theory/__init__.py
+-rw-r--r--   0        0        0  1626320 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/assets/genie.hdf5
+-rw-r--r--   0        0        0      649 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/assets/theory_nnusf.yaml
+-rw-r--r--   0        0        0     1245 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/bodek_yang/__init__.py
+-rw-r--r--   0        0        0      157 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/bodek_yang/cuts.py
+-rw-r--r--   0        0        0     1532 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/bodek_yang/load.py
+-rw-r--r--   0        0        0      800 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/bodek_yang/runcards.py
+-rw-r--r--   0        0        0     4209 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/compare_to_data.py
+-rw-r--r--   0        0        0       47 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/data_vs_theory/__init__.py
+-rw-r--r--   0        0        0      646 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/data_vs_theory/runcards.py
+-rw-r--r--   0        0        0      885 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/defs.py
+-rw-r--r--   0        0        0     1991 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/grids.py
+-rw-r--r--   0        0        0       47 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/highq/__init__.py
+-rw-r--r--   0        0        0     1377 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/highq/load.py
+-rw-r--r--   0        0        0     3960 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/highq/runcards.py
+-rw-r--r--   0        0        0    12073 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/predictions.py
+-rw-r--r--   0        0        0     5969 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/runcards.py
+-rw-r--r--   0        0        0       47 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/yadknots/__init__.py
+-rw-r--r--   0        0        0     1187 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/theory/yadknots/runcards.py
+-rw-r--r--   0        0        0     6366 2023-04-11 21:01:32.739949 nnusf-0.2.5/src/nnusf/utils.py
+-rw-r--r--   0        0        0     1610 2023-04-11 21:01:32.739949 nnusf-0.2.5/tests/test_loader.py
+-rw-r--r--   0        0        0      156 2023-04-11 21:01:32.739949 nnusf-0.2.5/tests/theory/test_bodek_yang.py
+-rw-r--r--   0        0        0     4252 1970-01-01 00:00:00.000000 nnusf-0.2.5/PKG-INFO
```

### Comparing `nnusf-0.2.4/LICENSE` & `nnusf-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/README.md` & `nnusf-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/pyproject.toml` & `nnusf-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nnusf"
-version = "0.2.4"
+version = "0.2.5"
 description = "Predictions for all-energy neutrino structure functions"
 readme = "README.md"
 authors = [
   "Alessandro Candido <candido.ale@gmail.com>",
   "Alfonso Garcia <pochoarus@msn.com>",
   "Giacomo Magni <giac.magni@gmail.com>",
   "Tanjona R. Rabemananjara <tanjona.lspc@gmail.com>",
```

### Comparing `nnusf-0.2.4/src/nnusf/cli/data.py` & `nnusf-0.2.5/src/nnusf/cli/data.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/cli/extra.py` & `nnusf-0.2.5/src/nnusf/cli/extra.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/cli/fit.py` & `nnusf-0.2.5/src/nnusf/cli/fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import pathlib
 
 import click
 
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 
-from ..export_lhapdf import dump_grids
+from ..lhapdf import dump_grids
 from ..sffit import postfit, run_sffit
 from . import base
 
 
 @base.command.group("fit")
 def subcommand():
     """Fit structure functions."""
```

### Comparing `nnusf-0.2.4/src/nnusf/cli/plot.py` & `nnusf-0.2.5/src/nnusf/cli/plot.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/cli/report.py` & `nnusf-0.2.5/src/nnusf/cli/report.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/cli/theory.py` & `nnusf-0.2.5/src/nnusf/cli/theory.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/data/coefficients.py` & `nnusf-0.2.5/src/nnusf/data/coefficients.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/data/combine_tables.py` & `nnusf-0.2.5/src/nnusf/data/combine_tables.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/data/filters.py` & `nnusf-0.2.5/src/nnusf/data/filters.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/data/loader.py` & `nnusf-0.2.5/src/nnusf/data/loader.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/data/matching_grids.py` & `nnusf-0.2.5/src/nnusf/data/matching_grids.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/data/utils.py` & `nnusf-0.2.5/src/nnusf/data/utils.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/export_lhapdf/dump_grids.py` & `nnusf-0.2.5/src/nnusf/lhapdf/dump_grids.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/export_lhapdf/utils.py` & `nnusf-0.2.5/src/nnusf/lhapdf/utils.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/filters/filter_bebcwa59.py` & `nnusf-0.2.5/src/nnusf/filters/filter_bebcwa59.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/filters/filter_ccfr.py` & `nnusf-0.2.5/src/nnusf/filters/filter_ccfr.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/filters/filter_cdhsw.py` & `nnusf-0.2.5/src/nnusf/filters/filter_cdhsw.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/filters/filter_charm.py` & `nnusf-0.2.5/src/nnusf/filters/filter_charm.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/filters/filter_chorus.py` & `nnusf-0.2.5/src/nnusf/filters/filter_chorus.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/filters/filter_nutev.py` & `nnusf-0.2.5/src/nnusf/filters/filter_nutev.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/get/gettheory.py` & `nnusf-0.2.5/src/nnusf/get/gettheory.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/plot/covmat.py` & `nnusf-0.2.5/src/nnusf/plot/covmat.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/plot/fit.py` & `nnusf-0.2.5/src/nnusf/plot/fit.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 
 import numpy as np
 import tensorflow as tf
 import yaml
 from matplotlib import pyplot as plt
 from matplotlib.figure import Figure
 
-from ..sffit.check_gls import check_gls_sumrules
+from ..sffit.sum_rules import check_sumrule, effective_charge
 from ..sffit.load_data import load_experimental_data
 from ..sffit.load_fit_data import get_predictions_q, load_models
-from .utils import plot_point_cov
+from .utils import plot_point_cov, format_jlab
 
 _logger = logging.getLogger(__name__)
 PARRENT_PATH = pathlib.Path(__file__).parents[1]
 MPLSTYLE = PARRENT_PATH.joinpath("plotstyle.mplstyle")
 plt.style.use(MPLSTYLE)
 
-basis = [
+EQ_LABELS = {"GLS": r"$F_3$", "Bjorken": r"$F_1$"}
+
+BASIS = [
     r"$F_2^\nu$",
     r"$F_L^\nu$",
     r"$xF_3^\nu$",
     r"$F_2^{\bar{\nu}}$",
     r"$F_L^{\bar{\nu}}$",
     r"$xF_3^{\bar{\nu}}$",
 ]
@@ -166,23 +168,23 @@
         ax.axvline(
             x=sf_dist.mean() - sf_dist.std(), lw=0.75, ls="--", color="C1"
         )
         ax.axvline(
             x=sf_dist.mean() + sf_dist.std(), lw=0.75, ls="--", color="C1"
         )
 
-        ax.text(0.88, 0.8, basis[index], size=16, transform=ax.transAxes)
+        ax.text(0.88, 0.8, BASIS[index], size=16, transform=ax.transAxes)
         if index >= 3:
             ax.set_xlabel(r"$\alpha$")
         if index == 0 or index == 3:
             ax.set_ylabel(r"$\rm{Frequency}$")
         if index == 0:
             ax.legend()
 
-    save_path = pathlib.Path(kwargs["output"]) / f"smallx_exponent"
+    save_path = pathlib.Path(kwargs["output"]) / "smallx_exponent"
     save_figs(fig, save_path, dpi=350)
 
 
 def training_epochs_distribution(**kwargs):
     fitinfo = pathlib.Path(kwargs["fit"]).glob("replica_*/fitinfo.json")
 
     tr_epochs = []
@@ -215,25 +217,25 @@
     ax.grid(color="grey", alpha=0.2, linewidth=0.5, zorder=0)
     ax.legend()
 
     save_path = pathlib.Path(kwargs["output"]) / "distr_epochs"
     save_figs(fig, save_path, dpi=350)
 
 
-def gls_sum_rules(**kwargs):
-    q2grids, gls_results, xf3avg_int = check_gls_sumrules(**kwargs)
+def check_sum_rules(**kwargs):
+    q2grids, gls_results, preds_int = check_sumrule(**kwargs)
 
-    xf3avg_int_mean = np.mean(xf3avg_int, axis=0)
-    xf3avg_int_stdev = np.std(xf3avg_int, axis=0)
+    preds_int_mean = np.mean(preds_int, axis=0)
+    preds_int_stdev = np.std(preds_int, axis=0)
 
     fig, ax = plt.subplots()
     ax.errorbar(
         q2grids,
-        xf3avg_int_mean,
-        yerr=xf3avg_int_stdev,
+        preds_int_mean,
+        yerr=preds_int_stdev,
         color="C1",
         fmt=".",
         marker="s",
         markersize=11,
         mfc="w",
         label=r"$\rm{NNSF}\nu$",
         capsize=6,
@@ -241,49 +243,98 @@
     )
     ax.scatter(
         q2grids,
         gls_results,
         color="C0",
         s=45,
         marker="o",
-        label=r"$\rm{GLS}$",
+        label=r"$\rm{" + f"{kwargs['rule']}" + r"}$",
         zorder=1,
     )
 
     xmin_log = abs(kwargs["nx_specs"]["xmin_log"])
-    if xmin_log == 3:
-        xmin_label = r"$10^{-3}$"
-    elif xmin_log == 4:
-        xmin_label = r"$10^{-4}$"
-    elif xmin_log == 2:
-        xmin_label = r"$10^{-2}$"
-    else:
-        raise ValueError("Value non-recognised!!!")
+    xmin_label = r"$10^{" + f"-{xmin_log}" + r"}$"
 
     ax.grid(alpha=0.1)
     ax.legend(
         title=rf"$A={kwargs['a_value']}$" + r",~$x_{\rm min}=$" + xmin_label
     )
     ax.set_xlabel(r"$Q^2~[\rm{GeV}^2]$")
     ax.set_ylabel(r"$\rm{Value}$")
-    plotname = f"gls_sumrule_a{kwargs['a_value']}_xmin{abs(xmin_log)}"
+
+    plotname = f"{kwargs['rule'].lower()}_sumrule_a{kwargs['a_value']}_xmin{xmin_log}"
     save_path = pathlib.Path(kwargs["output"]) / plotname
+
+    save_figs(fig, save_path)
+
+
+def check_effective_charge(**kwargs):
+    # Compute a_eff as a function of Q2 using NN model
+    q2grids, preds_int = effective_charge(**kwargs)
+
+    # Load the experimental values including uncertainties
+    q_values, central, error = format_jlab(data="JLAB")
+
+    fig, ax = plt.subplots()
+    ax.errorbar(
+        q_values,
+        central / np.pi,
+        yerr=error,
+        color="C0",
+        # fmt=".",
+        marker="o",
+        markersize=11,
+        mfc="w",
+        label=r"$\rm{JLAB~(EG1,EG4,E97110)}$",
+        capsize=6,
+        zorder=0,
+        linestyle="none",
+    )
+
+    # Compute the 68% Confidence Level for NN predictions
+    lower_68 = np.sort(preds_int, axis=0)[int(.16 * preds_int.shape[0])]
+    upper_68 = np.sort(preds_int, axis=0)[int(.84 * preds_int.shape[0])]
+    mean_prd = np.mean(preds_int, axis=0)
+    ax.fill_between(
+        np.sqrt(q2grids),
+        lower_68,
+        upper_68,
+        color="C1",
+        alpha=0.15,
+        label=r"$\rm{NNSF}\nu$",
+    )
+    ax.plot(np.sqrt(q2grids), mean_prd, color="C1", lw=1.5)
+
+    xmin_log = abs(kwargs["nx_specs"]["xmin_log"])
+    xmin_label = r"$10^{" + f"-{xmin_log}" + r"}$"
+
+    ax.grid(alpha=0.1)
+    ax.legend(
+        title=rf"$A={kwargs['a_value']}$" + r",~$x_{\rm min}=$" + xmin_label
+    )
+    ax.set_xlim(left=np.sqrt(q2grids).min(), right=np.sqrt(q2grids).max())
+    ax.set_xlabel(r"$Q~[\rm{GeV}]$")
+    ax.set_ylabel(r"$\alpha_{\rm eff}$" + f"({EQ_LABELS[kwargs['rule']]})")
+
+    plotname = f"{kwargs['rule'].lower()}_aseff_a{kwargs['a_value']}_xmin{xmin_log}"
+    save_path = pathlib.Path(kwargs["output"]) / plotname
+
     save_figs(fig, save_path)
 
 
 def sfs_q_replicas(**kwargs):
     prediction_info = get_predictions_q(**kwargs)
     predictions = prediction_info.predictions
     if not isinstance(predictions, np.ndarray):
         raise InputError("The input x should be a float.")
     q_grid = prediction_info.q
     for prediction_index in range(predictions.shape[2]):
         fig, ax = plt.subplots()
         ax.set_xlabel("Q2 (GeV)")
-        ax.set_ylabel(basis[prediction_index])
+        ax.set_ylabel(BASIS[prediction_index])
         ax.set_title(f"x={prediction_info.x}, A={prediction_info.A}")
         prediction = predictions[:, :, prediction_index]
         for replica_prediction in prediction:
             ax.plot(q_grid, replica_prediction, color="C0")
         savepath = (
             pathlib.Path(kwargs["output"])
             / f"plot_sfs_q_replicas_{prediction_index}"
@@ -301,15 +352,15 @@
     lower_68 = np.sort(predictions, axis=0)[int(0.16 * n_sfs)]
     upper_68 = np.sort(predictions, axis=0)[int(0.84 * n_sfs)]
     mean_sfs = np.mean(predictions, axis=0)
     std_sfs = np.std(predictions, axis=0)
     for prediction_index in range(predictions.shape[2]):
         fig, ax = plt.subplots()
         ax.set_xlabel(r"$Q^2~[\mathrm{GeV^2}]$")
-        ax.set_ylabel(basis[prediction_index])
+        ax.set_ylabel(BASIS[prediction_index])
         ax.set_title(f"x={prediction_info.x}, A={prediction_info.A}")
         ax.plot(
             q_grid,
             mean_sfs[:, prediction_index] - std_sfs[:, prediction_index],
             color="C0",
             linestyle="--",
         )
```

### Comparing `nnusf-0.2.4/src/nnusf/plot/kinematics.py` & `nnusf-0.2.5/src/nnusf/plot/kinematics.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/plot/matching.py` & `nnusf-0.2.5/src/nnusf/plot/matching.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/plot/sf.py` & `nnusf-0.2.5/src/nnusf/plot/sf.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/plot/th_covmat.py` & `nnusf-0.2.5/src/nnusf/plot/th_covmat.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/plotstyle.mplstyle` & `nnusf-0.2.5/src/nnusf/plotstyle.mplstyle`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/reports/assets/index.html` & `nnusf-0.2.5/src/nnusf/reports/assets/index.html`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/reports/assets/report.css` & `nnusf-0.2.5/src/nnusf/reports/assets/report.css`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/reports/genfiles.py` & `nnusf-0.2.5/src/nnusf/reports/genfiles.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/reports/genhtml.py` & `nnusf-0.2.5/src/nnusf/reports/genhtml.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/scripts/gettheory.py` & `nnusf-0.2.5/src/nnusf/scripts/gettheory.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/scripts/integrate.py` & `nnusf-0.2.5/src/nnusf/scripts/integrate.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/scripts/isoscalar.py` & `nnusf-0.2.5/src/nnusf/scripts/isoscalar.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 TODO: Add exception for LHAPDF set that contains subgrids.
 """
 import logging
 
 import numpy as np
 
-from ..export_lhapdf.dump_grids import dump_pred_lhapdf
-from ..export_lhapdf.utils import install_pdf
+from ..lhapdf.dump_grids import dump_pred_lhapdf
+from ..lhapdf.utils import install_pdf
 from ..utils import ROUNDING, compute_lhapdf
 
 _logger = logging.getLogger(__name__)
 
 
 ISOSPIN_CONJUGATION = {-2: -1, -1: -2, 1: 2, 2: 1}
```

### Comparing `nnusf-0.2.4/src/nnusf/sffit/callbacks.py` & `nnusf-0.2.5/src/nnusf/sffit/callbacks.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/sffit/compute_expchi2.py` & `nnusf-0.2.5/src/nnusf/sffit/compute_expchi2.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/sffit/layers.py` & `nnusf-0.2.5/src/nnusf/sffit/layers.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/sffit/load_data.py` & `nnusf-0.2.5/src/nnusf/sffit/load_data.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/sffit/load_fit_data.py` & `nnusf-0.2.5/src/nnusf/sffit/load_fit_data.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/sffit/model_gen.py` & `nnusf-0.2.5/src/nnusf/sffit/model_gen.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/sffit/postfit.py` & `nnusf-0.2.5/src/nnusf/sffit/postfit.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/sffit/run_sffit.py` & `nnusf-0.2.5/src/nnusf/sffit/run_sffit.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/sffit/scaling.py` & `nnusf-0.2.5/src/nnusf/sffit/scaling.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/sffit/train_model.py` & `nnusf-0.2.5/src/nnusf/sffit/train_model.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/sffit/utils.py` & `nnusf-0.2.5/src/nnusf/sffit/utils.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/theory/assets/genie.hdf5` & `nnusf-0.2.5/src/nnusf/theory/assets/genie.hdf5`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/theory/assets/theory_nnusf.yaml` & `nnusf-0.2.5/src/nnusf/theory/assets/theory_nnusf.yaml`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/theory/bodek_yang/__init__.py` & `nnusf-0.2.5/src/nnusf/theory/bodek_yang/__init__.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/theory/bodek_yang/load.py` & `nnusf-0.2.5/src/nnusf/theory/bodek_yang/load.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/theory/bodek_yang/runcards.py` & `nnusf-0.2.5/src/nnusf/theory/bodek_yang/runcards.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/theory/compare_to_data.py` & `nnusf-0.2.5/src/nnusf/theory/compare_to_data.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/theory/data_vs_theory/runcards.py` & `nnusf-0.2.5/src/nnusf/theory/data_vs_theory/runcards.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/theory/defs.py` & `nnusf-0.2.5/src/nnusf/theory/defs.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/theory/grids.py` & `nnusf-0.2.5/src/nnusf/theory/grids.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/theory/highq/load.py` & `nnusf-0.2.5/src/nnusf/theory/highq/load.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/theory/highq/runcards.py` & `nnusf-0.2.5/src/nnusf/theory/highq/runcards.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/theory/predictions.py` & `nnusf-0.2.5/src/nnusf/theory/predictions.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,24 @@
 import matplotlib.colors as clr
 import matplotlib.pyplot as plt
 import numpy as np
 import numpy.typing as npt
 import pineappl
 import yaml
 
-from nnusf.export_lhapdf.dump_grids import ROUNDING
-
-from .. import utils
-from ..export_lhapdf.dump_grids import LHAPDF_ID, dump_pred_lhapdf
 from . import defs
 from .bodek_yang import load
+from .. import utils
+from ..lhapdf.dump_grids import LHAPDF_ID, dump_pred_lhapdf
+from ..utils import ROUNDING
 
 _logger = logging.getLogger(__name__)
 
-ROUNDING = 6
 # The labels and IDs elow have to match exactly
 SFS_LABEL = ["F2nu", "FLnu", "xF3nu", "F2nub", "FLnub", "xF3nub"]
-LHAPDF_ID = [1001, 1002, 1003, 2001, 2002, 2003, 3001, 3002, 3003]
 
 
 def plot(
     pred: npt.NDArray,
     genie: load.Data,
     gmask: npt.NDArray,
     obs: str,
```

### Comparing `nnusf-0.2.4/src/nnusf/theory/runcards.py` & `nnusf-0.2.5/src/nnusf/theory/runcards.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/theory/yadknots/runcards.py` & `nnusf-0.2.5/src/nnusf/theory/yadknots/runcards.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/src/nnusf/utils.py` & `nnusf-0.2.5/src/nnusf/utils.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/tests/test_loader.py` & `nnusf-0.2.5/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.4/PKG-INFO` & `nnusf-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnusf
-Version: 0.2.4
+Version: 0.2.5
 Summary: Predictions for all-energy neutrino structure functions
 Home-page: https://github.com/NNPDF/nnusf
 Author: Alessandro Candido
 Author-email: candido.ale@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nnusf Version: 0.2.4 Summary: Predictions for all-
+Metadata-Version: 2.1 Name: nnusf Version: 0.2.5 Summary: Predictions for all-
 energy neutrino structure functions Home-page: https://github.com/NNPDF/nnusf
 Author: Alessandro Candido Author-email: candido.ale@gmail.com Requires-Python:
 >=3.9,<3.11 Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering Classifier:
```

