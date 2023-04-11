# Comparing `tmp/qp-prob-0.7.1.tar.gz` & `tmp/qp-prob-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qp-prob-0.7.1.tar", last modified: Wed Nov  9 22:40:13 2022, max compression
+gzip compressed data, was "qp-prob-0.8.0.tar", last modified: Tue Apr 11 01:52:12 2023, max compression
```

## Comparing `qp-prob-0.7.1.tar` & `qp-prob-0.8.0.tar`

### file list

```diff
@@ -1,87 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:40:13.361105 qp-prob-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-09 22:39:58.000000 qp-prob-0.7.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-11-09 22:39:58.000000 qp-prob-0.7.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-09 22:39:58.000000 qp-prob-0.7.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:40:13.345105 qp-prob-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:40:13.349105 qp-prob-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-11-09 22:39:58.000000 qp-prob-0.7.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-11-09 22:39:58.000000 qp-prob-0.7.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-11-09 22:39:58.000000 qp-prob-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    12812 2022-11-09 22:39:58.000000 qp-prob-0.7.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)     1686 2022-11-09 22:39:58.000000 qp-prob-0.7.1/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-11-09 22:39:58.000000 qp-prob-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3720 2022-11-09 22:40:13.361105 qp-prob-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2048 2022-11-09 22:39:58.000000 qp-prob-0.7.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)       52 2022-11-09 22:39:58.000000 qp-prob-0.7.1/do_cover.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:40:13.353105 qp-prob-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-11-09 22:39:58.000000 qp-prob-0.7.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     6764 2022-11-09 22:39:58.000000 qp-prob-0.7.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-11-09 22:39:58.000000 qp-prob-0.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     9914 2022-11-09 22:39:58.000000 qp-prob-0.7.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)   861344 2022-11-09 22:39:58.000000 qp-prob-0.7.1/docs/demo.html
--rw-r--r--   0 runner    (1001) docker     (121)     2858 2022-11-09 22:39:58.000000 qp-prob-0.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-11-09 22:39:58.000000 qp-prob-0.7.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)   757141 2022-11-09 22:39:58.000000 qp-prob-0.7.1/docs/practical_example.html
--rw-r--r--   0 runner    (1001) docker     (121)     2965 2022-11-09 22:39:58.000000 qp-prob-0.7.1/docs/qp.rst
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-11-09 22:39:58.000000 qp-prob-0.7.1/docs/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:40:13.353105 qp-prob-0.7.1/nb/
--rw-r--r--   0 runner    (1001) docker     (121)    32257 2022-11-09 22:39:58.000000 qp-prob-0.7.1/nb/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-11-09 22:39:58.000000 qp-prob-0.7.1/nb/iterator_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    11839 2022-11-09 22:39:58.000000 qp-prob-0.7.1/nb/practical_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-11-09 22:39:58.000000 qp-prob-0.7.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (121)      326 2022-11-09 22:39:58.000000 qp-prob-0.7.1/render_nb.sh
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-09 22:39:58.000000 qp-prob-0.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-09 22:40:13.361105 qp-prob-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-09 22:39:58.000000 qp-prob-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:40:13.345105 qp-prob-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:40:13.361105 qp-prob-0.7.1/src/qp/
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-09 22:40:12.000000 qp-prob-0.7.1/src/qp/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    11300 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/conversion_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:40:13.361105 qp-prob-0.7.1/src/qp/data/
--rw-r--r--   0 runner    (1001) docker     (121)   161680 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/data/CFHTLens_sample.P.npy
--rw-r--r--   0 runner    (1001) docker     (121)    14000 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/data/test.hdf5
--rw-r--r--   0 runner    (1001) docker     (121)     5697 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/dict_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    20726 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (121)    10628 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     6549 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/hist_pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)    12926 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/interp_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:40:13.361105 qp-prob-0.7.1/src/qp/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6808 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/metrics/array_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3322 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/metrics/brier.py
--rw-r--r--   0 runner    (1001) docker     (121)    16855 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     7610 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/metrics/pit.py
--rw-r--r--   0 runner    (1001) docker     (121)     6187 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/mixmod_pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)    14236 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/pdf_gen.py
--rw-r--r--   0 runner    (1001) docker     (121)     7203 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)    11548 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/quant_pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/scipy_pdfs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4532 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/sparse_pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)    10097 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/sparse_rep.py
--rw-r--r--   0 runner    (1001) docker     (121)    10555 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/spline_pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/test_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     7824 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)    23910 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-11-09 22:39:58.000000 qp-prob-0.7.1/src/qp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:40:13.361105 qp-prob-0.7.1/src/qp_prob.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3720 2022-11-09 22:40:13.000000 qp-prob-0.7.1/src/qp_prob.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-11-09 22:40:13.000000 qp-prob-0.7.1/src/qp_prob.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 22:40:13.000000 qp-prob-0.7.1/src/qp_prob.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-11-09 22:40:13.000000 qp-prob-0.7.1/src/qp_prob.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-11-09 22:40:13.000000 qp-prob-0.7.1/src/qp_prob.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:40:13.345105 qp-prob-0.7.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:40:13.361105 qp-prob-0.7.1/tests/qp/
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-11-09 22:39:58.000000 qp-prob-0.7.1/tests/qp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-11-09 22:39:58.000000 qp-prob-0.7.1/tests/qp/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-11-09 22:39:58.000000 qp-prob-0.7.1/tests/qp/fidelity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2821 2022-11-09 22:39:58.000000 qp-prob-0.7.1/tests/qp/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (121)     4607 2022-11-09 22:39:58.000000 qp-prob-0.7.1/tests/qp/test_brier.py
--rw-r--r--   0 runner    (1001) docker     (121)     7240 2022-11-09 22:39:58.000000 qp-prob-0.7.1/tests/qp/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (121)     2744 2022-11-09 22:39:58.000000 qp-prob-0.7.1/tests/qp/test_eval_funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-11-09 22:39:58.000000 qp-prob-0.7.1/tests/qp/test_flex_coefs.npy
--rw-r--r--   0 runner    (1001) docker     (121)     1781 2022-11-09 22:39:58.000000 qp-prob-0.7.1/tests/qp/test_infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (121)    14633 2022-11-09 22:39:58.000000 qp-prob-0.7.1/tests/qp/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3010 2022-11-09 22:39:58.000000 qp-prob-0.7.1/tests/qp/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-11-09 22:39:58.000000 qp-prob-0.7.1/tests/qp/test_pit.py
--rw-r--r--   0 runner    (1001) docker     (121)     2894 2022-11-09 22:39:58.000000 qp-prob-0.7.1/tests/qp/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:12.003129 qp-prob-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-11 01:52:01.000000 qp-prob-0.8.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-11 01:52:01.000000 qp-prob-0.8.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-11 01:52:01.000000 qp-prob-0.8.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.995129 qp-prob-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.995129 qp-prob-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-04-11 01:52:01.000000 qp-prob-0.8.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-04-11 01:52:01.000000 qp-prob-0.8.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1251 2023-04-11 01:52:01.000000 qp-prob-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-04-11 01:52:01.000000 qp-prob-0.8.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-11 01:52:01.000000 qp-prob-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3720 2023-04-11 01:52:12.003129 qp-prob-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-04-11 01:52:01.000000 qp-prob-0.8.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)       52 2023-04-11 01:52:01.000000 qp-prob-0.8.0/do_cover.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.999129 qp-prob-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     6764 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9914 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)   861344 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/demo.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (122)   757141 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/practical_example.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/qp.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.999129 qp-prob-0.8.0/nb/
+-rw-r--r--   0 runner    (1001) docker     (122)    32323 2023-04-11 01:52:01.000000 qp-prob-0.8.0/nb/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-04-11 01:52:01.000000 qp-prob-0.8.0/nb/iterator_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    15156 2023-04-11 01:52:01.000000 qp-prob-0.8.0/nb/metrics_examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     4917 2023-04-11 01:52:01.000000 qp-prob-0.8.0/nb/mixmod_examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    11839 2023-04-11 01:52:01.000000 qp-prob-0.8.0/nb/practical_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    37404 2023-04-11 01:52:01.000000 qp-prob-0.8.0/nb/quantile_parameterization_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-04-11 01:52:01.000000 qp-prob-0.8.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (122)      326 2023-04-11 01:52:01.000000 qp-prob-0.8.0/render_nb.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-11 01:52:01.000000 qp-prob-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 01:52:12.003129 qp-prob-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-11 01:52:01.000000 qp-prob-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.995129 qp-prob-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.999129 qp-prob-0.8.0/src/qp/
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-11 01:52:11.000000 qp-prob-0.8.0/src/qp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11413 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/conversion_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.999129 qp-prob-0.8.0/src/qp/data/
+-rw-r--r--   0 runner    (1001) docker     (122)   161680 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/data/CFHTLens_sample.P.npy
+-rw-r--r--   0 runner    (1001) docker     (122)    16848 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/data/test.hdf5
+-rw-r--r--   0 runner    (1001) docker     (122)     5697 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/dict_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    21140 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11359 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6521 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/hist_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12842 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/interp_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.999129 qp-prob-0.8.0/src/qp/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4454 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/metrics/array_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3322 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/metrics/brier.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/metrics/goodness_of_fit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17889 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7560 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/metrics/pit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6155 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/mixmod_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/packed_interp_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4298 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/packing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14160 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/pdf_gen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7203 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9099 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/quant_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:12.003129 qp-prob-0.8.0/src/qp/quantile_pdf_constructors/
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/quantile_pdf_constructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/quantile_pdf_constructors/abstract_pdf_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4535 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/quantile_pdf_constructors/cdf_spline_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6796 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/quantile_pdf_constructors/dual_spline_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4251 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/quantile_pdf_constructors/piecewise_constant.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3952 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/quantile_pdf_constructors/piecewise_linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/scipy_pdfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4448 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/sparse_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10121 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/sparse_rep.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10537 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/spline_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7824 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23972 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:12.003129 qp-prob-0.8.0/src/qp_prob.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3720 2023-04-11 01:52:11.000000 qp-prob-0.8.0/src/qp_prob.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-04-11 01:52:11.000000 qp-prob-0.8.0/src/qp_prob.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 01:52:11.000000 qp-prob-0.8.0/src/qp_prob.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-11 01:52:11.000000 qp-prob-0.8.0/src/qp_prob.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        3 2023-04-11 01:52:11.000000 qp-prob-0.8.0/src/qp_prob.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.995129 qp-prob-0.8.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:12.003129 qp-prob-0.8.0/tests/qp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:12.003129 qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4854 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/test_cdf_spline_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4145 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/test_dual_spline_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3433 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/test_piecewise_constant.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/test_piecewise_linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4607 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_brier.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2744 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_eval_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4448 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_flex_coefs.npy
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15872 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_pit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5816 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_scipy_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_utils.py
```

### Comparing `qp-prob-0.7.1/.github/workflows/pypi.yaml` & `qp-prob-0.8.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/.github/workflows/python-package.yml` & `qp-prob-0.8.0/.github/workflows/python-package.yml`

 * *Files 20% similar despite different names*

```diff
@@ -21,26 +21,26 @@
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
+        sudo apt-get update
         sudo apt install -y libopenmpi-dev libhdf5-mpi-dev
         python -m pip install --upgrade pip
         pip install .
         pip install .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-        CC="mpicc" HDF5_MPI="ON" pip install --upgrade --force-reinstall --no-binary=h5py h5py
     - name: Lint with pylint
       run: |
         # stop the build if there are Python syntax errors or undefined names
-        pylint --reports=no --errors-only qp
+        pylint --reports=no --errors-only --ignored-modules=scipy.special qp
         # stp the build if there are a lot of messages
-        pylint --reports=no --fail-under=9.5 qp
+        pylint --reports=no --fail-under=9.5 --ignored-modules=scipy.special qp
         # exit-zero treats all errors as warnings.
         pylint --exit-zero qp
     - name: Test with pytest
       run: |
         python -m pytest --cov-report=xml
         mpiexec -np 2 python -m pytest --no-cov tests/qp/test_parallel.py
     - name: Upload coverage to Codecov
```

### Comparing `qp-prob-0.7.1/.gitignore` & `qp-prob-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/.travis.yml` & `qp-prob-0.8.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/LICENSE` & `qp-prob-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/PKG-INFO` & `qp-prob-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qp-prob
-Version: 0.7.1
+Version: 0.8.0
 License: MIT License
         
         Copyright (c) 2016 Alex Malz & Phil Marshall
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `qp-prob-0.7.1/README.md` & `qp-prob-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/docs/.gitignore` & `qp-prob-0.8.0/docs/.gitignore`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/docs/Makefile` & `qp-prob-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/docs/conf.py` & `qp-prob-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/docs/contributing.rst` & `qp-prob-0.8.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/docs/demo.html` & `qp-prob-0.8.0/docs/demo.html`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/docs/index.rst` & `qp-prob-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/docs/practical_example.html` & `qp-prob-0.8.0/docs/practical_example.html`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/docs/qp.rst` & `qp-prob-0.8.0/docs/qp.rst`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/nb/demo.ipynb` & `qp-prob-0.8.0/nb/demo.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.953155287936771%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'To run `qp`, you will need to first install the module "*

 * *            'by following the instructions '*

 * *            "[here](https://github.com/LSSTDESC/qp/blob/main/docs/install.rst).')], delete: [2]}}, "*

 * *            "24: {'source': {insert: [(5, 'quant_dist = qp.quant(quants=quants, locs=locs)\\n'), "*

 * *            "(9, 'quant_dist1 = qp.quant(quants=np.atleast_1d(quants), "*

 * *            "locs=np.atleast_2d(locs[0]))\\n')], delete: [9, 5]}}, 47: {'source': {insert: [(1 […]*

```diff
@@ -30,15 +30,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Requirements\n",
                 "\n",
-                "To run `qp`, you will need to first install the module by following the instructions [here](https://github.com/LSSTDESC/qp/blob/u/eacharles/eac-dev-v2/docs/install.rst)."
+                "To run `qp`, you will need to first install the module by following the instructions [here](https://github.com/LSSTDESC/qp/blob/main/docs/install.rst)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -309,19 +309,19 @@
             "outputs": [],
             "source": [
                 "# Define the quantile values to compute the locations for\n",
                 "quants = np.linspace(0.01, 0.99, 7)\n",
                 "# Compute the corresponding locations\n",
                 "locs = norm_dist1.ppf(quants)\n",
                 "# Construct the distribution using the quantile value and locations\n",
-                "quant_dist = qp.quant_piecewise(quants=quants, locs=locs)\n",
+                "quant_dist = qp.quant(quants=quants, locs=locs)\n",
                 "quant_vals = quant_dist.pdf(xvals)\n",
                 "print(\"The input and output shapes are:\", xvals.shape, quant_vals.shape)\n",
                 "# Construct a single PDF for plotting\n",
-                "quant_dist1 = qp.quant_piecewise(quants=np.atleast_1d(quants), locs=np.atleast_2d(locs[0]))\n",
+                "quant_dist1 = qp.quant(quants=np.atleast_1d(quants), locs=np.atleast_2d(locs[0]))\n",
                 "fig, axes = qp.plotting.plot_native(quant_dist1, xlim=(-5., 5.), label=\"quantiles\")\n",
                 "leg = fig.legend()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -611,15 +611,15 @@
                 "print(\"Making interp\")\n",
                 "ens_i = ens_n.convert_to(qp.interp_gen, xvals=bins)\n",
                 "print(\"Making spline\")\n",
                 "ens_s = ens_n.convert_to(qp.spline_gen, xvals=bins, method=\"xy\")\n",
                 "#print(\"Making spline from samples\")\n",
                 "#ens_s = ens_n.convert_to(qp.spline_gen, xvals=bins, samples=1000, method=\"samples\")\n",
                 "print(\"Making quants\")\n",
-                "ens_q = ens_n.convert_to(qp.quant_piecewise_gen, quants=quants)\n",
+                "ens_q = ens_n.convert_to(qp.quant_gen, quants=quants)\n",
                 "print(\"Making mixmod\")\n",
                 "ens_m = ens_n.convert_to(qp.mixmod_gen, samples=1000, ncomps=3)\n",
                 "#print(\"Making flexcode\")\n",
                 "#ens_f = ens_n.convert_to(qp.flex_gen, grid=bins, basis_system='cosine')"
             ]
         },
         {
@@ -890,27 +890,32 @@
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "qp_issue_25",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.11"
+            "version": "3.10.8"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "9be1a7334e581107f2753dc5e5ebb12b8975e5f80325d35375311bd0b6b51792"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `qp-prob-0.7.1/nb/iterator_demo.ipynb` & `qp-prob-0.8.0/nb/iterator_demo.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/nb/practical_example.ipynb` & `qp-prob-0.8.0/nb/practical_example.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/pyproject.toml` & `qp-prob-0.8.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 dynamic = ["version"]
 dependencies = [
     "matplotlib",
     "numpy",
     "scipy >= 1.9.0",
     "scikit-learn",
     "tables_io >= 0.7.7",
+    "deprecated",
 ]
 
 
 [metadata]
 author = "Alex Malz, Phil Marshall, Eric Charles"
 author_email = "aimalz@nyu.edu, pjm@slac.stanford.edu, echarles@slac.stanford.edu"
 description = "Quantile parametrization of probability distribution functions"
@@ -65,7 +66,27 @@
 branch = true
 
 [tool.pytest.ini_options]
 addopts = [
     "--cov=qp",
     "--cov-report=html"
 ]
+
+[tool.pylint]
+disable = [
+    "abstract-method",
+    "invalid-name",
+    "too-many-statements",
+    "too-many-arguments",
+    "too-many-instance-attributes",
+    "missing-module-docstring",
+    "missing-class-docstring",
+    "missing-function-docstring",
+    "too-few-public-methods",
+    "duplicate-code",
+    "use-dict-literal",
+    "consider-using-f-string",
+]
+max-line-length = 150
+max-locals = 50
+max-branches = 25
+max-public-methods = 50
```

### Comparing `qp-prob-0.7.1/src/qp/conversion_funcs.py` & `qp-prob-0.8.0/src/qp/conversion_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """This module implements functions to convert distributions between various representations
 These functions should then be registered with the `qp.ConversionDict` using `qp_add_mapping`.
 That will allow the automated conversion mechanisms to work.
 """
 import numpy as np
 
 from sklearn import mixture
-from .sparse_rep import indices2shapes, build_sparse_representation, decode_sparse_indices
 from scipy import integrate as sciint
 from scipy import interpolate as sciinterp
 
+from .sparse_rep import indices2shapes, build_sparse_representation, decode_sparse_indices
+
 def extract_vals_at_x(in_dist, **kwargs):
     """Convert using a set of x and y values.
 
     Parameters
     ----------
     in_dist : `qp.Ensemble`
         Input distributions
@@ -201,24 +202,26 @@
 
     Keywords
     --------
     ncomps : `int`
         Number of components in mixture model to use
     nsamples : `int`
         Number of samples to generate
+    random_state : `int`
+        Used to reproducibly generate random variate from in_dist
 
     Returns
     -------
     data : `dict`
         The extracted data
     """
     n_comps = kwargs.pop('ncomps', 3)
     n_sample = kwargs.pop('nsamples', 1000)
-    #samples = in_dist.rvs(size=(in_dist.npdf, n_sample))
-    samples = in_dist.rvs(size=n_sample)
+    random_state = kwargs.pop('random_state', None)
+    samples = in_dist.rvs(size=n_sample, random_state=random_state)
     def mixmod_helper(samps):
         estimator = mixture.GaussianMixture(n_components=n_comps)
         estimator.fit(samps.reshape(-1, 1))
         weights = estimator.weights_
         means = estimator.means_[:, 0]
         stdevs = np.sqrt(estimator.covariances_[:, 0, 0])
         ov = np.vstack([weights, means, stdevs])
```

### Comparing `qp-prob-0.7.1/src/qp/data/CFHTLens_sample.P.npy` & `qp-prob-0.8.0/src/qp/data/CFHTLens_sample.P.npy`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/src/qp/data/test.hdf5` & `qp-prob-0.8.0/src/qp/data/test.hdf5`

 * *Files 14% similar despite different names*

#### h5dump {}

```diff
@@ -1,9 +1,117 @@
-HDF5 "/tmp/diffoscope_sbvpluuq_/tmpn_2cdcpf_TarContainer/0/42.hdf5" {
+HDF5 "/tmp/diffoscope_sbvpluuq_/tmpwsp4x18f_TarContainer/0/44.hdf5" {
 GROUP "/" {
+   GROUP "ancil" {
+      DATASET "mode" {
+         DATATYPE  H5T_IEEE_F64LE
+         DATASPACE  SIMPLE { ( 100, 1 ) / ( 100, 1 ) }
+         DATA {
+         (0,0): 0.11,
+         (1,0): 0,
+         (2,0): 0.14,
+         (3,0): 0.24,
+         (4,0): 0,
+         (5,0): 0,
+         (6,0): 0,
+         (7,0): 0,
+         (8,0): 0,
+         (9,0): 0,
+         (10,0): 0.315,
+         (11,0): 0,
+         (12,0): 0,
+         (13,0): 0,
+         (14,0): 0,
+         (15,0): 0,
+         (16,0): 0.735,
+         (17,0): 0,
+         (18,0): 0.82,
+         (19,0): 0.2,
+         (20,0): 0,
+         (21,0): 0.75,
+         (22,0): 0.14,
+         (23,0): 0,
+         (24,0): 0,
+         (25,0): 0.57,
+         (26,0): 0,
+         (27,0): 0.25,
+         (28,0): 0.625,
+         (29,0): 0,
+         (30,0): 0.1,
+         (31,0): 0,
+         (32,0): 0,
+         (33,0): 0,
+         (34,0): 0.035,
+         (35,0): 0,
+         (36,0): 0,
+         (37,0): 0.845,
+         (38,0): 0,
+         (39,0): 0.96,
+         (40,0): 0,
+         (41,0): 0.7,
+         (42,0): 0.18,
+         (43,0): 0.825,
+         (44,0): 0.905,
+         (45,0): 0,
+         (46,0): 0,
+         (47,0): 0,
+         (48,0): 0.115,
+         (49,0): 0.465,
+         (50,0): 0,
+         (51,0): 0.57,
+         (52,0): 0,
+         (53,0): 0,
+         (54,0): 0,
+         (55,0): 0.445,
+         (56,0): 0.085,
+         (57,0): 0,
+         (58,0): 0,
+         (59,0): 0.61,
+         (60,0): 0.45,
+         (61,0): 0,
+         (62,0): 0,
+         (63,0): 0,
+         (64,0): 0.615,
+         (65,0): 0,
+         (66,0): 0,
+         (67,0): 0,
+         (68,0): 0.265,
+         (69,0): 0,
+         (70,0): 0.685,
+         (71,0): 0.335,
+         (72,0): 0.33,
+         (73,0): 1,
+         (74,0): 0,
+         (75,0): 0,
+         (76,0): 0,
+         (77,0): 0.84,
+         (78,0): 0.45,
+         (79,0): 0,
+         (80,0): 0,
+         (81,0): 0.44,
+         (82,0): 0.095,
+         (83,0): 0.285,
+         (84,0): 0.32,
+         (85,0): 0.725,
+         (86,0): 0,
+         (87,0): 0,
+         (88,0): 0,
+         (89,0): 0,
+         (90,0): 0,
+         (91,0): 0,
+         (92,0): 0.465,
+         (93,0): 0.2,
+         (94,0): 0,
+         (95,0): 0,
+         (96,0): 0.33,
+         (97,0): 0.19,
+         (98,0): 0,
+         (99,0): 0
+         }
+      }
+   }
    GROUP "data" {
       DATASET "means" {
          DATATYPE  H5T_IEEE_F64LE
          DATASPACE  SIMPLE { ( 100, 3 ) / ( 100, 3 ) }
          DATA {
          (0,0): 0.0949178, 1.29877, -0.925832,
          (1,0): -0.963886, 0.171347, -2.08733,
```

### Comparing `qp-prob-0.7.1/src/qp/dict_utils.py` & `qp-prob-0.8.0/src/qp/dict_utils.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/src/qp/ensemble.py` & `qp-prob-0.8.0/src/qp/ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,14 +424,29 @@
             (s) at which to evaluate the pdfs
 
         Returns
         -------
         """
         return self._frozen.sf(q)
 
+    def logsf(self, q):
+        """Evaluates the log of the survival function of the distribution
+
+        Parameters
+        ----------
+        q: float or ndarray, float
+            location(s) at which to evaluate the pdfs
+
+        Returns
+        -------
+        float or ndarray
+            Log of the survival function
+        """
+        return self._frozen.logsf(q)
+
     def isf(self, q):
         """
         Evaluates the inverse of the survival fraction of the distribution
 
         Parameters
         ----------
         x: float or ndarray, float
@@ -663,15 +678,19 @@
     #     -------
     #     self.stacked: tuple, ndarray, float
     #         pair of arrays for locations where approximations were evaluated
     #         and the values of the stacked PDFs at those points
     #
     #     Notes
     #     -----
-    #     Stacking refers to taking the sum of PDFs evaluated on a shared grid and normalizing it such that it integrates to unity.  This is equivalent to calculating an average probability (based on the PDFs in the ensemble) over the grid.  This probably should be done in a script and not by qp!  The right way to do it would be to call qp.Ensemble.evaluate() and sum those outputs appropriately.
+    #     Stacking refers to taking the sum of PDFs evaluated on a shared grid and
+    #     normalizing it such that it integrates to unity.  This is equivalent to
+    #     calculating an average probability (based on the PDFs in the ensemble) over the grid.
+    #     This probably should be done in a script and not by qp!  The right way to do it would be to call
+    #     qp.Ensemble.evaluate() and sum those outputs appropriately.
     #     TO DO: make this do something more efficient for mixmod, grid, histogram, samples
     #     TO DO: enable stacking on irregular grid
     #     """
     #     loc_range = max(loc) - min(loc)
     #     delta = loc_range / len(loc)
     #     evaluated = self.evaluate(loc, using=using, norm=True, vb=vb)
     #     stack = np.mean(evaluated[1], axis=0)
```

### Comparing `qp-prob-0.7.1/src/qp/factory.py` & `qp-prob-0.8.0/src/qp/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class Factory(OrderedDict):
     """Factory that creates and mangages PDFs
 
     """
     def __init__(self):
         """C'tor"""
-        super(Factory, self).__init__()
+        super().__init__()
         self._load_scipy_classes()
 
     @staticmethod
     def _build_data_dict(md_table, data_table):
         """Convert the tables to a dictionary that can be used to build an Ensemble"""
         data_dict = {}
 
@@ -116,15 +116,44 @@
         """
         if class_name not in self: #pragma: no cover
             raise KeyError("Class nameed %s is not in factory" % class_name)
         the_class = self[class_name]
         ctor_func = the_class.creation_method(method)
         return Ensemble(ctor_func, data)
 
+    def from_tables(self, tables):
+        """Build this ensemble from a tables
+        
+        Parameters
+        ----------
+        tables: `dict` 
+
+        Notes
+        -----
+        This will use information in the meta data table to figure out how to construct the data
+        need to build the ensemble.
+        """
+        md_table = tables['meta']
+        data_table = tables['data']
+        ancil_table = tables.get('ancil')
 
+        data = self._build_data_dict(md_table, data_table)
+
+        pdf_name = data.pop('pdf_name')
+        pdf_version = data.pop('pdf_version')
+        if pdf_name not in self: #pragma: no cover
+            raise KeyError("Class nameed %s is not in factory" % pdf_name)
+
+        the_class = self[pdf_name]
+        reader_convert = the_class.reader_method(pdf_version)
+        ctor_func = the_class.creation_method(None)
+        if reader_convert is not None: #pragma: no cover
+            data = reader_convert(data)
+        return Ensemble(ctor_func, data=data, ancil=ancil_table)
+       
     def read(self, filename):
         """Read this ensemble from a file
 
         Parameters
         ----------
         filename : `str`
 
@@ -142,58 +171,56 @@
         else:
             keys = None
             allow_missing_keys = False
 
         tables = io.read(filename, NUMPY_DICT, keys=keys,
                          allow_missing_keys=allow_missing_keys) #pylint: disable=no-member
 
-        md_table = tables['meta']
-        data_table = tables['data']
-        ancil_table = tables.get('ancil')
+        return self.from_tables(tables)
 
-        data = self._build_data_dict(md_table, data_table)
+    def data_length(self, filename):
+        """Get the size of data
 
-        pdf_name = data.pop('pdf_name')
-        pdf_version = data.pop('pdf_version')
-        if pdf_name not in self: #pragma: no cover
-            raise KeyError("Class nameed %s is not in factory" % pdf_name)
-
-        the_class = self[pdf_name]
-        reader_convert = the_class.reader_method(pdf_version)
-        ctor_func = the_class.creation_method(None)
-        if reader_convert is not None: #pragma: no cover
-            data = reader_convert(data)
-        return Ensemble(ctor_func, data=data, ancil=ancil_table)
+        Parameters
+        ----------
+        filename : `str`
 
+        Returns
+        -------
+        nrows : `int`
+        """
+        f, _ = io.readHdf5Group(filename, 'data')
+        num_rows = io.getGroupInputDataLength(f)
+        return num_rows
 
     def iterator(self, filename, chunk_size=100_000, rank=0, parallel_size=1):
         """Return an iterator for chunked read
 
         Parameters
         ----------
         filename : `str`
 
         chunk_size : `int`
         """
         extension = os.path.splitext(filename)[1]
         if extension not in ['.hdf5']:  #pragma: no cover
             raise TypeError("Can only use qp.iterator on hdf5 files")
-        
+
         metadata = io.readHdf5ToDict(filename, 'meta')
         pdf_name = metadata.pop('pdf_name')[0].decode()
         pdf_version = metadata.pop('pdf_version')[0]
         if pdf_name not in self: #pragma: no cover
             raise KeyError("Class nameed %s is not in factory" % pdf_name)
         the_class = self[pdf_name]
-        reader_convert = the_class.reader_method(pdf_version)
+        # reader_convert = the_class.reader_method(pdf_version)
         ctor_func = the_class.creation_method(None)
-        
+
         f, infp = io.readHdf5Group(filename, 'data')
         try:
-            ancil_f, ancil_infp = io.readHdf5Group(filename, 'data')
+            ancil_f, ancil_infp = io.readHdf5Group(filename, 'ancil')
         except KeyError:  #pragma: no cover
             ancil_f, ancil_infp = (None, None)
         num_rows = io.getGroupInputDataLength(f)
         ranges = io.data_ranges_by_rank(num_rows, chunk_size, parallel_size, rank)
         data = self._build_data_dict(metadata, {})
         ancil_data = OrderedDict()
         for start, end in ranges:
@@ -202,15 +229,15 @@
             if ancil_f is not None:
                 for key, val in ancil_f.items():
                     ancil_data[key] = io.readHdf5DatasetToArray(val, start, end)
             yield start, end, Ensemble(ctor_func, data=data, ancil=ancil_data)
         infp.close()
         if ancil_infp is not None:
             ancil_infp.close()
-        
+
     def convert(self, in_dist, class_name, **kwds):
         """Read an ensemble to a different repersenation
 
         Parameters
         ----------
         in_dist : `qp.Ensemble`
             Input distributions
@@ -303,7 +330,9 @@
 stats = _FACTORY
 add_class = _FACTORY.add_class
 create = _FACTORY.create
 read = _FACTORY.read
 iterator = _FACTORY.iterator
 convert = _FACTORY.convert
 concatenate = _FACTORY.concatenate
+data_length = _FACTORY.data_length
+from_tables = _FACTORY.from_tables
```

### Comparing `qp-prob-0.7.1/src/qp/hist_pdf.py` & `qp-prob-0.8.0/src/qp/hist_pdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             sums = np.sum(pdfs_2d*self._hbin_widths, axis=1)
             self._hpdfs = (pdfs_2d.T / sums).T
         else: #pragma: no cover
             self._hpdfs = reshape_to_pdf_size(pdfs, -1)
         self._hcdfs = None
         # Set support
         kwargs['shape'] = pdfs.shape[:-1]
-        super(hist_gen, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._addmetadata('bins', self._hbins)
         self._addobjdata('pdfs', self._hpdfs)
 
 
     def _compute_cdfs(self):
         copy_shape = np.array(self._hpdfs.shape)
         copy_shape[-1] += 1
@@ -133,15 +133,15 @@
         xv = 0.5*(self._hbins[1:] + self._hbins[:-1])
         return np.sum(xv**m * self._hpdfs, axis=1) * dx
 
     def _updated_ctor_param(self):
         """
         Set the bins as additional constructor argument
         """
-        dct = super(hist_gen, self)._updated_ctor_param()
+        dct = super()._updated_ctor_param()
         dct['bins'] = self._hbins
         dct['pdfs'] = self._hpdfs
         return dct
 
     @classmethod
     def get_allocation_kwds(cls, npdf, **kwargs):
         if 'bins' not in kwargs: #pragma: no cover
```

### Comparing `qp-prob-0.7.1/src/qp/interp_pdf.py` & `qp-prob-0.8.0/src/qp/interp_pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         if check_input:
             self._compute_ycumul()
             self._yvals = (self._yvals.T / self._ycumul[:,-1]).T
             self._ycumul = (self._ycumul.T / self._ycumul[:,-1]).T
         else:  # pragma: no cover
             self._ycumul = None
 
-        super(interp_gen, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._addmetadata('xvals', self._xvals)
         self._addobjdata('yvals', self._yvals)
 
     def _compute_ycumul(self):
         copy_shape = np.array(self._yvals.shape)
         self._ycumul = np.ndarray(copy_shape)
         self._ycumul[:, 0] = 0.5 * self._yvals[:, 0] * (self._xvals[1] - self._xvals[0])
@@ -140,15 +140,15 @@
         dx = self._xvals[1] - self._xvals[0]
         return np.sum(self._xvals**m * self._yvals, axis=1) * dx
 
     def _updated_ctor_param(self):
         """
         Set the bins as additional constructor argument
         """
-        dct = super(interp_gen, self)._updated_ctor_param()
+        dct = super()._updated_ctor_param()
         dct['xvals'] = self._xvals
         dct['yvals'] = self._yvals
         return dct
 
     @classmethod
     def get_allocation_kwds(cls, npdf, **kwargs):
         """
@@ -250,15 +250,15 @@
         kwargs['shape'] = np.shape(xvals)[:-1]
 
         check_input = kwargs.pop('check_input', True)
         self._yvals = reshape_to_pdf_size(yvals, -1)
         if check_input:
             self._yvals = normalize_interp1d(self._xvals, self._yvals)
         self._ycumul = None
-        super(interp_irregular_gen, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._addobjdata('xvals', self._xvals)
         self._addobjdata('yvals', self._yvals)
 
     def _compute_ycumul(self):
         copy_shape = np.array(self._yvals.shape)
         self._ycumul = np.ndarray(copy_shape)
         self._ycumul[:,0] = 0.
@@ -296,15 +296,15 @@
                                            bounds_error=False, fill_value=(self._xmin, self._xmax)).ravel()
 
 
     def _updated_ctor_param(self):
         """
         Set the bins as additional constructor argument
         """
-        dct = super(interp_irregular_gen, self)._updated_ctor_param()
+        dct = super()._updated_ctor_param()
         dct['xvals'] = self._xvals
         dct['yvals'] = self._yvals
         return dct
 
     @classmethod
     def get_allocation_kwds(cls, npdf, **kwargs):
         """
```

### Comparing `qp-prob-0.7.1/src/qp/metrics/brier.py` & `qp-prob-0.8.0/src/qp/metrics/brier.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/src/qp/metrics/metrics.py` & `qp-prob-0.8.0/src/qp/metrics/metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """This module implements some performance metrics for distribution parameterization"""
 import logging
 from collections import namedtuple
 from functools import partial
+from deprecated import deprecated
 
 import numpy as np
 
-import qp.metrics.array_metrics as array_metrics
+from qp.metrics import array_metrics
+from qp.metrics.goodness_of_fit import goodness_of_fit_metrics
 from qp.metrics.brier import Brier
 from qp.utils import epsilon
 
 Grid = namedtuple('Grid', ['grid_values', 'cardinality', 'resolution', 'hist_bin_edges', 'limits'])
 
 def _calculate_grid_parameters(limits, dx:float=0.01) -> Grid:
     """
@@ -181,15 +183,16 @@
 
     def evaluate_pdf_at_z(z, dist):
         return dist.pdf(z)[0][0]
 
     for n in range(0, p.npdf):
 
         if p[n].npdf != 1:
-            raise ValueError('quick_rbpe only handles Ensembles with a single PDF, for ensembles with more than one PDF, use the qp.metrics.risk_based_point_estimate function.')
+            raise ValueError('quick_rbpe only handles Ensembles with a single PDF '
+                             'for ensembles with more than one PDF, use the qp.metrics.risk_based_point_estimate function.')
 
         this_dist_pdf_at_z = partial(evaluate_pdf_at_z, dist=p[n])
         integration_bounds = (p[n].ppf(0.01)[0][0], p[n].ppf(0.99)[0][0])
 
         rbpes.append(array_metrics.quick_rbpe(this_dist_pdf_at_z, integration_bounds, limits))
 
     return np.array(rbpes)
@@ -242,148 +245,61 @@
 
     # instantiate the Brier metric object
     brier_metric_evaluation = Brier(pdf_values, truth_array)
 
     # return the results of evaluating the Brier metric
     return brier_metric_evaluation.evaluate()
 
-def calculate_anderson_darling(p, scipy_distribution='norm', num_samples=100, _random_state=None):
-    """Calculate the Anderson-Darling statistic using scipy.stats.anderson for each distribution
-    in an Ensemble. For more details see:
-    https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.anderson.html
-
-    Parameters
-    ----------
-    p : qp.Ensemble
-        An Ensemble of distributions to be tested
-    scipy_distribution : {'norm', 'expon', 'logistic', 'gumbel', 'gumbel_l', 'gumbel_r', 'extreme1'}, optional
-        The type of distribution to test against.
-    num_samples : int, optional
-        Number of random variable samples to generate for each distribution in the calculation
-    _random_state : int, optional
-        For testing purposes only, this is used to specify a reproducible set of random variables.
+@deprecated(
+    reason="""
+    This implementation is deprecated for performance reasons and does not accommodate N vs 1 comparisons.
+    Please use calculate_goodness_of_fit instead. This method is for testing purposes only.
+    """,
+    category=DeprecationWarning)
+def calculate_anderson_darling(p, scipy_distribution='norm', num_samples=100, _random_state=None):  # pylint: disable=unused-argument
+    """This function is deprecated and will be completely removed in a later version.
+    Please use `calculate_goodness_of_fit` instead.
 
     Returns
     -------
-    [Result objects]
-        A array of objects with attributes ``statistic``, ``critical_values``, and ``significance_level``.
+    logger.warning
     """
+    logging.warning("This function is deprecated, please use `calculate_goodness_of_fit`") # pragma: no cover
 
-    try:
-        _check_ensemble_is_not_nested(p)
-    except ValueError:  #pragma: no cover - unittest coverage for _check_ensemble_is_not_nested is complete
-        logging.warning("Each element in the ensemble `p` must be a single distribution.")
-
-   # Pass an array of random variables and the name of a scipy distribution to the quick anderson darling function
-    output = [
-            array_metrics.quick_anderson_darling(
-                np.squeeze(p_dist.rvs(size=num_samples, random_state=_random_state)),
-                scipy_distribution=scipy_distribution
-            )
-            for p_dist in p
-        ]
-
-    return output
-
-def calculate_cramer_von_mises(p, q, num_samples=100, _random_state=None, **kwargs):
-    """Calculate the Cramer von Mises statistic using scipy.stats.cramervonmises for each pair of distributions
-    in two input Ensembles. For more details see:
-    https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.cramervonmises.html
-
-    Parameters
-    ----------
-    p : qp.Ensemble
-        An Ensemble of distributions to be tested
-    q : qp.Ensemble
-        A second Ensemble of distributions each with a defined ``cdf`` method, to be tested against
-    num_samples : int, optional
-        Number of random variable samples to generate for the calculation
-    _random_state : int, optional
-        For testing purposes only, this is used to specify a reproducible set of random variables.
+@deprecated(
+    reason="""
+    This implementation is deprecated for performance reasons and does not accommodate N vs 1 comparisons.
+    Please use calculate_goodness_of_fit instead. This method is for testing purposes only.
+    """,
+    category=DeprecationWarning)
+def calculate_cramer_von_mises(p, q, num_samples=100, _random_state=None, **kwargs):  # pylint: disable=unused-argument
+    """This function is deprecated and will be completely removed in a later version.
+    Please use `calculate_goodness_of_fit` instead.
 
     Returns
     -------
-    [Result objects]
-        A array of objects with attributes ``statistic`` and ``pvalue``.
+    logger.warning
     """
+    logging.warning("This function is deprecated, please use `calculate_goodness_of_fit`") # pragma: no cover
 
-    try:
-        _check_ensembles_are_same_size(p, q)
-    except ValueError:  #pragma: no cover - unittest coverage for _check_ensembles_are_same_size is complete
-        logging.warning("Input ensembles should have the same number of distributions")
-
-    try:
-        _check_ensemble_is_not_nested(p)
-    except ValueError:  #pragma: no cover - unittest coverage for _check_ensemble_is_not_nested is complete
-        logging.warning("Each element in the ensemble `p` must be a single distribution.")
-
-    try:
-        _check_ensemble_is_not_nested(q)
-    except ValueError:  #pragma: no cover - unittest coverage for _check_ensemble_is_not_nested is complete
-        logging.warning("Each element in the ensemble `q` must be a single distribution.")
-
-    # Pass an array of random variables and a cdf callable for each pair of distributions to the quick cvm statistic function
-    output = [
-            array_metrics.quick_cramer_von_mises(
-                np.squeeze(p_dist.rvs(size=num_samples, random_state=_random_state)),
-                q_dist.cdf,
-                **kwargs
-            )
-            for p_dist, q_dist in zip(p, q)
-        ]
-
-    return output
-
-def calculate_kolmogorov_smirnov(p, q, num_samples=100, **kwargs):
-    """Calculate the Kolmogorov-Smirnov statistic using scipy.stats.kstest for each pair of distributions
-    in two input Ensembles. For more details see:
-    https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.kstest.html 
-
-    Parameters
-    ----------
-    p : qp.Ensemble
-        An Ensemble of distributions to be tested
-    q : qp.Ensemble
-        A second Ensemble of distributions to be tested
-    num_samples : int, optional
-        Number of samples to use in the calculation
+@deprecated(
+    reason="""
+    This implementation is deprecated for performance reasons and does not accommodate N vs 1 comparisons.
+    Please use calculate_goodness_of_fit instead. This method is for testing purposes only.
+    """,
+    category=DeprecationWarning)
+def calculate_kolmogorov_smirnov(p, q, num_samples=100, _random_state=None):  # pylint: disable=unused-argument
+    """This function is deprecated and will be completely removed in a later version.
+    Please use `calculate_goodness_of_fit` instead.
 
     Returns
     -------
-    [KstestResult]
-        A array of KstestResult objects with attributes ``statistic`` and ``pvalue``.
+    logger.warning
     """
-
-    try:
-        _check_ensembles_are_same_size(p, q)
-    except ValueError:  #pragma: no cover - unittest coverage for _check_ensembles_are_same_size is complete
-        logging.warning("Input ensembles should have the same number of distributions")
-
-    try:
-        _check_ensemble_is_not_nested(p)
-    except ValueError:  #pragma: no cover - unittest coverage for _check_ensemble_is_not_nested is complete
-        logging.warning("Each element in the ensemble `p` must be a single distribution.")
-
-    try:
-        _check_ensemble_is_not_nested(q)
-    except ValueError:  #pragma: no cover - unittest coverage for _check_ensemble_is_not_nested is complete
-        logging.warning("Each element in the ensemble `q` must be a single distribution.")
-
-    # Pass the rvs and cdf functions for each pair of distributions to the quick ks statistic function
-    output = [
-            array_metrics.quick_kolmogorov_smirnov(
-                p_dist.rvs,
-                q_dist.cdf,
-                num_samples=num_samples,
-                **kwargs
-            )
-            for p_dist, q_dist in zip(p, q)
-        ]
-
-    return output
+    logging.warning("This function is deprecated, please use `calculate_goodness_of_fit`") # pragma: no cover
 
 def calculate_outlier_rate(p, lower_limit=0.0001, upper_limit=0.9999):
     """Fraction of outliers in each distribution
 
     Parameters
     ----------
     p : qp.Ensemble
@@ -404,14 +320,81 @@
         _check_ensemble_is_not_nested(p)
     except ValueError:  #pragma: no cover - unittest coverage for _check_ensemble_is_not_nested is complete
         logging.warning("Each element in the ensemble `p` must be a single distribution.")
 
     outlier_rates = [(dist.cdf(lower_limit) + (1. - dist.cdf(upper_limit)))[0][0] for dist in p]
     return outlier_rates
 
+def calculate_goodness_of_fit(estimate, reference, fit_metric='ad', num_samples=100, _random_state=None):
+    """This method calculates goodness of fit between the distributions in the
+    `estimate` and `reference` Ensembles using the specified fit_metric.
+
+    Parameters
+    ----------
+    estimate : Ensemble containing N distributions
+        Random variate samples will be drawn from this Ensemble
+    reference : Ensemble containing N or 1 distributions
+        The CDF of the distributions in this Ensemble are used in the goodness of fit
+        calculation.
+    fit_metric : string, optional
+        The goodness of fit metric to use. One of ['ad', 'cvm', 'ks']. For clarity,
+        'ad' = Anderson-Darling, 'cvm' = Cramer-von Mises, and 'ks' = Kolmogorov-Smirnov, by default 'ad'
+    num_samples : int, optional
+        Number of random variates to draw from each distribution in `estimate`, by default 100
+    _random_state : _type_, optional
+        Used for testing to create reproducible sets of random variates, by default None
+
+    Returns
+    -------
+    output: [float]
+        A array of floats where each element is the result of the statistic calculation.
+
+    Raises
+    ------
+    KeyError
+        If the requested `fit_metric` is not contained in `goodness_of_fit_metrics` dictionary,
+        raise a KeyError.
+
+    Notes
+    -----
+    The calculation of the goodness of fit metrics is not symmetric.
+    i.e. `calculate_goodness_of_fit(p, q, ...) != calculate_goodness_of_fit(q, p, ...)`
+
+    In the future, we should be able to do this directly from the PDFs without needing to
+    take random variates from the `estimate` Ensemble.
+
+    The vectorized implementations of fit metrics are copied over (unmodified) from
+    the developer branch of Scipy 1.10.0dev. When Scipy 1.10 is released, we can replace
+    the copied implementation with the ones in Scipy.
+    """
+
+    try:
+        _check_ensembles_contain_correct_number_of_distributions(estimate, reference)
+    except ValueError: #pragma: no cover - unittest coverage for _check_ensembles_contain_correct_number_of_distributions is complete
+        logging.warning("The ensemble `reference` should have 1 or N distributions. With N = number of distributions in the ensemble `estimate`.")
+
+    try:
+        _check_ensemble_is_not_nested(estimate)
+    except ValueError:  #pragma: no cover - unittest coverage for _check_ensemble_is_not_nested is complete
+        logging.warning("Each element in the ensemble `estimate` must be a single distribution.")
+
+    try:
+        _check_ensemble_is_not_nested(reference)
+    except ValueError:  #pragma: no cover - unittest coverage for _check_ensemble_is_not_nested is complete
+        logging.warning("Each element in the ensemble `reference` must be a single distribution.")
+
+    if fit_metric not in goodness_of_fit_metrics:
+        metrics = list(goodness_of_fit_metrics.keys())
+        raise KeyError(f"`fit_metric` should be one of {metrics}.")
+
+    return goodness_of_fit_metrics[fit_metric](
+        reference,
+        np.squeeze(estimate.rvs(size=num_samples, random_state=_random_state))
+    )
+
 def _check_ensembles_are_same_size(p, q):
     """This utility function ensures checks that two Ensembles contain an equal number of distribution objects.
 
     Args:
         p qp.Ensemble: An Ensemble containing 0 or more distributions
         q qp.Ensemble: A second Ensemble containing 0 or more distributions
 
@@ -429,7 +412,42 @@
 
     Raises:
         ValueError: If there are any elements of the input Ensemble that contain more than 1 PDF, raise an error.
     """
     for dist in p:
         if dist.npdf != 1:
             raise ValueError("Each element in the input Ensemble should be a single distribution.")
+
+def _check_ensembles_contain_correct_number_of_distributions(estimate, reference):
+    """This utility function ensures that the number of distributions in the ensembles matches
+    expectations. estimate can contain 1 to N distributions.
+    reference should contain either 1 or the same number of distributions
+    as estimate.
+
+    Example logic:
+    estimate=N, reference=N (1 <= N) -> Pass
+    estimate=N, reference=1 (1 <= N) -> Pass
+    estimate=1, reference=N (N != 1) -> Raise ValueError
+    estimate=N, reference=M (N != M) -> Raise ValueError
+
+    Parameters
+    ----------
+    estimate : Ensemble
+        Used to calculate goodness of fit metrics, random
+        variates will be produced from the distributions in this ensemble.
+    reference : Ensemble
+        The CDFs of the distributions in this ensemble will be used to calculate
+        goodness of fit metrics.
+
+    Raises
+    ------
+    ValueError
+        If the number of distributions in the reference ensemble does not meet the requirements,
+        raise a ValueError.
+    """
+
+    if estimate.npdf == reference.npdf:
+        pass
+    elif reference.npdf == 1:
+        pass
+    else:
+        raise ValueError("`reference` should contain either 1 distribution or the same number of distributions as `estimate`.")
```

### Comparing `qp-prob-0.7.1/src/qp/metrics/pit.py` & `qp-prob-0.8.0/src/qp/metrics/pit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import numpy as np
 from scipy import stats
 import qp
 from qp.metrics.metrics import calculate_outlier_rate
-from qp.metrics.array_metrics import quick_anderson_ksamp, quick_cramer_von_mises, quick_kolmogorov_smirnov
+from qp.metrics.array_metrics import quick_anderson_ksamp
 
 DEFAULT_QUANTS = np.linspace(0, 1, 100)
 
 class PIT():
     """PIT(qp_ens, true_vals, eval_grid=DEFAULT_QUANTS)
     Probability Integral Transform
 
@@ -43,19 +43,20 @@
         self._true_vals = true_vals
 
         # For each distribution in the Ensemble, calculate the CDF where x = known_true_value
         self._pit_samps = np.array([qp_ens[i].cdf(self._true_vals[i])[0][0] for i in range(len(self._true_vals))])
 
         n_pit = np.min([len(self._pit_samps), len(eval_grid)])
         if n_pit < len(eval_grid):
-            logging.warning('Number of pit samples is smaller than the evaluation grid size. Will create a new evaluation grid with size = number of pit samples')
+            logging.warning('Number of pit samples is smaller than the evaluation grid size. '
+                            'Will create a new evaluation grid with size = number of pit samples')
             eval_grid = np.linspace(0, 1, n_pit)
 
         data_quants = np.quantile(self._pit_samps, eval_grid)
-        self._pit = qp.Ensemble(qp.quant_piecewise, data=dict(quants=eval_grid, locs=np.atleast_2d(data_quants)))
+        self._pit = qp.Ensemble(qp.quant, data=dict(quants=eval_grid, locs=np.atleast_2d(data_quants)))
 
     @property
     def pit_samps(self):
         """Returns the PIT samples. i.e. ``CDF(true_vals)`` for each distribution in the Ensemble used to initialize the PIT object.
 
         Returns
         -------
@@ -67,15 +68,15 @@
     @property
     def pit(self):
         """Return the PIT Ensemble object
 
         Returns
         -------
         qp.Ensemble
-            An Ensemble containing 1 qp.quant_piecewise distribution.
+            An Ensemble containing 1 qp.quant distribution.
         """
         return self._pit
 
     def calculate_pit_meta_metrics(self):
         """Convenience method that will calculate all of the PIT meta metrics and return them 
             as a dictionary.
 
@@ -129,27 +130,27 @@
 
         Returns
         -------
         [Result objects]
             A array of objects with attributes `statistic` and `pvalue`
             For details see: https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.cramervonmises.html
         """
-        return quick_cramer_von_mises(self._pit_samps, stats.uniform.cdf)
+        return stats.cramervonmises(self._pit_samps, stats.uniform.cdf)
 
     def evaluate_PIT_KS(self):
         """Calculate the Kolmogorov-Smirnov statistic using scipy.stats.kstest. For more details see:
         https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.kstest.html
 
         Returns
         -------
         [Return Object]
             A array of objects with attributes `statistic` and `pvalue`.
             For details see: https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.kstest.html
         """
-        return quick_kolmogorov_smirnov(self._pit_samps, stats.uniform.cdf)
+        return stats.kstest(self._pit_samps, stats.uniform.cdf)
 
     def evaluate_PIT_outlier_rate(self, pit_min=0.0001, pit_max=0.9999):
         """Compute fraction of PIT outliers by evaluating the CDF of the distribution in the PIT Ensemble
         at `pit_min` and `pit_max`.
 
         Parameters
         ----------
@@ -159,15 +160,15 @@
             Upper bound for outliers, by default 0.9999
 
         Returns
         -------
         float
             The percentage of outliers in this distribution given the min and max bounds.
         """
-        return calculate_outlier_rate(self._pit, pit_min, pit_max)
+        return calculate_outlier_rate(self._pit, pit_min, pit_max)[0]
 
     def _trim_pit_values(self, cdf_min, cdf_max):
         """Remove and report any cdf(x) that are outside the min/max range.
 
         Parameters
         ----------
         cdf_min : float
```

### Comparing `qp-prob-0.7.1/src/qp/mixmod_pdf.py` & `qp-prob-0.8.0/src/qp/mixmod_pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         """
         self._scipy_version_warning()
         self._means = reshape_to_pdf_size(means, -1)
         self._stds = reshape_to_pdf_size(stds, -1)
         self._weights = reshape_to_pdf_size(weights, -1)
         kwargs['shape'] = means.shape[:-1]
         self._ncomps = means.shape[-1]
-        super(mixmod_gen, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._addobjdata('weights', self._weights)
         self._addobjdata('stds', self._stds)
         self._addobjdata('means', self._means)
 
     def _scipy_version_warning(self):
         import scipy #pylint: disable=import-outside-toplevel
         scipy_version = scipy.__version__
@@ -120,15 +120,15 @@
 
 
 
     def _updated_ctor_param(self):
         """
         Set the bins as additional constructor argument
         """
-        dct = super(mixmod_gen, self)._updated_ctor_param()
+        dct = super()._updated_ctor_param()
         dct['means'] = self._means
         dct['stds'] = self._stds
         dct['weights'] = self._weights
         return dct
 
 
     @classmethod
```

### Comparing `qp-prob-0.7.1/src/qp/pdf_gen.py` & `qp-prob-0.8.0/src/qp/pdf_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,15 @@
             The underlying distribution
         npdf : `int`
             The number of PDFs this object represents
         """
         self._shape = shape
         self._npdf = np.product(shape).astype(int)
         self._ndim = np.size(shape)
-        super(rv_frozen_func, self).__init__(dist, *args, **kwds)
+        super().__init__(dist, *args, **kwds)
 
     @property
     def ndim(self):
         """Return the number of dimensions of PDFs in this ensemble"""
         return self._ndim
 
     @property
@@ -222,15 +222,15 @@
     def __init__(self, dist, shape, *args, **kwds):
         """C'tor"""
         self._shape = shape
         self._npdf = np.product(shape).astype(int)
         self._ndim = np.size(shape)
         if self._npdf is not None:
             kwds.setdefault('row', np.expand_dims(np.arange(self._npdf).reshape(self._shape), -1))
-        super(rv_frozen_rows, self).__init__(dist, *args, **kwds)
+        super().__init__(dist, *args, **kwds)
 
     @property
     def ndim(self):
         """Return the number of dimensions of PDFs in this ensemble"""
         return self._ndim
 
     @property
@@ -271,15 +271,15 @@
     where each object represents a single distribtuion
 
     """
     def __init__(self, *args, **kwargs):
         """C'tor"""
         self._shape = kwargs.pop('shape', (1))
         self._npdf = np.product(self._shape).astype(int)
-        super(Pdf_rows_gen, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     @property
     def shape(self):
         """Return the shape of the set of PDFs this object represents"""
         return self._shape
 
     @property
@@ -375,15 +375,15 @@
     """Mixin class to extend `scipy.stats.rv_continuous` with
     information needed for `qp` for analytic distributions.
 
     """
     def __init__(self, *args, **kwargs):
         """C'tor"""
         # pylint: disable=no-member,protected-access
-        super(Pdf_gen_wrap, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._other_init(*args, **kwargs)
 
 
     def _my_freeze(self, *args, **kwds):
         """Freeze the distribution for the given arguments.
 
         Parameters
```

### Comparing `qp-prob-0.7.1/src/qp/plotting.py` & `qp-prob-0.8.0/src/qp/plotting.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/src/qp/quant_pdf.py` & `qp-prob-0.8.0/src/qp/quant_pdf.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 """This module implements a PDT distribution sub-class using interpolated quantiles
 """
-
+import logging
 import sys
 import numpy as np
 
 from scipy.stats import rv_continuous
 
 from qp.pdf_gen import Pdf_rows_gen
 
 from qp.conversion_funcs import extract_quantiles
 from qp.plotting import get_axes_and_xlims, plot_pdf_quantiles_on_axes
-from qp.utils import evaluate_hist_multi_x_multi_y,\
-     interpolate_multi_x_y, interpolate_x_multi_y,\
-     reshape_to_pdf_size
+from qp.utils import interpolate_multi_x_y, interpolate_x_multi_y, reshape_to_pdf_size
 from qp.test_data import QUANTS, QLOCS, TEST_XVALS
 from qp.factory import add_class
 
+from qp.quantile_pdf_constructors import \
+    AbstractQuantilePdfConstructor, \
+    CdfSplineDerivative, \
+    DualSplineAverage, \
+    PiecewiseConstant, \
+    PiecewiseLinear
+
 
 epsilon = sys.float_info.epsilon
 
 def pad_quantiles(quants, locs):
     """Pad the quantiles and locations used to build a quantile representation
 
     Paramters
@@ -60,14 +65,21 @@
 
     if pad_hi:
         quants_out[-1] = 1.
         locs_out[:, -1] = locs[:, -1] - (1. - quants[-1]) * (locs[:, -2] - locs[:, -1]) / (quants[-1] - quants[-2])
 
     return quants_out, locs_out
 
+DEFAULT_PDF_CONSTRUCTOR = 'piecewise_linear'
+PDF_CONSTRUCTORS = {
+    'cdf_spline_derivative': CdfSplineDerivative,
+    'dual_spline_average': DualSplineAverage,
+    'piecewise_linear': PiecewiseLinear,
+    'piecewise_constant': PiecewiseConstant,
+}
 
 class quant_gen(Pdf_rows_gen):
     """Quantile based distribution, where the PDF is defined piecewise from the quantiles
 
     Notes
     -----
     This implements a CDF by interpolating a set of quantile values
@@ -89,95 +101,143 @@
         Parameters
         ----------
         quants : array_like
            The quantiles used to build the CDF
         locs : array_like
            The locations at which those quantiles are reached
         """
-        kwargs['shape'] = locs.shape[:-1]
 
         self._xmin = np.min(locs)
         self._xmax = np.max(locs)
 
-        super(quant_gen, self).__init__(*args, **kwargs)
-
         locs_2d = reshape_to_pdf_size(locs, -1)
-        check_input = kwargs.pop('check_input', True)
-        if check_input:
+        self._check_input = kwargs.pop('check_input', True)
+        if self._check_input:
             quants, locs_2d = pad_quantiles(quants, locs_2d)
 
         self._quants = np.asarray(quants)
         self._nquants = self._quants.size
         if locs_2d.shape[-1] != self._nquants:  # pragma: no cover
             raise ValueError("Number of locations (%i) != number of quantile values (%i)" % (self._nquants, locs_2d.shape[-1]))
         self._locs = locs_2d
-        self._cdf_derivs = None
-        self._cdf_2nd_derivs = None
-        self._addmetadata('quants', self._quants)
-        self._addobjdata('locs', self._locs)
-
 
-    def _compute_derivs(self):
-        self._cdf_derivs = np.zeros(self.locs.shape)
-        self._cdf_2nd_derivs = np.zeros(self.locs.shape)
+        self._pdf_constructor_name = str(kwargs.pop('pdf_constructor_name', DEFAULT_PDF_CONSTRUCTOR))
+        self._pdf_constructor = None
+        self._instantiate_pdf_constructor()
 
-        self._cdf_derivs[:,0:-1] = (self._quants[1:] - self._quants[0:-1])/(self._locs[:,1:] - self._locs[:,0:-1])
-        self._cdf_2nd_derivs[:,0:-1] = self._cdf_derivs[:,1:]  - self._cdf_derivs[:,0:-1]
+        kwargs['shape'] = locs.shape[:-1]
+        super().__init__(*args, **kwargs)
 
+        self._addmetadata('quants', self._quants)
+        self._addmetadata('pdf_constructor_name', self._pdf_constructor_name)
+        self._addmetadata('check_input', self._check_input)
+        self._addobjdata('locs', self._locs)
 
     @property
     def quants(self):
         """Return quantiles used to build the CDF"""
         return self._quants
 
     @property
     def locs(self):
         """Return the locations at which those quantiles are reached"""
         return self._locs
 
-    def _pdf(self, x, row):
-        # pylint: disable=arguments-differ
-        if self._cdf_derivs is None:  # pragma: no cover
-            self._compute_derivs()
-        return evaluate_hist_multi_x_multi_y(x, row, self._locs, self._cdf_derivs, self._cdf_2nd_derivs).ravel()
+    @property
+    def pdf_constructor_name(self):
+        """Returns the name of the current pdf constructor. Matches a key in
+        the PDF_CONSTRUCTORS dictionary."""
+        return self._pdf_constructor_name
+
+    @pdf_constructor_name.setter
+    def pdf_constructor_name(self, value: str):
+        """Allows users to specify a different interpolator without having to recreate
+        the ensemble.
+
+        Parameters
+        ----------
+        value : str
+            One of the supported interpolators. See PDF_CONSTRUCTORS
+            dictionary for supported interpolators.
+
+        Raises
+        ------
+        ValueError
+            If the value provided isn't a key in PDF_CONSTRUCTORS, raise
+            a value error.
+        """
+        if value not in PDF_CONSTRUCTORS:
+            raise ValueError(f"Unknown interpolator provided: '{value}'. Allowed interpolators are {list(PDF_CONSTRUCTORS.keys())}")
+
+        if value is self._pdf_constructor_name:
+            logging.warning("Already using interpolator: '%s'.", value)
+            return
+
+        self._pdf_constructor_name = value
+        self._instantiate_pdf_constructor()
+        self._addmetadata('pdf_constructor_name', self._pdf_constructor_name)
+
+    @property
+    def pdf_constructor(self) -> AbstractQuantilePdfConstructor:
+        """Returns the current PDF constructor, and allows the user to interact
+        with its methods.
+
+        Returns
+        -------
+        AbstractQuantilePdfConstructor
+            Abstract base class of the active concrete PDF constructor.
+        """
+        return self._pdf_constructor
+
+    def _instantiate_pdf_constructor(self):
+        self._pdf_constructor = PDF_CONSTRUCTORS[self._pdf_constructor_name](
+            self._quants, self._locs)
+
+
+    def _pdf(self, x, *args):
+        # We're not requiring that the output be normalized!
+        # `util.normalize_interp1d` addresses _one_ of the ways that a reconstruction
+        # can be bad, but not all. It should be replaced with a more comprehensive
+        # normalization function.
+        # See qp issue #147
+        row = args[0]
+        return self._pdf_constructor.construct_pdf(x, row)
 
     def _cdf(self, x, row):
         # pylint: disable=arguments-differ
         return interpolate_multi_x_y(x, row, self._locs, self._quants,
                                      bounds_error=False, fill_value=(0., 1), kind="quadratic").ravel()
 
     def _ppf(self, x, row):
         # pylint: disable=arguments-differ
         return interpolate_x_multi_y(x, row, self._quants, self._locs,
                                      bounds_error=False, fill_value=(self._xmin, self._xmax), kind="quadratic").ravel()
 
     def _updated_ctor_param(self):
         """
-        Set the bins as additional construstor argument
+        Set the quants and locs as additional constructor arguments
         """
-        dct = super(quant_gen, self)._updated_ctor_param()
+        dct = super()._updated_ctor_param()
         dct['quants'] = self._quants
         dct['locs'] = self._locs
+        dct['pdf_constructor_name'] = self._pdf_constructor_name
+        dct['check_input'] = self._check_input
         return dct
 
     @classmethod
     def get_allocation_kwds(cls, npdf, **kwargs):
         """Return kwds necessary to create 'empty' hdf5 file with npdf entries
-        for iterative writeout
+        for iterative writeout.  We only need to allocate the objdata columns, as
+        the metadata can be written when we finalize the file.
         """
         try:
             quants = kwargs['quants']
         except ValueError: #pragma: no cover
             print("required argument 'quants' not included in kwargs")
         nquants = np.shape(quants)[-1]
-        # EC, I don't thing you need these lines, as you don't actually store the ends
-        #if quants[0] > sys.float_info.epsilon:
-        #    nquants += 1
-        #if quants[-1] < 1.:
-        #    nquants += 1
         return dict(locs=((npdf, nquants), 'f4'))
 
     @classmethod
     def plot_native(cls, pdf, **kwargs):
         """Plot the PDF in a way that is particular to this type of distibution
 
         For a quantile this shows the quantiles points
@@ -200,143 +260,7 @@
 
 quant = quant_gen.create
 
 quant_gen.test_data = dict(quant=dict(gen_func=quant, ctor_data=dict(quants=QUANTS, locs=QLOCS),\
                                           convert_data=dict(quants=QUANTS), test_xvals=TEST_XVALS))
 
 add_class(quant_gen)
-
-
-
-
-class quant_piecewise_gen(Pdf_rows_gen):
-    """Quantile based distribution, where the PDF is defined piecewise from the quantiles
-
-    Notes
-    -----
-    This implements a CDF by interpolating a set of quantile values
-
-    It simply takes a set of x and y values and uses `scipy.interpolate.interp1d` to
-    build the CDF
-    """
-    # pylint: disable=protected-access
-
-    name = 'quant_piecewise'
-    version = 0
-
-    _support_mask = rv_continuous._support_mask
-
-    def __init__(self, quants, locs, *args, **kwargs):
-        """
-        Create a new distribution using the given values
-
-        Parameters
-        ----------
-        quants : array_like
-           The quantiles used to build the CDF
-        locs : array_like
-           The locations at which those quantiles are reached
-        """
-        kwargs['shape'] = locs.shape[:-1]
-        self._xmin = np.min(locs)
-        self._xmax = np.max(locs)
-
-        super(quant_piecewise_gen, self).__init__(*args, **kwargs)
-
-        check_input = kwargs.pop('check_input', True)
-        locs_2d = reshape_to_pdf_size(locs, -1)
-        if check_input:
-            quants, locs_2d = pad_quantiles(quants, locs_2d)
-
-        self._quants = np.asarray(quants)
-        self._nquants = self._quants.size
-        if locs_2d.shape[-1] != self._nquants:  # pragma: no cover
-            raise ValueError("Number of locations (%i) != number of quantile values (%i)" % (self._nquants, locs_2d.shape[-1]))
-        self._locs = locs_2d
-        self._valatloc = None
-        self._addmetadata('quants', self._quants)
-        self._addobjdata('locs', self._locs)
-
-
-    def _compute_valatloc(self):
-        self._valatloc = (self._quants[1:] - self._quants[0:-1])/(self._locs[:,1:] - self._locs[:,0:-1])
-
-
-    @property
-    def quants(self):
-        """Return quantiles used to build the CDF"""
-        return self._quants
-
-    @property
-    def locs(self):
-        """Return the locations at which those quantiles are reached"""
-        return self._locs
-
-    def _pdf(self, x, row):
-        # pylint: disable=arguments-differ
-        if self._valatloc is None:  # pragma: no cover
-            self._compute_valatloc()
-        return evaluate_hist_multi_x_multi_y(x, row, self._locs, self._valatloc).ravel()
-
-
-    def _cdf(self, x, row):
-        # pylint: disable=arguments-differ
-        return interpolate_multi_x_y(x, row, self._locs, self._quants,
-                                     bounds_error=False, fill_value=(0., 1)).ravel()
-
-    def _ppf(self, x, row):
-        # pylint: disable=arguments-differ
-        return interpolate_x_multi_y(x, row, self._quants, self._locs,
-                                     bounds_error=False, fill_value=(self._xmin, self._xmax)).ravel()
-
-
-    def _updated_ctor_param(self):
-        """
-        Set the bins as additional construstor argument
-        """
-        dct = super(quant_piecewise_gen, self)._updated_ctor_param()
-        dct['quants'] = self._quants
-        dct['locs'] = self._locs
-        return dct
-
-    @classmethod
-    def get_allocation_kwds(cls, npdf, **kwargs):
-        """Return kwds necessary to create 'empty' hdf5 file with npdf entries
-        for iterative writeout
-        """
-        try:
-            quants = kwargs['quants']
-        except ValueError: #pragma: no cover
-            print("required argument 'quants' not included in kwargs")
-        nquants = np.shape(quants)[-1]
-        return dict(locs=((npdf, nquants), 'f4'))
-
-    @classmethod
-    def plot_native(cls, pdf, **kwargs):
-        """Plot the PDF in a way that is particular to this type of distibution
-
-        For a quantile this shows the quantiles points
-        """
-        axes, xlim, kw = get_axes_and_xlims(**kwargs)
-        xvals = np.linspace(xlim[0], xlim[1], kw.pop('npts', 101))
-        locs = np.squeeze(pdf.dist.locs[pdf.kwds['row']])
-        quants = np.squeeze(pdf.dist.quants)
-        yvals = np.squeeze(pdf.pdf(xvals))
-        return plot_pdf_quantiles_on_axes(axes, xvals, yvals, quantiles=(quants, locs), **kw)
-
-    @classmethod
-    def add_mappings(cls):
-        """
-        Add this classes mappings to the conversion dictionary
-        """
-        cls._add_creation_method(cls.create, None)
-        cls._add_extraction_method(extract_quantiles, None)
-
-    @classmethod
-    def make_test_data(cls):
-        """ Make data for unit tests """
-        cls.test_data = dict(quant_piecewise=dict(gen_func=quant_piecewise, ctor_data=dict(quants=QUANTS, locs=QLOCS),\
-                                                  convert_data=dict(quants=QUANTS), test_xvals=TEST_XVALS))
-
-quant_piecewise = quant_piecewise_gen.create
-
-add_class(quant_piecewise_gen)
```

### Comparing `qp-prob-0.7.1/src/qp/scipy_pdfs.py` & `qp-prob-0.8.0/src/qp/scipy_pdfs.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/src/qp/sparse_pdf.py` & `qp-prob-0.8.0/src/qp/sparse_pdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,41 +47,40 @@
         #normalize and sum the weighted pdfs
         x = sparse_meta['xvals']
         y = pdf_y.sum(axis=-1)
         norms = sciint.trapz(y.T, x)
         y /= norms
         kwargs.setdefault('xvals', x)
         kwargs.setdefault('yvals', y.T)
-        super(sparse_gen, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
         self._clearobjdata()
         self._addmetadata('xvals', self._xvals)
         self._addmetadata('mu', self.mu)
         self._addmetadata('sig', self.sig)
         self._addmetadata('dims', self.dims)
         self._addobjdata('sparse_indices', self.sparse_indices)
 
     def _updated_ctor_param(self):
         """
         Add the two constructor's arguments for the Factory
         """
-        dct = super(sparse_gen, self)._updated_ctor_param()
+        dct = super()._updated_ctor_param()
         dct['sparse_indices'] = self.sparse_indices
         dct['xvals'] = self._xvals
         dct['mu'] = self.mu
         dct['sig'] = self.sig
         dct['dims'] = self.dims
         return dct
 
     @classmethod
     def get_allocation_kwds(cls, npdf, **kwargs):
         if 'dims' not in kwargs:
             raise ValueError("required argument dims not in kwargs") #pragma: no cover
         nsp = np.array(kwargs['dims']).flatten()[4]
-        nmu = np.array(kwargs['dims']).flatten()[0]
         return dict(sparse_indices=((npdf, nsp), 'i8'))
 
     @classmethod
     def add_mappings(cls):
         """
         Add this classes mappings to the conversion dictionary
         """
```

### Comparing `qp-prob-0.7.1/src/qp/sparse_rep.py` & `qp-prob-0.8.0/src/qp/sparse_rep.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,18 +73,20 @@
 def sparse_basis(dictionary, query_vec, n_basis, tolerance=None):
     """
     Compute sparse representation of a vector given Dictionary  (basis)
     for a given tolerance or number of basis. It uses Cholesky decomposition to speed the process and to
     solve the linear operations adapted from Rubinstein, R., Zibulevsky, M. and Elad, M., Technical Report - CS
     Technion, April 2008
 
-    :param float dictionary: Array with all basis on each column, must has shape (len(vector), total basis) and each column must have euclidean l-2 norm equal to 1
+    :param float dictionary: Array with all basis on each column, 
+           must has shape (len(vector), total basis) and each column must have euclidean l-2 norm equal to 1
     :param float query_vec: vector of which a sparse representation is desired
     :param int n_basis: number of desired basis
-    :param float tolerance: tolerance desired if n_basis is not needed to be fixed, must input a large number for n_basis to assure achieving tolerance
+    :param float tolerance: tolerance desired if n_basis is not needed to be fixed, must input a large number 
+           for n_basis to assure achieving tolerance
 
     :return: indices, values (2 arrays one with the position and the second with the coefficients)
     """
 
     a_n = np.zeros(dictionary.shape[1])
     machine_eps = np.finfo(dictionary.dtype).eps
     alpha = np.dot(dictionary.T, query_vec)
```

### Comparing `qp-prob-0.7.1/src/qp/spline_pdf.py` & `qp-prob-0.8.0/src/qp/spline_pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     Returns
     -------
     ynorm: array-like
         Normalized y-vals
     """
 
     def row_integral(irow):
-        spl = lambda xv : splev(xv, splrep(xvals[irow], yvals[irow]))
+        def spl(xv):
+            return splev(xv, splrep(xvals[irow], yvals[irow]))
         return quad(spl, limits[0], limits[1], **kwargs)[0]
 
     vv = np.vectorize(row_integral)
     with errstate(all='ignore'):
         integrals = vv(np.arange(xvals.shape[0]))
     return (yvals.T / integrals).T
 
@@ -140,15 +141,15 @@
         #kwargs['b'] = self.b = np.max(splx)
         self._xmin = np.min(splx)
         self._xmax = np.max(splx)
         kwargs['shape'] = splx.shape[:-1]
         self._splx = reshape_to_pdf_size(splx, -1)
         self._sply = reshape_to_pdf_size(sply, -1)
         self._spln = reshape_to_pdf_size(spln, -1)
-        super(spline_gen, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._addobjdata('splx', self._splx)
         self._addobjdata('sply', self._sply)
         self._addobjdata('spln', self._spln)
 
 
     @staticmethod
     def build_normed_splines(xvals, yvals, **kwargs):
@@ -258,15 +259,15 @@
             vv = np.vectorize(cdf_row)
         return vv(x, row).ravel()
 
     def _updated_ctor_param(self):
         """
         Set the bins as additional constructor argument
         """
-        dct = super(spline_gen, self)._updated_ctor_param()
+        dct = super()._updated_ctor_param()
         dct['splx'] = self._splx
         dct['sply'] = self._sply
         dct['spln'] = self._spln
         return dct
 
     @classmethod
     def get_allocation_kwds(cls, npdf, **kwargs):
```

### Comparing `qp-prob-0.7.1/src/qp/test_data.py` & `qp-prob-0.8.0/src/qp/test_data.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/src/qp/test_funcs.py` & `qp-prob-0.8.0/src/qp/test_funcs.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/src/qp/utils.py` & `qp-prob-0.8.0/src/qp/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Utility functions for the qp package"""
 
+import sys
 import numpy as np
 
 from scipy import stats as sps
 from scipy.interpolate import interp1d
-import sys
 
 epsilon = sys.float_info.epsilon
 infty = sys.float_info.max * epsilon
 lims = (epsilon, 1.)
 
 CASE_PRODUCT = 0
 CASE_FACTOR = 1
@@ -177,16 +177,16 @@
     rr : array_like
         The y-values, properly shaped
 
     Notes
     -----
     The cases are:
 
-    CASE_FLAT : x, row have shapes (n) , (n) and do not factor
-    CASE_FACTOR : x, row can be factors to shapes (1, nx) and (npdf, 1)
+    CASE_FLAT : x, row have shapes (n), (n) and do not factor
+    CASE_FACTOR : x, row have shapes (n), (n) but can be factored to shapes (1, nx) and (npdf, 1) (i.e., they were flattend by scipy) 
     CASE_PRODUCT : x, row have shapes (1, nx) and (npdf, 1)
     CASE_2D : x, row have shapes (npdf, nx) and (npdf, nx)
     """
     nd_x = np.ndim(x)
     nd_row = np.ndim(row)
     #if nd_x > 2 or nd_row > 2:  #pragma: no cover
     #    raise ValueError("Too many dimensions: x(%s), row(%s)" % (np.shape(x), np.shape(row)))
```

### Comparing `qp-prob-0.7.1/src/qp_prob.egg-info/PKG-INFO` & `qp-prob-0.8.0/src/qp_prob.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qp-prob
-Version: 0.7.1
+Version: 0.8.0
 License: MIT License
         
         Copyright (c) 2016 Alex Malz & Phil Marshall
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `qp-prob-0.7.1/tests/qp/.gitignore` & `qp-prob-0.8.0/tests/qp/.gitignore`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/tests/qp/benchmark.py` & `qp-prob-0.8.0/tests/qp/benchmark.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/tests/qp/fidelity.py` & `qp-prob-0.8.0/tests/qp/fidelity.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/tests/qp/test_auto.py` & `qp-prob-0.8.0/tests/qp/test_auto.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/tests/qp/test_brier.py` & `qp-prob-0.8.0/tests/qp/test_brier.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/tests/qp/test_ensemble.py` & `qp-prob-0.8.0/tests/qp/test_ensemble.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Unit tests for PDF class
 """
 import copy
+import logging
 import numpy as np
 import unittest
 import qp
 from qp import test_data
 import os
 import sys
 
 from qp.test_funcs import assert_all_small, assert_all_close, build_ensemble
 from qp.plotting import init_matplotlib
+from qp.quantile_pdf_constructors import AbstractQuantilePdfConstructor
 
 
 class EnsembleTestCase(unittest.TestCase):
     """ Class to test qp.Ensemble functionality """
 
     def setUp(self):
         """
@@ -183,22 +185,74 @@
         key = 'interp'
         qp.interp_gen.make_test_data()
         cls_test_data = qp.interp_gen.test_data[key]
         ens_i = build_ensemble(cls_test_data)
         assert isinstance(ens_i.gen_obj, qp.interp_gen)
         self._run_ensemble_funcs(ens_i, cls_test_data['test_xvals'])
 
+    def test_packed_interp(self):
+        """ Run the ensemble tests on an ensemble of qp.packed_interp distributions """
+        key = 'lin_packed_interp'
+        qp.packed_interp_gen.make_test_data()
+        cls_test_data = qp.packed_interp_gen.test_data[key]
+        ens_i = build_ensemble(cls_test_data)
+        assert isinstance(ens_i.gen_obj, qp.packed_interp_gen)
+        self._run_ensemble_funcs(ens_i, cls_test_data['test_xvals'])
+        assert np.isfinite(ens_i.dist.yvals).all()
+
     def test_iterator(self):
         """ Test the iterated read """
         QP_DIR = os.path.abspath(os.path.dirname(qp.__file__))
         data_file = os.path.join(QP_DIR, 'data', 'test.hdf5')
         ens = qp.read(data_file)
+        data_length = qp.data_length(data_file)
+        assert data_length == ens.npdf
         itr = qp.iterator(data_file, 10)
         test_grid = np.linspace(0., 1., 11)
         for start, end, ens_i in itr:
             check_vals = ens[start:end].pdf(test_grid)
             test_vals = ens_i.pdf(test_grid)
             assert np.allclose(check_vals, test_vals)
 
+    def test_quant_get_default_pdf_constructor_name(self):
+        """Test that the getter for pdf constructor name works"""
+        quantiles = np.linspace(0.001, 0.999, 16)
+        locations = np.linspace(0, 5, 16)
+        quant_dist = qp.quant(quants=quantiles, locs=locations)
+        self.assertEqual(quant_dist.dist.pdf_constructor_name, 'piecewise_linear')
+
+    def test_quant_get_default_pdf_constructor(self):
+        """Test that the getter for pdf constructor returns an AbstractQuantilePdfConstructor"""
+        quantiles = np.linspace(0.001, 0.999, 16)
+        locations = np.linspace(0, 5, 16)
+        quant_dist = qp.quant(quants=quantiles, locs=locations)
+        assert isinstance(quant_dist.dist.pdf_constructor, AbstractQuantilePdfConstructor)
+
+    def test_quant_change_pdf_constructor(self):
+        """Test that changing the pdf constructor works as expected"""
+        quantiles = np.linspace(0.001, 0.999, 16)
+        locations = np.linspace(0, 5, 16)
+        quant_dist = qp.quant(quants=quantiles, locs=locations)
+        quant_dist.dist.pdf_constructor_name = 'piecewise_constant'
+        self.assertEqual(quant_dist.dist.pdf_constructor_name, 'piecewise_constant')
+
+    def test_quant_change_pdf_constructor_raises(self):
+        """Verify that attempting to change the pdf constructor to one that
+        isn't in the dictionary, will raise an error."""
+        quantiles = np.linspace(0.001, 0.999, 16)
+        locations = np.linspace(0, 5, 16)
+        quant_dist = qp.quant(quants=quantiles, locs=locations)
+        with self.assertRaises(ValueError):
+            quant_dist.dist.pdf_constructor_name = 'drewtonian'
+
+    def test_quant_change_pdf_constructor_warns(self):
+        """Verify that attempting to change the pdf constructor to the one
+        currently being used will log a warning."""
+        quantiles = np.linspace(0.001, 0.999, 16)
+        locations = np.linspace(0, 5, 16)
+        quant_dist = qp.quant(quants=quantiles, locs=locations)
+        with self.assertLogs(level=logging.WARNING) as log:
+            quant_dist.dist.pdf_constructor_name = 'piecewise_linear'
+            self.assertIn('Already using', log.output[0])
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `qp-prob-0.7.1/tests/qp/test_eval_funcs.py` & `qp-prob-0.8.0/tests/qp/test_eval_funcs.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/tests/qp/test_flex_coefs.npy` & `qp-prob-0.8.0/tests/qp/test_flex_coefs.npy`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/tests/qp/test_infrastructure.py` & `qp-prob-0.8.0/tests/qp/test_infrastructure.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/tests/qp/test_metrics.py` & `qp-prob-0.8.0/tests/qp/test_metrics.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import qp
 import qp.metrics
 import numpy as np
 
 from qp import test_funcs
 from qp.metrics.metrics import * 
 from qp.utils import epsilon
-
+from scipy import stats
 
 class MetricTestCase(unittest.TestCase):
     """ Tests for the metrics """
 
     def setUp(self):
         """
         Make any objects that are used in multiple tests.
@@ -82,16 +82,16 @@
 
         ens_i = self.ens_n[0].convert_to(qp.interp_gen, xvals=bins)
         ens_i_shift = self.ens_n_shift[0].convert_to(qp.interp_gen, xvals=bins)
 
         ens_s = self.ens_n[0].convert_to(qp.spline_gen, xvals=bins, method="xy")
         ens_s_shift = self.ens_n_shift[0].convert_to(qp.spline_gen, xvals=bins, method="xy")
 
-        ens_q = self.ens_n[0].convert_to(qp.quant_piecewise_gen, quants=quants)
-        ens_q_shift = self.ens_n_shift[0].convert_to(qp.quant_piecewise_gen, quants=quants)
+        ens_q = self.ens_n[0].convert_to(qp.quant_gen, quants=quants)
+        ens_q_shift = self.ens_n_shift[0].convert_to(qp.quant_gen, quants=quants)
 
         kld_histogram = qp.metrics.calculate_kld(ens_h, ens_h_shift, limits=(0.,2.5))
         assert np.all(kld_histogram == 0.)
 
         kld_interp = qp.metrics.calculate_kld(ens_i, ens_i_shift, limits=(0.,2.5))
         assert np.all(kld_interp == 0.)
 
@@ -130,16 +130,16 @@
 
         ens_i = self.ens_n[0].convert_to(qp.interp_gen, xvals=bins)
         ens_i_shift = self.ens_n_shift[0].convert_to(qp.interp_gen, xvals=bins)
 
         ens_s = self.ens_n[0].convert_to(qp.spline_gen, xvals=bins, method="xy")
         ens_s_shift = self.ens_n_shift[0].convert_to(qp.spline_gen, xvals=bins, method="xy")
 
-        ens_q = self.ens_n[0].convert_to(qp.quant_piecewise_gen, quants=quants)
-        ens_q_shift = self.ens_n_shift[0].convert_to(qp.quant_piecewise_gen, quants=quants)
+        ens_q = self.ens_n[0].convert_to(qp.quant_gen, quants=quants)
+        ens_q_shift = self.ens_n_shift[0].convert_to(qp.quant_gen, quants=quants)
 
         rmse_histogram = qp.metrics.calculate_rmse(ens_h, ens_h_shift, limits=(0.,2.5))
         assert np.all(rmse_histogram == 0.)
 
         rmse_interp = qp.metrics.calculate_rmse(ens_i, ens_i_shift, limits=(0.,2.5))
         assert np.all(rmse_interp == 0.)
 
@@ -171,15 +171,15 @@
         """ Test the risk_based_point_estimate method against different types of ensembles """
         bins = np.linspace(-5, 5, 11)
         quants = np.linspace(0.01, 0.99, 7)
 
         ens_h = self.ens_n[0].convert_to(qp.hist_gen, bins=bins)
         ens_i = self.ens_n[0].convert_to(qp.interp_gen, xvals=bins)
         ens_s = self.ens_n[0].convert_to(qp.spline_gen, xvals=bins, method="xy")
-        ens_q = self.ens_n[0].convert_to(qp.quant_piecewise_gen, quants=quants)
+        ens_q = self.ens_n[0].convert_to(qp.quant_gen, quants=quants)
         ens_m = self.ens_n[0].convert_to(qp.mixmod_gen, samples=1000, ncomps=3)
 
         rbpe_histogram = qp.metrics.calculate_rbpe(ens_h, limits=(0.,2.5))
         assert np.all(rbpe_histogram >= 0.)
         assert np.all(rbpe_histogram <= 2.5)
 
         rbpe_interp = qp.metrics.calculate_rbpe(ens_i, limits=(0.,2.5))
@@ -265,29 +265,14 @@
         self.assertTrue(np.isclose(output[0], 0))
 
     def test_calculate_outlier_rate_many_distributions(self):
         """Check that the outlier rate is correctly calculated for an Ensemble with many distributions"""
         output = qp.metrics.calculate_outlier_rate(self.ens_n)
         self.assertTrue(len(output) == 11)
 
-    def test_calculate_kolmogorov_smirnov(self):
-        """Bare minimum test to ensure that the data is flowing correctly"""
-        output = qp.metrics.calculate_kolmogorov_smirnov(self.ens_n, self.ens_n)
-        self.assertTrue(len(output) == self.ens_n.npdf)
-
-    def test_calculate_cramer_von_mises(self):
-        """Bare minimum test to ensure that the data is flowing correctly"""
-        output = qp.metrics.calculate_cramer_von_mises(self.ens_n, self.ens_n)
-        self.assertTrue(len(output) == self.ens_n.npdf)
-
-    def test_calculate_anderson_darling(self):
-        """Bare minimum test to ensure that the data is flowing correctly"""
-        output = qp.metrics.calculate_anderson_darling(self.ens_n, 'norm')
-        self.assertTrue(len(output) == self.ens_n.npdf)
-
     def test_check_ensembles_are_same_size(self):
         """Test that no Value Error is raised when the ensembles are the same size"""
         try:
             qp.metrics._check_ensembles_are_same_size(self.ens_n, self.ens_n_shift)  #pylint: disable=W0212
         except ValueError:
             self.fail("Unexpectedly raised ValueError")
 
@@ -310,9 +295,46 @@
         """Test that a ValueError is raised when a nested Ensemble is passed in"""
         with self.assertRaises(ValueError) as context:
             qp.metrics._check_ensemble_is_not_nested(self.ens_n_multi)  #pylint: disable=W0212
 
         error_msg = "Each element in the input Ensemble should be a single distribution."
         self.assertTrue(error_msg in str(context.exception))
 
+    def test_check_ensembles_contain_correct_number_of_distributions_base(self):
+        """Test base case of two ensembles the same size"""
+        try:
+            qp.metrics._check_ensembles_contain_correct_number_of_distributions(estimate=self.ens_n, reference=self.ens_n)
+        except ValueError:
+            self.fail("Unexpectedly raised ValueError")
+
+    def test_check_ensembles_contain_correct_number_of_distributions_both_size_1(self):
+        """Test base case of two ensembles with 1 distribution each"""
+        try:
+            qp.metrics._check_ensembles_contain_correct_number_of_distributions(estimate=self.ens_n[0], reference=self.ens_n[1])
+        except ValueError:
+            self.fail("Unexpected raised ValueError")
+
+    def test_check_ensembles_contain_correct_number_of_distributions_reference_has_1(self):
+        """Test case of reference ensemble has 1 distribution, estimate has N"""
+        try:
+            qp.metrics._check_ensembles_contain_correct_number_of_distributions(estimate=self.ens_n, reference=self.ens_n[1])
+        except ValueError:
+            self.fail("Unexpected raised ValueError")
+
+    def test_check_ensembles_contain_correct_number_of_distributions_with_different_sizes(self):
+        """Test the case of reference with M distributions, and estimate with N distributions"""
+        with self.assertRaises(ValueError) as context:
+            qp.metrics._check_ensembles_contain_correct_number_of_distributions(estimate=self.ens_n, reference=self.ens_n_plus_one)
+
+        error_msg = "`reference` should contain either"
+        self.assertTrue(error_msg in str(context.exception))
+
+    def test_calculate_goodness_of_fit_with_unsupported_fit_metric(self):
+        """Test that a KeyError is raised if an unsupported fit_metric is requested"""
+        with self.assertRaises(KeyError) as context:
+            qp.metrics.calculate_goodness_of_fit(self.ens_n, self.ens_n, 'xx')
+
+        error_msg = "`fit_metric` should be one of"
+        self.assertTrue(error_msg in str(context.exception))
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `qp-prob-0.7.1/tests/qp/test_parallel.py` & `qp-prob-0.8.0/tests/qp/test_parallel.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/tests/qp/test_pit.py` & `qp-prob-0.8.0/tests/qp/test_pit.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.7.1/tests/qp/test_utils.py` & `qp-prob-0.8.0/tests/qp/test_utils.py`

 * *Files identical despite different names*

