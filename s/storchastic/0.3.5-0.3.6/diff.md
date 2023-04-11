# Comparing `tmp/storchastic-0.3.5.tar.gz` & `tmp/storchastic-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/storchastic-0.3.5.tar", last modified: Tue Jul 20 08:37:57 2021, max compression
+gzip compressed data, was "storchastic-0.3.6.tar", last modified: Tue Apr 11 12:46:51 2023, max compression
```

## Comparing `storchastic-0.3.5.tar` & `storchastic-0.3.6.tar`

### file list

```diff
@@ -1,68 +1,74 @@
-drwxr-xr-x   0 emile      (501) staff       (20)        0 2021-07-20 08:37:57.965242 storchastic-0.3.5/
--rw-r--r--   0 emile      (501) staff       (20)     6321 2021-07-20 08:37:57.964881 storchastic-0.3.5/PKG-INFO
--rw-r--r--   0 emile      (501) staff       (20)     5132 2021-07-20 08:07:42.000000 storchastic-0.3.5/README.md
-drwxr-xr-x   0 emile      (501) staff       (20)        0 2021-07-20 08:37:57.930017 storchastic-0.3.5/examples/
--rw-r--r--   0 emile      (501) staff       (20)        0 2020-02-05 12:57:33.000000 storchastic-0.3.5/examples/__init__.py
--rw-r--r--   0 emile      (501) staff       (20)     1012 2020-05-29 14:43:06.000000 storchastic-0.3.5/examples/bernoulli_grad_var.py
--rw-r--r--   0 emile      (501) staff       (20)     1177 2020-11-17 09:03:12.000000 storchastic-0.3.5/examples/bernoulli_toy.py
--rw-r--r--   0 emile      (501) staff       (20)     2002 2021-05-26 08:21:02.000000 storchastic-0.3.5/examples/introduction.py
-drwxr-xr-x   0 emile      (501) staff       (20)        0 2021-07-20 08:37:57.933902 storchastic-0.3.5/examples/vae/
--rw-r--r--   0 emile      (501) staff       (20)       69 2020-03-31 15:25:48.000000 storchastic-0.3.5/examples/vae/__init__.py
--rw-r--r--   0 emile      (501) staff       (20)     2927 2021-05-27 07:57:17.000000 storchastic-0.3.5/examples/vae/bernoulli_vae.py
--rw-r--r--   0 emile      (501) staff       (20)     2883 2021-05-25 09:00:47.000000 storchastic-0.3.5/examples/vae/discrete_vae.py
--rw-r--r--   0 emile      (501) staff       (20)     1495 2020-04-09 11:33:08.000000 storchastic-0.3.5/examples/vae/normal_vae.py
--rw-r--r--   0 emile      (501) staff       (20)     9357 2021-05-26 12:00:18.000000 storchastic-0.3.5/examples/vae/train.py
--rw-r--r--   0 emile      (501) staff       (20)     3677 2021-05-25 08:04:51.000000 storchastic-0.3.5/examples/vae/vae.py
--rw-r--r--   0 emile      (501) staff       (20)     3589 2020-09-08 09:18:30.000000 storchastic-0.3.5/examples/vae_reference.py
--rw-r--r--   0 emile      (501) staff       (20)       38 2021-07-20 08:37:57.965416 storchastic-0.3.5/setup.cfg
--rw-r--r--   0 emile      (501) staff       (20)      780 2021-07-20 08:37:40.000000 storchastic-0.3.5/setup.py
-drwxr-xr-x   0 emile      (501) staff       (20)        0 2021-07-20 08:37:57.939781 storchastic-0.3.5/storch/
--rw-r--r--   0 emile      (501) staff       (20)     2286 2021-07-20 08:24:09.000000 storchastic-0.3.5/storch/__init__.py
--rw-r--r--   0 emile      (501) staff       (20)      110 2020-03-06 15:26:57.000000 storchastic-0.3.5/storch/exceptions.py
--rw-r--r--   0 emile      (501) staff       (20)     2581 2020-06-11 15:05:01.000000 storchastic-0.3.5/storch/excluded_init.py
--rw-r--r--   0 emile      (501) staff       (20)    10339 2021-07-20 08:07:42.000000 storchastic-0.3.5/storch/inference.py
-drwxr-xr-x   0 emile      (501) staff       (20)        0 2021-07-20 08:37:57.945218 storchastic-0.3.5/storch/method/
--rw-r--r--   0 emile      (501) staff       (20)      483 2021-04-13 09:24:53.000000 storchastic-0.3.5/storch/method/__init__.py
--rw-r--r--   0 emile      (501) staff       (20)     6185 2021-05-25 12:27:07.000000 storchastic-0.3.5/storch/method/arm.py
--rw-r--r--   0 emile      (501) staff       (20)     1706 2021-05-18 12:22:33.000000 storchastic-0.3.5/storch/method/baseline.py
--rw-r--r--   0 emile      (501) staff       (20)    23687 2021-07-20 08:07:42.000000 storchastic-0.3.5/storch/method/method.py
--rw-r--r--   0 emile      (501) staff       (20)     3199 2021-05-25 11:47:11.000000 storchastic-0.3.5/storch/method/multi_sample_reinforce.py
--rw-r--r--   0 emile      (501) staff       (20)    15668 2021-07-20 08:07:10.000000 storchastic-0.3.5/storch/method/relax.py
--rw-r--r--   0 emile      (501) staff       (20)     4851 2021-05-25 15:25:36.000000 storchastic-0.3.5/storch/method/unordered.py
-drwxr-xr-x   0 emile      (501) staff       (20)        0 2021-07-20 08:37:57.946585 storchastic-0.3.5/storch/nn/
--rw-r--r--   0 emile      (501) staff       (20)       43 2020-03-06 15:26:57.000000 storchastic-0.3.5/storch/nn/__init__.py
--rw-r--r--   0 emile      (501) staff       (20)     2055 2021-05-25 07:59:02.000000 storchastic-0.3.5/storch/nn/losses.py
-drwxr-xr-x   0 emile      (501) staff       (20)        0 2021-07-20 08:37:57.950716 storchastic-0.3.5/storch/sampling/
--rw-r--r--   0 emile      (501) staff       (20)      251 2021-04-13 09:24:53.000000 storchastic-0.3.5/storch/sampling/__init__.py
--rw-r--r--   0 emile      (501) staff       (20)     2947 2021-05-10 10:26:11.000000 storchastic-0.3.5/storch/sampling/expect.py
--rw-r--r--   0 emile      (501) staff       (20)     4934 2021-05-25 08:29:40.000000 storchastic-0.3.5/storch/sampling/method.py
--rw-r--r--   0 emile      (501) staff       (20)    27323 2021-05-10 10:26:11.000000 storchastic-0.3.5/storch/sampling/seq.py
--rw-r--r--   0 emile      (501) staff       (20)    13085 2021-05-10 10:26:11.000000 storchastic-0.3.5/storch/sampling/swor.py
--rw-r--r--   0 emile      (501) staff       (20)     5777 2021-05-25 15:20:15.000000 storchastic-0.3.5/storch/sampling/unordered_set.py
--rw-r--r--   0 emile      (501) staff       (20)    10376 2021-07-20 08:07:42.000000 storchastic-0.3.5/storch/storch.py
--rw-r--r--   0 emile      (501) staff       (20)    28817 2021-07-20 08:07:42.000000 storchastic-0.3.5/storch/tensor.py
--rw-r--r--   0 emile      (501) staff       (20)      651 2020-06-05 15:07:24.000000 storchastic-0.3.5/storch/typing.py
--rw-r--r--   0 emile      (501) staff       (20)     4006 2020-05-29 14:43:06.000000 storchastic-0.3.5/storch/unique.py
--rw-r--r--   0 emile      (501) staff       (20)    10017 2021-07-20 08:07:42.000000 storchastic-0.3.5/storch/util.py
--rw-r--r--   0 emile      (501) staff       (20)    19369 2021-07-20 08:27:20.000000 storchastic-0.3.5/storch/wrappers.py
-drwxr-xr-x   0 emile      (501) staff       (20)        0 2021-07-20 08:37:57.952378 storchastic-0.3.5/storchastic.egg-info/
--rw-r--r--   0 emile      (501) staff       (20)     6321 2021-07-20 08:37:57.000000 storchastic-0.3.5/storchastic.egg-info/PKG-INFO
--rw-r--r--   0 emile      (501) staff       (20)     1315 2021-07-20 08:37:57.000000 storchastic-0.3.5/storchastic.egg-info/SOURCES.txt
--rw-r--r--   0 emile      (501) staff       (20)        1 2021-07-20 08:37:57.000000 storchastic-0.3.5/storchastic.egg-info/dependency_links.txt
--rw-r--r--   0 emile      (501) staff       (20)       16 2021-07-20 08:37:57.000000 storchastic-0.3.5/storchastic.egg-info/requires.txt
--rw-r--r--   0 emile      (501) staff       (20)       21 2021-07-20 08:37:57.000000 storchastic-0.3.5/storchastic.egg-info/top_level.txt
-drwxr-xr-x   0 emile      (501) staff       (20)        0 2021-07-20 08:37:57.964125 storchastic-0.3.5/test/
--rw-r--r--   0 emile      (501) staff       (20)        0 2020-01-29 12:42:12.000000 storchastic-0.3.5/test/__init__.py
--rw-r--r--   0 emile      (501) staff       (20)    12515 2021-07-20 08:07:10.000000 storchastic-0.3.5/test/collect_env.py
--rw-r--r--   0 emile      (501) staff       (20)     2732 2021-07-20 08:07:10.000000 storchastic-0.3.5/test/is_unbiased.py
--rw-r--r--   0 emile      (501) staff       (20)      496 2020-02-27 16:05:39.000000 storchastic-0.3.5/test/pyro_enum.py
--rw-r--r--   0 emile      (501) staff       (20)     1177 2020-05-18 09:55:31.000000 storchastic-0.3.5/test/test.py
--rw-r--r--   0 emile      (501) staff       (20)      924 2021-07-20 08:07:42.000000 storchastic-0.3.5/test/test2.py
--rw-r--r--   0 emile      (501) staff       (20)      975 2020-04-23 14:54:53.000000 storchastic-0.3.5/test/test_allowed.py
--rw-r--r--   0 emile      (501) staff       (20)      332 2021-04-13 09:24:53.000000 storchastic-0.3.5/test/test_broadcast_all.py
--rw-r--r--   0 emile      (501) staff       (20)     3005 2020-05-18 09:55:31.000000 storchastic-0.3.5/test/test_swor.py
--rw-r--r--   0 emile      (501) staff       (20)     2411 2020-05-29 14:43:06.000000 storchastic-0.3.5/test/test_tensor.py
--rw-r--r--   0 emile      (501) staff       (20)      921 2021-07-20 08:07:42.000000 storchastic-0.3.5/test/testancestral.py
--rw-r--r--   0 emile      (501) staff       (20)     1109 2021-04-19 13:18:25.000000 storchastic-0.3.5/test/testcat.py
--rw-r--r--   0 emile      (501) staff       (20)      331 2021-07-20 08:07:42.000000 storchastic-0.3.5/test/testmanycosts.py
--rw-r--r--   0 emile      (501) staff       (20)      513 2021-07-20 08:07:42.000000 storchastic-0.3.5/test/testrelax.py
+drwxr-xr-x   0 emile      (501) staff       (20)        0 2023-04-11 12:46:51.314044 storchastic-0.3.6/
+-rw-r--r--   0 emile      (501) staff       (20)    35149 2020-01-29 10:30:44.000000 storchastic-0.3.6/LICENSE
+-rw-r--r--   0 emile      (501) staff       (20)     5616 2023-04-11 12:46:51.313634 storchastic-0.3.6/PKG-INFO
+-rw-r--r--   0 emile      (501) staff       (20)     5149 2022-09-06 08:15:51.000000 storchastic-0.3.6/README.md
+drwxr-xr-x   0 emile      (501) staff       (20)        0 2023-04-11 12:46:51.287133 storchastic-0.3.6/examples/
+-rw-r--r--   0 emile      (501) staff       (20)        0 2020-02-05 12:57:33.000000 storchastic-0.3.6/examples/__init__.py
+-rw-r--r--   0 emile      (501) staff       (20)     1012 2020-05-29 14:43:06.000000 storchastic-0.3.6/examples/bernoulli_grad_var.py
+-rw-r--r--   0 emile      (501) staff       (20)     1177 2020-11-17 09:03:12.000000 storchastic-0.3.6/examples/bernoulli_toy.py
+-rw-r--r--   0 emile      (501) staff       (20)     2002 2021-05-26 08:21:02.000000 storchastic-0.3.6/examples/introduction.py
+-rw-r--r--   0 emile      (501) staff       (20)     7533 2022-05-03 10:01:15.000000 storchastic-0.3.6/examples/someone_test_file.py
+drwxr-xr-x   0 emile      (501) staff       (20)        0 2023-04-11 12:46:51.291813 storchastic-0.3.6/examples/vae/
+-rw-r--r--   0 emile      (501) staff       (20)       69 2020-03-31 15:25:48.000000 storchastic-0.3.6/examples/vae/__init__.py
+-rw-r--r--   0 emile      (501) staff       (20)     2927 2021-05-27 07:57:17.000000 storchastic-0.3.6/examples/vae/bernoulli_vae.py
+-rw-r--r--   0 emile      (501) staff       (20)     2883 2021-05-25 09:00:47.000000 storchastic-0.3.6/examples/vae/discrete_vae.py
+-rw-r--r--   0 emile      (501) staff       (20)     1510 2023-03-07 16:05:37.000000 storchastic-0.3.6/examples/vae/normal_vae.py
+-rw-r--r--   0 emile      (501) staff       (20)     3595 2023-03-13 09:39:53.000000 storchastic-0.3.6/examples/vae/sample_k.py
+-rw-r--r--   0 emile      (501) staff       (20)     9357 2021-05-26 12:00:18.000000 storchastic-0.3.6/examples/vae/train.py
+-rw-r--r--   0 emile      (501) staff       (20)     3702 2023-03-07 16:08:01.000000 storchastic-0.3.6/examples/vae/vae.py
+-rw-r--r--   0 emile      (501) staff       (20)     3589 2020-09-08 09:18:30.000000 storchastic-0.3.6/examples/vae_reference.py
+-rw-r--r--   0 emile      (501) staff       (20)       38 2023-04-11 12:46:51.314264 storchastic-0.3.6/setup.cfg
+-rw-r--r--   0 emile      (501) staff       (20)      784 2023-04-11 12:46:41.000000 storchastic-0.3.6/setup.py
+drwxr-xr-x   0 emile      (501) staff       (20)        0 2023-04-11 12:46:51.296426 storchastic-0.3.6/storch/
+-rw-r--r--   0 emile      (501) staff       (20)     2351 2022-06-23 12:33:33.000000 storchastic-0.3.6/storch/__init__.py
+-rw-r--r--   0 emile      (501) staff       (20)      110 2020-03-06 15:26:57.000000 storchastic-0.3.6/storch/exceptions.py
+-rw-r--r--   0 emile      (501) staff       (20)     2581 2020-06-11 15:05:01.000000 storchastic-0.3.6/storch/excluded_init.py
+-rw-r--r--   0 emile      (501) staff       (20)    10610 2022-09-06 08:14:01.000000 storchastic-0.3.6/storch/inference.py
+drwxr-xr-x   0 emile      (501) staff       (20)        0 2023-04-11 12:46:51.300587 storchastic-0.3.6/storch/method/
+-rw-r--r--   0 emile      (501) staff       (20)      537 2022-06-21 10:31:18.000000 storchastic-0.3.6/storch/method/__init__.py
+-rw-r--r--   0 emile      (501) staff       (20)     6195 2022-05-02 08:32:39.000000 storchastic-0.3.6/storch/method/arm.py
+-rw-r--r--   0 emile      (501) staff       (20)     1706 2021-05-18 12:22:33.000000 storchastic-0.3.6/storch/method/baseline.py
+-rw-r--r--   0 emile      (501) staff       (20)    24066 2022-06-23 10:21:50.000000 storchastic-0.3.6/storch/method/method.py
+-rw-r--r--   0 emile      (501) staff       (20)     3460 2022-06-21 09:27:16.000000 storchastic-0.3.6/storch/method/multi_sample_reinforce.py
+-rw-r--r--   0 emile      (501) staff       (20)     1163 2022-06-21 15:32:27.000000 storchastic-0.3.6/storch/method/rao_blackwell.py
+-rw-r--r--   0 emile      (501) staff       (20)    15902 2022-05-03 08:50:30.000000 storchastic-0.3.6/storch/method/relax.py
+-rw-r--r--   0 emile      (501) staff       (20)     3862 2022-06-21 09:27:31.000000 storchastic-0.3.6/storch/method/unordered.py
+drwxr-xr-x   0 emile      (501) staff       (20)        0 2023-04-11 12:46:51.301438 storchastic-0.3.6/storch/nn/
+-rw-r--r--   0 emile      (501) staff       (20)       43 2020-03-06 15:26:57.000000 storchastic-0.3.6/storch/nn/__init__.py
+-rw-r--r--   0 emile      (501) staff       (20)     2055 2021-05-25 07:59:02.000000 storchastic-0.3.6/storch/nn/losses.py
+drwxr-xr-x   0 emile      (501) staff       (20)        0 2023-04-11 12:46:51.304675 storchastic-0.3.6/storch/sampling/
+-rw-r--r--   0 emile      (501) staff       (20)      306 2022-06-21 09:17:14.000000 storchastic-0.3.6/storch/sampling/__init__.py
+-rw-r--r--   0 emile      (501) staff       (20)     2947 2021-05-10 10:26:11.000000 storchastic-0.3.6/storch/sampling/expect.py
+-rw-r--r--   0 emile      (501) staff       (20)     4784 2022-01-27 11:49:05.000000 storchastic-0.3.6/storch/sampling/importance_sampling.py
+-rw-r--r--   0 emile      (501) staff       (20)     4900 2022-06-21 16:06:23.000000 storchastic-0.3.6/storch/sampling/mapo.py
+-rw-r--r--   0 emile      (501) staff       (20)     5103 2022-06-23 15:20:18.000000 storchastic-0.3.6/storch/sampling/method.py
+-rw-r--r--   0 emile      (501) staff       (20)    30171 2022-06-24 11:12:25.000000 storchastic-0.3.6/storch/sampling/seq.py
+-rw-r--r--   0 emile      (501) staff       (20)    13676 2022-06-24 14:03:22.000000 storchastic-0.3.6/storch/sampling/swor.py
+-rw-r--r--   0 emile      (501) staff       (20)     5493 2022-06-24 10:33:02.000000 storchastic-0.3.6/storch/sampling/unordered_set.py
+-rw-r--r--   0 emile      (501) staff       (20)    10837 2022-01-28 16:04:06.000000 storchastic-0.3.6/storch/storch.py
+-rw-r--r--   0 emile      (501) staff       (20)    29802 2022-09-06 08:08:17.000000 storchastic-0.3.6/storch/tensor.py
+-rw-r--r--   0 emile      (501) staff       (20)      651 2020-06-05 15:07:24.000000 storchastic-0.3.6/storch/typing.py
+-rw-r--r--   0 emile      (501) staff       (20)     4006 2020-05-29 14:43:06.000000 storchastic-0.3.6/storch/unique.py
+-rw-r--r--   0 emile      (501) staff       (20)    10072 2022-06-23 09:40:40.000000 storchastic-0.3.6/storch/util.py
+-rw-r--r--   0 emile      (501) staff       (20)    21173 2022-06-21 12:06:57.000000 storchastic-0.3.6/storch/wrappers.py
+drwxr-xr-x   0 emile      (501) staff       (20)        0 2023-04-11 12:46:51.306486 storchastic-0.3.6/storchastic.egg-info/
+-rw-r--r--   0 emile      (501) staff       (20)     5616 2023-04-11 12:46:51.000000 storchastic-0.3.6/storchastic.egg-info/PKG-INFO
+-rw-r--r--   0 emile      (501) staff       (20)     1472 2023-04-11 12:46:51.000000 storchastic-0.3.6/storchastic.egg-info/SOURCES.txt
+-rw-r--r--   0 emile      (501) staff       (20)        1 2023-04-11 12:46:51.000000 storchastic-0.3.6/storchastic.egg-info/dependency_links.txt
+-rw-r--r--   0 emile      (501) staff       (20)       32 2023-04-11 12:46:51.000000 storchastic-0.3.6/storchastic.egg-info/requires.txt
+-rw-r--r--   0 emile      (501) staff       (20)       21 2023-04-11 12:46:51.000000 storchastic-0.3.6/storchastic.egg-info/top_level.txt
+drwxr-xr-x   0 emile      (501) staff       (20)        0 2023-04-11 12:46:51.313007 storchastic-0.3.6/test/
+-rw-r--r--   0 emile      (501) staff       (20)        0 2020-01-29 12:42:12.000000 storchastic-0.3.6/test/__init__.py
+-rw-r--r--   0 emile      (501) staff       (20)    12515 2021-07-20 08:07:10.000000 storchastic-0.3.6/test/collect_env.py
+-rw-r--r--   0 emile      (501) staff       (20)     2732 2021-07-20 08:07:10.000000 storchastic-0.3.6/test/is_unbiased.py
+-rw-r--r--   0 emile      (501) staff       (20)      496 2020-02-27 16:05:39.000000 storchastic-0.3.6/test/pyro_enum.py
+-rw-r--r--   0 emile      (501) staff       (20)     1177 2020-05-18 09:55:31.000000 storchastic-0.3.6/test/test.py
+-rw-r--r--   0 emile      (501) staff       (20)      924 2021-07-20 08:07:42.000000 storchastic-0.3.6/test/test2.py
+-rw-r--r--   0 emile      (501) staff       (20)      975 2020-04-23 14:54:53.000000 storchastic-0.3.6/test/test_allowed.py
+-rw-r--r--   0 emile      (501) staff       (20)      332 2021-04-13 09:24:53.000000 storchastic-0.3.6/test/test_broadcast_all.py
+-rw-r--r--   0 emile      (501) staff       (20)     3005 2020-05-18 09:55:31.000000 storchastic-0.3.6/test/test_swor.py
+-rw-r--r--   0 emile      (501) staff       (20)     2411 2020-05-29 14:43:06.000000 storchastic-0.3.6/test/test_tensor.py
+-rw-r--r--   0 emile      (501) staff       (20)      921 2021-07-20 08:07:42.000000 storchastic-0.3.6/test/testancestral.py
+-rw-r--r--   0 emile      (501) staff       (20)     1109 2021-04-19 13:18:25.000000 storchastic-0.3.6/test/testcat.py
+-rw-r--r--   0 emile      (501) staff       (20)      331 2021-07-20 08:07:42.000000 storchastic-0.3.6/test/testmanycosts.py
+-rw-r--r--   0 emile      (501) staff       (20)      513 2021-07-20 08:07:42.000000 storchastic-0.3.6/test/testrelax.py
```

### Comparing `storchastic-0.3.5/PKG-INFO` & `storchastic-0.3.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,101 @@
 Metadata-Version: 2.1
 Name: storchastic
-Version: 0.3.5
+Version: 0.3.6
 Summary: Stochastic Deep Learning for PyTorch
 Home-page: https://github.com/HEmile/storchastic
 Author: Emile van Krieken
 Author-email: e.van.krieken@vu.nl
-License: UNKNOWN
-Description: ![](logo.png)
-        
-        
-        
-        
-        ## General Stochastic Automatic Differentiation for Pytorch
-        [![Documentation Status](https://readthedocs.org/projects/storchastic/badge/?version=latest)](https://storchastic.readthedocs.io/en/latest/?badge=latest)
-        
-        - [Documentation](https://storchastic.readthedocs.io/en/latest/)
-        - [Read the paper](https://arxiv.org/abs/2104.00428)
-        
-        **Storchastic** is a PyTorch library for stochastic gradient estimation in Deep Learning [1]. Many state of the art deep learning
-        models use gradient estimation, in particular within the fields of Variational Inference and Reinforcement Learning.
-        While PyTorch computes gradients of deterministic computation graphs automatically, it will not estimate
-        gradients on **stochastic computation graphs** [2].
-        
-        With Storchastic, you can easily define any stochastic deep learning model and let it estimate the gradients for you. 
-        Storchastic provides a large range of gradient estimation methods that you can plug and play, to figure out which one works
-        best for your problem. Storchastic provides automatic broadcasting of sampled batch dimensions, which increases code
-        readability and allows implementing complex models with ease.
-        
-        When dealing with continuous random variables and differentiable functions, the popular reparameterization method [3] is usually
-        very effective. However, this method is not applicable when dealing with discrete random variables or non-differentiable functions.
-        This is why Storchastic has a focus on gradient estimators for discrete random variables, non-differentiable functions and
-        sequence models.
-        
-        
-        [Documentation on Read the Docs.](https://storchastic.readthedocs.io/en/latest/)
-        
-        [Example: Discrete Variational Auto-Encoder](TODO)
-        
-        ## Installation
-        In your virtual Python environment, run
-        `pip install storchastic`
-        
-        **Requires** Pytorch 1.**8** and [Pyro](http://pyro.ai). The code is build using Python 3.8.
-        
-        ## Algorithms
-        Feel free to create an issue if an estimator is missing here.
-        - Reparameterization [1, 3]
-        - Score Function (REINFORCE) with Moving Average baseline [1, 4]
-        - Score Function with Batch Average Baseline [5, 6]
-        - Expected value for enumerable distributions
-        - (Straight through) Gumbel Softmax [7, 8]
-        - LAX, RELAX [9] 
-        - REBAR [10]
-        - REINFORCE Without Replacement [6]
-        - Unordered Set Estimator [13]
-        - ARM [15]
-        
-        ### In development
-        - Memory Augmented Policy Optimization [11]
-        - Rao-Blackwellized REINFORCE [12]
-        
-        ### Planned
-        - Measure valued derivatives [1, 14]
-        - Automatic Credit Assignment [16]
-        - ...
-        
-        ## References
-        - [1] [Monte Carlo Gradient Estimation in Machine Learning](https://arxiv.org/abs/1906.10652), Mohamed et al, 2019
-        - [2] [Gradient Estimation Using Stochastic Computation Graphs](https://arxiv.org/abs/1506.05254), Schulman et al, NeurIPS 2015
-        - [3] [Auto-Encoding Variational Bayes](https://arxiv.org/abs/1312.6114), Kingma and Welling, ICLR 2014
-        - [4] [Simple statistical gradient-following algorithms for connectionist reinforcement learning](https://link-springer-com.vu-nl.idm.oclc.org/article/10.1007/BF00992696), Williams, Machine Learning 1992
-        - [5] [Variational inference for Monte Carlo objectives](https://arxiv.org/abs/1602.06725), Mnih and Rezende, ICML 2016
-        - [6] [Buy 4 REINFORCE Samples, Get a Baseline for Free!](https://openreview.net/pdf?id=r1lgTGL5DE), Kool et al, ICLR Workshop dlStructPred 2019
-        - [7] [Categorical Reparameterization with Gumbel-Softmax](https://arxiv.org/abs/1611.01144), Jang et al, ICLR 2017
-        - [8] [The Concrete Distribution: A Continuous Relaxation of Discrete Random Variables](https://arxiv.org/abs/1611.00712), Maddison et al, ICLR 2017
-        - [9] [Backpropagation through the Void: Optimizing control variates for black-box gradient estimation](https://arxiv.org/abs/1711.00123), Grathwohl et al, ICLR 2018
-        - [10] [REBAR: Low-variance, unbiased gradient estimates for discrete latent variable models](https://arxiv.org/abs/1703.07370), Tucker et al, NeurIPS 2017
-        - [11] [Memory Augmented Policy Optimization for Program Synthesis and Semantic Parsing](https://arxiv.org/abs/1807.02322), Liang et al, NeurIPS 2018
-        - [12] [Rao-Blackwellized Stochastic Gradients for Discrete Distributions](https://arxiv.org/abs/1810.04777), Liu et al, ICML 2019
-        - [13] [Estimating Gradients for Discrete Random Variables by Sampling without Replacement](https://openreview.net/forum?id=rklEj2EFvB), Kool et al, ICLR 2020
-        - [14] [Measure-Valued Derivatives for Approximate Bayesian Inference](http://bayesiandeeplearning.org/2019/papers/76.pdf), Rosca et al, Workshop on Bayesian Deep Learning (NeurIPS 2019)
-        - [15] [ARM: Augment-REINFORCE-Merge Gradient for Stochastic Binary Networks](https://arxiv.org/abs/1807.11143), Yin and Zhou, ICLR 2019
-        - [16] [Credit Assignment Techniques in Stochastic Computation Graphs](https://arxiv.org/abs/1901.01761), Weber et al, AISTATS 2019
-        
-        ## Cite
-        To cite Storchastic, please cite this preprint:
-        ```
-        @article{van2021storchastic,
-          title={Storchastic: A Framework for General Stochastic Automatic Differentiation},
-          author={van Krieken, Emile and Tomczak, Jakub M and Teije, Annette ten},
-          journal={arXiv preprint arXiv:2104.00428},
-          year={2021}
-        }
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![](logo.png)
+
+
+
+
+## General Stochastic Automatic Differentiation for Pytorch
+[![Documentation Status](https://readthedocs.org/projects/storchastic/badge/?version=latest)](https://storchastic.readthedocs.io/en/latest/?badge=latest)
+
+- [Documentation](https://storchastic.readthedocs.io/en/latest/)
+- [Read the paper](https://arxiv.org/abs/2104.00428)
+
+**Storchastic** is a PyTorch library for stochastic gradient estimation in Deep Learning [1]. Many state of the art deep learning
+models use gradient estimation, in particular within the fields of Variational Inference and Reinforcement Learning.
+While PyTorch computes gradients of deterministic computation graphs automatically, it will not estimate
+gradients on **stochastic computation graphs** [2].
+
+With Storchastic, you can easily define any stochastic deep learning model and let it estimate the gradients for you. 
+Storchastic provides a large range of gradient estimation methods that you can plug and play, to figure out which one works
+best for your problem. Storchastic provides automatic broadcasting of sampled batch dimensions, which increases code
+readability and allows implementing complex models with ease.
+
+When dealing with continuous random variables and differentiable functions, the popular reparameterization method [3] is usually
+very effective. However, this method is not applicable when dealing with discrete random variables or non-differentiable functions.
+This is why Storchastic has a focus on gradient estimators for discrete random variables, non-differentiable functions and
+sequence models.
+
+
+[Documentation on Read the Docs.](https://storchastic.readthedocs.io/en/latest/)
+
+[Example: Discrete Variational Auto-Encoder](examples/vae/train.py)
+
+## Installation
+In your virtual Python environment, run
+`pip install storchastic`
+
+**Requires** Pytorch 1.**8** and [Pyro](http://pyro.ai). The code is build using Python 3.8.
+
+## Algorithms
+Feel free to create an issue if an estimator is missing here.
+- Reparameterization [1, 3]
+- Score Function (REINFORCE) with Moving Average baseline [1, 4]
+- Score Function with Batch Average Baseline [5, 6]
+- Expected value for enumerable distributions
+- (Straight through) Gumbel Softmax [7, 8]
+- LAX, RELAX [9] 
+- REBAR [10]
+- REINFORCE Without Replacement [6]
+- Unordered Set Estimator [13]
+- ARM [15]
+- Rao-Blackwellized REINFORCE [12]
+
+### In development
+- Memory Augmented Policy Optimization [11]
+
+### Planned
+- Measure valued derivatives [1, 14]
+- Automatic Credit Assignment [16]
+- ...
+
+## References
+- [1] [Monte Carlo Gradient Estimation in Machine Learning](https://arxiv.org/abs/1906.10652), Mohamed et al, 2019
+- [2] [Gradient Estimation Using Stochastic Computation Graphs](https://arxiv.org/abs/1506.05254), Schulman et al, NeurIPS 2015
+- [3] [Auto-Encoding Variational Bayes](https://arxiv.org/abs/1312.6114), Kingma and Welling, ICLR 2014
+- [4] [Simple statistical gradient-following algorithms for connectionist reinforcement learning](https://link-springer-com.vu-nl.idm.oclc.org/article/10.1007/BF00992696), Williams, Machine Learning 1992
+- [5] [Variational inference for Monte Carlo objectives](https://arxiv.org/abs/1602.06725), Mnih and Rezende, ICML 2016
+- [6] [Buy 4 REINFORCE Samples, Get a Baseline for Free!](https://openreview.net/pdf?id=r1lgTGL5DE), Kool et al, ICLR Workshop dlStructPred 2019
+- [7] [Categorical Reparameterization with Gumbel-Softmax](https://arxiv.org/abs/1611.01144), Jang et al, ICLR 2017
+- [8] [The Concrete Distribution: A Continuous Relaxation of Discrete Random Variables](https://arxiv.org/abs/1611.00712), Maddison et al, ICLR 2017
+- [9] [Backpropagation through the Void: Optimizing control variates for black-box gradient estimation](https://arxiv.org/abs/1711.00123), Grathwohl et al, ICLR 2018
+- [10] [REBAR: Low-variance, unbiased gradient estimates for discrete latent variable models](https://arxiv.org/abs/1703.07370), Tucker et al, NeurIPS 2017
+- [11] [Memory Augmented Policy Optimization for Program Synthesis and Semantic Parsing](https://arxiv.org/abs/1807.02322), Liang et al, NeurIPS 2018
+- [12] [Rao-Blackwellized Stochastic Gradients for Discrete Distributions](https://arxiv.org/abs/1810.04777), Liu et al, ICML 2019
+- [13] [Estimating Gradients for Discrete Random Variables by Sampling without Replacement](https://openreview.net/forum?id=rklEj2EFvB), Kool et al, ICLR 2020
+- [14] [Measure-Valued Derivatives for Approximate Bayesian Inference](http://bayesiandeeplearning.org/2019/papers/76.pdf), Rosca et al, Workshop on Bayesian Deep Learning (NeurIPS 2019)
+- [15] [ARM: Augment-REINFORCE-Merge Gradient for Stochastic Binary Networks](https://arxiv.org/abs/1807.11143), Yin and Zhou, ICLR 2019
+- [16] [Credit Assignment Techniques in Stochastic Computation Graphs](https://arxiv.org/abs/1901.01761), Weber et al, AISTATS 2019
+
+## Cite
+To cite Storchastic, please cite this preprint:
+```
+@article{van2021storchastic,
+  title={Storchastic: A Framework for General Stochastic Automatic Differentiation},
+  author={van Krieken, Emile and Tomczak, Jakub M and Teije, Annette ten},
+  journal={arXiv preprint arXiv:2104.00428},
+  year={2021}
+}
+```
```

### Comparing `storchastic-0.3.5/README.md` & `storchastic-0.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 very effective. However, this method is not applicable when dealing with discrete random variables or non-differentiable functions.
 This is why Storchastic has a focus on gradient estimators for discrete random variables, non-differentiable functions and
 sequence models.
 
 
 [Documentation on Read the Docs.](https://storchastic.readthedocs.io/en/latest/)
 
-[Example: Discrete Variational Auto-Encoder](TODO)
+[Example: Discrete Variational Auto-Encoder](examples/vae/train.py)
 
 ## Installation
 In your virtual Python environment, run
 `pip install storchastic`
 
 **Requires** Pytorch 1.**8** and [Pyro](http://pyro.ai). The code is build using Python 3.8.
 
@@ -43,18 +43,18 @@
 - Expected value for enumerable distributions
 - (Straight through) Gumbel Softmax [7, 8]
 - LAX, RELAX [9] 
 - REBAR [10]
 - REINFORCE Without Replacement [6]
 - Unordered Set Estimator [13]
 - ARM [15]
+- Rao-Blackwellized REINFORCE [12]
 
 ### In development
 - Memory Augmented Policy Optimization [11]
-- Rao-Blackwellized REINFORCE [12]
 
 ### Planned
 - Measure valued derivatives [1, 14]
 - Automatic Credit Assignment [16]
 - ...
 
 ## References
```

### Comparing `storchastic-0.3.5/examples/bernoulli_grad_var.py` & `storchastic-0.3.6/examples/bernoulli_grad_var.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/examples/bernoulli_toy.py` & `storchastic-0.3.6/examples/bernoulli_toy.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/examples/introduction.py` & `storchastic-0.3.6/examples/introduction.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/examples/vae/bernoulli_vae.py` & `storchastic-0.3.6/examples/vae/bernoulli_vae.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/examples/vae/discrete_vae.py` & `storchastic-0.3.6/examples/vae/discrete_vae.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/examples/vae/normal_vae.py` & `storchastic-0.3.6/examples/vae/normal_vae.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,23 @@
         # *2 because we compute both the mean and stdev
         fc3 = nn.Linear(prev_layer, latents * 2)
         fc4 = nn.Linear(latents, prev_layer)
         return fc3, fc4
 
     def initialize_method(self, args) -> storch.method.Method:
         if args.method == "reparameterization":
-            return storch.Reparameterization("z", n_samples=args.samples)
+            return storch.method.Reparameterization("z", n_samples=args.samples)
         elif args.method == "lax":
-            return storch.LAX("z", n_samples=args.samples, in_dim=args.latents)
+            return storch.method.LAX("z", n_samples=args.samples, in_dim=args.latents)
         elif args.method == "score":
-            return storch.ScoreFunction(
+            return storch.method.ScoreFunction(
                 "z", n_samples=args.samples, baseline_factory=args.baseline
             )
 
-    def prior(self, posterior: Distribution) -> Distribution:
+    def prior(self, posterior: Normal) -> Distribution:
         return Normal(torch.zeros_like(posterior.loc), torch.ones_like(posterior.scale))
 
     def variational_posterior(self, params) -> Distribution:
         mean, std = params
         return Normal(mean, std)
 
     def logits_to_params(self, logits, latents):
```

### Comparing `storchastic-0.3.5/examples/vae/train.py` & `storchastic-0.3.6/examples/vae/train.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/examples/vae/vae.py` & `storchastic-0.3.6/examples/vae/vae.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import storch
 from torch.distributions import Distribution
 
 
 class VAE(nn.Module):
     def __init__(self, args):
         super(VAE, self).__init__()
+        self.args = args
 
         self.latents = args.latents
         self.samples = args.samples
         self.sampling_method = self.initialize_method(args)
         self.fc1 = nn.Linear(784, 512)
         self.fc2 = nn.Linear(512, 256)
```

### Comparing `storchastic-0.3.5/examples/vae_reference.py` & `storchastic-0.3.6/examples/vae_reference.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/setup.py` & `storchastic-0.3.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="storchastic",  # Replace with your own username
-    version="0.3.5",
+    version="0.3.6",
     author="Emile van Krieken",
     author_email="e.van.krieken@vu.nl",
     description="Stochastic Deep Learning for PyTorch",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/HEmile/storchastic",
-    install_requires=[
-      "entmax",
-      "pyro-ppl"
-    ],
+    install_requires=["entmax", "pyro-ppl", "torch", "packaging"],
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
```

### Comparing `storchastic-0.3.5/storch/__init__.py` & `storchastic-0.3.6/storch/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 )
 from .tensor import Tensor, CostTensor, StochasticTensor, Plate, is_tensor
 
 import storch.sampling
 from .storch import *
 import storch.method
 import storch.typing
-from .inference import backward, add_cost, reset, denote_independent, gather_samples
+from .inference import backward, add_cost, reset, denote_independent, gather_samples, costs
 from .util import print_graph
 
 from .unique import unique, undo_unique
 from .exceptions import IllegalStorchExposeError
 from packaging import version
 
 import storch.nn
 
 
 import torch as _torch
 import pkgutil
 import sys
 
 _debug = False
+CHECK_DIFFERENTIABLE_PATH = False
 # Hard-coded monkey patches: These do not support __torch_function__ (PyTorch version 1.5.0)
 _torch.is_tensor = storch.is_tensor
 _torch.Tensor.to = deterministic(_torch.Tensor.to)
 _torch.Tensor.le = deterministic(_torch.Tensor.le)
 _torch.Tensor.gt = deterministic(_torch.Tensor.gt)
 # Cat currently does not support __torch_function__ https://github.com/pytorch/pytorch/issues/34294.
 # However, monkey patching it makes storchastic incompatible with torchvision. Use storch.cat or storch.gather_samples instead
@@ -41,17 +42,17 @@
 # Monkey patch every occurence of broadcast_all in the PyTorch code.
 # This should not be necessesary from PyTorch 1.8.0. See https://github.com/pytorch/pytorch/pull/48169
 if version.parse(torch.__version__) < version.parse("1.8.0"):
     _torch.distributions.utils.broadcast_all = deterministic(
         _torch.distributions.utils.broadcast_all
     )
 
-# Distributions import broadcast_all by name, meaning they refer to the non-monkey patched version.
-# Loop over every distribution to apply the monkey patch.
-for module_info in pkgutil.iter_modules(_torch.distributions.__path__):
-    module = sys.modules.get("torch.distributions." + module_info.name)
-    if "broadcast_all" in module.__dict__:
-        module.broadcast_all = _torch.distributions.utils.broadcast_all
+    # Distributions import broadcast_all by name, meaning they refer to the non-monkey patched version.
+    # Loop over every distribution to apply the monkey patch.
+    for module_info in pkgutil.iter_modules(_torch.distributions.__path__):
+        module = sys.modules.get("torch.distributions." + module_info.name)
+        if "broadcast_all" in module.__dict__:
+            module.broadcast_all = _torch.distributions.utils.broadcast_all
 
 # Validating arguments is not compatible with Storchastic as it does instanceof torch.Tensor checks
 # Necessary for PyTorch versions above 1.8.0
 _torch.distributions.Distribution.set_default_validate_args(False)
```

### Comparing `storchastic-0.3.5/storch/excluded_init.py` & `storchastic-0.3.6/storch/excluded_init.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/storch/inference.py` & `storchastic-0.3.6/storch/inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,31 +80,34 @@
             weight,
         )
     return IndependentTensor(
         cat_tensors, [], [], "_indep_" + plate_name, plate_name, weight
     )
 
 
-def add_cost(cost: Tensor, name: str):
-    if cost.event_shape != ():
-        if cost.event_shape == (1,):
-            cost = cost.squeeze(-1)
-        else:
-            raise ValueError("Can only register cost functions with empty event shapes")
-    if not name:
-        raise ValueError(
-            "No name provided to register cost node. Make sure to register an unique name with the cost."
-        )
-    cost = CostTensor(cost._tensor, [cost], cost.plates, name)
+def add_cost(cost: Union[Tensor, torch.Tensor], name: str):
+    if isinstance(cost, torch.Tensor):
+        cost = CostTensor(cost, [], [], name)
+    else:
+        if cost.event_shape != ():
+            if cost.event_shape == (1,):
+                cost = cost.squeeze(-1)
+            else:
+                raise ValueError("Can only register cost functions with empty event shapes")
+        if not name:
+            raise ValueError(
+                "No name provided to register cost node. Make sure to register an unique name with the cost."
+            )
+        cost = CostTensor(cost._tensor, [cost], cost.plates, name)
     if torch.is_grad_enabled():
         storch.inference._cost_tensors.append(cost)
     return cost
 
 
-def surrogate_loss(debug: bool=False) -> storch.Tensor:
+def surrogate_loss(debug: bool = False) -> storch.Tensor:
     costs: [storch.Tensor] = storch.inference._cost_tensors
     if not costs:
         raise RuntimeError("No cost nodes registered for backward call.")
     if debug:
         print_graph(costs)
 
     # Sum of averages of cost node tensors
@@ -119,15 +122,15 @@
         # if print_costs:
         #     print(c.name, ":", reduced_cost._tensor.item())
         # total_cost += reduced_cost
         # Compute gradients for the cost nodes themselves, if they require one.
         # if reduced_cost.requires_grad:
         #     accum_loss += reduced_cost
 
-        L = c._tensor.new_tensor(0.0)
+        L = c._tensor.new_tensor(0.0, dtype=torch.float32)
         surrogate_loss_c = 0.0
         # Walk topologically through the graph
         # This is a parallelized implementation of Algorithm 1 in the paper
         for parent in c.walk_parents(depth_first=False, reverse=True):
             # Instance check here instead of parent.stochastic, as backward methods are only used on these.
             if not isinstance(parent, StochasticTensor):
                 continue
@@ -139,29 +142,29 @@
             # Transpose the parent stochastic tensor, so that its shape is the same as the cost but the event shape, and
             # possibly extra dimensions...?
             parent_tensor = parent._tensor
             reduced_cost = c
             parent_plates = parent.multi_dim_plates()
             # Reduce all plates that are in the cost node but not in the parent node
             for plate in storch.order_plates(c.multi_dim_plates(), reverse=True):
-                if plate not in parent_plates:
+                if not plate.is_in(parent_plates):
                     reduced_cost = plate.reduce(reduced_cost, detach_weights=True)
             # Align the parent tensor so that the plate dimensions are in the same order as the cost tensor
             # TODO: This can probably be implemented with torch.movedim
             for index_c, plate in enumerate(reduced_cost.multi_dim_plates()):
-                index_p = parent_plates.index(plate)
+                index_p = plate.index_in(parent_plates)
                 if index_c != index_p:
                     parent_tensor = parent_tensor.transpose(index_p, index_c)
                     parent_plates[index_p], parent_plates[index_c] = (
                         parent_plates[index_c],
                         parent_plates[index_p],
                     )
             # Add empty (k=1) plates to new parent
             for plate in parent.plates:
-                if plate not in parent_plates:
+                if not plate.is_in(parent_plates):
                     parent_plates.append(plate)
 
             # Create new storch Tensors with different order of plates for the cost and parent
             new_parent = storch.tensor.StochasticTensor(
                 parent_tensor,
                 [],
                 parent_plates,
@@ -175,37 +178,43 @@
             # Fake the new parent to be the old parent within the graph by mimicking its place in the graph
             new_parent._parents = parent._parents
             for p, has_link in new_parent._parents:
                 p._children.append((new_parent, has_link))
             new_parent._children = parent._children
 
             # Compute the estimator
-            (
-                gradient_function,
-                control_variate,
-            ) = parent.method._estimator(new_parent, reduced_cost)
+            (gradient_function, control_variate,) = parent.method._estimator(
+                new_parent, reduced_cost
+            )
 
             if gradient_function is not None:
                 L = L + gradient_function
             # Compute control variate
             if control_variate is not None:
                 final_A = magic_box(L) * control_variate
                 final_A = storch.reduce_plates(
-                    final_A, detach_weights=False,  # TODO: Should this boolean be false or true?
+                    final_A,
+                    detach_weights=False,  # TODO: Should this boolean be false or true?
                 )
                 if final_A.ndim == 1:
                     final_A = final_A.squeeze(0)
                 surrogate_loss_c += final_A
+
         # Use magic box to distribute the cost to gradient function
         surrogate_loss_c += storch.reduce_plates(magic_box(L) * c, detach_weights=False)
         # Collect surrogate losses for all costs
         surrogate_losses.append(surrogate_loss_c)
     SL = torch.sum(torch.stack(surrogate_losses))
     return SL
 
+
+def costs() -> [CostTensor]:
+    return list(storch.inference._cost_tensors)
+
+
 def backward(
     debug: bool = False,
     create_graph: bool = False,
     update_estimator_params: bool = True,
 ) -> torch.Tensor:
     """
     Computes the gradients of the cost nodes with respect to the parameter nodes. It uses the storch
@@ -228,18 +237,18 @@
     costs: [storch.Tensor] = storch.inference._cost_tensors
     for c in costs:
         for parent in c.walk_parents():
             # Instance check here instead of parent.stochastic, as backward methods are only used on these.
             if isinstance(parent, StochasticTensor):
                 stochastic_nodes.add(parent)
                 if parent.requires_grad and parent.method:
-                    create_higher_order_graph = parent.method.should_create_higher_order_graph()
-                    _create_graph = (
-                            create_higher_order_graph or _create_graph
+                    create_higher_order_graph = (
+                        parent.method.should_create_higher_order_graph()
                     )
+                    _create_graph = create_higher_order_graph or _create_graph
     if isinstance(SL, storch.Tensor) and SL._tensor.requires_grad:
         SL._tensor.backward(create_graph=_create_graph)
 
     if update_estimator_params:
         for s_node in stochastic_nodes:
             if s_node.method:
                 s_node.method._update_parameters()
```

### Comparing `storchastic-0.3.5/storch/method/arm.py` & `storchastic-0.3.6/storch/method/arm.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         # The antithetic sample is not according to the true distribution, so we cannot count it during the weighting
         n = int(tensor.n / 2)
         weighting = tensor._tensor.new_zeros((tensor.n,))
         weighting[:n] = tensor._tensor.new_tensor(1.0 / n)
         return weighting
 
     def post_sample(self, tensor: storch.StochasticTensor) -> Optional[storch.Tensor]:
-        return tensor > 0.0
+        return (tensor > 0.0).float()
 
     def comp_estimator(
         self, tensor: torch.Tensor, cost: torch.Tensor, logits: torch.Tensor, plate_index: int, n: int
     ) -> Tuple[storch.Tensor, storch.Tensor]:
         _index_z = (slice(None),) * plate_index + (slice(n),)
         _index_z_tilde = (slice(None),) * plate_index + (slice(n, 2 * n),)
         z = tensor[_index_z]
```

### Comparing `storchastic-0.3.5/storch/method/baseline.py` & `storchastic-0.3.6/storch/method/baseline.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/storch/method/method.py` & `storchastic-0.3.6/storch/method/method.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,38 +6,39 @@
 import torch
 from typing import Optional, Type, Union, Dict, List, Callable, Tuple
 from storch.util import (
     has_differentiable_path,
     get_distr_parameters,
     rsample_gumbel_softmax,
     rsample_gumbel,
+    magic_box,
 )
 import storch
 from storch.method.baseline import MovingAverageBaseline, BatchAverageBaseline, Baseline
 from storch.sampling import (
     SamplingMethod,
     MonteCarlo,
     Enumerate,
 )
 import entmax
 
 
-
 class Method(ABC, torch.nn.Module):
     """
     Base class of gradient estimation methods.
 
     A :class:`Method` is a :class:`torch.nn.Module`, and can therefore contain parameters to optimize.
     Calling them (:meth:`forward`) with a PyTorch distribution returns a sampled Tensor of type :class:`storch.StochasticTensor`
     from that distribution that will use the gradient estimator in the backward pass when :func:`storch.backward` is called.
 
     Args:
         plate_name (str): The name of the :class:`.Plate` that samples of this method will use.
         sampling_method (storch.sampling.SamplingMethod): The method to sample tensors with given an input distribution.
     """
+
     def __init__(self, plate_name: str, sampling_method: SamplingMethod):
         super().__init__()
         self._estimation_pairs = []
         self.register_buffer("iterations", torch.tensor(0, dtype=torch.long))
         self.plate_name = plate_name
         self.sampling_method = sampling_method
         if not self.sampling_method.plate_name == plate_name:
@@ -54,14 +55,15 @@
         """
         return self.sample(distr)
 
     @staticmethod
     def _create_hook(sample: StochasticTensor, name: str, plates: List[Plate]):
         accum_grads = sample.param_grads
         del sample  # Remove from hook closure for GC reasons
+
         def hook(*args: Tuple[any]):
             # For some reason, this args unpacking is required for compatbility with registring on a .grad_fn...?
             # TODO: I'm sure there could be something wrong here
             grad = args[-1]
             if isinstance(grad, tuple):
                 grad = grad[0]
             try:
@@ -81,30 +83,33 @@
         # See also https://github.com/pytorch/pytorch/issues/12863
         def clean_graph() -> None:
             try:
                 nonlocal accum_grads
                 del accum_grads
             except (UnboundLocalError, NameError):
                 pass
+
         return hook, clean_graph
 
     def sample(self, distr: Distribution) -> storch.tensor.StochasticTensor:
         """
         Samples from the given distribution according to this Method's sampling scheme.
         :param distr:
         :return:
         """
-        # Unwrap the distributions parameters
-        params: Dict[str, storch.Tensor] = get_distr_parameters(
-            distr, filter_requires_grad=False
-        )
+
         parents: [torch.Tensor] = storch.wrappers._stochastic_parents.copy()
         # If we are in an @stochastic context, external plates might exist.
         plates: [Plate] = storch.wrappers._plate_links.copy()
         requires_grad = False
+
+        # Unwrap the distributions parameters
+        params: Dict[str, storch.Tensor] = get_distr_parameters(
+            distr, filter_requires_grad=False
+        )
         for name, p in params.items():
             requires_grad = requires_grad or p.requires_grad
             if isinstance(p, storch.Tensor):
                 parent_found = False
                 for _p in parents:
                     if _p is p:
                         parent_found = True
@@ -125,15 +130,15 @@
         s_tensor, plate = self.sampling_method(distr, parents, plates, requires_grad)
 
         s_tensor._set_method(self)
 
         batch_weighting = self.sampling_method.weighting_function(s_tensor, plate)
         if batch_weighting is not None:
             plate.weight = batch_weighting
-            # TODO: I don't think this code should be here.
+            # TODO: Is there a smarter way to handle this? Is it always properly added?
             # if isinstance(batch_weighting, storch.Tensor):
             #     batch_weighting.plates[0] = plate
 
         clean_hooks = []
         for name, param in params.items():
             # TODO: Possibly could find the wrong gradients here if multiple distributions use the same parameter?
             # This maybe requires copying the tensor hm...
@@ -178,31 +183,28 @@
                 [s_tensor],
                 s_tensor.plates,
                 s_tensor.name,
                 s_tensor.n,
                 s_tensor.distribution,
                 False,
             )
+            # TODO: why is _set_method not called on this new_s_tensor?
             new_s_tensor.param_grads = s_tensor.param_grads
             return new_s_tensor
         return s_tensor
 
     def _estimator(
         self, tensor: StochasticTensor, cost_node: CostTensor
-    ) -> Tuple[
-        Optional[storch.Tensor], Optional[storch.Tensor]
-    ]:
+    ) -> Tuple[Optional[storch.Tensor], Optional[storch.Tensor]]:
         self._estimation_pairs.append((tensor, cost_node))
         return self.estimator(tensor, cost_node)
 
     def estimator(
         self, tensor: StochasticTensor, cost_node: CostTensor
-    ) -> Tuple[
-        Optional[storch.Tensor], Optional[storch.Tensor]
-    ]:
+    ) -> Tuple[Optional[storch.Tensor], Optional[storch.Tensor]]:
         """
         Returns two terms that will be used for inferring higher-order gradient estimates.
         - The first return is the gradient function. It will be multiplied with the cost function.
           To get correct, unbiased estimates, the cost_node should not be involved in the computation.
           In REINFORCE-based methods, this is usually the score function.
           Methods that do not use a multiplicative estimator can return None.
         - The second return is the control variate, for instance a baseline in score-function based methods.
@@ -282,17 +284,15 @@
             )
         super().__init__(plate_name, _method.sampling_method)
         self._score_method = ScoreFunction(plate_name, sampling_method, n_samples)
         self._method = _method
 
     def estimator(
         self, tensor: StochasticTensor, cost_node: CostTensor
-    ) -> Tuple[
-        Optional[storch.Tensor],  Optional[storch.Tensor]
-    ]:
+    ) -> Tuple[Optional[storch.Tensor], Optional[storch.Tensor]]:
         return self._score_method.estimator(tensor, cost_node)
 
     def update_parameters(
         self, result_triples: [(StochasticTensor, CostTensor, torch.Tensor)]
     ):
         self._method.update_parameters(result_triples)
         self._score_method.update_parameters(result_triples)
@@ -319,15 +319,15 @@
         n_samples: int = 1,
     ):
         if not sampling_method:
             sampling_method = MonteCarlo(plate_name, n_samples)
         super().__init__(plate_name, sampling_method.set_mc_sample(self.reparam_sample))
 
     def is_pathwise(self, tensor: StochasticTensor, cost_node: CostTensor) -> bool:
-        if has_differentiable_path(cost_node, tensor):
+        if not storch.CHECK_DIFFERENTIABLE_PATH or has_differentiable_path(cost_node, tensor):
             # There is a differentiable path, so we will just use reparameterization here.
             return True
         raise ValueError(
             "There is no differentiable path between the cost tensor and the stochastic tensor. "
             "We cannot use reparameterization. Use a different gradient estimator, or make sure your"
             "code is differentiable."
         )
@@ -383,20 +383,20 @@
         amt_samples: int,
     ):
         return rsample_gumbel_softmax(
             distr, amt_samples, self.temperature, self.straight_through
         )
 
     def is_pathwise(self, tensor: StochasticTensor, cost_node: CostTensor) -> bool:
-        if has_differentiable_path(cost_node, tensor):
+        if not storch.CHECK_DIFFERENTIABLE_PATH or has_differentiable_path(cost_node, tensor):
             # There is a differentiable path, so we will just use reparameterization here.
             return True
         raise ValueError(
             "There is no differentiable path between the cost tensor and the stochastic tensor. "
-            "We cannot use reparameterization. Use a different gradient estimator, or make sure your"
+            "We cannot use reparameterization. Use a different gradient estimator, or make sure your "
             "code is differentiable."
         )
 
     def update_parameters(
         self, result_triples: [(StochasticTensor, CostTensor)]
     ) -> None:
         if self.temperature > self.min_temperature:
@@ -457,15 +457,15 @@
         gumbels = rsample_gumbel(distr, amt_samples)
         res = self.entmax(gumbels / self.temperature)
         return res
 
     def is_pathwise(
         self, tensor: storch.StochasticTensor, cost_node: storch.CostTensor
     ) -> bool:
-        if has_differentiable_path(cost_node, tensor):
+        if not storch.CHECK_DIFFERENTIABLE_PATH or has_differentiable_path(cost_node, tensor):
             # There is a differentiable path, so we will just use reparameterization here.
             return True
         raise ValueError(
             "There is no differentiable path between the cost tensor and the stochastic tensor. "
             "We cannot use reparameterization. Use a different gradient estimator, or make sure your"
             "code is differentiable."
         )
@@ -549,29 +549,32 @@
             elif baseline_factory == "none" or baseline_factory == "None":
                 self.baseline_factory = None
             else:
                 raise ValueError("Invalid baseline name", baseline_factory)
 
     def estimator(
         self, tensor: StochasticTensor, cost: CostTensor
-    ) -> Tuple[
-        Optional[storch.Tensor], Optional[storch.Tensor]
-    ]:
-        log_prob = tensor.distribution.log_prob(tensor)
+    ) -> Tuple[Optional[storch.Tensor], Optional[storch.Tensor]]:
+        log_prob: torch.Tensor = tensor.distribution.log_prob(tensor)
+
+        # tensor.distribution.logits.register_hook(lambda g: print("logits grad", g))
+        # print(cost)
+        # log_prob.register_hook(lambda g: print("grad", g))
         if len(log_prob.shape) > tensor.plate_dims:
             # Sum out over the event shape
             log_prob = log_prob.sum(
                 dim=list(range(tensor.plate_dims, len(log_prob.shape)))
             )
         if self.baseline_factory:
             baseline_name = "_b_" + tensor.name + "_" + cost.name
             if not hasattr(self, baseline_name):
                 setattr(self, baseline_name, self.baseline_factory(tensor, cost))
             baseline = getattr(self, baseline_name)
             baseline = baseline.compute_baseline(tensor, cost)
-            return log_prob, (1.0 - log_prob) * baseline
+            return log_prob, (1.0 - magic_box(log_prob)) * baseline
+
         return log_prob, None
 
 
 class Expect(Method):
     def __init__(self, plate_name: str, budget=10000):
         super().__init__(plate_name, Enumerate(plate_name, budget))
```

### Comparing `storchastic-0.3.5/storch/method/multi_sample_reinforce.py` & `storchastic-0.3.6/storch/method/multi_sample_reinforce.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-from typing import Optional
+from typing import Optional, Tuple
 
 import storch
 from storch.method.method import Method
 
 from storch.sampling import SampleWithoutReplacement
 
 
-class ScoreFunctionWOR(Method):
-    """
-    Implement Buy 4 REINFORCE Samples, Get a Baseline for Free! https://openreview.net/pdf?id=r1lgTGL5DE
-    Use biased=True for the biased normalized version which has lower variance.
-    """
-
-    def __init__(
-        self, plate_name: str, k: int, biased: bool = True, use_baseline: bool = True
-    ):
-        # Use k + 1 to be able to compute kappa, the k+1th perturbed log-prob
-        super().__init__(plate_name, SampleWithoutReplacement(plate_name, k, biased))
-        self.biased = biased
-        self.use_baseline = use_baseline
-
+class SeqMethod(Method):
     def is_pathwise(
         self, tensor: storch.StochasticTensor, cost_node: storch.CostTensor
     ) -> bool:
         # We only want to add a loss on the stochastic tensor with the same plate as the cost node.
         # This is because the estimator computes the gradient with the respect to the JOINT log probability.
         # If we would have added the gradient for all stochastic tensors, these would just be duplicates of the same
         # loss being added (ie that gradient would be oversampled)
@@ -37,35 +24,52 @@
                         # TODO: What exactly does this mean?
                         return True
                 raise ValueError(
                     "The given tensor contains an ancestral plate that the cost node doesn't have."
                 )
         return True
 
-    def multiplicative_estimator(
+
+class ScoreFunctionWOR(SeqMethod):
+    """
+    Implement Buy 4 REINFORCE Samples, Get a Baseline for Free! https://openreview.net/pdf?id=r1lgTGL5DE
+    Use biased=True for the biased normalized version which has lower variance.
+    """
+
+    def __init__(
+        self, plate_name: str, k: int, biased: bool = True, use_baseline: bool = True
+    ):
+        # Use k + 1 to be able to compute kappa, the k+1th perturbed log-prob
+        super().__init__(plate_name, SampleWithoutReplacement(plate_name, k, biased))
+        self.biased = biased
+        self.use_baseline = use_baseline
+
+    def estimator(
         self, tensor: storch.StochasticTensor, cost_node: storch.CostTensor
-    ) -> Optional[storch.Tensor]:
+    ) -> Tuple[Optional[storch.Tensor], Optional[storch.Tensor]]:
         cost_plate = None
         for _p in cost_node.plates:
             if _p.name == self.plate_name:
                 cost_plate = _p
                 break
         if self.use_baseline:
             iw = self.sampling_method.compute_iw(cost_plate, biased=False)
             BS = storch.sum(iw * cost_node, cost_plate)
             probs = cost_plate.log_probs.exp()
+            # TODO: These have not been derived in the proper storchastic form.
+            #  That is, the additive estimator is not a separate term, possibly introducing bias or variance.
             if self.biased:
                 # Equation 11
                 WS = storch.sum(iw, cost_plate)
                 WiS = (WS - iw + probs).detach()
                 diff_cost = cost_node - BS / WS
-                return storch.sum(iw / WiS * diff_cost.detach(), cost_plate)
+                return storch.sum(iw / WiS * diff_cost.detach(), cost_plate), None
             else:
                 # Equation 10
                 weighted_cost = cost_node * (1 - probs + iw)
                 diff_cost = weighted_cost - BS
-                return storch.sum(iw * diff_cost.detach(), cost_plate)
+                return storch.sum(iw * diff_cost.detach(), cost_plate), None
         else:
             # Equation 9
             # TODO: This seems inefficient... The plate should already contain the IW, right? Same for above if not self.biased
             iw = self.sampling_method.compute_iw(cost_plate, self.biased)
-            return storch.sum(cost_node.detach() * iw, self.plate_name)
+            return storch.sum(cost_node.detach() * iw, self.plate_name), None
```

### Comparing `storchastic-0.3.5/storch/method/relax.py` & `storchastic-0.3.6/storch/method/relax.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+
 from functools import reduce
 from operator import mul
 from typing import Optional, Callable, Tuple
 
 import torch
 from torch.distributions import Distribution, Bernoulli
 
@@ -340,14 +342,17 @@
         # Find grad of the distribution, then compute variance.
         # TODO: check if the set statement properly filters different results here
         tensors = list(set([result[0] for result in result_triples]))
         # minimize the variance of the gradient with respect to the input parameters
         for tensor in tensors:
             # TODO: We have to select the probs of the distribution here as that's what it flows to. Is this always correct?
             d_param = tensor.grad['probs']
+            if not d_param.requires_grad:
+                warnings.warn("Gradient of input tensor does not require grad which is needed to train the REBAR variance parameter.".format(tensor))
+                continue
             variance = (d_param ** 2).sum(d_param.event_dim_indices)
             var_loss = storch.reduce_plates(variance)
 
             d_variance = torch.autograd.grad(
                 [var_loss._tensor], self.control_params, retain_graph=True, allow_unused=True
             )
             for i in range(len(self.control_params)):
```

### Comparing `storchastic-0.3.5/storch/method/unordered.py` & `storchastic-0.3.6/storch/method/unordered.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional, Tuple
 
 import storch
-from storch.method.method import Method
+from storch.method.multi_sample_reinforce import SeqMethod
 from storch.sampling import UnorderedSet, GumbelSoftmaxWOR
 from storch.util import magic_box
 
 
-class UnorderedSetEstimator(Method):
+class UnorderedSetEstimator(SeqMethod):
     """
     Implements the Unordered Set REINFORCE Estimator with baseline from https://openreview.net/forum?id=rklEj2EFvB
     (Wouter Kool et al, ICLR 2020)
     It uses Stochastic Beam Search to sample from sequences of discrete random variables without replacement.
     Then it normalizes these samples, treating them as unordered samples without replacement, that is, as sets.
     The baseline takes a weighted average over the cost using these samples.
 
@@ -50,33 +50,14 @@
                 num_int_points,
                 a,
                 eos=eos,
             ),
         )
         self.use_baseline = use_baseline
 
-    def is_pathwise(
-        self, tensor: storch.StochasticTensor, cost_node: storch.CostTensor
-    ) -> bool:
-        # We only want to add a loss on the stochastic tensor with the same plate as the cost node.
-        # This is because the estimator computes the gradient with the respect to the JOINT log probability.
-        # If we would have added the gradient for all stochastic tensors, these would just be duplicates of the same
-        # loss being added (ie that gradient would be oversampled)
-        for distr_plate in tensor.plates:
-            if distr_plate.name == self.plate_name:
-                for cost_plate in cost_node.plates:
-                    if cost_plate.name == self.plate_name:
-                        if cost_plate is distr_plate:
-                            return False
-                        return True
-                raise ValueError(
-                    "The given tensor contains an ancestral plate that the cost node doesn't have."
-                )
-        return True
-
     def estimator(
         self, tensor: storch.StochasticTensor, cost_node: storch.CostTensor
     ) -> Tuple[
         Optional[storch.Tensor], Optional[storch.Tensor]
     ]:
         # Note: We automatically multiply with leave-one-out ratio in the plate reduction
         plate = None
@@ -95,15 +76,15 @@
         # Make sure the k dimension is recognized as batch dimension
         baseline = storch.Tensor(
             baseline._tensor, [baseline], baseline.plates + [plate]
         )
         return plate.log_probs, (1 - magic_box(plate.log_probs)) * baseline.detach()
 
 
-class UnorderedSetGumbelSoftmax(Method):
+class UnorderedSetGumbelSoftmax(SeqMethod):
     def __init__(
         self,
         plate_name: str,
         k: int,
         initial_temperature=1.0,
         min_temperature=1.0e-4,
         annealing_rate=1.0e-5,
```

### Comparing `storchastic-0.3.5/storch/nn/losses.py` & `storchastic-0.3.6/storch/nn/losses.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/storch/sampling/expect.py` & `storchastic-0.3.6/storch/sampling/expect.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/storch/sampling/method.py` & `storchastic-0.3.6/storch/sampling/method.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,17 +36,19 @@
     ) -> (storch.StochasticTensor, Plate):
         pass
 
     def weighting_function(
         self, tensor: storch.StochasticTensor, plate: Plate
     ) -> Optional[storch.Tensor]:
         """
-        Weight by the size of the sample. Overload this if your gradient estimation uses some kind of weighting
+        Weight by the size of the sample. Overload this if your sampling method uses some kind of weighting
         of the different events, like importance sampling or computing the expectation.
         If None is returned, it is assumed the samples are iid monte carlo samples.
+
+        This method is called from storch.method.Method.sample, and it is not needed to manually call this on created plates
         """
         return self.mc_weighting_function(tensor, plate)
 
     def mc_weighting_function(
         self, tensor: storch.StochasticTensor, plate: Plate
     ) -> Optional[storch.Tensor]:
         return None
@@ -60,15 +62,16 @@
     def mc_sample(
         self,
         distr: Distribution,
         parents: [storch.Tensor],
         plates: [Plate],
         amt_samples: int,
     ) -> torch.Tensor:
-        return distr.sample((self.n_samples,))
+        # TODO: Why does this ignore amt_samples?
+        return distr.sample((amt_samples,))
 
     def set_mc_sample(
         self,
         new_sample_func: Callable[
             [Distribution, [storch.Tensor], [Plate], int], torch.Tensor
         ],
     ) -> SamplingMethod:
```

### Comparing `storchastic-0.3.5/storch/sampling/seq.py` & `storchastic-0.3.6/storch/sampling/seq.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 import itertools
 from abc import abstractmethod
-from typing import Union, List, Optional, Tuple
+from typing import Union, List, Optional, Tuple, Callable, Iterable
+
+from storch import Plate
 
 from storch.typing import AnyTensor
 from storch.sampling.method import SamplingMethod
 from torch.distributions import Distribution
 import storch
 import torch
 
@@ -15,53 +17,62 @@
     def __init__(
         self,
         name: str,
         n: int,
         parents: List[storch.Plate],
         variable_index: int,
         parent_plate: AncestralPlate,
-        selected_samples: storch.Tensor,
-        log_probs: storch.Tensor,
+        selected_samples: Optional[storch.Tensor],
+        log_probs: Optional[storch.Tensor],
         weight: Optional[storch.Tensor] = None,
     ):
         super().__init__(name, n, parents, weight)
         assert (not parent_plate and variable_index == 0) or (
             parent_plate.n <= self.n and parent_plate.variable_index < variable_index
         )
         self.parent_plate = parent_plate
         self.selected_samples = selected_samples
-        self.log_probs = storch.Tensor(
-            log_probs._tensor, [log_probs], log_probs.plates + [self]
-        )
+        if isinstance(log_probs, storch.Tensor):
+            self.log_probs = storch.Tensor(
+                log_probs._tensor,
+                [log_probs],
+                log_probs.plates + [self]
+            )
         self.variable_index = variable_index
         self._in_recursion = False
         self._override_equality = False
 
     def __eq__(self, other):
-        if self._override_equality:
+        if not isinstance(other, AncestralPlate):
+            return False
+        if self._override_equality or other._override_equality:
             return other.name == self.name
         return (
             super().__eq__(other)
-            and isinstance(other, AncestralPlate)
             and self.variable_index == other.variable_index
         )
 
     def __repr__(self):
         return (
             "(Ancestral, " + self.variable_index.__repr__() + super().__repr__() + ")"
         )
 
     def on_collecting_args(self, plates: [storch.Plate]) -> bool:
         """
         Filter the collected plates to only keep the AncestralPlates (with the same name) that has the highest variable index.
         :param plates:
         :return:
         """
+        # TODO: It seems like in_recursion controls _override_equality. Does it have other uses? Can we remove it and just
+        #  use _override_equality?
+        # TODO: in the expand in on_unwrap_tensor, _override_equality needs to be true but isn't.
         if self._in_recursion:
             self._override_equality = True
+        if any(map(lambda plate: isinstance(plate, AncestralPlate) and plate._in_recursion, plates)) and not self._in_recursion:
+            return False
         return super().on_collecting_args(plates)
 
     def on_duplicate_plate(self, plate: storch.Plate) -> bool:
         if not isinstance(plate, AncestralPlate):
             raise ValueError(
                 "Received a plate with name "
                 + plate.name
@@ -70,68 +81,85 @@
         return plate.variable_index > self.variable_index
 
     def on_unwrap_tensor(self, tensor: storch.Tensor) -> storch.Tensor:
         """
         Gets called whenever the given tensor is being unwrapped and unsqueezed for batch use.
         This method should not be called on tensors whose variable index is higher than this plates.
 
+        selected_samples is used to choose from the parent plates what is the previous element in the sequence.
+        This is for example used in sampling without replacement.
+        If set to None, it is assumed the different sequences are indexed by the plate dimension.
+
         :param tensor: The input tensor that is being unwrapped
         :return: The tensor that will be unwrapped and unsqueezed in the future. Can be a modification of the input tensor.
         """
         if self._in_recursion:
             # Required when calling storch.gather in this method. It will call on_unwrap_tensor again.
             return tensor
-        for i, plate in enumerate(tensor.multi_dim_plates()):
+        # Find the corresponding ancestral plate
+        for i, plate in enumerate(tensor.plates):
             if plate.name != self.name:
                 continue
             assert isinstance(plate, AncestralPlate)
             if plate.variable_index == self.variable_index:
                 return tensor
             # This is true by the filtering at on_collecting_args
             assert plate.variable_index < self.variable_index
 
-            parent_plates = []
+            if self.selected_samples is None:
+                # If this sequence method does not explicitly select from previous samples, just return it with the current plate
+                new_plates = tensor.plates.copy()
+                new_plates[i] = self
+                return storch.Tensor(tensor._tensor, [tensor], new_plates)
+
+            downstream_plates = []
             current_plate = self
 
             # Collect the list of plates from the tensors variable index to this plates variable index
             while current_plate.variable_index != plate.variable_index:
-                parent_plates.append(current_plate)
+                downstream_plates.append(current_plate)
                 current_plate = current_plate.parent_plate
             assert current_plate == plate
 
             # Go over all parent plates and gather their respective choices.
-            for parent_plate in reversed(parent_plates):
+            for parent_plate in reversed(downstream_plates):
                 self._in_recursion = True
                 expanded_selected_samples = expand_with_ignore_as(
                     parent_plate.selected_samples, tensor, self.name
                 )
                 self._override_equality = False
                 # Gather what samples of the tensor are chosen by this plate (parent_plate)
                 tensor = storch.gather(
                     tensor, parent_plate.name, expanded_selected_samples
                 )
                 self._in_recursion = False
                 self._override_equality = False
             break
         return tensor
 
+    def index_in(self, plates: List[Plate]) -> int:
+        return list(map(lambda p: p.name, plates)).index(self.name)
+
+    def is_in(self, plates: Iterable[Plate]) -> bool:
+        return any(map(lambda p: p.name == self.name, plates))
 
 class SequenceDecoding(SamplingMethod):
     """
     Methods for generating sequences of discrete random variables.
     Examples: Simple ancestral sampling with replacement, beam search, Stochastic beam search (sampling without replacement)
     """
 
     EPS = 1e-8
 
     def __init__(self, plate_name: str, k: int, eos: None):
         super().__init__(plate_name)
         self.k = k
         self.eos = eos
         self.reset()
+        self.plate_first = True
 
     def reset(self):
         super().reset()
         # Cumulative log probabilities of the samples
         self.joint_log_probs = None
         # Chosen parent samples at the previous sample step
         self.parent_indexing = None
@@ -154,104 +182,93 @@
 
         """
         Sample from the distribution given the sequence so far.
         :param distribution: The distribution to sample from
         :return:
         """
 
-        # This code has three parts.
-        # The first prepares all necessary tensors to make sure they can be easily indexed.
-        # This part is quite long as there are many cases.
-        # 1) There have not been any variables sampled so far.
-        # 2) There have been variables sampled, but their results are NOT used to compute the input distribution.
-        #    in other words, the variable to sample is independent of the other sampled variables. However,
-        #    we should still keep track of the other sampled variables to make sure that it still samples without
-        #    replacement properly. In this case, the ancestral plate is not in the plates attribute.
-        #    We also have to make sure that we know in the future what samples are chosen for the _other_ samples.
-        # 3) There have been parents sampled, and this variable is dependent on at least some of them.
-        #    The plates list then contains the ancestral plate. We need to make sure we compute the joint log probs
-        #    for the conditional samples (ie, based on the different sampled variables in the ancestral dimension).
-        # The second part is a loop over all options for the event dimensions. This samples these conditionally
-        # independent samples in sequence. It samples indexes, not events.
-        # The third part after the loop uses the sampled indexes and matches it to the events to be used.
-
-        # LEGEND FOR SHAPE COMMENTS
-        # =========================
-        # To make this code generalize to every bayesian network, complicated shape management is necessary.
-        # The following are references to the shapes that are used within the method
-        #
-        # distr_plates: refers to the plates on the parameters of the distribution. Does *not* include
-        #  the k? ancestral plate (possibly empty)
-        # orig_distr_plates: refers to the plates on the parameters of the distribution, and *can* include
-        #  the k? ancestral plate (possibly empty)
-        # prev_plates: refers to the plates of the previous sampled variable in this swr sample (possibly empty)
-        # plates: refers to all plates except this ancestral plate, of which there are amt_plates. The first plates are
-        #  the distr_plates, after that the prev_plates that are _not_ in distr_plates.
-        #  It is composed of distr_plate x (ancstr_plates - distr_plates)
-        # events: refers to the conditionally independent dimensions of the distribution (the distributions batch shape minus the plates)
-        # k: refers to self.k
-        # k?: refers to an optional plate dimension of this ancestral plate. It either doesn't exist, or is the sample
-        #  dimension. If it exists, this means this sample is conditionally dependent on ancestors.
-        # |D_yv|: refers to the *size* of the domain
-        # amt_samples: refers to the current amount of sampled sequences. amt_samples <= k, but it can be lower if there
-        #  are not enough events to sample from (eg |D_yv| < k)
-        # event_shape: refers to the *shape* of the domain elements
-        #  (can be 0, eg Categorical, or equal to |D_yv| for OneHotCategorical)
-
         # Do the decoding step given the prepared tensors
-        samples, self.joint_log_probs, self.parent_indexing = self.decode(
+        samples, new_joint_log_probs, self.parent_indexing = self.decode(
             distr, self.joint_log_probs, parents, orig_distr_plates
         )
+        if new_joint_log_probs is not None:
+            self.joint_log_probs = new_joint_log_probs
+        else:
+            # We'll assign it later
+            self.joint_log_probs = None
 
         # Find out what sequences have reached the EOS token, and make sure to always sample EOS after that.
         # Does not contain the ancestral plate as this uses samples instead of s_tensor.
         if self.eos:
             self.finished_samples = samples.eq(self.eos)
 
-        k_index = 0
-        plates = orig_distr_plates
         if isinstance(samples, storch.Tensor):
             k_index = samples.plate_dims
             plates = samples.plates
             samples = samples._tensor
+        else:
+            plate_names = list(map(lambda p: p.name, orig_distr_plates))
+            k_index = plate_names.index(self.plate_name) if self.plate_name in plate_names else 0
+            plates = orig_distr_plates
+
 
         plate_size = samples.shape[k_index]
 
         # Remove the ancestral plate, if it already happens to be in
         to_remove = None
         for plate in plates:
             if plate.name == self.plate_name:
                 to_remove = plate
                 break
         if to_remove:
             plates.remove(to_remove)
 
         # Create the newly updated plate
         self.new_plate = self.create_plate(plate_size, plates.copy())
-        plates.append(self.new_plate)
+        # TODO: This can probably be simplified by assuming plate_first
+        plates.insert(k_index, self.new_plate)
 
         if self.parent_indexing is not None:
-            self.parent_indexing.plates.append(self.new_plate)
+            assert isinstance(self.parent_indexing, storch.Tensor)
+            # TODO: This too
+            self.parent_indexing.plates.insert(k_index, self.new_plate)
 
+        # Adjust the sequence based on parent samples chosen
         self.seq = list(map(lambda t: self.new_plate.on_unwrap_tensor(t), self.seq))
 
         # Construct the stochastic tensor
         s_tensor = storch.StochasticTensor(
             samples,
             parents,
             plates,
             self.plate_name,
             plate_size,
             distr,
-            requires_grad or self.joint_log_probs.requires_grad,
+            requires_grad or self.joint_log_probs is not None and self.joint_log_probs.requires_grad,
         )
 
+        # Update joint log probs if decoding method did not compute it
+        if new_joint_log_probs is None:
+            s_log_probs = distr.log_prob(s_tensor)
+            if self.joint_log_probs is not None:
+                self.joint_log_probs += s_log_probs
+            else:
+                self.joint_log_probs = s_log_probs
+
+            if self.finished_samples:
+                # Make sure we do not change the log probabilities for samples that were already finished
+                self.joint_log_probs = (
+                        self.joint_log_probs * self.finished_samples
+                        + self.joint_log_probs * (1 - self.finished_samples)
+                )
+            self.new_plate.log_probs = self.joint_log_probs
+            s_tensor._requires_grad = s_tensor.requires_grad or self.joint_log_probs.requires_grad
         self.seq.append(s_tensor)
 
-        # Increase variable index
+        # Increase variable index for next samples in sequence
         self.variable_index += 1
         return s_tensor, self.new_plate
 
     def weighting_function(
         self, tensor: storch.StochasticTensor, plate: storch.Plate
     ) -> Optional[storch.Tensor]:
         if self.eos:
@@ -318,69 +335,107 @@
         # This is required because storch.Tensor's do not support .all() and .bool()
         if isinstance(t, storch.Tensor):
             return t._tensor.all().bool()
         return t.all().bool()
 
 
 class MCDecoder(SequenceDecoding):
+
     def decode(
         self,
         distribution: Distribution,
         joint_log_probs: Optional[storch.Tensor],
         parents: [storch.Tensor],
         orig_distr_plates: [storch.Plate],
     ) -> (storch.Tensor, storch.Tensor, storch.Tensor):
 
         is_conditional_sample = False
 
         for plate in orig_distr_plates:
             if plate.name == self.plate_name:
                 is_conditional_sample = True
 
-        if is_conditional_sample:
-            sample = self.mc_sample(
-                distribution, parents, orig_distr_plates, 1
-            ).squeeze(0)
-        else:
-            sample = self.mc_sample(distribution, parents, orig_distr_plates, self.k)
-
-        s_log_probs = distribution.log_prob(sample)
-        if joint_log_probs:
-            joint_log_probs += s_log_probs
-        else:
-            joint_log_probs = s_log_probs
+        with storch.ignore_wrapping():
+            if is_conditional_sample:
+                sample = self.mc_sample(
+                    distribution, parents, orig_distr_plates, 1
+                ).squeeze(0)
+            else:
+                sample = self.mc_sample(distribution, parents, orig_distr_plates, self.k)
 
         if self.finished_samples:
-            # Make sure we do not change the log probabilities for samples that were already finished
-            joint_log_probs = (
-                joint_log_probs * self.finished_samples
-                + joint_log_probs * (1 - self.finished_samples)
-            )
             sample[self.finished_samples] = self.eos
 
-        return sample, joint_log_probs, None
+        return sample, None, None
+
+
+
 
 
 class IterDecoding(SequenceDecoding):
+
+    def __init__(self, plate_name, k, eos):
+        super().__init__(plate_name, k, eos)
+        self.plate_first = False
+
+    # Decodes a multivariable discrete distribution (independent over dimensions)
     def decode(
         self,
         distr: Distribution,
         joint_log_probs: Optional[storch.Tensor],
         parents: [storch.Tensor],
         orig_distr_plates: [storch.Plate],
     ) -> (storch.Tensor, storch.Tensor, storch.Tensor):
         """
         Decode given the input arguments
         :param distribution: The distribution to decode
         :param joint_log_probs: The log probabilities of the samples so far. prev_plates x amt_samples
         :param parents: List of parents of this tensor
         :param orig_distr_plates: List of plates from the distribution. Can include the self plate k.
         :return: 3-tuple of `storch.Tensor`. 1: The sampled value. 2: The new joint log probabilities of the samples.
-        3: How the samples index the parent samples. Can just be a range if there is no choosing happening.
+        3: How the samples index the parent samples. Can just be None if there is no choosing happening.
         """
+        # This code has three parts.
+        # The first prepares all necessary tensors to make sure they can be easily indexed.
+        # This part is quite long as there are many cases.
+        # 1) There have not been any variables sampled so far.
+        # 2) There have been variables sampled, but their results are NOT used to compute the input distribution.
+        #    in other words, the variable to sample is independent of the other sampled variables. However,
+        #    we should still keep track of the other sampled variables to make sure that it still samples without
+        #    replacement properly. In this case, the ancestral plate is not in the plates attribute.
+        #    We also have to make sure that we know in the future what samples are chosen for the _other_ samples.
+        # 3) There have been parents sampled, and this variable is dependent on at least some of them.
+        #    The plates list then contains the ancestral plate. We need to make sure we compute the joint log probs
+        #    for the conditional samples (ie, based on the different sampled variables in the ancestral dimension).
+        # The second part is a loop over all options for the event dimensions. This samples these conditionally
+        # independent samples in sequence. It samples indexes, not events.
+        # The third part after the loop uses the sampled indexes and matches it to the events to be used.
+
+        # LEGEND FOR SHAPE COMMENTS
+        # =========================
+        # To make this code generalize to every bayesian network, complicated shape management is necessary.
+        # The following are references to the shapes that are used within the method
+        #
+        # distr_plates: refers to the plates on the parameters of the distribution. Does *not* include
+        #  the k? ancestral plate (possibly empty)
+        # orig_distr_plates: refers to the plates on the parameters of the distribution, and *can* include
+        #  the k? ancestral plate (possibly empty)
+        # prev_plates: refers to the plates of the previous sampled variable in this swr sample (possibly empty)
+        # plates: refers to all plates except this ancestral plate, of which there are amt_plates. The first plates are
+        #  the distr_plates, after that the prev_plates that are _not_ in distr_plates.
+        #  It is composed of distr_plate x (ancstr_plates - distr_plates)
+        # events: refers to the conditionally independent dimensions of the distribution (the distributions batch shape minus the plates)
+        # k: refers to self.k
+        # k?: refers to an optional plate dimension of this ancestral plate. It either doesn't exist, or is the sample
+        #  dimension. If it exists, this means this sample is conditionally dependent on ancestors.
+        # |D_yv|: refers to the *size* of the domain
+        # amt_samples: refers to the current amount of sampled sequences. amt_samples <= k, but it can be lower if there
+        #  are not enough events to sample from (eg |D_yv| < k)
+        # event_shape: refers to the *shape* of the domain elements
+        #  (can be 0, eg Categorical, or equal to |D_yv| for OneHotCategorical)
         ancestral_distrplate_index = -1
         is_conditional_sample = False
 
         multi_dim_distr_plates = []
         multi_dim_index = 0
         for plate in orig_distr_plates:
             if plate.n > 1:
@@ -545,15 +600,15 @@
                 amt_multi_dim_plates,
                 amt_samples,
             )
         # Finally, index the support using the sampled indices to get the sample!
         if amt_samples < self.k:
             # plates x amt_samples x events
             sampled_support_indices = sampled_support_indices[
-                (...,) + (slice(amt_samples),) + (slice(None),) * len(ranges)
+                (...,) + (slice(amt_samples),)
             ]
         expanded_indices = right_expand_as(sampled_support_indices, support)
         sample = support.gather(dim=amt_multi_dim_plates, index=expanded_indices)
         return sample, joint_log_probs, parent_indexing
 
     @abstractmethod
     def decode_step(
```

### Comparing `storchastic-0.3.5/storch/sampling/swor.py` & `storchastic-0.3.6/storch/sampling/swor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from __future__ import annotations
-from typing import Optional, Union, List, Callable, Tuple
+from typing import Optional, Callable, Tuple
 
 import storch
 import torch
 from torch.distributions import Distribution, Gumbel
-import itertools
 from storch.sampling.method import SamplingMethod
 from storch.sampling.seq import IterDecoding, AncestralPlate, right_expand_as
 
 
 class SampleWithoutReplacement(IterDecoding):
     """
     Sampling method for sampling without replacement from (sequences of) discrete distributions.
     Implements Stochastic Beam Search https://arxiv.org/abs/1903.06059 with the weighting as defined by
     REINFORCE without replacement https://openreview.net/forum?id=r1lgTGL5DE
     """
 
     EPS = 1e-8
+    perturbed_log_probs: Optional[storch.Tensor] = None
 
     def __init__(self, plate_name: str, k: int, biased_iw: bool = False, eos=None):
         super().__init__(plate_name, k, eos)
         if k < 2:
             raise ValueError(
                 "Can only sample with replacement for more than 1 samples."
             )
         self.biased_iw = biased_iw
 
     def reset(self):
         super().reset()
         # Cumulative perturbed log probabilities of the samples
-        self.perturbed_log_probs: Optional[storch.Tensor] = None
+        self.perturbed_log_probs = None
 
     def decode_step(
         self,
         indices: Tuple[int],
         yv_log_probs: storch.Tensor,
         joint_log_probs: Optional[storch.Tensor],
         sampled_support_indices: Optional[storch.Tensor],
@@ -106,30 +106,32 @@
             # Then make sure the log probability of the eos token is equal to the last perturbed log prob.
             finished_vec[:, self.eos] = finished_perturb_log_probs
             cond_G_yv[self.finished_samples] = finished_vec
 
         if not first_sample:
             # plates x (k * |D_yv|) (k == prev_amt_samples, in this case)
             cond_G_yv = cond_G_yv.reshape(cond_G_yv.shape[:-2] + (-1,))
+            # Reshape log probs to plates x (k * |D_yv|). Matches perturbed shape.
+            all_joint_log_probs = all_joint_log_probs.reshape(cond_G_yv.shape)
 
         # Select the samples given the perturbed log probabilities
-        self.perturbed_log_probs, arg_top = self.select_samples(
+        self.perturbed_log_probs, joint_log_probs, arg_top = self.select_samples(
             cond_G_yv, all_joint_log_probs
         )
+        # Gather corresponding joint log probabilities.
+
         amt_samples = arg_top.shape[-1]
 
         if first_sample:
             # plates x amt_samples
-            joint_log_probs = all_joint_log_probs.gather(dim=-1, index=arg_top)
             # Index for the selected samples. Uses slice(amt_samples) for the first index in case k > |D_yv|
             # (:) * amt_plates + (indices for events) + amt_samples
             indexing = (slice(None),) * amt_plates + (slice(0, amt_samples),) + indices
             sampled_support_indices[indexing] = arg_top
         else:
-            # Gather corresponding joint log probabilities. First reshape like previous to plates x (k * |D_yv|).
             joint_log_probs = all_joint_log_probs.reshape(cond_G_yv.shape).gather(
                 dim=-1, index=arg_top
             )
 
             # |D_yv|
             size_domain = yv_log_probs.shape[-1]
 
@@ -147,60 +149,63 @@
             chosen_samples = arg_top.remainder(size_domain)
             indexing = (slice(None),) * amt_plates + (slice(0, amt_samples),) + indices
             sampled_support_indices[indexing] = chosen_samples
         return sampled_support_indices, joint_log_probs, parent_indexing, amt_samples
 
     def select_samples(
         self, perturbed_log_probs: storch.Tensor, joint_log_probs: storch.Tensor,
-    ) -> (storch.Tensor, storch.Tensor):
+    ) -> (storch.Tensor, storch.Tensor, storch.Tensor):
         """
         Given the perturbed log probabilities and the joint log probabilities of the new options, select which one to
         use for the sample.
         :param perturbed_log_probs: plates x (k? * |D_yv|). Perturbed log-probabilities. k is present if first_sample.
-        :param joint_log_probs: plates x k? x (k? * |D_yv|). Joint log probabilities of the options. k is present if first_sample.
+        :param joint_log_probs: plates x (k? * |D_yv|). Joint log probabilities of the options. k is present if first_sample.
         :param first_sample:
-        :return:
+        :return: perturbed log probs of chosen samples, joint log probs of chosen samples, index of chosen samples
         """
 
         # We can sample at most the amount of what we previous sampled, combined with every option in the current domain
         # That is: prev_amt_samples * |D_yv|.
         amt_samples = min(self.k, perturbed_log_probs.shape[-1])
         # Take the top k over conditional perturbed log probs
         # plates x amt_samples
-        return torch.topk(perturbed_log_probs, amt_samples, dim=-1)
+        perturbed_log_probs, arg_top = torch.topk(perturbed_log_probs, amt_samples, dim=-1)
+        joint_log_probs = joint_log_probs.gather(dim=-1, index=arg_top)
+        return perturbed_log_probs, joint_log_probs, arg_top
+
 
     def create_plate(self, plate_size: int, plates: [storch.Plate]) -> AncestralPlate:
         plate = super().create_plate(plate_size, plates)
         plate.perturb_log_probs = storch.Tensor(
             self.perturbed_log_probs._tensor,
             [self.perturbed_log_probs],
             self.perturbed_log_probs.plates + [plate],
         )
         return plate
 
     def weighting_function(
         self, tensor: storch.StochasticTensor, plate: storch.Plate
     ) -> Optional[storch.Tensor]:
+        # TODO: Doesnt take into account eos tokens
+        # TODO: Does this add the plate to the weighting function result? Could be a big bug!
         return self.compute_iw(plate, self.biased_iw).detach()
 
     def compute_iw(self, plate: AncestralPlate, biased: bool):
+        k = plate.perturb_log_probs.shape[-1]
         # Compute importance weights. The kth sample has 0 weight, and is only used to compute the importance weights
-        q = (
-            1
-            - (
-                -(
-                    plate.log_probs
-                    - plate.perturb_log_probs._tensor[..., self.k - 1].unsqueeze(-1)
-                ).exp()
-            ).exp()
-        ).detach()
+        # Equation 5
+        q = (1 - torch.exp(
+            - torch.exp(
+                plate.log_probs - plate.perturb_log_probs._tensor[..., k - 1].unsqueeze(-1)
+                ))).detach()
         iw = plate.log_probs.exp() / (q + self.EPS)
         # Set the weight of the kth sample (kappa) to 0.
-        iw[..., self.k - 1] = 0.0
+        iw[..., k - 1] = 0.0
         if biased:
+            # Equation 6 (normalization of importance weights)
             WS = storch.sum(iw, plate).detach()
             return iw / WS
         return iw
 
     def on_plate_already_present(self, plate: storch.Plate):
         if (
             not isinstance(plate, AncestralPlate)
@@ -221,15 +226,18 @@
 
 
 def log1mexp(a: torch.Tensor) -> torch.Tensor:
     """See appendix A of http://jmlr.org/papers/v21/19-985.html.
     Numerically stable implementation of log(1-exp(a))"""
     c = -0.693
     a1 = -a.abs()
-    return torch.where(a1 > c, torch.log(-a1.expm1()), torch.log1p(-a1.exp()))
+    eps = 1e-6
+    # exp_a = -a1.exp()
+    # assert (exp_a >= -1).all()
+    return torch.where(a1 > c, torch.log(-a1.expm1() + eps), torch.log1p(-a1.exp() + eps))
 
 
 @storch.deterministic
 def cond_gumbel_sample(all_joint_log_probs, perturbed_log_probs) -> torch.Tensor:
     # Sample plates x k? x |D_yv| Gumbel variables
     gumbel_d = Gumbel(loc=all_joint_log_probs, scale=1.0)
     G_yv = gumbel_d.rsample()
```

### Comparing `storchastic-0.3.5/storch/sampling/unordered_set.py` & `storchastic-0.3.6/storch/sampling/unordered_set.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ) -> Optional[storch.Tensor]:
         # plates_w_k is a sequence of plates of which one is the input ancestral plate
 
         # Computes p(s) * R(S^k, s), or the probability of the sample times the leave-one-out ratio.
         # For details, see https://openreview.net/pdf?id=rklEj2EFvB
         # Code based on https://github.com/wouterkool/estimating-gradients-without-replacement/blob/master/bernoulli/gumbel.py
         log_probs = plate.log_probs.detach()
-        # print("--------------------")
 
         # Compute integration points for the trapezoid rule: v should range from 0 to 1, where both v=0 and v=1 give a value of 0.
         # As the computation happens in log-space, take the logarithm of the result.
         # N
         v = (
             torch.arange(1, self.num_int_points, out=log_probs._tensor.new())
             / self.num_int_points
@@ -59,15 +58,14 @@
         # If g_bound >= 10, use the series expansion for stability with error O((e^-10)^6) (=8.7E-27)
         # See https://www.wolframalpha.com/input/?i=log%281+-+exp%28-y%29%29
         y = torch.exp(g_bound)
         # plates_w_k x N
         terms = torch.where(
             g_bound >= 10, -g_bound - y / 2 + y ** 2 / 24 - y ** 4 / 2880, log1mexp(y)
         )
-        # print("terms", terms._tensor[0])
 
         # Compute integrands (without subtracting the special value s)
         # plates x N
         sum_of_terms = storch.sum(terms, plate)
         phi_S = storch.logsumexp(log_probs, plate)
         phi_D_min_S = log1mexp(phi_S)
 
@@ -104,18 +102,14 @@
                 - terms[..., None, :] * skip_diag[..., None]
             )
             # plates_w_k x k
             log_p_S_without_ss = integrand_without_ss.logsumexp(dim=-1)
 
             plate.log_snd_leave_one_out = log_p_S_without_ss - log_p_S_without_s
 
-        # print("lloo", log_leave_one_out._tensor[0])
-        # print("log_probs", log_probs._tensor[0])
-        # print("weighting", (log_leave_one_out + log_probs).exp()._tensor[0])
-
         # Return the unordered set estimator weighting
         return (log_leave_one_out + log_probs).exp().detach()
 
 
 class GumbelSoftmaxWOR(UnorderedSet):
     def __init__(
         self,
@@ -141,15 +135,15 @@
         )
         from storch import conditional_gumbel_rsample
 
         gumbel_wor = conditional_gumbel_rsample(hard_sample, distr.probs,
                                                 isinstance(distr, torch.distributions.Bernoulli), self.temperature)
         gumbel_wor = storch.StochasticTensor(
             gumbel_wor._tensor,
-            list(zip(*hard_sample._parents))[0],
+            hard_sample.parents,
             hard_sample.plates,
             hard_sample.name,
             self.k,
             distr,
             requires_grad,
         )
         return gumbel_wor, plate
```

### Comparing `storchastic-0.3.5/storch/storch.py` & `storchastic-0.3.6/storch/storch.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,29 @@
                 index = index.name
             conv_indices.append(tensor.get_plate_dim_index(index))
             red_batches.append(index)
     return tuple(conv_indices), red_batches
 
 
 def mean(tensor: storch.Tensor, dims: _indices) -> storch.Tensor:
+    """
+    Simply takes the mean of the tensor over the dimensions given.
+    WARNING: This does NOT weight the different elements according to the plates. You will very likely want to
+    call the reduce_plates method instead.
+    """
     indices, reduced_batches = _convert_indices(tensor, dims)
     return storch.reduce(torch.mean, plates=reduced_batches)(tensor, indices)
 
 
 def sum(tensor: storch.Tensor, dims: _indices) -> storch.Tensor:
+    """
+    Simply sums the tensor over the dimensions given.
+    WARNING: This does NOT weight the different elements according to the plates. You will very likely want to
+    call the reduce_plates method instead.
+    """
     indices, reduced_batches = _convert_indices(tensor, dims)
     return storch.reduce(torch.sum, plates=reduced_batches)(tensor, indices)
 
 
 def logsumexp(tensor: storch.Tensor, dims: _indices) -> storch.Tensor:
     indices, reduced_batches = _convert_indices(tensor, dims)
     return storch.reduce(torch.logsumexp, plates=reduced_batches)(tensor, indices)
```

### Comparing `storchastic-0.3.5/storch/tensor.py` & `storchastic-0.3.6/storch/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
+
+from queue import Queue
+
 import torch
 import storch
 from torch.distributions import Distribution
 from collections import deque
-from typing import List, Iterable, Any, Callable, Iterator, Dict
+from typing import List, Iterable, Any, Callable, Iterator, Dict, Tuple, Deque
 import builtins
 from itertools import product
 from typing import Optional
 from storch.exceptions import IllegalStorchExposeError
 from storch.excluded_init import (
     exception_methods,
     excluded_methods,
@@ -126,14 +129,20 @@
 
         Returns:
             storch.Tensor: The tensor that will be unwrapped and unsqueezed in the future. Can be a modification of the input tensor.
 
         """
         return tensor
 
+    def index_in(self, plates: List[Plate]) -> int:
+        return plates.index(self)
+
+    def is_in(self, plates: Iterable[Plate]) -> bool:
+        return self in plates
+
 
 class Tensor:
     """
     A :class:`storch.Tensor` is a wrapper around a :class:`torch.Tensor` that acts like a normal :class:`torch.Tensor`
     with some restrictions and some extra data.
 
     By design, :class:`storch.Tensor` cannot expose the wrapped :class:`torch.Tensor` to regular Python control flow.
@@ -210,30 +219,33 @@
                     + " Tensor shape: "
                     + str(tensor.shape)
                 )
             batch_dims += 1
 
         self._name = name
         self._tensor = tensor
-        self._parents = []
+        self._parents: List[Tuple[Tensor, bool]] = []
         self._cleaned = False
-        differentiable_links = has_backwards_path(self, parents)
+        # DISCONTINUED FOR NOW BECAUSE OF PERFORMANCE OVERHEAD
+        # differentiable_links = has_backwards_path(self, parents)
         for i, p in enumerate(parents):
             # TODO: Should I re-add this?
             # if p.is_cost:
             #     raise ValueError("Cost nodes cannot have children.")
-            self._parents.append((p, differentiable_links[i]))
-            p._children.append((self, differentiable_links[i]))
+            # TODO: DIFFERENTIABLE LINKS MANUALLY SET TO FALSE. THIS MIGHT CAUSE BUGS IN THE FUTURE
+            self._parents.append((p, False))
+            p._children.append((self, False))
         self._children = []
         self.plate_dims = batch_dims
         self.event_shape = tensor.shape[batch_dims:]
         self.event_dims = len(self.event_shape)
         self.plates = plates
 
-    def __torch_function__(self, func, types, args=(), kwargs=None):
+    @classmethod
+    def __torch_function__(cls, func: Callable, types, args=(), kwargs=None) -> Callable:
         """
         Called whenever a torch.* or torch.nn.functional.* method is being called on a storch.Tensor. This wraps
         that method in the deterministic wrapper to properly handle all input arguments and outputs.
         """
         if kwargs is None:
             kwargs = {}
         func_name = func.__name__
@@ -251,24 +263,24 @@
                 func, args, kwargs, expand_plates=True
             )
         # if func_name in unwrap_only_methods:
         #     return storch.wrappers._unpack_wrapper(func)(*args, *kwargs)
 
         return storch.wrappers._handle_deterministic(func, args, kwargs)
 
-    def __getattr__(self, item):
+    def __getattr__(self, item) -> Any:
         """
         Called whenever an attribute is called on a storch.Tensor object that is not directly implemented by storch.Tensor.
         It defers it to the underlying torch.Tensor. If it is a callable (ie, torch.Tensor implements a function
         with the name item), it will wrap this callable with a deterministic wrapper.
 
         TODO: This should probably filter the methods
         """
         attr = getattr(torch.Tensor, item)
-        if isinstance(attr, Callable):
+        if callable(attr):
             func_name = attr.__name__
             if func_name in exception_methods:
                 raise IllegalStorchExposeError(
                     "Calling method "
                     + func_name
                     + " with storch tensors is not allowed."
                 )
@@ -293,80 +305,81 @@
         t = (
             (self.name + ": " if self.name else "") + "Stochastic"
             if self.stochastic
             else ("Cost" if self.is_cost else "Deterministic")
         )
         return t + " " + str(self._tensor) + " Batch links: " + str(self.plates)
 
-    def __repr__(self):
-        return self._tensor.__repr__()
+    def __repr__(self) -> str:
+        return f"[{repr(self.name)}, {repr(self._tensor)}, {repr(self.plates)}"
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return object.__hash__(self)
 
     @storch.deterministic
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         return self.__eq__(other)
 
     @storch.deterministic(l_broadcast=False)
     def __getitem__(self, index):
         return self.__getitem__(index)
 
     @storch.deterministic(l_broadcast=False)
     def __setitem__(self, index, value):
         return self.__setitem__(index, value)
 
     def _walk_backwards(
         self,
-        expand_fn,
+        expand_fn: Callable[[Tensor], Iterator[Tuple[Tensor, bool]]],
         depth_first=True,
         reverse=False, # Only supported for breadth-first
         only_differentiable=False,
         repeat_visited=False,
         walk_fn=lambda x: x,
-    ) -> Iterator:
+    ) -> Iterator[Tensor]:
         visited = set()
         visited_ordered = []
         if depth_first:
             S = [self]
             while S:
                 v = S.pop()
-                if repeat_visited or v not in visited:
+                if repeat_visited or not v.is_in(visited):
                     yield walk_fn(v)
                     visited.add(v)
                     for w, d in expand_fn(v):
                         if d or not only_differentiable:
                             S.append(w)
         else:
-            queue = deque()
+            queue: Deque[Tensor] = deque()
             visited.add(self)
             queue.append(self)
             while queue:
                 v = queue.popleft()
                 if reverse:
                     visited_ordered.append(v)
                 else:
                     yield walk_fn(v)
                 for w, d in expand_fn(v):
-                    if (repeat_visited or w not in visited) and (
+                    if (repeat_visited or not w.is_in(visited)) and (
                         d or not only_differentiable
                     ):
                         visited.add(w)
                         queue.append(w)
             if reverse:
-                return reversed(visited_ordered)
+                for v in reversed(visited_ordered):
+                    yield v
 
     def walk_parents(
         self,
         depth_first=True,
         reverse=False,
         only_differentiable=False,
         repeat_visited=False,
         walk_fn=lambda x: x,
-    ):
+    ) -> Iterator[Tensor]:
         """
         Searches through the parents of this Tensor in the stochastic computation graph.
 
         Args:
             depth_first: True to use depth first, otherwise breadth first.
             reverse: Reverse the order: If true, instead of first returning the immediate parents, return
                 the parents furthest up, working towards the immediate parents.
@@ -377,26 +390,28 @@
 
         Returns:
             Iterator of type that is equal to the output type of ``walk_fn``.
         """
         return self._walk_backwards(
             lambda p: p._parents,
             depth_first,
+            reverse,
             only_differentiable,
             repeat_visited,
             walk_fn,
         )
 
-    def walk_children(
+    def walk_children (
         self,
         depth_first=True,
+        reverse=False,
         only_differentiable=False,
         repeat_visited=False,
         walk_fn=lambda x: x,
-    ):
+    ) -> Iterator[Tensor]:
         """
         Searches through the children of this Tensor in the stochastic computation graph.
 
         Args:
             depth_first: True to use depth first, otherwise breadth first.
             only_differentiable: True to only walk over edges that are differentiable
             repeat_visited:
@@ -404,20 +419,21 @@
 
         Returns:
             Iterator of type that is equal to the output type of ``walk_fn``.
         """
         return self._walk_backwards(
             lambda p: p._children,
             depth_first,
+            reverse,
             only_differentiable,
             repeat_visited,
             walk_fn,
         )
 
-    def _clean(self):
+    def _clean(self) -> None:
         """
         Cleans up :attr:`_children` and :attr:`_parents` for all nodes in the subgraph of this node (depth first)
         """
         if self._cleaned:
             return
         self._cleaned = True
         for (node, _) in self._children:
@@ -447,14 +463,18 @@
         """
         Returns:
             bool: True if this is a cost node in the stochastic computation graph, False otherwise.
         """
         return False
 
     @property
+    def parents(self) -> List[Tensor]:
+        return list(map(lambda p: p[0], self._parents))
+
+    @property
     def requires_grad(self) -> bool:
         return self._tensor.requires_grad
 
     @property
     def plate_shape(self) -> torch.Size:
         return self._tensor.shape[: self.plate_dims]
 
@@ -532,14 +552,20 @@
         retain_graph: bool = False,
     ) -> None:
         raise NotImplementedError(
             "Cannot call .backward on storch.Tensor. Instead, register cost nodes using "
             "storch.add_cost, then use storch.backward()."
         )
 
+    def is_in(self, tensors: Iterable[Tensor]) -> bool:
+        for tensor in tensors:
+            if tensor is self:
+                return True
+
+        return False
     # region OperatorOverloads
 
     def __len__(self) -> int:
         return self._tensor.__len__()
 
     def __index__(self) -> int:
         raise IllegalStorchExposeError("Cannot use storch tensors as index.")
@@ -733,14 +759,16 @@
 
     def __rxor__(self, other):
         return torch.logical_xor(other, self)
 
     # endregion
 
 
+
+
 class CostTensor(Tensor):
     def __init__(self, tensor: torch.Tensor, parents, plate_links: [Plate], name: str):
         super().__init__(tensor, parents, plate_links, name)
 
     @property
     def is_cost(self) -> bool:
         return True
@@ -800,15 +828,15 @@
         plates: [Plate],
         name: str,
         n: int,
         distribution: Distribution,
         requires_grad: bool,
         method: Optional[storch.method.Method] = None,
     ):
-        self.distribution = distribution
+        self.distribution: Distribution = distribution
         super().__init__(tensor, parents, plates, name)
         self._requires_grad = requires_grad
         self.n = n
         self.method = method
         self.param_grads = {}
         self._grad = None
         self._clean_hooks = []
```

### Comparing `storchastic-0.3.5/storch/typing.py` & `storchastic-0.3.6/storch/typing.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/storch/unique.py` & `storchastic-0.3.6/storch/unique.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/storch/util.py` & `storchastic-0.3.6/storch/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 def magic_box(l: Tensor):
     """
     Implements the MagicBox operator from
     DiCE: The Infinitely Differentiable Monte-Carlo Estimator https://arxiv.org/abs/1802.05098
     It returns 1 in the forward pass, but returns magic_box(l) \cdot r in the backwards pass.
     This allows for any-order gradient estimation.
     """
-    return (l - l.detach()).exp()
+    return torch.exp(l - l.detach())
 
 def print_graph(costs: [CostTensor]):
     nodes = topological_sort(costs)
     counters = {"s": 1, "c": 1, "d": 1}
     names = {}
 
     def get_name(node, names):
@@ -137,14 +137,16 @@
         if isinstance(input, Tensor):
             input = input._tensor
         if output_t is input:
             # This can happen if the input is a parameter of the output distribution
             has_paths[i] = True
         else:
             to_search.append((i, input))
+    if len(to_search) == 0:
+        return False
     for p in walk_backward_graph(output_t):
         found_i = None
         for j, (i, input) in enumerate(to_search):
             if hasattr(p, "variable") and p.variable is input:
                 found_i = i
                 break
             elif input.grad_fn and p is input.grad_fn:
@@ -267,15 +269,15 @@
         slices = []
         for i in range(amt_slices):
             slices.append(slice(i * slice_length, (i + 1) * slice_length))
 
     new_plates = tensor.plates.copy()
 
     index = tensor.get_plate_dim_index(plate.name)
-    plates_index = new_plates.index(plate)
+    plates_index = new_plates.index_in(plate)
     if not create_plates and tensor.plate_dims != index + 1:
         for _plate in reversed(tensor.plates):
             if _plate.n > 1:
                 # Overwrite old plate
                 new_plates.remove(_plate)
                 new_plates[plates_index] = _plate
                 break
```

### Comparing `storchastic-0.3.5/storch/wrappers.py` & `storchastic-0.3.6/storch/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from __future__ import annotations
 
+from copy import copy
 from typing import Union, Any, Tuple, List, Optional, Dict, Callable
 
+from torch.distributions import Distribution
+
 import storch
 import torch
 from collections.abc import Iterable, Mapping
 from functools import wraps
 from storch.exceptions import IllegalStorchExposeError
 from contextlib import contextmanager
 
@@ -99,14 +102,15 @@
                 plate_dims.append(plate.n)
             else:
                 # Make sure to use a's plate size here. It's actually possible they are different in ancestral plates!
                 plate_dims.append(tensor.shape[i])
 
         # Optionally expand the singleton dimensions to the plate size
         if expand_plates:
+            # TODO: Can maybe be optimized by only running this if the shape is different
             tensor = tensor.expand(tuple(plate_dims) + tensor.shape[len(plate_dims) :])
         # Optionally flatten the plate dimensions to a single batch dimension
         if flatten_plates:
             assert expand_plates
             tensor = tensor.reshape((-1,) + tensor.shape[len(plate_dims) :])
 
         return tensor
@@ -136,14 +140,28 @@
                     flatten_plates,
                     event_dims,
                 )
             )
         if isinstance(a, tuple):
             return tuple(l)
         return l
+    elif isinstance(a, Distribution):
+        from storch.util import get_distr_parameters
+        params = get_distr_parameters(a, False)
+        params_unsq = _unsqueeze_and_unwrap(params, multi_dim_plates, align_tensors, l_broadcast, expand_plates, flatten_plates, event_dims)
+        try:
+            if 'logits' in params and 'probs' in params:
+                # Discrete distributions don't like it if you pass both probs and logits
+                _a = a.__class__(logits=params_unsq['logits'])
+            else:
+                # Attempt to instantiate a copy of the distribution using the unsqueezed parameters
+                _a = a.__class__(**params_unsq)
+        except Exception as e:
+            return a
+        return _a
     else:
         return a
 
 
 def _prepare_args(
     fn_args,
     fn_kwargs,
@@ -254,15 +272,34 @@
         return None, index
     if isinstance(o, storch.Tensor):
         if o.stochastic:
             raise RuntimeError(
                 "Creation of stochastic storch Tensor within deterministic context"
             )
         # TODO: Does this require shape checking? Parent/Plate checking?
-        return o, index + 1
+        #   This might be very buggy, hard to figure out how to merge these concepts... Try to prevent creating
+        #   storch.Tensors within deterministic contexts.
+        new_plates = o.plates.copy()
+        for plate in reversed(plates):
+            plate_found = False
+            for i, other_plate in enumerate(new_plates):
+                if plate.name == other_plate.name:
+                    plate_found = True
+                    if hasattr(plate, "variable_index") :
+                        assert hasattr(other_plate, "variable_index")
+                        if plate.variable_index > other_plate.variable_index:
+                            new_plates[i] = plate
+            if not plate_found:
+                new_plates.insert(0, plate)
+
+        new_parents = parents.copy()
+        new_parents.append(o)
+
+        t = storch.Tensor(o._tensor, parents, new_plates, name=name + str(index))
+        return t, index + 1
     if isinstance(o, torch.Tensor):  # Explicitly _not_ a storch.Tensor
         if unflatten_plates:
             plate_dims = tuple([plate.n for plate in plates if plate.n > 1])
             o = o.reshape(plate_dims + o.shape[1:])
         t = storch.Tensor(o, parents, plates, name=name + str(index))
         return t, index + 1
     if is_iterable(o):
```

### Comparing `storchastic-0.3.5/storchastic.egg-info/PKG-INFO` & `storchastic-0.3.6/storchastic.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,101 @@
 Metadata-Version: 2.1
 Name: storchastic
-Version: 0.3.5
+Version: 0.3.6
 Summary: Stochastic Deep Learning for PyTorch
 Home-page: https://github.com/HEmile/storchastic
 Author: Emile van Krieken
 Author-email: e.van.krieken@vu.nl
-License: UNKNOWN
-Description: ![](logo.png)
-        
-        
-        
-        
-        ## General Stochastic Automatic Differentiation for Pytorch
-        [![Documentation Status](https://readthedocs.org/projects/storchastic/badge/?version=latest)](https://storchastic.readthedocs.io/en/latest/?badge=latest)
-        
-        - [Documentation](https://storchastic.readthedocs.io/en/latest/)
-        - [Read the paper](https://arxiv.org/abs/2104.00428)
-        
-        **Storchastic** is a PyTorch library for stochastic gradient estimation in Deep Learning [1]. Many state of the art deep learning
-        models use gradient estimation, in particular within the fields of Variational Inference and Reinforcement Learning.
-        While PyTorch computes gradients of deterministic computation graphs automatically, it will not estimate
-        gradients on **stochastic computation graphs** [2].
-        
-        With Storchastic, you can easily define any stochastic deep learning model and let it estimate the gradients for you. 
-        Storchastic provides a large range of gradient estimation methods that you can plug and play, to figure out which one works
-        best for your problem. Storchastic provides automatic broadcasting of sampled batch dimensions, which increases code
-        readability and allows implementing complex models with ease.
-        
-        When dealing with continuous random variables and differentiable functions, the popular reparameterization method [3] is usually
-        very effective. However, this method is not applicable when dealing with discrete random variables or non-differentiable functions.
-        This is why Storchastic has a focus on gradient estimators for discrete random variables, non-differentiable functions and
-        sequence models.
-        
-        
-        [Documentation on Read the Docs.](https://storchastic.readthedocs.io/en/latest/)
-        
-        [Example: Discrete Variational Auto-Encoder](TODO)
-        
-        ## Installation
-        In your virtual Python environment, run
-        `pip install storchastic`
-        
-        **Requires** Pytorch 1.**8** and [Pyro](http://pyro.ai). The code is build using Python 3.8.
-        
-        ## Algorithms
-        Feel free to create an issue if an estimator is missing here.
-        - Reparameterization [1, 3]
-        - Score Function (REINFORCE) with Moving Average baseline [1, 4]
-        - Score Function with Batch Average Baseline [5, 6]
-        - Expected value for enumerable distributions
-        - (Straight through) Gumbel Softmax [7, 8]
-        - LAX, RELAX [9] 
-        - REBAR [10]
-        - REINFORCE Without Replacement [6]
-        - Unordered Set Estimator [13]
-        - ARM [15]
-        
-        ### In development
-        - Memory Augmented Policy Optimization [11]
-        - Rao-Blackwellized REINFORCE [12]
-        
-        ### Planned
-        - Measure valued derivatives [1, 14]
-        - Automatic Credit Assignment [16]
-        - ...
-        
-        ## References
-        - [1] [Monte Carlo Gradient Estimation in Machine Learning](https://arxiv.org/abs/1906.10652), Mohamed et al, 2019
-        - [2] [Gradient Estimation Using Stochastic Computation Graphs](https://arxiv.org/abs/1506.05254), Schulman et al, NeurIPS 2015
-        - [3] [Auto-Encoding Variational Bayes](https://arxiv.org/abs/1312.6114), Kingma and Welling, ICLR 2014
-        - [4] [Simple statistical gradient-following algorithms for connectionist reinforcement learning](https://link-springer-com.vu-nl.idm.oclc.org/article/10.1007/BF00992696), Williams, Machine Learning 1992
-        - [5] [Variational inference for Monte Carlo objectives](https://arxiv.org/abs/1602.06725), Mnih and Rezende, ICML 2016
-        - [6] [Buy 4 REINFORCE Samples, Get a Baseline for Free!](https://openreview.net/pdf?id=r1lgTGL5DE), Kool et al, ICLR Workshop dlStructPred 2019
-        - [7] [Categorical Reparameterization with Gumbel-Softmax](https://arxiv.org/abs/1611.01144), Jang et al, ICLR 2017
-        - [8] [The Concrete Distribution: A Continuous Relaxation of Discrete Random Variables](https://arxiv.org/abs/1611.00712), Maddison et al, ICLR 2017
-        - [9] [Backpropagation through the Void: Optimizing control variates for black-box gradient estimation](https://arxiv.org/abs/1711.00123), Grathwohl et al, ICLR 2018
-        - [10] [REBAR: Low-variance, unbiased gradient estimates for discrete latent variable models](https://arxiv.org/abs/1703.07370), Tucker et al, NeurIPS 2017
-        - [11] [Memory Augmented Policy Optimization for Program Synthesis and Semantic Parsing](https://arxiv.org/abs/1807.02322), Liang et al, NeurIPS 2018
-        - [12] [Rao-Blackwellized Stochastic Gradients for Discrete Distributions](https://arxiv.org/abs/1810.04777), Liu et al, ICML 2019
-        - [13] [Estimating Gradients for Discrete Random Variables by Sampling without Replacement](https://openreview.net/forum?id=rklEj2EFvB), Kool et al, ICLR 2020
-        - [14] [Measure-Valued Derivatives for Approximate Bayesian Inference](http://bayesiandeeplearning.org/2019/papers/76.pdf), Rosca et al, Workshop on Bayesian Deep Learning (NeurIPS 2019)
-        - [15] [ARM: Augment-REINFORCE-Merge Gradient for Stochastic Binary Networks](https://arxiv.org/abs/1807.11143), Yin and Zhou, ICLR 2019
-        - [16] [Credit Assignment Techniques in Stochastic Computation Graphs](https://arxiv.org/abs/1901.01761), Weber et al, AISTATS 2019
-        
-        ## Cite
-        To cite Storchastic, please cite this preprint:
-        ```
-        @article{van2021storchastic,
-          title={Storchastic: A Framework for General Stochastic Automatic Differentiation},
-          author={van Krieken, Emile and Tomczak, Jakub M and Teije, Annette ten},
-          journal={arXiv preprint arXiv:2104.00428},
-          year={2021}
-        }
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![](logo.png)
+
+
+
+
+## General Stochastic Automatic Differentiation for Pytorch
+[![Documentation Status](https://readthedocs.org/projects/storchastic/badge/?version=latest)](https://storchastic.readthedocs.io/en/latest/?badge=latest)
+
+- [Documentation](https://storchastic.readthedocs.io/en/latest/)
+- [Read the paper](https://arxiv.org/abs/2104.00428)
+
+**Storchastic** is a PyTorch library for stochastic gradient estimation in Deep Learning [1]. Many state of the art deep learning
+models use gradient estimation, in particular within the fields of Variational Inference and Reinforcement Learning.
+While PyTorch computes gradients of deterministic computation graphs automatically, it will not estimate
+gradients on **stochastic computation graphs** [2].
+
+With Storchastic, you can easily define any stochastic deep learning model and let it estimate the gradients for you. 
+Storchastic provides a large range of gradient estimation methods that you can plug and play, to figure out which one works
+best for your problem. Storchastic provides automatic broadcasting of sampled batch dimensions, which increases code
+readability and allows implementing complex models with ease.
+
+When dealing with continuous random variables and differentiable functions, the popular reparameterization method [3] is usually
+very effective. However, this method is not applicable when dealing with discrete random variables or non-differentiable functions.
+This is why Storchastic has a focus on gradient estimators for discrete random variables, non-differentiable functions and
+sequence models.
+
+
+[Documentation on Read the Docs.](https://storchastic.readthedocs.io/en/latest/)
+
+[Example: Discrete Variational Auto-Encoder](examples/vae/train.py)
+
+## Installation
+In your virtual Python environment, run
+`pip install storchastic`
+
+**Requires** Pytorch 1.**8** and [Pyro](http://pyro.ai). The code is build using Python 3.8.
+
+## Algorithms
+Feel free to create an issue if an estimator is missing here.
+- Reparameterization [1, 3]
+- Score Function (REINFORCE) with Moving Average baseline [1, 4]
+- Score Function with Batch Average Baseline [5, 6]
+- Expected value for enumerable distributions
+- (Straight through) Gumbel Softmax [7, 8]
+- LAX, RELAX [9] 
+- REBAR [10]
+- REINFORCE Without Replacement [6]
+- Unordered Set Estimator [13]
+- ARM [15]
+- Rao-Blackwellized REINFORCE [12]
+
+### In development
+- Memory Augmented Policy Optimization [11]
+
+### Planned
+- Measure valued derivatives [1, 14]
+- Automatic Credit Assignment [16]
+- ...
+
+## References
+- [1] [Monte Carlo Gradient Estimation in Machine Learning](https://arxiv.org/abs/1906.10652), Mohamed et al, 2019
+- [2] [Gradient Estimation Using Stochastic Computation Graphs](https://arxiv.org/abs/1506.05254), Schulman et al, NeurIPS 2015
+- [3] [Auto-Encoding Variational Bayes](https://arxiv.org/abs/1312.6114), Kingma and Welling, ICLR 2014
+- [4] [Simple statistical gradient-following algorithms for connectionist reinforcement learning](https://link-springer-com.vu-nl.idm.oclc.org/article/10.1007/BF00992696), Williams, Machine Learning 1992
+- [5] [Variational inference for Monte Carlo objectives](https://arxiv.org/abs/1602.06725), Mnih and Rezende, ICML 2016
+- [6] [Buy 4 REINFORCE Samples, Get a Baseline for Free!](https://openreview.net/pdf?id=r1lgTGL5DE), Kool et al, ICLR Workshop dlStructPred 2019
+- [7] [Categorical Reparameterization with Gumbel-Softmax](https://arxiv.org/abs/1611.01144), Jang et al, ICLR 2017
+- [8] [The Concrete Distribution: A Continuous Relaxation of Discrete Random Variables](https://arxiv.org/abs/1611.00712), Maddison et al, ICLR 2017
+- [9] [Backpropagation through the Void: Optimizing control variates for black-box gradient estimation](https://arxiv.org/abs/1711.00123), Grathwohl et al, ICLR 2018
+- [10] [REBAR: Low-variance, unbiased gradient estimates for discrete latent variable models](https://arxiv.org/abs/1703.07370), Tucker et al, NeurIPS 2017
+- [11] [Memory Augmented Policy Optimization for Program Synthesis and Semantic Parsing](https://arxiv.org/abs/1807.02322), Liang et al, NeurIPS 2018
+- [12] [Rao-Blackwellized Stochastic Gradients for Discrete Distributions](https://arxiv.org/abs/1810.04777), Liu et al, ICML 2019
+- [13] [Estimating Gradients for Discrete Random Variables by Sampling without Replacement](https://openreview.net/forum?id=rklEj2EFvB), Kool et al, ICLR 2020
+- [14] [Measure-Valued Derivatives for Approximate Bayesian Inference](http://bayesiandeeplearning.org/2019/papers/76.pdf), Rosca et al, Workshop on Bayesian Deep Learning (NeurIPS 2019)
+- [15] [ARM: Augment-REINFORCE-Merge Gradient for Stochastic Binary Networks](https://arxiv.org/abs/1807.11143), Yin and Zhou, ICLR 2019
+- [16] [Credit Assignment Techniques in Stochastic Computation Graphs](https://arxiv.org/abs/1901.01761), Weber et al, AISTATS 2019
+
+## Cite
+To cite Storchastic, please cite this preprint:
+```
+@article{van2021storchastic,
+  title={Storchastic: A Framework for General Stochastic Automatic Differentiation},
+  author={van Krieken, Emile and Tomczak, Jakub M and Teije, Annette ten},
+  journal={arXiv preprint arXiv:2104.00428},
+  year={2021}
+}
+```
```

### Comparing `storchastic-0.3.5/storchastic.egg-info/SOURCES.txt` & `storchastic-0.3.6/storchastic.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+LICENSE
 README.md
 setup.py
 examples/__init__.py
 examples/bernoulli_grad_var.py
 examples/bernoulli_toy.py
 examples/introduction.py
+examples/someone_test_file.py
 examples/vae_reference.py
 examples/vae/__init__.py
 examples/vae/bernoulli_vae.py
 examples/vae/discrete_vae.py
 examples/vae/normal_vae.py
+examples/vae/sample_k.py
 examples/vae/train.py
 examples/vae/vae.py
 storch/__init__.py
 storch/exceptions.py
 storch/excluded_init.py
 storch/inference.py
 storch/storch.py
@@ -22,20 +25,23 @@
 storch/util.py
 storch/wrappers.py
 storch/method/__init__.py
 storch/method/arm.py
 storch/method/baseline.py
 storch/method/method.py
 storch/method/multi_sample_reinforce.py
+storch/method/rao_blackwell.py
 storch/method/relax.py
 storch/method/unordered.py
 storch/nn/__init__.py
 storch/nn/losses.py
 storch/sampling/__init__.py
 storch/sampling/expect.py
+storch/sampling/importance_sampling.py
+storch/sampling/mapo.py
 storch/sampling/method.py
 storch/sampling/seq.py
 storch/sampling/swor.py
 storch/sampling/unordered_set.py
 storchastic.egg-info/PKG-INFO
 storchastic.egg-info/SOURCES.txt
 storchastic.egg-info/dependency_links.txt
```

### Comparing `storchastic-0.3.5/test/collect_env.py` & `storchastic-0.3.6/test/collect_env.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/test/is_unbiased.py` & `storchastic-0.3.6/test/is_unbiased.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/test/test.py` & `storchastic-0.3.6/test/test.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/test/test2.py` & `storchastic-0.3.6/test/test2.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/test/test_allowed.py` & `storchastic-0.3.6/test/test_allowed.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/test/test_swor.py` & `storchastic-0.3.6/test/test_swor.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/test/test_tensor.py` & `storchastic-0.3.6/test/test_tensor.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/test/testancestral.py` & `storchastic-0.3.6/test/testancestral.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/test/testcat.py` & `storchastic-0.3.6/test/testcat.py`

 * *Files identical despite different names*

### Comparing `storchastic-0.3.5/test/testrelax.py` & `storchastic-0.3.6/test/testrelax.py`

 * *Files identical despite different names*

