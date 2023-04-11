# Comparing `tmp/causal_testing_framework-3.1.0.tar.gz` & `tmp/causal_testing_framework-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causal_testing_framework-3.1.0.tar", last modified: Thu Mar 23 16:26:52 2023, max compression
+gzip compressed data, was "causal_testing_framework-3.2.0.tar", last modified: Tue Apr 11 10:17:13 2023, max compression
```

## Comparing `causal_testing_framework-3.1.0.tar` & `causal_testing_framework-3.2.0.tar`

### file list

```diff
@@ -1,155 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.509918 causal_testing_framework-3.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.493917 causal_testing_framework-3.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.493917 causal_testing_framework-3.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.493917 causal_testing_framework-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/.github/workflows/ci-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/.github/workflows/lint-format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/.mega-linter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-03-23 16:26:52.509918 causal_testing_framework-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.493917 causal_testing_framework-3.1.0/causal_testing/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.493917 causal_testing_framework-3.1.0/causal_testing/data_collection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/data_collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/data_collection/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.493917 causal_testing_framework-3.1.0/causal_testing/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/generation/abstract_causal_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.493917 causal_testing_framework-3.1.0/causal_testing/json_front/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/json_front/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/json_front/json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.493917 causal_testing_framework-3.1.0/causal_testing/specification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26401 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/specification/causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/specification/causal_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/specification/metamorphic_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/specification/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/specification/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.497917 causal_testing_framework-3.1.0/causal_testing/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/testing/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/testing/causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13167 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/testing/causal_test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/testing/causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/testing/causal_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/testing/causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/testing/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    30574 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/testing/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/testing/intervention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/causal_testing/testing/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.497917 causal_testing_framework-3.1.0/causal_testing_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-03-23 16:26:52.000000 causal_testing_framework-3.1.0/causal_testing_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-03-23 16:26:52.000000 causal_testing_framework-3.1.0/causal_testing_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 16:26:52.000000 causal_testing_framework-3.1.0/causal_testing_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-23 16:26:52.000000 causal_testing_framework-3.1.0/causal_testing_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-23 16:26:52.000000 causal_testing_framework-3.1.0/causal_testing_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.497917 causal_testing_framework-3.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.497917 causal_testing_framework-3.1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/source/description.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.497917 causal_testing_framework-3.1.0/docs/source/frontends/
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/source/frontends/json_front_end.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/source/frontends/test_suite.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/source/glossary.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.497917 causal_testing_framework-3.1.0/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/source/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.497917 causal_testing_framework-3.1.0/docs/source/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/source/modules/causal_specification.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/source/modules/causal_tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/source/modules/data_collector.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/source/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.497917 causal_testing_framework-3.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.489917 causal_testing_framework-3.1.0/examples/covasim_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.501917 causal_testing_framework-3.1.0/examples/covasim_/doubling_beta/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/covasim_/doubling_beta/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/covasim_/doubling_beta/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/covasim_/doubling_beta/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.501917 causal_testing_framework-3.1.0/examples/covasim_/doubling_beta/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1355776 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    16444 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/covasim_/doubling_beta/example_beta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.501917 causal_testing_framework-3.1.0/examples/covasim_/vaccinating_elderly/
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/covasim_/vaccinating_elderly/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/covasim_/vaccinating_elderly/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/covasim_/vaccinating_elderly/dag.png
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/covasim_/vaccinating_elderly/example_vaccine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.501917 causal_testing_framework-3.1.0/examples/lr91/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/lr91/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/lr91/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    73886 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/lr91/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.501917 causal_testing_framework-3.1.0/examples/lr91/data/
--rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/lr91/data/normalised_results.csv
--rw-r--r--   0 runner    (1001) docker     (123)    40686 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/lr91/data/results.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/lr91/example_max_conductances.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/lr91/example_max_conductances_test_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.501917 causal_testing_framework-3.1.0/examples/poisson/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson/causal_tests.json
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson/example_run_causal_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.505917 causal_testing_framework-3.1.0/examples/poisson-line-process/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    53765 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.489917 causal_testing_framework-3.1.0/examples/poisson-line-process/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.505917 causal_testing_framework-3.1.0/examples/poisson-line-process/data/random/
--rw-r--r--   0 runner    (1001) docker     (123)   102007 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/data/random/data_random_1000.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.505917 causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14925 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/examples/poisson-line-process/example_poisson_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.505917 causal_testing_framework-3.1.0/images/
--rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 16:26:52.509918 causal_testing_framework-3.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.505917 causal_testing_framework-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.505917 causal_testing_framework-3.1.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   374288 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/data/nhefs.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.505917 causal_testing_framework-3.1.0/tests/data_collection_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/data_collection_tests/test_observational_data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.505917 causal_testing_framework-3.1.0/tests/generation_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/generation_tests/test_abstract_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.505917 causal_testing_framework-3.1.0/tests/json_front_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/json_front_tests/test_json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.493917 causal_testing_framework-3.1.0/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.505917 causal_testing_framework-3.1.0/tests/resources/data/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/resources/data/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/resources/data/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/resources/data/tests.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.509918 causal_testing_framework-3.1.0/tests/specification_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/specification_tests/test_causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/specification_tests/test_metamorphic_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/specification_tests/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:26:52.509918 causal_testing_framework-3.1.0/tests/testing_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/testing_tests/test_causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/testing_tests/test_causal_test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/testing_tests/test_causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/testing_tests/test_causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-03-23 16:26:04.000000 causal_testing_framework-3.1.0/tests/testing_tests/test_estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.784882 causal_testing_framework-3.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.756882 causal_testing_framework-3.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.756882 causal_testing_framework-3.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.756882 causal_testing_framework-3.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.github/workflows/ci-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.github/workflows/lint-format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.mega-linter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-11 10:17:13.784882 causal_testing_framework-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.760882 causal_testing_framework-3.2.0/causal_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.760882 causal_testing_framework-3.2.0/causal_testing/data_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/data_collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/data_collection/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.760882 causal_testing_framework-3.2.0/causal_testing/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/generation/abstract_causal_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.760882 causal_testing_framework-3.2.0/causal_testing/json_front/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/json_front/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14630 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/json_front/json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.760882 causal_testing_framework-3.2.0/causal_testing/specification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26479 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/specification/causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/specification/causal_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/specification/metamorphic_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/specification/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/specification/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.764882 causal_testing_framework-3.2.0/causal_testing/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13167 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/causal_test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/causal_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30688 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/intervention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.764882 causal_testing_framework-3.2.0/causal_testing_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-11 10:17:13.000000 causal_testing_framework-3.2.0/causal_testing_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-11 10:17:13.000000 causal_testing_framework-3.2.0/causal_testing_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:17:13.000000 causal_testing_framework-3.2.0/causal_testing_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-11 10:17:13.000000 causal_testing_framework-3.2.0/causal_testing_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 10:17:13.000000 causal_testing_framework-3.2.0/causal_testing_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.764882 causal_testing_framework-3.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.768882 causal_testing_framework-3.2.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/description.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.768882 causal_testing_framework-3.2.0/docs/source/frontends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/frontends/json_front_end.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/frontends/test_suite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/glossary.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.768882 causal_testing_framework-3.2.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/images/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.768882 causal_testing_framework-3.2.0/docs/source/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/modules/causal_specification.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/modules/causal_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/modules/data_collector.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.768882 causal_testing_framework-3.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.752882 causal_testing_framework-3.2.0/examples/covasim_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.768882 causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.768882 causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1355776 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    16444 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/example_beta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.772882 causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/dag.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/example_vaccine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.772882 causal_testing_framework-3.2.0/examples/lr91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/lr91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/lr91/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    73886 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/lr91/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.772882 causal_testing_framework-3.2.0/examples/lr91/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/lr91/data/normalised_results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40686 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/lr91/data/results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/lr91/example_max_conductances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/lr91/example_max_conductances_test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.776882 causal_testing_framework-3.2.0/examples/poisson/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson/causal_tests.json
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson/example_run_causal_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.776882 causal_testing_framework-3.2.0/examples/poisson-line-process/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    53765 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.752882 causal_testing_framework-3.2.0/examples/poisson-line-process/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.776882 causal_testing_framework-3.2.0/examples/poisson-line-process/data/random/
+-rw-r--r--   0 runner    (1001) docker     (123)   102007 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/random/data_random_1000.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.776882 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14925 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/example_poisson_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.780882 causal_testing_framework-3.2.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/images/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:17:13.784882 causal_testing_framework-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.780882 causal_testing_framework-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.780882 causal_testing_framework-3.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   374288 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/data/nhefs.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.780882 causal_testing_framework-3.2.0/tests/data_collection_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/data_collection_tests/test_observational_data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.780882 causal_testing_framework-3.2.0/tests/generation_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/generation_tests/test_abstract_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.780882 causal_testing_framework-3.2.0/tests/json_front_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/json_front_tests/test_json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.752882 causal_testing_framework-3.2.0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.784882 causal_testing_framework-3.2.0/tests/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/resources/data/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/resources/data/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/resources/data/data_with_meta.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/resources/data/tests.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.784882 causal_testing_framework-3.2.0/tests/specification_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/specification_tests/test_causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/specification_tests/test_metamorphic_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/specification_tests/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.784882 causal_testing_framework-3.2.0/tests/testing_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/testing_tests/test_estimators.py
```

### Comparing `causal_testing_framework-3.1.0/.github/CONTRIBUTING.md` & `causal_testing_framework-3.2.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `causal_testing_framework-3.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `causal_testing_framework-3.2.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/.github/workflows/ci-tests.yaml` & `causal_testing_framework-3.2.0/.github/workflows/ci-tests.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/.github/workflows/lint-format.yaml` & `causal_testing_framework-3.2.0/.github/workflows/lint-format.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/.github/workflows/publish-to-pypi.yaml` & `causal_testing_framework-3.2.0/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/.gitignore` & `causal_testing_framework-3.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/.pylintrc` & `causal_testing_framework-3.2.0/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 # Control the amount of potential inferred values when inferring a single
 # object. This can help the performance when dealing with large functions or
 # complex, nested conditions.
 limit-inference-results=100
 
 # List of plugins (as comma separated values of python module names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.docparams
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Minimum Python version to use for version dependent checks. Will default to
 # the version used to run pylint.
 py-version=3.9
```

### Comparing `causal_testing_framework-3.1.0/.readthedocs.yaml` & `causal_testing_framework-3.2.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/LICENSE` & `causal_testing_framework-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/PKG-INFO` & `causal_testing_framework-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal_testing_framework
-Version: 3.1.0
+Version: 3.2.0
 Summary: A framework for causal testing using causal directed acyclic graphs.
 Author: The CITCOM team
 License: MIT
 Project-URL: Bug_Tracker, https://github.com/CITCOM-project/CausalTestingFramework/issues
 Project-URL: Documentation, https://causal-testing-framework.readthedocs.io/
 Project-URL: Source, https://github.com/CITCOM-project/CausalTestingFramework
 Keywords: causal inference,verification
```

### Comparing `causal_testing_framework-3.1.0/README.md` & `causal_testing_framework-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/causal_testing/data_collection/data_collector.py` & `causal_testing_framework-3.2.0/causal_testing/data_collection/data_collector.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/causal_testing/generation/abstract_causal_test_case.py` & `causal_testing_framework-3.2.0/causal_testing/generation/abstract_causal_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/causal_testing/json_front/json_class.py` & `causal_testing_framework-3.2.0/causal_testing/json_front/json_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """This module contains the JsonUtility class, details of using this class can be found here:
 https://causal-testing-framework.readthedocs.io/en/latest/json_front_end.html"""
 
 import argparse
 import json
 import logging
 
-from abc import ABC
 from dataclasses import dataclass
 from pathlib import Path
+from statistics import StatisticsError
 
 import pandas as pd
 import scipy
 from fitter import Fitter, get_common_distributions
 
 from causal_testing.data_collection.data_collector import ObservationalDataCollector
 from causal_testing.generation.abstract_causal_test_case import AbstractCausalTestCase
@@ -22,15 +22,15 @@
 from causal_testing.testing.causal_test_case import CausalTestCase
 from causal_testing.testing.causal_test_engine import CausalTestEngine
 from causal_testing.testing.estimators import Estimator
 
 logger = logging.getLogger(__name__)
 
 
-class JsonUtility(ABC):
+class JsonUtility:
     """
     The JsonUtility Class provides the functionality to use structured JSON to setup and run causal tests on the
     CausalTestingFramework.
 
     :attr {Path} json_path: Path to the JSON input file.
     :attr {Path} dag_path: Path to the dag.dot file containing the Causal DAG.
     :attr {Path} data_path: Path to the csv data file.
@@ -39,62 +39,54 @@
     :attr {Meta} metas: Causal variables representing metavariables.
     :attr {pd.DataFrame}: Pandas DataFrame containing runtime data.
     :attr {dict} test_plan: Dictionary containing the key value pairs from the loaded json test plan.
     :attr {Scenario} modelling_scenario:
     :attr {CausalSpecification} causal_specification:
     """
 
-    def __init__(self, log_path):
-        self.paths = None
+    def __init__(self, output_path: str, output_overwrite: bool = False):
+        self.input_paths = None
         self.variables = None
         self.data = []
         self.test_plan = None
-        self.modelling_scenario = None
+        self.scenario = None
         self.causal_specification = None
-        self.setup_logger(log_path)
+        self.output_path = Path(output_path)
+        self.check_file_exists(self.output_path, output_overwrite)
 
     def set_paths(self, json_path: str, dag_path: str, data_paths: str):
         """
         Takes a path of the directory containing all scenario specific files and creates individual paths for each file
         :param json_path: string path representation to .json file containing test specifications
         :param dag_path: string path representation to the .dot file containing the Causal DAG
-        :param data_path: string path representation to the data file
+        :param data_paths: string path representation to the data files
         """
-        self.paths = JsonClassPaths(json_path=json_path, dag_path=dag_path, data_paths=data_paths)
+        self.input_paths = JsonClassPaths(json_path=json_path, dag_path=dag_path, data_paths=data_paths)
 
-    def set_variables(self, inputs: list[dict], outputs: list[dict], metas: list[dict]):
-        """Populate the Causal Variables
-        :param inputs:
-        :param outputs:
-        :param metas:
-        """
-
-        self.variables = CausalVariables(inputs=inputs, outputs=outputs, metas=metas)
-
-    def setup(self):
+    def setup(self, scenario: Scenario):
         """Function to populate all the necessary parts of the json_class needed to execute tests"""
-        self.modelling_scenario = Scenario(self.variables.inputs + self.variables.outputs + self.variables.metas, None)
-        self.modelling_scenario.setup_treatment_variables()
+        self.scenario = scenario
+        self.scenario.setup_treatment_variables()
         self.causal_specification = CausalSpecification(
-            scenario=self.modelling_scenario, causal_dag=CausalDAG(self.paths.dag_path)
+            scenario=self.scenario, causal_dag=CausalDAG(self.input_paths.dag_path)
         )
         self._json_parse()
         self._populate_metas()
 
     def _create_abstract_test_case(self, test, mutates, effects):
         assert len(test["mutations"]) == 1
         abstract_test = AbstractCausalTestCase(
-            scenario=self.modelling_scenario,
+            scenario=self.scenario,
             intervention_constraints=[mutates[v](k) for k, v in test["mutations"].items()],
-            treatment_variable=next(self.modelling_scenario.variables[v] for v in test["mutations"]),
+            treatment_variable=next(self.scenario.variables[v] for v in test["mutations"]),
             expected_causal_effect={
-                self.modelling_scenario.variables[variable]: effects[effect]
+                self.scenario.variables[variable]: effects[effect]
                 for variable, effect in test["expectedEffect"].items()
             },
-            effect_modifiers={self.modelling_scenario.variables[v] for v in test["effect_modifiers"]}
+            effect_modifiers={self.scenario.variables[v] for v in test["effect_modifiers"]}
             if "effect_modifiers" in test
             else {},
             estimate_type=test["estimate_type"],
             effect=test.get("effect", "total"),
         )
         return abstract_test
 
@@ -109,52 +101,55 @@
         failures = 0
         for test in self.test_plan["tests"]:
             if "skip" in test and test["skip"]:
                 continue
             abstract_test = self._create_abstract_test_case(test, mutates, effects)
 
             concrete_tests, dummy = abstract_test.generate_concrete_tests(5, 0.05)
-            logger.info("Executing test: %s", test["name"])
-            logger.info(abstract_test)
-            logger.info([abstract_test.treatment_variable.name, abstract_test.treatment_variable.distribution])
-            logger.info("Number of concrete tests for test case: %s", str(len(concrete_tests)))
             failures = self._execute_tests(concrete_tests, estimators, test, f_flag)
-            logger.info("%s/%s failed for %s\n", failures, len(concrete_tests), test["name"])
+            msg = (
+                f"Executing test: {test['name']} \n"
+                + "abstract_test \n"
+                + f"{abstract_test} \n"
+                + f"{abstract_test.treatment_variable.name},{abstract_test.treatment_variable.distribution} \n"
+                + f"Number of concrete tests for test case: {str(len(concrete_tests))} \n"
+                + f"{failures}/{len(concrete_tests)} failed for {test['name']}"
+            )
+            self._append_to_file(msg, logging.INFO)
 
     def _execute_tests(self, concrete_tests, estimators, test, f_flag):
         failures = 0
         for concrete_test in concrete_tests:
             failed = self._execute_test_case(concrete_test, estimators[test["estimator"]], f_flag)
             if failed:
                 failures += 1
         return failures
 
     def _json_parse(self):
         """Parse a JSON input file into inputs, outputs, metas and a test plan"""
-        with open(self.paths.json_path, encoding="utf-8") as f:
+        with open(self.input_paths.json_path, encoding="utf-8") as f:
             self.test_plan = json.load(f)
-        for data_file in self.paths.data_paths:
+        for data_file in self.input_paths.data_paths:
             df = pd.read_csv(data_file, header=0)
             self.data.append(df)
         self.data = pd.concat(self.data)
 
     def _populate_metas(self):
         """
         Populate data with meta-variable values and add distributions to Causal Testing Framework Variables
         """
-        for meta in self.variables.metas:
+        for meta in self.scenario.variables_of_type(Meta):
             meta.populate(self.data)
-
-        for var in self.variables.metas + self.variables.outputs:
+        for var in self.scenario.variables_of_type(Meta).union(self.scenario.variables_of_type(Output)):
             if not var.distribution:
                 fitter = Fitter(self.data[var.name], distributions=get_common_distributions())
                 fitter.fit()
                 (dist, params) = list(fitter.get_best(method="sumsquare_error").items())[0]
                 var.distribution = getattr(scipy.stats, dist)(**params)
-                logger.info(var.name + f" {dist}({params})")
+                self._append_to_file(var.name + f" {dist}({params})", logging.INFO)
 
     def _execute_test_case(self, causal_test_case: CausalTestCase, estimator: Estimator, f_flag: bool) -> bool:
         """Executes a singular test case, prints the results and returns the test case result
         :param causal_test_case: The concrete test case to be executed
         :param f_flag: Failure flag that if True the script will stop executing when a test fails.
         :return: A boolean that if True indicates the causal test case passed and if false indicates the test case
          failed.
@@ -173,33 +168,34 @@
         if causal_test_result.ci_low() and causal_test_result.ci_high():
             result_string = (
                 f"{causal_test_result.ci_low()} < {causal_test_result.test_value.value} <  "
                 f"{causal_test_result.ci_high()}"
             )
         else:
             result_string = f"{causal_test_result.test_value.value} no confidence intervals"
-        if f_flag:
-            assert test_passes, (
-                f"{causal_test_case}\n    FAILED - expected {causal_test_case.expected_causal_effect}, "
-                f"got {result_string}"
-            )
+
         if not test_passes:
+            if f_flag:
+                raise StatisticsError(
+                    f"{causal_test_case}\n    FAILED - expected {causal_test_case.expected_causal_effect}, "
+                    f"got {result_string}"
+                )
             failed = True
             logger.warning("   FAILED- expected %s, got %s", causal_test_case.expected_causal_effect, result_string)
         return failed
 
     def _setup_test(self, causal_test_case: CausalTestCase, estimator: Estimator) -> tuple[CausalTestEngine, Estimator]:
         """Create the necessary inputs for a single test case
         :param causal_test_case: The concrete test case to be executed
         :returns:
                 - causal_test_engine - Test Engine instance for the test being run
                 - estimation_model - Estimator instance for the test being run
         """
 
-        data_collector = ObservationalDataCollector(self.modelling_scenario, self.data)
+        data_collector = ObservationalDataCollector(self.scenario, self.data)
         causal_test_engine = CausalTestEngine(self.causal_specification, data_collector, index_col=0)
 
         minimal_adjustment_set = self.causal_specification.causal_dag.identification(causal_test_case.base_test_case)
         treatment_var = causal_test_case.treatment_variable
         minimal_adjustment_set = minimal_adjustment_set - {treatment_var}
         estimation_model = estimator(
             treatment=treatment_var.name,
@@ -218,23 +214,40 @@
     def add_modelling_assumptions(self, estimation_model: Estimator):  # pylint: disable=unused-argument
         """Optional abstract method where user functionality can be written to determine what assumptions are required
         for specific test cases
         :param estimation_model: estimator model instance for the current running test.
         """
         return
 
+    def _append_to_file(self, line: str, log_level: int = None):
+        """Appends given line(s) to the current output file. If log_level is specified it also logs that message to the
+        logging level.
+        :param line: The line or lines of text to be appended to the file
+        :param log_level: An integer representing the logging level as specified by pythons inbuilt logging module. It
+        is possible to use the inbuilt logging level variables such as logging.INFO and logging.WARNING
+        """
+        with open(self.output_path, "a", encoding="utf-8") as f:
+            f.write(
+                line + "\n",
+            )
+        if log_level:
+            logger.log(level=log_level, msg=line)
+
     @staticmethod
-    def setup_logger(log_path: str):
-        """Setups up logging instance for the module and adds a FileHandler stream so all stdout prints are also
-        sent to the logfile
-        :param log_path: Path specifying location and name of the logging file to be used
-        """
-        setup_log = logging.getLogger(__name__)
-        file_handler = logging.FileHandler(Path(log_path))
-        setup_log.addHandler(file_handler)
+    def check_file_exists(output_path: Path, overwrite: bool):
+        """Method that checks if the given path to an output file already exists. If overwrite is true the check is
+        passed.
+        :param output_path: File path for the output file of the JSON Frontend
+        :param overwrite: bool that if true, the current file can be overwritten
+        """
+        if output_path.is_file():
+            if overwrite:
+                output_path.unlink()
+            else:
+                raise FileExistsError(f"Chosen file output ({output_path}) already exists")
 
     @staticmethod
     def get_args(test_args=None) -> argparse.Namespace:
         """Command-line arguments
 
         :return: parsed command line arguments
         """
@@ -243,14 +256,20 @@
         )
         parser.add_argument(
             "-f",
             help="if included, the script will stop if a test fails",
             action="store_true",
         )
         parser.add_argument(
+            "-w",
+            help="Specify to overwrite any existing output files. This can lead to the loss of existing outputs if not "
+            "careful",
+            action="store_true",
+        )
+        parser.add_argument(
             "--log_path",
             help="Specify a directory to change the location of the log file",
             default="./json_frontend.log",
         )
         parser.add_argument(
             "--data_path",
             help="Specify path to file containing runtime data",
@@ -285,21 +304,21 @@
 
     def __init__(self, json_path: str, dag_path: str, data_paths: str):
         self.json_path = Path(json_path)
         self.dag_path = Path(dag_path)
         self.data_paths = [Path(path) for path in data_paths]
 
 
-@dataclass()
+@dataclass
 class CausalVariables:
     """
-    A dataclass that converts
+    A dataclass that converts lists of dictionaries into lists of Causal Variables
     """
 
-    inputs: list[Input]
-    outputs: list[Output]
-    metas: list[Meta]
-
     def __init__(self, inputs: list[dict], outputs: list[dict], metas: list[dict]):
         self.inputs = [Input(**i) for i in inputs]
         self.outputs = [Output(**o) for o in outputs]
         self.metas = [Meta(**m) for m in metas] if metas else []
+
+    def __iter__(self):
+        for var in self.inputs + self.outputs + self.metas:
+            yield var
```

### Comparing `causal_testing_framework-3.1.0/causal_testing/specification/causal_dag.py` & `causal_testing_framework-3.2.0/causal_testing/specification/causal_dag.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import logging
 from itertools import combinations
 from random import sample
 from typing import Union
 
 import networkx as nx
 
+from causal_testing.testing.base_test_case import BaseTestCase
+
 from .scenario import Scenario
 from .variable import Output
 
 Node = Union[str, int]  # Node type hint: A node is a string or an int
 
 logger = logging.getLogger(__name__)
 
@@ -492,15 +494,15 @@
         :return: Whether the given variable is or depends on an output.
         :rtype: bool
         """
         if isinstance(scenario.variables[node], Output):
             return True
         return any((self.depends_on_outputs(n, scenario) for n in self.graph.predecessors(node)))
 
-    def identification(self, base_test_case):
+    def identification(self, base_test_case: BaseTestCase):
         """Identify and return the minimum adjustment set
 
         :param base_test_case: A base test case instance containing the outcome_variable and the
         treatment_variable required for identification.
         :return minimal_adjustment_set: The smallest set of variables which can be adjusted for to obtain a causal
         estimate as opposed to a purely associational estimate.
         """
```

### Comparing `causal_testing_framework-3.1.0/causal_testing/specification/causal_specification.py` & `causal_testing_framework-3.2.0/causal_testing/specification/causal_specification.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/causal_testing/specification/metamorphic_relation.py` & `causal_testing_framework-3.2.0/causal_testing/specification/metamorphic_relation.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,14 @@
     """
     metamorphic_relations = []
     for node_pair in combinations(dag.graph.nodes, 2):
         (u, v) = node_pair
 
         # Create a ShouldNotCause relation for each pair of nodes that are not directly connected
         if ((u, v) not in dag.graph.edges) and ((v, u) not in dag.graph.edges):
-
             # Case 1: U --> ... --> V
             if u in nx.ancestors(dag.graph, v):
                 adj_set = list(dag.direct_effect_adjustment_sets([u], [v])[0])
                 metamorphic_relations.append(ShouldNotCause(u, v, adj_set, dag))
 
             # Case 2: V --> ... --> U
             elif v in nx.ancestors(dag.graph, u):
```

### Comparing `causal_testing_framework-3.1.0/causal_testing/specification/scenario.py` & `causal_testing_framework-3.2.0/causal_testing/specification/scenario.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/causal_testing/specification/variable.py` & `causal_testing_framework-3.2.0/causal_testing/specification/variable.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/causal_testing/testing/base_test_case.py` & `causal_testing_framework-3.2.0/causal_testing/testing/base_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/causal_testing/testing/causal_test_case.py` & `causal_testing_framework-3.2.0/causal_testing/testing/causal_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/causal_testing/testing/causal_test_engine.py` & `causal_testing_framework-3.2.0/causal_testing/testing/causal_test_engine.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/causal_testing/testing/causal_test_outcome.py` & `causal_testing_framework-3.2.0/causal_testing/testing/causal_test_outcome.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/causal_testing/testing/causal_test_result.py` & `causal_testing_framework-3.2.0/causal_testing/testing/causal_test_result.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/causal_testing/testing/causal_test_suite.py` & `causal_testing_framework-3.2.0/causal_testing/testing/causal_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/causal_testing/testing/estimators.py` & `causal_testing_framework-3.2.0/causal_testing/testing/estimators.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,18 +154,18 @@
             if str(treatment_and_adjustments_cols.dtypes[col]) == "object":
                 treatment_and_adjustments_cols = pd.get_dummies(
                     treatment_and_adjustments_cols, columns=[col], drop_first=True
                 )
         model = smf.logit(formula=self.formula, data=data).fit(disp=0)
         return model
 
-    def estimate(self, data: pd.DataFrame, adjustment_config=None) -> RegressionResultsWrapper:
+    def estimate(self, data: pd.DataFrame, adjustment_config: dict = None) -> RegressionResultsWrapper:
         """add terms to the dataframe and estimate the outcome from the data
         :param data: A pandas dataframe containing execution data from the system-under-test.
-
+        :param adjustment_config: Dictionary containing the adjustment configuration of the adjustment set
         """
         if adjustment_config is None:
             adjustment_config = {}
         if set(self.adjustment_set) != set(adjustment_config):
             raise ValueError(
                 f"Invalid adjustment configuration {adjustment_config}. Must specify values for {self.adjustment_set}"
             )
```

### Comparing `causal_testing_framework-3.1.0/causal_testing/testing/intervention.py` & `causal_testing_framework-3.2.0/causal_testing/testing/intervention.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/causal_testing/testing/validation.py` & `causal_testing_framework-3.2.0/causal_testing/testing/validation.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/causal_testing_framework.egg-info/PKG-INFO` & `causal_testing_framework-3.2.0/causal_testing_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal-testing-framework
-Version: 3.1.0
+Version: 3.2.0
 Summary: A framework for causal testing using causal directed acyclic graphs.
 Author: The CITCOM team
 License: MIT
 Project-URL: Bug_Tracker, https://github.com/CITCOM-project/CausalTestingFramework/issues
 Project-URL: Documentation, https://causal-testing-framework.readthedocs.io/
 Project-URL: Source, https://github.com/CITCOM-project/CausalTestingFramework
 Keywords: causal inference,verification
```

### Comparing `causal_testing_framework-3.1.0/causal_testing_framework.egg-info/SOURCES.txt` & `causal_testing_framework-3.2.0/causal_testing_framework.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 tests/test_helpers.py
 tests/data/nhefs.csv
 tests/data_collection_tests/test_observational_data_collector.py
 tests/generation_tests/test_abstract_test_case.py
 tests/json_front_tests/test_json_class.py
 tests/resources/data/dag.dot
 tests/resources/data/data.csv
+tests/resources/data/data_with_meta.csv
 tests/resources/data/tests.json
 tests/specification_tests/test_causal_dag.py
 tests/specification_tests/test_metamorphic_relations.py
 tests/specification_tests/test_variable.py
 tests/testing_tests/test_causal_test_case.py
 tests/testing_tests/test_causal_test_engine.py
 tests/testing_tests/test_causal_test_outcome.py
```

### Comparing `causal_testing_framework-3.1.0/docs/Makefile` & `causal_testing_framework-3.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/docs/README.md` & `causal_testing_framework-3.2.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/docs/make.bat` & `causal_testing_framework-3.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/docs/source/conf.py` & `causal_testing_framework-3.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/docs/source/description.rst` & `causal_testing_framework-3.2.0/docs/source/description.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/docs/source/frontends/json_front_end.rst` & `causal_testing_framework-3.2.0/docs/source/frontends/json_front_end.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/docs/source/frontends/test_suite.rst` & `causal_testing_framework-3.2.0/docs/source/frontends/test_suite.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/docs/source/images/workflow.png` & `causal_testing_framework-3.2.0/docs/source/images/workflow.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/docs/source/index.rst` & `causal_testing_framework-3.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/docs/source/installation.rst` & `causal_testing_framework-3.2.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/docs/source/modules/causal_specification.rst` & `causal_testing_framework-3.2.0/docs/source/modules/causal_specification.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/docs/source/modules/causal_tests.rst` & `causal_testing_framework-3.2.0/docs/source/modules/causal_tests.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/docs/source/modules/data_collector.rst` & `causal_testing_framework-3.2.0/docs/source/modules/data_collector.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/docs/source/usage.rst` & `causal_testing_framework-3.2.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/covasim_/doubling_beta/README.md` & `causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/covasim_/doubling_beta/dag.png` & `causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv` & `causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/covasim_/doubling_beta/example_beta.py` & `causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/example_beta.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/covasim_/vaccinating_elderly/README.md` & `causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/covasim_/vaccinating_elderly/dag.png` & `causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/covasim_/vaccinating_elderly/example_vaccine.py` & `causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/example_vaccine.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/lr91/README.md` & `causal_testing_framework-3.2.0/examples/lr91/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/lr91/dag.dot` & `causal_testing_framework-3.2.0/examples/lr91/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/lr91/dag.png` & `causal_testing_framework-3.2.0/examples/lr91/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/lr91/data/normalised_results.csv` & `causal_testing_framework-3.2.0/examples/lr91/data/normalised_results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/lr91/data/results.csv` & `causal_testing_framework-3.2.0/examples/lr91/data/results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/lr91/example_max_conductances.py` & `causal_testing_framework-3.2.0/examples/lr91/example_max_conductances.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/lr91/example_max_conductances_test_suite.py` & `causal_testing_framework-3.2.0/examples/lr91/example_max_conductances_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson/README.md` & `causal_testing_framework-3.2.0/examples/poisson/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson/causal_tests.json` & `causal_testing_framework-3.2.0/examples/poisson/causal_tests.json`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson/dag.dot` & `causal_testing_framework-3.2.0/examples/poisson/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson/data.csv` & `causal_testing_framework-3.2.0/examples/poisson/data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson/example_run_causal_tests.py` & `causal_testing_framework-3.2.0/examples/poisson/example_run_causal_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,17 +131,15 @@
     "LinearRegressionEstimator": LinearRegressionEstimator,
 }
 
 # Create input structure required to create a modelling scenario
 modelling_inputs = (
     [Input(i["name"], i["datatype"], i["distribution"]) for i in inputs]
     + [Output(i["name"], i["datatype"]) for i in outputs]
-    + [Meta(i["name"], i["datatype"], [i["populate"]]) for i in metas]
-    if metas
-    else list()
+    + ([Meta(i["name"], i["datatype"], i["populate"]) for i in metas] if metas else list())
 )
 
 # Create modelling scenario to access z3 variable mirrors
 modelling_scenario = Scenario(modelling_inputs, None)
 modelling_scenario.setup_treatment_variables()
 
 mutates = {
@@ -170,25 +168,23 @@
 
     json_utility = MyJsonUtility(log_path)  # Create an instance of the extended JsonUtility class
     json_utility.set_paths(
         json_path, dag_path, [data_path]
     )  # Set the path to the data.csv, dag.dot and causal_tests.json file
 
     # Load the Causal Variables into the JsonUtility class ready to be used in the tests
-    json_utility.set_variables(inputs, outputs, metas)
-    json_utility.setup()  # Sets up all the necessary parts of the json_class needed to execute tests
+    json_utility.setup(scenario=modelling_scenario)  # Sets up all the necessary parts of the json_class needed to execute tests
 
     json_utility.generate_tests(effects, mutates, estimators, False)
 
 
 if __name__ == "__main__":
     args = MyJsonUtility.get_args()
     json_utility = MyJsonUtility(args.log_path)  # Create an instance of the extended JsonUtility class
     json_utility.set_paths(
         args.json_path, args.dag_path, args.data_path
     )  # Set the path to the data.csv, dag.dot and causal_tests.json file
 
     # Load the Causal Variables into the JsonUtility class ready to be used in the tests
-    json_utility.set_variables(inputs, outputs, metas)
-    json_utility.setup()  # Sets up all the necessary parts of the json_class needed to execute tests
+    json_utility.setup(scenario=modelling_scenario)  # Sets up all the necessary parts of the json_class needed to execute tests
 
     json_utility.generate_tests(effects, mutates, estimators, args.f)
```

### Comparing `causal_testing_framework-3.1.0/examples/poisson-line-process/README.md` & `causal_testing_framework-3.2.0/examples/poisson-line-process/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson-line-process/dag.png` & `causal_testing_framework-3.2.0/examples/poisson-line-process/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson-line-process/data/random/data_random_1000.csv` & `causal_testing_framework-3.2.0/examples/poisson-line-process/data/random/data_random_1000.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv` & `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv` & `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv` & `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv` & `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv` & `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv` & `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv` & `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv` & `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv` & `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv` & `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/examples/poisson-line-process/example_poisson_process.py` & `causal_testing_framework-3.2.0/examples/poisson-line-process/example_poisson_process.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/images/workflow.png` & `causal_testing_framework-3.2.0/images/workflow.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/pyproject.toml` & `causal_testing_framework-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/tests/data/nhefs.csv` & `causal_testing_framework-3.2.0/tests/data/nhefs.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/tests/data_collection_tests/test_observational_data_collector.py` & `causal_testing_framework-3.2.0/tests/data_collection_tests/test_observational_data_collector.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/tests/generation_tests/test_abstract_test_case.py` & `causal_testing_framework-3.2.0/tests/generation_tests/test_abstract_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/tests/specification_tests/test_causal_dag.py` & `causal_testing_framework-3.2.0/tests/specification_tests/test_causal_dag.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/tests/specification_tests/test_metamorphic_relations.py` & `causal_testing_framework-3.2.0/tests/specification_tests/test_metamorphic_relations.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/tests/specification_tests/test_variable.py` & `causal_testing_framework-3.2.0/tests/specification_tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/tests/test_helpers.py` & `causal_testing_framework-3.2.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/tests/testing_tests/test_causal_test_case.py` & `causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/tests/testing_tests/test_causal_test_engine.py` & `causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_engine.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/tests/testing_tests/test_causal_test_outcome.py` & `causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_outcome.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/tests/testing_tests/test_causal_test_suite.py` & `causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.1.0/tests/testing_tests/test_estimators.py` & `causal_testing_framework-3.2.0/tests/testing_tests/test_estimators.py`

 * *Files identical despite different names*

