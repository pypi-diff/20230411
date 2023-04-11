# Comparing `tmp/lightning-fabric-2.0.1.tar.gz` & `tmp/lightning-fabric-2.0.1.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-fabric-2.0.1.tar", last modified: Thu Mar 30 14:47:01 2023, max compression
+gzip compressed data, was "lightning-fabric-2.0.1.post0.tar", last modified: Tue Apr 11 18:44:36 2023, max compression
```

## Comparing `lightning-fabric-2.0.1.tar` & `lightning-fabric-2.0.1.post0.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.914367 lightning-fabric-2.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.906367 lightning-fabric-2.0.1/.actions/
--rw-r--r--   0 runner    (1001) docker     (122)    17395 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (122)    11349 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     8279 2023-03-30 14:47:01.914367 lightning-fabric-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    22118 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.906367 lightning-fabric-2.0.1/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.906367 lightning-fabric-2.0.1/requirements/fabric/
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/requirements/fabric/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/requirements/fabric/devel.txt
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/requirements/fabric/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/requirements/fabric/examples.txt
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/requirements/fabric/strategies.txt
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/requirements/fabric/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-30 14:47:01.914367 lightning-fabric-2.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     7917 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.906367 lightning-fabric-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.910367 lightning-fabric-2.0.1/src/lightning_fabric/
--rw-r--r--   0 runner    (1001) docker     (122)    10727 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/src/lightning_fabric/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6967 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/src/lightning_fabric/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      477 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/src/lightning_fabric/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/src/lightning_fabric/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/src/lightning_fabric/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.910367 lightning-fabric-2.0.1/src/lightning_fabric/accelerators/
--rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/accelerators/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2722 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/accelerators/cpu.py
--rw-r--r--   0 runner    (1001) docker     (122)    13986 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/accelerators/cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/accelerators/mps.py
--rw-r--r--   0 runner    (1001) docker     (122)     4579 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/accelerators/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     5846 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/accelerators/tpu.py
--rw-r--r--   0 runner    (1001) docker     (122)     7053 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    27495 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/connector.py
--rw-r--r--   0 runner    (1001) docker     (122)    39832 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/fabric.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.910367 lightning-fabric-2.0.1/src/lightning_fabric/loggers/
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7694 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/loggers/csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4500 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)    12795 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.910367 lightning-fabric-2.0.1/src/lightning_fabric/plugins/
--rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.910367 lightning-fabric-2.0.1/src/lightning_fabric/plugins/collectives/
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/collectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3650 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/collectives/collective.py
--rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/collectives/single_device.py
--rw-r--r--   0 runner    (1001) docker     (122)     8127 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/collectives/torch_collective.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.910367 lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/
--rw-r--r--   0 runner    (1001) docker     (122)     1309 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/cluster_environment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/kubeflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     3662 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/lightning.py
--rw-r--r--   0 runner    (1001) docker     (122)     7571 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/lsf.py
--rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/mpi.py
--rw-r--r--   0 runner    (1001) docker     (122)     7610 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/slurm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/torchelastic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2641 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.910367 lightning-fabric-2.0.1/src/lightning_fabric/plugins/io/
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2584 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/io/checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     4183 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/io/torch_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/io/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.914367 lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/
--rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5094 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/amp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (122)     1874 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/double.py
--rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (122)     5025 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/tpu.py
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/tpu_bf16.py
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.914367 lightning-fabric-2.0.1/src/lightning_fabric/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)     1538 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8907 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/ddp.py
--rw-r--r--   0 runner    (1001) docker     (122)    37180 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (122)     3579 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/dp.py
--rw-r--r--   0 runner    (1001) docker     (122)    15697 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.914367 lightning-fabric-2.0.1/src/lightning_fabric/strategies/launchers/
--rw-r--r--   0 runner    (1001) docker     (122)      933 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     8044 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/launchers/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (122)     6865 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/launchers/subprocess_script.py
--rw-r--r--   0 runner    (1001) docker     (122)     4208 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/launchers/xla.py
--rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (122)     4441 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/single_device.py
--rw-r--r--   0 runner    (1001) docker     (122)     1975 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/single_tpu.py
--rw-r--r--   0 runner    (1001) docker     (122)    14896 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/strategy.py
--rw-r--r--   0 runner    (1001) docker     (122)     8804 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/strategies/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.914367 lightning-fabric-2.0.1/src/lightning_fabric/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)      918 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4636 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/apply_func.py
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (122)    20420 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4119 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/device_dtype_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     7329 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/device_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)    13054 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     4764 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/rank_zero.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     5486 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/seed.py
--rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/src/lightning_fabric/version.info
--rw-r--r--   0 runner    (1001) docker     (122)     9162 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:47:01.910367 lightning-fabric-2.0.1/src/lightning_fabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8279 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4304 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      853 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-03-30 14:47:01.000000 lightning-fabric-2.0.1/src/lightning_fabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-30 14:46:48.000000 lightning-fabric-2.0.1/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.979967 lightning-fabric-2.0.1.post0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.967967 lightning-fabric-2.0.1.post0/.actions/
+-rw-r--r--   0 runner    (1001) docker     (122)    17395 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11349 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     8285 2023-04-11 18:44:36.979967 lightning-fabric-2.0.1.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    22128 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.967967 lightning-fabric-2.0.1.post0/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/requirements/fabric/
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/requirements/fabric/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/requirements/fabric/devel.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/requirements/fabric/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/requirements/fabric/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/requirements/fabric/strategies.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/requirements/fabric/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 18:44:36.979967 lightning-fabric-2.0.1.post0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7917 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/src/lightning_fabric/
+-rw-r--r--   0 runner    (1001) docker     (122)    10727 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6967 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      477 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/
+-rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2722 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13986 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/mps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4579 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5846 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/tpu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7053 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27495 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/connector.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39832 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/fabric.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7694 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4500 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12795 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/
+-rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3650 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/collective.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8127 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/torch_collective.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.975968 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/
+-rw-r--r--   0 runner    (1001) docker     (122)     1309 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/cluster_environment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/kubeflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3662 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7571 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7610 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/torchelastic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2641 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.975968 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2584 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4183 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/torch_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.975968 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/
+-rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5094 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/amp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1874 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/double.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5025 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/tpu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/tpu_bf16.py
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.975968 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)     1538 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8907 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37212 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3579 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/dp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15697 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.975968 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/
+-rw-r--r--   0 runner    (1001) docker     (122)      933 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8044 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6865 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/subprocess_script.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4208 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/xla.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4441 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1975 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/single_tpu.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14896 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8804 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.979967 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)      918 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4636 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/apply_func.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20420 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4119 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/device_dtype_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7329 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/device_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13054 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4764 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/rank_zero.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5486 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/seed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/version.info
+-rw-r--r--   0 runner    (1001) docker     (122)     9162 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8285 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4304 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/src/version.info
```

### Comparing `lightning-fabric-2.0.1/.actions/assistant.py` & `lightning-fabric-2.0.1.post0/.actions/assistant.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/LICENSE` & `lightning-fabric-2.0.1.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/PKG-INFO` & `lightning-fabric-2.0.1.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-fabric
-Version: 2.0.1
+Version: 2.0.1.post0
 Summary: UNKNOWN
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: lightning-fabric Version: 2.0.1 Summary: UNKNOWN
-Home-page: https://github.com/Lightning-AI/lightning Author: Lightning AI et
-al. Author-email: pytorch@lightning.ai License: Apache-2.0 Download-URL: https:
-//github.com/Lightning-AI/lightning Project-URL: Bug Tracker, https://
+Metadata-Version: 2.1 Name: lightning-fabric Version: 2.0.1.post0 Summary:
+UNKNOWN Home-page: https://github.com/Lightning-AI/lightning Author: Lightning
+AI et al. Author-email: pytorch@lightning.ai License: Apache-2.0 Download-URL:
+https://github.com/Lightning-AI/lightning Project-URL: Bug Tracker, https://
 github.com/Lightning-AI/lightning/issues Project-URL: Documentation, https://
 pytorch-lightning.rtfd.io/en/latest/ Project-URL: Source Code, https://
 github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI Platform:
 UNKNOWN Classifier: Environment :: Console Classifier: Natural Language ::
 English Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
```

### Comparing `lightning-fabric-2.0.1/README.md` & `lightning-fabric-2.0.1.post0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -485,15 +485,15 @@
 
 ______________________________________________________________________
 
 ## Community
 
 The lightning community is maintained by
 
-- [10+ core contributors](https://lightning.ai/docs/pytorch/latest/governance.html) who are all a mix of professional engineers, Research Scientists, and Ph.D. students from top AI labs.
+- [10+ core contributors](https://lightning.ai/docs/pytorch/latest/community/governance.html) who are all a mix of professional engineers, Research Scientists, and Ph.D. students from top AI labs.
 - 590+ active community contributors.
 
 Want to help us build Lightning and reduce boilerplate for thousands of researchers? [Learn how to make your first contribution here](https://lightning.ai/docs/pytorch/stable/generated/CONTRIBUTING.html)
 
 Lightning is also part of the [PyTorch ecosystem](https://pytorch.org/ecosystem/) which requires projects to have solid testing, documentation and support.
 
 ### Asking for help
```

### Comparing `lightning-fabric-2.0.1/pyproject.toml` & `lightning-fabric-2.0.1.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/setup.py` & `lightning-fabric-2.0.1.post0/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/CHANGELOG.md` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/README.md` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/README.md`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/__init__.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/__setup__.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/__setup__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/accelerators/__init__.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/accelerators/accelerator.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/accelerators/cpu.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/cpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/accelerators/cuda.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/cuda.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/accelerators/mps.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/mps.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/accelerators/registry.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/accelerators/tpu.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/cli.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/connector.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/connector.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/fabric.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/fabric.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/loggers/__init__.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/loggers/csv_logs.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/csv_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/loggers/logger.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/loggers/tensorboard.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/__init__.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/collectives/collective.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/collective.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/collectives/single_device.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/collectives/torch_collective.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/torch_collective.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/__init__.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/cluster_environment.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/cluster_environment.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/kubeflow.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/kubeflow.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/lightning.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/lightning.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/lsf.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/lsf.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/mpi.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/mpi.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/slurm.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/slurm.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/torchelastic.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/torchelastic.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/environments/xla.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/io/__init__.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/io/checkpoint_io.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/checkpoint_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/io/torch_io.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/torch_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/io/xla.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/__init__.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/amp.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/amp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/deepspeed.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/double.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/double.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/fsdp.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/precision.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/tpu.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/tpu_bf16.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/tpu_bf16.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/plugins/precision/utils.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/__init__.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/ddp.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/ddp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/deepspeed.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/deepspeed.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,19 +36,21 @@
 from lightning_fabric.utilities.rank_zero import rank_zero_info, rank_zero_only, rank_zero_warn
 from lightning_fabric.utilities.seed import reset_seed
 from lightning_fabric.utilities.types import _PATH
 
 _DEEPSPEED_AVAILABLE = (
     # DeepSpeed fails under 0.8.2 with torch 2.0: https://github.com/microsoft/DeepSpeed/pull/2863
     RequirementCache("deepspeed>=0.8.2")
-    or not _TORCH_GREATER_EQUAL_2_0
-    # check packaging because of https://github.com/microsoft/DeepSpeed/pull/2771
-    # remove the packaging check when min version is >=0.8.1
-    and RequirementCache("deepspeed")
-    and RequirementCache("packaging>=20.0")
+    or (
+        not _TORCH_GREATER_EQUAL_2_0
+        and RequirementCache("deepspeed")
+        # check packaging because of https://github.com/microsoft/DeepSpeed/pull/2771
+        # remove the packaging check when min version is >=0.8.1
+        and RequirementCache("packaging>=20.0")
+    )
 )
 if TYPE_CHECKING and _DEEPSPEED_AVAILABLE:
     import deepspeed
 
 
 # TODO(fabric): Links in the docstrings to PL-specific deepspeed user docs need to be replaced.
 class DeepSpeedStrategy(DDPStrategy, _Sharded):
```

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/dp.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/dp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/fsdp.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/launchers/__init__.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/launchers/base.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/base.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/launchers/launcher.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/launchers/multiprocessing.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/launchers/subprocess_script.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/subprocess_script.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/launchers/xla.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/parallel.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/parallel.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/registry.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/single_device.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/single_tpu.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/single_tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/strategy.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/strategies/xla.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/__init__.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/apply_func.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/apply_func.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/cloud_io.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/cloud_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/data.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/data.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/device_dtype_mixin.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/device_dtype_mixin.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/device_parser.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/device_parser.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/distributed.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/enums.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/exceptions.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/imports.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/logger.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/optimizer.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/optimizer.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/rank_zero.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/rank_zero.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/registry.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/seed.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/seed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/types.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/utilities/warnings.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric/wrappers.py` & `lightning-fabric-2.0.1.post0/src/lightning_fabric/wrappers.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric.egg-info/PKG-INFO` & `lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-fabric
-Version: 2.0.1
+Version: 2.0.1.post0
 Summary: UNKNOWN
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: lightning-fabric Version: 2.0.1 Summary: UNKNOWN
-Home-page: https://github.com/Lightning-AI/lightning Author: Lightning AI et
-al. Author-email: pytorch@lightning.ai License: Apache-2.0 Download-URL: https:
-//github.com/Lightning-AI/lightning Project-URL: Bug Tracker, https://
+Metadata-Version: 2.1 Name: lightning-fabric Version: 2.0.1.post0 Summary:
+UNKNOWN Home-page: https://github.com/Lightning-AI/lightning Author: Lightning
+AI et al. Author-email: pytorch@lightning.ai License: Apache-2.0 Download-URL:
+https://github.com/Lightning-AI/lightning Project-URL: Bug Tracker, https://
 github.com/Lightning-AI/lightning/issues Project-URL: Documentation, https://
 pytorch-lightning.rtfd.io/en/latest/ Project-URL: Source Code, https://
 github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI Platform:
 UNKNOWN Classifier: Environment :: Console Classifier: Natural Language ::
 English Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
```

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric.egg-info/SOURCES.txt` & `lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1/src/lightning_fabric.egg-info/requires.txt` & `lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/requires.txt`

 * *Files identical despite different names*

