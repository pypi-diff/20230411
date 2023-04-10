# Comparing `tmp/modularbayes-0.1.2.tar.gz` & `tmp/modularbayes-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modularbayes-0.1.2.tar", last modified: Sat Dec  3 19:21:51 2022, max compression
+gzip compressed data, was "modularbayes-0.1.3.tar", last modified: Mon Apr 10 23:43:42 2023, max compression
```

## Comparing `modularbayes-0.1.2.tar` & `modularbayes-0.1.3.tar`

### file list

```diff
@@ -1,85 +1,88 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.808639 modularbayes-0.1.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1070 2022-11-14 17:37:23.000000 modularbayes-0.1.2/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       57 2022-12-03 16:15:38.000000 modularbayes-0.1.2/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5876 2022-12-03 19:21:51.808639 modularbayes-0.1.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4879 2022-12-03 19:20:10.000000 modularbayes-0.1.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.788639 modularbayes-0.1.2/examples/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.792639 modularbayes-0.1.2/examples/epidemiology/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.796639 modularbayes-0.1.2/examples/epidemiology/configs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1751 2022-11-26 22:02:38.000000 modularbayes-0.1.2/examples/epidemiology/configs/flow_mf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2107 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/epidemiology/configs/flow_mf_vmp_map.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2153 2022-11-26 22:02:42.000000 modularbayes-0.1.2/examples/epidemiology/configs/flow_nsf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2338 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/epidemiology/configs/flow_nsf_vmp_flow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2512 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/epidemiology/configs/flow_nsf_vmp_map.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      431 2022-11-26 22:02:52.000000 modularbayes-0.1.2/examples/epidemiology/configs/mcmc.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.796639 modularbayes-0.1.2/examples/epidemiology/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      135 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/epidemiology/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      822 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/epidemiology/data/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13076 2022-11-26 22:36:44.000000 modularbayes-0.1.2/examples/epidemiology/flows.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5838 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/epidemiology/log_prob_fun.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1873 2022-11-26 23:08:02.000000 modularbayes-0.1.2/examples/epidemiology/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4485 2022-12-03 19:01:26.000000 modularbayes-0.1.2/examples/epidemiology/plot.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8091 2022-11-26 22:37:46.000000 modularbayes-0.1.2/examples/epidemiology/run_mcmc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18556 2022-11-26 22:09:28.000000 modularbayes-0.1.2/examples/epidemiology/train_flow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17089 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/epidemiology/train_vmp_flow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16526 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/epidemiology/train_vmp_map.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.796639 modularbayes-0.1.2/examples/random_effects/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.800639 modularbayes-0.1.2/examples/random_effects/configs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2581 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/random_effects/configs/flow_nsf_cut1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2523 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/random_effects/configs/flow_nsf_cut2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2581 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/random_effects/configs/flow_nsf_cut3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2499 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/random_effects/configs/flow_nsf_full.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3136 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/random_effects/configs/flow_nsf_vmp_flow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3098 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/random_effects/configs/flow_nsf_vmp_map.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      747 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/random_effects/configs/mcmc_cut1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      750 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/random_effects/configs/mcmc_cut2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      747 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/random_effects/configs/mcmc_cut3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      744 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/random_effects/configs/mcmc_full.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12911 2022-11-26 22:37:14.000000 modularbayes-0.1.2/examples/random_effects/flows.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3660 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/random_effects/log_prob_fun.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1873 2022-11-26 23:07:57.000000 modularbayes-0.1.2/examples/random_effects/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5240 2022-12-03 19:01:56.000000 modularbayes-0.1.2/examples/random_effects/plot.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9342 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/random_effects/run_mcmc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21709 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/random_effects/train_flow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30453 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/random_effects/train_vmp_flow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28496 2022-11-14 17:37:23.000000 modularbayes-0.1.2/examples/random_effects/train_vmp_map.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.800639 modularbayes-0.1.2/modularbayes/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2212 2022-12-03 18:53:36.000000 modularbayes-0.1.2/modularbayes/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.804639 modularbayes-0.1.2/modularbayes/_src/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-14 17:37:23.000000 modularbayes-0.1.2/modularbayes/_src/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.804639 modularbayes-0.1.2/modularbayes/_src/bijectors/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-14 17:37:23.000000 modularbayes-0.1.2/modularbayes/_src/bijectors/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4589 2022-11-14 17:37:23.000000 modularbayes-0.1.2/modularbayes/_src/bijectors/blockwise.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1663 2022-12-03 16:52:48.000000 modularbayes-0.1.2/modularbayes/_src/bijectors/conditional_bijector.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2456 2022-12-03 16:46:59.000000 modularbayes-0.1.2/modularbayes/_src/bijectors/conditional_chain.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1920 2022-11-14 17:37:23.000000 modularbayes-0.1.2/modularbayes/_src/bijectors/conditional_masked_coupling.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2498 2022-12-03 16:47:32.000000 modularbayes-0.1.2/modularbayes/_src/bijectors/conditional_masked_coupling_extra.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.804639 modularbayes-0.1.2/modularbayes/_src/conditioners/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-26 22:28:20.000000 modularbayes-0.1.2/modularbayes/_src/conditioners/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2668 2022-12-03 17:29:48.000000 modularbayes-0.1.2/modularbayes/_src/conditioners/base.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.804639 modularbayes-0.1.2/modularbayes/_src/distributions/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-14 17:37:23.000000 modularbayes-0.1.2/modularbayes/_src/distributions/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2022-11-14 17:37:23.000000 modularbayes-0.1.2/modularbayes/_src/distributions/conditional_transformed.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      712 2022-12-03 16:39:32.000000 modularbayes-0.1.2/modularbayes/_src/distributions/transformed.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.808639 modularbayes-0.1.2/modularbayes/_src/metaposterior/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       77 2022-11-14 17:37:23.000000 modularbayes-0.1.2/modularbayes/_src/metaposterior/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2322 2022-12-03 17:28:37.000000 modularbayes-0.1.2/modularbayes/_src/metaposterior/vmp_map.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1435 2022-12-03 17:24:53.000000 modularbayes-0.1.2/modularbayes/_src/typing.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.808639 modularbayes-0.1.2/modularbayes/_src/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-14 17:37:23.000000 modularbayes-0.1.2/modularbayes/_src/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2899 2022-12-03 17:29:05.000000 modularbayes-0.1.2/modularbayes/_src/utils/misc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6038 2022-11-14 17:37:23.000000 modularbayes-0.1.2/modularbayes/_src/utils/training.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.804639 modularbayes-0.1.2/modularbayes.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5876 2022-12-03 19:21:51.000000 modularbayes-0.1.2/modularbayes.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2600 2022-12-03 19:21:51.000000 modularbayes-0.1.2/modularbayes.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-12-03 19:21:51.000000 modularbayes-0.1.2/modularbayes.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-12-03 16:33:35.000000 modularbayes-0.1.2/modularbayes.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      240 2022-12-03 19:21:51.000000 modularbayes-0.1.2/modularbayes.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       35 2022-12-03 19:21:51.000000 modularbayes-0.1.2/modularbayes.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-03 19:21:51.808639 modularbayes-0.1.2/requirements/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2022-11-14 17:37:23.000000 modularbayes-0.1.2/requirements/requirements-devel.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2022-11-14 17:37:23.000000 modularbayes-0.1.2/requirements/requirements-setup.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2022-12-03 17:43:43.000000 modularbayes-0.1.2/requirements/requirements-tests.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2022-12-03 18:45:44.000000 modularbayes-0.1.2/requirements/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-12-03 19:21:51.808639 modularbayes-0.1.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2260 2022-11-14 17:37:23.000000 modularbayes-0.1.2/setup.py
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.191038 modularbayes-0.1.3/
+-rw-r--r--   0 carmona    (501) staff       (20)     1070 2023-04-10 23:31:55.000000 modularbayes-0.1.3/LICENSE
+-rw-r--r--   0 carmona    (501) staff       (20)       57 2023-04-10 23:31:55.000000 modularbayes-0.1.3/MANIFEST.in
+-rw-r--r--   0 carmona    (501) staff       (20)     5956 2023-04-10 23:43:42.190650 modularbayes-0.1.3/PKG-INFO
+-rw-r--r--   0 carmona    (501) staff       (20)     4959 2023-04-10 23:31:55.000000 modularbayes-0.1.3/README.md
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.145299 modularbayes-0.1.3/examples/
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.156129 modularbayes-0.1.3/examples/epidemiology/
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.159996 modularbayes-0.1.3/examples/epidemiology/configs/
+-rw-r--r--   0 carmona    (501) staff       (20)     2058 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/configs/flow_mf.py
+-rw-r--r--   0 carmona    (501) staff       (20)     2396 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/configs/flow_mf_vmp_map.py
+-rw-r--r--   0 carmona    (501) staff       (20)     2467 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/configs/flow_nsf.py
+-rw-r--r--   0 carmona    (501) staff       (20)     2675 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/configs/flow_nsf_vmp_flow.py
+-rw-r--r--   0 carmona    (501) staff       (20)     2810 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/configs/flow_nsf_vmp_map.py
+-rw-r--r--   0 carmona    (501) staff       (20)      742 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/configs/mcmc.py
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.161399 modularbayes-0.1.3/examples/epidemiology/data/
+-rw-r--r--   0 carmona    (501) staff       (20)      135 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/data/__init__.py
+-rw-r--r--   0 carmona    (501) staff       (20)      822 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/data/load.py
+-rw-r--r--   0 carmona    (501) staff       (20)    13927 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/flows.py
+-rw-r--r--   0 carmona    (501) staff       (20)     4840 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/log_prob_fun.py
+-rw-r--r--   0 carmona    (501) staff       (20)     1637 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/main.py
+-rw-r--r--   0 carmona    (501) staff       (20)     6526 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/plot.py
+-rw-r--r--   0 carmona    (501) staff       (20)    17477 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/sample_mcmc.py
+-rw-r--r--   0 carmona    (501) staff       (20)    14600 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/train_flow.py
+-rw-r--r--   0 carmona    (501) staff       (20)    14132 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/train_vmp_flow.py
+-rw-r--r--   0 carmona    (501) staff       (20)    14165 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/train_vmp_map.py
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.166036 modularbayes-0.1.3/examples/random_effects/
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.173342 modularbayes-0.1.3/examples/random_effects/configs/
+-rw-r--r--   0 carmona    (501) staff       (20)     2595 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_cut1.py
+-rw-r--r--   0 carmona    (501) staff       (20)     2537 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_cut2.py
+-rw-r--r--   0 carmona    (501) staff       (20)     2594 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_cut3.py
+-rw-r--r--   0 carmona    (501) staff       (20)     2512 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_full.py
+-rw-r--r--   0 carmona    (501) staff       (20)     3232 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_vmp_flow.py
+-rw-r--r--   0 carmona    (501) staff       (20)     3197 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_vmp_map.py
+-rw-r--r--   0 carmona    (501) staff       (20)      874 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/mcmc_cut1.py
+-rw-r--r--   0 carmona    (501) staff       (20)      877 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/mcmc_cut2.py
+-rw-r--r--   0 carmona    (501) staff       (20)      874 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/mcmc_cut3.py
+-rw-r--r--   0 carmona    (501) staff       (20)      830 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/mcmc_full.py
+-rw-r--r--   0 carmona    (501) staff       (20)    12151 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/flows.py
+-rw-r--r--   0 carmona    (501) staff       (20)     3064 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/log_prob_fun.py
+-rw-r--r--   0 carmona    (501) staff       (20)     1637 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/main.py
+-rw-r--r--   0 carmona    (501) staff       (20)     5650 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/plot.py
+-rw-r--r--   0 carmona    (501) staff       (20)    17434 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/sample_mcmc.py
+-rw-r--r--   0 carmona    (501) staff       (20)    15350 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/train_flow.py
+-rw-r--r--   0 carmona    (501) staff       (20)    14409 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/train_vmp_flow.py
+-rw-r--r--   0 carmona    (501) staff       (20)    13460 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/train_vmp_map.py
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.173791 modularbayes-0.1.3/modularbayes/
+-rw-r--r--   0 carmona    (501) staff       (20)     2763 2023-04-10 23:43:16.000000 modularbayes-0.1.3/modularbayes/__init__.py
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.177903 modularbayes-0.1.3/modularbayes/_src/
+-rw-r--r--   0 carmona    (501) staff       (20)        0 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/__init__.py
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.180741 modularbayes-0.1.3/modularbayes/_src/bijectors/
+-rw-r--r--   0 carmona    (501) staff       (20)        0 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/bijectors/__init__.py
+-rw-r--r--   0 carmona    (501) staff       (20)     4245 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/bijectors/blockwise.py
+-rw-r--r--   0 carmona    (501) staff       (20)     1663 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/bijectors/conditional_bijector.py
+-rw-r--r--   0 carmona    (501) staff       (20)     2456 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/bijectors/conditional_chain.py
+-rw-r--r--   0 carmona    (501) staff       (20)     1920 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/bijectors/conditional_masked_coupling.py
+-rw-r--r--   0 carmona    (501) staff       (20)     2498 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/bijectors/conditional_masked_coupling_extra.py
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.181407 modularbayes-0.1.3/modularbayes/_src/conditioners/
+-rw-r--r--   0 carmona    (501) staff       (20)        0 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/conditioners/__init__.py
+-rw-r--r--   0 carmona    (501) staff       (20)     2668 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/conditioners/base.py
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.183338 modularbayes-0.1.3/modularbayes/_src/distributions/
+-rw-r--r--   0 carmona    (501) staff       (20)        0 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/distributions/__init__.py
+-rw-r--r--   0 carmona    (501) staff       (20)     2873 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/distributions/conditional_transformed.py
+-rw-r--r--   0 carmona    (501) staff       (20)      712 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/distributions/transformed.py
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.184643 modularbayes-0.1.3/modularbayes/_src/metaposterior/
+-rw-r--r--   0 carmona    (501) staff       (20)        0 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/metaposterior/__init__.py
+-rw-r--r--   0 carmona    (501) staff       (20)     2325 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/metaposterior/vmp_map.py
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.187035 modularbayes-0.1.3/modularbayes/_src/smi/
+-rw-r--r--   0 carmona    (501) staff       (20)     6183 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/smi/elbo.py
+-rw-r--r--   0 carmona    (501) staff       (20)     5131 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/smi/sampling.py
+-rw-r--r--   0 carmona    (501) staff       (20)     1313 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/typing.py
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.188383 modularbayes-0.1.3/modularbayes/_src/utils/
+-rw-r--r--   0 carmona    (501) staff       (20)        0 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/utils/__init__.py
+-rw-r--r--   0 carmona    (501) staff       (20)     3840 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/utils/misc.py
+-rw-r--r--   0 carmona    (501) staff       (20)     6007 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/utils/training.py
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.176803 modularbayes-0.1.3/modularbayes.egg-info/
+-rw-r--r--   0 carmona    (501) staff       (20)     5956 2023-04-10 23:43:42.000000 modularbayes-0.1.3/modularbayes.egg-info/PKG-INFO
+-rw-r--r--   0 carmona    (501) staff       (20)     2670 2023-04-10 23:43:42.000000 modularbayes-0.1.3/modularbayes.egg-info/SOURCES.txt
+-rw-r--r--   0 carmona    (501) staff       (20)        1 2023-04-10 23:43:42.000000 modularbayes-0.1.3/modularbayes.egg-info/dependency_links.txt
+-rw-r--r--   0 carmona    (501) staff       (20)        1 2023-04-10 23:40:56.000000 modularbayes-0.1.3/modularbayes.egg-info/not-zip-safe
+-rw-r--r--   0 carmona    (501) staff       (20)       84 2023-04-10 23:43:42.000000 modularbayes-0.1.3/modularbayes.egg-info/requires.txt
+-rw-r--r--   0 carmona    (501) staff       (20)       47 2023-04-10 23:43:42.000000 modularbayes-0.1.3/modularbayes.egg-info/top_level.txt
+drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.190140 modularbayes-0.1.3/requirements/
+-rw-r--r--   0 carmona    (501) staff       (20)       26 2023-04-10 23:31:55.000000 modularbayes-0.1.3/requirements/requirements-devel.txt
+-rw-r--r--   0 carmona    (501) staff       (20)       43 2023-04-10 23:31:55.000000 modularbayes-0.1.3/requirements/requirements-setup.txt
+-rw-r--r--   0 carmona    (501) staff       (20)       14 2023-04-10 23:31:55.000000 modularbayes-0.1.3/requirements/requirements-tests.txt
+-rw-r--r--   0 carmona    (501) staff       (20)       84 2023-04-10 23:31:55.000000 modularbayes-0.1.3/requirements/requirements.txt
+-rw-r--r--   0 carmona    (501) staff       (20)       38 2023-04-10 23:43:42.191197 modularbayes-0.1.3/setup.cfg
+-rw-r--r--   0 carmona    (501) staff       (20)     2260 2023-04-10 23:31:55.000000 modularbayes-0.1.3/setup.py
```

### Comparing `modularbayes-0.1.2/LICENSE` & `modularbayes-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.2/PKG-INFO` & `modularbayes-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modularbayes
-Version: 0.1.2
+Version: 0.1.3
 Summary: Modular Bayesian Inference.
 Home-page: https://github.com/chriscarmona/modularbayes
 Author: Chris Carmona
 Author-email: carmona@stats.ox.ac.uk
 Maintainer-email: carmona@stats.ox.ac.uk
 License: MIT
 Keywords: modular bayesian inference cut smi posterior probability distribution
@@ -44,14 +44,15 @@
 
 We provide code to replicate all the experiments from our article in the [examples](https://github.com/chriscarmona/modularbayes/tree/main/examples) folder.
 There are main two examples: 1) epidemiological model and 2) random effects model.
 By executing the `run.sh` bash script in that folder, one can train all variational posteriors and produce visualizations and summaries (follow [*Installation instructions*](#installation-instructions) and examine `run.sh` before execution).
 
 You can customize the output directories within the script and choose the experiments that you wish to run.
 ```bash
+pip install -Ur examples/requirements.txt
 chmod +x examples/run.sh
 bash examples/run.sh
 ```
 Results produced during the optimization can be monitored in [Tensorboard](https://www.tensorflow.org/tensorboard):
 ```bash
 WORK_DIR=$HOME/modularbayes-output
 tensorboard --logdir=$WORK_DIR
@@ -59,15 +60,15 @@
 
 ## Installation instructions
 
 1. \[Optional] Create a new virtual environment for this project (see [*Create a virtual environment*](#create-a-virtual-environment) below).
 2. Install JAX. This may vary according to your CUDA version (See [JAX installation](https://github.com/google/jax#installation)).
 3. Install the latest released version of `modularbayes` from [Pypi](https://pypi.org/project/modularbayes/) via:
 ```bash
-pip install modularbayes
+pip install -U modularbayes
 ```
 or you can install the latest development version from GitHub:
 ```bash
 pip install git+https://github.com/chriscarmona/modularbayes
 ```
 
 ## Citation
@@ -104,14 +105,15 @@
 ```
 
 ### Creating a virtual environment
 
 For OSX or Linux, you can use `venv` (see the [venv documentation](https://docs.python.org/3/library/venv.html)).
 
 ```bash
+rm -rf ~/.virtualenvs/modularbayes
 python3 -m venv ~/.virtualenvs/modularbayes
 source ~/.virtualenvs/modularbayes/bin/activate
 pip install -U pip
 pip install -U setuptools wheel
 ```
 
 Feel free to change the folder where the virtual environment is created by replacing `~/.virtualenvs/modularbayes` with a path of your choice in both commands.
```

### Comparing `modularbayes-0.1.2/README.md` & `modularbayes-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 We provide code to replicate all the experiments from our article in the [examples](https://github.com/chriscarmona/modularbayes/tree/main/examples) folder.
 There are main two examples: 1) epidemiological model and 2) random effects model.
 By executing the `run.sh` bash script in that folder, one can train all variational posteriors and produce visualizations and summaries (follow [*Installation instructions*](#installation-instructions) and examine `run.sh` before execution).
 
 You can customize the output directories within the script and choose the experiments that you wish to run.
 ```bash
+pip install -Ur examples/requirements.txt
 chmod +x examples/run.sh
 bash examples/run.sh
 ```
 Results produced during the optimization can be monitored in [Tensorboard](https://www.tensorflow.org/tensorboard):
 ```bash
 WORK_DIR=$HOME/modularbayes-output
 tensorboard --logdir=$WORK_DIR
@@ -34,15 +35,15 @@
 
 ## Installation instructions
 
 1. \[Optional] Create a new virtual environment for this project (see [*Create a virtual environment*](#create-a-virtual-environment) below).
 2. Install JAX. This may vary according to your CUDA version (See [JAX installation](https://github.com/google/jax#installation)).
 3. Install the latest released version of `modularbayes` from [Pypi](https://pypi.org/project/modularbayes/) via:
 ```bash
-pip install modularbayes
+pip install -U modularbayes
 ```
 or you can install the latest development version from GitHub:
 ```bash
 pip install git+https://github.com/chriscarmona/modularbayes
 ```
 
 ## Citation
@@ -79,14 +80,15 @@
 ```
 
 ### Creating a virtual environment
 
 For OSX or Linux, you can use `venv` (see the [venv documentation](https://docs.python.org/3/library/venv.html)).
 
 ```bash
+rm -rf ~/.virtualenvs/modularbayes
 python3 -m venv ~/.virtualenvs/modularbayes
 source ~/.virtualenvs/modularbayes/bin/activate
 pip install -U pip
 pip install -U setuptools wheel
 ```
 
 Feel free to change the folder where the virtual environment is created by replacing `~/.virtualenvs/modularbayes` with a path of your choice in both commands.
```

### Comparing `modularbayes-0.1.2/examples/epidemiology/configs/flow_mf.py` & `modularbayes-0.1.3/examples/epidemiology/configs/flow_mf.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,29 @@
 import ml_collections
 
 
 def get_config():
   """Get the hyperparameter configuration."""
   config = ml_collections.ConfigDict()
 
+  # Model hyper-parameters, defining the prior
+  config.prior_hparams = ml_collections.ConfigDict()
+  config.prior_hparams.phi_alpha = 1.
+  config.prior_hparams.phi_beta = 1.
+  config.prior_hparams.theta0_scale = 100.
+  config.prior_hparams.theta1_concentration = 1
+  config.prior_hparams.theta1_rate = 0.1
+
   config.method = 'flow'
 
   # SMI degree of influence of the poisson module
-  config.smi_eta = 1.0
+  config.smi_eta_cancer = 1.0
 
   # Defined in `epidemiology.models.flows`.
-  config.flow_name = 'mean_field'
+  config.flow_name = 'mf'
 
   # kwargs to be passed to the flow
   config.flow_kwargs = ml_collections.ConfigDict()
 
   # Number of posteriors samples to approximate the variational loss (ELBO).
   config.num_samples_elbo = 100
 
@@ -47,15 +55,15 @@
   # Initial seed for random numbers.
   config.seed = 0
 
   # How often to log images to monitor convergence.
   config.log_img_steps = config.training_steps / 10
 
   # Number of posteriors samples used in the plots.
-  config.num_samples_plot = 10_000
+  config.num_samples_plot = 40_000
 
   # How often to save model checkpoints.
   config.checkpoint_steps = config.training_steps / 4
 
   # How many checkpoints to keep.
   config.checkpoints_keep = 1
```

### Comparing `modularbayes-0.1.2/examples/epidemiology/configs/flow_mf_vmp_map.py` & `modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_cut3.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,72 +3,84 @@
 import ml_collections
 
 
 def get_config():
   """Get the hyperparameter configuration."""
   config = ml_collections.ConfigDict()
 
-  config.method = 'vmp_map'
+  # Data
+  config.num_groups = 30
+  config.num_obs_groups = [5, 5] + [5 for _ in range(config.num_groups - 2)]
+  config.loc_groups = [10., 5.] + [0. for _ in range(config.num_groups - 2)]
+  config.scale_groups = [1. for _ in range(config.num_groups)]
 
-  # Defined in `epidemiology.models.flows`.
-  config.flow_name = 'mean_field'
+  # Model hyper-parameters, defining the prior.
+  config.prior_hparams = None
 
+  config.method = 'flow'
+
+  # Defined in `flows`.
+  config.flow_name = 'nsf'
   # kwargs to be passed to the flow
   config.flow_kwargs = ml_collections.ConfigDict()
+  # Number of layers to use in the flow.
+  config.flow_kwargs.num_layers = 8
+  # Hidden sizes of the MLP conditioner.
+  config.flow_kwargs.hidden_sizes = [30] * 3 + [10]
+  # Number of bins to use in the rational-quadratic spline.
+  config.flow_kwargs.num_bins = 10
+  # the lower bound of the spline's range
+  config.flow_kwargs.range_min = -10.
+  # the upper bound of the spline's range
+  config.flow_kwargs.range_max = 40.
+
+  # SMI degree of influence
+  config.smi_eta_groups = [1., 0.0001
+                          ] + [1. for _ in range(config.num_groups - 2)]
+  config.plot_suffix = '_cut3'
 
-  # Number of posteriors samples to approximate the variational loss (ELBO).
-  config.num_samples_elbo = 50
+  # Number of samples used to estimate the ELBO.
+  config.num_samples_elbo = 10
 
   # Number of training steps to run.
-  config.training_steps = 10_000
+  config.training_steps = 30_000
 
   # Optimizer.
   config.optim_kwargs = ml_collections.ConfigDict()
   config.optim_kwargs.grad_clip_value = 1.0
   config.optim_kwargs.lr_schedule_name = 'warmup_exponential_decay_schedule'
   config.optim_kwargs.lr_schedule_kwargs = ml_collections.ConfigDict()
   config.optim_kwargs.lr_schedule_kwargs = {
       'init_value': 0.,
-      'peak_value': 3e-3,
-      'warmup_steps': 3_000,
+      'peak_value': 2e-3,
+      'warmup_steps': 2_000,
       'transition_steps': 10_000,
       'decay_rate': 0.5,
       'transition_begin': 0,
       'staircase': False,
       'end_value': None,
   }
 
   # How often to evaluate the model.
-  config.eval_steps = config.training_steps / 10
-  config.num_samples_eval = 5_000
+  config.eval_steps = int(config.training_steps / 10)
+  # config.eval_steps = config.training_steps / 10
 
   # Initial seed for random numbers.
   config.seed = 0
 
   # How often to log images to monitor convergence.
-  config.log_img_steps = config.training_steps / 10
+  config.log_img_steps = int(config.training_steps / 10)
 
   # Number of posteriors samples used in the plots.
-  config.num_samples_plot = 10_000
+  config.num_samples_plot = 40_000
 
-  config.eta_plot = [[1., 0.001], [1., 0.1], [1., 1.]]
+  config.num_samples_eval = 1_000
 
   # How often to save model checkpoints.
-  config.checkpoint_steps = config.training_steps / 4
+  config.checkpoint_steps = int(config.training_steps / 4)
 
   # How many checkpoints to keep.
   config.checkpoints_keep = 1
 
-  # Arguments for the Variational Meta-Posterior map
-  config.vmp_map_name = 'VmpMap'
-  config.vmp_map_kwargs = ml_collections.ConfigDict()
-  config.vmp_map_kwargs.hidden_sizes = [10] * 5
-
-  # Number of samples of eta for Meta-Posterior training
-  config.num_samples_eta = 25
-  config.eta_sampling_a = 0.2
-  config.eta_sampling_b = 1.0
-
-  config.lambda_idx_plot = [5 * i for i in range(5)]
-  config.constant_lambda_ignore_plot = False
+  config.num_samples_log_prob_test = 10_000
 
   return config
```

### Comparing `modularbayes-0.1.2/examples/epidemiology/configs/flow_nsf.py` & `modularbayes-0.1.3/examples/epidemiology/configs/flow_nsf.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,26 @@
 import ml_collections
 
 
 def get_config():
   """Get the hyperparameter configuration."""
   config = ml_collections.ConfigDict()
 
+  # Model hyper-parameters, defining the prior.
+  config.prior_hparams = ml_collections.ConfigDict()
+  config.prior_hparams.phi_alpha = 1.
+  config.prior_hparams.phi_beta = 1.
+  config.prior_hparams.theta0_scale = 100.
+  config.prior_hparams.theta1_concentration = 1
+  config.prior_hparams.theta1_rate = 0.1
+
   config.method = 'flow'
 
   # SMI degree of influence
-  config.smi_eta = 1.0
+  config.smi_eta_cancer = 1.0
 
   # Defined in `epidemiology.models.flows`.
   config.flow_name = 'nsf'
 
   # kwargs to be passed to the flow
   config.flow_kwargs = ml_collections.ConfigDict()
   # Number of layers to use in the flow.
@@ -45,27 +53,27 @@
       'warmup_steps': 1_000,
       'transition_steps': config.training_steps / 3,
       'decay_rate': 0.25,
       'transition_begin': 0,
       'staircase': False,
       'end_value': None,
   }
-  
+
   # How often to evaluate the model.
   config.eval_steps = config.training_steps / 10
   config.num_samples_eval = 5_000
 
   # Initial seed for random numbers.
   config.seed = 0
 
   # How often to log images to monitor convergence.
   config.log_img_steps = config.training_steps / 10
 
   # Number of posteriors samples used in the plots.
-  config.num_samples_plot = 10_000
+  config.num_samples_plot = 40_000
 
   config.num_samples_eval = 10_000
 
   # How often to save model checkpoints.
   config.checkpoint_steps = config.training_steps / 4
 
   # How many checkpoints to keep.
```

### Comparing `modularbayes-0.1.2/examples/epidemiology/configs/flow_nsf_vmp_flow.py` & `modularbayes-0.1.3/examples/epidemiology/configs/flow_nsf_vmp_flow.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 import ml_collections
 
 
 def get_config():
   """Get the hyperparameter configuration."""
   config = ml_collections.ConfigDict()
 
+  # Model hyper-parameters, defining the prior.
+  config.prior_hparams = ml_collections.ConfigDict()
+  config.prior_hparams.phi_alpha = 1.
+  config.prior_hparams.phi_beta = 1.
+  config.prior_hparams.theta0_scale = 100.
+  config.prior_hparams.theta1_concentration = 1
+  config.prior_hparams.theta1_rate = 0.1
+
   config.method = 'vmp_flow'
 
   # Defined in `epidemiology.models.flows`.
   config.flow_name = 'meta_nsf'
 
   # kwargs to be passed to the flow
   config.flow_kwargs = ml_collections.ConfigDict()
@@ -57,17 +65,18 @@
   # Initial seed for random numbers.
   config.seed = 0
 
   # How often to log images to monitor convergence.
   config.log_img_steps = config.training_steps / 10
 
   # Number of posteriors samples used in the plots.
-  config.num_samples_plot = 10_000
+  config.num_samples_plot = 40_000
 
-  config.eta_plot = [[1., 0.001], [1., 0.1], [1., 1.]]
+  config.smi_eta_dim = 2
+  config.smi_eta_cancer_plot = (0.001, 0.1, 0.2, 0.5, 1.)
 
   # How often to save model checkpoints.
   config.checkpoint_steps = config.training_steps / 4
 
   # How many checkpoints to keep.
   config.checkpoints_keep = 1
```

### Comparing `modularbayes-0.1.2/examples/epidemiology/configs/flow_nsf_vmp_map.py` & `modularbayes-0.1.3/examples/epidemiology/configs/flow_nsf_vmp_map.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 import ml_collections
 
 
 def get_config():
   """Get the hyperparameter configuration."""
   config = ml_collections.ConfigDict()
 
+  # Model hyper-parameters, defining the prior.
+  config.prior_hparams = ml_collections.ConfigDict()
+  config.prior_hparams.phi_alpha = 1.
+  config.prior_hparams.phi_beta = 1.
+  config.prior_hparams.theta0_scale = 100.
+  config.prior_hparams.theta1_concentration = 1
+  config.prior_hparams.theta1_rate = 0.1
+
   config.method = 'vmp_map'
 
   # Defined in `epidemiology.models.flows`.
   config.flow_name = 'nsf'
 
   # kwargs to be passed to the flow
   config.flow_kwargs = ml_collections.ConfigDict()
@@ -54,31 +62,31 @@
   # Initial seed for random numbers.
   config.seed = 0
 
   # How often to log images to monitor convergence.
   config.log_img_steps = config.training_steps / 10
 
   # Number of posteriors samples used in the plots.
-  config.num_samples_plot = 10_000
+  config.num_samples_plot = 40_000
 
-  config.eta_plot = [[1., 0.001], [1., 0.1], [1., 1.]]
+  config.smi_eta_dim = 2
+  config.smi_eta_cancer_plot = (0.001, 0.1, 0.2, 0.5, 1.)
 
   # How often to save model checkpoints.
   config.checkpoint_steps = config.training_steps / 4
 
   # How many checkpoints to keep.
   config.checkpoints_keep = 1
 
   # Arguments for the Variational Meta-Posterior map
-  config.vmp_map_name = 'VmpMap'
+  config.vmp_map_name = 'MLPVmpMap'
   config.vmp_map_kwargs = ml_collections.ConfigDict()
   config.vmp_map_kwargs.hidden_sizes = [10] * 5
 
   # Number of samples of eta for Meta-Posterior training
   config.num_samples_eta = 25
   config.eta_sampling_a = 0.2
   config.eta_sampling_b = 1.0
 
-  config.lambda_idx_plot = [50 * i for i in range(5)]
-  config.constant_lambda_ignore_plot = True
+  config.vmpmap_curves_idx = [50 * i for i in range(5)]
 
   return config
```

### Comparing `modularbayes-0.1.2/examples/epidemiology/data/load.py` & `modularbayes-0.1.3/examples/epidemiology/data/load.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.2/examples/epidemiology/flows.py` & `modularbayes-0.1.3/examples/epidemiology/flows.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,21 +3,50 @@
 import math
 
 from jax import numpy as jnp
 import distrax
 from tensorflow_probability.substrates import jax as tfp
 
 import modularbayes
-
 from modularbayes._src.typing import Any, Array, Dict, Sequence
 
+from log_prob_fun import ModelParamsCut, ModelParamsNoCut
+
 tfb = tfp.bijectors
 
 
-def mean_field_phi(
+def bijector_domain_nocut() -> distrax.Bijector:
+  """Returns a distrax bijector for the uncut parameters
+  The bijector maps from an unconstrained space to the parameter domain.
+  """
+  # phi goes to [0,1]
+  bij_nocut = distrax.Block(distrax.Sigmoid(), 1)
+  return bij_nocut
+
+
+def bijector_domain_cut() -> distrax.Bijector:
+  """Returns a distrax bijector for the cut parameters
+  The bijector maps from an unconstrained space to the parameter domain.
+  """
+  # theta1 goes to [-Inf,Inf]
+  # theta2 goes to [0,Inf]
+  block_bijectors = [
+      distrax.Block(tfb.Identity(), 1),
+      distrax.Block(tfb.Softplus(), 1),
+  ]
+  block_sizes = [
+      1,
+      1,
+  ]
+  bij_cut = modularbayes.Blockwise(
+      bijectors=block_bijectors, block_sizes=block_sizes)
+  return bij_cut
+
+
+def get_q_nocut_mf(
     phi_dim: int,
     **_,
 ) -> distrax.Transformed:
   """Creates a Mean Field Flow."""
 
   flow_dim = phi_dim
   event_shape = (flow_dim,)
@@ -27,29 +56,29 @@
   # Layer 1: Trainable Affine transformation
   conditioner = modularbayes.MeanFieldConditioner(flow_dim=flow_dim)
   loc, log_scale = conditioner()
   flow_layers.append(
       distrax.Block(distrax.ScalarAffine(shift=loc, log_scale=log_scale), 1))
 
   # Last Layer: Map values to parameter domain
-  # phi goes to [0,1]
-  flow_layers.append(distrax.Block(distrax.Sigmoid(), 1))
+  bij_nocut = bijector_domain_nocut()
+  flow_layers.append(bij_nocut)
 
-  # Chain all layers together
+  # Chain all flow layers together
   flow = distrax.Chain(flow_layers[::-1])
 
   base_distribution = distrax.MultivariateNormalDiag(
       loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
 
   q_distr = modularbayes.Transformed(base_distribution, flow)
 
   return q_distr
 
 
-def mean_field_theta(
+def get_q_cutgivennocut_mf(
     theta_dim: int,
     **_,
 ) -> modularbayes.ConditionalTransformed:
   """Creates a Mean Field Flow."""
 
   flow_dim = theta_dim
 
@@ -61,40 +90,29 @@
   conditioner = modularbayes.MeanFieldConditioner(flow_dim=flow_dim)
   loc, log_scale = conditioner()
   flow_layers.append(
       distrax.Block(distrax.ScalarAffine(shift=loc, log_scale=log_scale), 1))
   # flow_layers.append(tfb.Shift(loc)(tfb.Scale(log_scale=log_scale)))
 
   # Last layer: Map values to parameter domain
-  # theta1 goes to [-Inf,Inf]
-  # theta2 goes to [0,Inf]
-  block_bijectors = [
-      distrax.Block(tfb.Identity(), 1),
-      distrax.Block(tfb.Softplus(), 1),
-  ]
-  block_sizes = [
-      1,
-      1,
-  ]
-  flow_layers.append(
-      modularbayes.Blockwise(
-          bijectors=block_bijectors, block_sizes=block_sizes))
+  bij_cut = bijector_domain_cut()
+  flow_layers.append(bij_cut)
 
-  # Chain all layers together
+  # Chain all flow layers together
   flow = modularbayes.ConditionalChain(flow_layers[::-1])
 
   base_distribution = distrax.MultivariateNormalDiag(
       loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
 
   q_distr = modularbayes.ConditionalTransformed(base_distribution, flow)
 
   return q_distr
 
 
-def nsf_phi(
+def get_q_nocut_nsf(
     phi_dim: int,
     num_layers: int,
     hidden_sizes: Sequence[int],
     num_bins: int,
     range_min: float = 0.,
     range_max: float = 1.,
     **_,
@@ -127,47 +145,47 @@
   mask = mask.astype(bool)
 
   # Number of parameters for the rational-quadratic spline:
   # - `num_bins` bin widths
   # - `num_bins` bin heights
   # - `num_bins + 1` knot slopes
   # for a total of `3 * num_bins + 1` parameters.
-
   for _ in range(num_layers):
     layer = distrax.MaskedCoupling(
         mask=mask,
         bijector=bijector_fn,
         conditioner=modularbayes.MLPConditioner(
             output_dim=math.prod(event_shape),
             hidden_sizes=hidden_sizes,
             num_bijector_params=num_bijector_params,
-            name='conditioner_phi',
+            name='conditioner_nocut',
         ),
     )
     flow_layers.append(layer)
     # Flip the mask after each layer.
     mask = jnp.logical_not(mask)
 
   # Last layer: Map values to parameter domain
-  # phi goes to [0,1]
-  flow_layers.append(distrax.Block(distrax.Sigmoid(), 1))
+  bij_nocut = bijector_domain_nocut()
+  flow_layers.append(bij_nocut)
 
+  # Chain all flow layers together
   flow = distrax.Chain(flow_layers[::-1])
 
   # base_distribution = distrax.Independent(
   #     distrax.Uniform(low=jnp.zeros(event_shape), high=jnp.ones(event_shape)),
   #     reinterpreted_batch_ndims=len(event_shape))
 
   base_distribution = distrax.MultivariateNormalDiag(
       loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
 
   return modularbayes.Transformed(base_distribution, flow)
 
 
-def nsf_theta(
+def get_q_cutgivennocut_nsf(
     theta_dim: int,
     num_layers: int,
     hidden_sizes: Sequence[int],
     num_bins: int,
     range_min: float = 0.,
     range_max: float = 1.,
     **_,
@@ -216,40 +234,31 @@
         ),
     )
     flow_layers.append(layer)
     # Flip the mask after each layer.
     mask = jnp.logical_not(mask)
 
   # Last layer: Map values to parameter domain
-  # theta1 goes to [-Inf,Inf]
-  # theta2 goes to [0,Inf]
-  block_bijectors = [
-      distrax.Block(tfb.Identity(), 1),
-      distrax.Block(tfb.Softplus(), 1),
-  ]
-  block_sizes = [
-      1,
-      1,
-  ]
-  flow_layers.append(
-      modularbayes.Blockwise(
-          bijectors=block_bijectors, block_sizes=block_sizes))
+  bij_cut = bijector_domain_cut()
+  flow_layers.append(bij_cut)
+
+  # Chain all flow layers together
   flow = modularbayes.ConditionalChain(flow_layers[::-1])
 
   # base_distribution = distrax.Independent(
   #     distrax.Uniform(low=jnp.zeros(event_shape), high=jnp.ones(event_shape)),
   #     reinterpreted_batch_ndims=len(event_shape))
 
   base_distribution = distrax.MultivariateNormalDiag(
       loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
 
   return modularbayes.ConditionalTransformed(base_distribution, flow)
 
 
-def meta_nsf_phi(
+def get_q_nocut_meta_nsf(
     phi_dim: int,
     num_layers: int,
     hidden_sizes_conditioner: Sequence[int],
     hidden_sizes_conditioner_eta: Sequence[int],
     num_bins: int,
     range_min: float = 0.,
     range_max: float = 1.,
@@ -292,44 +301,45 @@
     layer = modularbayes.EtaConditionalMaskedCoupling(
         mask=mask,
         bijector=bijector_fn,
         conditioner_eta=modularbayes.MLPConditioner(
             output_dim=math.prod(event_shape),
             hidden_sizes=hidden_sizes_conditioner_eta,
             num_bijector_params=num_bijector_params,
-            name='conditioner_eta_phi',
+            name='conditioner_eta_nocut',
         ),
         conditioner=modularbayes.MLPConditioner(
             output_dim=math.prod(event_shape),
             hidden_sizes=hidden_sizes_conditioner,
             num_bijector_params=num_bijector_params,
-            name='conditioner_phi',
+            name='conditioner_nocut',
         ),
     )
     flow_layers.append(layer)
     # Flip the mask after each layer.
     mask = jnp.logical_not(mask)
 
-  # Last layer: Map values to parameter domain
-  # phi goes to [0,1]
-  flow_layers.append(distrax.Block(distrax.Sigmoid(), 1))
+  # Last Layer: Map values to parameter domain
+  bij_nocut = bijector_domain_nocut()
+  flow_layers.append(bij_nocut)
 
+  # Chain all flow layers together
   flow = modularbayes.ConditionalChain(flow_layers[::-1])
 
   # base_distribution = distrax.Independent(
   #     distrax.Uniform(low=jnp.zeros(event_shape), high=jnp.ones(event_shape)),
   #     reinterpreted_batch_ndims=len(event_shape))
 
   base_distribution = distrax.MultivariateNormalDiag(
       loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
 
   return modularbayes.ConditionalTransformed(base_distribution, flow)
 
 
-def meta_nsf_theta(
+def get_q_cutgivennocut_meta_nsf(
     theta_dim: int,
     num_layers: int,
     hidden_sizes_conditioner: Sequence[int],
     hidden_sizes_conditioner_eta: Sequence[int],
     num_bins: int,
     range_min: float = 0.,
     range_max: float = 1.,
@@ -386,69 +396,78 @@
         ),
     )
     flow_layers.append(layer)
     # Flip the mask after each layer.
     mask = jnp.logical_not(mask)
 
   # Last layer: Map values to parameter domain
-  # theta1 goes to [-Inf,Inf]
-  # theta2 goes to [0,Inf]
-  block_bijectors = [
-      distrax.Block(tfb.Identity(), 1),
-      distrax.Block(tfb.Softplus(), 1),
-  ]
-  block_sizes = [
-      1,
-      1,
-  ]
-  flow_layers.append(
-      modularbayes.Blockwise(
-          bijectors=block_bijectors, block_sizes=block_sizes))
+  bij_cut = bijector_domain_cut()
+  flow_layers.append(bij_cut)
+
+  # Chain all flow layers together
   flow = modularbayes.ConditionalChain(flow_layers[::-1])
 
   base_distribution = distrax.MultivariateNormalDiag(
       loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
 
   q_distr = modularbayes.ConditionalTransformed(base_distribution, flow)
 
   return q_distr
 
 
-def split_flow_phi(
-    samples: Array,
+def split_flow_nocut(
+    concat_params: Array,
     phi_dim: int,
     **_,
 ) -> Dict[str, Any]:
   """Get model parameters by splitting samples from the flow."""
 
   flow_dim = phi_dim
 
-  assert samples.ndim == 2
-  assert samples.shape[-1] == flow_dim
-
-  samples_dict = {}
+  assert concat_params.ndim == 1
+  assert concat_params.shape[-1] == flow_dim
 
-  # phi: Human-Papilloma virus (HPV) prevalence on each population
-  samples_dict['phi'] = samples
+  model_params_nocut = ModelParamsNoCut(phi=concat_params)
 
-  return samples_dict
+  return model_params_nocut
 
 
-def split_flow_theta(
-    samples: Array,
+def split_flow_cut(
+    concat_params: Array,
     theta_dim: int,
-    is_aux: bool,
     **_,
 ) -> Dict[str, Any]:
-  """Get model parameters by splitting samples from the flow."""
-
+  """Get model parameters by splitting samples from the flow.
+  
+  The parameter theta contain the intercept and slope of the
+  prevalence-incidence model.
+  """
   flow_dim = theta_dim
 
-  assert samples.ndim == 2
-  assert samples.shape[-1] == flow_dim
+  assert concat_params.ndim == 1
+  assert concat_params.shape[-1] == flow_dim
+  assert theta_dim == 2
+  theta0, theta1 = jnp.split(concat_params, [1], axis=-1)
+
+  model_params_cut = ModelParamsCut(theta0=theta0, theta1=theta1)
+
+  return model_params_cut
+
 
-  samples_dict = {}
+def concat_flow_nocut(
+    model_params: ModelParamsNoCut,
+    **_,
+) -> Dict[str, Any]:
+  """Concatenate model parameters from ModelParamsNoCut into a single array."""
+  concat_params = model_params[0]
+  assert concat_params.ndim == 1
+  return concat_params
 
-  # theta: Intercept and slope of the prevalence-incidence model
-  samples_dict['theta' + ('_aux' if is_aux else '')] = samples
 
-  return samples_dict
+def concat_flow_cut(
+    model_params: ModelParamsNoCut,
+    **_,
+) -> Dict[str, Any]:
+  """Concatenate model parameters from ModelParamsCut into a single array."""
+  concat_params = jnp.concatenate(model_params, axis=-1)
+  assert concat_params.ndim == 1
+  return concat_params
```

### Comparing `modularbayes-0.1.2/examples/epidemiology/main.py` & `modularbayes-0.1.3/examples/epidemiology/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 
 from absl import app
 from absl import flags
 from absl import logging
 
 import jax
 from ml_collections import config_flags
-import tensorflow as tf
 
-import run_mcmc
+import sample_mcmc
 import train_flow
 import train_vmp_flow
 import train_vmp_map
 
 FLAGS = flags.FLAGS
 
 flags.DEFINE_string('workdir', None, 'Directory to store model data.')
@@ -35,25 +34,20 @@
 
   # log to a file
   if FLAGS.log_dir:
     if not os.path.exists(FLAGS.log_dir):
       os.makedirs(FLAGS.log_dir)
     logging.get_absl_handler().use_absl_log_file()
 
-  # Hide any GPUs form TensorFlow. Otherwise TF might reserve memory and make
-  # it unavailable to JAX.
-  tf.config.experimental.set_visible_devices([], 'GPU')
-  tf.config.experimental.set_visible_devices([], 'TPU')
-
   logging.info('JAX process: %d / %d', jax.process_index(), jax.process_count())
   logging.info('JAX local devices: %r', jax.local_devices())
   logging.info('JAX device count: %r', jax.device_count())
 
   if FLAGS.config.method == 'mcmc':
-    run_mcmc.sample_and_evaluate(FLAGS.config, FLAGS.workdir)
+    sample_mcmc.sample_and_evaluate(FLAGS.config, FLAGS.workdir)
   elif FLAGS.config.method == 'flow':
     train_flow.train_and_evaluate(FLAGS.config, FLAGS.workdir)
   elif FLAGS.config.method == 'vmp_flow':
     train_vmp_flow.train_and_evaluate(FLAGS.config, FLAGS.workdir)
   elif FLAGS.config.method == 'vmp_map':
     train_vmp_map.train_and_evaluate(FLAGS.config, FLAGS.workdir)
```

### Comparing `modularbayes-0.1.2/examples/epidemiology/train_flow.py` & `modularbayes-0.1.3/examples/random_effects/train_vmp_flow.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,549 +1,355 @@
-"""A simple example of a flow model trained on Epidemiology data."""
+"""Training a Variational Meta-Posterior, using the VMP flow."""
+
 import pathlib
 
 from absl import logging
 
 import numpy as np
+
+from arviz import InferenceData
+
 from flax.metrics import tensorboard
 
 import jax
 from jax import numpy as jnp
 
 import haiku as hk
 import optax
 
 import flows
-import log_prob_fun
+from flows import split_flow_nocut, split_flow_cut
+from log_prob_fun import (ModelParams, ModelParamsCut, SmiEta, logprob_joint,
+                          sample_eta_values)
 import plot
-import data
+from train_flow import load_data, make_optimizer, sample_q_as_az
 
+from modularbayes import (sample_q_nocut, sample_q_cutgivennocut,
+                          elbo_smi_vmpflow)
 from modularbayes._src.utils.training import TrainState
 from modularbayes import (flatten_dict, initial_state_ckpt, update_states,
                           save_checkpoint)
-from modularbayes._src.typing import (Any, Array, Batch, ConfigDict, Dict,
-                                      IntLike, List, Optional, PRNGKey,
-                                      Sequence, SmiEta, SummaryWriter, Tuple,
-                                      Union)
+from modularbayes._src.typing import (Any, Array, Callable, ConfigDict, Dict,
+                                      List, Optional, PRNGKey, Tuple)
 
 # Set high precision for matrix multiplication in jax
 jax.config.update('jax_default_matmul_precision', 'float32')
 
 np.set_printoptions(suppress=True, precision=4)
 
 
-def load_dataset() -> Dict[str, Array]:
-  """Load Epidemiology data from Plummer."""
-  dataset_dict = dict(
-      zip(['Z', 'N', 'Y', 'T'],
-          np.split(data.epidemiology.to_numpy(), 4, axis=-1)))
-  dataset_dict = {
-      key: jnp.array(value.squeeze()) for key, value in dataset_dict.items()
-  }
-  return dataset_dict
-
-
-def make_optimizer(
-    lr_schedule_name,
-    lr_schedule_kwargs,
-    grad_clip_value,
-) -> optax.GradientTransformation:
-  """Define optimizer to train the Flow."""
-  schedule = getattr(optax, lr_schedule_name)(**lr_schedule_kwargs)
-
-  optimizer = optax.chain(*[
-      optax.clip_by_global_norm(max_norm=grad_clip_value),
-      optax.adabelief(learning_rate=schedule),
-  ])
-  return optimizer
-
-
-def q_distr_phi(
-    flow_name: str,
-    flow_kwargs: Dict[str, Any],
-    sample_shape: Union[IntLike, Sequence[IntLike]],
-) -> Dict[str, Any]:
-  """Sample from model posterior"""
-
-  q_distr_out = {}
-
-  # Define normalizing flows
-  q_distr = getattr(flows, flow_name + '_phi')(**flow_kwargs)
-
-  # Sample from flows
-  (phi_sample, phi_log_prob_posterior,
-   phi_base_sample) = q_distr.sample_and_log_prob_with_base(
-       seed=hk.next_rng_key(),
-       sample_shape=sample_shape,
-   )
-
-  # Split flow into model parameters
-  q_distr_out['posterior_sample'] = {}
-  q_distr_out['posterior_sample'].update(
-      flows.split_flow_phi(
-          samples=phi_sample,
-          **flow_kwargs,
-      ))
-
-  # sample from base distribution that generated phi
-  q_distr_out['phi_base_sample'] = phi_base_sample
-
-  # log P(phi)
-  q_distr_out['phi_log_prob'] = phi_log_prob_posterior
-
-  return q_distr_out
-
-
-def q_distr_theta(
-    flow_name: str,
-    flow_kwargs: Dict[str, Any],
-    phi_base_sample: Array,
-    is_aux: bool,
-) -> Dict[str, Any]:
-  """Sample from model posterior"""
-
-  q_distr_out = {}
-
-  num_samples = phi_base_sample.shape[0]
-
-  # Define normalizing flows
-  q_distr = getattr(flows, flow_name + '_theta')(**flow_kwargs)
-
-  # Sample from flows
-  (theta_sample, theta_log_prob_posterior) = q_distr.sample_and_log_prob(
-      seed=hk.next_rng_key(),
-      sample_shape=(num_samples,),
-      context=phi_base_sample,
-  )
-
-  # Split flow into model parameters
-  q_distr_out['posterior_sample'] = {}
-  q_distr_out['posterior_sample'].update(
-      flows.split_flow_theta(
-          samples=theta_sample,
-          is_aux=is_aux,
-          **flow_kwargs,
-      ))
-
-  # log P(theta|phi)
-  q_distr_out['theta_' + ('aux_' if is_aux else '') +
-              'log_prob'] = theta_log_prob_posterior
-
-  return q_distr_out
-
-
-def sample_all_flows(
-    params_tuple: Tuple[hk.Params],
-    prng_key: PRNGKey,
-    flow_name: str,
-    flow_kwargs: Dict[str, Any],
-    sample_shape: Union[IntLike, Sequence[IntLike]],
-) -> Dict[str, Any]:
-  """Sample from model posterior"""
-
-  prng_seq = hk.PRNGSequence(prng_key)
-
-  # phi
-  q_distr_out = hk.transform(q_distr_phi).apply(
-      params_tuple[0],
-      next(prng_seq),
-      flow_name=flow_name,
-      flow_kwargs=flow_kwargs,
-      sample_shape=sample_shape,
-  )
-
-  # theta
-  q_distr_out_theta = hk.transform(q_distr_theta).apply(
-      params_tuple[1],
-      next(prng_seq),
-      flow_name=flow_name,
-      flow_kwargs=flow_kwargs,
-      phi_base_sample=q_distr_out['phi_base_sample'],
-      is_aux=False,
-  )
-  q_distr_out['posterior_sample'].update(q_distr_out_theta['posterior_sample'])
-  q_distr_out['theta_log_prob'] = q_distr_out_theta['theta_log_prob']
-
-  if flow_kwargs.is_smi:
-    q_distr_out_theta_aux = hk.transform(q_distr_theta).apply(
-        params_tuple[2],
-        next(prng_seq),
-        flow_name=flow_name,
-        flow_kwargs=flow_kwargs,
-        phi_base_sample=q_distr_out['phi_base_sample'],
-        is_aux=True,
-    )
-    q_distr_out['posterior_sample'].update(
-        q_distr_out_theta_aux['posterior_sample'])
-    q_distr_out['theta_aux_log_prob'] = q_distr_out_theta_aux[
-        'theta_aux_log_prob']
-
-  return q_distr_out
-
-
-def elbo_estimate(
-    params_tuple: Tuple[hk.Params],
-    batch: Batch,
-    prng_key: PRNGKey,
-    num_samples: int,
-    flow_name: str,
-    flow_kwargs: Dict[str, Any],
-    smi_eta: Optional[SmiEta],
-) -> Dict[str, Array]:
-  """Estimate ELBO
-
-  Monte Carlo estimate of ELBO for the two stages of variational SMI.
-  Incorporates the stop_gradient operator for the secong stage.
-  """
-
-  # Sample from flow
-  q_distr_out = sample_all_flows(
-      params_tuple=params_tuple,
-      prng_key=prng_key,
-      flow_name=flow_name,
-      flow_kwargs=flow_kwargs,
-      sample_shape=(num_samples,),
-  )
-
-  is_smi = False if smi_eta is None else True
-
-  shared_params_names = [
-      'phi',
-  ]
-  refit_params_names = [
-      'theta',
-  ]
-
-  # ELBO stage 1: Power posterior
-  if is_smi:
-    posterior_sample_dict_stg1 = {}
-    for key in shared_params_names:
-      posterior_sample_dict_stg1[key] = q_distr_out['posterior_sample'][key]
-    for key in refit_params_names:
-      posterior_sample_dict_stg1[key] = q_distr_out['posterior_sample'][key +
-                                                                        '_aux']
-    log_prob_joint_stg1 = log_prob_fun.log_prob_joint(
-        batch=batch,
-        posterior_sample_dict=posterior_sample_dict_stg1,
-        smi_eta=smi_eta,
-    )
-    log_q_stg1 = (
-        q_distr_out['phi_log_prob'] + q_distr_out['theta_aux_log_prob'])
-
-    elbo_stg1 = log_prob_joint_stg1 - log_q_stg1
-  else:
-    elbo_stg1 = 0.
-
-  # ELBO stage 2: Refit theta
-  posterior_sample_dict_stg2 = {}
-  for key in shared_params_names:
-    if is_smi:
-      posterior_sample_dict_stg2[key] = jax.lax.stop_gradient(
-          q_distr_out['posterior_sample'][key])
-    else:
-      posterior_sample_dict_stg2[key] = q_distr_out['posterior_sample'][key]
-  for key in refit_params_names:
-    posterior_sample_dict_stg2[key] = q_distr_out['posterior_sample'][key]
-  log_prob_joint_stg2 = log_prob_fun.log_prob_joint(
-      batch=batch,
-      posterior_sample_dict=posterior_sample_dict_stg2,
-      smi_eta=None,
-  )
-  if is_smi:
-    log_q_stg2 = (
-        jax.lax.stop_gradient(q_distr_out['phi_log_prob']) +
-        q_distr_out['theta_log_prob'])
-  else:
-    log_q_stg2 = (q_distr_out['phi_log_prob'] + q_distr_out['theta_log_prob'])
-
-  elbo_stg2 = log_prob_joint_stg2 - log_q_stg2
-
-  elbo_dict = {'stage_1': elbo_stg1, 'stage_2': elbo_stg2}
-
-  return elbo_dict
-
-
 def loss(params_tuple: Tuple[hk.Params], *args, **kwargs) -> Array:
   """Define training loss function."""
 
   ### Compute ELBO ###
-  elbo_dict = elbo_estimate(params_tuple=params_tuple, *args, **kwargs)
+  elbo_dict = elbo_smi_vmpflow(lambda_tuple=params_tuple, *args, **kwargs)
 
   # Our loss is the Negative ELBO
   loss_avg = -(jnp.nanmean(elbo_dict['stage_1'] + elbo_dict['stage_2']))
 
   return loss_avg
 
 
 def log_images(
     state_list: List[TrainState],
     prng_key: PRNGKey,
-    flow_name: str,
-    flow_kwargs: Dict[str, Any],
+    config: ConfigDict,
+    dataset: Dict[str, Any],
     num_samples_plot: int,
-    smi_eta: Optional[SmiEta] = None,
-    summary_writer: Optional[SummaryWriter] = None,
+    flow_get_fn_nocut: Callable,
+    flow_get_fn_cutgivennocut: Callable,
+    summary_writer: Optional[tensorboard.SummaryWriter] = None,
     workdir_png: Optional[str] = None,
 ) -> None:
   """Plots to monitor during training."""
 
-  # Sample from flow
-  q_distr_out = sample_all_flows(
-      params_tuple=[state.params for state in state_list],
-      prng_key=prng_key,
-      flow_name=flow_name,
-      flow_kwargs=flow_kwargs,
-      sample_shape=(num_samples_plot,),
-  )
-
-  plot.posterior_samples(
-      posterior_sample_dict=q_distr_out['posterior_sample'],
-      summary_writer=summary_writer,
-      step=state_list[0].step,
-      eta=smi_eta['modules'][0][1],
-      workdir_png=workdir_png,
-  )
-
-
-def compute_elpd(
-    state_list: List[TrainState],
-    batch: Batch,
-    prng_key: PRNGKey,
-    flow_name: str,
-    flow_kwargs: Dict[str, Any],
-    num_samples: int,
-):
-  """Compute ELPD via WAIC"""
-
-  # Sample from flow
-  q_distr_out = sample_all_flows(
-      params_tuple=[state.params for state in state_list],
-      prng_key=prng_key,
-      flow_name=flow_name,
-      flow_kwargs=flow_kwargs,
-      sample_shape=(num_samples,),
-  )
-
-  loglik_pointwise = log_prob_fun.log_lik_vectorised(
-      batch['Z'],
-      batch['Y'],
-      batch['N'],
-      batch['T'],
-      q_distr_out['posterior_sample']['phi'],
-      q_distr_out['posterior_sample']['theta'],
-  )
+  prng_seq = hk.PRNGSequence(prng_key)
 
-  lpd = jax.scipy.special.logsumexp(
-      loglik_pointwise, axis=0) - jnp.log(num_samples)  # colLogMeanExps
-  p_waic = jnp.var(loglik_pointwise, axis=0)
-  elpd_waic = lpd - p_waic
-
-  # posterior_az = az.InferenceData(
-  #     posterior=az.dict_to_dataset({
-  #         k: np.expand_dims(v, axis=0)
-  #         for k, v in posterior_sample_dict.items()
-  #     }),
-  #     log_likelihood=az.dict_to_dataset(
-  #         {'x': np.expand_dims(loglik_pointwise[:, :, 1], axis=0)}),
-  # )
-  # posterior_az.log_likelihood.stack(__sample__=("chain", "draw")).shape
-  # elpd_data = az.loo(data=posterior_az, pointwise=True)
+  assert len(config.smi_eta_plot.keys()) > 0, 'No eta values to plot'
 
-  return elpd_waic
+  # Plot posterior samples
+  for suffix, eta_groups_i in config.smi_eta_plot.items():
+    # Define eta
+    eta_groups_i = jnp.array(eta_groups_i)
+    assert all(eta_groups_i >= 0.0) and all(eta_groups_i <= 1.0), (
+        'eta must be in [0, 1]')
+    smi_etas = SmiEta(
+        groups=jnp.broadcast_to(eta_groups_i,
+                                (num_samples_plot,) + eta_groups_i.shape),)
+    # Sample from flow
+    az_data = sample_q_as_az(
+        lambda_tuple=tuple(x.params for x in state_list),
+        dataset=dataset,
+        prng_key=next(prng_seq),
+        flow_get_fn_nocut=flow_get_fn_nocut,
+        flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+        flow_kwargs=config.flow_kwargs,
+        eta_values=(smi_etas[0] if len(smi_etas) == 1 else jnp.stack(
+            smi_etas, axis=-1)),
+    )
+    plot.posterior_plots(
+        az_data=az_data,
+        show_sigma_trace=False,
+        show_beta_trace=False,
+        show_tau_trace=False,
+        betasigma_pairplot_groups=(0, 1, 2),
+        tausigma_pairplot_groups=(0, 1, 2),
+        suffix=f'_{suffix}',
+        step=state_list[0].step,
+        workdir_png=workdir_png,
+        summary_writer=summary_writer,
+    )
 
 
 def train_and_evaluate(config: ConfigDict, workdir: str) -> TrainState:
   """Execute model training and evaluation loop.
 
   Args:
     config: Hyperparameter configuration for training and evaluation.
     workdir: Directory where the tensorboard summaries are written to.
 
   Returns:
     Final TrainState.
   """
 
+  # Add trailing slash
+  workdir = workdir.rstrip("/") + '/'
+
   # Initialize random keys
   prng_seq = hk.PRNGSequence(config.seed)
 
-  # Full dataset used everytime
-  # Small data, no need to batch
-  train_ds = load_dataset()
-
-  smi_eta = {'modules': [[1.0, config.smi_eta]]}
-
-  phi_dim = train_ds['Z'].shape[0]
-  theta_dim = 2
-
-  # phi_dim and theta_dim are also arguments of the flow,
-  # as they define its dimension
-  config.flow_kwargs.phi_dim = phi_dim
-  config.flow_kwargs.theta_dim = theta_dim
+  # True generative parameters
+  true_params = ModelParams(
+      beta=jnp.array(config.loc_groups),
+      sigma=jnp.array(config.scale_groups),
+      tau=None,
+  )
+
+  # Generate dataset
+  train_ds = load_data(
+      prng_key=next(prng_seq),
+      num_obs_groups=config.num_obs_groups,
+      loc_groups=true_params.beta,
+      scale_groups=true_params.sigma,
+  )
+
+  # num_groups is also a parameter of the flow,
+  # as it define its dimension
+  config.flow_kwargs.num_groups = config.num_groups
   # Also is_smi modifies the dimension of the flow, due to the duplicated params
-  config.flow_kwargs.is_smi = (smi_eta is not None)
+  config.flow_kwargs.is_smi = True
 
   # writer = metric_writers.create_default_writer(
   #     logdir=workdir, just_logging=jax.host_id() != 0)
   if jax.process_index() == 0:
     summary_writer = tensorboard.SummaryWriter(workdir)
     summary_writer.hparams(flatten_dict(config))
   else:
     summary_writer = None
 
-  if smi_eta is not None:
-    smi_eta = {k: jnp.array(v) for k, v in smi_eta.items()}
+  # Functions that generate the NF for no-cut params
+  flow_get_fn_nocut = getattr(flows, 'get_q_nocut_' + config.flow_name)
+  # Functions that generate the NF for cut params (conditional on no-cut params)
+  flow_get_fn_cutgivennocut = getattr(flows,
+                                      'get_q_cutgivennocut_' + config.flow_name)
 
   checkpoint_dir = str(pathlib.Path(workdir) / 'checkpoints')
   state_list = []
   state_name_list = []
 
-  state_name_list.append('phi')
+  state_name_list.append('lambda_nocut')
   state_list.append(
       initial_state_ckpt(
           checkpoint_dir=f'{checkpoint_dir}/{state_name_list[-1]}',
-          forward_fn=hk.transform(q_distr_phi),
+          forward_fn=sample_q_nocut,
           forward_fn_kwargs={
-              'flow_name': config.flow_name,
-              'flow_kwargs': config.flow_kwargs,
-              'sample_shape': (config.num_samples_elbo,)
+              'flow_get_fn':
+                  flow_get_fn_nocut,
+              'flow_kwargs':
+                  config.flow_kwargs,
+              'split_flow_fn':
+                  split_flow_nocut,
+              'eta_values':
+                  jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
           },
           prng_key=next(prng_seq),
           optimizer=make_optimizer(**config.optim_kwargs),
       ))
 
-  # Get an initial sample of phi
-  # (used below to initialize theta)
-  phi_base_sample_init = hk.transform(q_distr_phi).apply(
+  # Get an initial sample of the base distribution of nocut params
+  nocut_base_sample_init = sample_q_nocut.apply(
       state_list[0].params,
       next(prng_seq),
-      flow_name=config.flow_name,
+      flow_get_fn=flow_get_fn_nocut,
       flow_kwargs=config.flow_kwargs,
-      sample_shape=(config.num_samples_elbo,),
-  )['phi_base_sample']
+      split_flow_fn=split_flow_nocut,
+      eta_values=jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
+  )['sample_base']
 
-  state_name_list.append('theta')
+  state_name_list.append('lambda_cut')
   state_list.append(
       initial_state_ckpt(
           checkpoint_dir=f'{checkpoint_dir}/{state_name_list[-1]}',
-          forward_fn=hk.transform(q_distr_theta),
+          forward_fn=sample_q_cutgivennocut,
           forward_fn_kwargs={
-              'flow_name': config.flow_name,
-              'flow_kwargs': config.flow_kwargs,
-              'phi_base_sample': phi_base_sample_init,
-              'is_aux': False,
+              'flow_get_fn':
+                  flow_get_fn_cutgivennocut,
+              'flow_kwargs':
+                  config.flow_kwargs,
+              'split_flow_fn':
+                  split_flow_cut,
+              'nocut_base_sample':
+                  nocut_base_sample_init,
+              'eta_values':
+                  jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
           },
           prng_key=next(prng_seq),
           optimizer=make_optimizer(**config.optim_kwargs),
       ))
   if config.flow_kwargs.is_smi:
-    state_name_list.append('theta_aux')
+    state_name_list.append('lambda_cut_aux')
     state_list.append(
         initial_state_ckpt(
             checkpoint_dir=f'{checkpoint_dir}/{state_name_list[-1]}',
-            forward_fn=hk.transform(q_distr_theta),
+            forward_fn=sample_q_cutgivennocut,
             forward_fn_kwargs={
-                'flow_name': config.flow_name,
-                'flow_kwargs': config.flow_kwargs,
-                'phi_base_sample': phi_base_sample_init,
-                'is_aux': True,
+                'flow_get_fn':
+                    flow_get_fn_cutgivennocut,
+                'flow_kwargs':
+                    config.flow_kwargs,
+                'split_flow_fn':
+                    split_flow_cut,
+                'nocut_base_sample':
+                    nocut_base_sample_init,
+                'eta_values':
+                    jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
             },
             prng_key=next(prng_seq),
             optimizer=make_optimizer(**config.optim_kwargs),
         ))
 
   # Print a useful summary of the execution of the flow architecture.
-  logging.info('FLOW PHI:')
+  logging.info('\nFlow no-cut parameters:\n')
   tabulate_fn_ = hk.experimental.tabulate(
-      f=lambda params, prng_key: hk.transform(q_distr_phi).apply(
+      f=lambda params, prng_key: sample_q_nocut.apply(
           params,
           prng_key,
-          flow_name=config.flow_name,
+          flow_get_fn=flow_get_fn_nocut,
           flow_kwargs=config.flow_kwargs,
-          sample_shape=(config.num_samples_elbo,),
+          split_flow_fn=split_flow_nocut,
+          eta_values=jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
       ),
       columns=(
           "module",
           "owned_params",
           "params_size",
           "params_bytes",
       ),
       filters=("has_params",),
   )
   summary = tabulate_fn_(state_list[0].params, next(prng_seq))
   for line in summary.split("\n"):
     logging.info(line)
 
-  logging.info('FLOW THETA:')
+  logging.info('\nFlow cut parameters:\n')
   tabulate_fn_ = hk.experimental.tabulate(
-      f=lambda params, prng_key: hk.transform(q_distr_theta).apply(
+      f=lambda params, prng_key: sample_q_cutgivennocut.apply(
           params,
           prng_key,
-          flow_name=config.flow_name,
+          flow_get_fn=flow_get_fn_cutgivennocut,
           flow_kwargs=config.flow_kwargs,
-          phi_base_sample=phi_base_sample_init,
-          is_aux=False,
+          split_flow_fn=split_flow_cut,
+          nocut_base_sample=nocut_base_sample_init,
+          eta_values=jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
       ),
       columns=(
           "module",
           "owned_params",
           "params_size",
           "params_bytes",
       ),
       filters=("has_params",),
   )
   summary = tabulate_fn_(state_list[1].params, next(prng_seq))
   for line in summary.split("\n"):
     logging.info(line)
 
   # Jit function to update training states
-  update_states_jit = lambda state_list, batch, prng_key, smi_eta: update_states(
-      state_list=state_list,
-      batch=batch,
-      prng_key=prng_key,
-      optimizer=make_optimizer(**config.optim_kwargs),
-      loss_fn=loss,
-      loss_fn_kwargs={
-          'num_samples': config.num_samples_elbo,
-          'flow_name': config.flow_name,
-          'flow_kwargs': config.flow_kwargs,
-          'smi_eta': smi_eta,
-      },
-  )
-  update_states_jit = jax.jit(update_states_jit)
+  @jax.jit
+  def update_states_jit(state_list, batch, prng_key):
+    return update_states(
+        state_list=state_list,
+        batch=batch,
+        prng_key=prng_key,
+        optimizer=make_optimizer(**config.optim_kwargs),
+        loss_fn=loss,
+        loss_fn_kwargs={
+            'num_samples': config.num_samples_elbo,
+            'logprob_joint_fn': logprob_joint,
+            'flow_get_fn_nocut': flow_get_fn_nocut,
+            'flow_get_fn_cutgivennocut': flow_get_fn_cutgivennocut,
+            'flow_kwargs': config.flow_kwargs,
+            'prior_hparams': config.prior_hparams,
+            'model_params_tupleclass': ModelParams,
+            'model_params_cut_tupleclass': ModelParamsCut,
+            'split_flow_fn_nocut': split_flow_nocut,
+            'split_flow_fn_cut': split_flow_cut,
+            'sample_eta_fn': sample_eta_values,
+            'sample_eta_kwargs': {
+                'num_groups': config.num_groups,
+                'eta_sampling_a': 1.,
+                'eta_sampling_b': 1.
+            },
+        },
+    )
 
-  elbo_validation_jit = lambda state_list, batch, prng_key, smi_eta: elbo_estimate(
-      params_tuple=[state.params for state in state_list],
-      batch=batch,
-      prng_key=prng_key,
-      num_samples=config.num_samples_eval,
-      flow_name=config.flow_name,
-      flow_kwargs=config.flow_kwargs,
-      smi_eta=smi_eta,
-  )
-  elbo_validation_jit = jax.jit(elbo_validation_jit)
+  @jax.jit
+  def elbo_validation_jit(state_list, batch, prng_key):
+    return elbo_smi_vmpflow(
+        lambda_tuple=tuple(state.params for state in state_list),
+        batch=batch,
+        prng_key=prng_key,
+        num_samples=config.num_samples_eval,
+        logprob_joint_fn=logprob_joint,
+        flow_get_fn_nocut=flow_get_fn_nocut,
+        flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+        flow_kwargs=config.flow_kwargs,
+        prior_hparams=config.prior_hparams,
+        model_params_tupleclass=ModelParams,
+        model_params_cut_tupleclass=ModelParamsCut,
+        split_flow_fn_nocut=split_flow_nocut,
+        split_flow_fn_cut=split_flow_cut,
+        sample_eta_fn=sample_eta_values,
+        sample_eta_kwargs={
+            'num_groups': config.num_groups,
+            'eta_sampling_a': 1.,
+            'eta_sampling_b': 1.
+        },
+    )
 
   if state_list[0].step < config.training_steps:
-    logging.info('Training variational posterior...')
+    logging.info('Training Variational Meta-Posterior (VMP-flow)...')
 
   # Reset random key sequence
   prng_seq = hk.PRNGSequence(config.seed)
 
   while state_list[0].step < config.training_steps:
 
     # Plots to monitor training
     if ((state_list[0].step == 0) or
         (state_list[0].step % config.log_img_steps == 0)):
       # print("Logging images...\n")
       log_images(
           state_list=state_list,
           prng_key=next(prng_seq),
-          flow_name=config.flow_name,
-          flow_kwargs=config.flow_kwargs,
+          config=config,
+          dataset=train_ds,
           num_samples_plot=config.num_samples_plot,
-          smi_eta=smi_eta,
+          flow_get_fn_nocut=flow_get_fn_nocut,
+          flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
           summary_writer=summary_writer,
           workdir_png=workdir,
       )
 
     # Log learning rate
     summary_writer.scalar(
         tag='learning_rate',
@@ -553,15 +359,14 @@
     )
 
     # SGD step
     state_list, metrics = update_states_jit(
         state_list=state_list,
         batch=train_ds,
         prng_key=next(prng_seq),
-        smi_eta=smi_eta,
     )
     # The computed training loss corresponds to the model before update
     summary_writer.scalar(
         tag='train_loss',
         value=metrics['train_loss'],
         step=state_list[0].step - 1,
     )
@@ -575,15 +380,14 @@
       logging.info("STEP: %5d; training loss: %.3f", state_list[0].step - 1,
                    metrics["train_loss"])
 
       elbo_dict = elbo_validation_jit(
           state_list=state_list,
           batch=train_ds,
           prng_key=next(prng_seq),
-          smi_eta=smi_eta,
       )
       for k, v in elbo_dict.items():
         summary_writer.scalar(
             tag=f'elbo_{k}',
             value=v.mean(),
             step=state_list[0].step,
         )
@@ -610,23 +414,24 @@
         keep=config.checkpoints_keep,
     )
 
   # Last plot of posteriors
   log_images(
       state_list=state_list,
       prng_key=next(prng_seq),
-      flow_name=config.flow_name,
-      flow_kwargs=config.flow_kwargs,
+      config=config,
+      dataset=train_ds,
       num_samples_plot=config.num_samples_plot,
-      smi_eta=smi_eta,
+      flow_get_fn_nocut=flow_get_fn_nocut,
+      flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
       summary_writer=summary_writer,
       workdir_png=workdir,
   )
 
   return state_list
 
 
 # # For debugging
 # config = get_config()
-# config.flow_kwargs.smi_eta = {'modules': [[1.0, 1.0]]}
-# workdir = pathlib.Path.home()/'smi/output/epidemiology/mean_field/eta_1.0'
-# train_and_evaluate(config, workdir)
+# import pathlib
+# workdir = str(pathlib.Path.home() / f'modularbayes-output-exp/random_effects/nsf/vmp_flow')
+# # train_and_evaluate(config, workdir)
```

### Comparing `modularbayes-0.1.2/examples/epidemiology/train_vmp_flow.py` & `modularbayes-0.1.3/examples/random_effects/train_flow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,509 +1,381 @@
-"""A simple example of a flow model trained on Epidemiology data."""
+"""Training a Normalizing Flow."""
 import pathlib
 
 from absl import logging
 
 import numpy as np
 
+from arviz import InferenceData
+
 from flax.metrics import tensorboard
 
 import jax
 from jax import numpy as jnp
 
 import haiku as hk
 import optax
+import distrax
 
 import flows
-import log_prob_fun
+from flows import split_flow_nocut, split_flow_cut
+from log_prob_fun import ModelParams, ModelParamsCut, SmiEta, logprob_joint
 import plot
-from train_flow import load_dataset, make_optimizer
 
+from modularbayes import (sample_q_nocut, sample_q_cutgivennocut, sample_q,
+                          elbo_smi)
 from modularbayes._src.utils.training import TrainState
 from modularbayes import (flatten_dict, initial_state_ckpt, update_states,
                           save_checkpoint)
-from modularbayes._src.typing import (Any, Array, Batch, ConfigDict, Dict, List,
-                                      Optional, PRNGKey, SmiEta, SummaryWriter,
-                                      Tuple)
+from modularbayes._src.typing import (Any, Array, Callable, ConfigDict, Dict,
+                                      List, Optional, PRNGKey, Tuple)
 
 # Set high precision for matrix multiplication in jax
 jax.config.update('jax_default_matmul_precision', 'float32')
 
 np.set_printoptions(suppress=True, precision=4)
 
 
-def q_distr_phi(
-    flow_name: str,
-    flow_kwargs: Dict[str, Any],
-    eta: Array,
-) -> Dict[str, Any]:
-  """Sample from model posterior"""
-
-  q_distr_out = {}
-
-  # Define normalizing flows
-  q_distr = getattr(flows, flow_name + '_phi')(**flow_kwargs)
-
-  num_samples = eta.shape[0]
-
-  # Sample from flows
-  (phi_sample, phi_log_prob_posterior,
-   phi_base_sample) = q_distr.sample_and_log_prob_with_base(
-       seed=hk.next_rng_key(),
-       sample_shape=(num_samples,),
-       context=[eta, None],
-   )
-
-  # Split flow into model parameters
-  q_distr_out['posterior_sample'] = {}
-  q_distr_out['posterior_sample'].update(
-      flows.split_flow_phi(
-          samples=phi_sample,
-          **flow_kwargs,
-      ))
-
-  # sample from base distribution that generated phi
-  q_distr_out['phi_base_sample'] = phi_base_sample
-
-  # log P(phi)
-  q_distr_out['phi_log_prob'] = phi_log_prob_posterior
-
-  return q_distr_out
-
-
-def q_distr_theta(
-    flow_name: str,
-    flow_kwargs: Dict[str, Any],
-    phi_base_sample: Array,
-    eta: Array,
-    is_aux: bool,
-) -> Dict[str, Any]:
-  """Sample from model posterior"""
-
-  q_distr_out = {}
-
-  num_samples = phi_base_sample.shape[0]
-
-  # Define normalizing flows
-  q_distr = getattr(flows, flow_name + '_theta')(**flow_kwargs)
-
-  # Sample from flow
-  (theta_sample, theta_log_prob_posterior) = q_distr.sample_and_log_prob(
-      seed=hk.next_rng_key(),
-      sample_shape=(num_samples,),
-      context=[eta, phi_base_sample],
-  )
-
-  # Split flow into model parameters
-  q_distr_out['posterior_sample'] = {}
-  q_distr_out['posterior_sample'].update(
-      flows.split_flow_theta(
-          samples=theta_sample,
-          is_aux=is_aux,
-          **flow_kwargs,
-      ))
-
-  # log P(theta|phi)
-  q_distr_out['theta_' + ('aux_' if is_aux else '') +
-              'log_prob'] = theta_log_prob_posterior
-
-  return q_distr_out
-
-
-def sample_all_flows(
-    params_tuple: Tuple[hk.Params],
+def load_data(
     prng_key: PRNGKey,
-    flow_name: str,
-    flow_kwargs: Dict[str, Any],
-    smi_eta: SmiEta,
-) -> Dict[str, Any]:
-  """Sample from model posterior"""
-
-  prng_seq = hk.PRNGSequence(prng_key)
-
-  # phi
-  q_distr_out = hk.transform(q_distr_phi).apply(
-      params_tuple[0],
-      next(prng_seq),
-      flow_name=flow_name,
-      flow_kwargs=flow_kwargs,
-      eta=smi_eta['modules'],
-  )
-
-  # theta
-  q_distr_out_theta = hk.transform(q_distr_theta).apply(
-      params_tuple[1],
-      next(prng_seq),
-      flow_name=flow_name,
-      flow_kwargs=flow_kwargs,
-      phi_base_sample=q_distr_out['phi_base_sample'],
-      eta=smi_eta['modules'],
-      is_aux=False,
-  )
-  q_distr_out['posterior_sample'].update(q_distr_out_theta['posterior_sample'])
-  q_distr_out['theta_log_prob'] = q_distr_out_theta['theta_log_prob']
-
-  q_distr_out_theta_aux = hk.transform(q_distr_theta).apply(
-      params_tuple[2],
-      next(prng_seq),
-      flow_name=flow_name,
-      flow_kwargs=flow_kwargs,
-      phi_base_sample=q_distr_out['phi_base_sample'],
-      eta=smi_eta['modules'],
-      is_aux=True,
-  )
-  q_distr_out['posterior_sample'].update(
-      q_distr_out_theta_aux['posterior_sample'])
-  q_distr_out['theta_aux_log_prob'] = q_distr_out_theta_aux[
-      'theta_aux_log_prob']
-
-  return q_distr_out
-
-
-def elbo_estimate_along_eta(
-    params_tuple: Tuple[hk.Params],
-    batch: Batch,
-    prng_key: PRNGKey,
-    num_samples: int,
-    flow_name: str,
-    flow_kwargs: Dict[str, Any],
-    eta_sampling_a: float,
-    eta_sampling_b: float,
+    num_obs_groups: Array,
+    loc_groups: Array,
+    scale_groups: Array,
 ) -> Dict[str, Array]:
-  """Estimate ELBO
-
-  Monte Carlo estimate of ELBO for the two stages of variational SMI.
-  Incorporates the stop_gradient operator for the secong stage.
-  """
-
-  prng_seq = hk.PRNGSequence(prng_key)
-
-  # Sample eta values (only for Y module)
-  etas_elbo = jax.random.beta(
-      key=next(prng_seq),
-      a=eta_sampling_a,
-      b=eta_sampling_b,
-      shape=(num_samples, 1),
-  )
-  # Set eta_z=1
-  etas_elbo = jnp.concatenate([jnp.ones_like(etas_elbo), etas_elbo], axis=-1)
-  smi_eta_elbo = {'modules': etas_elbo}
+  """Generate random effects data as in Liu 2009."""
 
-  # Sample from flow
-  q_distr_out = sample_all_flows(
-      params_tuple=params_tuple,
-      prng_key=next(prng_seq),
-      flow_name=flow_name,
-      flow_kwargs=flow_kwargs,
-      smi_eta=smi_eta_elbo,
-  )
-
-  shared_params_names = [
-      'phi',
-  ]
-  refit_params_names = [
-      'theta',
-  ]
-
-  # ELBO stage 1: Power posterior
-  posterior_sample_dict_stg1 = {}
-  for key in shared_params_names:
-    posterior_sample_dict_stg1[key] = q_distr_out['posterior_sample'][key]
-  for key in refit_params_names:
-    posterior_sample_dict_stg1[key] = q_distr_out['posterior_sample'][key +
-                                                                      '_aux']
-
-  log_prob_joint_stg1 = jax.vmap(
-      lambda posterior_sample_i, smi_eta_i: log_prob_fun.log_prob_joint(
-          batch=batch,
-          posterior_sample_dict=posterior_sample_i,
-          smi_eta=smi_eta_i,
-      ))(
-          jax.tree_map(lambda x: jnp.expand_dims(x, 1),
-                       posterior_sample_dict_stg1),
-          smi_eta_elbo,
-      )
-
-  log_q_stg1 = q_distr_out['phi_log_prob'] + q_distr_out['theta_aux_log_prob']
-
-  #TODO: check reshape
-  elbo_stg1 = log_prob_joint_stg1.reshape(-1) - log_q_stg1
-
-  # ELBO stage 2: Refit theta
-  posterior_sample_dict_stg2 = {}
-  for key in shared_params_names:
-    posterior_sample_dict_stg2[key] = jax.lax.stop_gradient(
-        q_distr_out['posterior_sample'][key])
-  for key in refit_params_names:
-    posterior_sample_dict_stg2[key] = q_distr_out['posterior_sample'][key]
-
-  log_prob_joint_stg2 = jax.vmap(
-      lambda posterior_sample_i: log_prob_fun.log_prob_joint(
-          batch=batch,
-          posterior_sample_dict=posterior_sample_i,
-          smi_eta=None,
-      ))(
-          jax.tree_map(lambda x: jnp.expand_dims(x, 1),
-                       posterior_sample_dict_stg2))
-
-  log_q_stg2 = (
-      jax.lax.stop_gradient(q_distr_out['phi_log_prob']) +
-      q_distr_out['theta_log_prob'])
-
-  # TODO: check reshape
-  elbo_stg2 = log_prob_joint_stg2.reshape(-1) - log_q_stg2
-
-  elbo_dict = {'stage_1': elbo_stg1, 'stage_2': elbo_stg2}
-
-  return elbo_dict
+  num_groups = len(num_obs_groups)
+  assert len(loc_groups) == num_groups
+  assert len(scale_groups) == num_groups
+
+  num_obs_groups = jnp.array(num_obs_groups).astype(int)
+  loc_groups = jnp.array(loc_groups)
+  scale_groups = jnp.array(scale_groups)
+
+  loc_pointwise = jnp.repeat(loc_groups, num_obs_groups)
+  scale_pointwise = jnp.repeat(scale_groups, num_obs_groups)
+
+  z = jax.random.normal(key=prng_key, shape=loc_pointwise.shape)
+
+  dataset_dict = {
+      'Y': loc_pointwise + z * scale_pointwise,
+      'group': jnp.repeat(jnp.arange(num_groups), num_obs_groups),
+      'num_obs_groups': num_obs_groups,
+  }
+
+  return dataset_dict
+
+
+def make_optimizer(
+    lr_schedule_name,
+    lr_schedule_kwargs,
+    grad_clip_value,
+) -> optax.GradientTransformation:
+  """Define optimizer to train the Flow."""
+  schedule = getattr(optax, lr_schedule_name)(**lr_schedule_kwargs)
+
+  optimizer = optax.chain(*[
+      optax.clip_by_global_norm(max_norm=grad_clip_value),
+      optax.adabelief(learning_rate=schedule),
+  ])
+  return optimizer
 
 
 def loss(params_tuple: Tuple[hk.Params], *args, **kwargs) -> Array:
   """Define training loss function."""
 
   ### Compute ELBO ###
-  elbo_dict = elbo_estimate_along_eta(
-      params_tuple=params_tuple, *args, **kwargs)
+  elbo_dict = elbo_smi(lambda_tuple=params_tuple, *args, **kwargs)
 
   # Our loss is the Negative ELBO
   loss_avg = -(jnp.nanmean(elbo_dict['stage_1'] + elbo_dict['stage_2']))
 
   return loss_avg
 
 
-def log_images(
-    state_list: List[TrainState],
+def sample_q_as_az(
+    lambda_tuple: Tuple[hk.Params],
+    dataset: Dict[str, Any],
     prng_key: PRNGKey,
-    config: ConfigDict,
-    num_samples_plot: int,
-    summary_writer: Optional[SummaryWriter] = None,
-    workdir_png: Optional[str] = None,
-) -> None:
+    flow_get_fn_nocut: Callable,
+    flow_get_fn_cutgivennocut: Callable,
+    flow_kwargs: Dict[str, Any],
+    sample_shape: Optional[Tuple[int]] = None,
+    eta_values: Optional[Array] = None,
+) -> InferenceData:
   """Plots to monitor during training."""
-
-  prng_seq = hk.PRNGSequence(prng_key)
-
-  eta_plot = jnp.array(config.eta_plot)
-
-  assert eta_plot.ndim == 2
-
-  # Plot posterior samples
-  key_flow = next(prng_seq)
-  for i in range(eta_plot.shape[0]):
-    # Sample from flow
-    q_distr_out = sample_all_flows(
-        params_tuple=[state.params for state in state_list],
-        prng_key=key_flow,
-        flow_name=config.flow_name,
-        flow_kwargs=config.flow_kwargs,
-        smi_eta={
-            'modules':
-                jnp.broadcast_to(eta_plot[[i], :],
-                                 (num_samples_plot,) + eta_plot.shape[1:])
-        },
-    )
-
-    plot.posterior_samples(
-        posterior_sample_dict=q_distr_out['posterior_sample'],
-        summary_writer=summary_writer,
-        step=state_list[0].step,
-        eta=eta_plot[i][1],
-        workdir_png=workdir_png,
-    )
+  assert sample_shape is not None or eta_values is not None, (
+      'Either sample_shape or eta_values must be provided.')
+  assert sample_shape is None or eta_values is None, (
+      'Only one of sample_shape or eta_values must be provided.')
+  # Sample from flow
+  q_distr_out = sample_q(
+      lambda_tuple=lambda_tuple,
+      prng_key=prng_key,
+      flow_get_fn_nocut=flow_get_fn_nocut,
+      flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+      flow_kwargs=flow_kwargs,
+      model_params_tupleclass=ModelParams,
+      split_flow_fn_nocut=split_flow_nocut,
+      split_flow_fn_cut=split_flow_cut,
+      sample_shape=sample_shape,
+      eta_values=eta_values,
+  )
+  # Add dimension for "chains"
+  model_params_az = jax.tree_map(lambda x: x[None, ...],
+                                 q_distr_out['model_params_sample'])
+  # Create InferenceData object
+  az_data = plot.arviz_from_samples(
+      dataset=dataset,
+      model_params=model_params_az,
+  )
+  return az_data
 
 
 def train_and_evaluate(config: ConfigDict, workdir: str) -> TrainState:
   """Execute model training and evaluation loop.
 
   Args:
     config: Hyperparameter configuration for training and evaluation.
     workdir: Directory where the tensorboard summaries are written to.
 
   Returns:
     Final TrainState.
   """
 
+  # Add trailing slash
+  workdir = workdir.rstrip("/") + '/'
+
   # Initialize random keys
   prng_seq = hk.PRNGSequence(config.seed)
 
-  # Full dataset used everytime
-  # Small data, no need to batch
-  train_ds = load_dataset()
-
-  phi_dim = train_ds['Z'].shape[0]
-  theta_dim = 2
-
-  # phi_dim and theta_dim are also arguments of the flow,
-  # as they define its dimension
-  config.flow_kwargs.phi_dim = phi_dim
-  config.flow_kwargs.theta_dim = theta_dim
+  # True generative parameters
+  true_params = ModelParams(
+      beta=jnp.array(config.loc_groups),
+      sigma=jnp.array(config.scale_groups),
+      tau=None,
+  )
+
+  # Generate dataset
+  train_ds = load_data(
+      prng_key=next(prng_seq),
+      num_obs_groups=config.num_obs_groups,
+      loc_groups=true_params.beta,
+      scale_groups=true_params.sigma,
+  )
+
+  # Generate new observations from the true generative model
+  y_new = distrax.Normal(
+      loc=true_params.beta[train_ds['group']],
+      scale=true_params.sigma[train_ds['group']],
+  ).sample(
+      seed=next(prng_seq), sample_shape=(config.num_samples_eval,))
+
+  # Set eta for modules
+  smi_eta = SmiEta(groups=jnp.array(config.smi_eta_groups))
+
+  # num_groups is also a parameter of the flow,
+  # as it define its dimension
+  config.flow_kwargs.num_groups = config.num_groups
   # Also is_smi modifies the dimension of the flow, due to the duplicated params
-  config.flow_kwargs.is_smi = True
+  config.flow_kwargs.is_smi = (smi_eta is not None)
 
   # writer = metric_writers.create_default_writer(
   #     logdir=workdir, just_logging=jax.host_id() != 0)
   if jax.process_index() == 0:
     summary_writer = tensorboard.SummaryWriter(workdir)
     summary_writer.hparams(flatten_dict(config))
   else:
     summary_writer = None
 
+  # Functions that generate the NF for no-cut params
+  flow_get_fn_nocut = getattr(flows, 'get_q_nocut_' + config.flow_name)
+  # Functions that generate the NF for cut params (conditional on no-cut params)
+  flow_get_fn_cutgivennocut = getattr(flows,
+                                      'get_q_cutgivennocut_' + config.flow_name)
+
   checkpoint_dir = str(pathlib.Path(workdir) / 'checkpoints')
   state_list = []
   state_name_list = []
 
-  state_name_list.append('phi')
+  state_name_list.append('lambda_nocut')
   state_list.append(
       initial_state_ckpt(
           checkpoint_dir=f'{checkpoint_dir}/{state_name_list[-1]}',
-          forward_fn=hk.transform(q_distr_phi),
+          forward_fn=sample_q_nocut,
           forward_fn_kwargs={
-              'flow_name': config.flow_name,
+              'flow_get_fn': flow_get_fn_nocut,
               'flow_kwargs': config.flow_kwargs,
-              'eta': jnp.ones((config.num_samples_elbo, 2)),
+              'split_flow_fn': split_flow_nocut,
+              'sample_shape': (config.num_samples_elbo,),
           },
           prng_key=next(prng_seq),
           optimizer=make_optimizer(**config.optim_kwargs),
       ))
 
-  # Get an initial sample of phi
-  # (used below to initialize theta)
-  phi_base_sample_init = hk.transform(q_distr_phi).apply(
+  # Get an initial sample of the base distribution of nocut params
+  nocut_base_sample_init = sample_q_nocut.apply(
       state_list[0].params,
       next(prng_seq),
-      flow_name=config.flow_name,
+      flow_get_fn=flow_get_fn_nocut,
       flow_kwargs=config.flow_kwargs,
-      eta=jnp.ones((config.num_samples_elbo, 2)),
-  )['phi_base_sample']
+      split_flow_fn=split_flow_nocut,
+      sample_shape=(config.num_samples_elbo,),
+  )['sample_base']
 
-  state_name_list.append('theta')
+  state_name_list.append('lambda_cut')
   state_list.append(
       initial_state_ckpt(
           checkpoint_dir=f'{checkpoint_dir}/{state_name_list[-1]}',
-          forward_fn=hk.transform(q_distr_theta),
+          forward_fn=sample_q_cutgivennocut,
           forward_fn_kwargs={
-              'flow_name': config.flow_name,
+              'flow_get_fn': flow_get_fn_cutgivennocut,
               'flow_kwargs': config.flow_kwargs,
-              'phi_base_sample': phi_base_sample_init,
-              'eta': jnp.ones((config.num_samples_elbo, 2)),
-              'is_aux': False,
+              'split_flow_fn': split_flow_cut,
+              'nocut_base_sample': nocut_base_sample_init,
           },
           prng_key=next(prng_seq),
           optimizer=make_optimizer(**config.optim_kwargs),
       ))
   if config.flow_kwargs.is_smi:
-    state_name_list.append('theta_aux')
+    state_name_list.append('lambda_cut_aux')
     state_list.append(
         initial_state_ckpt(
             checkpoint_dir=f'{checkpoint_dir}/{state_name_list[-1]}',
-            forward_fn=hk.transform(q_distr_theta),
+            forward_fn=sample_q_cutgivennocut,
             forward_fn_kwargs={
-                'flow_name': config.flow_name,
+                'flow_get_fn': flow_get_fn_cutgivennocut,
                 'flow_kwargs': config.flow_kwargs,
-                'phi_base_sample': phi_base_sample_init,
-                'eta': jnp.ones((config.num_samples_elbo, 2)),
-                'is_aux': True,
+                'split_flow_fn': split_flow_cut,
+                'nocut_base_sample': nocut_base_sample_init,
             },
             prng_key=next(prng_seq),
             optimizer=make_optimizer(**config.optim_kwargs),
         ))
 
   # Print a useful summary of the execution of the flow architecture.
-  logging.info('FLOW PHI:')
+  logging.info('\nFlow no-cut parameters:\n')
   tabulate_fn_ = hk.experimental.tabulate(
-      f=lambda params, prng_key: hk.transform(q_distr_phi).apply(
+      f=lambda params, prng_key: sample_q_nocut.apply(
           params,
           prng_key,
-          flow_name=config.flow_name,
+          flow_get_fn=flow_get_fn_nocut,
           flow_kwargs=config.flow_kwargs,
-          eta=jnp.ones((config.num_samples_elbo, 2)),
+          split_flow_fn=split_flow_nocut,
+          sample_shape=(config.num_samples_elbo,),
       ),
       columns=(
           "module",
           "owned_params",
           "params_size",
           "params_bytes",
       ),
       filters=("has_params",),
   )
   summary = tabulate_fn_(state_list[0].params, next(prng_seq))
   for line in summary.split("\n"):
     logging.info(line)
 
-  logging.info('FLOW THETA:')
+  logging.info('\nFlow cut parameters:\n')
   tabulate_fn_ = hk.experimental.tabulate(
-      f=lambda params, prng_key: hk.transform(q_distr_theta).apply(
+      f=lambda params, prng_key: sample_q_cutgivennocut.apply(
           params,
           prng_key,
-          flow_name=config.flow_name,
+          flow_get_fn=flow_get_fn_cutgivennocut,
           flow_kwargs=config.flow_kwargs,
-          phi_base_sample=phi_base_sample_init,
-          eta=jnp.ones((config.num_samples_elbo, 2)),
-          is_aux=False,
+          split_flow_fn=split_flow_cut,
+          nocut_base_sample=nocut_base_sample_init,
       ),
       columns=(
           "module",
           "owned_params",
           "params_size",
           "params_bytes",
       ),
       filters=("has_params",),
   )
   summary = tabulate_fn_(state_list[1].params, next(prng_seq))
   for line in summary.split("\n"):
     logging.info(line)
 
   # Jit function to update training states
-  update_states_jit = lambda state_list, batch, prng_key: update_states(
-      state_list=state_list,
-      batch=batch,
-      prng_key=prng_key,
-      optimizer=make_optimizer(**config.optim_kwargs),
-      loss_fn=loss,
-      loss_fn_kwargs={
-          'num_samples': config.num_samples_elbo,
-          'flow_name': config.flow_name,
-          'flow_kwargs': config.flow_kwargs,
-          'eta_sampling_a': config.eta_sampling_a,
-          'eta_sampling_b': config.eta_sampling_b,
-      },
-  )
-  update_states_jit = jax.jit(update_states_jit)
+  @jax.jit
+  def update_states_jit(state_list, batch, prng_key, smi_eta):
+    return update_states(
+        state_list=state_list,
+        batch=batch,
+        prng_key=prng_key,
+        optimizer=make_optimizer(**config.optim_kwargs),
+        loss_fn=loss,
+        loss_fn_kwargs={
+            'num_samples': config.num_samples_elbo,
+            'logprob_joint_fn': logprob_joint,
+            'flow_get_fn_nocut': flow_get_fn_nocut,
+            'flow_get_fn_cutgivennocut': flow_get_fn_cutgivennocut,
+            'flow_kwargs': config.flow_kwargs,
+            'prior_hparams': config.prior_hparams,
+            'model_params_tupleclass': ModelParams,
+            'model_params_cut_tupleclass': ModelParamsCut,
+            'split_flow_fn_nocut': split_flow_nocut,
+            'split_flow_fn_cut': split_flow_cut,
+            'smi_eta': smi_eta,
+        },
+    )
 
-  elbo_validation_jit = lambda state_list, batch, prng_key: elbo_estimate_along_eta(
-      params_tuple=tuple(state.params for state in state_list),
-      batch=batch,
-      prng_key=prng_key,
-      num_samples=config.num_samples_eval,
-      flow_name=config.flow_name,
-      flow_kwargs=config.flow_kwargs,
-      eta_sampling_a=1.,
-      eta_sampling_b=1.,
-  )
-  elbo_validation_jit = jax.jit(elbo_validation_jit)
+  @jax.jit
+  def elbo_validation_jit(state_list, batch, prng_key, smi_eta):
+    return elbo_smi(
+        lambda_tuple=tuple(state.params for state in state_list),
+        batch=batch,
+        prng_key=prng_key,
+        num_samples=config.num_samples_eval,
+        logprob_joint_fn=logprob_joint,
+        flow_get_fn_nocut=flow_get_fn_nocut,
+        flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+        flow_kwargs=config.flow_kwargs,
+        prior_hparams=config.prior_hparams,
+        model_params_tupleclass=ModelParams,
+        model_params_cut_tupleclass=ModelParamsCut,
+        split_flow_fn_nocut=split_flow_nocut,
+        split_flow_fn_cut=split_flow_cut,
+        smi_eta=smi_eta,
+    )
 
   if state_list[0].step < config.training_steps:
-    logging.info('Training Variational Meta-Posterior (VMP-flow)...')
+    logging.info('Training variational posterior...')
 
   # Reset random key sequence
   prng_seq = hk.PRNGSequence(config.seed)
 
   while state_list[0].step < config.training_steps:
 
     # Plots to monitor training
     if ((state_list[0].step == 0) or
         (state_list[0].step % config.log_img_steps == 0)):
       # print("Logging images...\n")
-      log_images(
-          state_list=state_list,
+      az_data = sample_q_as_az(
+          lambda_tuple=tuple(x.params for x in state_list),
+          dataset=train_ds,
           prng_key=next(prng_seq),
-          config=config,
-          num_samples_plot=config.num_samples_plot,
-          summary_writer=summary_writer,
+          flow_get_fn_nocut=flow_get_fn_nocut,
+          flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+          flow_kwargs=config.flow_kwargs,
+          sample_shape=(config.num_samples_plot,),
+      )
+      plot.posterior_plots(
+          az_data=az_data,
+          show_sigma_trace=False,
+          show_beta_trace=False,
+          show_tau_trace=False,
+          betasigma_pairplot_groups=(0, 1, 2),
+          tausigma_pairplot_groups=(0, 1, 2),
+          suffix=config.plot_suffix,
+          step=state_list[0].step,
           workdir_png=workdir,
+          summary_writer=summary_writer,
       )
 
     # Log learning rate
     summary_writer.scalar(
         tag='learning_rate',
         value=getattr(optax, config.optim_kwargs.lr_schedule_name)(
             **config.optim_kwargs.lr_schedule_kwargs)(state_list[0].step),
@@ -511,38 +383,39 @@
     )
 
     # SGD step
     state_list, metrics = update_states_jit(
         state_list=state_list,
         batch=train_ds,
         prng_key=next(prng_seq),
+        smi_eta=smi_eta,
     )
     # The computed training loss corresponds to the model before update
     summary_writer.scalar(
         tag='train_loss',
         value=metrics['train_loss'],
         step=state_list[0].step - 1,
     )
 
     if state_list[0].step == 1:
       logging.info("STEP: %5d; training loss: %.3f", state_list[0].step - 1,
                    metrics["train_loss"])
 
     # Metrics for evaluation
     if state_list[0].step % config.eval_steps == 0:
-
       logging.info("STEP: %5d; training loss: %.3f", state_list[0].step - 1,
                    metrics["train_loss"])
 
-      elbo_validation_dict = elbo_validation_jit(
+      elbo_dict = elbo_validation_jit(
           state_list=state_list,
           batch=train_ds,
           prng_key=next(prng_seq),
+          smi_eta=smi_eta,
       )
-      for k, v in elbo_validation_dict.items():
+      for k, v in elbo_dict.items():
         summary_writer.scalar(
             tag=f'elbo_{k}',
             value=v.mean(),
             step=state_list[0].step,
         )
 
     if state_list[0].step % config.checkpoint_steps == 0:
@@ -564,17 +437,37 @@
     save_checkpoint(
         state=state_i,
         checkpoint_dir=f'{checkpoint_dir}/{state_name_i}',
         keep=config.checkpoints_keep,
     )
 
   # Last plot of posteriors
-  log_images(
-      state_list=state_list,
+  az_data = sample_q_as_az(
+      lambda_tuple=tuple(x.params for x in state_list),
+      dataset=train_ds,
       prng_key=next(prng_seq),
-      config=config,
-      num_samples_plot=config.num_samples_plot,
-      summary_writer=summary_writer,
+      flow_get_fn_nocut=flow_get_fn_nocut,
+      flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+      flow_kwargs=config.flow_kwargs,
+      sample_shape=(config.num_samples_plot,),
+  )
+  plot.posterior_plots(
+      az_data=az_data,
+      show_sigma_trace=False,
+      show_beta_trace=False,
+      show_tau_trace=False,
+      betasigma_pairplot_groups=(0, 1, 2),
+      tausigma_pairplot_groups=(0, 1, 2),
+      suffix=config.plot_suffix,
+      step=state_list[0].step,
       workdir_png=workdir,
+      summary_writer=summary_writer,
   )
 
   return state_list
+
+
+# # For debugging
+# config = get_config()
+# import pathlib
+# workdir = str(pathlib.Path.home() / f'modularbayes-output-exp/random_effects/nsf/full')
+# # train_and_evaluate(config, workdir)
```

### Comparing `modularbayes-0.1.2/examples/random_effects/configs/flow_nsf_cut1.py` & `modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_cut1.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
   # Data
   config.num_groups = 30
   config.num_obs_groups = [5, 5] + [5 for _ in range(config.num_groups - 2)]
   config.loc_groups = [10., 5.] + [0. for _ in range(config.num_groups - 2)]
   config.scale_groups = [1. for _ in range(config.num_groups)]
 
+  # Model hyper-parameters, defining the prior.
+  config.prior_hparams = None
+
   config.method = 'flow'
 
   # Defined in `flows`.
   config.flow_name = 'nsf'
 
   # kwargs to be passed to the flow
   config.flow_kwargs = ml_collections.ConfigDict()
@@ -30,19 +33,18 @@
   config.flow_kwargs.range_min = -10.
   # the upper bound of the spline's range
   config.flow_kwargs.range_max = 40.
 
   # SMI degree of influence
   config.smi_eta_groups = [0.0001, 1.
                           ] + [1. for _ in range(config.num_groups - 2)]
-  config.flow_kwargs.smi_eta = {'groups': config.smi_eta_groups}
-  config.plot_suffix = 'cut1'
+  config.plot_suffix = '_cut1'
 
   # Number of samples used to estimate the ELBO.
-  config.num_samples_elbo = 200
+  config.num_samples_elbo = 10
 
   # Number of training steps to run.
   config.training_steps = 30_000
 
   # Optimizer.
   config.optim_kwargs = ml_collections.ConfigDict()
   config.optim_kwargs.grad_clip_value = 1.0
@@ -66,15 +68,15 @@
   # Initial seed for random numbers.
   config.seed = 0
 
   # How often to log images to monitor convergence.
   config.log_img_steps = int(config.training_steps / 10)
 
   # Number of posteriors samples used in the plots.
-  config.num_samples_plot = 10_000
+  config.num_samples_plot = 40_000
 
   config.num_samples_eval = 1_000
 
   # How often to save model checkpoints.
   config.checkpoint_steps = int(config.training_steps / 4)
 
   # How many checkpoints to keep.
```

### Comparing `modularbayes-0.1.2/examples/random_effects/configs/flow_nsf_cut2.py` & `modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_cut2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
   # Data
   config.num_groups = 30
   config.num_obs_groups = [5, 5] + [5 for _ in range(config.num_groups - 2)]
   config.loc_groups = [10., 5.] + [0. for _ in range(config.num_groups - 2)]
   config.scale_groups = [1. for _ in range(config.num_groups)]
 
+  # Model hyper-parameters, defining the prior.
+  config.prior_hparams = None
+
   config.method = 'flow'
 
   # Defined in `flows`.
   config.flow_name = 'nsf'
   # kwargs to be passed to the flow
   config.flow_kwargs = ml_collections.ConfigDict()
   # Number of layers to use in the flow.
@@ -29,19 +32,18 @@
   config.flow_kwargs.range_min = -10.
   # the upper bound of the spline's range
   config.flow_kwargs.range_max = 40.
 
   # SMI degree of influence
   config.smi_eta_groups = [0.0001, 0.0001
                           ] + [1. for _ in range(config.num_groups - 2)]
-  config.flow_kwargs.smi_eta = {'groups': config.smi_eta_groups}
-  config.plot_suffix = 'cut2'
+  config.plot_suffix = '_cut2'
 
   # Number of samples used to estimate the ELBO.
-  config.num_samples_elbo = 200
+  config.num_samples_elbo = 10
 
   # Number of training steps to run.
   config.training_steps = 30_000
 
   # Optimizer.
   config.optim_kwargs = ml_collections.ConfigDict()
   config.optim_kwargs.grad_clip_value = 1.0
@@ -64,15 +66,15 @@
   # Initial seed for random numbers.
   config.seed = 0
 
   # How often to log images to monitor convergence.
   config.log_img_steps = config.training_steps / 10
 
   # Number of posteriors samples used in the plots.
-  config.num_samples_plot = 10_000
+  config.num_samples_plot = 40_000
 
   config.num_samples_eval = 1_000
 
   # How often to save model checkpoints.
   config.checkpoint_steps = config.training_steps / 4
 
   # How many checkpoints to keep.
```

### Comparing `modularbayes-0.1.2/examples/random_effects/configs/flow_nsf_cut3.py` & `modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_vmp_map.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,77 +9,91 @@
 
   # Data
   config.num_groups = 30
   config.num_obs_groups = [5, 5] + [5 for _ in range(config.num_groups - 2)]
   config.loc_groups = [10., 5.] + [0. for _ in range(config.num_groups - 2)]
   config.scale_groups = [1. for _ in range(config.num_groups)]
 
-  config.method = 'flow'
+  # Model hyper-parameters, defining the prior.
+  config.prior_hparams = None
+
+  config.method = 'vmp_map'
 
   # Defined in `flows`.
   config.flow_name = 'nsf'
-
   # kwargs to be passed to the flow
   config.flow_kwargs = ml_collections.ConfigDict()
   # Number of layers to use in the flow.
   config.flow_kwargs.num_layers = 8
   # Hidden sizes of the MLP conditioner.
   config.flow_kwargs.hidden_sizes = [30] * 3 + [10]
   # Number of bins to use in the rational-quadratic spline.
   config.flow_kwargs.num_bins = 10
   # the lower bound of the spline's range
   config.flow_kwargs.range_min = -10.
   # the upper bound of the spline's range
   config.flow_kwargs.range_max = 40.
 
-  # SMI degree of influence
-  config.smi_eta_groups = [1., 0.0001
-                          ] + [1. for _ in range(config.num_groups - 2)]
-  config.flow_kwargs.smi_eta = {'groups': config.smi_eta_groups}
-  config.plot_suffix = 'cut3'
-
-  # Number of samples used to estimate the ELBO.
-  config.num_samples_elbo = 200
+  config.num_samples_elbo = 10
+  config.num_samples_eval = 5_000
 
   # Number of training steps to run.
-  config.training_steps = 30_000
+  config.training_steps = 100_000
 
-  # Optimizer.
+  # Optimizer
   config.optim_kwargs = ml_collections.ConfigDict()
   config.optim_kwargs.grad_clip_value = 1.0
+  # Using SGD with warm restarts, from Loschilov & Hutter (arXiv:1608.03983).
   config.optim_kwargs.lr_schedule_name = 'warmup_exponential_decay_schedule'
   config.optim_kwargs.lr_schedule_kwargs = ml_collections.ConfigDict()
   config.optim_kwargs.lr_schedule_kwargs = {
       'init_value': 0.,
-      'peak_value': 2e-3,
-      'warmup_steps': 2_000,
-      'transition_steps': 10_000,
+      'peak_value': 3e-4,
+      'warmup_steps': 3_000,
+      'transition_steps': 20_000,
       'decay_rate': 0.5,
       'transition_begin': 0,
       'staircase': False,
       'end_value': None,
   }
 
   # How often to evaluate the model.
   config.eval_steps = int(config.training_steps / 10)
-  # config.eval_steps = config.training_steps / 10
 
   # Initial seed for random numbers.
   config.seed = 0
 
   # How often to log images to monitor convergence.
   config.log_img_steps = int(config.training_steps / 10)
 
   # Number of posteriors samples used in the plots.
-  config.num_samples_plot = 10_000
+  config.num_samples_plot = 40_000
 
-  config.num_samples_eval = 1_000
+  config.smi_eta_dim = config.num_groups
+  config.smi_eta_plot = {
+      'full': [1. for _ in range(config.smi_eta_dim)],
+      'cut1': [0.0001, 1.] + [1. for _ in range(config.smi_eta_dim - 2)],
+      'cut2': [0.0001, 0.0001] + [1. for _ in range(config.smi_eta_dim - 2)],
+      'cut3': [1., 0.0001] + [1. for _ in range(config.smi_eta_dim - 2)],
+  }
 
   # How often to save model checkpoints.
   config.checkpoint_steps = int(config.training_steps / 4)
 
   # How many checkpoints to keep.
   config.checkpoints_keep = 1
 
-  config.num_samples_log_prob_test = 10_000
+  # Arguments for the Variational Meta-Posterior map
+  config.vmp_map_name = 'MLPVmpMap'
+  config.vmp_map_kwargs = ml_collections.ConfigDict()
+  eta_dim = config.num_groups
+  config.vmp_map_kwargs.hidden_sizes = [eta_dim * 10] * 5 + [20]
+
+  # Number of samples of eta for Meta-Posterior training
+  config.num_samples_eta = 25
+  config.eta_sampling_a = 0.2
+  config.eta_sampling_b = 1.0
+
+  config.lambda_idx_plot = [50 * i for i in range(5)]
+  config.constant_lambda_ignore_plot = True
 
   return config
```

### Comparing `modularbayes-0.1.2/examples/random_effects/configs/flow_nsf_full.py` & `modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_full.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 
   # Data
   config.num_groups = 30
   config.num_obs_groups = [5, 5] + [5 for _ in range(config.num_groups - 2)]
   config.loc_groups = [10., 5.] + [0. for _ in range(config.num_groups - 2)]
   config.scale_groups = [1. for _ in range(config.num_groups)]
 
+  # Model hyper-parameters, defining the prior.
+  config.prior_hparams = None
+
   config.method = 'flow'
 
   # Defined in `flows`.
   config.flow_name = 'nsf'
-
   # kwargs to be passed to the flow
   config.flow_kwargs = ml_collections.ConfigDict()
   # Number of layers to use in the flow.
   config.flow_kwargs.num_layers = 8
   # Hidden sizes of the MLP conditioner.
   config.flow_kwargs.hidden_sizes = [30] * 3 + [10]
   # Number of bins to use in the rational-quadratic spline.
@@ -29,19 +31,18 @@
   # the lower bound of the spline's range
   config.flow_kwargs.range_min = -10.
   # the upper bound of the spline's range
   config.flow_kwargs.range_max = 40.
 
   # SMI degree of influence
   config.smi_eta_groups = [1., 1.] + [1. for _ in range(config.num_groups - 2)]
-  config.flow_kwargs.smi_eta = {'groups': config.smi_eta_groups}
-  config.plot_suffix = 'full'
+  config.plot_suffix = '_full'
 
   # Number of samples used to estimate the ELBO.
-  config.num_samples_elbo = 200
+  config.num_samples_elbo = 10
 
   # Number of training steps to run.
   config.training_steps = 30_000
 
   # Optimizer.
   config.optim_kwargs = ml_collections.ConfigDict()
   config.optim_kwargs.grad_clip_value = 1.0
@@ -64,15 +65,15 @@
   # Initial seed for random numbers.
   config.seed = 0
 
   # How often to log images to monitor convergence.
   config.log_img_steps = int(config.training_steps / 10)
 
   # Number of posteriors samples used in the plots.
-  config.num_samples_plot = 10_000
+  config.num_samples_plot = 40_000
 
   config.num_samples_eval = 1_000
 
   # How often to save model checkpoints.
   config.checkpoint_steps = int(config.training_steps / 4)
 
   # How many checkpoints to keep.
```

### Comparing `modularbayes-0.1.2/examples/random_effects/configs/flow_nsf_vmp_flow.py` & `modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_vmp_flow.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 
   # Data
   config.num_groups = 30
   config.num_obs_groups = [5, 5] + [5 for _ in range(config.num_groups - 2)]
   config.loc_groups = [10., 5.] + [0. for _ in range(config.num_groups - 2)]
   config.scale_groups = [1. for _ in range(config.num_groups)]
 
+  # Model hyper-parameters, defining the prior.
+  config.prior_hparams = None
+
   config.method = 'vmp_flow'
 
   # Defined in `flows`.
   config.flow_name = 'meta_nsf'
-
   # kwargs to be passed to the flow
   config.flow_kwargs = ml_collections.ConfigDict()
   # Number of layers to use in the flow.
   config.flow_kwargs.num_layers = 8
   # Hidden sizes
   # Hidden sizes of the MLP conditioner.
   config.flow_kwargs.hidden_sizes_conditioner = [30] * 3 + [10]
@@ -30,15 +32,15 @@
   # Number of bins to use in the rational-quadratic spline.
   config.flow_kwargs.num_bins = 10
   # the lower bound of the spline's range
   config.flow_kwargs.range_min = -10.
   # the upper bound of the spline's range
   config.flow_kwargs.range_max = 40.
 
-  config.num_samples_elbo = 100
+  config.num_samples_elbo = 10
   config.num_samples_eval = 10_000
 
   # Number of training steps to run.
   config.training_steps = 200_000
 
   # Number of SGD steps to find the best eta
   config.eta_star_steps = 5_000
@@ -64,31 +66,31 @@
   config.optim_kwargs_eta = ml_collections.ConfigDict()
   config.optim_kwargs_eta.learning_rate = 1e-4
 
   # How often to evaluate the model.
   config.eval_steps = int(config.training_steps / 10)
 
   # Initial seed for random numbers.
-  config.seed = 123
+  config.seed = 0
 
   # How often to log images to monitor convergence.
   config.log_img_steps = int(config.training_steps / 10)
 
   # Number of posteriors samples used in the plots.
-  config.num_samples_plot = 10_000
+  config.num_samples_plot = 40_000
 
   config.num_samples_elpd = 1_000
 
-  config.eta_plot = [
-      [1. for _ in range(config.num_groups)],
-      [0.0001, 1.] + [1. for _ in range(config.num_groups - 2)],
-      [0.0001, 0.0001] + [1. for _ in range(config.num_groups - 2)],
-      [1., 0.0001] + [1. for _ in range(config.num_groups - 2)],
-  ]
-  config.suffix_eta_plot = ['full', 'cut1', 'cut2', 'cut3']
+  config.smi_eta_dim = config.num_groups
+  config.smi_eta_plot = {
+      'full': [1. for _ in range(config.smi_eta_dim)],
+      'cut1': [0.0001, 1.] + [1. for _ in range(config.smi_eta_dim - 2)],
+      'cut2': [0.0001, 0.0001] + [1. for _ in range(config.smi_eta_dim - 2)],
+      'cut3': [1., 0.0001] + [1. for _ in range(config.smi_eta_dim - 2)],
+  }
 
   # How often to save model checkpoints.
   config.checkpoint_steps = int(config.training_steps / 4)
 
   # How many checkpoints to keep.
   config.checkpoints_keep = 1
```

### Comparing `modularbayes-0.1.2/examples/random_effects/configs/mcmc_cut1.py` & `modularbayes-0.1.3/examples/random_effects/configs/mcmc_cut1.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 
   # Data
   config.num_groups = 30
   config.num_obs_groups = [5, 5] + [5 for _ in range(config.num_groups - 2)]
   config.loc_groups = [10., 5.] + [0. for _ in range(config.num_groups - 2)]
   config.scale_groups = [1. for _ in range(config.num_groups)]
 
+  # Model hyper-parameters, defining the prior.
+  config.prior_hparams = None
+
   config.method = 'mcmc'
 
-  # MCMC
-  config.num_samples = 10000
-  config.num_samples_subchain = 100
-  config.num_burnin_steps = 2000
-  config.mcmc_step_size = 0.01
-
-  config.smi_eta = {
-      'groups': [0.001, 1.] + [1. for _ in range(config.num_groups - 2)],
-  }
-  config.plot_suffix = 'cut1'
+  config.num_chains = 4
+  config.num_samples = 10_000
+  config.num_samples_subchain_stg2 = 50
+  config.num_samples_perchunk_stg2 = 1_000
+  config.num_steps_call_warmup = 100
+
+  config.smi_eta_groups = [0.001, 1.
+                          ] + [1. for _ in range(config.num_groups - 2)]
+  config.plot_suffix = '_cut1'
 
   config.seed = 0
 
   return config
```

### Comparing `modularbayes-0.1.2/examples/random_effects/configs/mcmc_cut2.py` & `modularbayes-0.1.3/examples/random_effects/configs/mcmc_cut2.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 
   # Data
   config.num_groups = 30
   config.num_obs_groups = [5, 5] + [5 for _ in range(config.num_groups - 2)]
   config.loc_groups = [10., 5.] + [0. for _ in range(config.num_groups - 2)]
   config.scale_groups = [1. for _ in range(config.num_groups)]
 
+  # Model hyper-parameters, defining the prior.
+  config.prior_hparams = None
+
   config.method = 'mcmc'
 
-  # MCMC
-  config.num_samples = 10000
-  config.num_samples_subchain = 100
-  config.num_burnin_steps = 2000
-  config.mcmc_step_size = 0.01
-
-  config.smi_eta = {
-      'groups': [0.001, 0.001] + [1. for _ in range(config.num_groups - 2)],
-  }
-  config.plot_suffix = 'cut2'
+  config.num_chains = 4
+  config.num_samples = 10_000
+  config.num_samples_subchain_stg2 = 50
+  config.num_samples_perchunk_stg2 = 1_000
+  config.num_steps_call_warmup = 100
+
+  config.smi_eta_groups = [0.001, 0.001
+                          ] + [1. for _ in range(config.num_groups - 2)]
+  config.plot_suffix = '_cut2'
 
   config.seed = 0
 
   return config
```

### Comparing `modularbayes-0.1.2/examples/random_effects/configs/mcmc_cut3.py` & `modularbayes-0.1.3/examples/random_effects/configs/mcmc_cut3.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 
   # Data
   config.num_groups = 30
   config.num_obs_groups = [5, 5] + [5 for _ in range(config.num_groups - 2)]
   config.loc_groups = [10., 5.] + [0. for _ in range(config.num_groups - 2)]
   config.scale_groups = [1. for _ in range(config.num_groups)]
 
+  # Model hyper-parameters, defining the prior.
+  config.prior_hparams = None
+
   config.method = 'mcmc'
 
-  # MCMC
-  config.num_samples = 10000
-  config.num_samples_subchain = 100
-  config.num_burnin_steps = 2000
-  config.mcmc_step_size = 0.01
-
-  config.smi_eta = {
-      'groups': [1., 0.001] + [1. for _ in range(config.num_groups - 2)],
-  }
-  config.plot_suffix = 'cut3'
+  config.num_chains = 4
+  config.num_samples = 10_000
+  config.num_samples_subchain_stg2 = 50
+  config.num_samples_perchunk_stg2 = 1_000
+  config.num_steps_call_warmup = 100
+
+  config.smi_eta_groups = [1., 0.001
+                          ] + [1. for _ in range(config.num_groups - 2)]
+  config.plot_suffix = '_cut3'
 
   config.seed = 0
 
   return config
```

### Comparing `modularbayes-0.1.2/examples/random_effects/flows.py` & `modularbayes-0.1.3/examples/random_effects/flows.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,111 +5,62 @@
 from jax import numpy as jnp
 import distrax
 from tensorflow_probability.substrates import jax as tfp
 
 import modularbayes
 from modularbayes._src.typing import Any, Array, Dict, Sequence
 
-tfb = tfp.bijectors
-
-
-def mean_field_sigma(
-    num_groups: int,
-    **_,
-) -> modularbayes.Transformed:
-  """Creates a Mean Field Flow."""
+from log_prob_fun import ModelParamsCut, ModelParamsNoCut
 
-  flow_dim = num_groups  # sigma's
-  event_shape = (flow_dim,)
-
-  flow_layers = []
+tfb = tfp.bijectors
 
-  # Layer 1: Trainable Affine transformation
-  conditioner = modularbayes.MeanFieldConditioner(flow_dim=flow_dim)
-  loc, log_scale = conditioner()
-  flow_layers.append(
-      distrax.Block(distrax.ScalarAffine(shift=loc, log_scale=log_scale), 1))
-  # flow_layers.append(tfb.Shift(loc)(tfb.Scale(log_scale=log_scale)))
 
-  # Last layer: Map values to parameter domain
+def bijector_domain_nocut() -> distrax.Bijector:
+  """Returns a distrax bijector for the uncut parameters
+  The bijector maps from an unconstrained space to the parameter domain.
+  """
   # sigma goes to [0,Inf]
-  flow_layers.append(distrax.Block(tfb.Softplus(), 1))
-
-  # Chain all layers together
-  flow = distrax.Chain(flow_layers[::-1])
-
-  base_distribution = distrax.MultivariateNormalDiag(
-      loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
-
-  q_distr = modularbayes.Transformed(base_distribution, flow)
+  bij_nocut = distrax.Block(tfb.Softplus(), 1)
+  return bij_nocut
 
-  return q_distr
 
-
-def mean_field_beta_tau(
-    num_groups: int,
-    **_,
-) -> modularbayes.ConditionalTransformed:
-  """Creates a Mean Field Flow."""
-
-  flow_dim = num_groups + 1  # beta's and tau
-
-  event_shape = (flow_dim,)
-
-  flow_layers = []
-
-  # Layer 1: Trainable Affine transformation
-  conditioner = modularbayes.MeanFieldConditioner(flow_dim=flow_dim)
-  loc, log_scale = conditioner()
-  flow_layers.append(
-      distrax.Block(distrax.ScalarAffine(shift=loc, log_scale=log_scale), 1))
-  # flow_layers.append(tfb.Shift(loc)(tfb.Scale(log_scale=log_scale)))
-
-  # Last layer: Map values to parameter domain
-  # beta goes to [-Inf,Inf]
-  # tau goes to [0,Inf]
+def bijector_domain_cut(num_groups: int) -> distrax.Bijector:
+  """Returns a distrax bijector for the cut parameters
+  The bijector maps from an unconstrained space to the parameter domain.
+  """
   block_bijectors = [
       distrax.Block(tfb.Identity(), 1),
       distrax.Block(tfb.Softplus(), 1),
   ]
   block_sizes = [num_groups, 1]
-  flow_layers.append(
-      modularbayes.Blockwise(
-          bijectors=block_bijectors, block_sizes=block_sizes))
-
-  # Chain all layers together
-  flow = modularbayes.ConditionalChain(flow_layers[::-1])
+  bij_cut = modularbayes.Blockwise(
+      bijectors=block_bijectors, block_sizes=block_sizes)
+  return bij_cut
 
-  base_distribution = distrax.MultivariateNormalDiag(
-      loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
-
-  q_distr = modularbayes.ConditionalTransformed(base_distribution, flow)
-
-  return q_distr
 
-
-def nsf_sigma(
+def get_q_nocut_nsf(
     num_groups: int,
     num_layers: int,
     hidden_sizes: Sequence[int],
     num_bins: int,
     range_min: float = 0.,
     range_max: float = 1.,
     **_,
-) -> modularbayes.Transformed:
+) -> distrax.Transformed:
   """Creates the Rational Quadratic Flow model.
 
   Args:
   range_min: the lower bound of the spline's range. Below `range_min`, the
     bijector defaults to a linear transformation.
   range_max: the upper bound of the spline's range. Above `range_max`, the
     bijector defaults to a linear transformation.
   """
 
-  flow_dim = num_groups  # sigma's
+  flow_dim = num_groups
+
   event_shape = (flow_dim,)
 
   flow_layers = []
 
   # Number of parameters required by the bijector (rational quadratic spline)
   num_bijector_params = 3 * num_bins + 1
 
@@ -123,46 +74,47 @@
   mask = mask.astype(bool)
 
   # Number of parameters for the rational-quadratic spline:
   # - `num_bins` bin widths
   # - `num_bins` bin heights
   # - `num_bins + 1` knot slopes
   # for a total of `3 * num_bins + 1` parameters.
-
   for _ in range(num_layers):
     layer = distrax.MaskedCoupling(
         mask=mask,
         bijector=bijector_fn,
         conditioner=modularbayes.MLPConditioner(
             output_dim=math.prod(event_shape),
             hidden_sizes=hidden_sizes,
             num_bijector_params=num_bijector_params,
-            name='conditioner_sigma',
+            name='conditioner_nocut',
         ),
     )
     flow_layers.append(layer)
     # Flip the mask after each layer.
     mask = jnp.logical_not(mask)
 
   # Last layer: Map values to parameter domain
-  # sigma goes to [0,Inf]
-  flow_layers.append(distrax.Block(tfb.Softplus(), 1))
+  bij_nocut = bijector_domain_nocut()
+  flow_layers.append(bij_nocut)
 
-  # Chain all layers together
+  # Chain all flow layers together
   flow = distrax.Chain(flow_layers[::-1])
 
+  # base_distribution = distrax.Independent(
+  #     distrax.Uniform(low=jnp.zeros(event_shape), high=jnp.ones(event_shape)),
+  #     reinterpreted_batch_ndims=len(event_shape))
+
   base_distribution = distrax.MultivariateNormalDiag(
       loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
 
-  q_distr = modularbayes.Transformed(base_distribution, flow)
-
-  return q_distr
+  return modularbayes.Transformed(base_distribution, flow)
 
 
-def nsf_beta_tau(
+def get_q_cutgivennocut_nsf(
     num_groups: int,
     num_layers: int,
     hidden_sizes: Sequence[int],
     num_bins: int,
     range_min: float = 0.,
     range_max: float = 1.,
     **_,
@@ -172,16 +124,15 @@
   Args:
   range_min: the lower bound of the spline's range. Below `range_min`, the
     bijector defaults to a linear transformation.
   range_max: the upper bound of the spline's range. Above `range_max`, the
     bijector defaults to a linear transformation.
   """
 
-  flow_dim = num_groups + 1  # beta's and tau
-
+  flow_dim = num_groups + 1
   event_shape = (flow_dim,)
 
   flow_layers = []
 
   # Number of parameters required by the bijector (rational quadratic spline)
   num_bijector_params = 3 * num_bins + 1
 
@@ -204,45 +155,39 @@
     layer = modularbayes.ConditionalMaskedCoupling(
         mask=mask,
         bijector=bijector_fn,
         conditioner=modularbayes.MLPConditioner(
             output_dim=math.prod(event_shape),
             hidden_sizes=hidden_sizes,
             num_bijector_params=num_bijector_params,
-            name='conditioner_beta_tau',
+            name='conditioner_theta',
         ),
     )
     flow_layers.append(layer)
     # Flip the mask after each layer.
     mask = jnp.logical_not(mask)
 
   # Last layer: Map values to parameter domain
-  # beta goes to [-Inf,Inf]
-  # tau goes to [0,Inf]
-  block_bijectors = [
-      distrax.Block(tfb.Identity(), 1),
-      distrax.Block(tfb.Softplus(), 1),
-  ]
-  block_sizes = [num_groups, 1]
-  flow_layers.append(
-      modularbayes.Blockwise(
-          bijectors=block_bijectors, block_sizes=block_sizes))
+  bij_cut = bijector_domain_cut(num_groups=num_groups)
+  flow_layers.append(bij_cut)
 
-  # Chain all layers together
+  # Chain all flow layers together
   flow = modularbayes.ConditionalChain(flow_layers[::-1])
 
+  # base_distribution = distrax.Independent(
+  #     distrax.Uniform(low=jnp.zeros(event_shape), high=jnp.ones(event_shape)),
+  #     reinterpreted_batch_ndims=len(event_shape))
+
   base_distribution = distrax.MultivariateNormalDiag(
       loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
 
-  q_distr = modularbayes.ConditionalTransformed(base_distribution, flow)
-
-  return q_distr
+  return modularbayes.ConditionalTransformed(base_distribution, flow)
 
 
-def meta_nsf_sigma(
+def get_q_nocut_meta_nsf(
     num_groups: int,
     num_layers: int,
     hidden_sizes_conditioner: Sequence[int],
     hidden_sizes_conditioner_eta: Sequence[int],
     num_bins: int,
     range_min: float = 0.,
     range_max: float = 1.,
@@ -253,15 +198,16 @@
   Args:
   range_min: the lower bound of the spline's range. Below `range_min`, the
     bijector defaults to a linear transformation.
   range_max: the upper bound of the spline's range. Above `range_max`, the
     bijector defaults to a linear transformation.
   """
 
-  flow_dim = num_groups  # sigma's
+  flow_dim = num_groups
+
   event_shape = (flow_dim,)
 
   flow_layers = []
 
   # Number of parameters required by the bijector (rational quadratic spline)
   num_bijector_params = 3 * num_bins + 1
 
@@ -284,43 +230,45 @@
     layer = modularbayes.EtaConditionalMaskedCoupling(
         mask=mask,
         bijector=bijector_fn,
         conditioner_eta=modularbayes.MLPConditioner(
             output_dim=math.prod(event_shape),
             hidden_sizes=hidden_sizes_conditioner_eta,
             num_bijector_params=num_bijector_params,
-            name='conditioner_eta_sigma',
+            name='conditioner_eta_nocut',
         ),
         conditioner=modularbayes.MLPConditioner(
             output_dim=math.prod(event_shape),
             hidden_sizes=hidden_sizes_conditioner,
             num_bijector_params=num_bijector_params,
-            name='conditioner_sigma',
+            name='conditioner_nocut',
         ),
     )
     flow_layers.append(layer)
     # Flip the mask after each layer.
     mask = jnp.logical_not(mask)
 
-  # Last layer: Map values to parameter domain
-  # sigma goes to [0,Inf]
-  flow_layers.append(distrax.Block(tfb.Softplus(), 1))
+  # Last Layer: Map values to parameter domain
+  bij_nocut = bijector_domain_nocut()
+  flow_layers.append(bij_nocut)
 
-  # Chain all layers together
+  # Chain all flow layers together
   flow = modularbayes.ConditionalChain(flow_layers[::-1])
 
+  # base_distribution = distrax.Independent(
+  #     distrax.Uniform(low=jnp.zeros(event_shape), high=jnp.ones(event_shape)),
+  #     reinterpreted_batch_ndims=len(event_shape))
+
   base_distribution = distrax.MultivariateNormalDiag(
       loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
 
-  q_distr = modularbayes.ConditionalTransformed(base_distribution, flow)
-
-  return q_distr
+  return modularbayes.ConditionalTransformed(base_distribution, flow)
 
 
-def meta_nsf_beta_tau(
+def get_q_cutgivennocut_meta_nsf(
     num_groups: int,
     num_layers: int,
     hidden_sizes_conditioner: Sequence[int],
     hidden_sizes_conditioner_eta: Sequence[int],
     num_bins: int,
     range_min: float = 0.,
     range_max: float = 1.,
@@ -331,16 +279,15 @@
   Args:
   range_min: the lower bound of the spline's range. Below `range_min`, the
     bijector defaults to a linear transformation.
   range_max: the upper bound of the spline's range. Above `range_max`, the
     bijector defaults to a linear transformation.
   """
 
-  flow_dim = num_groups + 1  # beta's and tau
-
+  flow_dim = num_groups + 1
   event_shape = (flow_dim,)
 
   flow_layers = []
 
   # Number of parameters required by the bijector (rational quadratic spline)
   num_bijector_params = 3 * num_bins + 1
 
@@ -363,83 +310,92 @@
     layer = modularbayes.EtaConditionalMaskedCoupling(
         mask=mask,
         bijector=bijector_fn,
         conditioner_eta=modularbayes.MLPConditioner(
             output_dim=math.prod(event_shape),
             hidden_sizes=hidden_sizes_conditioner_eta,
             num_bijector_params=num_bijector_params,
-            name='conditioner_eta_beta_tau',
+            name='conditioner_eta_theta',
         ),
         conditioner=modularbayes.MLPConditioner(
+            # input_dim=math.prod(event_shape),
             output_dim=math.prod(event_shape),
             hidden_sizes=hidden_sizes_conditioner,
             num_bijector_params=num_bijector_params,
-            name='conditioner_beta_tau',
+            name='conditioner_theta',
         ),
     )
     flow_layers.append(layer)
     # Flip the mask after each layer.
     mask = jnp.logical_not(mask)
 
   # Last layer: Map values to parameter domain
-  # beta goes to [-Inf,Inf]
-  # tau goes to [0,Inf]
-  block_bijectors = [
-      distrax.Block(tfb.Identity(), 1),
-      distrax.Block(tfb.Softplus(), 1),
-  ]
-  block_sizes = [num_groups, 1]
-  flow_layers.append(
-      modularbayes.Blockwise(
-          bijectors=block_bijectors, block_sizes=block_sizes))
+  bij_cut = bijector_domain_cut(num_groups=num_groups)
+  flow_layers.append(bij_cut)
 
-  # Chain all layers together
+  # Chain all flow layers together
   flow = modularbayes.ConditionalChain(flow_layers[::-1])
 
   base_distribution = distrax.MultivariateNormalDiag(
       loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
 
   q_distr = modularbayes.ConditionalTransformed(base_distribution, flow)
 
   return q_distr
 
 
-def split_flow_sigma(
-    samples: Array,
+def split_flow_nocut(
+    concat_params: Array,
     num_groups: int,
     **_,
 ) -> Dict[str, Any]:
   """Get model parameters by splitting samples from the flow."""
 
-  flow_dim = num_groups  # sigma's
-  assert samples.ndim == 2
-  assert samples.shape[-1] == flow_dim
+  flow_dim = num_groups
 
-  samples_dict = {}
+  assert concat_params.ndim == 1
+  assert concat_params.shape[-1] == flow_dim
 
-  # sigma
-  samples_dict['sigma'] = samples
+  model_params_nocut = ModelParamsNoCut(sigma=concat_params)
 
-  return samples_dict
+  return model_params_nocut
 
 
-def split_flow_beta_tau(
-    samples: Array,
+def split_flow_cut(
+    concat_params: Array,
     num_groups: int,
-    is_aux: bool,
     **_,
 ) -> Dict[str, Any]:
-  """Get model parameters by splitting samples from the flow."""
+  """Get model parameters by splitting samples from the flow.
+  
+  The parameter theta contain the intercept and slope of the
+  prevalence-incidence model.
+  """
+  flow_dim = num_groups + 1
 
-  flow_dim = num_groups + 1  # beta's and tau
+  assert concat_params.ndim == 1
+  assert concat_params.shape[-1] == flow_dim
+  beta, tau = jnp.split(concat_params, [num_groups], axis=-1)
 
-  assert samples.ndim == 2
-  assert samples.shape[-1] == flow_dim
+  model_params_cut = ModelParamsCut(beta=beta, tau=tau)
 
-  samples_dict = {}
+  return model_params_cut
 
-  # beta and tau
-  (samples_dict['beta' + ('_aux' if is_aux else '')],
-   samples_dict['tau' + ('_aux' if is_aux else '')]) = jnp.split(
-       samples, [num_groups], axis=-1)
 
-  return samples_dict
+def concat_flow_nocut(
+    model_params: ModelParamsNoCut,
+    **_,
+) -> Dict[str, Any]:
+  """Concatenate model parameters from ModelParamsNoCut into a single array."""
+  concat_params = model_params[0]
+  assert concat_params.ndim == 1
+  return concat_params
+
+
+def concat_flow_cut(
+    model_params: ModelParamsNoCut,
+    **_,
+) -> Dict[str, Any]:
+  """Concatenate model parameters from ModelParamsCut into a single array."""
+  concat_params = jnp.concatenate(model_params, axis=-1)
+  assert concat_params.ndim == 1
+  return concat_params
```

### Comparing `modularbayes-0.1.2/examples/random_effects/main.py` & `modularbayes-0.1.3/examples/random_effects/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 
 from absl import app
 from absl import flags
 from absl import logging
 
 import jax
 from ml_collections import config_flags
-import tensorflow as tf
 
-import run_mcmc
+import sample_mcmc
 import train_flow
 import train_vmp_flow
 import train_vmp_map
 
 FLAGS = flags.FLAGS
 
 flags.DEFINE_string('workdir', None, 'Directory to store model data.')
@@ -35,25 +34,20 @@
 
   # log to a file
   if FLAGS.log_dir:
     if not os.path.exists(FLAGS.log_dir):
       os.makedirs(FLAGS.log_dir)
     logging.get_absl_handler().use_absl_log_file()
 
-  # Hide any GPUs form TensorFlow. Otherwise TF might reserve memory and make
-  # it unavailable to JAX.
-  tf.config.experimental.set_visible_devices([], 'GPU')
-  tf.config.experimental.set_visible_devices([], 'TPU')
-
   logging.info('JAX process: %d / %d', jax.process_index(), jax.process_count())
   logging.info('JAX local devices: %r', jax.local_devices())
   logging.info('JAX device count: %r', jax.device_count())
 
   if FLAGS.config.method == 'mcmc':
-    run_mcmc.sample_and_evaluate(FLAGS.config, FLAGS.workdir)
+    sample_mcmc.sample_and_evaluate(FLAGS.config, FLAGS.workdir)
   elif FLAGS.config.method == 'flow':
     train_flow.train_and_evaluate(FLAGS.config, FLAGS.workdir)
   elif FLAGS.config.method == 'vmp_flow':
     train_vmp_flow.train_and_evaluate(FLAGS.config, FLAGS.workdir)
   elif FLAGS.config.method == 'vmp_map':
     train_vmp_map.train_and_evaluate(FLAGS.config, FLAGS.workdir)
```

### Comparing `modularbayes-0.1.2/modularbayes/__init__.py` & `modularbayes-0.1.3/modularbayes/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 """modularbayes: Variational methods for Bayesian Semi-Modular Inference."""
 
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 from modularbayes._src.bijectors.blockwise import Blockwise
 from modularbayes._src.bijectors.conditional_bijector import ConditionalBijector
 from modularbayes._src.bijectors.conditional_chain import ConditionalChain
 from modularbayes._src.bijectors.conditional_masked_coupling import ConditionalMaskedCoupling
 from modularbayes._src.bijectors.conditional_masked_coupling_extra import EtaConditionalMaskedCoupling
 
 from modularbayes._src.conditioners.base import MeanFieldConditioner
 from modularbayes._src.conditioners.base import MLPConditioner
 
 from modularbayes._src.distributions.conditional_transformed import ConditionalTransformed
 from modularbayes._src.distributions.transformed import Transformed
 
-from modularbayes._src.metaposterior.vmp_map import VmpMap
+from modularbayes._src.metaposterior.vmp_map import MLPVmpMap
+
+from modularbayes._src.smi.sampling import sample_q_nocut
+from modularbayes._src.smi.sampling import sample_q_cutgivennocut
+from modularbayes._src.smi.sampling import sample_q
+from modularbayes._src.smi.elbo import elbo_smi
+from modularbayes._src.smi.elbo import elbo_smi_vmpflow
+from modularbayes._src.smi.elbo import elbo_smi_vmpmap
 
 from modularbayes._src.utils.misc import cart2pol
+from modularbayes._src.utils.misc import clean_filename
 from modularbayes._src.utils.misc import colour_fader
 from modularbayes._src.utils.misc import flatten_dict
 from modularbayes._src.utils.misc import list_from_csv
 from modularbayes._src.utils.misc import plot_to_image
 from modularbayes._src.utils.misc import normalize_images
 
 from modularbayes._src.utils.training import TrainState
@@ -38,16 +46,23 @@
     'ConditionalChain',
     'ConditionalMaskedCoupling',
     'EtaConditionalMaskedCoupling',
     'MeanFieldConditioner',
     'MLPConditioner',
     'ConditionalTransformed',
     'Transformed',
-    'VmpMap',
+    'MLPVmpMap',
+    'sample_q_nocut',
+    'sample_q_cutgivennocut',
+    'sample_q',
+    'elbo_smi',
+    'elbo_smi_vmpflow',
+    'elbo_smi_vmpmap',
     'cart2pol',
+    'clean_filename',
     'colour_fader',
     'flatten_dict',
     'list_from_csv',
     'plot_to_image',
     'normalize_images',
     'TrainState',
     'initial_state',
```

### Comparing `modularbayes-0.1.2/modularbayes/_src/bijectors/blockwise.py` & `modularbayes-0.1.3/modularbayes/_src/bijectors/blockwise.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,34 +26,22 @@
   Example Use:
 
   ```python
   blockwise = tfb.Blockwise(
       bijectors=[tfb.Exp(), tfb.Sigmoid()], block_sizes=[2, 1]
     )
   y = blockwise.forward(x)
-
-  # Equivalent to:
-  x_0, x_1 = tf.split(x, [2, 1], axis=-1)
-  y_0 = tfb.Exp().forward(x_0)
-  y_1 = tfb.Sigmoid().forward(x_1)
-  y = tf.concat([y_0, y_1], axis=-1)
   ```
 
   Keyword arguments can be passed to the inner bijectors by utilizing the inner
   bijector names, e.g.:
 
   ```python
   blockwise = tfb.Blockwise([Bijector1(name='b1'), Bijector2(name='b2')])
   y = blockwise.forward(x, b1={'arg': 1}, b2={'arg': 2})
-
-  # Equivalent to:
-  x_0, x_1 = tf.split(x, [1, 1], axis=-1)
-  y_0 = Bijector1().forward(x_0, arg=1)
-  y_1 = Bijector2().forward(x_1, arg=2)
-  y = tf.concat([y_0, y_1], axis=-1)
   ```
 
   """
 
   def __init__(
       self,
       bijectors: Sequence[BijectorLike],
```

### Comparing `modularbayes-0.1.2/modularbayes/_src/bijectors/conditional_bijector.py` & `modularbayes-0.1.3/modularbayes/_src/bijectors/conditional_bijector.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.2/modularbayes/_src/bijectors/conditional_chain.py` & `modularbayes-0.1.3/modularbayes/_src/bijectors/conditional_chain.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.2/modularbayes/_src/bijectors/conditional_masked_coupling.py` & `modularbayes-0.1.3/modularbayes/_src/bijectors/conditional_masked_coupling.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.2/modularbayes/_src/bijectors/conditional_masked_coupling_extra.py` & `modularbayes-0.1.3/modularbayes/_src/bijectors/conditional_masked_coupling_extra.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.2/modularbayes/_src/conditioners/base.py` & `modularbayes-0.1.3/modularbayes/_src/conditioners/base.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.2/modularbayes/_src/distributions/conditional_transformed.py` & `modularbayes-0.1.3/modularbayes/_src/distributions/conditional_transformed.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.2/modularbayes/_src/distributions/transformed.py` & `modularbayes-0.1.3/modularbayes/_src/distributions/transformed.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.2/modularbayes/_src/metaposterior/vmp_map.py` & `modularbayes-0.1.3/modularbayes/_src/metaposterior/vmp_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import haiku as hk
 import jax
 from jax import numpy as jnp
 
 from modularbayes._src.typing import Array, List, Optional
 
 
-class VmpMap(hk.Module):
+class MLPVmpMap(hk.Module):
   """Trainable mapping from eta to normalizing flow parameters."""
 
   def __init__(
       self,
       params_flow_init: hk.Params,
       hidden_sizes: List[int],
       name: Optional[str] = None,
```

### Comparing `modularbayes-0.1.2/modularbayes/_src/typing.py` & `modularbayes-0.1.3/modularbayes/_src/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 
 from pathlib import Path, PosixPath
 
 import jax
 
 import numpy as np
 
-from flax.metrics.tensorboard import SummaryWriter
-
 from chex import Array, PRNGKey
 
 from collections import OrderedDict
 from ml_collections import ConfigDict
 
 from tensorflow_probability.substrates import jax as tfp
 
@@ -33,16 +31,14 @@
 Batch = Mapping[str, ArrayNumpy]
 
 RangeFloat = Tuple[float, float]
 RangeInt = Tuple[int, Union[int, None]]
 
 Kernel = tfp.math.psd_kernels.PositiveSemidefiniteKernel
 
-SmiEta = Mapping[str, np.ndarray]
-
 __all__ = [
     'Any',
     'Array',
     'ArrayNumpy',
     'ArraySharded',
     'BijectorParams',
     'Callable',
@@ -63,12 +59,10 @@
     'Path',
     'PosixPath',
     'RangeFloat',
     'RangeInt',
     'Sequence',
     'Scalar',
     'Shape',
-    'SmiEta',
-    'SummaryWriter',
     'Tuple',
     'Union',
 ]
```

### Comparing `modularbayes-0.1.2/modularbayes/_src/utils/training.py` & `modularbayes-0.1.3/modularbayes/_src/utils/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 import functools
 import os
 import pathlib
 import pickle
 
 from absl import logging
 
-from tensorflow.io import gfile
-
 import haiku as hk
 import jax
 from jax import lax
 from jax import numpy as jnp
 
 import optax
 
 from modularbayes._src.typing import (Any, Batch, Callable, Dict, List, Metrics,
-                                 NamedTuple, PRNGKey, Tuple, Union)
+                                      NamedTuple, PRNGKey, Tuple, Union)
 
 
 def save_ckpt(state: NamedTuple, path: Union[str, pathlib.Path]) -> None:
   r"""Save Haiku state.
 
     A more mature checkpointing implementation might:
     - Use np.savez() to store the core data instead of pickle.
@@ -112,15 +110,15 @@
       save_ckpt(state, str(pathlib.Path(checkpoint_dir) / checkpoint_file_now))
 
     if len(checkpoint_files) > keep:
       old_ckpts = checkpoint_files[:-keep]
       for old_ckpt in old_ckpts:
         ckpt_path = pathlib.Path(checkpoint_dir) / old_ckpt
         logging.info('Removing checkpoint at %s', ckpt_path)
-        gfile.remove(ckpt_path)
+        os.remove(ckpt_path)
 
 
 def update_state(
     state: TrainState,
     batch: Batch,
     prng_key: PRNGKey,
     optimizer: optax.GradientTransformation,
```

### Comparing `modularbayes-0.1.2/modularbayes.egg-info/PKG-INFO` & `modularbayes-0.1.3/modularbayes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modularbayes
-Version: 0.1.2
+Version: 0.1.3
 Summary: Modular Bayesian Inference.
 Home-page: https://github.com/chriscarmona/modularbayes
 Author: Chris Carmona
 Author-email: carmona@stats.ox.ac.uk
 Maintainer-email: carmona@stats.ox.ac.uk
 License: MIT
 Keywords: modular bayesian inference cut smi posterior probability distribution
@@ -44,14 +44,15 @@
 
 We provide code to replicate all the experiments from our article in the [examples](https://github.com/chriscarmona/modularbayes/tree/main/examples) folder.
 There are main two examples: 1) epidemiological model and 2) random effects model.
 By executing the `run.sh` bash script in that folder, one can train all variational posteriors and produce visualizations and summaries (follow [*Installation instructions*](#installation-instructions) and examine `run.sh` before execution).
 
 You can customize the output directories within the script and choose the experiments that you wish to run.
 ```bash
+pip install -Ur examples/requirements.txt
 chmod +x examples/run.sh
 bash examples/run.sh
 ```
 Results produced during the optimization can be monitored in [Tensorboard](https://www.tensorflow.org/tensorboard):
 ```bash
 WORK_DIR=$HOME/modularbayes-output
 tensorboard --logdir=$WORK_DIR
@@ -59,15 +60,15 @@
 
 ## Installation instructions
 
 1. \[Optional] Create a new virtual environment for this project (see [*Create a virtual environment*](#create-a-virtual-environment) below).
 2. Install JAX. This may vary according to your CUDA version (See [JAX installation](https://github.com/google/jax#installation)).
 3. Install the latest released version of `modularbayes` from [Pypi](https://pypi.org/project/modularbayes/) via:
 ```bash
-pip install modularbayes
+pip install -U modularbayes
 ```
 or you can install the latest development version from GitHub:
 ```bash
 pip install git+https://github.com/chriscarmona/modularbayes
 ```
 
 ## Citation
@@ -104,14 +105,15 @@
 ```
 
 ### Creating a virtual environment
 
 For OSX or Linux, you can use `venv` (see the [venv documentation](https://docs.python.org/3/library/venv.html)).
 
 ```bash
+rm -rf ~/.virtualenvs/modularbayes
 python3 -m venv ~/.virtualenvs/modularbayes
 source ~/.virtualenvs/modularbayes/bin/activate
 pip install -U pip
 pip install -U setuptools wheel
 ```
 
 Feel free to change the folder where the virtual environment is created by replacing `~/.virtualenvs/modularbayes` with a path of your choice in both commands.
```

### Comparing `modularbayes-0.1.2/modularbayes.egg-info/SOURCES.txt` & `modularbayes-0.1.3/modularbayes.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 MANIFEST.in
 README.md
 setup.py
 examples/epidemiology/flows.py
 examples/epidemiology/log_prob_fun.py
 examples/epidemiology/main.py
 examples/epidemiology/plot.py
-examples/epidemiology/run_mcmc.py
+examples/epidemiology/sample_mcmc.py
 examples/epidemiology/train_flow.py
 examples/epidemiology/train_vmp_flow.py
 examples/epidemiology/train_vmp_map.py
 examples/epidemiology/configs/flow_mf.py
 examples/epidemiology/configs/flow_mf_vmp_map.py
 examples/epidemiology/configs/flow_nsf.py
 examples/epidemiology/configs/flow_nsf_vmp_flow.py
@@ -18,15 +18,15 @@
 examples/epidemiology/configs/mcmc.py
 examples/epidemiology/data/__init__.py
 examples/epidemiology/data/load.py
 examples/random_effects/flows.py
 examples/random_effects/log_prob_fun.py
 examples/random_effects/main.py
 examples/random_effects/plot.py
-examples/random_effects/run_mcmc.py
+examples/random_effects/sample_mcmc.py
 examples/random_effects/train_flow.py
 examples/random_effects/train_vmp_flow.py
 examples/random_effects/train_vmp_map.py
 examples/random_effects/configs/flow_nsf_cut1.py
 examples/random_effects/configs/flow_nsf_cut2.py
 examples/random_effects/configs/flow_nsf_cut3.py
 examples/random_effects/configs/flow_nsf_full.py
@@ -54,14 +54,16 @@
 modularbayes/_src/conditioners/__init__.py
 modularbayes/_src/conditioners/base.py
 modularbayes/_src/distributions/__init__.py
 modularbayes/_src/distributions/conditional_transformed.py
 modularbayes/_src/distributions/transformed.py
 modularbayes/_src/metaposterior/__init__.py
 modularbayes/_src/metaposterior/vmp_map.py
+modularbayes/_src/smi/elbo.py
+modularbayes/_src/smi/sampling.py
 modularbayes/_src/utils/__init__.py
 modularbayes/_src/utils/misc.py
 modularbayes/_src/utils/training.py
 requirements/requirements-devel.txt
 requirements/requirements-setup.txt
 requirements/requirements-tests.txt
 requirements/requirements.txt
```

### Comparing `modularbayes-0.1.2/setup.py` & `modularbayes-0.1.3/setup.py`

 * *Files identical despite different names*

