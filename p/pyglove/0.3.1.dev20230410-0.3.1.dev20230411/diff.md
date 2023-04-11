# Comparing `tmp/pyglove-0.3.1.dev20230410.tar.gz` & `tmp/pyglove-0.3.1.dev20230411.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.3.1.dev20230410.tar", last modified: Mon Apr 10 08:07:13 2023, max compression
+gzip compressed data, was "pyglove-0.3.1.dev20230411.tar", last modified: Tue Apr 11 08:06:30 2023, max compression
```

## Comparing `pyglove-0.3.1.dev20230410.tar` & `pyglove-0.3.1.dev20230411.tar`

### file list

```diff
@@ -1,185 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.957354 pyglove-0.3.1.dev20230410/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-04-10 08:07:13.957354 pyglove-0.3.1.dev20230410/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-10 08:07:07.000000 pyglove-0.3.1.dev20230410/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.909351 pyglove-0.3.1.dev20230410/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.913351 pyglove-0.3.1.dev20230410/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.913351 pyglove-0.3.1.dev20230410/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.917352 pyglove-0.3.1.dev20230410/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64411 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.921352 pyglove-0.3.1.dev20230410/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.929352 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.929352 pyglove-0.3.1.dev20230410/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.937353 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69390 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20199 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19686 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    31696 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    56822 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    24944 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    27051 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    26885 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    50738 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27877 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    71612 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.941353 pyglove-0.3.1.dev20230410/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13822 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.949354 pyglove-0.3.1.dev20230410/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    44450 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    23474 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    77073 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)    93868 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.949354 pyglove-0.3.1.dev20230410/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.949354 pyglove-0.3.1.dev20230410/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.957354 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50096 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.957354 pyglove-0.3.1.dev20230410/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.957354 pyglove-0.3.1.dev20230410/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/ext/scalars/step_wise_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/pyglove/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:07:13.909351 pyglove-0.3.1.dev20230410/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-04-10 08:07:13.000000 pyglove-0.3.1.dev20230410/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-10 08:07:13.000000 pyglove-0.3.1.dev20230410/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:07:13.000000 pyglove-0.3.1.dev20230410/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 08:07:13.000000 pyglove-0.3.1.dev20230410/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:07:13.957354 pyglove-0.3.1.dev20230410/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-10 08:06:43.000000 pyglove-0.3.1.dev20230410/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.957217 pyglove-0.3.1.dev20230411/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-11 08:06:30.957217 pyglove-0.3.1.dev20230411/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-11 08:06:28.000000 pyglove-0.3.1.dev20230411/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.925216 pyglove-0.3.1.dev20230411/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.929216 pyglove-0.3.1.dev20230411/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.929216 pyglove-0.3.1.dev20230411/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.937216 pyglove-0.3.1.dev20230411/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64411 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.941216 pyglove-0.3.1.dev20230411/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.945217 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.949216 pyglove-0.3.1.dev20230411/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.949216 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69390 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21002 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31696 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56822 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25404 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27851 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26885 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50738 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27877 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71612 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.953217 pyglove-0.3.1.dev20230411/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13822 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.953217 pyglove-0.3.1.dev20230411/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45005 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23659 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77073 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93868 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.953217 pyglove-0.3.1.dev20230411/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.953217 pyglove-0.3.1.dev20230411/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.957217 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50096 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.957217 pyglove-0.3.1.dev20230411/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.957217 pyglove-0.3.1.dev20230411/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/ext/scalars/step_wise_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/pyglove/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:06:30.929216 pyglove-0.3.1.dev20230411/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-11 08:06:30.000000 pyglove-0.3.1.dev20230411/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-04-11 08:06:30.000000 pyglove-0.3.1.dev20230411/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:06:30.000000 pyglove-0.3.1.dev20230411/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 08:06:30.000000 pyglove-0.3.1.dev20230411/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 08:06:30.000000 pyglove-0.3.1.dev20230411/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:06:30.957217 pyglove-0.3.1.dev20230411/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-11 08:06:16.000000 pyglove-0.3.1.dev20230411/setup.py
```

### Comparing `pyglove-0.3.1.dev20230410/LICENSE` & `pyglove-0.3.1.dev20230411/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/PKG-INFO` & `pyglove-0.3.1.dev20230411/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230410
+Version: 0.3.1.dev20230411
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,15 +42,15 @@
 
 PyGlove is a general-purpose library for Python object manipulation.
 It introduces symbolic object-oriented programming to Python, allowing
 direct manipulation of objects that makes meta-programs much easier to write.
 It has been used to handle complex machine learning scenarios, such as AutoML,
 as well as facilitating daily programming tasks with extra flexibility.
 
-PyGlove is lightweight and has no dependencies beyond the Python interpreter.
+PyGlove is lightweight and has very few dependencies beyond the Python interpreter.
 It provides:
 
 * A mutable symbolic object model for Python;
 * A rich set of operations for Python object manipulation;
 * A solution for automatic search of better Python programs, including:
   * An easy-to-use API for dropping search into an arbitrary pre-existing Python
     program;
```

### Comparing `pyglove-0.3.1.dev20230410/README.md` & `pyglove-0.3.1.dev20230411/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 PyGlove is a general-purpose library for Python object manipulation.
 It introduces symbolic object-oriented programming to Python, allowing
 direct manipulation of objects that makes meta-programs much easier to write.
 It has been used to handle complex machine learning scenarios, such as AutoML,
 as well as facilitating daily programming tasks with extra flexibility.
 
-PyGlove is lightweight and has no dependencies beyond the Python interpreter.
+PyGlove is lightweight and has very few dependencies beyond the Python interpreter.
 It provides:
 
 * A mutable symbolic object model for Python;
 * A rich set of operations for Python object manipulation;
 * A solution for automatic search of better Python programs, including:
   * An easy-to-use API for dropping search into an arbitrary pre-existing Python
     program;
```

### Comparing `pyglove-0.3.1.dev20230410/pyglove/__init__.py` & `pyglove-0.3.1.dev20230411/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/__init__.py` & `pyglove-0.3.1.dev20230411/pyglove/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,20 +259,21 @@
 from pyglove.core import object_utils
 KeyPath = object_utils.KeyPath
 MISSING_VALUE = object_utils.MISSING_VALUE
 
 Formattable = object_utils.Formattable
 MaybePartial = object_utils.MaybePartial
 JSONConvertible = object_utils.JSONConvertible
+DocStr = object_utils.DocStr
 
 registered_types = object_utils.registered_types
 is_partial = object_utils.is_partial
 format = object_utils.format   # pylint: disable=redefined-builtin
 print = object_utils.print    # pylint: disable=redefined-builtin
-
+docstr = object_utils.docstr
 
 #
 # Symbols from `logging.py`.
 #
 
 from pyglove.core import logging
```

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/detouring/__init__.py` & `pyglove-0.3.1.dev20230411/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/detouring/class_detour.py` & `pyglove-0.3.1.dev20230411/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/__init__.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/base.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/base_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/categorical.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/categorical_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/custom.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/custom_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/deduping.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/deduping_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/dna_generator.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/numerical.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/numerical_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/random.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/random_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/space.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/space_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/sweeping.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/geno/sweeping_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/__init__.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/base.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/categorical.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/categorical_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/custom.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/custom_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/derived.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/derived_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/evolvable.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/iter.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/iter_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/numerical.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/numerical_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/object_template.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/hyper/object_template_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/logging.py` & `pyglove-0.3.1.dev20230411/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/logging_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/object_utils/__init__.py` & `pyglove-0.3.1.dev20230411/pyglove/core/object_utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # pylint: disable=line-too-long
-"""Utility library for handling hierarchical Python objects.
+"""Utility library that provides common traits for objects in Python.
 
 Overview
 --------
 
-``pg.object_utils`` facilitates the handling of hierarchical
-Python objects. It sits at the bottom of all PyGlove modules and empowers other
+``pg.object_utils`` sits at the bottom of all PyGlove modules and empowers other
 modules with the following features:
 
   +---------------------+--------------------------------------------+
   | Functionality       | API                                        |
   +=====================+============================================+
   | Formatting          | :class:`pg.Formattable`,                   |
   |                     |                                            |
@@ -58,14 +57,18 @@
   | transformation      |                                            |
   |                     | :func:`pg.object_utils.merge`,             |
   |                     |                                            |
   |                     | :func:`pg.object_utils.canonicalize`,      |
   |                     |                                            |
   |                     | :func:`pg.object_utils.flatten`            |
   +---------------------+--------------------------------------------+
+  | Code generation     | :class:`pg.object_utils.make_function`     |
+  +---------------------+--------------------------------------------+
+  | Docstr handling     | :class:`pg.docstr`,                        |
+  +---------------------+--------------------------------------------+
 """
 # pylint: enable=line-too-long
 # pylint: disable=g-bad-import-order
 
 # Common traits.
 from pyglove.core.object_utils.common_traits import Nestable
 from pyglove.core.object_utils.common_traits import JSONValueType
@@ -108,9 +111,18 @@
 from pyglove.core.object_utils.formatting import message_on_path
 from pyglove.core.object_utils.formatting import BracketType
 from pyglove.core.object_utils.formatting import bracket_chars
 
 # Handling code generation.
 from pyglove.core.object_utils.codegen import make_function
 
+# Handling docstrings.
+from pyglove.core.object_utils.docstr_utils import DocStr
+from pyglove.core.object_utils.docstr_utils import DocStrStyle
+from pyglove.core.object_utils.docstr_utils import DocStrEntry
+from pyglove.core.object_utils.docstr_utils import DocStrExample
+from pyglove.core.object_utils.docstr_utils import DocStrArgument
+from pyglove.core.object_utils.docstr_utils import DocStrReturns
+from pyglove.core.object_utils.docstr_utils import DocStrRaises
+from pyglove.core.object_utils.docstr_utils import docstr
 
 # pylint: enable=g-bad-import-order
```

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/object_utils/codegen.py` & `pyglove-0.3.1.dev20230411/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/object_utils/common_traits.py` & `pyglove-0.3.1.dev20230411/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/object_utils/formatting.py` & `pyglove-0.3.1.dev20230411/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.3.1.dev20230411/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/object_utils/missing.py` & `pyglove-0.3.1.dev20230411/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/object_utils/missing_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/object_utils/thread_local.py` & `pyglove-0.3.1.dev20230411/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/object_utils/value_location.py` & `pyglove-0.3.1.dev20230411/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/patching/__init__.py` & `pyglove-0.3.1.dev20230411/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/patching/object_factory.py` & `pyglove-0.3.1.dev20230411/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/patching/object_factory_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/patching/pattern_based.py` & `pyglove-0.3.1.dev20230411/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/patching/rule_based.py` & `pyglove-0.3.1.dev20230411/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/patching/rule_based_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/__init__.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/base.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/base_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/class_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,18 @@
   def sym_wrapped(self):
     """Returns symbolically wrapped object."""
 
 
 class _SubclassedWrapperBase(ClassWrapper):
   """Base for class wrappers using multi-inheritance."""
 
+  # If True, fill the descriptions of schema fields automatically from the
+  # class and __init__ docstrings.
+  auto_doc = False
+
   def __init__(self, *args, **kwargs):
     """Overridden __init__ to construct symbolic wrapper only."""
     # NOTE(daiyip): We avoid `__init__` to be called multiple times.
     # This behavior is intended for a use case that detours a source class to
     # a function that returns an instance of the source class' symbolic
     # wrapper. The function may want to pass modified arguments to the
     # symbolic wrapper's `__init__`, but since the symbolic wrapper is a
@@ -111,15 +115,16 @@
     inherits_sym_init = getattr(cls.__init__, 'is_sym_init', False)
     if not inherits_sym_init:
       # This means the class is either wrapped from a user class
       # or subclassing a symbolic wrapper with its own __init__.
       # In both cases, we need to generate an __init__ wrapper for
       # calling the symbolic initialization.
       setattr(cls, '__orig_init__', cls.__init__)
-      init_arg_list, arg_fields = _extract_init_args_and_fields(cls)
+      description, init_arg_list, arg_fields = _extract_init_signature(
+          cls, auto_doc=cls.auto_doc)
       @functools.wraps(cls.__init__)
       def _sym_init(self, *args, **kwargs):
         _SubclassedWrapperBase.__init__(self, *args, **kwargs)
 
         # The following code is to deal with call to `super().__init__()`.
         # In such case, we need to invoke the original __init__ instead of
         # the symbolic init, which can be told by the
@@ -130,15 +135,16 @@
       setattr(_sym_init, '__signature__', inspect.signature(cls.__init__))
       setattr(_sym_init, 'is_sym_init', True)
       setattr(cls, '__init__', _sym_init)
 
       # We do not extend existing schema which is inherited from the base
       # class.
       schema_utils.update_schema(
-          cls, arg_fields, init_arg_list=init_arg_list, extend=False)
+          cls, arg_fields, init_arg_list=init_arg_list,
+          extend=False, description=description)
     else:
       assert hasattr(cls, '__orig_init__')
 
   def _init_user_cls(self, *args, **kwargs):
     """Init user class."""
     self.__orig_init__(*args, **kwargs)
 
@@ -198,16 +204,18 @@
   def sym_wrapped(self):
     """Returns wrapped object."""
     return self
 
 
 def _subclassed_wrapper(
     user_cls,
+    *,
     use_symbolic_repr: bool,
     use_symbolic_comp: bool,
+    use_auto_doc: bool,
     reset_state_fn: Optional[Callable[[Any], None]],
     class_name: Optional[Text] = None,
     module_name: Optional[Text] = None):
   """Class wrapper implementation by regular multi-inheritance."""
   # NOTE(daiyip): The user class may have a user-defined metaclass, which
   # conflicts with the metaclass of the symbolic base. Therefore, we detect
   # such case and create a common metaclass when a conflict is detected.
@@ -224,14 +232,18 @@
     """Class wrapper bound to a user class."""
     sym_wrapped_cls = user_cls
 
     # Disable auto register so we can use function module and name
     # for registration later.
     auto_register = False
 
+    # If True, set the descriptions of schema fields automatically from
+    # class and __init__ docstrings.
+    auto_doc = use_auto_doc
+
     # NOTE(daiyip): For class wrappers, all symbolic properties are exposed from
     # `self.sym_init_args`. Therefore we do not allow symbolic members to be
     # accessed or changed via attributes using `self.<member_name>`.
     allow_symbolic_attribute = False
 
     # This class property lets `pg.Object` control whether to delegate the
     # implementation of `__setattr__` to `object.__setattr__`, when the flag is
@@ -270,19 +282,21 @@
 
 def wrap(
     cls,
     init_args: Optional[List[Union[
         Tuple[Union[Text, pg_typing.KeySpec], pg_typing.ValueSpec, Text],
         Tuple[Union[Text, pg_typing.KeySpec], pg_typing.ValueSpec, Text, Any]
     ]]] = None,
+    *,
     reset_state_fn: Optional[Callable[[Any], None]] = None,
     repr: bool = True,    # pylint: disable=redefined-builtin
     eq: bool = False,
     class_name: Optional[str] = None,
     module_name: Optional[str] = None,
+    auto_doc: bool = False,
     serialization_key: Optional[str] = None,
     additional_keys: Optional[List[str]] = None,
     override: Optional[Dict[str, Any]] = None
 ) -> Type['ClassWrapper']:
   """Makes a symbolic class wrapper from a regular Python class.
 
   ``pg.wrap`` is called by :func:`pyglove.symbolize` for symbolizing existing
@@ -343,14 +357,16 @@
         `__hash__`, use symbolic eq/hash.
       If False (default), use `user_cls`'s definition if present, or the
         definitions from the `object` class.
     class_name: An optional string used as class name for the wrapper class.
       If None, the wrapper class will use the class name of the wrapped class.
     module_name: An optional string used as module name for the wrapper class.
       If None, the wrapper class will use the module name of the wrapped class.
+    auto_doc: If True, the descriptions for init argument fields will be
+      extracted from docstring if present.
     serialization_key: An optional string to be used as the serialization key
       for the class during `sym_jsonify`. If None, `cls.type_name` will be used.
       This is introduced for scenarios when we want to relocate a class, before
       the downstream can recognize the new location, we need the class to
       serialize it using previous key.
     additional_keys: An optional list of strings as additional keys to
       deserialize an object of the registered class. This can be useful
@@ -370,24 +386,28 @@
   if not issubclass(cls, ClassWrapper):
     cls = _subclassed_wrapper(
         cls,
         use_symbolic_repr=repr,
         use_symbolic_comp=eq,
         reset_state_fn=reset_state_fn,
         class_name=class_name,
-        module_name=module_name)
+        module_name=module_name,
+        use_auto_doc=auto_doc)
 
   if issubclass(cls, ClassWrapper):
     # Update init argument specifications according to user specified specs.
     # Replace schema instead of extending it.
-    init_arg_list, arg_fields = _extract_init_args_and_fields(cls, init_args)
+    description, init_arg_list, arg_fields = _extract_init_signature(
+        cls, init_args, auto_doc=auto_doc)
     schema_utils.update_schema(
-        cls, arg_fields,
+        cls,
+        arg_fields,
         init_arg_list=init_arg_list,
         extend=False,
+        description=description,
         serialization_key=serialization_key,
         additional_keys=additional_keys)
 
   if override:
     for k, v in override.items():
       setattr(cls, k, v)
   return cls
@@ -486,24 +506,45 @@
           and c not in (ClassWrapper, _SubclassedWrapperBase)
           and (not where or where(c))
           and c.sym_wrapped_cls is not None):
         wrapper_classes.append(c)
   return detouring.detour([(c.sym_wrapped_cls, c) for c in wrapper_classes])
 
 
-def _extract_init_args_and_fields(cls, arg_specs=None):
+def _extract_init_signature(
+    cls,
+    arg_specs=None,
+    auto_doc: bool = False):
   """Extract argument fields from class __init__ method."""
   init_method = getattr(cls, '__orig_init__', cls.__init__)
+
+  description = None
+  args_docstr = dict()
+  if auto_doc:
+    # Read args docstr from both class doc string and __init__ doc string.
+    if cls.__doc__:
+      cls_docstr = object_utils.DocStr.parse(cls.__doc__)
+      description = schema_utils.schema_description_from_docstr(
+          cls_docstr, include_long_description=True)
+      args_docstr = cls_docstr.args
+    if init_method.__doc__:
+      init_docstr = object_utils.DocStr.parse(init_method.__doc__)
+      args_docstr.update(init_docstr.args)
+
   if init_method is object.__init__:
-    arg_fields = arg_specs or []
+    if arg_specs:
+      raise ValueError(
+          f'{cls.__name__}.__init__ takes no argument while non-empty `args` '
+          f'is provided: {arg_specs}')
     init_arg_list = []
+    arg_fields = []
   else:
     signature = pg_typing.get_signature(init_method)
     if not signature.args or signature.args[0].name != 'self':
       raise ValueError(
           f'{cls.__name__}.__init__ must have `self` as the first argument.')
     # Remove field for 'self'.
-    arg_fields = pg_typing.get_arg_fields(signature, arg_specs)[1:]
+    arg_fields = pg_typing.get_arg_fields(signature, arg_specs, args_docstr)[1:]
     init_arg_list = [arg.name for arg in signature.args[1:]]
     if signature.has_varargs:
       init_arg_list.append(f'*{signature.varargs.name}')
-  return (init_arg_list, arg_fields)
+  return (description, init_arg_list, arg_fields)
```

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for pyglove.symbolic.class_wrapper."""
 
 import copy
+import dataclasses
 import inspect
 import unittest
 
 from pyglove.core import detouring as pg_detouring
 from pyglove.core import typing as pg_typing
 
 from pyglove.core.symbolic.base import eq as pg_eq
@@ -151,14 +152,56 @@
         ('p', pg_typing.Int()),
         ('q', pg_typing.Int()),
     ])
     a = A1(1, p=2, q=3)
     self.assertEqual(a.z, 7)   # 1 + 1 + 2 + 3
     self.assertNotIn('z', a.sym_init_args)
 
+  def test_wrap_with_auto_doc(self):
+
+    class A:
+      """A test class."""
+
+      def __init__(self, x, y):
+        """Init method.
+        
+        Args:
+          x: Argument x.
+          y: Argument y.
+        """
+        self.x = x
+        self.y = y
+
+    A1 = pg_wrap(A, auto_doc=True)  # pylint: disable=invalid-name
+    self.assertEqual(A1.schema.description, 'A test class.')
+    self.assertEqual(list(A1.schema.fields.values()), [
+        pg_typing.Field('x', pg_typing.Any(), 'Argument x.'),
+        pg_typing.Field('y', pg_typing.Any(), 'Argument y.'),
+    ])
+
+  def test_wrap_dataclass_with_auto_doc(self):
+
+    @dataclasses.dataclass
+    class A:
+      """A test class.
+      
+      Attributes:
+        x: Argument x.
+        y: Argument y.
+      """
+      x: int
+      y: str
+
+    A1 = pg_wrap(A, auto_doc=True)  # pylint: disable=invalid-name
+    self.assertEqual(A1.schema.description, 'A test class.')
+    self.assertEqual(list(A1.schema.fields.values()), [
+        pg_typing.Field('x', pg_typing.Any(annotation=int), 'Argument x.'),
+        pg_typing.Field('y', pg_typing.Any(annotation=str), 'Argument y.'),
+    ])
+
   def test_automatic_reset_state(self):
 
     class A:
 
       def __init__(self, v):
         if hasattr(self, 'x'):
           self.y = v
@@ -405,14 +448,17 @@
       pass
 
     A1 = pg_wrap(A)  # pylint: disable=invalid-name
     self.assertTrue(pg_eq(A1(), A1()))
     self.assertEqual(repr(A1), f'Symbolic[{A1.sym_wrapped_cls!r}]')
     a = A1()
     self.assertIs(a.sym_wrapped, a)
+    with self.assertRaisesRegex(
+        ValueError, '.* takes no argument while non-empty `args` is provided'):
+      _ = pg_wrap(A, [('x', pg_typing.Int())])
 
     class B:
 
       def __init__(self, x):
         self.x = x
         self.y = x + 1
```

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/dict.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/dict.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/dict_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/dict_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/diff.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/diff_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/flags.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/flags_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/functor.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/functor.py`

 * *Files 2% similar despite different names*

```diff
@@ -442,14 +442,16 @@
     func: Callable,  # pylint: disable=g-bare-generic
     args: Optional[List[Union[
         Tuple[Tuple[str, pg_typing.KeySpec], pg_typing.ValueSpec, str],
         Tuple[Tuple[str, pg_typing.KeySpec], pg_typing.ValueSpec, str, Any]]]
     ] = None,   # pylint: disable=bad-continuation
     returns: Optional[pg_typing.ValueSpec] = None,
     base_class: Optional[Type['Functor']] = None,
+    *,
+    auto_doc: bool = False,
     serialization_key: Optional[str] = None,
     additional_keys: Optional[List[str]] = None,
     add_to_registry: bool = False,
 ) -> Type[Functor]:
   """Returns a functor class from a function.
 
   Args:
@@ -489,14 +491,17 @@
             ]
             # Prebind a=1, b=2, with default value c=1.
             assert foo(1, 2)() == 4
 
     returns: Optional schema specification for the return value.
     base_class: Optional base class (derived from `symbolic.Functor`).
       If None, returned type will inherit from `Functor` directly.
+    auto_doc: If True, the descriptions of argument fields will be inherited
+      from funciton docstr if they are not explicitly specified through
+      ``args``.
     serialization_key: An optional string to be used as the serialization key
       for the class during `sym_jsonify`. If None, `cls.type_name` will be used.
       This is introduced for scenarios when we want to relocate a class, before
       the downstream can recognize the new location, we need the class to
       serialize it using previous key.
     additional_keys: An optional list of strings as additional keys to
       deserialize an object of the registered class. This can be useful
@@ -511,16 +516,24 @@
     KeyError: names of symbolic arguments are not compatible with
       function signature.
     TypeError: types of symbolic arguments are not compatible with
       function signature.
     ValueError: default values of symbolic arguments are not compatible
       with  function signature.
   """
+  args_docstr = None
+  description = None
+  if auto_doc:
+    docstr = object_utils.docstr(func)
+    if docstr:
+      args_docstr = docstr.args
+      description = schema_utils.schema_description_from_docstr(docstr)
+
   signature = pg_typing.get_signature(func)
-  arg_fields = pg_typing.get_arg_fields(signature, args)
+  arg_fields = pg_typing.get_arg_fields(signature, args, args_docstr)
   if returns is not None and pg_typing.MISSING_VALUE != returns.default:
     raise ValueError('return value spec should not have default value.')
 
   base_class = base_class or Functor
 
   class _Functor(base_class):
     """Functor wrapper for input function."""
@@ -545,14 +558,15 @@
   init_arg_list = [arg.name for arg in signature.args]
   if signature.varargs:
     init_arg_list.append(f'*{signature.varargs.name}')
   schema_utils.update_schema(
       cls,
       arg_fields,
       init_arg_list=init_arg_list,
+      description=description,
       serialization_key=serialization_key,
       additional_keys=additional_keys,
       add_to_registry=add_to_registry)
 
   # Update signature with symbolic value specs.
   def _value_spec_by_name(name: str):
     field = cls.schema.get_field(name)  # pytype: disable=attribute-error  # re-none
```

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/functor_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/functor_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,21 +90,20 @@
   def test_automatic_typing(self):
     @pg_functor()
     def f(a, b, *args, c=0, **kwargs):
       return a + b + c + sum(args) + sum(kwargs.values())
 
     self.assertEqual(
         list(f.schema.values()), [
-            pg_typing.Field('a', pg_typing.Any(), 'Argument \'a\'.'),
-            pg_typing.Field('b', pg_typing.Any(), 'Argument \'b\'.'),
-            pg_typing.Field('args', pg_typing.List(pg_typing.Any(), default=[]),
-                            'Wildcard positional arguments.'),
-            pg_typing.Field('c', pg_typing.Any(default=0), 'Argument \'c\'.'),
-            pg_typing.Field(pg_typing.StrKey(), pg_typing.Any(),
-                            'Wildcard keyword arguments.'),
+            pg_typing.Field('a', pg_typing.Any()),
+            pg_typing.Field('b', pg_typing.Any()),
+            pg_typing.Field('args',
+                            pg_typing.List(pg_typing.Any(), default=[])),
+            pg_typing.Field('c', pg_typing.Any(default=0)),
+            pg_typing.Field(pg_typing.StrKey(), pg_typing.Any()),
         ])
     self.assertEqual(f.signature.args, [
         pg_typing.Argument('a', pg_typing.Any()),
         pg_typing.Argument('b', pg_typing.Any())
     ])
     self.assertEqual(
         f.signature.varargs,
@@ -156,14 +155,45 @@
 
     # Override default value.
     self.assertEqual(f.partial(a=2)(), 4)
     self.assertEqual(f.partial(a=2, override_args=True)(a=3), 5)
     self.assertEqual(f.partial(a=1, b=1, override_args=True)(a=2, b=2), 4)
     self.assertEqual(f.partial(2, 4, override_args=True)(1), 5)
 
+  def test_auto_doc(self):
+    @pg_functor([
+        ('a', pg_typing.Int()),
+        ('b', pg_typing.Int()),
+    ], returns=pg_typing.Int(), auto_doc=True)
+    def f(a=1, b=2):
+      """Compute the sum.
+      
+      Args:
+        a: an integer.
+        b: another integer.
+      
+      Returns:
+        Sum of two integers.
+      """
+      return a + b
+
+    self.assertEqual(f.schema.description, 'Compute the sum.')
+    self.assertEqual(
+        list(f.schema.values()), [
+            pg_typing.Field('a', pg_typing.Int(default=1), 'an integer.'),
+            pg_typing.Field('b', pg_typing.Int(default=2), 'another integer.'),
+        ])
+    self.assertEqual(f.signature.return_value, pg_typing.Int())
+    self.assertFalse(f.signature.has_varargs)
+    self.assertFalse(f.signature.has_varkw)
+    self.assertEqual(f.partial()(), 3)
+    self.assertEqual(f.partial(a=2)(b=2), 4)
+    self.assertEqual(f.partial(a=3, b=2)(), 5)
+    self.assertEqual(f.partial(1, 2)(), 3)
+
   def test_partial_typing(self):
     @pg_functor([
         ('c', pg_typing.Int()),
         ('a', pg_typing.Int()),
     ])
     def f(a, b=1, c=1):
       return a + b + c
@@ -174,15 +204,15 @@
         pg_typing.Argument('c', pg_typing.Int(default=1)),
     ])
     self.assertFalse(f.signature.has_varargs)
     self.assertFalse(f.signature.has_varkw)
     self.assertEqual(
         list(f.schema.values()), [
             pg_typing.Field('a', pg_typing.Int()),
-            pg_typing.Field('b', pg_typing.Any(default=1), 'Argument \'b\'.'),
+            pg_typing.Field('b', pg_typing.Any(default=1)),
             pg_typing.Field('c', pg_typing.Int(default=1)),
         ])
     self.assertEqual(f.partial()(a=2), 4)
     # Override 'a' with 2, provide 'b' with 2, use 'c' from default value 1.
     self.assertEqual(f.partial()(2, 2), 5)
 
     # 'a' is not provided.
```

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/list.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/list.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/list_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/list_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/object.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/object.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/object_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/object_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/origin.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/origin_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/schema_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,17 @@
     cls,
     fields: List[Union[
         pg_typing.Field,
         Tuple[Union[str, pg_typing.KeySpec], pg_typing.ValueSpec, str],
         Tuple[Union[str, pg_typing.KeySpec], pg_typing.ValueSpec, str, Any]]],
     metadata: Optional[Dict[str, Any]] = None,
     init_arg_list: Optional[Sequence[str]] = None,
+    *,
     extend: bool = True,
+    description: Optional[str] = None,
     serialization_key: Optional[str] = None,
     additional_keys: Optional[List[str]] = None,
     add_to_registry: bool = True) -> None:
   """Updates the schema for a ``pg.Object`` subclass.
 
   This function allows the user to update the symbolic fields associated
   with a symbolic class. It was intended to support meta-programming
@@ -75,14 +77,15 @@
       list for `__init__`. This is helpful when symbolic attributes are
       inherited from base classes or the user want to change its order.
       If not provided, the `init_arg_list` will be automatically generated
       from symbolic attributes defined from ``pg.members`` in their declaration
       order, from the base classes to the subclass.
     extend: If True, extend existing schema using `fields`. Otherwise replace
       existing schema with a new schema created from `fields`.
+    description: An optional description to set.
     serialization_key: An optional string to be used as the serialization key
       for the class during `sym_jsonify`. If None, `cls.type_name` will be used.
       This is introduced for scenarios when we want to relocate a class, before
       the downstream can recognize the new location, we need the class to
       serialize it using previous key.
     additional_keys: An optional list of strings as additional keys to
       deserialize an object of the registered class. This can be useful
@@ -105,14 +108,17 @@
   setattr(cls, '__serialization_key__', serialization_key or cls.type_name)
 
   if init_arg_list is None:
     init_arg_list = metadata.pop('init_arg_list', auto_init_arg_list(cls))
   validate_init_arg_list(init_arg_list, cls_schema)
   cls_schema.metadata['init_arg_list'] = init_arg_list
 
+  if description is not None:
+    cls_schema.set_description(description)
+
   if add_to_registry:
     register_serialization_keys(
         cls, serialization_key, additional_keys)
 
   cls._update_init_signature_based_on_schema()  # pylint: disable=protected-access
   cls._generate_sym_attributes_if_enabled()  # pylint: disable=protected-access
 
@@ -207,7 +213,22 @@
           _formalize_field(
               object_utils.KeyPath(i, path),
               pg_typing.Field(field.key, c, 'Union sub-type.'))
     return True
 
   object_utils.traverse(schema.fields, _formalize_field)
   return schema
+
+
+def schema_description_from_docstr(
+    docstr: Optional[object_utils.DocStr],
+    include_long_description: bool = False) -> Optional[str]:
+  """Gets schema description from DocStr."""
+  if docstr is None:
+    return None
+  description = docstr.short_description
+  if include_long_description:
+    if docstr.blank_after_short_description:
+      description += '\n'
+    if docstr.long_description:
+      description += '\n' + docstr.long_description
+  return description.rstrip('\n')
```

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/symbolize.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/tuning/__init__.py` & `pyglove-0.3.1.dev20230411/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/tuning/backend.py` & `pyglove-0.3.1.dev20230411/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/tuning/backend_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/tuning/early_stopping.py` & `pyglove-0.3.1.dev20230411/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/tuning/local_backend.py` & `pyglove-0.3.1.dev20230411/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/tuning/protocols.py` & `pyglove-0.3.1.dev20230411/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/tuning/protocols_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/tuning/sample.py` & `pyglove-0.3.1.dev20230411/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/tuning/sample_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/__init__.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/callable_ext.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/callable_signature.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/callable_signature.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/callable_signature_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/class_schema.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/class_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -499,14 +499,18 @@
     self._metadata = metadata or {}
 
   @property
   def description(self) -> str:
     """Description of this field."""
     return self._description
 
+  def set_description(self, description: str) -> None:
+    """Sets the description for this field."""
+    self._description = description
+
   @property
   def key(self) -> KeySpec:
     """Key specification of this field."""
     return self._key
 
   @property
   def value(self) -> ValueSpec:
@@ -713,25 +717,28 @@
   """
 
   def __init__(
       self,
       fields: List[Field],
       name: Optional[str] = None,
       base_schema_list: Optional[List['Schema']] = None,
+      description: Optional[str] = None,
+      *,
       allow_nonconst_keys: bool = False,
       metadata: Optional[Dict[str, Any]] = None):
     """Constructor.
 
     Args:
       fields: A list of Field as the definition of the schema. The order of the
         fields will be preserved.
       name: Optional name of this schema. Useful for debugging.
       base_schema_list: List of schema used as base. When present, fields
         from these schema will be copied to this schema. Fields from the
         latter schema will override those from the former ones.
+      description: Optional str as the description for the schema.
       allow_nonconst_keys: Whether immediate fields can use non-const keys.
       metadata: Optional dict of user objects as schema-level metadata.
 
     Raises:
       TypeError: Argument `fields` is not a list.
       KeyError: If a field name contains characters ('.') which is not
         allowed, or a field name from `fields` already exists in parent
@@ -742,14 +749,15 @@
     """
     if not isinstance(fields, list):
       raise TypeError('Argument \'fields\' must be a list.')
 
     self._name = name
     self._allow_nonconst_keys = allow_nonconst_keys
     self._fields = {f.key: f for f in fields}
+    self._description = description
     self._metadata = metadata or {}
 
     self._dynamic_field = None
     for f in fields:
       if not f.key.is_const:
         self._dynamic_field = f
         break
@@ -855,14 +863,23 @@
     if self._allow_nonconst_keys:
       for key_spec, field in self._fields.items():
         if key_spec.match(key):
           return field
     return None
 
   @property
+  def description(self) -> str:
+    """Returns the description for the schema."""
+    return self._description
+
+  def set_description(self, description: str) -> None:
+    """Sets the description for the schema."""
+    self._description = description
+
+  @property
   def dynamic_field(self) -> Optional[Field]:
     """Returns the field that matches multiple keys if any."""
     return self._dynamic_field
 
   def resolve(
       self, keys: Iterable[str]
   ) -> Tuple[Dict[KeySpec, List[str]], List[str]]:
```

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/class_schema_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/class_schema_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,21 @@
     # Test Schema.name
     self.assertEqual(s.name, 'schema1')
 
     # Test Schema.set_name
     s.set_name('schema2')
     self.assertEqual(s.name, 'schema2')
 
+    # Test Schema.description.
+    self.assertIsNone(s.description)
+
+    # Test Schema.set_description.
+    s.set_description('schema1')
+    self.assertEqual(s.description, 'schema1')
+
     # Test equal.
     self.assertEqual(s, s)
     self.assertNotEqual(s, class_schema.create_schema([]))
 
     with self.assertRaisesRegex(
         TypeError, 'Argument \'fields\' must be a list.'):
       Schema({'a': vs.Int()})
```

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/class_schema_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,30 +9,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Typing helpers."""
 
-from typing import Any, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from pyglove.core import object_utils
 from pyglove.core.typing import callable_signature
 from pyglove.core.typing import class_schema
 from pyglove.core.typing import key_specs as ks
 from pyglove.core.typing import value_specs as vs
 
 
 def get_arg_fields(
     signature: callable_signature.Signature,
     args: Optional[List[Union[
         Tuple[Union[str, class_schema.KeySpec], class_schema.ValueSpec, str],
         Tuple[Union[str, class_schema.KeySpec],
               class_schema.ValueSpec, str, Any]]]
-    ] = None   # pylint: disable=bad-continuation
+    ] = None,   # pylint: disable=bad-continuation
+    args_docstr: Optional[Dict[str, object_utils.DocStrArgument]] = None
 ) -> List[class_schema.Field]:
   """Get schema fields for the arguments from a function or method signature.
 
   Args:
     signature: A `Signature` object.
     args: (Optional) explicit value specifications for the arguments, which is a
       list of tuples in:
@@ -45,14 +46,17 @@
         ``StrKey`` object, it specifies a field that matches any keys beyond
         the regular arguments for the ``**kwargs``.
       * `value-spec` - a ``ValueSpec`` object asssociate with the argument
         name.
       * `description` - an optional string as the description for the argument.
       * `metadata-objects` - an optional list of any type, which can be
         used to generate code according to the schema.
+    args_docstr: (Optional) a dict of argument names to
+      :class:`pg.object_utils.DocStrArgument` object. If present, they will
+      be used as the description for the ``Field`` objects.
 
   Returns:
     `Field` objects for the arguments from the `signature` in declaration order.
     If an argument is not present in `args`, it will be considered an `Any`.
     Otherwise it will create a `Field` from the explicit specifications. Default
     values for the arguments will be automatially propagated from the signature
     to the fields.
@@ -65,14 +69,21 @@
     ValueError: The value spec defined in `args` does not align with the default
       values from the signature.
   """
   arg_dict = dict()
   kwarg_spec = None
   varargs_spec = None
 
+  def maybe_add_description(arg_name, field):
+    if args_docstr and not field.description:
+      arg_docstr = args_docstr.get(arg_name, None)
+      if arg_docstr is not None:
+        field.set_description(arg_docstr.description)
+    return field
+
   func_arg_names = set(signature.arg_names)
   # Extra legal argument names that are out of function signature, it is not
   # empty only when function allow **kwargs.
   extra_arg_names = []
   for arg in args or []:
     if isinstance(arg[0], ks.StrKey):
       if kwarg_spec is not None:
@@ -97,68 +108,71 @@
       arg_dict[arg[0]] = arg
 
   def get_arg_field(arg_spec):
     arg_name = arg_spec.name
     decl_spec = arg_spec.value_spec
     if arg_name not in arg_dict:
       # Automatic generate symbolic declaration for missing arguments.
-      arg_field = (arg_name, decl_spec, f'Argument {arg_name!r}.')
+      arg_spec = (arg_name, decl_spec)
     else:
-      arg_field = arg_dict[arg_name]
-      if not decl_spec.is_compatible(arg_field[1]):
+      arg_spec = arg_dict[arg_name]
+      if not decl_spec.is_compatible(arg_spec[1]):
         raise TypeError(
-            f'{signature.id}: the value spec ({arg_field[1]!r}) of symbolic '
+            f'{signature.id}: the value spec ({arg_spec[1]!r}) of symbolic '
             f'argument {arg_name} is not compatible with the value spec '
             f'({decl_spec!r}) from function signature.')
-      if arg_field[1].default in [object_utils.MISSING_VALUE, None]:
-        arg_field[1].extend(decl_spec).set_default(decl_spec.default)
-      elif (decl_spec.default != arg_field[1].default
-            and (not isinstance(arg_field[1], vs.Dict)
+      if arg_spec[1].default in [object_utils.MISSING_VALUE, None]:
+        arg_spec[1].extend(decl_spec).set_default(decl_spec.default)
+      elif (decl_spec.default != arg_spec[1].default
+            and (not isinstance(arg_spec[1], vs.Dict)
                  or decl_spec.default != object_utils.MISSING_VALUE)):
         raise ValueError(
-            f'{signature.id}: the default value ({arg_field[1].default!r}) '
+            f'{signature.id}: the default value ({arg_spec[1].default!r}) '
             f'of symbolic argument {arg_name!r} does not equal to the default '
             f'value ({decl_spec.default!r}) specified at function signature '
             f'declaration.')
-    return arg_field
-
-  arg_fields = []
-
+    return maybe_add_description(arg_name, class_schema.Field(*arg_spec))
   # Add positional named arguments.
-  arg_fields.extend([get_arg_field(arg) for arg in signature.args])
+  arg_fields: List[class_schema.Field] = [
+      get_arg_field(arg) for arg in signature.args]
 
   # Add positional wildcard arguments.
   if signature.varargs:
     if varargs_spec is None:
       varargs_spec = (
           ks.ConstStrKey(signature.varargs.name),
-          vs.List(vs.Any()),
-          'Wildcard positional arguments.')
+          vs.List(vs.Any()))
     elif not isinstance(varargs_spec[1], vs.List):
       raise ValueError(
           f'{signature.id}: the value spec for positional wildcard argument '
           f'{varargs_spec[0]!r} must be a `pg.typing.List` instance. '
           f'Encountered: {varargs_spec[1]!r}.')
     varargs_spec[1].set_default([])
-    arg_fields.append(varargs_spec)
+    vararg_field = maybe_add_description(
+        f'*{signature.varargs.name}', class_schema.Field(*varargs_spec))
+    arg_fields.append(vararg_field)
 
   # Add keyword-only arguments.
   arg_fields.extend([get_arg_field(arg) for arg in signature.kwonlyargs])
 
   # Add extra arguments that are keyword wildcard.
   for arg_name in extra_arg_names:
-    arg_fields.append(arg_dict[arg_name])
+    arg_field = maybe_add_description(
+        arg_name,
+        class_schema.Field(*arg_dict[arg_name]))
+    arg_fields.append(arg_field)
 
   # Add keyword wildcard arguments.
   if signature.varkw:
     if kwarg_spec is None:
-      kwarg_spec = (ks.StrKey(), vs.Any(),
-                    'Wildcard keyword arguments.')
-    arg_fields.append(kwarg_spec)
-  return [class_schema.Field(*arg_decl) for arg_decl in arg_fields]
+      kwarg_spec = (ks.StrKey(), vs.Any())
+    varkw_field = maybe_add_description(
+        f'**{signature.varkw.name}', class_schema.Field(*kwarg_spec))
+    arg_fields.append(varkw_field)
+  return arg_fields
 
 
 def get_init_signature(
     schema: class_schema.Schema,
     module_name: str,
     name: str,
     qualname: Optional[str] = None,
```

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/class_schema_utils_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for pyglove.core.typing.class_schema_utils."""
 
 import unittest
 
+from pyglove.core import object_utils
 from pyglove.core.typing import callable_signature
 from pyglove.core.typing import class_schema
 from pyglove.core.typing import class_schema_utils
 from pyglove.core.typing import key_specs as ks
 from pyglove.core.typing import value_specs as vs
 
 
@@ -26,62 +27,86 @@
   """Tests for `get_arg_fields`."""
 
   def test_basics(self):
     signature = callable_signature.get_signature(
         lambda a, *args, b=1, **kwargs: 1)
     arg_fields = class_schema_utils.get_arg_fields(signature)
     self.assertEqual(arg_fields, [
-        class_schema.Field('a', vs.Any(), 'Argument \'a\'.'),
+        class_schema.Field('a', vs.Any()),
         class_schema.Field(
-            'args', vs.List(vs.Any(), default=[]),
-            'Wildcard positional arguments.'),
+            'args', vs.List(vs.Any(), default=[])),
         class_schema.Field(
-            'b', vs.Any().set_default(1), 'Argument \'b\'.'),
-        class_schema.Field(ks.StrKey(), vs.Any(), 'Wildcard keyword arguments.')
+            'b', vs.Any().set_default(1)),
+        class_schema.Field(ks.StrKey(), vs.Any())
     ])
 
   def test_full_typing(self):
     signature = callable_signature.get_signature(
         lambda a, *args, b='foo', **kwargs: 1)
     arg_fields = class_schema_utils.get_arg_fields(signature, [
         ('b', vs.Str()),
         ('args', vs.List(vs.Int())),
         ('a', vs.Int()),
         ('c', vs.Str()),
     ])
     self.assertEqual(arg_fields, [
         class_schema.Field('a', vs.Int()),
-        class_schema.Field(
-            'args', vs.List(vs.Int(), default=[])),
+        class_schema.Field('args', vs.List(vs.Int(), default=[])),
         class_schema.Field('b', vs.Str(default='foo')),
         class_schema.Field('c', vs.Str()),
-        class_schema.Field(ks.StrKey(), vs.Any(), 'Wildcard keyword arguments.')
+        class_schema.Field(ks.StrKey(), vs.Any())
     ])
 
   def test_partial_typing(self):
     signature = callable_signature.get_signature(lambda a, b='foo': 1)
     arg_fields = class_schema_utils.get_arg_fields(signature, [
         ('b', vs.Str()),
     ])
     self.assertEqual(arg_fields, [
-        class_schema.Field('a', vs.Any(), 'Argument \'a\'.'),
+        class_schema.Field('a', vs.Any()),
         class_schema.Field('b', vs.Str(default='foo')),
     ])
 
     # Special cases for Dict
     signature = callable_signature.get_signature(lambda a: 1)
     arg_fields = class_schema_utils.get_arg_fields(signature, [
         ('a', vs.Dict([
             ('x', vs.Int())
         ])),
     ])
     self.assertEqual(arg_fields, [
         class_schema.Field('a', vs.Dict([('x', vs.Int())]))
     ])
 
+  def test_use_docstr_as_description(self):
+    signature = callable_signature.get_signature(
+        lambda a, *args, b='foo', **kwargs: 1)
+    arg_fields = class_schema_utils.get_arg_fields(
+        signature,
+        [
+            ('a', vs.Int()),
+            ('b', vs.Str(default='foo'), 'Original description for b'),
+        ],
+        {
+            'a': object_utils.DocStrArgument(name='a', description='An int'),
+            'b': object_utils.DocStrArgument(name='b', description='A str'),
+            '*args': object_utils.DocStrArgument(name='*args',
+                                                 description='Args'),
+            '**kwargs': object_utils.DocStrArgument(name='**kwargs',
+                                                    description='Kwargs'),
+        })
+    self.assertEqual(arg_fields, [
+        class_schema.Field('a', vs.Int(), 'An int'),
+        class_schema.Field(
+            'args', vs.List(vs.Any(), default=[]), 'Args'),
+        class_schema.Field('b', vs.Str(default='foo'),
+                           'Original description for b'),
+        class_schema.Field(ks.StrKey(), vs.Any(), 'Kwargs')
+    ])
+
   def test_bad_typing(self):
     with self.assertRaisesRegex(
         KeyError, 'multiple StrKey found in symbolic arguments declaration.'):
       class_schema_utils.get_arg_fields(
           callable_signature.get_signature(lambda a: 1),
           [(ks.StrKey(), vs.Int()), (ks.StrKey(), vs.Int())])
```

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/custom_typing.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/key_specs.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/key_specs_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/pytype_support.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/type_conversion.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/typed_missing.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/value_specs.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/value_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/core/typing/value_specs_test.py` & `pyglove-0.3.1.dev20230411/pyglove/core/typing/value_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/__init__.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/early_stopping/base.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/__init__.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/base.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/base_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/mutators.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/neat.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/neat_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/nsga2.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/recombinators.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/selectors.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/where.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/evolution/where_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/mutfun/__init__.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/mutfun/base.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/mutfun/base_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/scalars/__init__.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/scalars/base.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/scalars/base_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/scalars/maths.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/scalars/maths_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/scalars/randoms.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/scalars/step_wise.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.3.1.dev20230411/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove/generators.py` & `pyglove-0.3.1.dev20230411/pyglove/generators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230410/pyglove.egg-info/PKG-INFO` & `pyglove-0.3.1.dev20230411/pyglove.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230410
+Version: 0.3.1.dev20230411
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,15 +42,15 @@
 
 PyGlove is a general-purpose library for Python object manipulation.
 It introduces symbolic object-oriented programming to Python, allowing
 direct manipulation of objects that makes meta-programs much easier to write.
 It has been used to handle complex machine learning scenarios, such as AutoML,
 as well as facilitating daily programming tasks with extra flexibility.
 
-PyGlove is lightweight and has no dependencies beyond the Python interpreter.
+PyGlove is lightweight and has very few dependencies beyond the Python interpreter.
 It provides:
 
 * A mutable symbolic object model for Python;
 * A rich set of operations for Python object manipulation;
 * A solution for automatic search of better Python programs, including:
   * An easy-to-use API for dropping search into an arbitrary pre-existing Python
     program;
```

### Comparing `pyglove-0.3.1.dev20230410/pyglove.egg-info/SOURCES.txt` & `pyglove-0.3.1.dev20230411/pyglove.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 pyglove/__init__.py
 pyglove/generators.py
 pyglove.egg-info/PKG-INFO
 pyglove.egg-info/SOURCES.txt
 pyglove.egg-info/dependency_links.txt
+pyglove.egg-info/requires.txt
 pyglove.egg-info/top_level.txt
 pyglove/core/__init__.py
 pyglove/core/logging.py
 pyglove/core/logging_test.py
 pyglove/core/detouring/__init__.py
 pyglove/core/detouring/class_detour.py
 pyglove/core/detouring/class_detour_test.py
@@ -51,14 +52,16 @@
 pyglove/core/hyper/object_template.py
 pyglove/core/hyper/object_template_test.py
 pyglove/core/object_utils/__init__.py
 pyglove/core/object_utils/codegen.py
 pyglove/core/object_utils/codegen_test.py
 pyglove/core/object_utils/common_traits.py
 pyglove/core/object_utils/common_traits_test.py
+pyglove/core/object_utils/docstr_utils.py
+pyglove/core/object_utils/docstr_utils_test.py
 pyglove/core/object_utils/formatting.py
 pyglove/core/object_utils/formatting_test.py
 pyglove/core/object_utils/hierarchical.py
 pyglove/core/object_utils/hierarchical_test.py
 pyglove/core/object_utils/missing.py
 pyglove/core/object_utils/missing_test.py
 pyglove/core/object_utils/thread_local.py
@@ -91,14 +94,15 @@
 pyglove/core/symbolic/list_test.py
 pyglove/core/symbolic/object.py
 pyglove/core/symbolic/object_test.py
 pyglove/core/symbolic/origin.py
 pyglove/core/symbolic/origin_test.py
 pyglove/core/symbolic/pure_symbolic.py
 pyglove/core/symbolic/schema_utils.py
+pyglove/core/symbolic/schema_utils_test.py
 pyglove/core/symbolic/symbolize.py
 pyglove/core/symbolic/symbolize_test.py
 pyglove/core/tuning/__init__.py
 pyglove/core/tuning/backend.py
 pyglove/core/tuning/backend_test.py
 pyglove/core/tuning/early_stopping.py
 pyglove/core/tuning/local_backend.py
```

### Comparing `pyglove-0.3.1.dev20230410/setup.py` & `pyglove-0.3.1.dev20230411/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,17 +34,30 @@
   if '--nightly' in sys.argv:
     nightly_label = datetime.datetime.now().strftime('%Y%m%d')
     version = f'{version}.dev{nightly_label}'
     sys.argv.remove('--nightly')
   return version
 
 
-def _parse_requirements(requirements_txt_path):
+def _parse_requirements(requirements_txt_path: str) -> list[str]:
+  """Returns a list of dependencies for setup() from requirements.txt."""
+
+  def _strip_comments_from_line(s: str) -> str:
+    """Parses a line of a requirements.txt file."""
+    requirement, *_ = s.split('#')
+    return requirement.strip()
+
+  # Currently a requirements.txt is being used to specify dependencies. In order
+  # to avoid specifying it in two places, we're going to use that file as the
+  # source of truth.
   with open(requirements_txt_path) as fp:
-    return fp.read().splitlines()
+    # Parse comments.
+    lines = [_strip_comments_from_line(line) for line in fp.read().splitlines()]
+    # Remove empty lines and direct github repos (not allowed in PyPI setups)
+    return [l for l in lines if (l and 'github.com' not in l)]
 
 
 _VERSION = _get_version()
 
 setup(
     name='pyglove',
     version=_VERSION,
@@ -53,15 +66,15 @@
     author='PyGlove Authors',
     description='PyGlove: A library for manipulating Python objects.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author_email='pyglove-authors@google.com',
     # Contained modules and scripts.
     packages=find_namespace_packages(include=['pyglove*']),
-    install_requires=[],
+    install_requires=_parse_requirements('requirements.txt'),
     extras_require={},
     requires_python='>=3.7',
     include_package_data=True,
     # PyPI package information.
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
@@ -72,9 +85,11 @@
         'Programming Language :: Python :: 3.9',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Human Machine Interfaces',
         'Topic :: Software Development :: Code Generators',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Software Development :: Libraries',
     ],
-    keywords='ai machine learning automl mutable symbolic framework meta-programming',
+    keywords=(
+        'ai machine learning automl mutable symbolic '
+        'framework meta-programming'),
 )
```

