# Comparing `tmp/UtilsRL-0.5.5.tar.gz` & `tmp/UtilsRL-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UtilsRL-0.5.5.tar", last modified: Fri Mar 31 06:25:52 2023, max compression
+gzip compressed data, was "UtilsRL-0.5.6.tar", last modified: Tue Apr 11 03:05:11 2023, max compression
```

## Comparing `UtilsRL-0.5.5.tar` & `UtilsRL-0.5.6.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:52.716145 UtilsRL-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-31 06:25:52.716145 UtilsRL-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:52.704145 UtilsRL-0.5.5/UtilsRL/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:52.708145 UtilsRL-0.5.5/UtilsRL/data_structure/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/data_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/data_structure/data_structure.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:52.708145 UtilsRL-0.5.5/UtilsRL/env/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/env/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:52.708145 UtilsRL-0.5.5/UtilsRL/env/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/env/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/env/wrapper/atari_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/env/wrapper/base_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/env/wrapper/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/env/wrapper/mujoco_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:52.708145 UtilsRL-0.5.5/UtilsRL/exp/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/exp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/exp/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/exp/_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/exp/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/exp/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/exp/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:52.712144 UtilsRL-0.5.5/UtilsRL/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/logger/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/logger/composite_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/logger/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/logger/text_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/logger/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:52.712144 UtilsRL-0.5.5/UtilsRL/math/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/math/distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:52.712144 UtilsRL-0.5.5/UtilsRL/misc/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/misc/chore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/misc/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/misc/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:52.712144 UtilsRL-0.5.5/UtilsRL/net/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/net/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/net/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/net/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/net/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/net/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/net/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:52.712144 UtilsRL-0.5.5/UtilsRL/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/plot/tb_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:52.716145 UtilsRL-0.5.5/UtilsRL/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30972 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/rl/actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:52.716145 UtilsRL-0.5.5/UtilsRL/rl/buffer/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/rl/buffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/rl/buffer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/rl/buffer/prioritized_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/rl/buffer/transition_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/rl/buffer/trjectory_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/rl/critic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/rl/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/rl/video_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:52.716145 UtilsRL-0.5.5/UtilsRL/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/third_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/UtilsRL/third_party/tqdm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:25:52.708145 UtilsRL-0.5.5/UtilsRL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-31 06:25:52.000000 UtilsRL-0.5.5/UtilsRL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-31 06:25:52.000000 UtilsRL-0.5.5/UtilsRL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 06:25:52.000000 UtilsRL-0.5.5/UtilsRL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-31 06:25:52.000000 UtilsRL-0.5.5/UtilsRL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-31 06:25:52.000000 UtilsRL-0.5.5/UtilsRL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 06:25:52.716145 UtilsRL-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-03-31 06:25:42.000000 UtilsRL-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.139198 UtilsRL-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-11 03:05:11.139198 UtilsRL-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.131198 UtilsRL-0.5.6/UtilsRL/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.131198 UtilsRL-0.5.6/UtilsRL/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/data_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/data_structure/data_structure.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.131198 UtilsRL-0.5.6/UtilsRL/env/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/env/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.131198 UtilsRL-0.5.6/UtilsRL/env/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/env/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/env/wrapper/atari_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/env/wrapper/base_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/env/wrapper/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/env/wrapper/dmc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/env/wrapper/mujoco_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.135198 UtilsRL-0.5.6/UtilsRL/exp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/exp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/exp/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/exp/_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/exp/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/exp/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/exp/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.135198 UtilsRL-0.5.6/UtilsRL/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/logger/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/logger/composite_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/logger/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/logger/text_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/logger/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.135198 UtilsRL-0.5.6/UtilsRL/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/math/distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.135198 UtilsRL-0.5.6/UtilsRL/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/misc/chore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/misc/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/misc/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.135198 UtilsRL-0.5.6/UtilsRL/net/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/net/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/net/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/net/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/net/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/net/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.135198 UtilsRL-0.5.6/UtilsRL/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/plot/tb_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.135198 UtilsRL-0.5.6/UtilsRL/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30972 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.139198 UtilsRL-0.5.6/UtilsRL/rl/buffer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/buffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/buffer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/buffer/prioritized_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/buffer/transition_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/buffer/trjectory_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/rl/video_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.139198 UtilsRL-0.5.6/UtilsRL/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/UtilsRL/third_party/tqdm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:05:11.131198 UtilsRL-0.5.6/UtilsRL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-11 03:05:11.000000 UtilsRL-0.5.6/UtilsRL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-11 03:05:11.000000 UtilsRL-0.5.6/UtilsRL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:05:11.000000 UtilsRL-0.5.6/UtilsRL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 03:05:11.000000 UtilsRL-0.5.6/UtilsRL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 03:05:11.000000 UtilsRL-0.5.6/UtilsRL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 03:05:11.139198 UtilsRL-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-11 03:05:03.000000 UtilsRL-0.5.6/setup.py
```

### Comparing `UtilsRL-0.5.5/LICENSE` & `UtilsRL-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/PKG-INFO` & `UtilsRL-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UtilsRL
-Version: 0.5.5
+Version: 0.5.6
 Summary: A python module desgined for RL logging, monitoring and experiments managing. 
 Home-page: https://github.com/typoverflow/UtilsRL
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `UtilsRL-0.5.5/README.md` & `UtilsRL-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/data_structure/data_structure.cc` & `UtilsRL-0.5.6/UtilsRL/data_structure/data_structure.cc`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/env/wrapper/atari_wrapper.py` & `UtilsRL-0.5.6/UtilsRL/env/wrapper/atari_wrapper.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/env/wrapper/base_wrapper.py` & `UtilsRL-0.5.6/UtilsRL/env/wrapper/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/env/wrapper/compat.py` & `UtilsRL-0.5.6/UtilsRL/env/wrapper/compat.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/env/wrapper/mujoco_wrapper.py` & `UtilsRL-0.5.6/UtilsRL/env/wrapper/mujoco_wrapper.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/exp/__init__.py` & `UtilsRL-0.5.6/UtilsRL/exp/__init__.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/exp/_device.py` & `UtilsRL-0.5.6/UtilsRL/exp/_device.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/exp/argparse.py` & `UtilsRL-0.5.6/UtilsRL/exp/argparse.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/exp/precision.py` & `UtilsRL-0.5.6/UtilsRL/exp/precision.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/exp/snapshot.py` & `UtilsRL-0.5.6/UtilsRL/exp/snapshot.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/logger/base_logger.py` & `UtilsRL-0.5.6/UtilsRL/logger/base_logger.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/logger/composite_logger.py` & `UtilsRL-0.5.6/UtilsRL/logger/composite_logger.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/logger/tensorboard_logger.py` & `UtilsRL-0.5.6/UtilsRL/logger/tensorboard_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import pickle
 import numpy as np
 from abc import ABC, abstractmethod
 from datetime import datetime
 from typing import Dict as DictLike
-from typing import Optional, Sequence, Union, Any
+from typing import Optional, Sequence, Union, Any, List
 
 from UtilsRL.logger.base_logger import LogLevel, BaseLogger, make_unique_name, save_fn, load_fn
 
 numpy_compatible = np.ndarray
 try:
     import torch
     numpy_compatible = torch.Tensor
@@ -151,14 +151,28 @@
         :param vid_tensor: video data. 
         :param global_step: global step.
         :param fps: frames per second.
         :param dataformat: specify different permutation of the video tensor.
         """
         self.tb_writer.add_video(tag, vid_tensor, step, fps)
 
+    def log_histogram(
+        self, 
+        tag: str, 
+        values: Union[np.ndarray, List], 
+        step: Optional[int]=None, 
+    ):
+        """Add histogram to tensorboard. 
+        
+        :param tag: the identifier of the histogram.
+        :param values: the values, should be list or np.ndarray. 
+        :param global_step: global step.
+        """
+        self.tb_writer.add_histogram(tag, np.asarray(values), step)
+
     def log_object(
         self,
         name: str, 
         object: Any, 
         type: Optional[str]="model", 
         path: Optional[str] = None, 
         protocol: str="torch"):
```

### Comparing `UtilsRL-0.5.5/UtilsRL/logger/text_logger.py` & `UtilsRL-0.5.6/UtilsRL/logger/text_logger.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/logger/wandb_logger.py` & `UtilsRL-0.5.6/UtilsRL/logger/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/math/distributions.py` & `UtilsRL-0.5.6/UtilsRL/math/distributions.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/misc/chore.py` & `UtilsRL-0.5.6/UtilsRL/misc/chore.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/misc/decorator.py` & `UtilsRL-0.5.6/UtilsRL/misc/decorator.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/misc/namespace.py` & `UtilsRL-0.5.6/UtilsRL/misc/namespace.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/monitor.py` & `UtilsRL-0.5.6/UtilsRL/monitor.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/net/basic.py` & `UtilsRL-0.5.6/UtilsRL/net/basic.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/net/cnn.py` & `UtilsRL-0.5.6/UtilsRL/net/cnn.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/net/mlp.py` & `UtilsRL-0.5.6/UtilsRL/net/mlp.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/net/rnn.py` & `UtilsRL-0.5.6/UtilsRL/net/rnn.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/plot/tb_parser.py` & `UtilsRL-0.5.6/UtilsRL/plot/tb_parser.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/rl/actor.py` & `UtilsRL-0.5.6/UtilsRL/rl/actor.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/rl/buffer/__init__.py` & `UtilsRL-0.5.6/UtilsRL/rl/buffer/__init__.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/rl/buffer/base.py` & `UtilsRL-0.5.6/UtilsRL/rl/buffer/base.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/rl/buffer/prioritized_replay.py` & `UtilsRL-0.5.6/UtilsRL/rl/buffer/prioritized_replay.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -175,8 +175,8 @@
             batch_idx = np.asarray([batch_idx, ])
         metric_value = np.asarray(metric_value)
         if len(metric_value.shape) == 0:
             metric_value = np.asarray([metric_value, ])
         # update crendential
         self.max_metric_value = max(np.max(metric_value), self.max_metric_value)
         self.sum_tree.update(batch_idx, self.metric_fn(metric_value))
-        self.min_tree.update(batch_idx, self.metric_fn(metric_value))
+        self.min_tree.update(batch_idx, self.metric_fn(metric_value))
```

### Comparing `UtilsRL-0.5.5/UtilsRL/rl/buffer/transition_replay.py` & `UtilsRL-0.5.6/UtilsRL/rl/buffer/transition_replay.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/rl/buffer/trjectory_replay.py` & `UtilsRL-0.5.6/UtilsRL/rl/buffer/trjectory_replay.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/rl/critic.py` & `UtilsRL-0.5.6/UtilsRL/rl/critic.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/rl/normalizer.py` & `UtilsRL-0.5.6/UtilsRL/rl/normalizer.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/rl/video_recorder.py` & `UtilsRL-0.5.6/UtilsRL/rl/video_recorder.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL/third_party/tqdm.py` & `UtilsRL-0.5.6/UtilsRL/third_party/tqdm.py`

 * *Files identical despite different names*

### Comparing `UtilsRL-0.5.5/UtilsRL.egg-info/PKG-INFO` & `UtilsRL-0.5.6/UtilsRL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UtilsRL
-Version: 0.5.5
+Version: 0.5.6
 Summary: A python module desgined for RL logging, monitoring and experiments managing. 
 Home-page: https://github.com/typoverflow/UtilsRL
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `UtilsRL-0.5.5/UtilsRL.egg-info/SOURCES.txt` & `UtilsRL-0.5.6/UtilsRL.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 UtilsRL/data_structure/__init__.py
 UtilsRL/data_structure/data_structure.cc
 UtilsRL/env/__init__.py
 UtilsRL/env/wrapper/__init__.py
 UtilsRL/env/wrapper/atari_wrapper.py
 UtilsRL/env/wrapper/base_wrapper.py
 UtilsRL/env/wrapper/compat.py
+UtilsRL/env/wrapper/dmc_wrapper.py
 UtilsRL/env/wrapper/mujoco_wrapper.py
 UtilsRL/exp/__init__.py
 UtilsRL/exp/_device.py
 UtilsRL/exp/_seed.py
 UtilsRL/exp/argparse.py
 UtilsRL/exp/precision.py
 UtilsRL/exp/snapshot.py
@@ -32,15 +33,14 @@
 UtilsRL/math/__init__.py
 UtilsRL/math/distributions.py
 UtilsRL/misc/__init__.py
 UtilsRL/misc/chore.py
 UtilsRL/misc/decorator.py
 UtilsRL/misc/namespace.py
 UtilsRL/net/__init__.py
-UtilsRL/net/attention.py
 UtilsRL/net/basic.py
 UtilsRL/net/cnn.py
 UtilsRL/net/mlp.py
 UtilsRL/net/rnn.py
 UtilsRL/net/utils.py
 UtilsRL/plot/__init__.py
 UtilsRL/plot/tb_parser.py
```

### Comparing `UtilsRL-0.5.5/setup.py` & `UtilsRL-0.5.6/setup.py`

 * *Files identical despite different names*

