# Comparing `tmp/frinx-python-sdk-0.0.7.tar.gz` & `tmp/frinx-python-sdk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frinx-python-sdk-0.0.7.tar", last modified: Wed Apr  5 08:03:27 2023, max compression
+gzip compressed data, was "frinx-python-sdk-0.0.8.tar", last modified: Tue Apr 11 09:27:55 2023, max compression
```

## Comparing `frinx-python-sdk-0.0.7.tar` & `frinx-python-sdk-0.0.8.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.256883 frinx-python-sdk-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-05 08:03:27.256883 frinx-python-sdk-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 08:03:27.256883 frinx-python-sdk-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.248883 frinx-python-sdk-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.248883 frinx-python-sdk-0.0.7/src/frinx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.248883 frinx-python-sdk-0.0.7/src/frinx/client/
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/client/ConductorWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/client/FrinxConductorWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/client/conductor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.248883 frinx-python-sdk-0.0.7/src/frinx/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/conductor_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/frinx_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/import_workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.248883 frinx-python-sdk-0.0.7/src/frinx/common/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/logging/logging-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/logging/logging_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.252883 frinx-python-sdk-0.0.7/src/frinx/common/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/worker/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/worker/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/worker/task_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/worker/task_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.252883 frinx-python-sdk-0.0.7/src/frinx/common/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/workflow/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    17783 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/workflow/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/common/workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.252883 frinx-python-sdk-0.0.7/src/frinx/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.252883 frinx-python-sdk-0.0.7/src/frinx/services/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/http/http_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.252883 frinx-python-sdk-0.0.7/src/frinx/services/inventory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17102 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/inventory/inventory_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/inventory/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/inventory/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.252883 frinx-python-sdk-0.0.7/src/frinx/services/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/monitoring/influxdb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/monitoring/influxdb_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/task_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.252883 frinx-python-sdk-0.0.7/src/frinx/services/uniconfig/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/uniconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/uniconfig/cli_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/uniconfig/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/uniconfig/netconf_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/uniconfig/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    19269 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/uniconfig/uniconfig_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/services/uniconfig/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.252883 frinx-python-sdk-0.0.7/src/frinx/workers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.252883 frinx-python-sdk-0.0.7/src/frinx/workers/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workers/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workers/http/http_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.252883 frinx-python-sdk-0.0.7/src/frinx/workers/inventory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workers/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workers/inventory/inventory_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.252883 frinx-python-sdk-0.0.7/src/frinx/workers/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workers/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workers/monitoring/influxdb_workers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.256883 frinx-python-sdk-0.0.7/src/frinx/workers/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workers/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workers/test/test_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.256883 frinx-python-sdk-0.0.7/src/frinx/workers/uniconfig/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workers/uniconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workers/uniconfig/cli_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workers/uniconfig/netconf_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12557 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workers/uniconfig/uniconfig_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.256883 frinx-python-sdk-0.0.7/src/frinx/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.256883 frinx-python-sdk-0.0.7/src/frinx/workflows/inventory/
--rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workflows/inventory/inventory_workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.256883 frinx-python-sdk-0.0.7/src/frinx/workflows/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workflows/misc/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workflows/misc/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.256883 frinx-python-sdk-0.0.7/src/frinx/workflows/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workflows/monitoring/influxdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.256883 frinx-python-sdk-0.0.7/src/frinx/workflows/uniconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-05 08:03:16.000000 frinx-python-sdk-0.0.7/src/frinx/workflows/uniconfig/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:03:27.256883 frinx-python-sdk-0.0.7/src/frinx_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-05 08:03:27.000000 frinx-python-sdk-0.0.7/src/frinx_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-05 08:03:27.000000 frinx-python-sdk-0.0.7/src/frinx_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 08:03:27.000000 frinx-python-sdk-0.0.7/src/frinx_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-05 08:03:27.000000 frinx-python-sdk-0.0.7/src/frinx_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 08:03:27.000000 frinx-python-sdk-0.0.7/src/frinx_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.741463 frinx-python-sdk-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.741463 frinx-python-sdk-0.0.8/src/frinx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.741463 frinx-python-sdk-0.0.8/src/frinx/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/client/ConductorWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/client/FrinxConductorWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/client/conductor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.741463 frinx-python-sdk-0.0.8/src/frinx/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/conductor_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/frinx_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/import_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.741463 frinx-python-sdk-0.0.8/src/frinx/common/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/logging/logging-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/logging/logging_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.741463 frinx-python-sdk-0.0.8/src/frinx/common/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/worker/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/worker/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/worker/task_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/worker/task_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.741463 frinx-python-sdk-0.0.8/src/frinx/common/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/workflow/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17783 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/workflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/common/workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.741463 frinx-python-sdk-0.0.8/src/frinx/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.741463 frinx-python-sdk-0.0.8/src/frinx/services/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/http/http_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/src/frinx/services/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17102 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/inventory/inventory_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/inventory/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/inventory/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/src/frinx/services/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/monitoring/influxdb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/monitoring/influxdb_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/task_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/src/frinx/services/uniconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/uniconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/uniconfig/cli_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/uniconfig/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/uniconfig/netconf_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/uniconfig/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19269 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/uniconfig/uniconfig_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/services/uniconfig/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/src/frinx/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/src/frinx/workers/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workers/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workers/http/http_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/src/frinx/workers/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workers/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workers/inventory/inventory_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/src/frinx/workers/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workers/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workers/monitoring/influxdb_workers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/src/frinx/workers/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workers/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workers/test/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/src/frinx/workers/uniconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workers/uniconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workers/uniconfig/cli_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workers/uniconfig/netconf_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12557 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workers/uniconfig/uniconfig_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/src/frinx/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/src/frinx/workflows/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workflows/inventory/inventory_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/src/frinx/workflows/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workflows/misc/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workflows/misc/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/src/frinx/workflows/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workflows/monitoring/influxdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/src/frinx/workflows/uniconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-11 09:27:47.000000 frinx-python-sdk-0.0.8/src/frinx/workflows/uniconfig/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:27:55.745463 frinx-python-sdk-0.0.8/src/frinx_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-11 09:27:55.000000 frinx-python-sdk-0.0.8/src/frinx_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-11 09:27:55.000000 frinx-python-sdk-0.0.8/src/frinx_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:27:55.000000 frinx-python-sdk-0.0.8/src/frinx_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-11 09:27:55.000000 frinx-python-sdk-0.0.8/src/frinx_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 09:27:55.000000 frinx-python-sdk-0.0.8/src/frinx_python_sdk.egg-info/top_level.txt
```

### Comparing `frinx-python-sdk-0.0.7/setup.py` & `frinx-python-sdk-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """
     return open(os.path.join(os.path.dirname(__file__), file_name)).read()
 
 
 setup(
     name="frinx-python-sdk",
     package_dir={"": "src"},
-    version="0.0.7",
+    version="0.0.8",
     description="Python SDK for Frinx Machine Workflow Manager",
     data_files=[("logging", ["src/frinx/common/logging/logging-config.json"])],
     author="FRINXio",
     author_email="info@frinx.io",
     url="https://github.com/FRINXio/fm-base-workers",
     keywords=["frinx-machine", "conductor"],
     include_package_data=True,
```

### Comparing `frinx-python-sdk-0.0.7/src/frinx/client/ConductorWorker.py` & `frinx-python-sdk-0.0.8/src/frinx/client/ConductorWorker.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/client/FrinxConductorWrapper.py` & `frinx-python-sdk-0.0.8/src/frinx/client/FrinxConductorWrapper.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/client/conductor.py` & `frinx-python-sdk-0.0.8/src/frinx/client/conductor.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/common/conductor_enums.py` & `frinx-python-sdk-0.0.8/src/frinx/common/conductor_enums.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/common/frinx_rest.py` & `frinx-python-sdk-0.0.8/src/frinx/common/frinx_rest.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/common/import_workflows.py` & `frinx-python-sdk-0.0.8/src/frinx/common/import_workflows.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/common/logging/logging-config.json` & `frinx-python-sdk-0.0.8/src/frinx/common/logging/logging-config.json`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/common/logging/logging_common.py` & `frinx-python-sdk-0.0.8/src/frinx/common/logging/logging_common.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/common/util.py` & `frinx-python-sdk-0.0.8/src/frinx/common/util.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/common/worker/service.py` & `frinx-python-sdk-0.0.8/src/frinx/common/worker/service.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/common/worker/task.py` & `frinx-python-sdk-0.0.8/src/frinx/common/worker/task.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/common/worker/task_def.py` & `frinx-python-sdk-0.0.8/src/frinx/common/worker/task_def.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/common/worker/task_result.py` & `frinx-python-sdk-0.0.8/src/frinx/common/worker/task_result.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/common/worker/worker.py` & `frinx-python-sdk-0.0.8/src/frinx/common/worker/worker.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/common/workflow/service.py` & `frinx-python-sdk-0.0.8/src/frinx/common/workflow/service.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/common/workflow/task.py` & `frinx-python-sdk-0.0.8/src/frinx/common/workflow/task.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/common/workflow/workflow.py` & `frinx-python-sdk-0.0.8/src/frinx/common/workflow/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     rbac: Optional[List[object]] = Field(default=None)  # TODO why list[str] return error
 
     # PREDEFINED
     restartable: bool = Field(default=False)
     output_parameters: dict[str, object] = Field(default={})
     input_parameters: list[WorkflowInputField | str] = Field(default=[])
     tasks: list[WorkflowTaskImpl] = Field(default=[])
-    timeout_policy: TimeoutPolicy = Field(default=TimeoutPolicy.ALERT_ONLY)
+    timeout_policy: TimeoutPolicy = Field(default=TimeoutPolicy.TIME_OUT_WORKFLOW)
     timeout_seconds: int = Field(default=60)
 
     owner_app: str = Field(default=None)
     create_time: int = Field(default=None)
     update_time: int = Field(default=None)
     created_by: str = Field(default=None)
     updated_by: str = Field(default=None)
```

### Comparing `frinx-python-sdk-0.0.7/src/frinx/main.py` & `frinx-python-sdk-0.0.8/src/frinx/main.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/services/http/http_worker.py` & `frinx-python-sdk-0.0.8/src/frinx/services/http/http_worker.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/services/inventory/inventory_worker.py` & `frinx-python-sdk-0.0.8/src/frinx/services/inventory/inventory_worker.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/services/inventory/templates.py` & `frinx-python-sdk-0.0.8/src/frinx/services/inventory/templates.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/services/inventory/utils.py` & `frinx-python-sdk-0.0.8/src/frinx/services/inventory/utils.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/services/monitoring/influxdb_utils.py` & `frinx-python-sdk-0.0.8/src/frinx/services/monitoring/influxdb_utils.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/services/monitoring/influxdb_worker.py` & `frinx-python-sdk-0.0.8/src/frinx/services/monitoring/influxdb_worker.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/services/task_response.py` & `frinx-python-sdk-0.0.8/src/frinx/services/task_response.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/services/uniconfig/cli_worker.py` & `frinx-python-sdk-0.0.8/src/frinx/services/uniconfig/cli_worker.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/services/uniconfig/models.py` & `frinx-python-sdk-0.0.8/src/frinx/services/uniconfig/models.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/services/uniconfig/netconf_worker.py` & `frinx-python-sdk-0.0.8/src/frinx/services/uniconfig/netconf_worker.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/services/uniconfig/templates.py` & `frinx-python-sdk-0.0.8/src/frinx/services/uniconfig/templates.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/services/uniconfig/uniconfig_worker.py` & `frinx-python-sdk-0.0.8/src/frinx/services/uniconfig/uniconfig_worker.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/services/uniconfig/utils.py` & `frinx-python-sdk-0.0.8/src/frinx/services/uniconfig/utils.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/workers/http/http_worker.py` & `frinx-python-sdk-0.0.8/src/frinx/workers/http/http_worker.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/workers/inventory/inventory_worker.py` & `frinx-python-sdk-0.0.8/src/frinx/workers/inventory/inventory_worker.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/workers/monitoring/influxdb_workers.py` & `frinx-python-sdk-0.0.8/src/frinx/workers/monitoring/influxdb_workers.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/workers/test/test_worker.py` & `frinx-python-sdk-0.0.8/src/frinx/workers/test/test_worker.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/workers/uniconfig/cli_worker.py` & `frinx-python-sdk-0.0.8/src/frinx/workers/uniconfig/cli_worker.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/workers/uniconfig/netconf_worker.py` & `frinx-python-sdk-0.0.8/src/frinx/workers/uniconfig/netconf_worker.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/workers/uniconfig/uniconfig_worker.py` & `frinx-python-sdk-0.0.8/src/frinx/workers/uniconfig/uniconfig_worker.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/workflows/inventory/inventory_workflows.py` & `frinx-python-sdk-0.0.8/src/frinx/workflows/inventory/inventory_workflows.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/workflows/misc/http.py` & `frinx-python-sdk-0.0.8/src/frinx/workflows/misc/http.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/workflows/misc/test.py` & `frinx-python-sdk-0.0.8/src/frinx/workflows/misc/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from frinx.common.workflow.service import ServiceWorkflowsImpl
+from frinx.common.conductor_enums import TimeoutPolicy
 from frinx.common.workflow.task import DynamicForkTask
 from frinx.common.workflow.task import DynamicForkTaskInputParameters
 from frinx.common.workflow.task import JoinTask
 from frinx.common.workflow.task import SimpleTask
 from frinx.common.workflow.task import SimpleTaskInputParameters
 from frinx.common.workflow.workflow import FrontendWFInputFieldType
 from frinx.common.workflow.workflow import WorkflowImpl
@@ -12,14 +12,15 @@
 
 class TestWorkflow(WorkflowImpl):
     name = "Test_workflow"
     version = 1
     description = "Test workflow built from test workers"
     labels = ["TEST"]
     timeout_seconds = 60 * 5
+    timeout_policy = TimeoutPolicy.TIME_OUT_WORKFLOW
 
     class WorkflowInput(WorkflowImpl.WorkflowInput):
         num_paragraphs = WorkflowInputField(
             name="num_paragraphs",
             frontend_default_value=10,
             description="Paragraphs to generate",
             type=FrontendWFInputFieldType.INT,
@@ -85,14 +86,15 @@
 
 class TestForkWorkflow(WorkflowImpl):
     name = "Test_fork_workflow"
     version = 1
     description = "Test workflows executed in a parallel, dynamic fork"
     labels = ["TEST"]
     timeout_seconds = 60 * 5
+    timeout_policy = TimeoutPolicy.TIME_OUT_WORKFLOW
 
     class WorkflowInput(TestWorkflow.WorkflowInput):
         fork_count = WorkflowInputField(
             name="fork_count",
             frontend_default_value=10,
             description="How many forks to execute in parallel",
             type=FrontendWFInputFieldType.INT,
```

### Comparing `frinx-python-sdk-0.0.7/src/frinx/workflows/monitoring/influxdb.py` & `frinx-python-sdk-0.0.8/src/frinx/workflows/monitoring/influxdb.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx/workflows/uniconfig/transactions.py` & `frinx-python-sdk-0.0.8/src/frinx/workflows/uniconfig/transactions.py`

 * *Files identical despite different names*

### Comparing `frinx-python-sdk-0.0.7/src/frinx_python_sdk.egg-info/SOURCES.txt` & `frinx-python-sdk-0.0.8/src/frinx_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

