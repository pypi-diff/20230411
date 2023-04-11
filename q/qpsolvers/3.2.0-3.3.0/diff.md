# Comparing `tmp/qpsolvers-3.2.0.tar.gz` & `tmp/qpsolvers-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qpsolvers-3.2.0.tar", last modified: Wed Mar 29 16:07:34 2023, max compression
+gzip compressed data, was "qpsolvers-3.3.0.tar", last modified: Tue Apr 11 12:21:12 2023, max compression
```

## Comparing `qpsolvers-3.2.0.tar` & `qpsolvers-3.3.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0     1758 2023-03-29 16:04:08.418756 qpsolvers-3.2.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2529 2023-03-29 16:03:40.695119 qpsolvers-3.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      128 2023-03-03 11:09:52.358283 qpsolvers-3.2.0/.gitignore
--rw-r--r--   0        0        0    15351 2023-03-29 16:06:05.577220 qpsolvers-3.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      916 2023-02-28 14:28:36.811176 qpsolvers-3.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     7652 2021-03-24 14:54:52.923152 qpsolvers-3.2.0/LICENSE
--rw-r--r--   0        0        0     9661 2023-03-28 08:42:54.624660 qpsolvers-3.2.0/README.md
--rw-r--r--   0        0        0      832 2023-02-28 13:41:23.525818 qpsolvers-3.2.0/THANKS
--rw-r--r--   0        0        0     2740 2023-02-23 09:14:02.675958 qpsolvers-3.2.0/benchmark/benchmark_dense_problem.py
--rw-r--r--   0        0        0     2077 2023-02-23 09:14:02.675958 qpsolvers-3.2.0/benchmark/benchmark_model_predictive_control.py
--rw-r--r--   0        0        0     3471 2023-02-23 09:14:02.675958 qpsolvers-3.2.0/benchmark/benchmark_random_problems.py
--rw-r--r--   0        0        0     3017 2023-02-23 09:14:02.675958 qpsolvers-3.2.0/benchmark/benchmark_sparse_problem.py
--rw-r--r--   0        0        0     9656 2023-03-03 11:09:52.358283 qpsolvers-3.2.0/doc/conf.py
--rw-r--r--   0        0        0     2590 2023-03-03 11:09:52.362283 qpsolvers-3.2.0/doc/developer-notes.rst
--rw-r--r--   0        0        0      102 2023-02-28 13:41:23.525818 qpsolvers-3.2.0/doc/environment.yml
--rw-r--r--   0        0        0      931 2023-03-03 11:09:52.362283 qpsolvers-3.2.0/doc/index.rst
--rw-r--r--   0        0        0     3707 2023-03-03 11:09:52.362283 qpsolvers-3.2.0/doc/installation.rst
--rw-r--r--   0        0        0     1006 2023-03-03 11:09:52.362283 qpsolvers-3.2.0/doc/least-squares.rst
--rw-r--r--   0        0        0     5559 2023-03-03 15:29:30.344114 qpsolvers-3.2.0/doc/quadratic-programming.rst
--rw-r--r--   0        0        0     2255 2023-03-03 11:09:52.362283 qpsolvers-3.2.0/doc/references.rst
--rw-r--r--   0        0        0      900 2023-03-03 15:28:57.696416 qpsolvers-3.2.0/doc/supported-solvers.rst
--rw-r--r--   0        0        0      473 2023-03-03 15:09:27.367215 qpsolvers-3.2.0/doc/unsupported-solvers.rst
--rw-r--r--   0        0        0      636 2023-02-28 14:10:40.413484 qpsolvers-3.2.0/examples/README.md
--rw-r--r--   0        0        0     2030 2023-02-28 14:10:40.413484 qpsolvers-3.2.0/examples/box_inequalities.py
--rw-r--r--   0        0        0     1601 2023-02-23 09:14:02.683958 qpsolvers-3.2.0/examples/constrained_linear_regression.py
--rw-r--r--   0        0        0     2790 2023-02-28 14:10:40.413484 qpsolvers-3.2.0/examples/dual_multipliers.py
--rw-r--r--   0        0        0     1867 2023-02-28 14:10:40.413484 qpsolvers-3.2.0/examples/least_squares.py
--rw-r--r--   0        0        0     8297 2023-02-23 09:14:02.683958 qpsolvers-3.2.0/examples/model_predictive_control.py
--rw-r--r--   0        0        0     2045 2023-03-03 11:01:10.969238 qpsolvers-3.2.0/examples/quadratic_program.py
--rw-r--r--   0        0        0     2656 2023-03-28 08:42:54.624660 qpsolvers-3.2.0/examples/sparse_least_squares.py
--rw-r--r--   0        0        0     2080 2023-03-09 10:38:34.379711 qpsolvers-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     2255 2023-03-29 16:06:13.681114 qpsolvers-3.2.0/qpsolvers/__init__.py
--rw-r--r--   0        0        0     1317 2023-03-03 15:09:27.367215 qpsolvers-3.2.0/qpsolvers/_internals.py
--rw-r--r--   0        0        0     1216 2023-02-23 09:14:02.687958 qpsolvers-3.2.0/qpsolvers/conversions/__init__.py
--rw-r--r--   0        0        0     2317 2023-02-23 09:14:02.687958 qpsolvers-3.2.0/qpsolvers/conversions/ensure_sparse_matrices.py
--rw-r--r--   0        0        0     3561 2023-02-28 14:10:40.413484 qpsolvers-3.2.0/qpsolvers/conversions/linear_from_box_inequalities.py
--rw-r--r--   0        0        0     3762 2023-02-28 14:10:40.417483 qpsolvers-3.2.0/qpsolvers/conversions/socp_from_qp.py
--rw-r--r--   0        0        0     2254 2023-02-23 09:14:02.687958 qpsolvers-3.2.0/qpsolvers/conversions/split_dual_linear_box.py
--rw-r--r--   0        0        0     1677 2023-02-28 14:10:40.417483 qpsolvers-3.2.0/qpsolvers/exceptions.py
--rw-r--r--   0        0        0     8531 2023-02-28 14:10:40.417483 qpsolvers-3.2.0/qpsolvers/problem.py
--rw-r--r--   0        0        0     1825 2023-03-28 08:42:54.624660 qpsolvers-3.2.0/qpsolvers/problems.py
--rw-r--r--   0        0        0     7693 2023-02-28 14:10:40.417483 qpsolvers-3.2.0/qpsolvers/solution.py
--rw-r--r--   0        0        0     7412 2023-03-28 08:42:54.624660 qpsolvers-3.2.0/qpsolvers/solve_ls.py
--rw-r--r--   0        0        0     3437 2023-03-03 15:09:27.367215 qpsolvers-3.2.0/qpsolvers/solve_problem.py
--rw-r--r--   0        0        0     4670 2023-02-28 14:10:40.417483 qpsolvers-3.2.0/qpsolvers/solve_qp.py
--rw-r--r--   0        0        0     1717 2023-02-28 14:10:40.417483 qpsolvers-3.2.0/qpsolvers/solve_unconstrained.py
--rw-r--r--   0        0        0    11231 2023-03-03 15:09:27.367215 qpsolvers-3.2.0/qpsolvers/solvers/__init__.py
--rw-r--r--   0        0        0     6511 2023-03-03 15:09:27.367215 qpsolvers-3.2.0/qpsolvers/solvers/clarabel_.py
--rw-r--r--   0        0        0     8934 2023-03-28 08:42:54.628660 qpsolvers-3.2.0/qpsolvers/solvers/cvxopt_.py
--rw-r--r--   0        0        0     8390 2023-03-03 11:00:10.845570 qpsolvers-3.2.0/qpsolvers/solvers/ecos_.py
--rw-r--r--   0        0        0     7654 2023-02-28 13:53:41.462586 qpsolvers-3.2.0/qpsolvers/solvers/gurobi_.py
--rw-r--r--   0        0        0     9373 2023-02-28 13:53:41.462586 qpsolvers-3.2.0/qpsolvers/solvers/highs_.py
--rw-r--r--   0        0        0     9624 2023-02-28 14:10:40.417483 qpsolvers-3.2.0/qpsolvers/solvers/osqp_.py
--rw-r--r--   0        0        0     9790 2023-03-03 15:09:27.367215 qpsolvers-3.2.0/qpsolvers/solvers/proxqp_.py
--rw-r--r--   0        0        0    13411 2023-02-28 14:10:40.417483 qpsolvers-3.2.0/qpsolvers/solvers/qpoases_.py
--rw-r--r--   0        0        0    10591 2023-02-28 14:10:40.417483 qpsolvers-3.2.0/qpsolvers/solvers/qpswift_.py
--rw-r--r--   0        0        0     7021 2023-02-28 14:10:40.417483 qpsolvers-3.2.0/qpsolvers/solvers/quadprog_.py
--rw-r--r--   0        0        0     9763 2023-02-28 13:54:05.726084 qpsolvers-3.2.0/qpsolvers/solvers/scs_.py
--rw-r--r--   0        0        0     2808 2023-03-03 15:09:27.367215 qpsolvers-3.2.0/qpsolvers/unsupported/__init__.py
--rw-r--r--   0        0        0     4246 2023-03-03 15:09:27.367215 qpsolvers-3.2.0/qpsolvers/unsupported/mosek_.py
--rw-r--r--   0        0        0     6501 2023-03-03 15:09:27.367215 qpsolvers-3.2.0/qpsolvers/unsupported/nppro_.py
--rw-r--r--   0        0        0     2390 2023-02-28 13:27:49.518364 qpsolvers-3.2.0/qpsolvers/utils.py
--rw-r--r--   0        0        0       59 2021-04-09 11:14:24.912320 qpsolvers-3.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2612 2023-03-28 08:42:54.628660 qpsolvers-3.2.0/tests/problems.py
--rw-r--r--   0        0        0     4990 2023-02-23 09:14:02.695958 qpsolvers-3.2.0/tests/solved_problems.py
--rw-r--r--   0        0        0     2252 2023-02-28 13:41:23.529818 qpsolvers-3.2.0/tests/test_clarabel.py
--rw-r--r--   0        0        0     3681 2023-02-28 13:41:23.529818 qpsolvers-3.2.0/tests/test_conversions.py
--rw-r--r--   0        0        0     3948 2023-02-28 13:52:35.807944 qpsolvers-3.2.0/tests/test_cvxopt.py
--rw-r--r--   0        0        0     1370 2023-02-28 13:42:47.800084 qpsolvers-3.2.0/tests/test_ecos.py
--rw-r--r--   0        0        0     1527 2023-02-28 13:41:23.529818 qpsolvers-3.2.0/tests/test_gurobi.py
--rw-r--r--   0        0        0     1773 2023-02-28 13:41:23.529818 qpsolvers-3.2.0/tests/test_highs.py
--rw-r--r--   0        0        0     1377 2023-02-28 13:41:23.529818 qpsolvers-3.2.0/tests/test_mosek.py
--rw-r--r--   0        0        0     1348 2023-03-03 11:09:52.362283 qpsolvers-3.2.0/tests/test_nppro.py
--rw-r--r--   0        0        0     1370 2023-02-28 13:41:23.529818 qpsolvers-3.2.0/tests/test_osqp.py
--rw-r--r--   0        0        0     3584 2023-02-28 14:10:40.417483 qpsolvers-3.2.0/tests/test_problem.py
--rw-r--r--   0        0        0     3570 2023-02-28 14:10:40.421483 qpsolvers-3.2.0/tests/test_proxqp.py
--rw-r--r--   0        0        0     3191 2023-02-28 13:41:23.529818 qpsolvers-3.2.0/tests/test_qpoases.py
--rw-r--r--   0        0        0     1733 2023-02-28 13:41:23.529818 qpsolvers-3.2.0/tests/test_qpswift.py
--rw-r--r--   0        0        0     2332 2023-02-28 14:10:40.421483 qpsolvers-3.2.0/tests/test_quadprog.py
--rw-r--r--   0        0        0     1695 2023-02-28 14:10:40.421483 qpsolvers-3.2.0/tests/test_scs.py
--rw-r--r--   0        0        0     2640 2023-02-28 14:10:40.421483 qpsolvers-3.2.0/tests/test_solution.py
--rw-r--r--   0        0        0     9194 2023-03-28 08:42:54.628660 qpsolvers-3.2.0/tests/test_solve_ls.py
--rw-r--r--   0        0        0    10923 2023-03-09 10:38:34.379711 qpsolvers-3.2.0/tests/test_solve_problem.py
--rw-r--r--   0        0        0    25373 2023-03-01 15:42:31.974853 qpsolvers-3.2.0/tests/test_solve_qp.py
--rw-r--r--   0        0        0     3012 2023-02-28 14:10:40.421483 qpsolvers-3.2.0/tests/test_unfeasible_problem.py
--rw-r--r--   0        0        0     1865 2023-02-28 13:41:23.529818 qpsolvers-3.2.0/tests/test_utils.py
--rw-r--r--   0        0        0     2260 2023-03-29 16:04:08.418756 qpsolvers-3.2.0/tox.ini
--rw-r--r--   0        0        0    11600 1970-01-01 00:00:00.000000 qpsolvers-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1590 2023-04-11 09:56:34.196100 qpsolvers-3.3.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     2529 2023-03-29 16:03:40.695119 qpsolvers-3.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      128 2023-03-03 11:09:52.358283 qpsolvers-3.3.0/.gitignore
+-rw-r--r--   0        0        0    15793 2023-04-11 12:17:50.779162 qpsolvers-3.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      916 2023-02-28 14:28:36.811176 qpsolvers-3.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     7652 2021-03-24 14:54:52.923152 qpsolvers-3.3.0/LICENSE
+-rw-r--r--   0        0        0     9754 2023-04-11 09:57:38.987082 qpsolvers-3.3.0/README.md
+-rw-r--r--   0        0        0      832 2023-02-28 13:41:23.525818 qpsolvers-3.3.0/THANKS
+-rw-r--r--   0        0        0     2740 2023-02-23 09:14:02.675958 qpsolvers-3.3.0/benchmark/benchmark_dense_problem.py
+-rw-r--r--   0        0        0     2077 2023-02-23 09:14:02.675958 qpsolvers-3.3.0/benchmark/benchmark_model_predictive_control.py
+-rw-r--r--   0        0        0     3471 2023-02-23 09:14:02.675958 qpsolvers-3.3.0/benchmark/benchmark_random_problems.py
+-rw-r--r--   0        0        0     3017 2023-02-23 09:14:02.675958 qpsolvers-3.3.0/benchmark/benchmark_sparse_problem.py
+-rw-r--r--   0        0        0     9656 2023-03-03 11:09:52.358283 qpsolvers-3.3.0/doc/conf.py
+-rw-r--r--   0        0        0     2924 2023-04-11 09:56:34.196100 qpsolvers-3.3.0/doc/developer-notes.rst
+-rw-r--r--   0        0        0      265 2023-04-11 09:56:34.196100 qpsolvers-3.3.0/doc/environment.yml
+-rw-r--r--   0        0        0      931 2023-03-03 11:09:52.362283 qpsolvers-3.3.0/doc/index.rst
+-rw-r--r--   0        0        0     3707 2023-03-03 11:09:52.362283 qpsolvers-3.3.0/doc/installation.rst
+-rw-r--r--   0        0        0     1006 2023-03-03 11:09:52.362283 qpsolvers-3.3.0/doc/least-squares.rst
+-rw-r--r--   0        0        0     5559 2023-03-03 15:29:30.344114 qpsolvers-3.3.0/doc/quadratic-programming.rst
+-rw-r--r--   0        0        0     2521 2023-04-11 09:56:34.196100 qpsolvers-3.3.0/doc/references.rst
+-rw-r--r--   0        0        0      968 2023-04-11 09:56:34.196100 qpsolvers-3.3.0/doc/supported-solvers.rst
+-rw-r--r--   0        0        0      473 2023-03-03 15:09:27.367215 qpsolvers-3.3.0/doc/unsupported-solvers.rst
+-rw-r--r--   0        0        0      636 2023-02-28 14:10:40.413484 qpsolvers-3.3.0/examples/README.md
+-rw-r--r--   0        0        0     2030 2023-02-28 14:10:40.413484 qpsolvers-3.3.0/examples/box_inequalities.py
+-rw-r--r--   0        0        0     1601 2023-02-23 09:14:02.683958 qpsolvers-3.3.0/examples/constrained_linear_regression.py
+-rw-r--r--   0        0        0     2790 2023-02-28 14:10:40.413484 qpsolvers-3.3.0/examples/dual_multipliers.py
+-rw-r--r--   0        0        0     1867 2023-02-28 14:10:40.413484 qpsolvers-3.3.0/examples/least_squares.py
+-rw-r--r--   0        0        0     8297 2023-02-23 09:14:02.683958 qpsolvers-3.3.0/examples/model_predictive_control.py
+-rw-r--r--   0        0        0     2045 2023-03-03 11:01:10.969238 qpsolvers-3.3.0/examples/quadratic_program.py
+-rw-r--r--   0        0        0     2656 2023-03-28 08:42:54.624660 qpsolvers-3.3.0/examples/sparse_least_squares.py
+-rw-r--r--   0        0        0     2100 2023-04-11 09:56:47.503891 qpsolvers-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2295 2023-04-11 12:18:06.354909 qpsolvers-3.3.0/qpsolvers/__init__.py
+-rw-r--r--   0        0        0     1317 2023-03-03 15:09:27.367215 qpsolvers-3.3.0/qpsolvers/_internals.py
+-rw-r--r--   0        0        0     1216 2023-02-23 09:14:02.687958 qpsolvers-3.3.0/qpsolvers/conversions/__init__.py
+-rw-r--r--   0        0        0     2317 2023-02-23 09:14:02.687958 qpsolvers-3.3.0/qpsolvers/conversions/ensure_sparse_matrices.py
+-rw-r--r--   0        0        0     3561 2023-02-28 14:10:40.413484 qpsolvers-3.3.0/qpsolvers/conversions/linear_from_box_inequalities.py
+-rw-r--r--   0        0        0     3762 2023-02-28 14:10:40.417483 qpsolvers-3.3.0/qpsolvers/conversions/socp_from_qp.py
+-rw-r--r--   0        0        0     2284 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/conversions/split_dual_linear_box.py
+-rw-r--r--   0        0        0     1677 2023-02-28 14:10:40.417483 qpsolvers-3.3.0/qpsolvers/exceptions.py
+-rw-r--r--   0        0        0     8531 2023-02-28 14:10:40.417483 qpsolvers-3.3.0/qpsolvers/problem.py
+-rw-r--r--   0        0        0     6610 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/problems.py
+-rw-r--r--   0        0        0     7795 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solution.py
+-rw-r--r--   0        0        0     7412 2023-03-28 08:42:54.624660 qpsolvers-3.3.0/qpsolvers/solve_ls.py
+-rw-r--r--   0        0        0     3437 2023-03-03 15:09:27.367215 qpsolvers-3.3.0/qpsolvers/solve_problem.py
+-rw-r--r--   0        0        0     4698 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solve_qp.py
+-rw-r--r--   0        0        0     1743 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solve_unconstrained.py
+-rw-r--r--   0        0        0    12032 2023-04-11 09:56:34.196100 qpsolvers-3.3.0/qpsolvers/solvers/__init__.py
+-rw-r--r--   0        0        0     6665 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/clarabel_.py
+-rw-r--r--   0        0        0     9089 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/cvxopt_.py
+-rw-r--r--   0        0        0     6441 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/daqp_.py
+-rw-r--r--   0        0        0     8434 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/ecos_.py
+-rw-r--r--   0        0        0     7813 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/gurobi_.py
+-rw-r--r--   0        0        0     9571 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/highs_.py
+-rw-r--r--   0        0        0     9733 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/osqp_.py
+-rw-r--r--   0        0        0     9807 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/proxqp_.py
+-rw-r--r--   0        0        0    13544 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/qpoases_.py
+-rw-r--r--   0        0        0    10619 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/qpswift_.py
+-rw-r--r--   0        0        0     6046 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/quadprog_.py
+-rw-r--r--   0        0        0     9904 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/solvers/scs_.py
+-rw-r--r--   0        0        0     2808 2023-03-03 15:09:27.367215 qpsolvers-3.3.0/qpsolvers/unsupported/__init__.py
+-rw-r--r--   0        0        0     4274 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/unsupported/mosek_.py
+-rw-r--r--   0        0        0     6453 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/qpsolvers/unsupported/nppro_.py
+-rw-r--r--   0        0        0     2390 2023-02-28 13:27:49.518364 qpsolvers-3.3.0/qpsolvers/utils.py
+-rw-r--r--   0        0        0       59 2021-04-09 11:14:24.912320 qpsolvers-3.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2612 2023-03-28 08:42:54.628660 qpsolvers-3.3.0/tests/problems.py
+-rw-r--r--   0        0        0     2214 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/tests/test_clarabel.py
+-rw-r--r--   0        0        0     3681 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_conversions.py
+-rw-r--r--   0        0        0     3940 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/tests/test_cvxopt.py
+-rw-r--r--   0        0        0     1370 2023-03-31 12:30:36.615914 qpsolvers-3.3.0/tests/test_ecos.py
+-rw-r--r--   0        0        0     1527 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_gurobi.py
+-rw-r--r--   0        0        0     1773 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_highs.py
+-rw-r--r--   0        0        0     1377 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_mosek.py
+-rw-r--r--   0        0        0     1348 2023-03-03 11:09:52.362283 qpsolvers-3.3.0/tests/test_nppro.py
+-rw-r--r--   0        0        0     1370 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_osqp.py
+-rw-r--r--   0        0        0     3584 2023-02-28 14:10:40.417483 qpsolvers-3.3.0/tests/test_problem.py
+-rw-r--r--   0        0        0     3570 2023-02-28 14:10:40.421483 qpsolvers-3.3.0/tests/test_proxqp.py
+-rw-r--r--   0        0        0     3191 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_qpoases.py
+-rw-r--r--   0        0        0     1733 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_qpswift.py
+-rw-r--r--   0        0        0     2332 2023-02-28 14:10:40.421483 qpsolvers-3.3.0/tests/test_quadprog.py
+-rw-r--r--   0        0        0     1695 2023-02-28 14:10:40.421483 qpsolvers-3.3.0/tests/test_scs.py
+-rw-r--r--   0        0        0     2640 2023-02-28 14:10:40.421483 qpsolvers-3.3.0/tests/test_solution.py
+-rw-r--r--   0        0        0     9194 2023-03-28 08:42:54.628660 qpsolvers-3.3.0/tests/test_solve_ls.py
+-rw-r--r--   0        0        0    11123 2023-04-11 10:02:56.850101 qpsolvers-3.3.0/tests/test_solve_problem.py
+-rw-r--r--   0        0        0    25373 2023-03-31 12:28:59.113529 qpsolvers-3.3.0/tests/test_solve_qp.py
+-rw-r--r--   0        0        0     3012 2023-02-28 14:10:40.421483 qpsolvers-3.3.0/tests/test_unfeasible_problem.py
+-rw-r--r--   0        0        0     1865 2023-02-28 13:41:23.529818 qpsolvers-3.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2426 2023-04-11 09:56:47.503891 qpsolvers-3.3.0/tox.ini
+-rw-r--r--   0        0        0    11721 1970-01-01 00:00:00.000000 qpsolvers-3.3.0/PKG-INFO
```

### Comparing `qpsolvers-3.2.0/.github/workflows/docs.yml` & `qpsolvers-3.3.0/.github/workflows/docs.yml`

 * *Files 16% similar despite different names*

```diff
@@ -25,18 +25,14 @@
               uses: mamba-org/provision-with-micromamba@main
               with:
                   cache-downloads: true
                   cache-env: true
                   environment-file: doc/environment.yml
                   environment-name: qpsolvers
 
-            - name: "Install PyPI dependencies"
-              run: |
-                  pip install furo highspy sphinx sphinx-autodoc-typehints sphinx-mathjax-offline
-
             - name: "Checkout qpSWIFT"
               uses: actions/checkout@v3
               with:
                   repository: qpSWIFT/qpSWIFT
                   path: qpSWIFT
 
             - name: "Install qpSWIFT"
```

### Comparing `qpsolvers-3.2.0/.github/workflows/test.yml` & `qpsolvers-3.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/CHANGELOG.md` & `qpsolvers-3.3.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [3.3.0] - 2023/04/11
+
+### Added
+
+- New sample problems in ``qpsolvers.problems``
+- New solver: [DAQP](https://darnstrom.github.io/daqp/) (thanks to @darnstrom)
+
+### Changed
+
+- Dual multipliers are empty arrays rather than None when no constraint
+- Store solver results even when solution is not found
+- Switch to ``Solution.found`` as solver success status (thanks to @rxian)
+
+### Fixed
+
+- Unit test on actual solution to QPSUT03 problem
+
 ## [3.2.0] - 2023/03/29
 
 ### Added
 
 - Sparse strategy to convert LS problems to QP (thanks to @bodono)
 - Start ``problems`` submodule to collect sample test problems
```

### Comparing `qpsolvers-3.2.0/CONTRIBUTING.md` & `qpsolvers-3.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/LICENSE` & `qpsolvers-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/README.md` & `qpsolvers-3.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 
 ## Solvers
 
 | Solver | Keyword | Algorithm | API | License | Warm-start |
 | ------ | ------- | --------- | --- | ------- |------------|
 | [Clarabel](https://github.com/oxfordcontrol/Clarabel.rs) | ``clarabel`` | Interior point | Sparse | Apache-2.0 | ✖️ |
 | [CVXOPT](http://cvxopt.org/) | ``cvxopt`` | Interior point | Dense | GPL-3.0 | ✔️ |
+| [DAQP](https://github.com/darnstrom/daqp) | ``daqp`` | Active set | Dense | MIT | ✖️ |
 | [ECOS](https://web.stanford.edu/~boyd/papers/ecos.html) | ``ecos`` | Interior point | Sparse | GPL-3.0 | ✖️ |
 | [Gurobi](https://www.gurobi.com/) | ``gurobi`` | Interior point | Sparse | Commercial | ✖️ |
 | [HiGHS](https://highs.dev/) | ``highs`` | Active set | Sparse | MIT | ✖️ |
 | [MOSEK](https://mosek.com/) | ``mosek`` | Interior point | Sparse | Commercial | ✔️ |
 | NPPro | ``nppro`` | Active set | Dense | Commercial | ✔️ |
 | [OSQP](https://osqp.org/) | ``osqp`` | Augmented Lagrangian | Sparse | Apache-2.0 | ✔️ |
 | [ProxQP](https://github.com/Simple-Robotics/proxsuite) | ``proxqp`` | Augmented Lagrangian | Dense & Sparse | BSD-2-Clause | ✔️ |
```

### Comparing `qpsolvers-3.2.0/THANKS` & `qpsolvers-3.3.0/THANKS`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/benchmark/benchmark_dense_problem.py` & `qpsolvers-3.3.0/benchmark/benchmark_dense_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/benchmark/benchmark_model_predictive_control.py` & `qpsolvers-3.3.0/benchmark/benchmark_model_predictive_control.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/benchmark/benchmark_random_problems.py` & `qpsolvers-3.3.0/benchmark/benchmark_random_problems.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/benchmark/benchmark_sparse_problem.py` & `qpsolvers-3.3.0/benchmark/benchmark_sparse_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/doc/conf.py` & `qpsolvers-3.3.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/doc/developer-notes.rst` & `qpsolvers-3.3.0/doc/developer-notes.rst`

 * *Files 8% similar despite different names*

```diff
@@ -54,16 +54,18 @@
         pass
 
 5. Append the solver identifier to ``dense_solvers`` or ``sparse_solvers``, if applicable
 6. Import ``awesomeqp_solve_qp`` from ``qpsolvers/__init__.py`` and add it to ``__all__``
 7. Import ``awesomeqp_solve_qp`` from the convenience ``__init__.py`` at the root of the repository, and add it to ``__all__``
 8. Add the solver to ``doc/src/supported-solvers.rst``
 9. Add the solver to the *Solvers* section of the README
-10. Log the new solver as an addition in the changelog
-11. Update the benchmark: run the scripts ``examples/benchmark_*.py`` and update the corresponding tables and plot in the README
+10. Assuming AwesomeQP is distributed on `PyPI <https://pypi.org/>`__, add it to the ``testenv`` and ``testenv:coverage`` environments in ``tox.ini`` for unit testing
+11. Assuming AwesomeQP is distributed on `PyPI <https://pypi.org/>`__, add it to the ``pip install`` line in the documentation workflow ``.github/workflows/docs.yml``
+12. Log the new solver as an addition in the changelog
+13. Update the benchmark: run the scripts ``examples/benchmark_*.py`` and update the corresponding tables and plot in the README
 
 Problem conversions
 ===================
 
 .. automodule:: qpsolvers.conversions
     :members:
```

### Comparing `qpsolvers-3.2.0/doc/index.rst` & `qpsolvers-3.3.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/doc/installation.rst` & `qpsolvers-3.3.0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/doc/least-squares.rst` & `qpsolvers-3.3.0/doc/least-squares.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/doc/quadratic-programming.rst` & `qpsolvers-3.3.0/doc/quadratic-programming.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/doc/references.rst` & `qpsolvers-3.3.0/doc/references.rst`

 * *Files 10% similar despite different names*

```diff
@@ -17,7 +17,9 @@
 .. [Ferreau2014] `qpOASES: A parametric active-set algorithm for quadratic programming <http://mpc.zib.de/archive/2014/4/Ferreau2014_Article_QpOASESAParametricActive-setAl.pdf>`_, H. J. Ferreau, C. Kirches, A. Potschka, H. G. Bock and M. Diehl. Mathematical Programming Computation, 2014, vol. 6, no 4, p. 327-363.
 
 .. [Domahidi2013] `ECOS: An SOCP solver for embedded systems <https://web.stanford.edu/~boyd/papers/ecos.html>`_, A. Domahidi, E. Chu and S. Boyd. European Control Conference. IEEE, 2013. p. 3071-3076.
 
 .. [Vandenberghe2010] `The CVXOPT linear and quadratic cone program solvers <https://www.seas.ucla.edu/~vandenbe/publications/coneprog.pdf>`_, L. Vandenberghe. 2010.
 
 .. [Goldfarb1983] *A numerically stable dual method for solving strictly convex quadratic programs*. D. Goldfarb and A. Idnani. Mathematical Programming, vol. 27, p. 1-33.
+
+.. [Arnstrom2022] `A dual active-set solver for embedded quadratic programming using recursive LDL updates <https://doi.org/10.1109/TAC.2022.3176430>`_, D. Arnström, A. Bemporad and D. Axehill. IEEE Transactions on Automatic Control, 2022, 67, no. 8 p. 4362-4369.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qpsolvers-3.2.0/doc/supported-solvers.rst` & `qpsolvers-3.3.0/doc/supported-solvers.rst`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 
 CVXOPT
 ======
 
 .. automodule:: qpsolvers.solvers.cvxopt_
     :members:
 
+DAQP
+======
+
+.. automodule:: qpsolvers.solvers.daqp_
+    :members:
+
 ECOS
 ====
 
 .. automodule:: qpsolvers.solvers.ecos_
     :members:
 
 Gurobi
```

### Comparing `qpsolvers-3.2.0/examples/README.md` & `qpsolvers-3.3.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/examples/box_inequalities.py` & `qpsolvers-3.3.0/examples/box_inequalities.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/examples/constrained_linear_regression.py` & `qpsolvers-3.3.0/examples/constrained_linear_regression.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/examples/dual_multipliers.py` & `qpsolvers-3.3.0/examples/dual_multipliers.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/examples/least_squares.py` & `qpsolvers-3.3.0/examples/least_squares.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/examples/model_predictive_control.py` & `qpsolvers-3.3.0/examples/model_predictive_control.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/examples/quadratic_program.py` & `qpsolvers-3.3.0/examples/quadratic_program.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/examples/sparse_least_squares.py` & `qpsolvers-3.3.0/examples/sparse_least_squares.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/pyproject.toml` & `qpsolvers-3.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 dependencies = [
+    "daqp >=0.5.0",
     "ecos >=2.0.8",
     "numpy >=1.15.4",
     "osqp >=0.6.2",
     "scipy >=1.2.0",
     "scs >=3.2.0",
 ]
 keywords = ["quadratic programming", "solver", "numerical optimization"]
```

### Comparing `qpsolvers-3.2.0/qpsolvers/__init__.py` & `qpsolvers-3.3.0/qpsolvers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from .problem import Problem
 from .solution import Solution
 from .solve_ls import solve_ls
 from .solve_qp import solve_problem, solve_qp
 from .solve_unconstrained import solve_unconstrained
 from .solvers import (
     cvxopt_solve_qp,
+    daqp_solve_qp,
     dense_solvers,
     ecos_solve_qp,
     gurobi_solve_qp,
     highs_solve_qp,
     osqp_solve_qp,
     proxqp_solve_qp,
     qpoases_solve_qp,
@@ -47,28 +48,29 @@
     quadprog_solve_qp,
     scs_solve_qp,
     sparse_solvers,
 )
 from .unsupported import mosek_solve_qp, nppro_solve_qp
 from .utils import print_matrix_vector
 
-__version__ = "3.2.0"
+__version__ = "3.3.0"
 
 __all__ = [
     "NoSolverSelected",
     "ParamError",
     "Problem",
     "ProblemError",
     "QPError",
     "Solution",
     "SolverError",
     "SolverNotFound",
     "__version__",
     "available_solvers",
     "cvxopt_solve_qp",
+    "daqp_solve_qp",
     "dense_solvers",
     "ecos_solve_qp",
     "gurobi_solve_qp",
     "highs_solve_qp",
     "mosek_solve_qp",
     "nppro_solve_qp",
     "osqp_solve_qp",
```

### Comparing `qpsolvers-3.2.0/qpsolvers/_internals.py` & `qpsolvers-3.3.0/qpsolvers/_internals.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/qpsolvers/conversions/__init__.py` & `qpsolvers-3.3.0/qpsolvers/conversions/__init__.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/qpsolvers/conversions/ensure_sparse_matrices.py` & `qpsolvers-3.3.0/qpsolvers/conversions/ensure_sparse_matrices.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/qpsolvers/conversions/linear_from_box_inequalities.py` & `qpsolvers-3.3.0/qpsolvers/conversions/linear_from_box_inequalities.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/qpsolvers/conversions/socp_from_qp.py` & `qpsolvers-3.3.0/qpsolvers/conversions/socp_from_qp.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/qpsolvers/conversions/split_dual_linear_box.py` & `qpsolvers-3.3.0/qpsolvers/conversions/split_dual_linear_box.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,18 +43,19 @@
         Lower bound constraint vector.
     ub :
         Upper bound constraint vector.
 
     Returns
     -------
     :
-        Pair :code:`z, z_box` of linear and box multipliers. Both can be
-        `None` if there is no corresponding constraint.
+        Pair :code:`z, z_box` of linear and box multipliers. Both can be empty
+        arrays if there is no corresponding constraint.
     """
-    z, z_box = None, None
+    z = np.empty((0,))
+    z_box = np.empty((0,))
     if lb is not None and ub is not None:
         n_lb = lb.shape[0]
         n_ub = ub.shape[0]
         n_box = n_lb + n_ub
         z_box = z_stacked[-n_ub:] - z_stacked[-n_box:-n_ub]
         z = z_stacked[:-n_box]
     elif ub is not None:  # lb is None
```

### Comparing `qpsolvers-3.2.0/qpsolvers/exceptions.py` & `qpsolvers-3.3.0/qpsolvers/exceptions.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/qpsolvers/problem.py` & `qpsolvers-3.3.0/qpsolvers/problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/qpsolvers/problems.py` & `qpsolvers-3.3.0/tests/test_highs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2016-2023 the qpsolvers contributors.
+# Copyright (C) 2016-2022 Stéphane Caron and the qpsolvers contributors.
 #
 # This file is part of qpsolvers.
 #
 # qpsolvers is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -14,52 +14,42 @@
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with qpsolvers. If not, see <http://www.gnu.org/licenses/>.
 
-"""Collection of sample problems."""
+"""Unit tests for HiGHS."""
 
-import numpy as np
-import scipy.sparse as spa
+import unittest
+import warnings
 
+from .problems import get_sd3310_problem
 
-def get_sparse_least_squares(n):
-    """
-    Get a sparse least squares problem.
-
-    Parameters
-    ----------
-    n :
-        Problem size.
-
-    Notes
-    -----
-    This problem was inspired by `this question on Stack Overflow
-    <https://stackoverflow.com/q/73656257/3721564>`__.
-    """
-    # minimize 1/2 || x - s ||^2
-    R = spa.eye(n, format="csc")
-    s = np.array(range(n), dtype=float)
-
-    # such that G * x <= h
-    G = spa.diags(
-        diagonals=[
-            [1.0 if i % 2 == 0 else 0.0 for i in range(n)],
-            [1.0 if i % 3 == 0 else 0.0 for i in range(n - 1)],
-            [1.0 if i % 5 == 0 else 0.0 for i in range(n - 1)],
-        ],
-        offsets=[0, 1, -1],
-        format="csc",
-    )
-    h = np.ones(G.shape[0])
-
-    # such that sum(x) == 42
-    A = spa.csc_matrix(np.ones((1, n)))
-    b = np.array([42.0]).reshape((1,))
-
-    # such that x >= 0
-    lb = np.zeros(n)
-    ub = None
+try:
+    from qpsolvers.solvers.highs_ import highs_solve_qp
+
+    class TestHiGHS(unittest.TestCase):
+        """Test fixture for the HiGHS solver."""
+
+        def setUp(self):
+            """Prepare test fixture."""
+            warnings.simplefilter("ignore", category=UserWarning)
+
+        def test_highs_tolerances(self):
+            problem = get_sd3310_problem()
+            x = highs_solve_qp(
+                problem.P,
+                problem.q,
+                problem.G,
+                problem.h,
+                problem.A,
+                problem.b,
+                time_limit=0.1,
+                primal_feasibility_tolerance=1e-1,
+                dual_feasibility_tolerance=1e-1,
+            )
+            self.assertIsNotNone(x)
 
-    return R, s, G, h, A, b, lb, ub
+
+except ImportError:  # solver not installed
+    warnings.warn("Skipping HiGHS tests as the solver is not installed")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qpsolvers-3.2.0/qpsolvers/solution.py` & `qpsolvers-3.3.0/qpsolvers/solution.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,19 @@
     """Solution returned by a QP solver for a given problem.
 
     Attributes
     ----------
     extras :
         Other outputs, specific to each solver.
 
+    found :
+        True if the solution was found successfully by a solver, False if the
+        solver did not find a solution or detected an unfeasible problem,
+        ``None`` if no solver was run.
+
     problem :
         Quadratic program the solution corresponds to.
 
     obj :
         Value of the primal objective at the solution (``None`` if no solution
         was found).
 
@@ -76,25 +81,21 @@
           are active and :math:`lb_i < x_i < ub_i`.
         - If :math:`z_{box,i} > 0`, then the upper bound :math:`x_i = ub_i` is
           active at the solution.
     """
 
     problem: Problem
     extras: dict = field(default_factory=dict)
+    found: Optional[bool] = None
     obj: Optional[float] = None
     x: Optional[np.ndarray] = None
     y: Optional[np.ndarray] = None
     z: Optional[np.ndarray] = None
     z_box: Optional[np.ndarray] = None
 
-    @property
-    def found(self) -> bool:
-        """Check whether the solver found a solution."""
-        return self.x is not None
-
     def is_optimal(self, eps_abs: float) -> bool:
         """Check whether the solution is indeed optimal.
 
         Parameters
         ----------
         eps_abs :
             Absolute tolerance for the primal residual, dual residual and
```

### Comparing `qpsolvers-3.2.0/qpsolvers/solve_ls.py` & `qpsolvers-3.3.0/qpsolvers/solve_ls.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/qpsolvers/solve_problem.py` & `qpsolvers-3.3.0/qpsolvers/solve_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/qpsolvers/solve_qp.py` & `qpsolvers-3.3.0/qpsolvers/solve_qp.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,8 +139,8 @@
     if solver is None:
         raise NoSolverSelected(
             "Set the `solver` keyword argument to one of the "
             f"available solvers in {available_solvers}"
         )
     problem = Problem(P, q, G, h, A, b, lb, ub)
     solution = solve_problem(problem, solver, initvals, verbose, **kwargs)
-    return solution.x
+    return solution.x if solution.found else None
```

### Comparing `qpsolvers-3.2.0/qpsolvers/solve_unconstrained.py` & `qpsolvers-3.3.0/qpsolvers/solve_unconstrained.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,8 +51,9 @@
     solution.x = lsqr(P, -q)[0]
     cost_check = np.linalg.norm(P @ solution.x + q)
     if cost_check > 1e-8:
         raise ProblemError(
             f"problem is unbounded below (cost_check={cost_check:.1e}), "
             "q has component in the nullspace of P"
         )
+    solution.found = True
     return solution
```

### Comparing `qpsolvers-3.2.0/qpsolvers/solvers/__init__.py` & `qpsolvers-3.3.0/qpsolvers/solvers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,56 @@
     available_solvers.append("cvxopt")
     dense_solvers.append("cvxopt")
     sparse_solvers.append("cvxopt")
 except ImportError:
     pass
 
 
+# DAQP
+# ========
+
+daqp_solve_qp: Optional[
+    Callable[
+        [
+            ndarray,
+            ndarray,
+            Optional[ndarray],
+            Optional[ndarray],
+            Optional[ndarray],
+            Optional[ndarray],
+            Optional[ndarray],
+            Optional[ndarray],
+            Optional[ndarray],
+            bool,
+        ],
+        Optional[ndarray],
+    ]
+] = None
+
+daqp_solve_problem: Optional[
+    Callable[
+        [
+            Problem,
+            Optional[ndarray],
+            bool,
+        ],
+        Solution,
+    ]
+] = None
+
+try:
+    from .daqp_ import daqp_solve_problem, daqp_solve_qp
+
+    solve_function["daqp"] = daqp_solve_problem
+    available_solvers.append("daqp")
+    dense_solvers.append("daqp")
+except ImportError:
+    pass
+
+
 # ECOS
 # ====
 
 ecos_solve_problem: Optional[
     Callable[
         [
             Problem,
@@ -512,14 +554,15 @@
     )
 
 
 __all__ = [
     "available_solvers",
     "clarabel_solve_qp",
     "cvxopt_solve_qp",
+    "daqp_solve_qp",
     "dense_solvers",
     "ecos_solve_qp",
     "gurobi_solve_qp",
     "highs_solve_qp",
     "osqp_solve_qp",
     "proxqp_solve_qp",
     "qpoases_solve_qp",
```

### Comparing `qpsolvers-3.2.0/qpsolvers/solvers/clarabel_.py` & `qpsolvers-3.3.0/qpsolvers/solvers/clarabel_.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,26 +134,28 @@
     solution.obj = result.obj_val
     solution.extras = {
         "s": result.s,
         "status": result.status,
         "solve_time": result.solve_time,
     }
 
-    if result.status != clarabel.SolverStatus.Solved:
+    solution.found = result.status == clarabel.SolverStatus.Solved
+    if not solution.found:
         warnings.warn(f"Clarabel.rs terminated with status {result.status}")
-        return solution
 
     solution.x = np.array(result.x)
     meq = A.shape[0] if A is not None else 0
-    if meq > 0:
-        solution.y = result.z[:meq]
+    solution.y = result.z[:meq] if meq > 0 else np.empty((0,))
     if G is not None:
         z, z_box = split_dual_linear_box(np.array(result.z[meq:]), lb, ub)
         solution.z = z
         solution.z_box = z_box
+    else:  # G is None
+        solution.z = np.empty((0,))
+        solution.z_box = np.empty((0,))
     return solution
 
 
 def clarabel_solve_qp(
     P: Union[np.ndarray, spa.csc_matrix],
     q: np.ndarray,
     G: Optional[Union[np.ndarray, spa.csc_matrix]] = None,
@@ -209,8 +211,8 @@
     Returns
     -------
     :
         Primal solution to the QP, if found, otherwise ``None``.
     """
     problem = Problem(P, q, G, h, A, b, lb, ub)
     solution = clarabel_solve_problem(problem, initvals, verbose, **kwargs)
-    return solution.x
+    return solution.x if solution.found else None
```

### Comparing `qpsolvers-3.2.0/qpsolvers/solvers/cvxopt_.py` & `qpsolvers-3.3.0/qpsolvers/solvers/cvxopt_.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,24 +184,29 @@
         error = str(exception)
         if "Rank(A)" in error:
             raise ProblemError(error) from exception
         raise SolverError(error) from exception
 
     solution = Solution(problem)
     solution.extras = res
-    if "optimal" not in res["status"]:
-        return solution
+    solution.found = "optimal" in res["status"]
     solution.x = np.array(res["x"]).reshape((q.shape[0],))
-    if b is not None:
-        solution.y = np.array(res["y"]).reshape((b.shape[0],))
+    solution.y = (
+        np.array(res["y"]).reshape((b.shape[0],))
+        if b is not None
+        else np.empty((0,))
+    )
     if h is not None:
         z_cvx = np.array(res["z"]).reshape((h.shape[0],))
         z, z_box = split_dual_linear_box(z_cvx, lb, ub)
         solution.z = z
         solution.z_box = z_box
+    else:  # h is None
+        solution.z = np.empty((0,))
+        solution.z_box = np.empty((0,))
     solution.obj = res["primal objective"]
     return solution
 
 
 def cvxopt_solve_qp(
     P: Union[np.ndarray, spa.csc_matrix],
     q: np.ndarray,
@@ -278,8 +283,8 @@
     SolverError
         If CVXOPT failed with an error.
     """
     problem = Problem(P, q, G, h, A, b, lb, ub)
     solution = cvxopt_solve_problem(
         problem, solver, initvals, verbose, **kwargs
     )
-    return solution.x
+    return solution.x if solution.found else None
```

### Comparing `qpsolvers-3.2.0/qpsolvers/solvers/ecos_.py` & `qpsolvers-3.3.0/qpsolvers/solvers/ecos_.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,18 +143,18 @@
         A_socp = spa.hstack([A, spa.csc_matrix((A.shape[0], 1))], format="csc")
         result = solve(c_socp, G_socp, h_socp, dims, A_socp, b, **kwargs)
     else:
         result = solve(c_socp, G_socp, h_socp, dims, **kwargs)
     flag = result["info"]["exitFlag"]
     solution = Solution(problem)
     solution.extras = result["info"]
-    if flag != 0:
+    solution.found = flag == 0
+    if not solution.found:
         meaning = __exit_flag_meaning__.get(flag, "unknown exit flag")
         warnings.warn(f"ECOS returned exit flag {flag} ({meaning})")
-        return solution
     solution.x = result["x"][:-1]
     if A is not None:
         solution.y = result["y"]
     if G is not None:
         z_ecos = result["z"][: G.shape[0]]
         z, z_box = split_dual_linear_box(z_ecos, lb, ub)
         solution.z = z
@@ -248,8 +248,8 @@
     See the `ECOS Python wrapper documentation
     <https://github.com/embotech/ecos-python#calling-ecos-from-python>`_ for
     more details. You can also check out [tolerances]_ for a primer on
     primal-dual residuals or the duality gap.
     """
     problem = Problem(P, q, G, h, A, b, lb, ub)
     solution = ecos_solve_problem(problem, initvals, verbose, **kwargs)
-    return solution.x
+    return solution.x if solution.found else None
```

### Comparing `qpsolvers-3.2.0/qpsolvers/solvers/gurobi_.py` & `qpsolvers-3.3.0/qpsolvers/solvers/gurobi_.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,38 +119,38 @@
         ub_constr = model.addMConstr(identity, x, GRB.LESS_EQUAL, ub)
     objective = 0.5 * (x @ P @ x) + q @ x
     model.setObjective(objective, sense=GRB.MINIMIZE)
     model.optimize()
 
     solution = Solution(problem)
     solution.extras["status"] = model.status
-    if model.status not in (GRB.OPTIMAL, GRB.SUBOPTIMAL):
-        return solution
-    solution.x = x.X
-    __retrieve_dual(solution, ineq_constr, eq_constr, lb_constr, ub_constr)
+    solution.found = model.status in (GRB.OPTIMAL, GRB.SUBOPTIMAL)
+    if solution.found:
+        solution.x = x.X
+        __retrieve_dual(solution, ineq_constr, eq_constr, lb_constr, ub_constr)
     return solution
 
 
 def __retrieve_dual(
     solution: Solution,
     ineq_constr: Optional[gurobipy.MConstr],
     eq_constr: Optional[gurobipy.MConstr],
     lb_constr: Optional[gurobipy.MConstr],
     ub_constr: Optional[gurobipy.MConstr],
 ) -> None:
-    if ineq_constr is not None:
-        solution.z = ineq_constr.Pi
-    if eq_constr is not None:
-        solution.y = -eq_constr.Pi
+    solution.z = ineq_constr.Pi if ineq_constr is not None else np.empty((0,))
+    solution.y = -eq_constr.Pi if eq_constr is not None else np.empty((0,))
     if lb_constr is not None and ub_constr is not None:
         solution.z_box = -ub_constr.Pi - lb_constr.Pi
     elif ub_constr is not None:  # lb_constr is None
         solution.z_box = -ub_constr.Pi
     elif lb_constr is not None:  # ub_constr is None
         solution.z_box = -lb_constr.Pi
+    else:  # lb_constr is None and ub_constr is None
+        solution.z_box = np.empty((0,))
 
 
 def gurobi_solve_qp(
     P: Union[np.ndarray, spa.csc_matrix],
     q: np.ndarray,
     G: Optional[Union[np.ndarray, spa.csc_matrix]] = None,
     h: Optional[np.ndarray] = None,
@@ -234,8 +234,8 @@
 
     Lower values for primal or dual tolerances yield more precise solutions at
     the cost of computation time. See *e.g.* [tolerances]_ for a primer of
     solver tolerances.
     """
     problem = Problem(P, q, G, h, A, b, lb, ub)
     solution = gurobi_solve_problem(problem, initvals, verbose, **kwargs)
-    return solution.x
+    return solution.x if solution.found else None
```

### Comparing `qpsolvers-3.2.0/qpsolvers/solvers/highs_.py` & `qpsolvers-3.3.0/qpsolvers/solvers/highs_.py`

 * *Files 4% similar despite different names*

```diff
@@ -209,25 +209,33 @@
     solver.passModel(model)
     solver.run()
 
     result = solver.getSolution()
     model_status = solver.getModelStatus()
 
     solution = Solution(problem)
-    if model_status != highspy.HighsModelStatus.kOptimal:
-        return solution
+    solution.found = model_status == highspy.HighsModelStatus.kOptimal
     solution.x = np.array(result.col_value)
     if G is not None:
         solution.z = -np.array(result.row_dual[: G.shape[0]])
-        if A is not None:
-            solution.y = -np.array(result.row_dual[G.shape[0] :])
-    elif A is not None:  # G is None
-        solution.y = -np.array(result.row_dual)
-    if lb is not None or ub is not None:
-        solution.z_box = -np.array(result.col_dual)
+        solution.y = (
+            -np.array(result.row_dual[G.shape[0] :])
+            if A is not None
+            else np.empty((0,))
+        )
+    else:  # G is None
+        solution.z = np.empty((0,))
+        solution.y = (
+            -np.array(result.row_dual) if A is not None else np.empty((0,))
+        )
+    solution.z_box = (
+        -np.array(result.col_dual)
+        if lb is not None or ub is not None
+        else np.empty((0,))
+    )
     return solution
 
 
 def highs_solve_qp(
     P: Union[np.ndarray, spa.csc_matrix],
     q: np.ndarray,
     G: Optional[Union[np.ndarray, spa.csc_matrix]] = None,
@@ -305,8 +313,8 @@
          - Run time limit in seconds.
 
     Check out the `HiGHS documentation <https://ergo-code.github.io/HiGHS/>`_
     for more information on the solver.
     """
     problem = Problem(P, q, G, h, A, b, lb, ub)
     solution = highs_solve_problem(problem, initvals, verbose, **kwargs)
-    return solution.x
+    return solution.x if solution.found else None
```

### Comparing `qpsolvers-3.2.0/qpsolvers/solvers/osqp_.py` & `qpsolvers-3.3.0/qpsolvers/solvers/osqp_.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,26 +152,27 @@
 
     solution = Solution(problem)
     solution.extras = {
         "dual_inf_cert": res.dual_inf_cert,
         "info": res.info,
         "prim_inf_cert": res.prim_inf_cert,
     }
-    if res.info.status_val != success_status:
+    solution.found = res.info.status_val == success_status
+    if not solution.found:
         warnings.warn(f"OSQP exited with status '{res.info.status}'")
-        return solution
     solution.x = res.x
     m = G.shape[0] if G is not None else 0
     meq = A.shape[0] if A is not None else 0
-    if G is not None:
-        solution.z = res.y[:m]
-    if A is not None:
-        solution.y = res.y[m : m + meq]
-    if lb is not None or ub is not None:
-        solution.z_box = res.y[m + meq :]
+    solution.z = res.y[:m] if G is not None else np.empty((0,))
+    solution.y = res.y[m : m + meq] if A is not None else np.empty((0,))
+    solution.z_box = (
+        res.y[m + meq :]
+        if lb is not None or ub is not None
+        else np.empty((0,))
+    )
     return solution
 
 
 def osqp_solve_qp(
     P: Union[np.ndarray, csc_matrix],
     q: np.ndarray,
     G: Optional[Union[np.ndarray, csc_matrix]] = None,
@@ -281,8 +282,8 @@
 
     Lower values for absolute or relative tolerances yield more precise
     solutions at the cost of computation time. See *e.g.* [tolerances]_ for an
     overview of solver tolerances.
     """
     problem = Problem(P, q, G, h, A, b, lb, ub)
     solution = osqp_solve_problem(problem, initvals, verbose, **kwargs)
-    return solution.x
+    return solution.x if solution.found else None
```

### Comparing `qpsolvers-3.2.0/qpsolvers/solvers/proxqp_.py` & `qpsolvers-3.3.0/qpsolvers/solvers/proxqp_.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,16 +223,15 @@
         l_prox,
         u_prox,
         verbose=verbose,
         **kwargs,
     )
     solution = Solution(problem)
     solution.extras = {"info": result.info}
-    if result.info.status != proxqp.QPSolverOutput.PROXQP_SOLVED:
-        return solution
+    solution.found = result.info.status == proxqp.QPSolverOutput.PROXQP_SOLVED
     solution.x = result.x
     solution.y = result.y
     if lb is not None or ub is not None:
         solution.z = result.z[:-n]
         solution.z_box = result.z[-n:]
     else:  # lb is None and ub is None
         solution.z = result.z
@@ -302,8 +301,8 @@
     :
         Primal solution to the QP, if found, otherwise ``None``.
     """
     problem = Problem(P, q, G, h, A, b, lb, ub)
     solution = proxqp_solve_problem(
         problem, initvals, verbose, backend, **kwargs
     )
-    return solution.x
+    return solution.x if solution.found else None
```

### Comparing `qpsolvers-3.2.0/qpsolvers/solvers/qpoases_.py` & `qpsolvers-3.3.0/qpsolvers/solvers/qpoases_.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,33 +277,35 @@
     except TypeError as error:
         raise ProblemError("problem has sparse matrices") from error
 
     solution = Solution(problem)
     solution.extras = {
         "nWSR": n_wsr[0],
     }
+    solution.found = True
     if RET_INIT_FAILED <= return_value <= RET_INIT_FAILED_REGULARISATION:
-        return solution
+        solution.found = False
     if return_value == ReturnValue.MAX_NWSR_REACHED:
         warnings.warn(f"qpOASES reached the maximum number of WSR ({max_wsr})")
-        return solution
+        solution.found = False
 
     x_opt = np.empty((n,))
     z_opt = np.empty((n + C.shape[0],))
     qp.getPrimalSolution(x_opt)  # can't return RET_QP_NOT_SOLVED at this point
     qp.getDualSolution(z_opt)
     solution.x = x_opt
-    m = G.shape[0] if G is not None else 0
-    if lb is not None or ub is not None:
-        solution.z_box = -z_opt[:n]
-    if G is not None:
-        solution.z = -z_opt[n : n + m]
-    if A is not None:
-        solution.y = -z_opt[n + m : n + m + A.shape[0]]
     solution.obj = qp.getObjVal()
+    m = G.shape[0] if G is not None else 0
+    solution.y = (
+        -z_opt[n + m : n + m + A.shape[0]] if A is not None else np.empty((0,))
+    )
+    solution.z = -z_opt[n : n + m] if G is not None else np.empty((0,))
+    solution.z_box = (
+        -z_opt[:n] if lb is not None or ub is not None else np.empty((0,))
+    )
     return solution
 
 
 def qpoases_solve_qp(
     P: np.ndarray,
     q: np.ndarray,
     G: Optional[np.ndarray] = None,
@@ -420,8 +422,8 @@
         initvals,
         verbose,
         max_wsr,
         time_limit,
         predefined_options,
         **kwargs,
     )
-    return solution.x
+    return solution.x if solution.found else None
```

### Comparing `qpsolvers-3.2.0/qpsolvers/solvers/qpswift_.py` & `qpsolvers-3.3.0/qpsolvers/solvers/qpswift_.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,19 +158,17 @@
     solution = Solution(problem)
     solution.extras = {
         "basicInfo": basic_info,
         "advInfo": adv_info,
     }
     solution.obj = adv_info["fval"]
     exit_flag = basic_info["ExitFlag"]
-    if exit_flag != 0:
-        return solution
+    solution.found = exit_flag == 0
     solution.x = result["sol"]
-    if A is not None:
-        solution.y = adv_info["y"]
+    solution.y = adv_info["y"] if A is not None else np.empty((0,))
     z, z_box = split_dual_linear_box(adv_info["z"], lb, ub)
     solution.z = z
     solution.z_box = z_box
     return solution
 
 
 def qpswift_solve_qp(
@@ -302,8 +300,8 @@
     As qpSWIFT does not sanity check its inputs, it should be used with a
     little more care than the other solvers. For instance, make sure you don't
     have zero rows in your input matrices, as it can `make the solver
     numerically unstable <https://github.com/qpSWIFT/qpSWIFT/issues/3>`_.
     """
     problem = Problem(P, q, G, h, A, b, lb, ub)
     solution = qpswift_solve_problem(problem, initvals, verbose, **kwargs)
-    return solution.x
+    return solution.x if solution.found else None
```

### Comparing `qpsolvers-3.2.0/qpsolvers/solvers/quadprog_.py` & `qpsolvers-3.3.0/qpsolvers/solvers/quadprog_.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 """Solver interface for `quadprog <https://github.com/quadprog/quadprog>`__.
 
 quadprog is a C implementation of the Goldfarb-Idnani dual algorithm
 [Goldfarb1983]_. It works best on well-conditioned dense problems.
 """
 
 import warnings
-from typing import Optional, Tuple
+from typing import Optional
 
 import numpy as np
 from numpy import hstack, vstack
 from quadprog import solve_qp
 
 from ..conversions import linear_from_box_inequalities, split_dual_linear_box
 from ..exceptions import ProblemError
@@ -97,87 +97,47 @@
         meq = A.shape[0]
     else:  # no equality constraint
         if G is not None and h is not None:
             qp_C = -G.T
             qp_b = -h
         meq = 0
 
+    solution = Solution(problem)
     try:
         x, obj, xu, iterations, y, iact = solve_qp(
             qp_G, qp_a, qp_C, qp_b, meq, **kwargs
         )
+        solution.found = True
+        solution.x = x
+        solution.obj = obj
+
+        z, z_box = split_dual_linear_box(y[meq:], lb, ub)
+        solution.y = y[:meq] if meq > 0 else np.empty((0,))
+        solution.z = z
+        solution.z_box = z_box
+
+        solution.extras = {
+            "iact": iact,
+            "iterations": iterations,
+            "xu": xu,
+        }
     except TypeError as error:
         raise ProblemError("problem has sparse matrices") from error
     except ValueError as error:
+        solution.found = False
         error_message = str(error)
         if "matrix G is not positive definite" in error_message:
             # quadprog writes G the cost matrix that we write P in this package
             raise ProblemError("matrix P is not positive definite") from error
-        no_solution = Solution(problem)
-        if "no solution" in error_message:
-            return no_solution
-        warnings.warn(f"quadprog raised a ValueError: {error_message}")
-        return no_solution
-
-    solution = Solution(problem)
-    solution.x = x
-    solution.obj = obj
+        if "no solution" not in error_message:
+            warnings.warn(f"quadprog raised a ValueError: {error_message}")
 
-    z, ys, z_box = __convert_dual_multipliers(y, meq, lb, ub)
-    solution.y = ys
-    solution.z = z
-    solution.z_box = z_box
-
-    solution.extras = {
-        "iact": iact,
-        "iterations": iterations,
-        "xu": xu,
-    }
     return solution
 
 
-def __convert_dual_multipliers(
-    y: np.ndarray,
-    meq: int,
-    lb: Optional[np.ndarray],
-    ub: Optional[np.ndarray],
-) -> Tuple[Optional[np.ndarray], Optional[np.ndarray], Optional[np.ndarray]]:
-    """Convert dual multipliers from quadprog to qpsolvers QP formulation.
-
-    Parameters
-    ----------
-    y :
-        Dual multipliers from quadprog.
-    meq :
-        Number of equality constraints.
-    lb :
-        Lower bound vector for box inequalities, if any.
-    ub :
-        Upper bound vector for box inequalities, if any.
-
-    Returns
-    -------
-    :
-        Tuple of dual multipliers :code:`z, ys, z_box` corresponding
-        respectively to linear inequalities, linear equalities, and box
-        inequalities.
-
-    Raises
-    ------
-    ProblemError :
-        If the problem is ill-formed in some way, for instance if some matrices
-        are not dense.
-    """
-    z, ys, z_box = None, None, None
-    if meq > 0:
-        ys = y[:meq]
-    z, z_box = split_dual_linear_box(y[meq:], lb, ub)
-    return z, ys, z_box
-
-
 def quadprog_solve_qp(
     P: np.ndarray,
     q: np.ndarray,
     G: Optional[np.ndarray] = None,
     h: Optional[np.ndarray] = None,
     A: Optional[np.ndarray] = None,
     b: Optional[np.ndarray] = None,
@@ -230,8 +190,8 @@
     Returns
     -------
     :
         Primal solution to the QP, if found, otherwise ``None``.
     """
     problem = Problem(P, q, G, h, A, b, lb, ub)
     solution = quadprog_solve_problem(problem, initvals, verbose, **kwargs)
-    return solution.x
+    return solution.x if solution.found else None
```

### Comparing `qpsolvers-3.2.0/qpsolvers/solvers/scs_.py` & `qpsolvers-3.3.0/qpsolvers/solvers/scs_.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,27 +184,32 @@
         __add_box_cone(n, lb, ub, cone, data)
     kwargs["verbose"] = verbose
     result = solve(data, cone, **kwargs)
 
     solution = Solution(problem)
     solution.extras = result["info"]
     status_val = result["info"]["status_val"]
-    if status_val != 1:
+    solution.found = status_val == 1
+    if not solution.found:
         warnings.warn(
             f"SCS returned {status_val}: {__status_val_meaning__[status_val]}"
         )
-        return solution
     solution.x = result["x"]
     meq = A.shape[0] if A is not None else 0
-    if A is not None:
-        solution.y = result["y"][:meq]
-    if G is not None:
-        solution.z = result["y"][meq : meq + G.shape[0]]
-    if lb is not None or ub is not None:
-        solution.z_box = -result["y"][-n:]
+    solution.y = result["y"][:meq] if A is not None else np.empty((0,))
+    solution.z = (
+        result["y"][meq : meq + G.shape[0]]
+        if G is not None
+        else np.empty((0,))
+    )
+    solution.z_box = (
+        -result["y"][-n:]
+        if lb is not None or ub is not None
+        else np.empty((0,))
+    )
     return solution
 
 
 def scs_solve_qp(
     P: Union[ndarray, csc_matrix],
     q: ndarray,
     G: Optional[Union[ndarray, csc_matrix]] = None,
@@ -300,8 +305,8 @@
 
     Check out the `SCS settings
     <https://www.cvxgrp.org/scs/api/settings.html#settings>`_ documentation for
     all available settings.
     """
     problem = Problem(P, q, G, h, A, b, lb, ub)
     solution = scs_solve_problem(problem, initvals, verbose, **kwargs)
-    return solution.x
+    return solution.x if solution.found else None
```

### Comparing `qpsolvers-3.2.0/qpsolvers/unsupported/__init__.py` & `qpsolvers-3.3.0/qpsolvers/unsupported/__init__.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/qpsolvers/unsupported/mosek_.py` & `qpsolvers-3.3.0/qpsolvers/unsupported/mosek_.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,8 +138,8 @@
     Returns
     -------
     :
         Solution to the QP, if found, otherwise ``None``.
     """
     problem = Problem(P, q, G, h, A, b, lb, ub)
     solution = mosek_solve_problem(problem, initvals, verbose, **kwargs)
-    return solution.x
+    return solution.x if solution.found else None
```

### Comparing `qpsolvers-3.2.0/qpsolvers/unsupported/nppro_.py` & `qpsolvers-3.3.0/qpsolvers/unsupported/nppro_.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,26 +134,23 @@
     x0 = np.asarray(x0, order="C", dtype=np.float64)
 
     # Call solver
     x, fval, exitflag, iter_ = solver.solve(P, q, A_, l_, u_, lb_, ub_, x0)
 
     # Store solution
     solution = Solution(problem)
-    if exitflag != 0 or np.isnan(x).any():
+    solution.found = exitflag == 0 and not np.isnan(x).any()
+    if not solution.found:
         # The second condition typically handle positive semi-definite cases
         # that are not catched by the solver yet
         warnings.warn(f"NPPro exited with status {exitflag}")
-        return solution
     solution.x = x
-    if G is not None:
-        solution.z = None  # not available yet
-    if A is not None:
-        solution.y = None  # not available yet
-    if lb is not None or ub is not None:
-        solution.z_box = None  # not available yet
+    solution.z = None  # not available yet
+    solution.y = None  # not available yet
+    solution.z_box = None  # not available yet
     solution.extras = {
         "cost": fval,
         "iter": iter_,
     }
     return solution
 
 
@@ -214,8 +211,8 @@
 
     Notes
     -----
     See the Notes section in :func:`nppro_solve_problem`.
     """
     problem = Problem(P, q, G, h, A, b, lb, ub)
     solution = nppro_solve_problem(problem, initvals, **kwargs)
-    return solution.x
+    return solution.x if solution.found else None
```

### Comparing `qpsolvers-3.2.0/qpsolvers/utils.py` & `qpsolvers-3.3.0/qpsolvers/utils.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/problems.py` & `qpsolvers-3.3.0/tests/problems.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/solved_problems.py` & `qpsolvers-3.3.0/qpsolvers/problems.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2016-2022 Stéphane Caron and the qpsolvers contributors.
+# Copyright (C) 2016-2023 the qpsolvers contributors.
 #
 # This file is part of qpsolvers.
 #
 # qpsolvers is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
@@ -14,47 +14,102 @@
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with qpsolvers. If not, see <http://www.gnu.org/licenses/>.
 
-"""Reference problems with their solutions.
+"""Collection of sample problems."""
 
-The prefix "QPSUT" stands for "qpsolvers unit test".
-"""
+from typing import Tuple
 
 import numpy as np
+import scipy.sparse as spa
 
-from qpsolvers import Problem, Solution
+from .problem import Problem
+from .solution import Solution
 
 
-def get_qpsut01() -> Solution:
-    """Get QPSUT01 problem and its solution."""
+def get_sparse_least_squares(n):
+    """
+    Get a sparse least squares problem.
+
+    Parameters
+    ----------
+    n :
+        Problem size.
+
+    Notes
+    -----
+    This problem was inspired by `this question on Stack Overflow
+    <https://stackoverflow.com/q/73656257/3721564>`__.
+    """
+    # minimize 1/2 || x - s ||^2
+    R = spa.eye(n, format="csc")
+    s = np.array(range(n), dtype=float)
+
+    # such that G * x <= h
+    G = spa.diags(
+        diagonals=[
+            [1.0 if i % 2 == 0 else 0.0 for i in range(n)],
+            [1.0 if i % 3 == 0 else 0.0 for i in range(n - 1)],
+            [1.0 if i % 5 == 0 else 0.0 for i in range(n - 1)],
+        ],
+        offsets=[0, 1, -1],
+        format="csc",
+    )
+    h = np.ones(G.shape[0])
+
+    # such that sum(x) == 42
+    A = spa.csc_matrix(np.ones((1, n)))
+    b = np.array([42.0]).reshape((1,))
+
+    # such that x >= 0
+    lb = np.zeros(n)
+    ub = None
+
+    return R, s, G, h, A, b, lb, ub
+
+
+def get_qpsut01() -> Tuple[Problem, Solution]:
+    """Get QPSUT01 problem and its solution.
+
+    Returns
+    -------
+    :
+        Problem-solution pair.
+    """
     M = np.array([[1.0, 2.0, 0.0], [-8.0, 3.0, 2.0], [0.0, 1.0, 1.0]])
     P = np.dot(M.T, M)  # this is a positive definite matrix
     q = np.dot(np.array([3.0, 2.0, 3.0]), M)
     G = np.array([[4.0, 2.0, 0.0], [-1.0, 2.0, -1.0]])
     h = np.array([1.0, -2.0])
     A = np.array([1.0, 1.0, 1.0]).reshape((1, 3))
     b = np.array([1.0])
     lb = np.array([-0.5, -0.4, -0.5])
     ub = np.array([1.0, 1.0, 1.0])
     problem = Problem(P, q, G, h, A, b, lb, ub)
 
     solution = Solution(problem)
+    solution.found = True
     solution.x = np.array([0.4, -0.4, 1.0])
     solution.z = np.array([0.0, 0.0])
     solution.y = np.array([-5.8])
     solution.z_box = np.array([0.0, -1.8, 3.0])
-    return solution
+    return problem, solution
 
 
-def get_qpsut02() -> Solution:
-    """Get QPSUT02 problem and its solution."""
+def get_qpsut02() -> Tuple[Problem, Solution]:
+    """Get QPSUT02 problem and its solution.
+
+    Returns
+    -------
+    :
+        Problem-solution pair.
+    """
     M = np.array(
         [
             [1.0, -2.0, 0.0, 8.0],
             [-6.0, 3.0, 1.0, 4.0],
             [-2.0, 1.0, 0.0, 1.0],
             [9.0, 9.0, 5.0, 3.0],
         ]
@@ -75,24 +130,30 @@
     )
     b = np.array([10.0, 0.0])
     lb = np.array([-2.0, -1.0, -3.0, 1.0])
     ub = np.array([4.0, 2.0, 6.0, 10.0])
     problem = Problem(P, q, G, h, A, b, lb, ub)
 
     solution = Solution(problem)
+    solution.found = True
     solution.x = np.array([1.36597938, -1.0, 6.0, 3.63402062])
     solution.z = np.array([0.0])
     solution.y = np.array([-377.60314303, -62.75251185])  # YMMV
     solution.z_box = np.array([0.0, -138.9585918, 37.53106937, 0.0])  # YMMV
-    return solution
+    return problem, solution
 
 
-def get_qpsut03() -> Solution:
+def get_qpsut03() -> Tuple[Problem, Solution]:
     """Get QPSUT03 problem and its solution.
 
+    Returns
+    -------
+    :
+        Problem-solution pair.
+
     Notes
     -----
     This problem has partial box bounds, that is, -infinity on some lower
     bounds and +infinity on some upper bounds.
     """
     M = np.array(
         [
@@ -109,62 +170,80 @@
     A = None
     b = None
     lb = np.array([-np.inf, -0.4, -np.inf, -1.0])
     ub = np.array([np.inf, np.inf, 0.5, 1.0])
     problem = Problem(P, q, G, h, A, b, lb, ub)
 
     solution = Solution(problem)
-    solution.x = np.array([0.4, -0.4, 1.0])
-    solution.z = np.array([0.0, 0.0])
-    solution.y = np.array([-5.8])
-    solution.z_box = np.array([0.0, -1.8, 3.0])
-    return solution
-
-
-def get_maros_meszaros_qptest():
-    """Get QPTEST problem from the Maros-Meszaros test set."""
-    P = np.array([[8.0, 2.0], [2.0, 10.0]])
-    q = np.array([1.5, -2.0])
-    G = np.array([[-1.0, 2.0], [-2.0, -1.0]])
-    h = np.array([6.0, -2.0])
-    lb = np.array([0.0, 0.0])
-    ub = np.array([20.0, np.inf])
-    problem = Problem(P, q, G, h, lb=lb, ub=ub)
-
-    solution = Solution(problem)
-    solution.x = np.array([0.7625, 0.475])
-    solution.z = np.array([0.0, 4.275])
-    solution.z_box = np.array([0.0, 0.0])
-    return solution
+    solution.found = True
+    solution.x = np.array([0.18143455, 0.00843864, -2.35442995, 0.35443034])
+    solution.z = np.array([])
+    solution.y = np.array([])
+    solution.z_box = np.array([0.0, 0.0, 0.0, 0.0])
+    return problem, solution
 
 
-def get_qpsut04() -> Solution:
-    """
-    Get QPSUT04 problem and its solution.
+def get_qpsut04() -> Tuple[Problem, Solution]:
+    """Get QPSUT04 problem and its solution.
+
+    Returns
+    -------
+    :
+        Problem-solution pair.
     """
     n = 3
     P = np.eye(n)
     q = 0.01 * np.ones(shape=(n, 1))  # non-flat vector
     G = np.eye(n)
     h = np.ones(shape=(n,))
     A = np.ones(shape=(n,))
     b = np.ones(shape=(1,))
     problem = Problem(P, q, G, h, A, b)
 
     solution = Solution(problem)
+    solution.found = True
     solution.x = 1.0 / 3.0 * np.ones(n)
     solution.y = np.array([1.0 / 3.0 + 0.01])
     solution.z = np.zeros(n)
-    return solution
+    return problem, solution
 
 
-def get_qpsut05() -> Solution:
-    """
-    Get QPSUT05 problem and its solution.
+def get_qpsut05() -> Tuple[Problem, Solution]:
+    """Get QPSUT05 problem and its solution.
+
+    Returns
+    -------
+    :
+        Problem-solution pair.
     """
     P = np.array([2.0])
     q = np.array([-2.0])
     problem = Problem(P, q)
 
     solution = Solution(problem)
+    solution.found = True
     solution.x = np.array([1.0])
-    return solution
+    return problem, solution
+
+
+def get_qptest():
+    """Get QPTEST problem from the Maros-Meszaros test set.
+
+    Returns
+    -------
+    :
+        Problem-solution pair.
+    """
+    P = np.array([[8.0, 2.0], [2.0, 10.0]])
+    q = np.array([1.5, -2.0])
+    G = np.array([[-1.0, 2.0], [-2.0, -1.0]])
+    h = np.array([6.0, -2.0])
+    lb = np.array([0.0, 0.0])
+    ub = np.array([20.0, np.inf])
+    problem = Problem(P, q, G, h, lb=lb, ub=ub)
+
+    solution = Solution(problem)
+    solution.found = True
+    solution.x = np.array([0.7625, 0.475])
+    solution.z = np.array([0.0, 4.275])
+    solution.z_box = np.array([0.0, 0.0])
+    return problem, solution
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qpsolvers-3.2.0/tests/test_clarabel.py` & `qpsolvers-3.3.0/tests/test_clarabel.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,42 +19,40 @@
 # along with qpsolvers. If not, see <http://www.gnu.org/licenses/>.
 
 """Unit tests for Clarabel."""
 
 import unittest
 import warnings
 
-from .solved_problems import get_qpsut01
+from qpsolvers.problems import get_qpsut01
 
 try:
     import clarabel
 
     from qpsolvers.solvers.clarabel_ import clarabel_solve_problem
 
     class TestClarabel(unittest.TestCase):
         """Test fixture for the Clarabel.rs solver."""
 
         def test_time_limit(self):
             """Call Clarabel.rs with an infeasibly low time limit."""
-            ref_solution = get_qpsut01()
-            problem = ref_solution.problem
+            problem, ref_solution = get_qpsut01()
             solution = clarabel_solve_problem(problem, time_limit=1e-10)
             status = solution.extras["status"]
             self.assertEqual(status, clarabel.SolverStatus.MaxTime)
             # See https://github.com/oxfordcontrol/Clarabel.rs/issues/10
             self.assertFalse(status != clarabel.SolverStatus.MaxTime)
 
         def test_status(self):
             """Check that result status is consistent with its string repr.
 
             Context: https://github.com/oxfordcontrol/Clarabel.rs/issues/10
             """
-            problem = get_qpsut01().problem
+            problem, _ = get_qpsut01()
             solution = clarabel_solve_problem(problem)
             status = solution.extras["status"]
             check_1 = str(status) != "Solved"
             check_2 = status != clarabel.SolverStatus.Solved
             self.assertEqual(check_1, check_2)
 
-
 except ImportError:  # solver not installed
     warnings.warn("Skipping Clarabel.rs tests as the solver is not installed")
```

### Comparing `qpsolvers-3.2.0/tests/test_conversions.py` & `qpsolvers-3.3.0/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/test_cvxopt.py` & `qpsolvers-3.3.0/tests/test_cvxopt.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 import numpy as np
 import scipy.sparse as spa
 from numpy import array, ones
 from numpy.linalg import norm
 
 from .problems import get_sd3310_problem
-from .solved_problems import get_qpsut01
+from qpsolvers.problems import get_qpsut01
 
 try:
     import cvxopt
 
     from qpsolvers.solvers.cvxopt_ import cvxopt_solve_problem, cvxopt_solve_qp
 
     class TestCVXOPT(unittest.TestCase):
@@ -97,22 +97,22 @@
                 feastol=1e-2,
                 refinement=3,
             )
             self.assertIsNotNone(x)
 
         def test_infinite_linear_bounds(self):
             """CVXOPT does not yield a domain error on infinite bounds."""
-            problem = get_qpsut01().problem
+            problem, _ = get_qpsut01()
             problem.h[1] = +np.inf
             x = cvxopt_solve_problem(problem)
             self.assertIsNotNone(x)
 
         def test_infinite_box_bounds(self):
             """CVXOPT does not yield a domain error infinite box bounds."""
-            problem = get_qpsut01().problem
+            problem, _ = get_qpsut01()
             problem.lb[1] = -np.inf
             problem.ub[1] = +np.inf
             x = cvxopt_solve_problem(problem)
             self.assertIsNotNone(x)
 
 
 except ImportError:  # solver not installed
```

### Comparing `qpsolvers-3.2.0/tests/test_ecos.py` & `qpsolvers-3.3.0/tests/test_ecos.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/test_gurobi.py` & `qpsolvers-3.3.0/tests/test_gurobi.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/test_highs.py` & `qpsolvers-3.3.0/tests/test_scs.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,42 +14,39 @@
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with qpsolvers. If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for HiGHS."""
+"""Unit tests for SCS."""
 
 import unittest
 import warnings
 
+import numpy as np
+
+from qpsolvers import ProblemError
+
 from .problems import get_sd3310_problem
 
 try:
-    from qpsolvers.solvers.highs_ import highs_solve_qp
+    from qpsolvers.solvers.scs_ import scs_solve_qp
 
-    class TestHiGHS(unittest.TestCase):
-        """Test fixture for the HiGHS solver."""
+    class TestSCS(unittest.TestCase):
+        """Tests specific to SCS."""
 
-        def setUp(self):
-            """Prepare test fixture."""
-            warnings.simplefilter("ignore", category=UserWarning)
+        def test_problem(self):
+            problem = get_sd3310_problem()
+            P, q, G, h, A, b, lb, ub = problem.unpack()
+            self.assertIsNotNone(scs_solve_qp(P, q, G, h, A, b, lb, ub))
 
-        def test_highs_tolerances(self):
+        def test_unbounded_below(self):
             problem = get_sd3310_problem()
-            x = highs_solve_qp(
-                problem.P,
-                problem.q,
-                problem.G,
-                problem.h,
-                problem.A,
-                problem.b,
-                time_limit=0.1,
-                primal_feasibility_tolerance=1e-1,
-                dual_feasibility_tolerance=1e-1,
-            )
-            self.assertIsNotNone(x)
+            P, q, _, _, _, _, _, _ = problem.unpack()
+            P -= np.eye(3)  # make problem unbounded
+            with self.assertRaises(ProblemError):
+                scs_solve_qp(P, q)
 
 
 except ImportError:  # solver not installed
-    warnings.warn("Skipping HiGHS tests as the solver is not installed")
+    warnings.warn("Skipping SCS tests as the solver is not installed")
```

### Comparing `qpsolvers-3.2.0/tests/test_mosek.py` & `qpsolvers-3.3.0/tests/test_mosek.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/test_nppro.py` & `qpsolvers-3.3.0/tests/test_nppro.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/test_osqp.py` & `qpsolvers-3.3.0/tests/test_osqp.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/test_problem.py` & `qpsolvers-3.3.0/tests/test_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/test_proxqp.py` & `qpsolvers-3.3.0/tests/test_proxqp.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/test_qpoases.py` & `qpsolvers-3.3.0/tests/test_qpoases.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/test_qpswift.py` & `qpsolvers-3.3.0/tests/test_qpswift.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/test_quadprog.py` & `qpsolvers-3.3.0/tests/test_quadprog.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/test_solution.py` & `qpsolvers-3.3.0/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/test_solve_ls.py` & `qpsolvers-3.3.0/tests/test_solve_ls.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/test_solve_problem.py` & `qpsolvers-3.3.0/tests/test_solve_problem.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,22 +23,21 @@
 import math
 import unittest
 
 import numpy as np
 from numpy.linalg import norm
 
 from qpsolvers import available_solvers, solve_problem
-
-from .solved_problems import (
-    get_maros_meszaros_qptest,
+from qpsolvers.problems import (
     get_qpsut01,
     get_qpsut02,
     get_qpsut03,
     get_qpsut04,
     get_qpsut05,
+    get_qptest,
 )
 
 
 class TestSolveProblem(unittest.TestCase):
     """Test fixture for primal and dual solutions of a variety of problems.
 
     Notes
@@ -61,16 +60,15 @@
         Returns
         -------
         test : function
             Test function for that solver.
         """
 
         def test(self):
-            ref_solution = get_qpsut01()
-            problem = ref_solution.problem
+            problem, ref_solution = get_qpsut01()
             solution = solve_problem(problem, solver=solver)
             eps_abs = (
                 5e-1
                 if solver == "osqp"
                 else 5e-3
                 if solver == "proxqp"
                 else 1e-4
@@ -101,16 +99,15 @@
         Returns
         -------
         test : function
             Test function for that solver.
         """
 
         def test(self):
-            ref_solution = get_qpsut02()
-            problem = ref_solution.problem
+            problem, ref_solution = get_qpsut02()
             solution = solve_problem(problem, solver=solver)
             eps_abs = (
                 5e-2
                 if solver == "ecos"
                 else 5e-4
                 if solver in ["proxqp", "scs"]
                 else 1e-4
@@ -142,17 +139,23 @@
         Returns
         -------
         test : function
             Test function for that solver.
         """
 
         def test(self):
-            ref_solution = get_qpsut03()
-            problem = ref_solution.problem
+            problem, ref_solution = get_qpsut03()
             solution = solve_problem(problem, solver=solver)
+            self.assertEqual(solution.y.shape, (0,))
+            self.assertEqual(solution.z.shape, (0,))
+            self.assertAlmostEqual(
+                np.linalg.norm(solution.z_box),
+                0.0,
+                places=3 if solver == "cvxopt" else 7,
+            )
             self.assertFalse(math.isnan(solution.duality_gap()))
 
         return test
 
     @staticmethod
     def get_test_qpsut04(solver: str):
         """
@@ -166,16 +169,15 @@
         Returns
         -------
         test : function
             Test function for that solver.
         """
 
         def test(self):
-            ref_solution = get_qpsut04()
-            problem = ref_solution.problem
+            problem, ref_solution = get_qpsut04()
             solution = solve_problem(problem, solver=solver)
             eps_abs = 2e-4 if solver == "osqp" else 1e-6
             self.assertLess(norm(solution.x - ref_solution.x), eps_abs)
             self.assertLess(norm(solution.z - ref_solution.z), eps_abs)
             self.assertTrue(np.isfinite(solution.duality_gap()))
 
         return test
@@ -193,25 +195,24 @@
         Returns
         -------
         test : function
             Test function for that solver.
         """
 
         def test(self):
-            ref_solution = get_qpsut05()
-            problem = ref_solution.problem
+            problem, ref_solution = get_qpsut05()
             solution = solve_problem(problem, solver=solver)
             eps_abs = 2e-5 if solver == "ecos" else 1e-6
             self.assertLess(norm(solution.x - ref_solution.x), eps_abs)
             self.assertTrue(np.isfinite(solution.duality_gap()))
 
         return test
 
     @staticmethod
-    def get_test_maros_meszaros_qptest(solver):
+    def get_test_qptest(solver):
         """Get test function for the QPTEST problem.
 
         Parameters
         ----------
         solver : string
             Name of the solver to test.
 
@@ -222,16 +223,15 @@
 
         Note
         ----
         ECOS fails to solve this problem.
         """
 
         def test(self):
-            solution = get_maros_meszaros_qptest()
-            problem = solution.problem
+            problem, solution = get_qptest()
             result = solve_problem(problem, solver=solver)
             tolerance = (
                 1e1
                 if solver == "gurobi"
                 else 1.0
                 if solver == "proxqp"
                 else 2e-3
@@ -267,15 +267,15 @@
         Returns
         -------
         test : function
             Test function for that solver.
         """
 
         def test(self):
-            problem = get_qpsut01().problem
+            problem, _ = get_qpsut01()
             problem.lb[1] = -np.inf
             problem.ub[1] = +np.inf
             result = solve_problem(problem, solver=solver)
             self.assertIsNotNone(result.x)
             self.assertIsNotNone(result.z)
             self.assertIsNotNone(result.z_box)
 
@@ -293,15 +293,15 @@
         Returns
         -------
         test : function
             Test function for that solver.
         """
 
         def test(self):
-            problem = get_qpsut01().problem
+            problem, _ = get_qpsut01()
             problem.h[0] = +np.inf
             result = solve_problem(problem, solver=solver)
             self.assertIsNotNone(result.x)
             self.assertIsNotNone(result.z)
             self.assertIsNotNone(result.z_box)
 
         return test
@@ -315,38 +315,41 @@
         TestSolveProblem.get_test_qpsut01(solver),
     )
     setattr(
         TestSolveProblem,
         f"test_qpsut02_{solver}",
         TestSolveProblem.get_test_qpsut02(solver),
     )
-    setattr(
-        TestSolveProblem,
-        f"test_qpsut03_{solver}",
-        TestSolveProblem.get_test_qpsut03(solver),
-    )
+    if solver not in ["ecos", "qpswift"]:
+        # ECOS: https://github.com/qpsolvers/qpsolvers/issues/160
+        # qpSWIFT: https://github.com/qpsolvers/qpsolvers/issues/159
+        setattr(
+            TestSolveProblem,
+            f"test_qpsut03_{solver}",
+            TestSolveProblem.get_test_qpsut03(solver),
+        )
     setattr(
         TestSolveProblem,
         f"test_qpsut04_{solver}",
         TestSolveProblem.get_test_qpsut04(solver),
     )
     if solver not in ["osqp", "qpswift"]:
         # OSQP: see https://github.com/osqp/osqp-python/issues/104
         setattr(
             TestSolveProblem,
             f"test_qpsut05_{solver}",
             TestSolveProblem.get_test_qpsut05(solver),
         )
     if solver not in ["ecos", "qpswift"]:
-        # See https://github.com/qpsolvers/qpsolvers/issues/159
-        # See https://github.com/qpsolvers/qpsolvers/issues/160
+        # ECOS: https://github.com/qpsolvers/qpsolvers/issues/160
+        # qpSWIFT: https://github.com/qpsolvers/qpsolvers/issues/159
         setattr(
             TestSolveProblem,
-            f"test_maros_meszaros_qptest_{solver}",
-            TestSolveProblem.get_test_maros_meszaros_qptest(solver),
+            f"test_qptest_{solver}",
+            TestSolveProblem.get_test_qptest(solver),
         )
     if solver not in ["ecos", "qpswift"]:
         # See https://github.com/qpsolvers/qpsolvers/issues/159
         # See https://github.com/qpsolvers/qpsolvers/issues/160
         setattr(
             TestSolveProblem,
             f"test_infinite_box_bounds_{solver}",
```

### Comparing `qpsolvers-3.2.0/tests/test_solve_qp.py` & `qpsolvers-3.3.0/tests/test_solve_qp.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/test_unfeasible_problem.py` & `qpsolvers-3.3.0/tests/test_unfeasible_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tests/test_utils.py` & `qpsolvers-3.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.2.0/tox.ini` & `qpsolvers-3.3.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     macos-latest: macos
     windows-latest: windows
 
 [testenv]
 deps =
     clarabel >=0.4.1
     cvxopt >=1.2.6
+    daqp >=0.5.0
     ecos >=2.0.8
     gurobipy >=9.5.2
     numpy <1.24.0
     osqp >=0.6.2
     quadprog >=0.1.11
     scipy >=1.2.0
     scs >=3.2.0
@@ -34,14 +35,15 @@
     python -m unittest discover
 
 [testenv:coverage]
 deps =
     clarabel >=0.4.1
     coverage >=5.5
     cvxopt >=1.2.6
+    daqp >=0.5.0
     ecos >=2.0.8
     gurobipy >=9.5.2
     highspy >=1.1.2.dev3
     numpy <1.24.0
     osqp >=0.6.2
     proxsuite >=0.3.1
     quadprog >=0.1.11
@@ -69,13 +71,13 @@
 ; E0611: No name 'solve_qp' in module 'quadprog' (false positive, we have mypy to cover such errors)
 ; E1130: bad operand type for unary - (false positives fixed in newer versions of pylint, see https://github.com/PyCQA/pylint/issues/2436, anyhow we have mypy to cover such errors)
 ; R0801: Similar lines in * files (all our functions have the same prototype)
 ; R0902: Too many instance attributes (our QP formulation has 8 > 7)
 ; R0913: Too many arguments (our functions have more than 5 arguments)
 ; R0914: Too many local variables (our functions usually have more than 15 local variables)
 disable=C0103, E0611, E1130, R0801, R0902, R0913, R0914, import-error
-generated-members=gurobipy.Model, gurobipy.MConstr, proxsuite.proxqp, qpSWIFT.run
+generated-members=clarabel.DefaultSettings, clarabel.DefaultSolver, clarabel.NonnegativeConeT, clarabel.SolverStatus, clarabel.ZeroConeT, daqp.solve, gurobipy.Model, gurobipy.MConstr, proxsuite.proxqp, qpSWIFT.run
 
 [mypy]
 disable_error_code = attr-defined, name-defined
 ignore_missing_imports = True
 warn_no_return = True
```

### Comparing `qpsolvers-3.2.0/PKG-INFO` & `qpsolvers-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qpsolvers
-Version: 3.2.0
+Version: 3.3.0
 Summary: Quadratic programming solvers in Python with a unified API.
 Keywords: quadratic programming,solver,numerical optimization
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Dist: daqp >=0.5.0
 Requires-Dist: ecos >=2.0.8
 Requires-Dist: numpy >=1.15.4
 Requires-Dist: osqp >=0.6.2
 Requires-Dist: scipy >=1.2.0
 Requires-Dist: scs >=3.2.0
 Requires-Dist: clarabel >=0.4.1 ; extra == "open_source_solvers"
 Requires-Dist: cvxopt >=1.2.6 ; extra == "open_source_solvers"
@@ -109,14 +110,15 @@
 
 ## Solvers
 
 | Solver | Keyword | Algorithm | API | License | Warm-start |
 | ------ | ------- | --------- | --- | ------- |------------|
 | [Clarabel](https://github.com/oxfordcontrol/Clarabel.rs) | ``clarabel`` | Interior point | Sparse | Apache-2.0 | ✖️ |
 | [CVXOPT](http://cvxopt.org/) | ``cvxopt`` | Interior point | Dense | GPL-3.0 | ✔️ |
+| [DAQP](https://github.com/darnstrom/daqp) | ``daqp`` | Active set | Dense | MIT | ✖️ |
 | [ECOS](https://web.stanford.edu/~boyd/papers/ecos.html) | ``ecos`` | Interior point | Sparse | GPL-3.0 | ✖️ |
 | [Gurobi](https://www.gurobi.com/) | ``gurobi`` | Interior point | Sparse | Commercial | ✖️ |
 | [HiGHS](https://highs.dev/) | ``highs`` | Active set | Sparse | MIT | ✖️ |
 | [MOSEK](https://mosek.com/) | ``mosek`` | Interior point | Sparse | Commercial | ✔️ |
 | NPPro | ``nppro`` | Active set | Dense | Commercial | ✔️ |
 | [OSQP](https://osqp.org/) | ``osqp`` | Augmented Lagrangian | Sparse | Apache-2.0 | ✔️ |
 | [ProxQP](https://github.com/Simple-Robotics/proxsuite) | ``proxqp`` | Augmented Lagrangian | Dense & Sparse | BSD-2-Clause | ✔️ |
```

