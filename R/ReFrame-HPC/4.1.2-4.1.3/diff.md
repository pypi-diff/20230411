# Comparing `tmp/ReFrame-HPC-4.1.2.tar.gz` & `tmp/ReFrame-HPC-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReFrame-HPC-4.1.2.tar", last modified: Sun Apr  2 19:25:07 2023, max compression
+gzip compressed data, was "ReFrame-HPC-4.1.3.tar", last modified: Tue Apr 11 19:55:47 2023, max compression
```

## Comparing `ReFrame-HPC-4.1.2.tar` & `ReFrame-HPC-4.1.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:25:07.889562 ReFrame-HPC-4.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-02 19:25:07.889562 ReFrame-HPC-4.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/README_minimal.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:25:07.877562 ReFrame-HPC-4.1.2/ReFrame_HPC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-02 19:25:07.000000 ReFrame-HPC-4.1.2/ReFrame_HPC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-02 19:25:07.000000 ReFrame-HPC-4.1.2/ReFrame_HPC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 19:25:07.000000 ReFrame-HPC-4.1.2/ReFrame_HPC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-02 19:25:07.000000 ReFrame-HPC-4.1.2/ReFrame_HPC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-02 19:25:07.000000 ReFrame-HPC-4.1.2/ReFrame_HPC.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:25:07.877562 ReFrame-HPC-4.1.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/bin/reframe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:25:07.877562 ReFrame-HPC-4.1.2/reframe/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:25:07.881562 ReFrame-HPC-4.1.2/reframe/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    31089 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/buildsystems.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23075 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/deferrable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    44510 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:25:07.881562 ReFrame-HPC-4.1.2/reframe/core/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/launchers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/launchers/mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/launchers/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)    32216 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    35258 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    37547 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    93588 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:25:07.881562 ReFrame-HPC-4.1.2/reframe/core/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/schedulers/flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/schedulers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/schedulers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/schedulers/oar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/schedulers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/schedulers/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/schedulers/sge.py
--rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/schedulers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    22673 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/core/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:25:07.885563 ReFrame-HPC-4.1.2/reframe/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/frontend/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/frontend/autodetect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/frontend/ci.py
--rw-r--r--   0 runner    (1001) docker     (123)    54049 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/frontend/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/frontend/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:25:07.885563 ReFrame-HPC-4.1.2/reframe/frontend/executors/
--rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/frontend/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22001 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/frontend/executors/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/frontend/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/frontend/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/frontend/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/frontend/runreport.py
--rw-r--r--   0 runner    (1001) docker     (123)    15952 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/frontend/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/frontend/testgenerators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:25:07.885563 ReFrame-HPC-4.1.2/reframe/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    25779 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/schemas/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/schemas/junit.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/schemas/runreport.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 19:25:07.889562 ReFrame-HPC-4.1.2/reframe/utility/
--rw-r--r--   0 runner    (1001) docker     (123)    47416 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/utility/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/utility/cpuinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/utility/jsonext.py
--rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/utility/osext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/utility/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/utility/sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/utility/typecheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/utility/udeps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-02 19:24:56.000000 ReFrame-HPC-4.1.2/reframe/utility/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-02 19:25:07.889562 ReFrame-HPC-4.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.108786 ReFrame-HPC-4.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-11 19:55:47.108786 ReFrame-HPC-4.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/README_minimal.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.096786 ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-11 19:55:47.000000 ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-11 19:55:47.000000 ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:55:47.000000 ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-11 19:55:47.000000 ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 19:55:47.000000 ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.096786 ReFrame-HPC-4.1.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/bin/reframe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.096786 ReFrame-HPC-4.1.3/reframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.100786 ReFrame-HPC-4.1.3/reframe/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31089 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/buildsystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23075 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/deferrable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44510 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.100786 ReFrame-HPC-4.1.3/reframe/core/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/launchers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/launchers/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/launchers/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32228 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35258 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37547 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93588 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.104786 ReFrame-HPC-4.1.3/reframe/core/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/oar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22673 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.104786 ReFrame-HPC-4.1.3/reframe/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/autodetect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54049 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.104786 ReFrame-HPC-4.1.3/reframe/frontend/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22001 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/executors/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/runreport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15952 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/testgenerators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.104786 ReFrame-HPC-4.1.3/reframe/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    25779 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/schemas/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/schemas/junit.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/schemas/runreport.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.108786 ReFrame-HPC-4.1.3/reframe/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)    47416 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/cpuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/jsonext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/osext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/udeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-11 19:55:47.108786 ReFrame-HPC-4.1.3/setup.cfg
```

### Comparing `ReFrame-HPC-4.1.2/LICENSE` & `ReFrame-HPC-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/PKG-INFO` & `ReFrame-HPC-4.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.1.2
+Version: 4.1.3
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ReFrame-HPC-4.1.2/README.md` & `ReFrame-HPC-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/README_minimal.md` & `ReFrame-HPC-4.1.3/README_minimal.md`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/ReFrame_HPC.egg-info/PKG-INFO` & `ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.1.2
+Version: 4.1.3
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ReFrame-HPC-4.1.2/ReFrame_HPC.egg-info/SOURCES.txt` & `ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/bin/reframe` & `ReFrame-HPC-4.1.3/bin/reframe`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/__init__.py` & `ReFrame-HPC-4.1.3/reframe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # ReFrame Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import os
 import sys
 
-VERSION = '4.1.2'
+VERSION = '4.1.3'
 INSTALL_PREFIX = os.path.normpath(
     os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 )
 MIN_PYTHON_VERSION = (3, 6, 0)
 
 # Check python version
 if sys.version_info[:3] < MIN_PYTHON_VERSION:
```

### Comparing `ReFrame-HPC-4.1.2/reframe/core/backends.py` & `ReFrame-HPC-4.1.3/reframe/core/backends.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/buildsystems.py` & `ReFrame-HPC-4.1.3/reframe/core/buildsystems.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/builtins.py` & `ReFrame-HPC-4.1.3/reframe/core/builtins.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/config.py` & `ReFrame-HPC-4.1.3/reframe/core/config.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/containers.py` & `ReFrame-HPC-4.1.3/reframe/core/containers.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/decorators.py` & `ReFrame-HPC-4.1.3/reframe/core/decorators.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/deferrable.py` & `ReFrame-HPC-4.1.3/reframe/core/deferrable.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/environments.py` & `ReFrame-HPC-4.1.3/reframe/core/environments.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/exceptions.py` & `ReFrame-HPC-4.1.3/reframe/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/fields.py` & `ReFrame-HPC-4.1.3/reframe/core/fields.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/fixtures.py` & `ReFrame-HPC-4.1.3/reframe/core/fixtures.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/hooks.py` & `ReFrame-HPC-4.1.3/reframe/core/hooks.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/launchers/__init__.py` & `ReFrame-HPC-4.1.3/reframe/core/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/launchers/local.py` & `ReFrame-HPC-4.1.3/reframe/core/launchers/local.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/launchers/mpi.py` & `ReFrame-HPC-4.1.3/reframe/core/launchers/mpi.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/launchers/ssh.py` & `ReFrame-HPC-4.1.3/reframe/core/launchers/ssh.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/logging.py` & `ReFrame-HPC-4.1.3/reframe/core/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,16 +276,16 @@
         for var, info in perfvars.items():
             val, ref, lower, upper, unit = info
             record = {
                 'check_perf_var': var.split(':')[-1],
                 'check_perf_value': val,
                 'check_perf_unit': unit,
                 'check_perf_ref': ref,
-                'check_perf_lower': lower,
-                'check_perf_upper': upper
+                'check_perf_lower_thres': lower,
+                'check_perf_upper_thres': upper
             }
             try:
                 chunks.append(self.__fmtperf % record)
             except ValueError:
                 chunks.append("<error formatting the performance record: "
                               "please check the 'format_perfvars' string>")
```

### Comparing `ReFrame-HPC-4.1.2/reframe/core/meta.py` & `ReFrame-HPC-4.1.3/reframe/core/meta.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/modules.py` & `ReFrame-HPC-4.1.3/reframe/core/modules.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/namespaces.py` & `ReFrame-HPC-4.1.3/reframe/core/namespaces.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/parameters.py` & `ReFrame-HPC-4.1.3/reframe/core/parameters.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/pipeline.py` & `ReFrame-HPC-4.1.3/reframe/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/runtime.py` & `ReFrame-HPC-4.1.3/reframe/core/runtime.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/schedulers/__init__.py` & `ReFrame-HPC-4.1.3/reframe/core/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/schedulers/flux.py` & `ReFrame-HPC-4.1.3/reframe/core/schedulers/flux.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/schedulers/local.py` & `ReFrame-HPC-4.1.3/reframe/core/schedulers/local.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/schedulers/lsf.py` & `ReFrame-HPC-4.1.3/reframe/core/schedulers/lsf.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/schedulers/oar.py` & `ReFrame-HPC-4.1.3/reframe/core/schedulers/oar.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/schedulers/pbs.py` & `ReFrame-HPC-4.1.3/reframe/core/schedulers/pbs.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/schedulers/registry.py` & `ReFrame-HPC-4.1.3/reframe/core/schedulers/registry.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/schedulers/sge.py` & `ReFrame-HPC-4.1.3/reframe/core/schedulers/sge.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/schedulers/slurm.py` & `ReFrame-HPC-4.1.3/reframe/core/schedulers/slurm.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/settings.py` & `ReFrame-HPC-4.1.3/reframe/core/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,16 +58,16 @@
                         '%(check_job_completion_time)s,%(version)s,'
                         '%(check_display_name)s,%(check_system)s,'
                         '%(check_partition)s,%(check_environ)s,'
                         '%(check_jobid)s,%(check_result)s,%(check_perfvalues)s'
                     ),
                     'format_perfvars': (
                         '%(check_perf_value)s,%(check_perf_unit)s,'
-                        '%(check_perf_ref)s,%(check_perf_lower)s,'
-                        '%(check_perf_upper)s,'
+                        '%(check_perf_ref)s,%(check_perf_lower_thres)s,'
+                        '%(check_perf_upper_thres)s,'
                     ),
                     'append': True
                 }
             ]
         }
     ]   # end of logging
 }
```

### Comparing `ReFrame-HPC-4.1.2/reframe/core/shell.py` & `ReFrame-HPC-4.1.3/reframe/core/shell.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/systems.py` & `ReFrame-HPC-4.1.3/reframe/core/systems.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/variables.py` & `ReFrame-HPC-4.1.3/reframe/core/variables.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/core/warnings.py` & `ReFrame-HPC-4.1.3/reframe/core/warnings.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/frontend/argparse.py` & `ReFrame-HPC-4.1.3/reframe/frontend/argparse.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/frontend/autodetect.py` & `ReFrame-HPC-4.1.3/reframe/frontend/autodetect.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/frontend/ci.py` & `ReFrame-HPC-4.1.3/reframe/frontend/ci.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             f'--prefix={prefix}', config_opt,
             f'{" ".join("-c " + c for c in checkpath)}',
             f'-R' if recurse else '',
             f'--report-file={report_file}',
             f'--restore-session={restore_files}' if restore_files else '',
             f'--report-junit={testcase.check.unique_name}-report.xml',
             f'{"".join("-" + verbosity)}' if verbosity else '',
-            '-n', f"'^{testcase.check.unique_name}$'", '-r',
+            '-n', f'/{testcase.check.hashcode}', '-r',
             *child_pipeline_opts
         ])
 
     max_level = 0   # We need the maximum level to generate the stages section
     json = {
         'cache': {
             'key': '${CI_COMMIT_REF_SLUG}',
```

### Comparing `ReFrame-HPC-4.1.2/reframe/frontend/cli.py` & `ReFrame-HPC-4.1.3/reframe/frontend/cli.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/frontend/dependencies.py` & `ReFrame-HPC-4.1.3/reframe/frontend/dependencies.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/frontend/executors/__init__.py` & `ReFrame-HPC-4.1.3/reframe/frontend/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/frontend/executors/policies.py` & `ReFrame-HPC-4.1.3/reframe/frontend/executors/policies.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/frontend/filters.py` & `ReFrame-HPC-4.1.3/reframe/frontend/filters.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/frontend/loader.py` & `ReFrame-HPC-4.1.3/reframe/frontend/loader.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/frontend/printer.py` & `ReFrame-HPC-4.1.3/reframe/frontend/printer.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/frontend/runreport.py` & `ReFrame-HPC-4.1.3/reframe/frontend/runreport.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/frontend/statistics.py` & `ReFrame-HPC-4.1.3/reframe/frontend/statistics.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/frontend/testgenerators.py` & `ReFrame-HPC-4.1.3/reframe/frontend/testgenerators.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/schemas/config.json` & `ReFrame-HPC-4.1.3/reframe/schemas/config.json`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/schemas/junit.xsd` & `ReFrame-HPC-4.1.3/reframe/schemas/junit.xsd`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/schemas/runreport.json` & `ReFrame-HPC-4.1.3/reframe/schemas/runreport.json`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/utility/__init__.py` & `ReFrame-HPC-4.1.3/reframe/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/utility/color.py` & `ReFrame-HPC-4.1.3/reframe/utility/color.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/utility/cpuinfo.py` & `ReFrame-HPC-4.1.3/reframe/utility/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/utility/jsonext.py` & `ReFrame-HPC-4.1.3/reframe/utility/jsonext.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/utility/osext.py` & `ReFrame-HPC-4.1.3/reframe/utility/osext.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/utility/profile.py` & `ReFrame-HPC-4.1.3/reframe/utility/profile.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/utility/sanity.py` & `ReFrame-HPC-4.1.3/reframe/utility/sanity.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/utility/typecheck.py` & `ReFrame-HPC-4.1.3/reframe/utility/typecheck.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/utility/udeps.py` & `ReFrame-HPC-4.1.3/reframe/utility/udeps.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/reframe/utility/versioning.py` & `ReFrame-HPC-4.1.3/reframe/utility/versioning.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.2/setup.cfg` & `ReFrame-HPC-4.1.3/setup.cfg`

 * *Files identical despite different names*

