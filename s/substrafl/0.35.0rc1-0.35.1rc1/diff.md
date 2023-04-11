# Comparing `tmp/substrafl-0.35.0rc1.tar.gz` & `tmp/substrafl-0.35.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrafl-0.35.0rc1.tar", last modified: Fri Mar 31 09:17:09 2023, max compression
+gzip compressed data, was "substrafl-0.35.1rc1.tar", last modified: Tue Apr 11 14:52:27 2023, max compression
```

## Comparing `substrafl-0.35.0rc1.tar` & `substrafl-0.35.1rc1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:17:09.006435 substrafl-0.35.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-31 09:17:09.006435 substrafl-0.35.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 09:17:09.006435 substrafl-0.35.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:17:09.002435 substrafl-0.35.0rc1/substrafl/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:17:09.002435 substrafl-0.35.0rc1/substrafl/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/algorithms/algo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:17:09.002435 substrafl-0.35.0rc1/substrafl/algorithms/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/algorithms/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15386 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18027 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    23421 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/algorithms/pytorch/weight_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/evaluation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14468 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:17:09.002435 substrafl-0.35.0rc1/substrafl/index_generator/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/index_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/index_generator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/index_generator/np_index_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/model_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:17:09.002435 substrafl-0.35.0rc1/substrafl/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/nodes/aggregation_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/nodes/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:17:09.006435 substrafl-0.35.0rc1/substrafl/nodes/references/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/nodes/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/nodes/references/local_state.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/nodes/references/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/nodes/test_data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/nodes/train_data_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:17:09.006435 substrafl-0.35.0rc1/substrafl/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/remote/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/remote/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:17:09.006435 substrafl-0.35.0rc1/substrafl/remote/register/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/remote/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/remote/register/generate_wheel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/remote/register/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/remote/remote_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:17:09.006435 substrafl-0.35.0rc1/substrafl/remote/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/remote/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/remote/serializers/pickle_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/remote/serializers/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/remote/substratools_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:17:09.006435 substrafl-0.35.0rc1/substrafl/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12031 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/strategies/fed_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14974 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/strategies/newton_raphson.py
--rw-r--r--   0 runner    (1001) docker     (123)    17681 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/strategies/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/strategies/single_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-03-31 09:17:06.000000 substrafl-0.35.0rc1/substrafl/strategies/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 09:17:09.002435 substrafl-0.35.0rc1/substrafl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-31 09:17:08.000000 substrafl-0.35.0rc1/substrafl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-31 09:17:08.000000 substrafl-0.35.0rc1/substrafl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 09:17:08.000000 substrafl-0.35.0rc1/substrafl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-31 09:17:08.000000 substrafl-0.35.0rc1/substrafl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-31 09:17:08.000000 substrafl-0.35.0rc1/substrafl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.050597 substrafl-0.35.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-11 14:52:27.050597 substrafl-0.35.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 14:52:27.050597 substrafl-0.35.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.042597 substrafl-0.35.1rc1/substrafl/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.042597 substrafl-0.35.1rc1/substrafl/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/algo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.046597 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15386 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_base_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18027 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23421 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/weight_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/evaluation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14468 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.046597 substrafl-0.35.1rc1/substrafl/index_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/index_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/index_generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/index_generator/np_index_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/model_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.046597 substrafl-0.35.1rc1/substrafl/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/aggregation_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.046597 substrafl-0.35.1rc1/substrafl/nodes/references/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/references/local_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/references/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/test_data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/train_data_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.050597 substrafl-0.35.1rc1/substrafl/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.050597 substrafl-0.35.1rc1/substrafl/remote/register/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/register/generate_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/register/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/remote_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.050597 substrafl-0.35.1rc1/substrafl/remote/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/serializers/pickle_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/serializers/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/substratools_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.050597 substrafl-0.35.1rc1/substrafl/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12031 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/strategies/fed_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14974 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/strategies/newton_raphson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17681 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/strategies/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/strategies/single_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/strategies/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.042597 substrafl-0.35.1rc1/substrafl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-11 14:52:26.000000 substrafl-0.35.1rc1/substrafl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-11 14:52:27.000000 substrafl-0.35.1rc1/substrafl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:52:26.000000 substrafl-0.35.1rc1/substrafl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-11 14:52:26.000000 substrafl-0.35.1rc1/substrafl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 14:52:26.000000 substrafl-0.35.1rc1/substrafl.egg-info/top_level.txt
```

### Comparing `substrafl-0.35.0rc1/LICENSE` & `substrafl-0.35.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/PKG-INFO` & `substrafl-0.35.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrafl
-Version: 0.35.0rc1
+Version: 0.35.1rc1
 Summary: A high-level federated learning Python library to run      federated learning experiments at scale on a Substra network
 Home-page: https://docs.substra.org/
 Author: Owkin, Inc.
 License: Apache 2.0
 Description: readme
 Keywords: substrafl
 Platform: UNKNOWN
```

### Comparing `substrafl-0.35.0rc1/README.md` & `substrafl-0.35.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/pyproject.toml` & `substrafl-0.35.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/setup.py` & `substrafl-0.35.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     packages=find_packages(exclude=["tests*", "benchmark*"]),
     # Not compatible with substratools 0.8.0 because
     # that release is private and in the Docker container
     # it has access only to the public PyPi
     install_requires=[
         "numpy>=1.20.3,!=1.24.*",
         "cloudpickle>=1.6.0",
-        "substra~=0.43.0rc1",
+        "substra~=0.43.0",
         "substratools~=0.20.0",
         "pydantic>=1.9.0",
         "pip>=21.2",
         "wheel",
         "six",
         "packaging",
     ],
```

### Comparing `substrafl-0.35.0rc1/substrafl/__init__.py` & `substrafl-0.35.1rc1/substrafl/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/algorithms/algo.py` & `substrafl-0.35.1rc1/substrafl/algorithms/algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/algorithms/pytorch/__init__.py` & `substrafl-0.35.1rc1/substrafl/algorithms/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py` & `substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_base_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py` & `substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py` & `substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py` & `substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py` & `substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/algorithms/pytorch/weight_manager.py` & `substrafl-0.35.1rc1/substrafl/algorithms/pytorch/weight_manager.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/dependency.py` & `substrafl-0.35.1rc1/substrafl/dependency.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/evaluation_strategy.py` & `substrafl-0.35.1rc1/substrafl/evaluation_strategy.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/exceptions.py` & `substrafl-0.35.1rc1/substrafl/exceptions.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/experiment.py` & `substrafl-0.35.1rc1/substrafl/experiment.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/index_generator/base.py` & `substrafl-0.35.1rc1/substrafl/index_generator/base.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/index_generator/np_index_generator.py` & `substrafl-0.35.1rc1/substrafl/index_generator/np_index_generator.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/logger.py` & `substrafl-0.35.1rc1/substrafl/logger.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/model_loading.py` & `substrafl-0.35.1rc1/substrafl/model_loading.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/nodes/__init__.py` & `substrafl-0.35.1rc1/substrafl/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/nodes/aggregation_node.py` & `substrafl-0.35.1rc1/substrafl/nodes/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/nodes/node.py` & `substrafl-0.35.1rc1/substrafl/nodes/node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/nodes/test_data_node.py` & `substrafl-0.35.1rc1/substrafl/nodes/test_data_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/nodes/train_data_node.py` & `substrafl-0.35.1rc1/substrafl/nodes/train_data_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/remote/decorators.py` & `substrafl-0.35.1rc1/substrafl/remote/decorators.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/remote/operations.py` & `substrafl-0.35.1rc1/substrafl/remote/operations.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/remote/register/generate_wheel.py` & `substrafl-0.35.1rc1/substrafl/remote/register/generate_wheel.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,15 +79,16 @@
             )
 
         shutil.copy(wheel_path, wheels_dir / wheel_name)
 
         # Necessary command to install the wheel in the docker image
         force_reinstall = "--force-reinstall " if lib_name in ["substratools", "substra"] else ""
         install_cmd = (
-            f"RUN cd {dest_dir} && python{python_major_minor}" f" -m pip install {force_reinstall}{wheel_name}\n"
+            f"COPY {dest_dir}/{wheel_name} . \n"
+            + f"RUN python{python_major_minor} -m pip install {force_reinstall}{wheel_name}\n"
         )
         install_cmds.append(install_cmd)
 
     return "\n".join(install_cmds)
 
 
 def pypi_lib_wheels(lib_modules: List, operation_dir: Path, python_major_minor: str, dest_dir: str) -> str:
@@ -131,11 +132,11 @@
                     LOCAL_WHEELS_FOLDER,
                     f"{lib_module.__name__}=={lib_module.__version__}",
                 ]
             )
 
         # Get wheel name based on current version
         shutil.copy(LOCAL_WHEELS_FOLDER / wheel_name, wheels_dir / wheel_name)
-        install_cmd = f"RUN cd {dest_dir} && python{python_major_minor} -m pip install {wheel_name}\n"
+        install_cmd = f"COPY {dest_dir}/{wheel_name} . \n RUN python{python_major_minor} -m pip install {wheel_name}\n"
         install_cmds.append(install_cmd)
 
     return "\n".join(install_cmds)
```

### Comparing `substrafl-0.35.0rc1/substrafl/remote/register/register.py` & `substrafl-0.35.1rc1/substrafl/remote/register/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,29 +38,30 @@
 {substratools_version}-nvidiacuda11.8.0-base-ubuntu22.04-python{python_version}"
 
 SUBSTRAFL_FOLDER = "substrafl_internal"
 
 DOCKERFILE_TEMPLATE = """
 FROM {docker_image}
 
-COPY . .
-
 # install dependencies
 RUN python{python_version} -m pip install -U pip
 
 # Install substrafl, substra (and substratools if editable mode)
 {cl_deps}
 
 # PyPi dependencies
 {pypi_dependencies}
 
 # Install local dependencies
 {local_dependencies}
 
 ENTRYPOINT ["python{python_version}", "function.py", "--function-name", "{method_name}"]
+
+COPY . .
+
 """
 
 FUNCTION = """
 import json
 import cloudpickle
 
 import substratools as tools
@@ -84,15 +85,15 @@
 """
 
 
 def _copy_local_packages(
     path: Path, local_dependencies: typing.List[Path], python_major_minor: str, operation_dir: Path
 ):
     """Copy the local libraries given by the user and generate the installation command."""
-    dependencies_buffer = list()
+    dependencies_buffer = []
     path.mkdir(exist_ok=True)
     for dependency_path in local_dependencies:
         dest_path = path / dependency_path.name
         if dependency_path.is_dir():
             shutil.copytree(
                 dependency_path,
                 dest_path,
@@ -104,19 +105,22 @@
         elif dependency_path.is_file():
             shutil.copy(dependency_path, dest_path)
         else:
             raise ValueError(f"Does not exist {dependency_path}")
 
         dependencies_buffer.append(f"{dest_path.relative_to(operation_dir)}")
 
-    local_dependencies_cmd = (
-        f"RUN python{python_major_minor} -m pip install --no-cache-dir " + " ".join(dependencies_buffer)
-        if len(local_dependencies) > 0
-        else ""
+    local_dependencies_cmd = "\n".join(
+        [
+            f"COPY {dependency}  {dependency} \n"
+            + f"RUN python{python_major_minor} -m pip install --no-cache-dir {dependency} \n"
+            for dependency in dependencies_buffer
+        ]
     )
+
     return local_dependencies_cmd
 
 
 def _copy_local_code(path: Path, operation_dir: Path):
     """Copy the local code given by the user to the operation directory."""
     if path.is_dir():
         shutil.copytree(path, operation_dir / path.name)
```

### Comparing `substrafl-0.35.0rc1/substrafl/remote/remote_struct.py` & `substrafl-0.35.1rc1/substrafl/remote/remote_struct.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/remote/serializers/pickle_serializer.py` & `substrafl-0.35.1rc1/substrafl/remote/serializers/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/remote/substratools_methods.py` & `substrafl-0.35.1rc1/substrafl/remote/substratools_methods.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/schemas.py` & `substrafl-0.35.1rc1/substrafl/schemas.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/strategies/fed_avg.py` & `substrafl-0.35.1rc1/substrafl/strategies/fed_avg.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/strategies/newton_raphson.py` & `substrafl-0.35.1rc1/substrafl/strategies/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/strategies/scaffold.py` & `substrafl-0.35.1rc1/substrafl/strategies/scaffold.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/strategies/single_organization.py` & `substrafl-0.35.1rc1/substrafl/strategies/single_organization.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl/strategies/strategy.py` & `substrafl-0.35.1rc1/substrafl/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.0rc1/substrafl.egg-info/PKG-INFO` & `substrafl-0.35.1rc1/substrafl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrafl
-Version: 0.35.0rc1
+Version: 0.35.1rc1
 Summary: A high-level federated learning Python library to run      federated learning experiments at scale on a Substra network
 Home-page: https://docs.substra.org/
 Author: Owkin, Inc.
 License: Apache 2.0
 Description: readme
 Keywords: substrafl
 Platform: UNKNOWN
```

### Comparing `substrafl-0.35.0rc1/substrafl.egg-info/SOURCES.txt` & `substrafl-0.35.1rc1/substrafl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

