# Comparing `tmp/evosax-0.1.3.tar.gz` & `tmp/evosax-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evosax-0.1.3.tar", last modified: Tue Mar 14 08:37:19 2023, max compression
+gzip compressed data, was "evosax-0.1.4.tar", last modified: Tue Apr 11 14:56:36 2023, max compression
```

## Comparing `evosax-0.1.3.tar` & `evosax-0.1.4.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:37:19.541726 evosax-0.1.3/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10238 2023-03-14 08:37:09.000000 evosax-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-14 08:37:09.000000 evosax-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    24877 2023-03-14 08:37:19.541726 evosax-0.1.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    24177 2023-03-14 08:37:09.000000 evosax-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:37:19.533726 evosax-0.1.3/evosax/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:37:19.537726 evosax-0.1.3/evosax/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/networks/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/networks/lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/networks/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/networks/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:37:19.537726 evosax-0.1.3/evosax/problems/
--rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19031 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/problems/bbob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/problems/bbob_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/problems/control_gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/problems/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/problems/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:37:19.537726 evosax-0.1.3/evosax/restarts/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/restarts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/restarts/bipop_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/restarts/ipop_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/restarts/restarter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/restarts/simple_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/restarts/termination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:37:19.541726 evosax-0.1.3/evosax/strategies/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1407 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/ars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/asebo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/bipop_cma_es.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:37:19.541726 evosax-0.1.3/evosax/strategies/ckpt/
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/ckpt/2023_03_les_v1.pkl
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/ckpt/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10808 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/cma_es.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/cr_fm_nes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6861 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/de.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/des.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/esmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/full_iamalgam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/gesmr_ga.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/gld.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/guided_es.py
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/indep_iamalgam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/ipop_cma_es.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/les.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/lm_ma_es.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/ma_es.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/mr15_ga.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4478 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/open_es.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4285 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/pbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/persistent_es.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5990 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/pgpe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5099 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/pso.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    10169 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/rm_es.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/samr_ga.py
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/sep_cma_es.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/sim_anneal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4296 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/simple_es.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5194 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/simple_ga.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/snes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategies/xnes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5703 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:37:19.541726 evosax-0.1.3/evosax/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/utils/eigen_decomp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5029 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/utils/es_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/utils/evojax_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/utils/learned_eo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10025 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/utils/optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2828 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/utils/reshape_fitness.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3489 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/utils/reshape_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-03-14 08:37:09.000000 evosax-0.1.3/evosax/utils/visualizer_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:37:19.537726 evosax-0.1.3/evosax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24877 2023-03-14 08:37:19.000000 evosax-0.1.3/evosax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-14 08:37:19.000000 evosax-0.1.3/evosax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 08:37:19.000000 evosax-0.1.3/evosax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 08:37:19.000000 evosax-0.1.3/evosax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-14 08:37:19.000000 evosax-0.1.3/evosax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-14 08:37:19.000000 evosax-0.1.3/evosax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 08:37:19.541726 evosax-0.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2027 2023-03-14 08:37:09.000000 evosax-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:56:36.880170 evosax-0.1.4/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10238 2023-04-11 14:56:20.000000 evosax-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-11 14:56:20.000000 evosax-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25599 2023-04-11 14:56:36.880170 evosax-0.1.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24899 2023-04-11 14:56:20.000000 evosax-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:56:36.872170 evosax-0.1.4/evosax/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2089 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:56:36.872170 evosax-0.1.4/evosax/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/networks/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/networks/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/networks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/networks/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:56:36.876170 evosax-0.1.4/evosax/problems/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19109 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/problems/bbob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/problems/bbob_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/problems/control_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/problems/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/problems/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:56:36.876170 evosax-0.1.4/evosax/restarts/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/restarts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/restarts/bipop_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/restarts/ipop_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/restarts/restarter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/restarts/simple_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/restarts/termination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:56:36.880170 evosax-0.1.4/evosax/strategies/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/ars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/asebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/bipop_cma_es.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:56:36.880170 evosax-0.1.4/evosax/strategies/ckpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/ckpt/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11131 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/cma_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/cr_fm_nes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7001 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/de.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/des.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/esmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/full_iamalgam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/gesmr_ga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/gld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/guided_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/indep_iamalgam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/ipop_cma_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/les.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/lga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/lm_ma_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/ma_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/mr15_ga.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4590 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/open_es.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4417 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/pbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/persistent_es.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6102 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/pgpe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5218 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/pso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/rm_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/samr_ga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/sep_cma_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/sim_anneal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4408 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/simple_es.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5313 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/simple_ga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/snes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategies/xnes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6098 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:56:36.880170 evosax-0.1.4/evosax/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/utils/eigen_decomp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5622 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/utils/es_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/utils/evojax_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/utils/les_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/utils/lga_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10025 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/utils/optimizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2828 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/utils/reshape_fitness.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3700 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/utils/reshape_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-04-11 14:56:20.000000 evosax-0.1.4/evosax/utils/visualizer_2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:56:36.872170 evosax-0.1.4/evosax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25599 2023-04-11 14:56:36.000000 evosax-0.1.4/evosax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-11 14:56:36.000000 evosax-0.1.4/evosax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:56:36.000000 evosax-0.1.4/evosax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:56:36.000000 evosax-0.1.4/evosax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-11 14:56:36.000000 evosax-0.1.4/evosax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 14:56:36.000000 evosax-0.1.4/evosax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 14:56:36.880170 evosax-0.1.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2049 2023-04-11 14:56:20.000000 evosax-0.1.4/setup.py
```

### Comparing `evosax-0.1.3/LICENSE` & `evosax-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/PKG-INFO` & `evosax-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: evosax
-Version: 0.1.3
+Version: 0.1.4
 Summary: JAX-Based Evolution Strategies
 Home-page: https://github.com/RobertTLange/evosax
-Download-URL: https://github.com/RobertTLange/evosax/archive/v0.1.3.tar.gz
+Download-URL: https://github.com/RobertTLange/evosax/archive/v0.1.4.tar.gz
 Author: Robert Tjarko Lange
 Author-email: robertlange0@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -49,22 +49,22 @@
 state.best_member, state.best_fitness
 ```
 
 ## Implemented Evolution Strategies 🦎
 
 | Strategy | Reference | Import | Example |
 | --- | --- | ---  | --- |
-| OpenES | [Salimans et al. (2017)](https://arxiv.org/pdf/1703.03864.pdf) | [`OpenES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/open_es.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/03_cnn_mnist.ipynb)
+| OpenAI-ES | [Salimans et al. (2017)](https://arxiv.org/pdf/1703.03864.pdf) | [`OpenES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/open_es.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/03_cnn_mnist.ipynb)
 | PGPE | [Sehnke et al. (2010)](https://citeseerx.ist.psu.edu/viewdoc/download;jsessionid=A64D1AE8313A364B814998E9E245B40A?doi=10.1.1.180.7104&rep=rep1&type=pdf) | [`PGPE`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/pgpe.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/02_mlp_control.ipynb)
 | ARS | [Mania et al. (2018)](https://arxiv.org/pdf/1803.07055.pdf) | [`ARS`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/ars.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/00_getting_started.ipynb)
 | ESMC | [Merchant et al. (2021)](https://proceedings.mlr.press/v139/merchant21a.html) | [`ESMC`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/esmc.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Persistent ES | [Vicol et al. (2021)](http://proceedings.mlr.press/v139/vicol21a.html) | [`PersistentES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/persistent_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/04_lrate_pes.ipynb)
 | xNES | [Wierstra et al. (2014)](https://www.jmlr.org/papers/volume15/wierstra14a/wierstra14a.pdf) | [`XNES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/xnes.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | SNES | [Wierstra et al. (2014)](https://www.jmlr.org/papers/volume15/wierstra14a/wierstra14a.pdf) | [`SNES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/sxnes.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
-| CR-FM-NES | [Nomura & Ono (2022)](https://arxiv.org/abs/2201.11422) | [`CR-FM-NES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/cr_fm_nes.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
+| CR-FM-NES | [Nomura & Ono (2022)](https://arxiv.org/abs/2201.11422) | [`CR_FM_NES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/cr_fm_nes.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Guided ES | [Maheswaranathan et al. (2018)](https://arxiv.org/abs/1806.10230) | [`GuidedES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/guided_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | ASEBO | [Choromanski et al. (2019)](https://arxiv.org/abs/1903.04268) | [`ASEBO`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/asebo.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | CMA-ES | [Hansen & Ostermeier (2001)](http://www.cmap.polytechnique.fr/~nikolaus.hansen/cmaartic.pdf) | [`CMA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/cma_es.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Sep-CMA-ES | [Ros & Hansen (2008)](https://hal.inria.fr/inria-00287367/document) | [`Sep_CMA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/sep_cma_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | BIPOP-CMA-ES | [Hansen (2009)](https://hal.inria.fr/inria-00382093/document) | [`BIPOP_CMA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/bipop_cma_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/06_restart_es.ipynb)
 | IPOP-CMA-ES | [Auer & Hansen (2005)](http://www.cmap.polytechnique.fr/~nikolaus.hansen/cec2005ipopcmaes.pdf) | [`IPOP_CMA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/ipop_cma_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/06_restart_es.ipynb)
 | Full-iAMaLGaM | [Bosman et al. (2013)](https://tinyurl.com/y9fcccx2) | [`Full_iAMaLGaM`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/full_iamalgam.py)  |[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
@@ -72,23 +72,24 @@
 | MA-ES | [Bayer & Sendhoff (2017)](https://www.honda-ri.de/pubs/pdf/3376.pdf) | [`MA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/ma_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | LM-MA-ES | [Loshchilov et al. (2017)](https://arxiv.org/pdf/1705.06693.pdf) | [`LM_MA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/lm_ma_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | RmES | [Li & Zhang (2017)](https://ieeexplore.ieee.org/document/8080257) | [`RmES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/rm_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Simple Genetic | [Such et al. (2017)](https://arxiv.org/abs/1712.06567) | [`SimpleGA`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/simple_ga.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | SAMR-GA | [Clune et al. (2008)](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1000187) | [`SAMR_GA`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/samr_ga.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | GESMR-GA | [Kumar et al. (2022)](https://arxiv.org/abs/2204.04817) | [`GESMR_GA`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/gesmr_ga.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | MR15-GA | [Rechenberg (1978)](https://link.springer.com/chapter/10.1007/978-3-642-81283-5_8) | [`MR15_GA`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/mr15_ga.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
+| LGA | [Lange et al. (2023b)](https://arxiv.org/abs/2304.03995) | [`LGA`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/lga.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Simple Gaussian | [Rechenberg (1978)](https://link.springer.com/chapter/10.1007/978-3-642-81283-5_8) | [`SimpleES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/simple_es.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
-| DES | [Lange et al. (2023)](https://arxiv.org/abs/2211.11260) | [`DES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/des.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
-| LES | [Lange et al. (2023)](https://arxiv.org/abs/2211.11260) | [`LES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/les.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
+| DES | [Lange et al. (2023a)](https://arxiv.org/abs/2211.11260) | [`DES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/des.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
+| LES | [Lange et al. (202a3)](https://arxiv.org/abs/2211.11260) | [`LES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/les.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Particle Swarm Optimization | [Kennedy & Eberhart (1995)](https://ieeexplore.ieee.org/document/488968) | [`PSO`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/pso.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Differential Evolution | [Storn & Price (1997)](https://www.metabolic-economics.de/pages/seminar_theoretische_biologie_2007/literatur/schaber/Storn1997JGlobOpt11.pdf) | [`DE`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/de.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | GLD | [Golovin et al. (2019)](https://arxiv.org/pdf/1911.06317.pdf) | [`GLD`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/gld.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Simulated Annealing | [Rasdi Rere et al. (2015)](https://www.sciencedirect.com/science/article/pii/S1877050915035759) | [`SimAnneal`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/sim_anneal.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Population-Based Training | [Jaderberg et al. (2017)](https://arxiv.org/abs/1711.09846) | [`PBT`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/pbt.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/05_quadratic_pbt.ipynb)
-
+| Random Search | [Bergstra & Bengio (2012)](https://www.jmlr.org/papers/volume13/bergstra12a/bergstra12a.pdf) | [`RandomSearch`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/random.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 
 
 
 
 ## Installation ⏳
 
 The latest `evosax` release can directly be installed from PyPI:
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: evosax Version: 0.1.3 Summary: JAX-Based Evolution
+Metadata-Version: 2.1 Name: evosax Version: 0.1.4 Summary: JAX-Based Evolution
 Strategies Home-page: https://github.com/RobertTLange/evosax Download-URL:
-https://github.com/RobertTLange/evosax/archive/v0.1.3.tar.gz Author: Robert
+https://github.com/RobertTLange/evosax/archive/v0.1.4.tar.gz Author: Robert
 Tjarko Lange Author-email: robertlange0@gmail.com Platform: any Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE # `evosax`: JAX-Based Evolution Strategies ð¦ [!
@@ -34,15 +34,15 @@
 strategy.initialize(rng, es_params) # Run ask-eval-tell loop - NOTE: By default
 minimization! for t in range(num_generations): rng, rng_gen, rng_eval =
 jax.random.split(rng, 3) x, state = strategy.ask(rng_gen, state, es_params)
 fitness = ... # Your population evaluation fct state = strategy.tell(x,
 fitness, state, es_params) # Get best overall population member & its fitness
 state.best_member, state.best_fitness ``` ## Implemented Evolution Strategies
 ð¦ | Strategy | Reference | Import | Example | | --- | --- | --- | --- | |
-OpenES | [Salimans et al. (2017)](https://arxiv.org/pdf/1703.03864.pdf) |
+OpenAI-ES | [Salimans et al. (2017)](https://arxiv.org/pdf/1703.03864.pdf) |
 [`OpenES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/
 open_es.py) | [![Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/
 main/examples/03_cnn_mnist.ipynb) | PGPE | [Sehnke et al. (2010)](https://
 citeseerx.ist.psu.edu/viewdoc/
 download;jsessionid=A64D1AE8313A364B814998E9E245B40A?doi=10.1.1.180.7104&rep=rep1&type=pdf)
 | [`PGPE`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/
@@ -69,15 +69,15 @@
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
 01_classic_benchmark.ipynb) | SNES | [Wierstra et al. (2014)](https://
 www.jmlr.org/papers/volume15/wierstra14a/wierstra14a.pdf) | [`SNES`](https://
 github.com/RobertTLange/evosax/tree/main/evosax/strategies/sxnes.py) | [!
 [Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
 01_classic_benchmark.ipynb) | CR-FM-NES | [Nomura & Ono (2022)](https://
-arxiv.org/abs/2201.11422) | [`CR-FM-NES`](https://github.com/RobertTLange/
+arxiv.org/abs/2201.11422) | [`CR_FM_NES`](https://github.com/RobertTLange/
 evosax/tree/main/evosax/strategies/cr_fm_nes.py) | [![Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
 01_classic_benchmark.ipynb) | Guided ES | [Maheswaranathan et al. (2018)]
 (https://arxiv.org/abs/1806.10230) | [`GuidedES`](https://github.com/
 RobertTLange/evosax/tree/main/evosax/strategies/guided_es.py) | [![Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
@@ -148,55 +148,64 @@
 //colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
 01_classic_benchmark.ipynb) | MR15-GA | [Rechenberg (1978)](https://
 link.springer.com/chapter/10.1007/978-3-642-81283-5_8) | [`MR15_GA`](https://
 github.com/RobertTLange/evosax/tree/main/evosax/strategies/mr15_ga.py) | [!
 [Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | Simple Gaussian | [Rechenberg (1978)](https://
-link.springer.com/chapter/10.1007/978-3-642-81283-5_8) | [`SimpleES`](https://
-github.com/RobertTLange/evosax/tree/main/evosax/strategies/simple_es.py) | [!
-[Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | DES | [Lange et al. (2023)](https://arxiv.org/
-abs/2211.11260) | [`DES`](https://github.com/RobertTLange/evosax/tree/main/
-evosax/strategies/des.py) | [![Colab](https://colab.research.google.com/assets/
+01_classic_benchmark.ipynb) | LGA | [Lange et al. (2023b)](https://arxiv.org/
+abs/2304.03995) | [`LGA`](https://github.com/RobertTLange/evosax/tree/main/
+evosax/strategies/lga.py) | [![Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/
+blob/main/examples/01_classic_benchmark.ipynb) | Simple Gaussian | [Rechenberg
+(1978)](https://link.springer.com/chapter/10.1007/978-3-642-81283-5_8) |
+[`SimpleES`](https://github.com/RobertTLange/evosax/tree/main/evosax/
+strategies/simple_es.py) | [![Colab](https://colab.research.google.com/assets/
 colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/
-blob/main/examples/01_classic_benchmark.ipynb) | LES | [Lange et al. (2023)]
-(https://arxiv.org/abs/2211.11260) | [`LES`](https://github.com/RobertTLange/
-evosax/tree/main/evosax/strategies/les.py) | [![Colab](https://
+blob/main/examples/01_classic_benchmark.ipynb) | DES | [Lange et al. (2023a)]
+(https://arxiv.org/abs/2211.11260) | [`DES`](https://github.com/RobertTLange/
+evosax/tree/main/evosax/strategies/des.py) | [![Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | Particle Swarm Optimization | [Kennedy & Eberhart
-(1995)](https://ieeexplore.ieee.org/document/488968) | [`PSO`](https://
-github.com/RobertTLange/evosax/tree/main/evosax/strategies/pso.py) | [![Colab]
-(https://colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | Differential Evolution | [Storn & Price (1997)]
-(https://www.metabolic-economics.de/pages/seminar_theoretische_biologie_2007/
-literatur/schaber/Storn1997JGlobOpt11.pdf) | [`DE`](https://github.com/
-RobertTLange/evosax/tree/main/evosax/strategies/de.py) | [![Colab](https://
+01_classic_benchmark.ipynb) | LES | [Lange et al. (202a3)](https://arxiv.org/
+abs/2211.11260) | [`LES`](https://github.com/RobertTLange/evosax/tree/main/
+evosax/strategies/les.py) | [![Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/
+blob/main/examples/01_classic_benchmark.ipynb) | Particle Swarm Optimization |
+[Kennedy & Eberhart (1995)](https://ieeexplore.ieee.org/document/488968) |
+[`PSO`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/
+pso.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/github/RobertTLange/evosax/blob/main/
+examples/01_classic_benchmark.ipynb) | Differential Evolution | [Storn & Price
+(1997)](https://www.metabolic-economics.de/pages/
+seminar_theoretische_biologie_2007/literatur/schaber/Storn1997JGlobOpt11.pdf) |
+[`DE`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/
+de.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/github/RobertTLange/evosax/blob/main/
+examples/01_classic_benchmark.ipynb) | GLD | [Golovin et al. (2019)](https://
+arxiv.org/pdf/1911.06317.pdf) | [`GLD`](https://github.com/RobertTLange/evosax/
+tree/main/evosax/strategies/gld.py) | [![Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | GLD | [Golovin et al. (2019)](https://arxiv.org/
-pdf/1911.06317.pdf) | [`GLD`](https://github.com/RobertTLange/evosax/tree/main/
-evosax/strategies/gld.py) | [![Colab](https://colab.research.google.com/assets/
+01_classic_benchmark.ipynb) | Simulated Annealing | [Rasdi Rere et al. (2015)]
+(https://www.sciencedirect.com/science/article/pii/S1877050915035759) |
+[`SimAnneal`](https://github.com/RobertTLange/evosax/tree/main/evosax/
+strategies/sim_anneal.py) | [![Colab](https://colab.research.google.com/assets/
 colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/
-blob/main/examples/01_classic_benchmark.ipynb) | Simulated Annealing | [Rasdi
-Rere et al. (2015)](https://www.sciencedirect.com/science/article/pii/
-S1877050915035759) | [`SimAnneal`](https://github.com/RobertTLange/evosax/tree/
-main/evosax/strategies/sim_anneal.py) | [![Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
+blob/main/examples/01_classic_benchmark.ipynb) | Population-Based Training |
+[Jaderberg et al. (2017)](https://arxiv.org/abs/1711.09846) | [`PBT`](https://
+github.com/RobertTLange/evosax/tree/main/evosax/strategies/pbt.py) | [![Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | Population-Based Training | [Jaderberg et al.
-(2017)](https://arxiv.org/abs/1711.09846) | [`PBT`](https://github.com/
-RobertTLange/evosax/tree/main/evosax/strategies/pbt.py) | [![Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
+05_quadratic_pbt.ipynb) | Random Search | [Bergstra & Bengio (2012)](https://
+www.jmlr.org/papers/volume13/bergstra12a/bergstra12a.pdf) | [`RandomSearch`]
+(https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/random.py)
+| [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-05_quadratic_pbt.ipynb) ## Installation â³ The latest `evosax` release can
+01_classic_benchmark.ipynb) ## Installation â³ The latest `evosax` release can
 directly be installed from PyPI: ``` pip install evosax ``` If you want to get
 the most recent commit, please install directly from the repository: ``` pip
 install git+https://github.com/RobertTLange/evosax.git@main ``` In order to use
 JAX on your accelerators, you can find more details in the [JAX documentation]
 (https://github.com/google/jax#installation). ## Examples ð * ð [Classic
 ES Tasks](https://github.com/RobertTLange/evosax/blob/main/examples/
 01_classic_benchmark.ipynb): API introduction on Rosenbrock function (CMA-ES,
```

### Comparing `evosax-0.1.3/README.md` & `evosax-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,22 @@
 state.best_member, state.best_fitness
 ```
 
 ## Implemented Evolution Strategies 🦎
 
 | Strategy | Reference | Import | Example |
 | --- | --- | ---  | --- |
-| OpenES | [Salimans et al. (2017)](https://arxiv.org/pdf/1703.03864.pdf) | [`OpenES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/open_es.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/03_cnn_mnist.ipynb)
+| OpenAI-ES | [Salimans et al. (2017)](https://arxiv.org/pdf/1703.03864.pdf) | [`OpenES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/open_es.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/03_cnn_mnist.ipynb)
 | PGPE | [Sehnke et al. (2010)](https://citeseerx.ist.psu.edu/viewdoc/download;jsessionid=A64D1AE8313A364B814998E9E245B40A?doi=10.1.1.180.7104&rep=rep1&type=pdf) | [`PGPE`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/pgpe.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/02_mlp_control.ipynb)
 | ARS | [Mania et al. (2018)](https://arxiv.org/pdf/1803.07055.pdf) | [`ARS`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/ars.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/00_getting_started.ipynb)
 | ESMC | [Merchant et al. (2021)](https://proceedings.mlr.press/v139/merchant21a.html) | [`ESMC`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/esmc.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Persistent ES | [Vicol et al. (2021)](http://proceedings.mlr.press/v139/vicol21a.html) | [`PersistentES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/persistent_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/04_lrate_pes.ipynb)
 | xNES | [Wierstra et al. (2014)](https://www.jmlr.org/papers/volume15/wierstra14a/wierstra14a.pdf) | [`XNES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/xnes.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | SNES | [Wierstra et al. (2014)](https://www.jmlr.org/papers/volume15/wierstra14a/wierstra14a.pdf) | [`SNES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/sxnes.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
-| CR-FM-NES | [Nomura & Ono (2022)](https://arxiv.org/abs/2201.11422) | [`CR-FM-NES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/cr_fm_nes.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
+| CR-FM-NES | [Nomura & Ono (2022)](https://arxiv.org/abs/2201.11422) | [`CR_FM_NES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/cr_fm_nes.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Guided ES | [Maheswaranathan et al. (2018)](https://arxiv.org/abs/1806.10230) | [`GuidedES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/guided_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | ASEBO | [Choromanski et al. (2019)](https://arxiv.org/abs/1903.04268) | [`ASEBO`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/asebo.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | CMA-ES | [Hansen & Ostermeier (2001)](http://www.cmap.polytechnique.fr/~nikolaus.hansen/cmaartic.pdf) | [`CMA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/cma_es.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Sep-CMA-ES | [Ros & Hansen (2008)](https://hal.inria.fr/inria-00287367/document) | [`Sep_CMA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/sep_cma_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | BIPOP-CMA-ES | [Hansen (2009)](https://hal.inria.fr/inria-00382093/document) | [`BIPOP_CMA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/bipop_cma_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/06_restart_es.ipynb)
 | IPOP-CMA-ES | [Auer & Hansen (2005)](http://www.cmap.polytechnique.fr/~nikolaus.hansen/cec2005ipopcmaes.pdf) | [`IPOP_CMA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/ipop_cma_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/06_restart_es.ipynb)
 | Full-iAMaLGaM | [Bosman et al. (2013)](https://tinyurl.com/y9fcccx2) | [`Full_iAMaLGaM`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/full_iamalgam.py)  |[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
@@ -53,23 +53,24 @@
 | MA-ES | [Bayer & Sendhoff (2017)](https://www.honda-ri.de/pubs/pdf/3376.pdf) | [`MA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/ma_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | LM-MA-ES | [Loshchilov et al. (2017)](https://arxiv.org/pdf/1705.06693.pdf) | [`LM_MA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/lm_ma_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | RmES | [Li & Zhang (2017)](https://ieeexplore.ieee.org/document/8080257) | [`RmES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/rm_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Simple Genetic | [Such et al. (2017)](https://arxiv.org/abs/1712.06567) | [`SimpleGA`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/simple_ga.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | SAMR-GA | [Clune et al. (2008)](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1000187) | [`SAMR_GA`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/samr_ga.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | GESMR-GA | [Kumar et al. (2022)](https://arxiv.org/abs/2204.04817) | [`GESMR_GA`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/gesmr_ga.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | MR15-GA | [Rechenberg (1978)](https://link.springer.com/chapter/10.1007/978-3-642-81283-5_8) | [`MR15_GA`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/mr15_ga.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
+| LGA | [Lange et al. (2023b)](https://arxiv.org/abs/2304.03995) | [`LGA`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/lga.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Simple Gaussian | [Rechenberg (1978)](https://link.springer.com/chapter/10.1007/978-3-642-81283-5_8) | [`SimpleES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/simple_es.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
-| DES | [Lange et al. (2023)](https://arxiv.org/abs/2211.11260) | [`DES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/des.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
-| LES | [Lange et al. (2023)](https://arxiv.org/abs/2211.11260) | [`LES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/les.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
+| DES | [Lange et al. (2023a)](https://arxiv.org/abs/2211.11260) | [`DES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/des.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
+| LES | [Lange et al. (202a3)](https://arxiv.org/abs/2211.11260) | [`LES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/les.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Particle Swarm Optimization | [Kennedy & Eberhart (1995)](https://ieeexplore.ieee.org/document/488968) | [`PSO`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/pso.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Differential Evolution | [Storn & Price (1997)](https://www.metabolic-economics.de/pages/seminar_theoretische_biologie_2007/literatur/schaber/Storn1997JGlobOpt11.pdf) | [`DE`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/de.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | GLD | [Golovin et al. (2019)](https://arxiv.org/pdf/1911.06317.pdf) | [`GLD`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/gld.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Simulated Annealing | [Rasdi Rere et al. (2015)](https://www.sciencedirect.com/science/article/pii/S1877050915035759) | [`SimAnneal`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/sim_anneal.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Population-Based Training | [Jaderberg et al. (2017)](https://arxiv.org/abs/1711.09846) | [`PBT`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/pbt.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/05_quadratic_pbt.ipynb)
-
+| Random Search | [Bergstra & Bengio (2012)](https://www.jmlr.org/papers/volume13/bergstra12a/bergstra12a.pdf) | [`RandomSearch`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/random.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 
 
 
 
 ## Installation ⏳
 
 The latest `evosax` release can directly be installed from PyPI:
```

#### html2text {}

```diff
@@ -25,15 +25,15 @@
 strategy.initialize(rng, es_params) # Run ask-eval-tell loop - NOTE: By default
 minimization! for t in range(num_generations): rng, rng_gen, rng_eval =
 jax.random.split(rng, 3) x, state = strategy.ask(rng_gen, state, es_params)
 fitness = ... # Your population evaluation fct state = strategy.tell(x,
 fitness, state, es_params) # Get best overall population member & its fitness
 state.best_member, state.best_fitness ``` ## Implemented Evolution Strategies
 ð¦ | Strategy | Reference | Import | Example | | --- | --- | --- | --- | |
-OpenES | [Salimans et al. (2017)](https://arxiv.org/pdf/1703.03864.pdf) |
+OpenAI-ES | [Salimans et al. (2017)](https://arxiv.org/pdf/1703.03864.pdf) |
 [`OpenES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/
 open_es.py) | [![Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/
 main/examples/03_cnn_mnist.ipynb) | PGPE | [Sehnke et al. (2010)](https://
 citeseerx.ist.psu.edu/viewdoc/
 download;jsessionid=A64D1AE8313A364B814998E9E245B40A?doi=10.1.1.180.7104&rep=rep1&type=pdf)
 | [`PGPE`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/
@@ -60,15 +60,15 @@
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
 01_classic_benchmark.ipynb) | SNES | [Wierstra et al. (2014)](https://
 www.jmlr.org/papers/volume15/wierstra14a/wierstra14a.pdf) | [`SNES`](https://
 github.com/RobertTLange/evosax/tree/main/evosax/strategies/sxnes.py) | [!
 [Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
 01_classic_benchmark.ipynb) | CR-FM-NES | [Nomura & Ono (2022)](https://
-arxiv.org/abs/2201.11422) | [`CR-FM-NES`](https://github.com/RobertTLange/
+arxiv.org/abs/2201.11422) | [`CR_FM_NES`](https://github.com/RobertTLange/
 evosax/tree/main/evosax/strategies/cr_fm_nes.py) | [![Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
 01_classic_benchmark.ipynb) | Guided ES | [Maheswaranathan et al. (2018)]
 (https://arxiv.org/abs/1806.10230) | [`GuidedES`](https://github.com/
 RobertTLange/evosax/tree/main/evosax/strategies/guided_es.py) | [![Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
@@ -139,55 +139,64 @@
 //colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
 01_classic_benchmark.ipynb) | MR15-GA | [Rechenberg (1978)](https://
 link.springer.com/chapter/10.1007/978-3-642-81283-5_8) | [`MR15_GA`](https://
 github.com/RobertTLange/evosax/tree/main/evosax/strategies/mr15_ga.py) | [!
 [Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | Simple Gaussian | [Rechenberg (1978)](https://
-link.springer.com/chapter/10.1007/978-3-642-81283-5_8) | [`SimpleES`](https://
-github.com/RobertTLange/evosax/tree/main/evosax/strategies/simple_es.py) | [!
-[Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | DES | [Lange et al. (2023)](https://arxiv.org/
-abs/2211.11260) | [`DES`](https://github.com/RobertTLange/evosax/tree/main/
-evosax/strategies/des.py) | [![Colab](https://colab.research.google.com/assets/
+01_classic_benchmark.ipynb) | LGA | [Lange et al. (2023b)](https://arxiv.org/
+abs/2304.03995) | [`LGA`](https://github.com/RobertTLange/evosax/tree/main/
+evosax/strategies/lga.py) | [![Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/
+blob/main/examples/01_classic_benchmark.ipynb) | Simple Gaussian | [Rechenberg
+(1978)](https://link.springer.com/chapter/10.1007/978-3-642-81283-5_8) |
+[`SimpleES`](https://github.com/RobertTLange/evosax/tree/main/evosax/
+strategies/simple_es.py) | [![Colab](https://colab.research.google.com/assets/
 colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/
-blob/main/examples/01_classic_benchmark.ipynb) | LES | [Lange et al. (2023)]
-(https://arxiv.org/abs/2211.11260) | [`LES`](https://github.com/RobertTLange/
-evosax/tree/main/evosax/strategies/les.py) | [![Colab](https://
+blob/main/examples/01_classic_benchmark.ipynb) | DES | [Lange et al. (2023a)]
+(https://arxiv.org/abs/2211.11260) | [`DES`](https://github.com/RobertTLange/
+evosax/tree/main/evosax/strategies/des.py) | [![Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | Particle Swarm Optimization | [Kennedy & Eberhart
-(1995)](https://ieeexplore.ieee.org/document/488968) | [`PSO`](https://
-github.com/RobertTLange/evosax/tree/main/evosax/strategies/pso.py) | [![Colab]
-(https://colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | Differential Evolution | [Storn & Price (1997)]
-(https://www.metabolic-economics.de/pages/seminar_theoretische_biologie_2007/
-literatur/schaber/Storn1997JGlobOpt11.pdf) | [`DE`](https://github.com/
-RobertTLange/evosax/tree/main/evosax/strategies/de.py) | [![Colab](https://
+01_classic_benchmark.ipynb) | LES | [Lange et al. (202a3)](https://arxiv.org/
+abs/2211.11260) | [`LES`](https://github.com/RobertTLange/evosax/tree/main/
+evosax/strategies/les.py) | [![Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/
+blob/main/examples/01_classic_benchmark.ipynb) | Particle Swarm Optimization |
+[Kennedy & Eberhart (1995)](https://ieeexplore.ieee.org/document/488968) |
+[`PSO`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/
+pso.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/github/RobertTLange/evosax/blob/main/
+examples/01_classic_benchmark.ipynb) | Differential Evolution | [Storn & Price
+(1997)](https://www.metabolic-economics.de/pages/
+seminar_theoretische_biologie_2007/literatur/schaber/Storn1997JGlobOpt11.pdf) |
+[`DE`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/
+de.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/github/RobertTLange/evosax/blob/main/
+examples/01_classic_benchmark.ipynb) | GLD | [Golovin et al. (2019)](https://
+arxiv.org/pdf/1911.06317.pdf) | [`GLD`](https://github.com/RobertTLange/evosax/
+tree/main/evosax/strategies/gld.py) | [![Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | GLD | [Golovin et al. (2019)](https://arxiv.org/
-pdf/1911.06317.pdf) | [`GLD`](https://github.com/RobertTLange/evosax/tree/main/
-evosax/strategies/gld.py) | [![Colab](https://colab.research.google.com/assets/
+01_classic_benchmark.ipynb) | Simulated Annealing | [Rasdi Rere et al. (2015)]
+(https://www.sciencedirect.com/science/article/pii/S1877050915035759) |
+[`SimAnneal`](https://github.com/RobertTLange/evosax/tree/main/evosax/
+strategies/sim_anneal.py) | [![Colab](https://colab.research.google.com/assets/
 colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/
-blob/main/examples/01_classic_benchmark.ipynb) | Simulated Annealing | [Rasdi
-Rere et al. (2015)](https://www.sciencedirect.com/science/article/pii/
-S1877050915035759) | [`SimAnneal`](https://github.com/RobertTLange/evosax/tree/
-main/evosax/strategies/sim_anneal.py) | [![Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
+blob/main/examples/01_classic_benchmark.ipynb) | Population-Based Training |
+[Jaderberg et al. (2017)](https://arxiv.org/abs/1711.09846) | [`PBT`](https://
+github.com/RobertTLange/evosax/tree/main/evosax/strategies/pbt.py) | [![Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | Population-Based Training | [Jaderberg et al.
-(2017)](https://arxiv.org/abs/1711.09846) | [`PBT`](https://github.com/
-RobertTLange/evosax/tree/main/evosax/strategies/pbt.py) | [![Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
+05_quadratic_pbt.ipynb) | Random Search | [Bergstra & Bengio (2012)](https://
+www.jmlr.org/papers/volume13/bergstra12a/bergstra12a.pdf) | [`RandomSearch`]
+(https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/random.py)
+| [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-05_quadratic_pbt.ipynb) ## Installation â³ The latest `evosax` release can
+01_classic_benchmark.ipynb) ## Installation â³ The latest `evosax` release can
 directly be installed from PyPI: ``` pip install evosax ``` If you want to get
 the most recent commit, please install directly from the repository: ``` pip
 install git+https://github.com/RobertTLange/evosax.git@main ``` In order to use
 JAX on your accelerators, you can find more details in the [JAX documentation]
 (https://github.com/google/jax#installation). ## Examples ð * ð [Classic
 ES Tasks](https://github.com/RobertTLange/evosax/blob/main/examples/
 01_classic_benchmark.ipynb): API introduction on Rosenbrock function (CMA-ES,
```

### Comparing `evosax-0.1.3/evosax/__init__.py` & `evosax-0.1.4/evosax/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     GESMR_GA,
     GuidedES,
     ASEBO,
     CR_FM_NES,
     MR15_GA,
     RandomSearch,
     LES,
+    LGA,
 )
 from .utils import FitnessShaper, ParameterReshaper, ESLog
 from .networks import NetworkMapper
 from .problems import ProblemMapper
 
 
 Strategies = {
@@ -67,14 +68,15 @@
     "GESMR_GA": GESMR_GA,
     "GuidedES": GuidedES,
     "ASEBO": ASEBO,
     "CR_FM_NES": CR_FM_NES,
     "MR15_GA": MR15_GA,
     "RandomSearch": RandomSearch,
     "LES": LES,
+    "LGA": LGA,
 }
 
 __all__ = [
     "Strategies",
     "EvoState",
     "EvoParams",
     "FitnessShaper",
@@ -111,8 +113,9 @@
     "GESMR_GA",
     "GuidedES",
     "ASEBO",
     "CR_FM_NES",
     "MR15_GA",
     "RandomSearch",
     "LES",
+    "LGA",
 ]
```

### Comparing `evosax-0.1.3/evosax/networks/cnn.py` & `evosax-0.1.4/evosax/networks/cnn.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/networks/lstm.py` & `evosax-0.1.4/evosax/networks/lstm.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/networks/mlp.py` & `evosax-0.1.4/evosax/networks/mlp.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/networks/shared.py` & `evosax-0.1.4/evosax/networks/shared.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/problems/bbob.py` & `evosax-0.1.4/evosax/problems/bbob.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,18 @@
     """BBOB Functions Benchmark Task.
     Functions from Hansen et al. (2009)
     'Real-parameter black-box optimization benchmarking 2009: Noiseless functions definitions'
     Link: https://numbbo.github.io/gforge/downloads/download16.00/bbobdocfunctions.pdf
     """
 
     def __init__(
-        self, fn_name: str = "Sphere", num_dims: int = 2, seed_id: int = 1
+        self,
+        fn_name: str = "Sphere",
+        num_dims: int = 2,
+        seed_id: int = 1,
     ):
         self.num_dims = num_dims
         # Create rotation matrices for non-separability
         rng = jax.random.PRNGKey(seed_id)
         self.seed_id = seed_id
         self.R, self.Q = self.get_rotation_matrices(rng)
         self.fn_name = fn_name
@@ -35,22 +38,22 @@
     @partial(jax.jit, static_argnums=(0,))
     def rollout(
         self,
         rng: chex.PRNGKey,
         eval_params: chex.Array,
         R: Optional[chex.Array] = None,
         Q: Optional[chex.Array] = None,
+        noise_std: float = 0.0,
     ) -> chex.Array:
         """Batch evaluate the proposal points."""
         if R is None:
-            R, Q = self.get_rotation_matrices(rng)
-        else:
             R, Q = self.R, self.Q
         val = jax.vmap(self.fn, in_axes=(0, None, None))(eval_params, R, Q)
-        return val
+        eval_noise = jax.random.normal(rng, shape=val.shape) * noise_std
+        return val + eval_noise
 
     def get_rotation_matrices(self, rng: chex.PRNGKey):
         """Sample two rotation matrices."""
         rng_q, rng_r = jax.random.split(rng)
         R = get_rotation(rng_r, self.num_dims)
         Q = get_rotation(rng_q, self.num_dims)
         return R, Q
```

### Comparing `evosax-0.1.3/evosax/problems/bbob_helpers.py` & `evosax-0.1.4/evosax/problems/bbob_helpers.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/problems/control_gym.py` & `evosax-0.1.4/evosax/problems/control_gym.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/problems/sequence.py` & `evosax-0.1.4/evosax/problems/sequence.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/problems/vision.py` & `evosax-0.1.4/evosax/problems/vision.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/restarts/bipop_restart.py` & `evosax-0.1.4/evosax/restarts/bipop_restart.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/restarts/ipop_restart.py` & `evosax-0.1.4/evosax/restarts/ipop_restart.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/restarts/restarter.py` & `evosax-0.1.4/evosax/restarts/restarter.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/restarts/simple_restart.py` & `evosax-0.1.4/evosax/restarts/simple_restart.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/restarts/termination.py` & `evosax-0.1.4/evosax/restarts/termination.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/strategies/__init__.py` & `evosax-0.1.4/evosax/strategies/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from .gesmr_ga import GESMR_GA
 from .guided_es import GuidedES
 from .asebo import ASEBO
 from .cr_fm_nes import CR_FM_NES
 from .mr15_ga import MR15_GA
 from .random import RandomSearch
 from .les import LES
+from .lga import LGA
 
 
 __all__ = [
     "SimpleGA",
     "SimpleES",
     "CMA_ES",
     "DE",
@@ -61,8 +62,9 @@
     "GESMR_GA",
     "GuidedES",
     "ASEBO",
     "CR_FM_NES",
     "MR15_GA",
     "RandomSearch",
     "LES",
+    "LGA",
 ]
```

### Comparing `evosax-0.1.3/evosax/strategies/ars.py` & `evosax-0.1.4/evosax/strategies/ars.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,28 +32,34 @@
 class ARS(Strategy):
     def __init__(
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         elite_ratio: float = 0.1,
-        opt_name: str = "sgd",
+        opt_name: str = "adam",
         lrate_init: float = 0.05,
         lrate_decay: float = 1.0,
         lrate_limit: float = 0.001,
         sigma_init: float = 0.03,
         sigma_decay: float = 1.0,
         sigma_limit: float = 0.01,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Augmented Random Search (Mania et al., 2018)
         Reference: https://arxiv.org/pdf/1803.07055.pdf"""
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         assert not self.popsize & 1, "Population size must be even"
         # ARS performs antithetic sampling & allows you to select
         # "b" elite perturbation directions for the update
         assert 0 <= elite_ratio <= 1
         self.elite_ratio = elite_ratio
         self.elite_popsize = max(1, int(self.popsize / 2 * self.elite_ratio))
```

### Comparing `evosax-0.1.3/evosax/strategies/asebo.py` & `evosax-0.1.4/evosax/strategies/asebo.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,27 +45,29 @@
         lrate_init: float = 0.05,
         lrate_decay: float = 1.0,
         lrate_limit: float = 0.001,
         sigma_init: float = 0.03,
         sigma_decay: float = 1.0,
         sigma_limit: float = 0.01,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float],
     ):
         """ASEBO (Choromanski et al., 2019)
         Reference: https://arxiv.org/abs/1903.04268
         Note that there are a couple of JAX-based adaptations:
         1. We always sample a fixed population size per generation
         2. We keep a fixed archive of gradients to estimate the subspace
         """
         super().__init__(
             popsize,
             num_dims,
             pholder_params,
             mean_decay,
+            n_devices,
             **fitness_kwargs,
         )
         assert not self.popsize & 1, "Population size must be even"
         assert opt_name in ["sgd", "adam", "rmsprop", "clipup"]
         self.optimizer = GradientOptimizer[opt_name](self.num_dims)
         self.subspace_dims = min(subspace_dims, self.num_dims)
         if self.subspace_dims < subspace_dims:
```

### Comparing `evosax-0.1.3/evosax/strategies/bipop_cma_es.py` & `evosax-0.1.4/evosax/strategies/bipop_cma_es.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,28 +23,30 @@
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         elite_ratio: float = 0.5,
         sigma_init: float = 1.0,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """BIPOP-CMA-ES (Hansen, 2009).
         Reference: https://hal.inria.fr/inria-00382093/document
         Inspired by: https://tinyurl.com/44y3ryhf"""
         self.strategy_name = "BIPOP_CMA_ES"
         # Instantiate base strategy & wrap it with restart wrapper
         self.strategy = CMA_ES(
             num_dims=num_dims,
             popsize=popsize,
             pholder_params=pholder_params,
             elite_ratio=elite_ratio,
             sigma_init=sigma_init,
             mean_decay=mean_decay,
+            n_devices=n_devices,
             **fitness_kwargs,
         )
         from ..restarts import BIPOP_Restarter
         from ..restarts.termination import spread_criterion, cma_criterion
 
         self.wrapped_strategy = BIPOP_Restarter(
             self.strategy,
```

### Comparing `evosax-0.1.3/evosax/strategies/cma_es.py` & `evosax-0.1.4/evosax/strategies/cma_es.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,18 @@
     init_min: float = 0.0
     init_max: float = 0.0
     clip_min: float = -jnp.finfo(jnp.float32).max
     clip_max: float = jnp.finfo(jnp.float32).max
 
 
 def get_cma_elite_weights(
-    popsize: int, elite_popsize: int, num_dims: int
+    popsize: int,
+    elite_popsize: int,
+    num_dims: int,
+    max_dims_sq: int,
 ) -> Tuple[chex.Array, chex.Array, float, float, float]:
     """Utility helper to create truncated elite weights for mean
     update and full weights for covariance update."""
     weights_prime = jnp.array(
         [jnp.log((popsize + 1) / 2) - jnp.log(i + 1) for i in range(popsize)]
     )
     mu_eff = (jnp.sum(weights_prime[:elite_popsize]) ** 2) / jnp.sum(
@@ -53,20 +56,20 @@
     )
     mu_eff_minus = (jnp.sum(weights_prime[elite_popsize:]) ** 2) / jnp.sum(
         weights_prime[elite_popsize:] ** 2
     )
 
     # lrates for rank-one and rank-μ C updates
     alpha_cov = 2
-    c_1 = alpha_cov / ((num_dims + 1.3) ** 2 + mu_eff)
+    c_1 = alpha_cov / ((max_dims_sq + 1.3) ** 2 + mu_eff)
     c_mu = jnp.minimum(
         1 - c_1 - 1e-8,
         alpha_cov
         * (mu_eff - 2 + 1 / mu_eff)
-        / ((num_dims + 2) ** 2 + alpha_cov * mu_eff / 2),
+        / ((max_dims_sq + 2) ** 2 + alpha_cov * mu_eff / 2),
     )
     min_alpha = jnp.minimum(
         1 + c_1 / c_mu, 1 + (2 * mu_eff_minus) / (mu_eff + 2)
     )
     min_alpha = jnp.minimum(min_alpha, (1 - c_1 - c_mu) / (num_dims * c_mu))
     positive_sum = jnp.sum(weights_prime * (weights_prime > 0))
     negative_sum = jnp.sum(jnp.abs(weights_prime * (weights_prime < 0)))
@@ -84,35 +87,44 @@
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         elite_ratio: float = 0.5,
         sigma_init: float = 1.0,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """CMA-ES (e.g. Hansen, 2016)
         Reference: https://arxiv.org/abs/1604.00772
         Inspired by: https://github.com/CyberAgentAILab/cmaes"""
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         assert 0 <= elite_ratio <= 1
         self.elite_ratio = elite_ratio
         self.elite_popsize = max(1, int(self.popsize * self.elite_ratio))
         self.strategy_name = "CMA_ES"
 
         # Set core kwargs es_params
         self.sigma_init = sigma_init
 
+        # Robustness for int32 - squaring in hyperparameter calculations
+        self.max_dims_sq = jnp.minimum(self.num_dims, 40000)
+
     @property
     def params_strategy(self) -> EvoParams:
         """Return default parameters of evolution strategy."""
         _, _, mu_eff, c_1, c_mu = get_cma_elite_weights(
-            self.popsize, self.elite_popsize, self.num_dims
+            self.popsize, self.elite_popsize, self.num_dims, self.max_dims_sq
         )
 
         # lrate for cumulation of step-size control and rank-one update
         c_sigma = (mu_eff + 2) / (self.num_dims + mu_eff + 5)
         d_sigma = (
             1
             + 2
@@ -121,15 +133,15 @@
         )
         c_c = (4 + mu_eff / self.num_dims) / (
             self.num_dims + 4 + 2 * mu_eff / self.num_dims
         )
         chi_n = jnp.sqrt(self.num_dims) * (
             1.0
             - (1.0 / (4.0 * self.num_dims))
-            + 1.0 / (21.0 * (self.num_dims ** 2))
+            + 1.0 / (21.0 * (self.max_dims_sq ** 2))
         )
 
         params = EvoParams(
             mu_eff=mu_eff,
             c_1=c_1,
             c_mu=c_mu,
             c_sigma=c_sigma,
@@ -141,15 +153,15 @@
         return params
 
     def initialize_strategy(
         self, rng: chex.PRNGKey, params: EvoParams
     ) -> EvoState:
         """`initialize` the evolution strategy."""
         weights, weights_truncated, _, _, _ = get_cma_elite_weights(
-            self.popsize, self.elite_popsize, self.num_dims
+            self.popsize, self.elite_popsize, self.num_dims, self.max_dims_sq
         )
         # Initialize evolution paths & covariance matrix
         initialization = jax.random.uniform(
             rng,
             (self.num_dims,),
             minval=params.init_min,
             maxval=params.init_max,
```

### Comparing `evosax-0.1.3/evosax/strategies/cr_fm_nes.py` & `evosax-0.1.4/evosax/strategies/cr_fm_nes.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,21 +77,27 @@
     def __init__(
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         sigma_init: float = 1.0,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Cost-Reduced Fast-Moving Natural ES (Nomura & Ono, 2022)
         Reference: https://arxiv.org/abs/2201.11422
         """
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         assert not self.popsize & 1, "Population size must be even"
         self.strategy_name = "CR_FM_NES"
 
         # Set core kwargs es_params (sigma)
         self.sigma_init = sigma_init
```

### Comparing `evosax-0.1.3/evosax/strategies/de.py` & `evosax-0.1.4/evosax/strategies/de.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,20 +30,27 @@
 
 class DE(Strategy):
     def __init__(
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Differential Evolution (Storn & Price, 1997)
         Reference: https://tinyurl.com/4pje5a74"""
         assert popsize > 6, "DE requires popsize > 6."
-        super().__init__(popsize, num_dims, pholder_params, **fitness_kwargs)
+        super().__init__(
+            popsize,
+            num_dims,
+            pholder_params,
+            n_devices=n_devices,
+            **fitness_kwargs
+        )
         self.strategy_name = "DE"
 
     @property
     def params_strategy(self) -> EvoParams:
         return EvoParams()
 
     def initialize_strategy(
@@ -88,15 +95,15 @@
             rng_members,
             member_ids,
             self.num_dims,
             state.archive,
             state.best_member,
             params,
         )
-        return jnp.squeeze(x), state
+        return jnp.squeeze(x, axis=2), state
 
     def tell_strategy(
         self,
         x: chex.Array,
         fitness: chex.Array,
         state: chex.ArrayTree,
         params: EvoParams,
```

### Comparing `evosax-0.1.3/evosax/strategies/des.py` & `evosax-0.1.4/evosax/strategies/des.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,19 +44,25 @@
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         temperature: float = 12.5,
         sigma_init: float = 0.1,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Discovered Evolution Strategy (Lange et al., 2023)"""
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         self.strategy_name = "DES"
         self.temperature = temperature
         self.sigma_init = sigma_init
 
     @property
     def params_strategy(self) -> EvoParams:
```

### Comparing `evosax-0.1.3/evosax/strategies/esmc.py` & `evosax-0.1.4/evosax/strategies/esmc.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,21 +41,27 @@
         lrate_init: float = 0.05,
         lrate_decay: float = 1.0,
         lrate_limit: float = 0.001,
         sigma_init: float = 0.03,
         sigma_decay: float = 1.0,
         sigma_limit: float = 0.01,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """ESMC (Merchant et al., 2021)
         Reference: https://proceedings.mlr.press/v139/merchant21a.html
         """
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         assert self.popsize & 1, "Population size must be odd"
         assert opt_name in ["sgd", "adam", "rmsprop", "clipup", "adan"]
         self.optimizer = GradientOptimizer[opt_name](self.num_dims)
         self.strategy_name = "ESMC"
 
         # Set core kwargs es_params (lrate/sigma schedules)
```

### Comparing `evosax-0.1.3/evosax/strategies/full_iamalgam.py` & `evosax-0.1.4/evosax/strategies/full_iamalgam.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,21 +46,27 @@
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         elite_ratio: float = 0.35,
         sigma_init: float = 0.0,
         sigma_decay: float = 0.99,
         sigma_limit: float = 0.0,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """(Iterative) AMaLGaM (Bosman et al., 2013) - Full Covariance
         Reference: https://tinyurl.com/y9fcccx2
         """
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         assert 0 <= elite_ratio <= 1
         self.elite_ratio = elite_ratio
         self.elite_popsize = max(1, int(self.popsize * self.elite_ratio))
         alpha_ams = (
             0.5
             * self.elite_ratio
```

### Comparing `evosax-0.1.3/evosax/strategies/gesmr_ga.py` & `evosax-0.1.4/evosax/strategies/gesmr_ga.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,26 @@
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         elite_ratio: float = 0.5,
         sigma_ratio: float = 0.5,
         sigma_init: float = 0.07,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Self-Adaptation Mutation Rate GA."""
 
-        super().__init__(popsize, num_dims, pholder_params, **fitness_kwargs)
+        super().__init__(
+            popsize,
+            num_dims,
+            pholder_params,
+            n_devices=n_devices,
+            **fitness_kwargs
+        )
         self.elite_ratio = elite_ratio
         self.elite_popsize = max(1, int(self.popsize * self.elite_ratio))
         self.num_sigma_groups = int(jnp.sqrt(self.popsize))
         self.members_per_group = int(
             jnp.ceil(self.popsize / self.num_sigma_groups)
         )
         self.sigma_ratio = sigma_ratio
```

### Comparing `evosax-0.1.3/evosax/strategies/gld.py` & `evosax-0.1.4/evosax/strategies/gld.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,20 +28,26 @@
 class GLD(Strategy):
     def __init__(
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Gradientless Descent (Golovin et al., 2019)
         Reference: https://arxiv.org/pdf/1911.06317.pdf"""
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         self.strategy_name = "GLD"
 
     @property
     def params_strategy(self) -> EvoParams:
         """Return default parameters of evolution strategy."""
         return EvoParams()
```

### Comparing `evosax-0.1.3/evosax/strategies/guided_es.py` & `evosax-0.1.4/evosax/strategies/guided_es.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,25 +45,27 @@
         lrate_init: float = 0.05,
         lrate_decay: float = 1.0,
         lrate_limit: float = 0.001,
         sigma_init: float = 0.03,
         sigma_decay: float = 1.0,
         sigma_limit: float = 0.01,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float],
     ):
         """Guided ES (Maheswaranathan et al., 2018)
         Reference: https://arxiv.org/abs/1806.10230
         Note that there are a couple of JAX-based adaptations:
         """
         super().__init__(
             popsize,
             num_dims,
             pholder_params,
             mean_decay,
+            n_devices,
             **fitness_kwargs,
         )
         assert not self.popsize & 1, "Population size must be even"
         assert opt_name in ["sgd", "adam", "rmsprop", "clipup", "adan"]
         assert (
             subspace_dims <= self.num_dims
         ), "Subspace has to be smaller than optimization dims."
```

### Comparing `evosax-0.1.3/evosax/strategies/indep_iamalgam.py` & `evosax-0.1.4/evosax/strategies/indep_iamalgam.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,21 +51,27 @@
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         elite_ratio: float = 0.35,
         sigma_init: float = 0.0,
         sigma_decay: float = 0.99,
         sigma_limit: float = 0.0,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """(Iterative) AMaLGaM (Bosman et al., 2013) - Diagonal Covariance
         Reference: https://tinyurl.com/y9fcccx2
         """
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         assert 0 <= elite_ratio <= 1
         self.elite_ratio = elite_ratio
         self.elite_popsize = max(1, int(self.popsize * self.elite_ratio))
         alpha_ams = (
             0.5
             * self.elite_ratio
```

### Comparing `evosax-0.1.3/evosax/strategies/ipop_cma_es.py` & `evosax-0.1.4/evosax/strategies/ipop_cma_es.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,28 +23,30 @@
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         elite_ratio: float = 0.5,
         sigma_init: float = 1.0,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """IPOP-CMA-ES (Auer & Hansen, 2005).
         Reference: http://www.cmap.polytechnique.fr/~nikolaus.hansen/cec2005ipopcmaes.pdf
         """
         self.strategy_name = "IPOP_CMA_ES"
         # Instantiate base strategy & wrap it with restart wrapper
         self.strategy = CMA_ES(
             popsize=popsize,
             num_dims=num_dims,
             pholder_params=pholder_params,
             elite_ratio=elite_ratio,
             sigma_init=sigma_init,
             mean_decay=mean_decay,
+            n_devices=n_devices,
             **fitness_kwargs
         )
         from ..restarts import IPOP_Restarter
         from ..restarts.termination import cma_criterion, spread_criterion
 
         self.wrapped_strategy = IPOP_Restarter(
             self.strategy,
```

### Comparing `evosax-0.1.3/evosax/strategies/les.py` & `evosax-0.1.4/evosax/strategies/les.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Optional, Tuple, Union
-import os
 import chex
 from flax import struct
 import jax
 import jax.numpy as jnp
 import pkgutil
-from ..utils.learned_eo import (
+from ..utils.les_tools import (
     AttentionWeights,
     EvoPathMLP,
     tanh_timestamp,
     EvolutionPath,
     FitnessFeatures,
     load_pkl_object,
 )
@@ -47,17 +46,26 @@
     def __init__(
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         net_params: Optional[chex.ArrayTree] = None,
         net_ckpt_path: Optional[str] = None,
+        mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float],
     ):
-        super().__init__(popsize, num_dims, pholder_params, **fitness_kwargs)
+        super().__init__(
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs,
+        )
         self.strategy_name = "LES"
         self.evopath = EvolutionPath(
             num_dims=self.num_dims, timescales=jnp.array([0.1, 0.5, 0.9])
         )
         self.weight_layer = AttentionWeights(8)
         self.lrate_layer = EvoPathMLP(8)
         self.fitness_features = FitnessFeatures(
@@ -67,19 +75,19 @@
         # Set net params provided at instantiation
         if net_params is not None:
             self.les_net_params = net_params
 
         # Load network weights from checkpoint
         if net_ckpt_path is not None:
             self.les_net_params = load_pkl_object(net_ckpt_path)
-            print(f"Loaded model from ckpt: {net_ckpt_path}")
+            print(f"Loaded LES model from ckpt: {net_ckpt_path}")
 
         if net_params is None and net_ckpt_path is None:
             ckpt_fname = "2023_03_les_v1.pkl"
-            data = pkgutil.get_data(__name__, f"ckpt/{ckpt_fname}")
+            data = pkgutil.get_data(__name__, f"ckpt/les/{ckpt_fname}")
             self.les_net_params = load_pkl_object(data, pkg_load=True)
             print(f"Loaded pretrained LES model from ckpt: {ckpt_fname}")
 
     @property
     def params_strategy(self) -> EvoParams:
         """Return default parameters of evolution strategy."""
         return EvoParams(net_params=self.les_net_params)
```

### Comparing `evosax-0.1.3/evosax/strategies/lm_ma_es.py` & `evosax-0.1.4/evosax/strategies/lm_ma_es.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,50 +44,59 @@
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         elite_ratio: float = 0.5,
         memory_size: int = 10,
         sigma_init: float = 1.0,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Limited Memory MA-ES (Loshchilov et al., 2017)
         Reference: https://arxiv.org/pdf/1705.06693.pdf
         """
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         assert 0 <= elite_ratio <= 1
         self.elite_ratio = elite_ratio
         self.elite_popsize = max(1, int(self.popsize * self.elite_ratio))
         self.memory_size = memory_size
         self.strategy_name = "LM_MA_ES"
 
         # Set core kwargs es_params
         self.sigma_init = sigma_init
 
+        # Robustness for int32 - squaring in hyperparameter calculations
+        self.max_dims_sq = jnp.minimum(self.num_dims, 40000)
+
     @property
     def params_strategy(self) -> EvoParams:
         """Return default parameters of evolution strategy."""
         _, weights_truncated, mu_eff, c_1, c_mu = get_cma_elite_weights(
-            self.popsize, self.elite_popsize, self.num_dims
+            self.popsize, self.elite_popsize, self.num_dims, self.max_dims_sq
         )
 
         # lrate for cumulation of step-size control and rank-one update
         c_sigma = (mu_eff + 2) / (self.num_dims + mu_eff + 5)
         d_sigma = (
             1
             + 2
             * jnp.maximum(0, jnp.sqrt((mu_eff - 1) / (self.num_dims + 1)) - 1)
             + c_sigma
         )
         chi_n = jnp.sqrt(self.num_dims) * (
             1.0
             - (1.0 / (4.0 * self.num_dims))
-            + 1.0 / (21.0 * (self.num_dims ** 2))
+            + 1.0 / (21.0 * (self.max_dims_sq ** 2))
         )
         mu_w = 1 / jnp.sum(weights_truncated ** 2)
         params = EvoParams(
             mu_eff=mu_eff,
             c_1=c_1,
             c_mu=c_mu,
             c_sigma=c_sigma,
@@ -99,15 +108,15 @@
         return params
 
     def initialize_strategy(
         self, rng: chex.PRNGKey, params: EvoParams
     ) -> EvoState:
         """`initialize` the evolution strategy."""
         _, weights_truncated, _, _, _ = get_cma_elite_weights(
-            self.popsize, self.elite_popsize, self.num_dims
+            self.popsize, self.elite_popsize, self.num_dims, self.max_dims_sq
         )
         c_d = jnp.array(
             [1 / (1.5 ** i * self.num_dims) for i in range(self.memory_size)]
         )
         c_c = jnp.array(
             [
                 self.popsize / (4 ** i * self.num_dims)
```

### Comparing `evosax-0.1.3/evosax/strategies/ma_es.py` & `evosax-0.1.4/evosax/strategies/ma_es.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,50 +40,59 @@
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         elite_ratio: float = 0.5,
         sigma_init: float = 1.0,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """MA-ES (Bayer & Sendhoff, 2017)
         Reference: https://www.honda-ri.de/pubs/pdf/3376.pdf
         """
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         assert 0 <= elite_ratio <= 1
         self.elite_ratio = elite_ratio
         self.elite_popsize = max(1, int(self.popsize * self.elite_ratio))
         self.strategy_name = "MA_ES"
 
         # Set core kwargs es_params
         self.sigma_init = sigma_init
 
+        # Robustness for int32 - squaring in hyperparameter calculations
+        self.max_dims_sq = jnp.minimum(self.num_dims, 40000)
+
     @property
     def params_strategy(self) -> EvoParams:
         """Return default parameters of evolution strategy."""
         _, _, mu_eff, c_1, c_mu = get_cma_elite_weights(
-            self.popsize, self.elite_popsize, self.num_dims
+            self.popsize, self.elite_popsize, self.num_dims, self.max_dims_sq
         )
 
         # lrate for cumulation of step-size control and rank-one update
         c_sigma = (mu_eff + 2) / (self.num_dims + mu_eff + 5)
         d_sigma = (
             1
             + 2
             * jnp.maximum(0, jnp.sqrt((mu_eff - 1) / (self.num_dims + 1)) - 1)
             + c_sigma
         )
 
         chi_n = jnp.sqrt(self.num_dims) * (
             1.0
             - (1.0 / (4.0 * self.num_dims))
-            + 1.0 / (21.0 * (self.num_dims ** 2))
+            + 1.0 / (21.0 * (self.max_dims_sq ** 2))
         )
 
         params = EvoParams(
             mu_eff=mu_eff,
             c_1=c_1,
             c_mu=c_mu,
             c_sigma=c_sigma,
@@ -94,15 +103,15 @@
         return params
 
     def initialize_strategy(
         self, rng: chex.PRNGKey, params: EvoParams
     ) -> EvoState:
         """`initialize` the evolution strategy."""
         _, weights_truncated, _, _, _ = get_cma_elite_weights(
-            self.popsize, self.elite_popsize, self.num_dims
+            self.popsize, self.elite_popsize, self.num_dims, self.max_dims_sq
         )
         # Initialize evolution paths & covariance matrix
         initialization = jax.random.uniform(
             rng,
             (self.num_dims,),
             minval=params.init_min,
             maxval=params.init_max,
```

### Comparing `evosax-0.1.3/evosax/strategies/mr15_ga.py` & `evosax-0.1.4/evosax/strategies/mr15_ga.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,21 +34,28 @@
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         elite_ratio: float = 0.0,
         sigma_ratio: float = 0.15,
         sigma_init: float = 0.1,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """1/5 MR Genetic Algorithm (Rechenberg, 1987)
         Reference: https://link.springer.com/chapter/10.1007/978-3-642-81283-5_8
         """
 
-        super().__init__(popsize, num_dims, pholder_params, **fitness_kwargs)
+        super().__init__(
+            popsize,
+            num_dims,
+            pholder_params,
+            n_devices=n_devices,
+            **fitness_kwargs
+        )
         self.elite_ratio = elite_ratio
         self.elite_popsize = max(1, int(self.popsize * self.elite_ratio))
         self.strategy_name = "MR15_GA"
 
         # Set core kwargs es_params
         self.sigma_ratio = sigma_ratio  # no. mutation that have to improve
         self.sigma_init = sigma_init
@@ -101,15 +108,15 @@
         idx_b = jax.random.choice(rng_idx_b, elite_ids, (self.popsize,))
         members_a = state.archive[idx_a]
         members_b = state.archive[idx_b]
         x = jax.vmap(single_mate, in_axes=(0, 0, 0, None))(
             rng_mate, members_a, members_b, params.cross_over_rate
         )
         x += epsilon
-        return jnp.squeeze(x), state
+        return x, state
 
     def tell_strategy(
         self,
         x: chex.Array,
         fitness: chex.Array,
         state: EvoState,
         params: EvoParams,
```

### Comparing `evosax-0.1.3/evosax/strategies/open_es.py` & `evosax-0.1.4/evosax/strategies/open_es.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,21 +39,27 @@
         lrate_init: float = 0.05,
         lrate_decay: float = 1.0,
         lrate_limit: float = 0.001,
         sigma_init: float = 0.03,
         sigma_decay: float = 1.0,
         sigma_limit: float = 0.01,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """OpenAI-ES (Salimans et al. (2017)
         Reference: https://arxiv.org/pdf/1703.03864.pdf
         Inspired by: https://github.com/hardmaru/estool/blob/master/es.py"""
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         assert not self.popsize & 1, "Population size must be even"
         assert opt_name in ["sgd", "adam", "rmsprop", "clipup", "adan"]
         self.optimizer = GradientOptimizer[opt_name](self.num_dims)
         self.strategy_name = "OpenES"
 
         # Set core kwargs es_params (lrate/sigma schedules)
```

### Comparing `evosax-0.1.3/evosax/strategies/pbt.py` & `evosax-0.1.4/evosax/strategies/pbt.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,19 +28,26 @@
 
 class PBT(Strategy):
     def __init__(
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Synchronous Population-Based Training (Jaderberg et al., 2017)
         Reference: https://arxiv.org/abs/1711.09846"""
-        super().__init__(popsize, num_dims, pholder_params, **fitness_kwargs)
+        super().__init__(
+            popsize,
+            num_dims,
+            pholder_params,
+            n_devices=n_devices,
+            **fitness_kwargs
+        )
         self.strategy_name = "PBT"
 
     @property
     def params_strategy(self) -> EvoParams:
         """Return default parameters of evolution strategy."""
         return EvoParams()
```

### Comparing `evosax-0.1.3/evosax/strategies/persistent_es.py` & `evosax-0.1.4/evosax/strategies/persistent_es.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,22 +43,28 @@
         lrate_init: float = 0.05,
         lrate_decay: float = 1.0,
         lrate_limit: float = 0.001,
         sigma_init: float = 0.03,
         sigma_decay: float = 1.0,
         sigma_limit: float = 0.01,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Persistent ES (Vicol et al., 2021).
         Reference: http://proceedings.mlr.press/v139/vicol21a.html
         Inspired by: http://proceedings.mlr.press/v139/vicol21a/vicol21a-supp.pdf
         """
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         assert not self.popsize & 1, "Population size must be even"
         assert opt_name in ["sgd", "adam", "rmsprop", "clipup", "adan"]
         self.optimizer = GradientOptimizer[opt_name](self.num_dims)
         self.strategy_name = "PersistentES"
 
         # Set core kwargs es_params (lrate/sigma schedules)
@@ -113,16 +119,16 @@
             jax.random.normal(rng, (self.popsize // 2, self.num_dims))
             * state.sigma
         )
         neg_perts = -pos_perts
         perts = jnp.concatenate([pos_perts, neg_perts], axis=0)
         # Add the perturbations from this unroll to the perturbation accumulators
         pert_accum = state.pert_accum + perts
-        y = state.mean + perts
-        return jnp.squeeze(y), state.replace(pert_accum=pert_accum)
+        x = state.mean + perts
+        return x, state.replace(pert_accum=pert_accum)
 
     def tell_strategy(
         self,
         x: chex.Array,
         fitness: chex.Array,
         state: EvoState,
         params: EvoParams,
```

### Comparing `evosax-0.1.3/evosax/strategies/pgpe.py` & `evosax-0.1.4/evosax/strategies/pgpe.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,21 +42,27 @@
         lrate_init: float = 0.15,
         lrate_decay: float = 1.0,
         lrate_limit: float = 0.001,
         sigma_init: float = 0.1,
         sigma_decay: float = 1.0,
         sigma_limit: float = 0.01,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """PGPE (e.g. Sehnke et al., 2010)
         Reference: https://tinyurl.com/2p8bn956
         Inspired by: https://github.com/hardmaru/estool/blob/master/es.py"""
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         assert 0 <= elite_ratio <= 1
         self.elite_ratio = elite_ratio
         self.elite_popsize = max(1, int(self.popsize / 2 * self.elite_ratio))
 
         assert not self.popsize & 1, "Population size must be even"
         assert opt_name in ["sgd", "adam", "rmsprop", "clipup", "adan"]
```

### Comparing `evosax-0.1.3/evosax/strategies/pso.py` & `evosax-0.1.4/evosax/strategies/pso.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,19 +32,26 @@
 
 class PSO(Strategy):
     def __init__(
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Particle Swarm Optimization (Kennedy & Eberhart, 1995)
         Reference: https://ieeexplore.ieee.org/document/488968"""
-        super().__init__(popsize, num_dims, pholder_params, **fitness_kwargs)
+        super().__init__(
+            popsize,
+            num_dims,
+            pholder_params,
+            n_devices=n_devices,
+            **fitness_kwargs
+        )
         self.strategy_name = "PSO"
 
     @property
     def params_strategy(self) -> EvoParams:
         """Return default parameters of evolution strategy."""
         return EvoParams()
 
@@ -95,15 +102,15 @@
             state.best_archive_fitness,
             params.inertia_coeff,
             params.cognitive_coeff,
             params.social_coeff,
         )
         # Update particle positions with velocity
         x = state.archive + vel
-        return jnp.squeeze(x), state.replace(velocity=vel)
+        return x, state.replace(velocity=vel)
 
     def tell_strategy(
         self,
         x: chex.Array,
         fitness: chex.Array,
         state: EvoState,
         params: EvoParams,
```

### Comparing `evosax-0.1.3/evosax/strategies/random.py` & `evosax-0.1.4/evosax/strategies/random.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,26 @@
 
 class RandomSearch(Strategy):
     def __init__(
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Simple Random Search Baseline"""
 
-        super().__init__(popsize, num_dims, pholder_params, **fitness_kwargs)
+        super().__init__(
+            popsize,
+            num_dims,
+            pholder_params,
+            n_devices=n_devices,
+            **fitness_kwargs
+        )
         self.strategy_name = "RandomSearch"
 
     @property
     def params_strategy(self) -> EvoParams:
         """Return default parameters of evolution strategy."""
         return EvoParams()
 
@@ -64,15 +71,15 @@
         """`ask` for new proposed candidates to evaluate next."""
         x = jax.random.uniform(
             rng,
             (self.popsize, self.num_dims),
             minval=params.range_min,
             maxval=params.range_max,
         )
-        return jnp.squeeze(x), state
+        return x, state
 
     def tell_strategy(
         self,
         x: chex.Array,
         fitness: chex.Array,
         state: EvoState,
         params: EvoParams,
```

### Comparing `evosax-0.1.3/evosax/strategies/rm_es.py` & `evosax-0.1.4/evosax/strategies/rm_es.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,21 +63,27 @@
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         elite_ratio: float = 0.5,
         memory_size: int = 10,
         sigma_init: float = 1.0,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Rank-m ES (Li & Zhang, 2017)
         Reference: https://ieeexplore.ieee.org/document/8080257
         """
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         assert 0 <= elite_ratio <= 1
         self.elite_ratio = elite_ratio
         self.elite_popsize = max(1, int(self.popsize * self.elite_ratio))
         self.memory_size = memory_size  # number of ranks
         self.strategy_name = "RmES"
```

### Comparing `evosax-0.1.3/evosax/strategies/samr_ga.py` & `evosax-0.1.4/evosax/strategies/samr_ga.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,26 @@
     def __init__(
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         elite_ratio: float = 0.0,
         sigma_init: float = 0.07,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Self-Adaptation Mutation Rate GA."""
 
-        super().__init__(popsize, num_dims, pholder_params, **fitness_kwargs)
+        super().__init__(
+            popsize,
+            num_dims,
+            pholder_params,
+            n_devices=n_devices,
+            **fitness_kwargs
+        )
         self.elite_ratio = elite_ratio
         self.elite_popsize = max(1, int(self.popsize * self.elite_ratio))
         self.strategy_name = "SAMR_GA"
 
         # Set core kwargs es_params
         self.sigma_init = sigma_init
```

### Comparing `evosax-0.1.3/evosax/strategies/sep_cma_es.py` & `evosax-0.1.4/evosax/strategies/sep_cma_es.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,25 +61,27 @@
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         elite_ratio: float = 0.5,
         sigma_init: float = 1.0,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Separable CMA-ES (e.g. Ros & Hansen, 2008)
         Reference: https://hal.inria.fr/inria-00287367/document
         Inspired by: github.com/CyberAgentAILab/cmaes/blob/main/cmaes/_sepcma.py
         """
         super().__init__(
             popsize,
             num_dims,
             pholder_params,
             mean_decay,
+            n_devices,
             **fitness_kwargs,
         )
         assert 0 <= elite_ratio <= 1
         self.elite_ratio = elite_ratio
         self.elite_popsize = max(1, int(self.popsize * self.elite_ratio))
         self.strategy_name = "Sep_CMA_ES"
 
@@ -114,15 +116,15 @@
             * jnp.maximum(0, jnp.sqrt((mu_eff - 1) / (self.num_dims + 1)) - 1)
             + c_sigma
         )
         c_c = 4 / (self.num_dims + 4)
         chi_n = jnp.sqrt(self.num_dims) * (
             1.0
             - (1.0 / (4.0 * self.num_dims))
-            + 1.0 / (21.0 * (self.num_dims ** 2))
+            + 1.0 / (21.0 * (self.max_dims_sq ** 2))
         )
         params = EvoParams(
             mu_eff=mu_eff,
             c_1=c_1,
             c_mu=c_mu,
             c_sigma=c_sigma,
             d_sigma=d_sigma,
```

### Comparing `evosax-0.1.3/evosax/strategies/sim_anneal.py` & `evosax-0.1.4/evosax/strategies/sim_anneal.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,20 +37,27 @@
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         sigma_init: float = 0.03,
         sigma_decay: float = 1.0,
         sigma_limit: float = 0.01,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Simulated Annealing (Rasdi Rere et al., 2015)
         Reference: https://www.sciencedirect.com/science/article/pii/S1877050915035759
         """
-        super().__init__(popsize, num_dims, pholder_params, **fitness_kwargs)
+        super().__init__(
+            popsize,
+            num_dims,
+            pholder_params,
+            n_devices=n_devices,
+            **fitness_kwargs
+        )
         self.strategy_name = "SimAnneal"
 
         # Set core kwargs es_params (lrate/sigma schedules)
         self.sigma_init = sigma_init
         self.sigma_decay = sigma_decay
         self.sigma_limit = sigma_limit
```

### Comparing `evosax-0.1.3/evosax/strategies/simple_es.py` & `evosax-0.1.4/evosax/strategies/simple_es.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,27 @@
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         elite_ratio: float = 0.5,
         sigma_init: float = 1.0,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Simple Gaussian Evolution Strategy (Rechenberg, 1975)
         Reference: https://onlinelibrary.wiley.com/doi/abs/10.1002/fedr.19750860506
         Inspired by: https://github.com/hardmaru/estool/blob/master/es.py"""
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         self.elite_ratio = elite_ratio
         self.elite_popsize = max(1, int(self.popsize * self.elite_ratio))
         self.strategy_name = "SimpleES"
 
         # Set core kwargs es_params
         self.sigma_init = sigma_init
```

### Comparing `evosax-0.1.3/evosax/strategies/simple_ga.py` & `evosax-0.1.4/evosax/strategies/simple_ga.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,21 +36,28 @@
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         elite_ratio: float = 0.5,
         sigma_init: float = 0.1,
         sigma_decay: float = 1.0,
         sigma_limit: float = 0.01,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Simple Genetic Algorithm (Such et al., 2017)
         Reference: https://arxiv.org/abs/1712.06567
         Inspired by: https://github.com/hardmaru/estool/blob/master/es.py"""
 
-        super().__init__(popsize, num_dims, pholder_params, **fitness_kwargs)
+        super().__init__(
+            popsize,
+            num_dims,
+            pholder_params,
+            n_devices=n_devices,
+            **fitness_kwargs
+        )
         self.elite_ratio = elite_ratio
         self.elite_popsize = max(1, int(self.popsize * self.elite_ratio))
         self.strategy_name = "SimpleGA"
 
         # Set core kwargs es_params
         self.sigma_init = sigma_init
         self.sigma_decay = sigma_decay
@@ -106,15 +113,15 @@
         idx_b = jax.random.choice(rng_idx_b, elite_ids, (self.popsize,))
         members_a = state.archive[idx_a]
         members_b = state.archive[idx_b]
         x = jax.vmap(single_mate, in_axes=(0, 0, 0, None))(
             rng_mate, members_a, members_b, params.cross_over_rate
         )
         x += epsilon
-        return jnp.squeeze(x), state
+        return x, state
 
     def tell_strategy(
         self,
         x: chex.Array,
         fitness: chex.Array,
         state: EvoState,
         params: EvoParams,
```

### Comparing `evosax-0.1.3/evosax/strategies/snes.py` & `evosax-0.1.4/evosax/strategies/snes.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,21 +54,27 @@
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         sigma_init: float = 1.0,
         temperature: float = 0.0,  # good values tend to be between 12 and 20
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Separable Exponential Natural ES (Wierstra et al., 2014)
         Reference: https://www.jmlr.org/papers/volume15/wierstra14a/wierstra14a.pdf
         """
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         self.strategy_name = "SNES"
 
         # Set core kwargs es_params
         self.sigma_init = sigma_init
         self.temperature = temperature
```

### Comparing `evosax-0.1.3/evosax/strategies/xnes.py` & `evosax-0.1.4/evosax/strategies/xnes.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,21 +39,27 @@
     def __init__(
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         sigma_init: float = 1.0,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Exponential Natural ES (Wierstra et al., 2014)
         Reference: https://www.jmlr.org/papers/volume15/wierstra14a/wierstra14a.pdf
         Inspired by: https://github.com/chanshing/xnes"""
         super().__init__(
-            popsize, num_dims, pholder_params, mean_decay, **fitness_kwargs
+            popsize,
+            num_dims,
+            pholder_params,
+            mean_decay,
+            n_devices,
+            **fitness_kwargs
         )
         self.strategy_name = "xNES"
 
         # Set core kwargs es_params
         self.sigma_init = sigma_init
 
     @property
```

### Comparing `evosax-0.1.3/evosax/strategy.py` & `evosax-0.1.4/evosax/strategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,23 +30,24 @@
 class Strategy(object):
     def __init__(
         self,
         popsize: int,
         num_dims: Optional[int] = None,
         pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
         mean_decay: float = 0.0,
+        n_devices: Optional[int] = None,
         **fitness_kwargs: Union[bool, int, float]
     ):
         """Base Class for an Evolution Strategy."""
         self.popsize = popsize
 
         # Setup optional parameter reshaper
         self.use_param_reshaper = pholder_params is not None
         if self.use_param_reshaper:
-            self.param_reshaper = ParameterReshaper(pholder_params)
+            self.param_reshaper = ParameterReshaper(pholder_params, n_devices)
             self.num_dims = self.param_reshaper.total_params
         else:
             self.num_dims = num_dims
         assert (
             self.num_dims is not None
         ), "Provide either num_dims or pholder_params to strategy."
 
@@ -62,23 +63,33 @@
     def default_params(self) -> EvoParams:
         """Return default parameters of evolution strategy."""
         params = self.params_strategy
         return params
 
     @partial(jax.jit, static_argnums=(0,))
     def initialize(
-        self, rng: chex.PRNGKey, params: Optional[EvoParams] = None
+        self,
+        rng: chex.PRNGKey,
+        params: Optional[EvoParams] = None,
+        init_mean: Optional[Union[chex.Array, chex.ArrayTree]] = None,
     ) -> EvoState:
         """`initialize` the evolution strategy."""
         # Use default hyperparameters if no other settings provided
         if params is None:
             params = self.default_params
 
         # Initialize strategy based on strategy-specific initialize method
         state = self.initialize_strategy(rng, params)
+
+        if init_mean is not None:
+            if self.use_param_reshaper:
+                init_mean = self.param_reshaper.flatten_single(init_mean)
+            else:
+                init_mean = jnp.asarray(init_mean)
+            state = state.replace(mean=init_mean)
         return state
 
     @partial(jax.jit, static_argnums=(0,))
     def ask(
         self,
         rng: chex.PRNGKey,
         state: EvoState,
@@ -88,15 +99,15 @@
         # Use default hyperparameters if no other settings provided
         if params is None:
             params = self.default_params
 
         # Generate proposal based on strategy-specific ask method
         x, state = self.ask_strategy(rng, state, params)
         # Clip proposal candidates into allowed range
-        x_clipped = jnp.clip(jnp.squeeze(x), params.clip_min, params.clip_max)
+        x_clipped = jnp.clip(x, params.clip_min, params.clip_max)
 
         # Reshape parameters into pytrees
         if self.use_param_reshaper:
             x_out = self.param_reshaper.reshape(x_clipped)
         else:
             x_out = x_clipped
         return x_out, state
```

### Comparing `evosax-0.1.3/evosax/utils/__init__.py` & `evosax-0.1.4/evosax/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/utils/eigen_decomp.py` & `evosax-0.1.4/evosax/utils/eigen_decomp.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/utils/es_logger.py` & `evosax-0.1.4/evosax/utils/es_logger.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,33 @@
+from typing import Optional, Union
 import pickle
 import jax
 import jax.numpy as jnp
 import chex
 from functools import partial
+from .reshape_params import ParameterReshaper
 
 
 class ESLog(object):
     def __init__(
-        self, num_dims: int, num_generations: int, top_k: int, maximize: bool
+        self,
+        num_dims: Optional[int] = None,
+        pholder_params: Optional[Union[chex.ArrayTree, chex.Array]] = None,
+        num_generations: int = 200,
+        top_k: int = 5,
+        maximize: bool = False,
     ):
         """Simple jittable logging tool for ES rollouts."""
-        self.num_dims = num_dims
+        # Setup optional parameter reshaper
+        self.use_param_reshaper = pholder_params is not None
+        if self.use_param_reshaper:
+            self.param_reshaper = ParameterReshaper(pholder_params, n_devices=1)
+            self.num_dims = self.param_reshaper.total_params
+        else:
+            self.num_dims = num_dims
         self.num_generations = num_generations
         self.top_k = top_k
         self.maximize = maximize
 
     @partial(jax.jit, static_argnums=(0,))
     def initialize(self) -> chex.ArrayTree:
         """Initialize the logger storage."""
@@ -43,25 +56,26 @@
             "log_gen_std": jnp.zeros(self.num_generations)
             - 1e10 * self.maximize
             + 1e10 * (1 - self.maximize),
             "gen_counter": 0,
         }
         return log
 
-    # @partial(jax.jit, static_argnums=(0,))
+    @partial(jax.jit, static_argnums=(0,))
     def update(
         self, log: chex.ArrayTree, x: chex.Array, fitness: chex.Array
     ) -> chex.ArrayTree:
         """Update the logging storage with newest data."""
         # Check if there are solutions better than current archive
         vals = jnp.hstack([log["top_fitness"], fitness])
+        if self.use_param_reshaper:
+            x = self.param_reshaper.flatten(x)
         params = jnp.vstack([log["top_params"], x])
-        top_idx = (
-            self.maximize * ((-1) * vals).argsort()
-            + ((1 - self.maximize) * vals.argsort())
+        top_idx = self.maximize * ((-1) * vals).argsort() + (
+            (1 - self.maximize) * vals.argsort()
         )
         log["top_fitness"] = vals[top_idx[: self.top_k]]
         log["top_params"] = params[top_idx[: self.top_k]]
         log["log_top_1"] = (
             log["log_top_1"].at[log["gen_counter"]].set(log["top_fitness"][0])
         )
         log["log_top_mean"] = (
```

### Comparing `evosax-0.1.3/evosax/utils/evojax_wrapper.py` & `evosax-0.1.4/evosax/utils/evojax_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,7 +47,12 @@
         """Return set of mean/best parameters."""
         return jnp.array(self.es_state.mean, copy=True)
 
     @best_params.setter
     def best_params(self, params: chex.Array) -> None:
         """Update the best parameters stored internally."""
         self.es_state = self.es_state.replace(mean=jnp.array(params, copy=True))
+
+    @property
+    def solution(self):
+        """Get evaluation parameters for current ES state."""
+        return self.es.get_eval_params(self.es_state)
```

### Comparing `evosax-0.1.3/evosax/utils/helpers.py` & `evosax-0.1.4/evosax/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/utils/learned_eo.py` & `evosax-0.1.4/evosax/utils/les_tools.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/utils/optimizer.py` & `evosax-0.1.4/evosax/utils/optimizer.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/utils/reshape_fitness.py` & `evosax-0.1.4/evosax/utils/reshape_fitness.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax/utils/reshape_params.py` & `evosax-0.1.4/evosax/utils/reshape_params.py`

 * *Files 15% similar despite different names*

```diff
@@ -68,27 +68,32 @@
     def multi_reshape(self, x: chex.Array) -> chex.ArrayTree:
         """Reshape parameters lying already on different devices."""
         # No reshaping required!
         vmap_shape = jax.vmap(self.reshape_single)
         return jax.pmap(vmap_shape)(x)
 
     def flatten(self, x: chex.ArrayTree) -> chex.Array:
-        """Reshaping pytree parameters into flat array."""
+        """Reshaping pytree parameters (population) into flat array."""
         vmap_flat = jax.vmap(ravel_pytree)
         if self.n_devices > 1:
             # Flattening of pmap paramater trees to apply vmap flattening
             def map_flat(x):
                 x_re = jax.tree_map(lambda x: x.reshape(-1, *x.shape[2:]), x)
                 return vmap_flat(x_re)
 
         else:
             map_flat = vmap_flat
         flat = map_flat(x)
+        # Out shape: (pop, params)
         return flat
 
+    def flatten_single(self, x: chex.ArrayTree) -> chex.Array:
+        """Reshaping pytree parameters (single) into flat array."""
+        return ravel_pytree(x)
+
     def multi_flatten(self, x: chex.Array) -> chex.ArrayTree:
         """Flatten parameters lying remaining on different devices."""
         # No reshaping required!
         vmap_flat = jax.vmap(ravel_pytree)
         return jax.pmap(vmap_flat)(x)
 
     def split_params_for_pmap(self, param: chex.Array) -> chex.Array:
```

### Comparing `evosax-0.1.3/evosax/utils/visualizer_2d.py` & `evosax-0.1.4/evosax/utils/visualizer_2d.py`

 * *Files identical despite different names*

### Comparing `evosax-0.1.3/evosax.egg-info/PKG-INFO` & `evosax-0.1.4/evosax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: evosax
-Version: 0.1.3
+Version: 0.1.4
 Summary: JAX-Based Evolution Strategies
 Home-page: https://github.com/RobertTLange/evosax
-Download-URL: https://github.com/RobertTLange/evosax/archive/v0.1.3.tar.gz
+Download-URL: https://github.com/RobertTLange/evosax/archive/v0.1.4.tar.gz
 Author: Robert Tjarko Lange
 Author-email: robertlange0@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -49,22 +49,22 @@
 state.best_member, state.best_fitness
 ```
 
 ## Implemented Evolution Strategies 🦎
 
 | Strategy | Reference | Import | Example |
 | --- | --- | ---  | --- |
-| OpenES | [Salimans et al. (2017)](https://arxiv.org/pdf/1703.03864.pdf) | [`OpenES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/open_es.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/03_cnn_mnist.ipynb)
+| OpenAI-ES | [Salimans et al. (2017)](https://arxiv.org/pdf/1703.03864.pdf) | [`OpenES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/open_es.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/03_cnn_mnist.ipynb)
 | PGPE | [Sehnke et al. (2010)](https://citeseerx.ist.psu.edu/viewdoc/download;jsessionid=A64D1AE8313A364B814998E9E245B40A?doi=10.1.1.180.7104&rep=rep1&type=pdf) | [`PGPE`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/pgpe.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/02_mlp_control.ipynb)
 | ARS | [Mania et al. (2018)](https://arxiv.org/pdf/1803.07055.pdf) | [`ARS`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/ars.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/00_getting_started.ipynb)
 | ESMC | [Merchant et al. (2021)](https://proceedings.mlr.press/v139/merchant21a.html) | [`ESMC`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/esmc.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Persistent ES | [Vicol et al. (2021)](http://proceedings.mlr.press/v139/vicol21a.html) | [`PersistentES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/persistent_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/04_lrate_pes.ipynb)
 | xNES | [Wierstra et al. (2014)](https://www.jmlr.org/papers/volume15/wierstra14a/wierstra14a.pdf) | [`XNES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/xnes.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | SNES | [Wierstra et al. (2014)](https://www.jmlr.org/papers/volume15/wierstra14a/wierstra14a.pdf) | [`SNES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/sxnes.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
-| CR-FM-NES | [Nomura & Ono (2022)](https://arxiv.org/abs/2201.11422) | [`CR-FM-NES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/cr_fm_nes.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
+| CR-FM-NES | [Nomura & Ono (2022)](https://arxiv.org/abs/2201.11422) | [`CR_FM_NES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/cr_fm_nes.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Guided ES | [Maheswaranathan et al. (2018)](https://arxiv.org/abs/1806.10230) | [`GuidedES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/guided_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | ASEBO | [Choromanski et al. (2019)](https://arxiv.org/abs/1903.04268) | [`ASEBO`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/asebo.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | CMA-ES | [Hansen & Ostermeier (2001)](http://www.cmap.polytechnique.fr/~nikolaus.hansen/cmaartic.pdf) | [`CMA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/cma_es.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Sep-CMA-ES | [Ros & Hansen (2008)](https://hal.inria.fr/inria-00287367/document) | [`Sep_CMA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/sep_cma_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | BIPOP-CMA-ES | [Hansen (2009)](https://hal.inria.fr/inria-00382093/document) | [`BIPOP_CMA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/bipop_cma_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/06_restart_es.ipynb)
 | IPOP-CMA-ES | [Auer & Hansen (2005)](http://www.cmap.polytechnique.fr/~nikolaus.hansen/cec2005ipopcmaes.pdf) | [`IPOP_CMA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/ipop_cma_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/06_restart_es.ipynb)
 | Full-iAMaLGaM | [Bosman et al. (2013)](https://tinyurl.com/y9fcccx2) | [`Full_iAMaLGaM`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/full_iamalgam.py)  |[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
@@ -72,23 +72,24 @@
 | MA-ES | [Bayer & Sendhoff (2017)](https://www.honda-ri.de/pubs/pdf/3376.pdf) | [`MA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/ma_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | LM-MA-ES | [Loshchilov et al. (2017)](https://arxiv.org/pdf/1705.06693.pdf) | [`LM_MA_ES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/lm_ma_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | RmES | [Li & Zhang (2017)](https://ieeexplore.ieee.org/document/8080257) | [`RmES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/rm_es.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Simple Genetic | [Such et al. (2017)](https://arxiv.org/abs/1712.06567) | [`SimpleGA`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/simple_ga.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | SAMR-GA | [Clune et al. (2008)](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1000187) | [`SAMR_GA`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/samr_ga.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | GESMR-GA | [Kumar et al. (2022)](https://arxiv.org/abs/2204.04817) | [`GESMR_GA`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/gesmr_ga.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | MR15-GA | [Rechenberg (1978)](https://link.springer.com/chapter/10.1007/978-3-642-81283-5_8) | [`MR15_GA`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/mr15_ga.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
+| LGA | [Lange et al. (2023b)](https://arxiv.org/abs/2304.03995) | [`LGA`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/lga.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Simple Gaussian | [Rechenberg (1978)](https://link.springer.com/chapter/10.1007/978-3-642-81283-5_8) | [`SimpleES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/simple_es.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
-| DES | [Lange et al. (2023)](https://arxiv.org/abs/2211.11260) | [`DES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/des.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
-| LES | [Lange et al. (2023)](https://arxiv.org/abs/2211.11260) | [`LES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/les.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
+| DES | [Lange et al. (2023a)](https://arxiv.org/abs/2211.11260) | [`DES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/des.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
+| LES | [Lange et al. (202a3)](https://arxiv.org/abs/2211.11260) | [`LES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/les.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Particle Swarm Optimization | [Kennedy & Eberhart (1995)](https://ieeexplore.ieee.org/document/488968) | [`PSO`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/pso.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Differential Evolution | [Storn & Price (1997)](https://www.metabolic-economics.de/pages/seminar_theoretische_biologie_2007/literatur/schaber/Storn1997JGlobOpt11.pdf) | [`DE`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/de.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | GLD | [Golovin et al. (2019)](https://arxiv.org/pdf/1911.06317.pdf) | [`GLD`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/gld.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Simulated Annealing | [Rasdi Rere et al. (2015)](https://www.sciencedirect.com/science/article/pii/S1877050915035759) | [`SimAnneal`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/sim_anneal.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 | Population-Based Training | [Jaderberg et al. (2017)](https://arxiv.org/abs/1711.09846) | [`PBT`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/pbt.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/05_quadratic_pbt.ipynb)
-
+| Random Search | [Bergstra & Bengio (2012)](https://www.jmlr.org/papers/volume13/bergstra12a/bergstra12a.pdf) | [`RandomSearch`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/random.py)  | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/01_classic_benchmark.ipynb)
 
 
 
 
 ## Installation ⏳
 
 The latest `evosax` release can directly be installed from PyPI:
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: evosax Version: 0.1.3 Summary: JAX-Based Evolution
+Metadata-Version: 2.1 Name: evosax Version: 0.1.4 Summary: JAX-Based Evolution
 Strategies Home-page: https://github.com/RobertTLange/evosax Download-URL:
-https://github.com/RobertTLange/evosax/archive/v0.1.3.tar.gz Author: Robert
+https://github.com/RobertTLange/evosax/archive/v0.1.4.tar.gz Author: Robert
 Tjarko Lange Author-email: robertlange0@gmail.com Platform: any Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE # `evosax`: JAX-Based Evolution Strategies ð¦ [!
@@ -34,15 +34,15 @@
 strategy.initialize(rng, es_params) # Run ask-eval-tell loop - NOTE: By default
 minimization! for t in range(num_generations): rng, rng_gen, rng_eval =
 jax.random.split(rng, 3) x, state = strategy.ask(rng_gen, state, es_params)
 fitness = ... # Your population evaluation fct state = strategy.tell(x,
 fitness, state, es_params) # Get best overall population member & its fitness
 state.best_member, state.best_fitness ``` ## Implemented Evolution Strategies
 ð¦ | Strategy | Reference | Import | Example | | --- | --- | --- | --- | |
-OpenES | [Salimans et al. (2017)](https://arxiv.org/pdf/1703.03864.pdf) |
+OpenAI-ES | [Salimans et al. (2017)](https://arxiv.org/pdf/1703.03864.pdf) |
 [`OpenES`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/
 open_es.py) | [![Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/blob/
 main/examples/03_cnn_mnist.ipynb) | PGPE | [Sehnke et al. (2010)](https://
 citeseerx.ist.psu.edu/viewdoc/
 download;jsessionid=A64D1AE8313A364B814998E9E245B40A?doi=10.1.1.180.7104&rep=rep1&type=pdf)
 | [`PGPE`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/
@@ -69,15 +69,15 @@
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
 01_classic_benchmark.ipynb) | SNES | [Wierstra et al. (2014)](https://
 www.jmlr.org/papers/volume15/wierstra14a/wierstra14a.pdf) | [`SNES`](https://
 github.com/RobertTLange/evosax/tree/main/evosax/strategies/sxnes.py) | [!
 [Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
 01_classic_benchmark.ipynb) | CR-FM-NES | [Nomura & Ono (2022)](https://
-arxiv.org/abs/2201.11422) | [`CR-FM-NES`](https://github.com/RobertTLange/
+arxiv.org/abs/2201.11422) | [`CR_FM_NES`](https://github.com/RobertTLange/
 evosax/tree/main/evosax/strategies/cr_fm_nes.py) | [![Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
 01_classic_benchmark.ipynb) | Guided ES | [Maheswaranathan et al. (2018)]
 (https://arxiv.org/abs/1806.10230) | [`GuidedES`](https://github.com/
 RobertTLange/evosax/tree/main/evosax/strategies/guided_es.py) | [![Colab]
 (https://colab.research.google.com/assets/colab-badge.svg)](https://
@@ -148,55 +148,64 @@
 //colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
 01_classic_benchmark.ipynb) | MR15-GA | [Rechenberg (1978)](https://
 link.springer.com/chapter/10.1007/978-3-642-81283-5_8) | [`MR15_GA`](https://
 github.com/RobertTLange/evosax/tree/main/evosax/strategies/mr15_ga.py) | [!
 [Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | Simple Gaussian | [Rechenberg (1978)](https://
-link.springer.com/chapter/10.1007/978-3-642-81283-5_8) | [`SimpleES`](https://
-github.com/RobertTLange/evosax/tree/main/evosax/strategies/simple_es.py) | [!
-[Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | DES | [Lange et al. (2023)](https://arxiv.org/
-abs/2211.11260) | [`DES`](https://github.com/RobertTLange/evosax/tree/main/
-evosax/strategies/des.py) | [![Colab](https://colab.research.google.com/assets/
+01_classic_benchmark.ipynb) | LGA | [Lange et al. (2023b)](https://arxiv.org/
+abs/2304.03995) | [`LGA`](https://github.com/RobertTLange/evosax/tree/main/
+evosax/strategies/lga.py) | [![Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/
+blob/main/examples/01_classic_benchmark.ipynb) | Simple Gaussian | [Rechenberg
+(1978)](https://link.springer.com/chapter/10.1007/978-3-642-81283-5_8) |
+[`SimpleES`](https://github.com/RobertTLange/evosax/tree/main/evosax/
+strategies/simple_es.py) | [![Colab](https://colab.research.google.com/assets/
 colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/
-blob/main/examples/01_classic_benchmark.ipynb) | LES | [Lange et al. (2023)]
-(https://arxiv.org/abs/2211.11260) | [`LES`](https://github.com/RobertTLange/
-evosax/tree/main/evosax/strategies/les.py) | [![Colab](https://
+blob/main/examples/01_classic_benchmark.ipynb) | DES | [Lange et al. (2023a)]
+(https://arxiv.org/abs/2211.11260) | [`DES`](https://github.com/RobertTLange/
+evosax/tree/main/evosax/strategies/des.py) | [![Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | Particle Swarm Optimization | [Kennedy & Eberhart
-(1995)](https://ieeexplore.ieee.org/document/488968) | [`PSO`](https://
-github.com/RobertTLange/evosax/tree/main/evosax/strategies/pso.py) | [![Colab]
-(https://colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | Differential Evolution | [Storn & Price (1997)]
-(https://www.metabolic-economics.de/pages/seminar_theoretische_biologie_2007/
-literatur/schaber/Storn1997JGlobOpt11.pdf) | [`DE`](https://github.com/
-RobertTLange/evosax/tree/main/evosax/strategies/de.py) | [![Colab](https://
+01_classic_benchmark.ipynb) | LES | [Lange et al. (202a3)](https://arxiv.org/
+abs/2211.11260) | [`LES`](https://github.com/RobertTLange/evosax/tree/main/
+evosax/strategies/les.py) | [![Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/
+blob/main/examples/01_classic_benchmark.ipynb) | Particle Swarm Optimization |
+[Kennedy & Eberhart (1995)](https://ieeexplore.ieee.org/document/488968) |
+[`PSO`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/
+pso.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/github/RobertTLange/evosax/blob/main/
+examples/01_classic_benchmark.ipynb) | Differential Evolution | [Storn & Price
+(1997)](https://www.metabolic-economics.de/pages/
+seminar_theoretische_biologie_2007/literatur/schaber/Storn1997JGlobOpt11.pdf) |
+[`DE`](https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/
+de.py) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/github/RobertTLange/evosax/blob/main/
+examples/01_classic_benchmark.ipynb) | GLD | [Golovin et al. (2019)](https://
+arxiv.org/pdf/1911.06317.pdf) | [`GLD`](https://github.com/RobertTLange/evosax/
+tree/main/evosax/strategies/gld.py) | [![Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | GLD | [Golovin et al. (2019)](https://arxiv.org/
-pdf/1911.06317.pdf) | [`GLD`](https://github.com/RobertTLange/evosax/tree/main/
-evosax/strategies/gld.py) | [![Colab](https://colab.research.google.com/assets/
+01_classic_benchmark.ipynb) | Simulated Annealing | [Rasdi Rere et al. (2015)]
+(https://www.sciencedirect.com/science/article/pii/S1877050915035759) |
+[`SimAnneal`](https://github.com/RobertTLange/evosax/tree/main/evosax/
+strategies/sim_anneal.py) | [![Colab](https://colab.research.google.com/assets/
 colab-badge.svg)](https://colab.research.google.com/github/RobertTLange/evosax/
-blob/main/examples/01_classic_benchmark.ipynb) | Simulated Annealing | [Rasdi
-Rere et al. (2015)](https://www.sciencedirect.com/science/article/pii/
-S1877050915035759) | [`SimAnneal`](https://github.com/RobertTLange/evosax/tree/
-main/evosax/strategies/sim_anneal.py) | [![Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
+blob/main/examples/01_classic_benchmark.ipynb) | Population-Based Training |
+[Jaderberg et al. (2017)](https://arxiv.org/abs/1711.09846) | [`PBT`](https://
+github.com/RobertTLange/evosax/tree/main/evosax/strategies/pbt.py) | [![Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-01_classic_benchmark.ipynb) | Population-Based Training | [Jaderberg et al.
-(2017)](https://arxiv.org/abs/1711.09846) | [`PBT`](https://github.com/
-RobertTLange/evosax/tree/main/evosax/strategies/pbt.py) | [![Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
+05_quadratic_pbt.ipynb) | Random Search | [Bergstra & Bengio (2012)](https://
+www.jmlr.org/papers/volume13/bergstra12a/bergstra12a.pdf) | [`RandomSearch`]
+(https://github.com/RobertTLange/evosax/tree/main/evosax/strategies/random.py)
+| [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/RobertTLange/evosax/blob/main/examples/
-05_quadratic_pbt.ipynb) ## Installation â³ The latest `evosax` release can
+01_classic_benchmark.ipynb) ## Installation â³ The latest `evosax` release can
 directly be installed from PyPI: ``` pip install evosax ``` If you want to get
 the most recent commit, please install directly from the repository: ``` pip
 install git+https://github.com/RobertTLange/evosax.git@main ``` In order to use
 JAX on your accelerators, you can find more details in the [JAX documentation]
 (https://github.com/google/jax#installation). ## Examples ð * ð [Classic
 ES Tasks](https://github.com/RobertTLange/evosax/blob/main/examples/
 01_classic_benchmark.ipynb): API introduction on Rosenbrock function (CMA-ES,
```

### Comparing `evosax-0.1.3/evosax.egg-info/SOURCES.txt` & `evosax-0.1.4/evosax.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 evosax/strategies/full_iamalgam.py
 evosax/strategies/gesmr_ga.py
 evosax/strategies/gld.py
 evosax/strategies/guided_es.py
 evosax/strategies/indep_iamalgam.py
 evosax/strategies/ipop_cma_es.py
 evosax/strategies/les.py
+evosax/strategies/lga.py
 evosax/strategies/lm_ma_es.py
 evosax/strategies/ma_es.py
 evosax/strategies/mr15_ga.py
 evosax/strategies/open_es.py
 evosax/strategies/pbt.py
 evosax/strategies/persistent_es.py
 evosax/strategies/pgpe.py
@@ -57,19 +58,19 @@
 evosax/strategies/samr_ga.py
 evosax/strategies/sep_cma_es.py
 evosax/strategies/sim_anneal.py
 evosax/strategies/simple_es.py
 evosax/strategies/simple_ga.py
 evosax/strategies/snes.py
 evosax/strategies/xnes.py
-evosax/strategies/ckpt/2023_03_les_v1.pkl
 evosax/strategies/ckpt/__init__.py
 evosax/utils/__init__.py
 evosax/utils/eigen_decomp.py
 evosax/utils/es_logger.py
 evosax/utils/evojax_wrapper.py
 evosax/utils/helpers.py
-evosax/utils/learned_eo.py
+evosax/utils/les_tools.py
+evosax/utils/lga_tools.py
 evosax/utils/optimizer.py
 evosax/utils/reshape_fitness.py
 evosax/utils/reshape_params.py
 evosax/utils/visualizer_2d.py
```

### Comparing `evosax-0.1.3/setup.py` & `evosax-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         "jax>=0.3.0",
         "jaxlib>=0.3.0",
         "chex",
         "flax",
         "numpy",
         "pyyaml",
         "pickle5; python_version < '3.8'",
+        "matplotlib",
     ],
 )
 
 setup(
     name="evosax",
     version=verstr,
     author="Robert Tjarko Lange",
```

