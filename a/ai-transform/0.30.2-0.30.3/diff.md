# Comparing `tmp/ai_transform-0.30.2.tar.gz` & `tmp/ai_transform-0.30.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_transform-0.30.2.tar", last modified: Tue Apr  4 06:25:57 2023, max compression
+gzip compressed data, was "ai_transform-0.30.3.tar", last modified: Tue Apr 11 03:15:14 2023, max compression
```

## Comparing `ai_transform-0.30.2.tar` & `ai_transform-0.30.3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.890206 ai_transform-0.30.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-04 06:25:37.000000 ai_transform-0.30.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-04 06:25:57.890206 ai_transform-0.30.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-04 06:25:37.000000 ai_transform-0.30.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.882206 ai_transform-0.30.2/ai_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.886206 ai_transform-0.30.2/ai_transform/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32153 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.886206 ai_transform-0.30.2/ai_transform/components/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/components/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.886206 ai_transform-0.30.2/ai_transform/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/dataset/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.886206 ai_transform-0.30.2/ai_transform/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/engine/abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/engine/dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/engine/in_memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/engine/multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/engine/small_batch_stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/engine/stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.886206 ai_transform-0.30.2/ai_transform/operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/operator/abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/operator/dense_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.890206 ai_transform-0.30.2/ai_transform/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/utils/document_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/utils/encode_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/utils/keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.890206 ai_transform-0.30.2/ai_transform/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/workflow/abstract_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/workflow/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-04 06:25:37.000000 ai_transform-0.30.2/ai_transform/workflow/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.886206 ai_transform-0.30.2/ai_transform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-04 06:25:57.000000 ai_transform-0.30.2/ai_transform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-04 06:25:57.000000 ai_transform-0.30.2/ai_transform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 06:25:57.000000 ai_transform-0.30.2/ai_transform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-04 06:25:57.000000 ai_transform-0.30.2/ai_transform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-04 06:25:57.000000 ai_transform-0.30.2/ai_transform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 06:25:57.890206 ai_transform-0.30.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-04 06:25:37.000000 ai_transform-0.30.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.890206 ai_transform-0.30.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.890206 ai_transform-0.30.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.890206 ai_transform-0.30.2/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_api/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_api/test_keyphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.890206 ai_transform-0.30.2/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_dataset/test_keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.890206 ai_transform-0.30.2/tests/core/test_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_engine/test_dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_engine/test_engine_playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_engine/test_multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_engine/test_stable_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.890206 ai_transform-0.30.2/tests/core/test_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_operator/test_abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_operator/test_document_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:57.890206 ai_transform-0.30.2/tests/core/test_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_workflow/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/core/test_workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-04 06:25:37.000000 ai_transform-0.30.2/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.023920 ai_transform-0.30.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-11 03:14:57.000000 ai_transform-0.30.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-11 03:15:14.023920 ai_transform-0.30.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-11 03:14:57.000000 ai_transform-0.30.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.015920 ai_transform-0.30.3/ai_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.015920 ai_transform-0.30.3/ai_transform/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32153 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.015920 ai_transform-0.30.3/ai_transform/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/components/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.015920 ai_transform-0.30.3/ai_transform/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/dataset/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/ai_transform/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/engine/abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/engine/dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/engine/in_memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/engine/multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/engine/small_batch_stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/engine/stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/ai_transform/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/operator/abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/operator/dense_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/ai_transform/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/utils/document_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/utils/encode_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/utils/keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/ai_transform/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/workflow/abstract_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/workflow/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-11 03:14:57.000000 ai_transform-0.30.3/ai_transform/workflow/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.015920 ai_transform-0.30.3/ai_transform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-11 03:15:14.000000 ai_transform-0.30.3/ai_transform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-11 03:15:14.000000 ai_transform-0.30.3/ai_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:15:14.000000 ai_transform-0.30.3/ai_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-11 03:15:14.000000 ai_transform-0.30.3/ai_transform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 03:15:14.000000 ai_transform-0.30.3/ai_transform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 03:15:14.023920 ai_transform-0.30.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-11 03:14:57.000000 ai_transform-0.30.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_api/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_api/test_keyphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.019920 ai_transform-0.30.3/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_dataset/test_keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.023920 ai_transform-0.30.3/tests/core/test_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_engine/test_dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_engine/test_engine_playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_engine/test_multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_engine/test_stable_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.023920 ai_transform-0.30.3/tests/core/test_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_operator/test_abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_operator/test_document_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:15:14.023920 ai_transform-0.30.3/tests/core/test_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_workflow/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/core/test_workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-11 03:14:57.000000 ai_transform-0.30.3/tests/test_connection_retry.py
```

### Comparing `ai_transform-0.30.2/LICENSE` & `ai_transform-0.30.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/README.md` & `ai_transform-0.30.3/README.md`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/__init__.py` & `ai_transform-0.30.3/ai_transform/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.30.2"
+__version__ = "0.30.3"
 
 from ai_transform.timer import Timer
 
 
 _TIMER = Timer()
 _TIMER.start()
```

### Comparing `ai_transform-0.30.2/ai_transform/api/api.py` & `ai_transform-0.30.3/ai_transform/api/api.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/api/client.py` & `ai_transform-0.30.3/ai_transform/api/client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/api/helpers.py` & `ai_transform-0.30.3/ai_transform/api/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/api/wrappers.py` & `ai_transform-0.30.3/ai_transform/api/wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,16 @@
                     }
                 )
                 if output_to_stdout:
                     print(to_log)
                 else:
                     logger.debug(to_log)
 
+                raise ValueError(to_log)
+
             if retry_func(result):
                 to_log_for_retry = "Manual Retry Triggered..."
                 if output_to_stdout:
                     print(to_log_for_retry)
                 else:
                     logger.debug(to_log_for_retry)
                 raise ManualRetry
```

### Comparing `ai_transform-0.30.2/ai_transform/components/components.py` & `ai_transform-0.30.3/ai_transform/components/components.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/config.py` & `ai_transform-0.30.3/ai_transform/config.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/dataset/dataset.py` & `ai_transform-0.30.3/ai_transform/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/dataset/field.py` & `ai_transform-0.30.3/ai_transform/dataset/field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/engine/abstract_engine.py` & `ai_transform-0.30.3/ai_transform/engine/abstract_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/engine/dense_output_engine.py` & `ai_transform-0.30.3/ai_transform/engine/dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/engine/in_memory_engine.py` & `ai_transform-0.30.3/ai_transform/engine/in_memory_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/engine/multipass_engine.py` & `ai_transform-0.30.3/ai_transform/engine/multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/engine/small_batch_stable_engine.py` & `ai_transform-0.30.3/ai_transform/engine/small_batch_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/engine/stable_engine.py` & `ai_transform-0.30.3/ai_transform/engine/stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/errors.py` & `ai_transform-0.30.3/ai_transform/errors.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/logger.py` & `ai_transform-0.30.3/ai_transform/logger.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/operator/abstract_operator.py` & `ai_transform-0.30.3/ai_transform/operator/abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/operator/dense_operator.py` & `ai_transform-0.30.3/ai_transform/operator/dense_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/timer.py` & `ai_transform-0.30.3/ai_transform/timer.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/types.py` & `ai_transform-0.30.3/ai_transform/types.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/utils/document.py` & `ai_transform-0.30.3/ai_transform/utils/document.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/utils/document_list.py` & `ai_transform-0.30.3/ai_transform/utils/document_list.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/utils/example_documents.py` & `ai_transform-0.30.3/ai_transform/utils/example_documents.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/utils/json_encoder.py` & `ai_transform-0.30.3/ai_transform/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/utils/keyphrase.py` & `ai_transform-0.30.3/ai_transform/utils/keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/workflow/abstract_workflow.py` & `ai_transform-0.30.3/ai_transform/workflow/abstract_workflow.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/workflow/context_manager.py` & `ai_transform-0.30.3/ai_transform/workflow/context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform/workflow/helpers.py` & `ai_transform-0.30.3/ai_transform/workflow/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/ai_transform.egg-info/SOURCES.txt` & `ai_transform-0.30.3/ai_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/setup.py` & `ai_transform-0.30.3/setup.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/tests/conftest.py` & `ai_transform-0.30.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/tests/core/test_api/test_endpoints.py` & `ai_transform-0.30.3/tests/core/test_api/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/tests/core/test_api/test_keyphrase.py` & `ai_transform-0.30.3/tests/core/test_api/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/tests/core/test_api/test_wrappers.py` & `ai_transform-0.30.3/tests/core/test_api/test_wrappers.py`

 * *Files 21% similar despite different names*

```diff
@@ -60,14 +60,47 @@
             else:
                 return False
 
         with redirect_stdout(f), redirect_stderr(u):
             resp = request_wrapper(
                 requests.get,
                 ("https://www.google.com",),
-                timeout=1,
                 num_retries=2,
                 retry_func=retry_func,
+                timeout=1,
                 output_to_stdout=True,
             )
 
         assert "Manual Retry" in str(u.getvalue()) + str(f.getvalue())
+
+    def test_request_wrapper_retry(self):
+        f = io.StringIO()
+        u = io.StringIO()
+
+        class TestRequest:
+            def __init__(self):
+                self.count = 0
+
+            def __call__(self, *args, **kwargs):
+                if self.count >= 2:
+                    return requests.get(*args, **kwargs)
+                else:
+                    self.count += 1
+                    placeholder = requests.Response()
+                    placeholder.status_code = 429
+                    placeholder._content = b"Simulated Rate Error"
+                    return placeholder
+
+        with redirect_stdout(f), redirect_stderr(u):
+            resp = request_wrapper(
+                TestRequest(),
+                ("https://www.google.com",),
+                num_retries=3,
+                timeout=1,
+                output_to_stdout=True,
+            )
+
+        assert resp.status_code == 200
+
+        logs = str(u.getvalue()) + str(f.getvalue())
+
+        assert logs.count("Simulated Rate Error") == 2
```

### Comparing `ai_transform-0.30.2/tests/core/test_dataset/test_dataset.py` & `ai_transform-0.30.3/tests/core/test_dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/tests/core/test_dataset/test_field.py` & `ai_transform-0.30.3/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/tests/core/test_dataset/test_keyphrase.py` & `ai_transform-0.30.3/tests/core/test_dataset/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/tests/core/test_engine/test_dense_output_engine.py` & `ai_transform-0.30.3/tests/core/test_engine/test_dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/tests/core/test_engine/test_engine.py` & `ai_transform-0.30.3/tests/core/test_engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/tests/core/test_engine/test_engine_playground.py` & `ai_transform-0.30.3/tests/core/test_engine/test_engine_playground.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/tests/core/test_engine/test_multipass_engine.py` & `ai_transform-0.30.3/tests/core/test_engine/test_multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/tests/core/test_engine/test_stable_engine.py` & `ai_transform-0.30.3/tests/core/test_engine/test_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/tests/core/test_operator/test_abstract_operator.py` & `ai_transform-0.30.3/tests/core/test_operator/test_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/tests/core/test_operator/test_document_diff.py` & `ai_transform-0.30.3/tests/core/test_operator/test_document_diff.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/tests/core/test_workflow/test_context_manager.py` & `ai_transform-0.30.3/tests/core/test_workflow/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.2/tests/core/test_workflow/test_workflow.py` & `ai_transform-0.30.3/tests/core/test_workflow/test_workflow.py`

 * *Files identical despite different names*

