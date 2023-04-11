# Comparing `tmp/science_optimization-9.0.1.tar.gz` & `tmp/science_optimization-9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "science_optimization-9.0.1.tar", max compression
+gzip compressed data, was "science_optimization-9.0.2.tar", max compression
```

## Comparing `science_optimization-9.0.1.tar` & `science_optimization-9.0.2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0      250 2022-11-08 13:42:14.460435 science_optimization-9.0.1/LICENSE
--rw-r--r--   0        0        0    11780 2022-11-08 13:53:18.706299 science_optimization-9.0.1/README.md
--rw-r--r--   0        0        0     3137 2023-03-23 19:11:45.733736 science_optimization-9.0.1/build.py
--rw-r--r--   0        0        0     1058 2023-04-10 17:53:18.176530 science_optimization-9.0.1/pyproject.toml
--rw-r--r--   0        0        0      193 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/__init__.py
--rw-r--r--   0        0        0      272 2023-03-23 19:11:41.489780 science_optimization-9.0.1/science_optimization/algorithms/__init__.py
--rw-r--r--   0        0        0      901 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/base_algorithms.py
--rw-r--r--   0        0        0       85 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/cutting_plane/__init__.py
--rw-r--r--   0        0        0     6028 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/cutting_plane/ellipsoid_method.py
--rw-r--r--   0        0        0       89 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/decomposition/__init__.py
--rw-r--r--   0        0        0     7106 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/decomposition/dual_decomposition.py
--rw-r--r--   0        0        0       77 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/derivative_free/__init__.py
--rw-r--r--   0        0        0    17247 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/derivative_free/nelder_mead.py
--rw-r--r--   0        0        0       88 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/lagrange/__init__.py
--rw-r--r--   0        0        0     5177 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/lagrange/augmented_lagrangian.py
--rw-r--r--   0        0        0      233 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/linear_programming/__init__.py
--rw-r--r--   0        0        0     4543 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/linear_programming/glop.py
--rw-r--r--   0        0        0     3347 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/linear_programming/scipy_base_linear.py
--rw-r--r--   0        0        0      429 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/linear_programming/scipy_interior_point_method.py
--rw-r--r--   0        0        0      395 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/linear_programming/scipy_simplex_method.py
--rw-r--r--   0        0        0      231 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/search_direction/__init__.py
--rw-r--r--   0        0        0     9608 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/search_direction/base_search_direction.py
--rw-r--r--   0        0        0      731 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/search_direction/gradient_algorithm.py
--rw-r--r--   0        0        0      589 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/search_direction/newton_algorithm.py
--rw-r--r--   0        0        0     3121 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/search_direction/quasi_newton.py
--rw-r--r--   0        0        0      197 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/unidimensional/__init__.py
--rw-r--r--   0        0        0     1824 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/unidimensional/base_unidimensional.py
--rw-r--r--   0        0        0     1305 2023-04-10 17:48:13.277434 science_optimization-9.0.1/science_optimization/algorithms/unidimensional/golden_section.py
--rw-r--r--   0        0        0     5579 2023-03-23 19:11:41.493780 science_optimization-9.0.1/science_optimization/algorithms/unidimensional/multimodal_golden_section.py
--rw-r--r--   0        0        0       63 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/utils/__init__.py
--rw-r--r--   0        0        0     4684 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/algorithms/utils/algorithms_utils.py
--rw-r--r--   0        0        0      255 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/builder/__init__.py
--rw-r--r--   0        0        0      504 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/builder/__init__.pyc
--rw-r--r--   0        0        0      446 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/builder/builder_optimization_problem.py
--rw-r--r--   0        0        0     4766 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/builder/constraint.py
--rw-r--r--   0        0        0     1823 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/builder/objective.py
--rw-r--r--   0        0        0    15936 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/builder/optimization_problem.py
--rw-r--r--   0        0        0     3292 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/builder/variable.py
--rw-r--r--   0        0        0      599 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/__init__.py
--rw-r--r--   0        0        0     2002 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/decomposition_example.py
--rw-r--r--   0        0        0     1323 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/examples/diet_example.py
--rw-r--r--   0        0        0     1542 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/ellipsoid_example.py
--rw-r--r--   0        0        0     1213 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/generic_function_example.py
--rw-r--r--   0        0        0      660 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/examples/kleeminty_example.py
--rw-r--r--   0        0        0      909 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/examples/lp_sampling.py
--rw-r--r--   0        0        0     1236 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/mgs_rastringin.py
--rw-r--r--   0        0        0     2003 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/multiobjective_example.py
--rw-r--r--   0        0        0     4106 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/examples/neldermead_article_example.py
--rw-r--r--   0        0        0    10402 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/examples/neldermead_example.py
--rw-r--r--   0        0        0     3144 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs0.py
--rw-r--r--   0        0        0     3295 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs1.py
--rw-r--r--   0        0        0     1655 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs2.py
--rw-r--r--   0        0        0     1956 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs3.py
--rw-r--r--   0        0        0     1622 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/plot_example.py
--rw-r--r--   0        0        0     1530 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/examples/quadratic_example.py
--rw-r--r--   0        0        0      318 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/__init__.py
--rw-r--r--   0        0        0    10400 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/base_function.py
--rw-r--r--   0        0        0     7807 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/functions_composite.py
--rw-r--r--   0        0        0     2486 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/generic_function.py
--rw-r--r--   0        0        0     5421 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/lagrange_function.py
--rw-r--r--   0        0        0     3173 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/linear_function.py
--rw-r--r--   0        0        0     8303 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/polynomial_function.py
--rw-r--r--   0        0        0     2821 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/function/quadratic_function.py
--rw-r--r--   0        0        0      297 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/problems/__init__.py
--rw-r--r--   0        0        0     2964 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/problems/diet.py
--rw-r--r--   0        0        0     2694 2022-11-08 13:53:18.706299 science_optimization-9.0.1/science_optimization/problems/generic.py
--rw-r--r--   0        0        0     2333 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/problems/klee_minty.py
--rw-r--r--   0        0        0     4853 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/problems/mip.py
--rw-r--r--   0        0        0     2416 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/problems/quadratic.py
--rw-r--r--   0        0        0     5971 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/problems/rosen_suzuki.py
--rw-r--r--   0        0        0     3145 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/problems/separable_resource_allocation.py
--rw-r--r--   0        0        0       67 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/profiling/__init__.py
--rw-r--r--   0        0        0     2164 2022-11-08 13:53:18.706299 science_optimization-9.0.1/science_optimization/profiling/profiling.py
--rw-r--r--   0        0        0      150 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/__init__.py
--rw-r--r--   0        0        0     2824 2022-11-08 13:42:14.460435 science_optimization-9.0.1/science_optimization/solvers/optimization_results.py
--rw-r--r--   0        0        0     2616 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/optimizer.py
--rw-r--r--   0        0        0      310 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/__init__.py
--rw-r--r--   0        0        0     5804 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/base_pareto_samplers.py
--rw-r--r--   0        0        0     8087 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/epsilon_sampler.py
--rw-r--r--   0        0        0     3270 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/lambda_sampler.py
--rw-r--r--   0        0        0     3845 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/mu_sampler.py
--rw-r--r--   0        0        0     3786 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/nondominated_sampler.py
--rw-r--r--   0        0        0     2202 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/random_sampler.py
--rw-r--r--   0        0        0      403 2023-03-23 19:11:41.497780 science_optimization-9.0.1/science_optimization/test/__init__.py
--rw-r--r--   0        0        0     4286 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/test_algorithm_utils.py
--rw-r--r--   0        0        0     3386 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/test_base_linear.py
--rw-r--r--   0        0        0     8060 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/test_builder_package.py
--rw-r--r--   0        0        0    39169 2023-03-23 19:11:41.501780 science_optimization-9.0.1/science_optimization/test/test_constraint_algorithms.py
--rw-r--r--   0        0        0    35781 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/test_functions.py
--rw-r--r--   0        0        0     4511 2022-11-08 13:53:18.706299 science_optimization-9.0.1/science_optimization/test/test_glop.py
--rw-r--r--   0        0        0     8156 2023-03-23 19:11:41.501780 science_optimization-9.0.1/science_optimization/test/test_pareto_sampler.py
--rw-r--r--   0        0        0     6502 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/test_problems.py
--rw-r--r--   0        0        0     4403 2023-03-23 19:11:41.501780 science_optimization-9.0.1/science_optimization/test/test_search_direction.py
--rw-r--r--   0        0        0     2912 2023-03-23 19:11:41.501780 science_optimization-9.0.1/science_optimization/test/test_unidimensional.py
--rw-r--r--   0        0        0    13229 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/valueslinear.pickle
--rw-r--r--   0        0        0    13262 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/valuesquad.pickle
--rw-r--r--   0        0        0    13262 2022-11-08 13:42:14.464435 science_optimization-9.0.1/science_optimization/test/valuessparse.pickle
--rw-r--r--   0        0        0        0 2023-03-23 19:11:45.733736 science_optimization-9.0.1/src/__init__.py
--rw-r--r--   0        0        0     9974 2022-11-08 13:42:14.464435 science_optimization-9.0.1/src/algorithms.h
--rw-r--r--   0        0        0    26683 2022-11-08 13:42:14.464435 science_optimization-9.0.1/src/matrix.h
--rw-r--r--   0        0        0     4064 2022-11-08 13:42:14.464435 science_optimization-9.0.1/src/nlpalg.cpp
--rw-r--r--   0        0        0   163623 2022-11-08 13:42:14.464435 science_optimization-9.0.1/src/nlpalg.pdf
--rw-r--r--   0        0        0     7608 2022-11-08 13:42:14.464435 science_optimization-9.0.1/src/pybind.vcxproj
--rw-r--r--   0        0        0    12983 1970-01-01 00:00:00.000000 science_optimization-9.0.1/PKG-INFO
+-rw-r--r--   0        0        0      250 2022-11-08 13:42:14.460435 science_optimization-9.0.2/LICENSE
+-rw-r--r--   0        0        0    11780 2022-11-08 13:53:18.706299 science_optimization-9.0.2/README.md
+-rw-r--r--   0        0        0     3137 2023-03-23 19:11:45.733736 science_optimization-9.0.2/build.py
+-rw-r--r--   0        0        0     1058 2023-04-11 14:51:56.727817 science_optimization-9.0.2/pyproject.toml
+-rw-r--r--   0        0        0      193 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/__init__.py
+-rw-r--r--   0        0        0      272 2023-04-11 14:49:06.902241 science_optimization-9.0.2/science_optimization/algorithms/__init__.py
+-rw-r--r--   0        0        0      901 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/algorithms/base_algorithms.py
+-rw-r--r--   0        0        0       85 2023-04-11 14:49:06.902241 science_optimization-9.0.2/science_optimization/algorithms/cutting_plane/__init__.py
+-rw-r--r--   0        0        0     6028 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/algorithms/cutting_plane/ellipsoid_method.py
+-rw-r--r--   0        0        0       89 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/algorithms/decomposition/__init__.py
+-rw-r--r--   0        0        0     7106 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/algorithms/decomposition/dual_decomposition.py
+-rw-r--r--   0        0        0       77 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/algorithms/derivative_free/__init__.py
+-rw-r--r--   0        0        0    17247 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/algorithms/derivative_free/nelder_mead.py
+-rw-r--r--   0        0        0       88 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/algorithms/lagrange/__init__.py
+-rw-r--r--   0        0        0     5177 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/algorithms/lagrange/augmented_lagrangian.py
+-rw-r--r--   0        0        0      233 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/algorithms/linear_programming/__init__.py
+-rw-r--r--   0        0        0     4543 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/algorithms/linear_programming/glop.py
+-rw-r--r--   0        0        0     3347 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/algorithms/linear_programming/scipy_base_linear.py
+-rw-r--r--   0        0        0      429 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/algorithms/linear_programming/scipy_interior_point_method.py
+-rw-r--r--   0        0        0      395 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/algorithms/linear_programming/scipy_simplex_method.py
+-rw-r--r--   0        0        0      231 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/algorithms/search_direction/__init__.py
+-rw-r--r--   0        0        0     9608 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/algorithms/search_direction/base_search_direction.py
+-rw-r--r--   0        0        0      731 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/algorithms/search_direction/gradient_algorithm.py
+-rw-r--r--   0        0        0      589 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/algorithms/search_direction/newton_algorithm.py
+-rw-r--r--   0        0        0     3121 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/algorithms/search_direction/quasi_newton.py
+-rw-r--r--   0        0        0      197 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/algorithms/unidimensional/__init__.py
+-rw-r--r--   0        0        0     1824 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/algorithms/unidimensional/base_unidimensional.py
+-rw-r--r--   0        0        0     1305 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/algorithms/unidimensional/golden_section.py
+-rw-r--r--   0        0        0     5579 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/algorithms/unidimensional/multimodal_golden_section.py
+-rw-r--r--   0        0        0       63 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/algorithms/utils/__init__.py
+-rw-r--r--   0        0        0     4684 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/algorithms/utils/algorithms_utils.py
+-rw-r--r--   0        0        0      255 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/builder/__init__.py
+-rw-r--r--   0        0        0      504 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/builder/__init__.pyc
+-rw-r--r--   0        0        0      446 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/builder/builder_optimization_problem.py
+-rw-r--r--   0        0        0     4766 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/builder/constraint.py
+-rw-r--r--   0        0        0     1823 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/builder/objective.py
+-rw-r--r--   0        0        0    15936 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/builder/optimization_problem.py
+-rw-r--r--   0        0        0     3292 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/builder/variable.py
+-rw-r--r--   0        0        0      599 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/examples/__init__.py
+-rw-r--r--   0        0        0     2002 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/examples/decomposition_example.py
+-rw-r--r--   0        0        0     1323 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/examples/diet_example.py
+-rw-r--r--   0        0        0     1542 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/examples/ellipsoid_example.py
+-rw-r--r--   0        0        0     1213 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/examples/generic_function_example.py
+-rw-r--r--   0        0        0      660 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/examples/kleeminty_example.py
+-rw-r--r--   0        0        0      909 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/examples/lp_sampling.py
+-rw-r--r--   0        0        0     1236 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/examples/mgs_rastringin.py
+-rw-r--r--   0        0        0     2003 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/examples/multiobjective_example.py
+-rw-r--r--   0        0        0     4106 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/examples/neldermead_article_example.py
+-rw-r--r--   0        0        0    10402 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/examples/neldermead_example.py
+-rw-r--r--   0        0        0     3144 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/examples/pareto_sampling_cs0.py
+-rw-r--r--   0        0        0     3295 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/examples/pareto_sampling_cs1.py
+-rw-r--r--   0        0        0     1655 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/examples/pareto_sampling_cs2.py
+-rw-r--r--   0        0        0     1956 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/examples/pareto_sampling_cs3.py
+-rw-r--r--   0        0        0     1622 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/examples/plot_example.py
+-rw-r--r--   0        0        0     1530 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/examples/quadratic_example.py
+-rw-r--r--   0        0        0      318 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/function/__init__.py
+-rw-r--r--   0        0        0    10400 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/function/base_function.py
+-rw-r--r--   0        0        0     7807 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/function/functions_composite.py
+-rw-r--r--   0        0        0     2486 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/function/generic_function.py
+-rw-r--r--   0        0        0     5421 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/function/lagrange_function.py
+-rw-r--r--   0        0        0     3173 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/function/linear_function.py
+-rw-r--r--   0        0        0     8303 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/function/polynomial_function.py
+-rw-r--r--   0        0        0     2821 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/function/quadratic_function.py
+-rw-r--r--   0        0        0      297 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/problems/__init__.py
+-rw-r--r--   0        0        0     2964 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/problems/diet.py
+-rw-r--r--   0        0        0     2694 2022-11-08 13:53:18.706299 science_optimization-9.0.2/science_optimization/problems/generic.py
+-rw-r--r--   0        0        0     2333 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/problems/klee_minty.py
+-rw-r--r--   0        0        0     4853 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/problems/mip.py
+-rw-r--r--   0        0        0     2416 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/problems/quadratic.py
+-rw-r--r--   0        0        0     5971 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/problems/rosen_suzuki.py
+-rw-r--r--   0        0        0     3145 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/problems/separable_resource_allocation.py
+-rw-r--r--   0        0        0       67 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/profiling/__init__.py
+-rw-r--r--   0        0        0     2164 2022-11-08 13:53:18.706299 science_optimization-9.0.2/science_optimization/profiling/profiling.py
+-rw-r--r--   0        0        0      150 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/solvers/__init__.py
+-rw-r--r--   0        0        0     2824 2022-11-08 13:42:14.460435 science_optimization-9.0.2/science_optimization/solvers/optimization_results.py
+-rw-r--r--   0        0        0     2616 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/solvers/optimizer.py
+-rw-r--r--   0        0        0      310 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/solvers/pareto_samplers/__init__.py
+-rw-r--r--   0        0        0     5804 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/solvers/pareto_samplers/base_pareto_samplers.py
+-rw-r--r--   0        0        0     8087 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/solvers/pareto_samplers/epsilon_sampler.py
+-rw-r--r--   0        0        0     3270 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/solvers/pareto_samplers/lambda_sampler.py
+-rw-r--r--   0        0        0     3845 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/solvers/pareto_samplers/mu_sampler.py
+-rw-r--r--   0        0        0     3786 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/solvers/pareto_samplers/nondominated_sampler.py
+-rw-r--r--   0        0        0     2202 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/solvers/pareto_samplers/random_sampler.py
+-rw-r--r--   0        0        0      403 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/test/__init__.py
+-rw-r--r--   0        0        0     4286 2022-11-08 13:42:14.464435 science_optimization-9.0.2/science_optimization/test/test_algorithm_utils.py
+-rw-r--r--   0        0        0     3386 2022-11-08 13:42:14.464435 science_optimization-9.0.2/science_optimization/test/test_base_linear.py
+-rw-r--r--   0        0        0     8060 2022-11-08 13:42:14.464435 science_optimization-9.0.2/science_optimization/test/test_builder_package.py
+-rw-r--r--   0        0        0    39169 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/test/test_constraint_algorithms.py
+-rw-r--r--   0        0        0    35781 2022-11-08 13:42:14.464435 science_optimization-9.0.2/science_optimization/test/test_functions.py
+-rw-r--r--   0        0        0     4511 2022-11-08 13:53:18.706299 science_optimization-9.0.2/science_optimization/test/test_glop.py
+-rw-r--r--   0        0        0     8156 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/test/test_pareto_sampler.py
+-rw-r--r--   0        0        0     6502 2022-11-08 13:42:14.464435 science_optimization-9.0.2/science_optimization/test/test_problems.py
+-rw-r--r--   0        0        0     4403 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/test/test_search_direction.py
+-rw-r--r--   0        0        0     2912 2023-04-11 14:49:06.906241 science_optimization-9.0.2/science_optimization/test/test_unidimensional.py
+-rw-r--r--   0        0        0    13229 2022-11-08 13:42:14.464435 science_optimization-9.0.2/science_optimization/test/valueslinear.pickle
+-rw-r--r--   0        0        0    13262 2022-11-08 13:42:14.464435 science_optimization-9.0.2/science_optimization/test/valuesquad.pickle
+-rw-r--r--   0        0        0    13262 2022-11-08 13:42:14.464435 science_optimization-9.0.2/science_optimization/test/valuessparse.pickle
+-rw-r--r--   0        0        0        0 2023-03-23 19:11:45.733736 science_optimization-9.0.2/src/__init__.py
+-rw-r--r--   0        0        0     9974 2022-11-08 13:42:14.464435 science_optimization-9.0.2/src/algorithms.h
+-rw-r--r--   0        0        0    26683 2022-11-08 13:42:14.464435 science_optimization-9.0.2/src/matrix.h
+-rw-r--r--   0        0        0     4064 2022-11-08 13:42:14.464435 science_optimization-9.0.2/src/nlpalg.cpp
+-rw-r--r--   0        0        0   163623 2022-11-08 13:42:14.464435 science_optimization-9.0.2/src/nlpalg.pdf
+-rw-r--r--   0        0        0     7608 2022-11-08 13:42:14.464435 science_optimization-9.0.2/src/pybind.vcxproj
+-rw-r--r--   0        0        0    12983 1970-01-01 00:00:00.000000 science_optimization-9.0.2/PKG-INFO
```

### Comparing `science_optimization-9.0.1/README.md` & `science_optimization-9.0.2/README.md`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/build.py` & `science_optimization-9.0.2/build.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/pyproject.toml` & `science_optimization-9.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "science-optimization"
-version = "9.0.1"
+version = "9.0.2"
 description = "A framework for optimization."
 authors = ["Matheus Mendonça <matheus.mendonca@enacom.com.br>"]
 readme = "README.md"
 packages = [
     {include = "science_optimization"},
     {include = "src"}    
 ]
```

### Comparing `science_optimization-9.0.1/science_optimization/algorithms/base_algorithms.py` & `science_optimization-9.0.2/science_optimization/algorithms/base_algorithms.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/algorithms/cutting_plane/ellipsoid_method.py` & `science_optimization-9.0.2/science_optimization/algorithms/cutting_plane/ellipsoid_method.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/algorithms/decomposition/dual_decomposition.py` & `science_optimization-9.0.2/science_optimization/algorithms/decomposition/dual_decomposition.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/algorithms/derivative_free/nelder_mead.py` & `science_optimization-9.0.2/science_optimization/algorithms/derivative_free/nelder_mead.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/algorithms/lagrange/augmented_lagrangian.py` & `science_optimization-9.0.2/science_optimization/algorithms/lagrange/augmented_lagrangian.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/algorithms/linear_programming/glop.py` & `science_optimization-9.0.2/science_optimization/algorithms/linear_programming/glop.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/algorithms/linear_programming/scipy_base_linear.py` & `science_optimization-9.0.2/science_optimization/algorithms/linear_programming/scipy_base_linear.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/algorithms/search_direction/base_search_direction.py` & `science_optimization-9.0.2/science_optimization/algorithms/search_direction/base_search_direction.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/algorithms/search_direction/gradient_algorithm.py` & `science_optimization-9.0.2/science_optimization/algorithms/search_direction/gradient_algorithm.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/algorithms/search_direction/newton_algorithm.py` & `science_optimization-9.0.2/science_optimization/algorithms/search_direction/newton_algorithm.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/algorithms/search_direction/quasi_newton.py` & `science_optimization-9.0.2/science_optimization/algorithms/search_direction/quasi_newton.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/algorithms/unidimensional/base_unidimensional.py` & `science_optimization-9.0.2/science_optimization/algorithms/unidimensional/base_unidimensional.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/algorithms/unidimensional/golden_section.py` & `science_optimization-9.0.2/science_optimization/algorithms/unidimensional/golden_section.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/algorithms/unidimensional/multimodal_golden_section.py` & `science_optimization-9.0.2/science_optimization/algorithms/unidimensional/multimodal_golden_section.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/algorithms/utils/algorithms_utils.py` & `science_optimization-9.0.2/science_optimization/algorithms/utils/algorithms_utils.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/builder/constraint.py` & `science_optimization-9.0.2/science_optimization/builder/constraint.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/builder/objective.py` & `science_optimization-9.0.2/science_optimization/builder/objective.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/builder/optimization_problem.py` & `science_optimization-9.0.2/science_optimization/builder/optimization_problem.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/builder/variable.py` & `science_optimization-9.0.2/science_optimization/builder/variable.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/__init__.py` & `science_optimization-9.0.2/science_optimization/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/decomposition_example.py` & `science_optimization-9.0.2/science_optimization/examples/decomposition_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/diet_example.py` & `science_optimization-9.0.2/science_optimization/examples/diet_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/ellipsoid_example.py` & `science_optimization-9.0.2/science_optimization/examples/ellipsoid_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/generic_function_example.py` & `science_optimization-9.0.2/science_optimization/examples/generic_function_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/kleeminty_example.py` & `science_optimization-9.0.2/science_optimization/examples/kleeminty_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/lp_sampling.py` & `science_optimization-9.0.2/science_optimization/examples/lp_sampling.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/mgs_rastringin.py` & `science_optimization-9.0.2/science_optimization/examples/mgs_rastringin.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/multiobjective_example.py` & `science_optimization-9.0.2/science_optimization/examples/multiobjective_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/neldermead_article_example.py` & `science_optimization-9.0.2/science_optimization/examples/neldermead_article_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/neldermead_example.py` & `science_optimization-9.0.2/science_optimization/examples/neldermead_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs0.py` & `science_optimization-9.0.2/science_optimization/examples/pareto_sampling_cs0.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs1.py` & `science_optimization-9.0.2/science_optimization/examples/pareto_sampling_cs1.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs2.py` & `science_optimization-9.0.2/science_optimization/examples/pareto_sampling_cs2.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/pareto_sampling_cs3.py` & `science_optimization-9.0.2/science_optimization/examples/pareto_sampling_cs3.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/plot_example.py` & `science_optimization-9.0.2/science_optimization/examples/plot_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/examples/quadratic_example.py` & `science_optimization-9.0.2/science_optimization/examples/quadratic_example.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/function/base_function.py` & `science_optimization-9.0.2/science_optimization/function/base_function.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/function/functions_composite.py` & `science_optimization-9.0.2/science_optimization/function/functions_composite.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/function/generic_function.py` & `science_optimization-9.0.2/science_optimization/function/generic_function.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/function/lagrange_function.py` & `science_optimization-9.0.2/science_optimization/function/lagrange_function.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/function/linear_function.py` & `science_optimization-9.0.2/science_optimization/function/linear_function.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/function/polynomial_function.py` & `science_optimization-9.0.2/science_optimization/function/polynomial_function.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/function/quadratic_function.py` & `science_optimization-9.0.2/science_optimization/function/quadratic_function.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/problems/diet.py` & `science_optimization-9.0.2/science_optimization/problems/diet.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/problems/generic.py` & `science_optimization-9.0.2/science_optimization/problems/generic.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/problems/klee_minty.py` & `science_optimization-9.0.2/science_optimization/problems/klee_minty.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/problems/mip.py` & `science_optimization-9.0.2/science_optimization/problems/mip.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/problems/quadratic.py` & `science_optimization-9.0.2/science_optimization/problems/quadratic.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/problems/rosen_suzuki.py` & `science_optimization-9.0.2/science_optimization/problems/rosen_suzuki.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/problems/separable_resource_allocation.py` & `science_optimization-9.0.2/science_optimization/problems/separable_resource_allocation.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/profiling/profiling.py` & `science_optimization-9.0.2/science_optimization/profiling/profiling.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/solvers/optimization_results.py` & `science_optimization-9.0.2/science_optimization/solvers/optimization_results.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/solvers/optimizer.py` & `science_optimization-9.0.2/science_optimization/solvers/optimizer.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/base_pareto_samplers.py` & `science_optimization-9.0.2/science_optimization/solvers/pareto_samplers/base_pareto_samplers.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/epsilon_sampler.py` & `science_optimization-9.0.2/science_optimization/solvers/pareto_samplers/epsilon_sampler.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/lambda_sampler.py` & `science_optimization-9.0.2/science_optimization/solvers/pareto_samplers/lambda_sampler.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/mu_sampler.py` & `science_optimization-9.0.2/science_optimization/solvers/pareto_samplers/mu_sampler.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/nondominated_sampler.py` & `science_optimization-9.0.2/science_optimization/solvers/pareto_samplers/nondominated_sampler.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/solvers/pareto_samplers/random_sampler.py` & `science_optimization-9.0.2/science_optimization/solvers/pareto_samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/test/test_algorithm_utils.py` & `science_optimization-9.0.2/science_optimization/test/test_algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/test/test_base_linear.py` & `science_optimization-9.0.2/science_optimization/test/test_base_linear.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/test/test_builder_package.py` & `science_optimization-9.0.2/science_optimization/test/test_builder_package.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/test/test_constraint_algorithms.py` & `science_optimization-9.0.2/science_optimization/test/test_constraint_algorithms.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/test/test_functions.py` & `science_optimization-9.0.2/science_optimization/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/test/test_glop.py` & `science_optimization-9.0.2/science_optimization/test/test_glop.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/test/test_pareto_sampler.py` & `science_optimization-9.0.2/science_optimization/test/test_pareto_sampler.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/test/test_problems.py` & `science_optimization-9.0.2/science_optimization/test/test_problems.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/test/test_search_direction.py` & `science_optimization-9.0.2/science_optimization/test/test_search_direction.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/test/test_unidimensional.py` & `science_optimization-9.0.2/science_optimization/test/test_unidimensional.py`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/test/valueslinear.pickle` & `science_optimization-9.0.2/science_optimization/test/valueslinear.pickle`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/test/valuesquad.pickle` & `science_optimization-9.0.2/science_optimization/test/valuesquad.pickle`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/science_optimization/test/valuessparse.pickle` & `science_optimization-9.0.2/science_optimization/test/valuessparse.pickle`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/src/algorithms.h` & `science_optimization-9.0.2/src/algorithms.h`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/src/matrix.h` & `science_optimization-9.0.2/src/matrix.h`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/src/nlpalg.cpp` & `science_optimization-9.0.2/src/nlpalg.cpp`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/src/nlpalg.pdf` & `science_optimization-9.0.2/src/nlpalg.pdf`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/src/pybind.vcxproj` & `science_optimization-9.0.2/src/pybind.vcxproj`

 * *Files identical despite different names*

### Comparing `science_optimization-9.0.1/PKG-INFO` & `science_optimization-9.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: science-optimization
-Version: 9.0.1
+Version: 9.0.2
 Summary: A framework for optimization.
 Author: Matheus Mendonça
 Author-email: matheus.mendonca@enacom.com.br
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

