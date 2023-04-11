# Comparing `tmp/ml-starter-0.0.8.tar.gz` & `tmp/ml-starter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.8.tar", last modified: Sun Apr  9 00:07:51 2023, max compression
+gzip compressed data, was "ml-starter-0.0.9.tar", last modified: Sun Apr  9 00:50:31 2023, max compression
```

## Comparing `ml-starter-0.0.8.tar` & `ml-starter-0.0.9.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.707039 ml-starter-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-09 00:07:35.000000 ml-starter-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-09 00:07:51.707039 ml-starter-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-09 00:07:35.000000 ml-starter-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.683039 ml-starter-0.0.8/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/__version__.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.683039 ml-starter-0.0.8/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.683039 ml-starter-0.0.8/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.687039 ml-starter-0.0.8/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.687039 ml-starter-0.0.8/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.687039 ml-starter-0.0.8/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.691039 ml-starter-0.0.8/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.691039 ml-starter-0.0.8/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/scripts/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/scripts/mp_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.691039 ml-starter-0.0.8/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17584 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.695039 ml-starter-0.0.8/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.695039 ml-starter-0.0.8/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.695039 ml-starter-0.0.8/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.695039 ml-starter-0.0.8/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.695039 ml-starter-0.0.8/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.699039 ml-starter-0.0.8/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/ddp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.699039 ml-starter-0.0.8/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/cpu_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.699039 ml-starter-0.0.8/ml/trainers/mixins/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.703039 ml-starter-0.0.8/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-09 00:07:35.000000 ml-starter-0.0.8/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:07:51.707039 ml-starter-0.0.8/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-09 00:07:51.000000 ml-starter-0.0.8/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-09 00:07:51.000000 ml-starter-0.0.8/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 00:07:51.000000 ml-starter-0.0.8/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 00:07:51.000000 ml-starter-0.0.8/ml_starter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-09 00:07:51.000000 ml-starter-0.0.8/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-09 00:07:51.000000 ml-starter-0.0.8/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-09 00:07:35.000000 ml-starter-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-09 00:07:35.000000 ml-starter-0.0.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-09 00:07:35.000000 ml-starter-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-09 00:07:51.707039 ml-starter-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-09 00:07:35.000000 ml-starter-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.749144 ml-starter-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-09 00:50:21.000000 ml-starter-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-09 00:50:31.749144 ml-starter-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-09 00:50:21.000000 ml-starter-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.729144 ml-starter-0.0.9/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/__version__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.733144 ml-starter-0.0.9/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21416 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.733144 ml-starter-0.0.9/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.733144 ml-starter-0.0.9/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.733144 ml-starter-0.0.9/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.737144 ml-starter-0.0.9/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.737144 ml-starter-0.0.9/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.737144 ml-starter-0.0.9/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/scripts/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/scripts/mp_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.737144 ml-starter-0.0.9/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17584 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.741144 ml-starter-0.0.9/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.741144 ml-starter-0.0.9/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.741144 ml-starter-0.0.9/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.741144 ml-starter-0.0.9/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.741144 ml-starter-0.0.9/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.741144 ml-starter-0.0.9/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/ddp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.745144 ml-starter-0.0.9/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/mixins/cpu_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.745144 ml-starter-0.0.9/ml/trainers/mixins/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/mixins/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/mixins/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/mixins/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/mixins/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/mixins/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/mixins/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.749144 ml-starter-0.0.9/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-09 00:50:21.000000 ml-starter-0.0.9/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:50:31.749144 ml-starter-0.0.9/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-09 00:50:31.000000 ml-starter-0.0.9/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-09 00:50:31.000000 ml-starter-0.0.9/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 00:50:31.000000 ml-starter-0.0.9/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 00:50:31.000000 ml-starter-0.0.9/ml_starter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-09 00:50:31.000000 ml-starter-0.0.9/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-09 00:50:31.000000 ml-starter-0.0.9/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-09 00:50:21.000000 ml-starter-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-09 00:50:21.000000 ml-starter-0.0.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-09 00:50:21.000000 ml-starter-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-09 00:50:31.749144 ml-starter-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-09 00:50:21.000000 ml-starter-0.0.9/setup.py
```

### Comparing `ml-starter-0.0.8/PKG-INFO` & `ml-starter-0.0.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: ml-starter
-Version: 0.0.8
-Summary: ML project template repository
-Home-page: https://github.com/codekansas/ml-starter
-Author: Benjamin Bolte
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # ML Starter
 
 This is the core code for my ML project template over [here](https://github.com/codekansas/ml-project-template).
 
 ## Installation
 
 ```bash
@@ -26,24 +11,24 @@
 This expects a project structure like this:
 
 ```bash
 .
 ├── configs
 │   └── my_config.yaml
 ├── project
-│   ├── loggers
-│   ├── lr_schedulers
-│   ├── models
-│   │   └── my_model.py
-│   ├── optimizers
-│   ├── scripts
-│   │   └── cli.py
-│   ├── tasks
-│   │   └── my_task.py
-│   └── trainers
+    ├── loggers
+    ├── lr_schedulers
+    ├── models
+    │   └── my_model.py
+    ├── optimizers
+    ├── scripts
+    │   └── cli.py
+    ├── tasks
+    │   └── my_task.py
+    └── trainers
 ```
 
 The `cli.py` file should look something like this:
 
 ```python
 from pathlib import Path
 
@@ -62,8 +47,17 @@
 
 You can then train a model for your config using this command:
 
 ```bash
 python -m project.scripts.cli train configs/my_config.yaml
 ```
 
-See the template repository for more details.
+This can be made more wieldy by adding it as an entry point to your `setup.cfg` file:
+
+```
+[options.entry_points]
+
+console_scripts =
+    runml = project.scripts.cli:cli_main
+```
+
+The template repository above already does this.
```

### Comparing `ml-starter-0.0.8/ml/api.py` & `ml-starter-0.0.9/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/core/config.py` & `ml-starter-0.0.9/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/core/env.py` & `ml-starter-0.0.9/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/core/registry.py` & `ml-starter-0.0.9/ml/core/registry.py`

 * *Files identical despite different names*

```diff
@@ -88,15 +88,15 @@
     @classmethod
     @abstractmethod
     def config_key(cls) -> str:
         """Returns the key for the current item from the config."""
 
     @classmethod
     def registry_path(cls) -> Path:
-        return Path(__file__).parent.resolve() / ".cache" / f"{cls.config_key()}.json"
+        return (get_project_root() or Path(__file__).parent.resolve()) / ".cache" / f"{cls.config_key()}.json"
 
     @classmethod
     @functools.lru_cache(None)
     def load_registry_locations(cls) -> None:
         registry_path = cls.registry_path()
         if not registry_path.exists():
             return
```

### Comparing `ml-starter-0.0.8/ml/core/state.py` & `ml-starter-0.0.9/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/loggers/base.py` & `ml-starter-0.0.9/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/loggers/meter.py` & `ml-starter-0.0.9/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/loggers/multi.py` & `ml-starter-0.0.9/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/loggers/stdout.py` & `ml-starter-0.0.9/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/loggers/tensorboard.py` & `ml-starter-0.0.9/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/lr_schedulers/base.py` & `ml-starter-0.0.9/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.9/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.9/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/lr_schedulers/linear.py` & `ml-starter-0.0.9/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.9/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.9/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/models/activations.py` & `ml-starter-0.0.9/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/models/base.py` & `ml-starter-0.0.9/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/models/embeddings.py` & `ml-starter-0.0.9/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/models/init.py` & `ml-starter-0.0.9/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/models/norms.py` & `ml-starter-0.0.9/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/optimizers/adam.py` & `ml-starter-0.0.9/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/optimizers/adamw.py` & `ml-starter-0.0.9/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/optimizers/adan.py` & `ml-starter-0.0.9/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/optimizers/base.py` & `ml-starter-0.0.9/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/optimizers/sgd.py` & `ml-starter-0.0.9/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/optimizers/shampoo.py` & `ml-starter-0.0.9/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/scripts/cli.py` & `ml-starter-0.0.9/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/scripts/compiler.py` & `ml-starter-0.0.9/ml/scripts/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/scripts/stage.py` & `ml-starter-0.0.9/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/scripts/train.py` & `ml-starter-0.0.9/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/base.py` & `ml-starter-0.0.9/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.9/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.9/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/datasets/collate.py` & `ml-starter-0.0.9/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.9/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.9/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.9/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.9/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.9/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/datasets/utils.py` & `ml-starter-0.0.9/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.9/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/environments/base.py` & `ml-starter-0.0.9/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/environments/utils.py` & `ml-starter-0.0.9/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/environments/worker.py` & `ml-starter-0.0.9/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/losses/reduce.py` & `ml-starter-0.0.9/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/rl/base.py` & `ml-starter-0.0.9/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/rl/replay.py` & `ml-starter-0.0.9/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/tasks/sl/base.py` & `ml-starter-0.0.9/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/base.py` & `ml-starter-0.0.9/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/ddp.py` & `ml-starter-0.0.9/ml/trainers/ddp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.9/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/mixins/device/auto.py` & `ml-starter-0.0.9/ml/trainers/mixins/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/mixins/device/base.py` & `ml-starter-0.0.9/ml/trainers/mixins/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/mixins/device/cpu.py` & `ml-starter-0.0.9/ml/trainers/mixins/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/mixins/device/gpu.py` & `ml-starter-0.0.9/ml/trainers/mixins/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/mixins/device/metal.py` & `ml-starter-0.0.9/ml/trainers/mixins/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.9/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.9/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.9/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.9/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.9/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/rl.py` & `ml-starter-0.0.9/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/sl.py` & `ml-starter-0.0.9/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/slurm.py` & `ml-starter-0.0.9/ml/trainers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/trainers/vanilla.py` & `ml-starter-0.0.9/ml/trainers/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/argparse.py` & `ml-starter-0.0.9/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/atomic.py` & `ml-starter-0.0.9/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/augmentation.py` & `ml-starter-0.0.9/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/caching.py` & `ml-starter-0.0.9/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/call_train.py` & `ml-starter-0.0.9/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/cli.py` & `ml-starter-0.0.9/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/colors.py` & `ml-starter-0.0.9/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/compiler.py` & `ml-starter-0.0.9/ml/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/data.py` & `ml-starter-0.0.9/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/datetime.py` & `ml-starter-0.0.9/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/distributed.py` & `ml-starter-0.0.9/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/io.py` & `ml-starter-0.0.9/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/large_models.py` & `ml-starter-0.0.9/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/logging.py` & `ml-starter-0.0.9/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/meter.py` & `ml-starter-0.0.9/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/staging.py` & `ml-starter-0.0.9/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/timer.py` & `ml-starter-0.0.9/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml/utils/video.py` & `ml-starter-0.0.9/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.9/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/pyproject.toml` & `ml-starter-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.8/setup.py` & `ml-starter-0.0.9/setup.py`

 * *Files identical despite different names*

