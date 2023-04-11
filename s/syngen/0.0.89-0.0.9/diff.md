# Comparing `tmp/syngen-0.0.89.tar.gz` & `tmp/syngen-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.0.89.tar", last modified: Tue Apr 11 09:12:48 2023, max compression
+gzip compressed data, was "syngen-0.0.9.tar", last modified: Fri Jul 29 15:03:43 2022, max compression
```

## Comparing `syngen-0.0.89.tar` & `syngen-0.0.9.tar`

### file list

```diff
@@ -1,78 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.191810 syngen-0.0.89/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-11 09:11:05.000000 syngen-0.0.89/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-11 09:11:05.000000 syngen-0.0.89/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-11 09:11:05.000000 syngen-0.0.89/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-11 09:12:48.191810 syngen-0.0.89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14148 2023-04-11 09:11:05.000000 syngen-0.0.89/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-11 09:11:05.000000 syngen-0.0.89/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-04-11 09:12:48.191810 syngen-0.0.89/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.175810 syngen-0.0.89/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.179810 syngen-0.0.89/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.183810 syngen-0.0.89/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.183810 syngen-0.0.89/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10091 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.183810 syngen-0.0.89/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.183810 syngen-0.0.89/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7294 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.183810 syngen-0.0.89/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.183810 syngen-0.0.89/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.179810 syngen-0.0.89/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.183810 syngen-0.0.89/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.187811 syngen-0.0.89/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43499 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.187811 syngen-0.0.89/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.187811 syngen-0.0.89/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6256 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.187811 syngen-0.0.89/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.187811 syngen-0.0.89/src/syngen/ml/train_chain/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/train_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15932 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/train_chain/train_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.187811 syngen-0.0.89/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5009 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.187811 syngen-0.0.89/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.191810 syngen-0.0.89/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    28464 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10390 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.191810 syngen-0.0.89/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11009 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.191810 syngen-0.0.89/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.191810 syngen-0.0.89/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12935 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-04-11 09:11:05.000000 syngen-0.0.89/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 09:12:48.183810 syngen-0.0.89/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-11 09:12:48.000000 syngen-0.0.89/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-04-11 09:12:48.000000 syngen-0.0.89/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 09:12:48.000000 syngen-0.0.89/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-11 09:12:48.000000 syngen-0.0.89/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-11 09:12:48.000000 syngen-0.0.89/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-11 09:12:48.000000 syngen-0.0.89/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.421023 syngen-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-07-29 15:01:35.000000 syngen-0.0.9/CHAGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2022-07-29 15:01:35.000000 syngen-0.0.9/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (121)    35129 2022-07-29 15:01:35.000000 syngen-0.0.9/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-07-29 15:01:35.000000 syngen-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-07-29 15:01:35.000000 syngen-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4518 2022-07-29 15:03:43.421023 syngen-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3748 2022-07-29 15:01:35.000000 syngen-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-07-29 15:01:35.000000 syngen-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1662 2022-07-29 15:01:35.000000 syngen-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2691 2022-07-29 15:03:43.425023 syngen-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.413023 syngen-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.417023 syngen-0.0.9/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3231 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.417023 syngen-0.0.9/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.417023 syngen-0.0.9/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.417023 syngen-0.0.9/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.417023 syngen-0.0.9/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.417023 syngen-0.0.9/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.417023 syngen-0.0.9/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22159 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/metrics/metrics_classes/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.417023 syngen-0.0.9/src/syngen/ml/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4778 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/pipeline/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.421023 syngen-0.0.9/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3692 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.421023 syngen-0.0.9/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.421023 syngen-0.0.9/src/syngen/ml/train_chain/
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/train_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8528 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/train_chain/train_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.421023 syngen-0.0.9/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.421023 syngen-0.0.9/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9163 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22795 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9588 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.421023 syngen-0.0.9/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9322 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/ml/vae/wrappers/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3030 2022-07-29 15:01:35.000000 syngen-0.0.9/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 15:03:43.417023 syngen-0.0.9/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4518 2022-07-29 15:03:43.000000 syngen-0.0.9/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-07-29 15:03:43.000000 syngen-0.0.9/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-29 15:03:43.000000 syngen-0.0.9/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-07-29 15:03:43.000000 syngen-0.0.9/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-07-29 15:03:43.000000 syngen-0.0.9/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-29 15:03:43.000000 syngen-0.0.9/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.0.89/LICENSE` & `syngen-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.0.89/src/syngen/infer.py` & `syngen-0.0.9/src/syngen/infer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,112 @@
+import click
 from typing import Optional
 
-import click
-from loguru import logger
+from syngen.ml.config import InferConfig
+from syngen.ml.reporters import Report, AccuracyReporter
+from syngen.ml.strategies import InferStrategy
+from syngen.ml.train_chain import VaeInferHandler
+from syngen.ml.data_loaders import MetadataLoader
+from syngen.ml.vae import VanillaVAEWrapper
+
+
+def get_metadata(config):
+    if config.metadata_path:
+        metadata = MetadataLoader().load_data(config.metadata_path)
+        return metadata
+    elif config.table_name:
+        metadata = {"table_name": config.table_name}
+        return metadata
+    else:
+        raise AttributeError("Either table name or path to metadata MUST be provided")
+
+
+def set_handler(config):
+    return VaeInferHandler(
+        metadata=get_metadata(config),
+        paths=config.set_paths(),
+        wrapper_name=VanillaVAEWrapper.__name__,
+        random_seed=config.random_seed,
+        keys_mode=config.keys_mode
+    )
+
 
-from syngen.ml.worker import Worker
+def set_reporters(config):
+    """
+    Set up reporter which used in order to create the report during infer process
+    """
+    accuracy_reporter = AccuracyReporter(
+        metadata={"table_name": config.table_name},
+        paths=config.set_paths()
+    )
+    Report().register_reporter(accuracy_reporter)
+
+
+def infer(config: InferConfig):
+    """
+    Launch the infer strategy
+    """
+    set_handler(config)
+
+    set_reporters(config)
+
+    infer_strategy = InferStrategy(
+        size=config.size,
+        run_parallel=config.run_parallel,
+        keys_mode=config.keys_mode,
+        metadata_path=config.metadata_path,
+        print_report=config.print_report,
+        batch_size=config.batch_size,
+        handler=set_handler(config)
+    )
+
+    infer_strategy.run()
 
 
 @click.command()
-@click.option("--metadata_path", type=str, default=None, help="Path to the metadata file")
-@click.option("--size", default=100, type=click.IntRange(1),
-              help="Desired number of rows to generate. If absent, it's defaulted to 100")
-@click.option("--table_name", default=None, type=str, help="Name of the table, same as in training")
-@click.option("--run_parallel", default=False, type=click.BOOL,
-              help="The flag which set whether to use multiprocessing (feasible for tables > 5000 rows)."
-                   "If absent, it's defaulted to False")
-@click.option("--batch_size", default=None, type=click.IntRange(1),
-              help="If specified, the generation is split into batches. This can save the RAM")
-@click.option("--random_seed", default=None, type=click.IntRange(0),
+@click.argument("size", type=int)
+@click.argument("table_name", type=str)
+@click.option("--run_parallel", default=True, type=bool)
+@click.option("--batch_size", default=None, type=int)
+@click.option("--keys_mode", default=None, type=str,
+              help ="When generating data for multiple tables use keys_mode = multable.")
+@click.option("--metadata_path", default=None, type=str)
+@click.option("--random_seed", default=None, type=int,
               help="Set any int in case you want reproducible results. To reproduce generated data again, "
                    "use the same int in this command.")
-@click.option("--print_report", default=False, type=click.BOOL,
-              help="Whether to print quality report. Might require significant time "
-                   "for big generated tables (>1000 rows). If absent, it's defaulted to False")
-def launch_infer(
-        metadata_path: Optional[str],
-        size: Optional[int],
-        table_name: Optional[str],
+@click.option("--print_report", default=False, type=bool,
+              help="Whether to print quality report. Might require significant time for big generated tables "
+                   "(>1000 rows)")
+def infer_model(
+        size: int,
+        table_name: str,
         run_parallel: bool,
         batch_size: Optional[int],
-        print_report: bool,
-        random_seed: Optional[int]
-):
+        keys_mode: Optional[bool],
+        metadata_path: Optional[str],
+        random_seed: Optional[int],
+        print_report: bool):
     """
     Launch the work of infer process
+
     Parameters
     ----------
-    metadata_path
     size
     table_name
     run_parallel
     batch_size
-    print_report
+    keys_mode
+    metadata_path
     random_seed
-    -------
-
+    print_report
     """
-    if not metadata_path and not table_name:
-        raise AttributeError("It seems that the information of metadata_path or table_name is absent. "
-                             "Please provide either the information of metadata_path or the information of table_name.")
-    if metadata_path:
-        if table_name:
-            logger.warning("The information of metadata_path was provided. "
-                           "In this case the information of table_name will be ignored.")
-            table_name = None
-        if not metadata_path.endswith(('.yaml', '.yml')):
-            raise NotImplementedError("This format for metadata_path is not supported. "
-                                      "Please provide metadata_path in '.yaml' or in '.yml' format")
-    settings = {
-        "size": size,
-        "run_parallel": run_parallel,
-        "batch_size": batch_size,
-        "print_report": print_report,
-        "random_seed": random_seed
-    }
-    worker = Worker(
-        table_name=table_name,
-        metadata_path=metadata_path,
-        settings=settings
+    infer_config = InferConfig(
+        size, run_parallel, table_name, batch_size,
+        keys_mode, metadata_path, random_seed, print_report
     )
-    worker.launch_infer()
+
+    infer(infer_config)
 
 
 if __name__ == "__main__":
-    launch_infer()
+    infer_model()
+
```

### Comparing `syngen-0.0.89/src/syngen/ml/reporters/reporters.py` & `syngen-0.0.9/src/syngen/ml/reporters/reporters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,63 @@
 from abc import abstractmethod
-from typing import List, Dict
-
+from typing import List
 import pandas as pd
-import numpy as np
 from loguru import logger
 
-from syngen.ml.utils import (
+from syngen.ml.pipeline import (
+    data_pipeline,
     get_nan_labels,
-    nan_labels_to_float,
-    fetch_dataset
+    nan_labels_to_float
 )
-from syngen.ml.metrics import AccuracyTest, SampleAccuracyTest
-from syngen.ml.data_loaders import DataLoader
+from syngen.ml.metrics import AccuracyTest
 from syngen.ml.metrics.utils import text_to_continuous
 
 
 class Reporter:
     """
     Abstract class for reporters
     """
-
-    def __init__(
-            self,
-            metadata: Dict[str, str],
-            paths: Dict[str, str],
-            config: Dict[str, str]
-    ):
-        self.metadata = metadata
+    def __init__(self, metadata: dict, paths: dict):
+        super().__init__()
         self.table_name = metadata["table_name"]
         self.paths = paths
-        self.config = config
-
-    def extract_report_data(self):
-        original, schema = DataLoader(self.paths["original_data_path"]).load_data()
-        synthetic, schema = DataLoader(self.paths["synthetic_data_path"]).load_data()
-        return original, synthetic
-
-    def fetch_data_types(self):
-        dataset = fetch_dataset(self.paths["dataset_pickle_path"])
-        types = (
-            dataset.str_columns, dataset.date_columns,
-            dataset.int_columns, dataset.float_columns,
-            dataset.binary_columns, dataset.categ_columns
-        )
-        return types
 
     def preprocess_data(self):
         """
         Preprocess original and synthetic data.
         Return original data, synthetic data, float columns, integer columns, categorical columns
         """
-        original, synthetic = self.extract_report_data()
-        missing_columns = set(original) - set(synthetic)
-        for col in missing_columns:
-            synthetic[col] = np.nan
+        original = pd.read_csv(self.paths["original_data_path"], engine="python")
+        synthetic = pd.read_csv(self.paths["synthetic_data_path"], engine="python")
         columns_nan_labels = get_nan_labels(original)
         original = nan_labels_to_float(original, columns_nan_labels)
         synthetic = nan_labels_to_float(synthetic, columns_nan_labels)
-        types = self.fetch_data_types()
-        str_columns, date_columns, int_columns, float_columns, binary_columns, categ_columns = types
-        original = original[[
-            col for col in original.columns
-            if col in set().union(*types)
-        ]]
-        synthetic = synthetic[[
-            col for col in synthetic.columns
-            if col in set().union(*types)
-        ]]
+        types = data_pipeline(original)
+        str_columns, float_columns, categ_columns, date_columns, int_columns, binary_columns = types
         for date_col in date_columns:
             original[date_col] = list(
                 map(lambda d: pd.Timestamp(d).value, original[date_col])
             )
             synthetic[date_col] = list(
                 map(lambda d: pd.Timestamp(d).value, synthetic[date_col])
             )
 
         int_columns = date_columns | int_columns
-
         original = text_to_continuous(original, str_columns).drop(str_columns, axis=1)
         synthetic = text_to_continuous(synthetic, str_columns).drop(str_columns, axis=1)
 
         for col in [i + "_word_count" for i in str_columns]:
-            if original[col].nunique() < 50:  # ToDo check if we need this
+            if original[col].nunique() < 50:
                 categ_columns = categ_columns | {col}
             else:
                 int_columns = int_columns | {col}
         int_columns = int_columns | {i + "_char_len" for i in str_columns}
-
         categ_columns = categ_columns | binary_columns
-        
-        for categ_col in categ_columns:
-            original[categ_col] = original[categ_col].astype(str)
-            synthetic[categ_col] = synthetic[categ_col].astype(str)
-        return original, synthetic, float_columns, int_columns, categ_columns, date_columns
+
+        return original, synthetic, float_columns, int_columns, categ_columns
 
     @abstractmethod
     def report(self, **kwargs):
         """
         Generate the report for certain test
         """
         pass
@@ -118,21 +79,14 @@
     def register_reporter(cls, reporter: Reporter):
         """
         Register all needed reporters
         """
         cls.__reporters.append(reporter)
 
     @classmethod
-    def clear_report(cls):
-        """
-        Delete unnecessary reporters
-        """
-        cls.__reporters.clear()
-
-    @classmethod
     def generate_report(cls):
         """
         Generate all needed reports
         """
         for reporter in cls.__reporters:
             reporter.report()
 
@@ -148,53 +102,17 @@
         """
         (
             original,
             synthetic,
             float_columns,
             int_columns,
             categ_columns,
-            date_columns
         ) = self.preprocess_data()
-        accuracy_test = AccuracyTest(original, synthetic, self.paths, self.table_name, self.config)
+        accuracy_test = AccuracyTest(original, synthetic, self.paths)
         accuracy_test.report(
             cont_columns=list(float_columns | int_columns),
-            categ_columns=list(categ_columns),
-            date_columns=list(date_columns)
+            categ_columns=list(categ_columns)
         )
         logger.info(
             f"Corresponding plot pickle files regarding to accuracy test were saved "
-            f"to folder '{self.paths['draws_path']}'."
-        )
-
-
-class SampleAccuracyReporter(Reporter):
-    """
-    Reporter for running accuracy test
-    """
-
-    def extract_report_data(self):
-        original, schema = DataLoader(self.paths["source_path"]).load_data()
-        sampled, schema = DataLoader(self.paths["input_data_path"]).load_data()
-        return original, sampled
-
-    def report(self):
-        """
-        Run the report
-        """
-        (
-            original,
-            sampled,
-            float_columns,
-            int_columns,
-            categ_columns,
-            date_columns
-        ) = self.preprocess_data()
-        accuracy_test = SampleAccuracyTest(original, sampled, self.paths, self.table_name, self.config)
-        accuracy_test.report(
-            cont_columns=list(float_columns | int_columns),
-            categ_columns=list(categ_columns),
-            date_columns=list(date_columns)
-        )
-        logger.info(
-            f"Corresponding plot pickle files regarding to sampled data accuracy test were saved "
-            f"to folder {self.paths['draws_path']}."
+            f"to folder 'model_artifacts/tmp_store/{self.table_name}/draws/'."
         )
```

### Comparing `syngen-0.0.89/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.0.9/src/syngen/ml/vae/models/custom_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         feature_input, feature_decoder = inputs
         self.add_loss(self.feature.loss, inputs=inputs)
         return feature_decoder
 
 
 class SampleLayer(Layer):
     def __init__(self, gamma, capacity, **kwargs):
-        super().__init__(**kwargs)
+        super(SampleLayer, self).__init__(**kwargs)
         self.gamma = gamma
         self.max_capacity = capacity
 
     def build(self, input_shape):
         super(SampleLayer, self).build(input_shape)
         self.built = True
```

### Comparing `syngen-0.0.89/src/syngen/ml/vae/models/features.py` & `syngen-0.0.9/src/syngen/ml/vae/models/features.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,122 +1,88 @@
 from collections import Counter
 from itertools import chain
 from typing import Union, List
 import re
-from lazy import lazy
-
 import category_encoders as ce
 import numpy as np
 import pandas as pd
 from pandas._libs.tslibs.parsing import guess_datetime_format
 import tensorflow as tf
 import tensorflow.keras.backend as K
-from scipy.stats import shapiro
-from sklearn.preprocessing import StandardScaler, MinMaxScaler
+from lazy import lazy
+from sklearn.preprocessing import StandardScaler
 from tensorflow.keras import losses
-from tensorflow.keras.layers import (
-    Bidirectional,
-    Dense,
-    Input,
-    LSTM,
-    Layer,
-    RepeatVector,
-    TimeDistributed
-)
-
-from syngen.ml.utils import slugify_parameters, inverse_dict
-
-
-class BaseFeature:
-    """
-    Base class for feature classes.
-    Each feature class implements feature preprocessing, transformation and inverse transformation.
-    What is more, each feature class contains modules for the neural network (NN), including
-    corresponding input, encoder, decoder, and loss
-    """
-    def __init__(self, name):
-        self.name: str = self._reset_name(name=name)
-        self.original_name: str = name
-        self.weight: float = 1.0
-
-    @staticmethod
-    @slugify_parameters()
-    def _reset_name(name):
-        """
-        Slugify the attribute 'name' of the instance
-        """
-        return name
-
-    def fit(self, data: pd.DataFrame):
-        """
-        Fit scalars, one-hot encoders, and mappers in the data
-        """
-        pass
-
-    def transform(self, data: pd.DataFrame) -> List:
-        """
-        Transform feature to numeric format according to the fitted preprocessors
-        """
-        pass
-
-    def inverse_transform(self, data: List) -> np.ndarray:
-        """
-        Inverse transform feature from numeric to original format to obtain an original-like table
-        """
-        pass
+from tensorflow.keras.layers import Bidirectional
+from tensorflow.keras.layers import Dense
+from tensorflow.keras.layers import Input
+from tensorflow.keras.layers import LSTM
+from tensorflow.keras.layers import Layer
+from tensorflow.keras.layers import RepeatVector
+from tensorflow.keras.layers import TimeDistributed
+from syngen.ml.vae.models.model import check_name
+
+
+def dict_inverse(dictionary):
+    return dict(zip(dictionary.values(), dictionary.keys()))
+
+
+"""
+Each feature class implements feature preprocessing, transformation and inverse transformation. 
+What is more, each feature class contains modules for the neural network (NN), including 
+corresponding input, encoder, decoder, and loss.
+
+Methods
+-------
+fit(data)
+    fir scalers, one-hot encoders and mappers on data
+
+transform(data)
+    transform feature to numeric format according to the fitted preprocessors
+
+inverse_transform(data)
+    inverse transform feature from numeric to original format to obtain an original-like table
+
+input()
+    define a feature-specific input for the NN
+
+encoder()
+    define a feature-specific encoder for the NN
+    
+create_decoder(encoder_output)
+    create a feature-specific decoder combining given decoder layers and encoder outputs
+    
+loss()
+    define a feature-specific loss taking into account the data types
+    
+__decoder_layer()
+    define an elementary layer for decoder to use in create_decoder() method
+"""
 
-    def input(self) -> tf.Tensor:
-        """
-        Define a feature-specific input for the NN
-        """
-        pass
-
-    def encoder(self) -> tf.Tensor:
-        """
-        Define a feature-specific encoder for the NN
-        """
-        pass
-
-    def __decoder_layer(self) -> tf.Tensor:
-        """
-        Define an elementary layer for decoder to use in create_decoder() method
-        """
-        pass
 
-    def create_decoder(self, encoder_output: tf.Tensor):
-        """
-        Create a feature-specific decoder combining given decoder layers and encoder outputs
-        """
-        pass
-
-    def loss(self) -> tf.Tensor:
-        """
-        Define a feature-specific loss taking into account the data types
-        """
-        pass
-
-
-class BinaryFeature(BaseFeature):
-    """
-    A class to process binary features, i.e. features containing only two unique values
-    """
-    def __init__(self, name: str):
-        super().__init__(name=name)
+class BinaryFeature:
+    # A class to process binary features, i.e. features containing only two unique values
+    def __init__(
+            self,
+            name: str,
+            weight: float = 1.0
+    ):
+        self.name = "_".join(name.split())
+        self.weight = weight
 
     def fit(self, data: pd.DataFrame):
         self.mapping = {k: n for n, k in enumerate(np.unique(data))}
-        self.inverse_mapping = inverse_dict(self.mapping)
+        self.inverse_mapping = dict_inverse(self.mapping)
         self.inverse_vectorizer = np.vectorize(self.inverse_mapping.get)
         self.input_dimension = data.shape[1]
 
-    def transform(self, data: pd.DataFrame) -> List:
+    def transform(self, data: pd.DataFrame) -> list:
         data = data.replace(self.mapping)
-        return data.astype("float64")
+        return data
 
-    def inverse_transform(self, data: List) -> np.ndarray:
+    def inverse_transform(self, data: list) -> np.ndarray:
         data = np.round(data)
         inversed = self.inverse_vectorizer(data)
         return np.where(inversed == "?", None, inversed)
 
     @lazy
     def input(self) -> tf.Tensor:
         return Input(shape=(self.input_dimension,), name="input_%s" % self.name)
@@ -137,26 +103,25 @@
     def loss(self) -> tf.Tensor:
         if not hasattr(self, "decoder"):
             Exception("Decoder isn't created")
 
         return self.weight * losses.binary_crossentropy(self.input, self.decoder)
 
 
-class ContinuousFeature(BaseFeature):
-    """
-    A class to process the continuous numeric features, including floats and integers
-    """
+class ContinuousFeature:
+    # A class to process the continuous numeric features, including floats and integers
     def __init__(
         self,
         name: str,
+        weight: float = 1.0,
         decoder_layers: Union[None, tuple, int] = (60,),
         weight_randomizer: Union[None, bool, tuple] = None,
         column_type=float,
     ):
-        super().__init__(name=name)
+
         if decoder_layers is None:
             decoder_layers = ()
         elif isinstance(decoder_layers, int):
             decoder_layers = (decoder_layers,)
 
         # TODO: teset features
         if weight_randomizer is None or (
@@ -164,31 +129,30 @@
         ):
             weight_randomizer = (1, 1)
         elif isinstance(weight_randomizer, bool) and weight_randomizer:
             weight_randomizer = (0, 1)
         elif isinstance(weight_randomizer, (float, int)):
             weight_randomizer = (weight_randomizer, weight_randomizer)
 
+        self.name = check_name("_".join(name.split()))
+        self.weight = weight
         self.decoder_layers = decoder_layers
         self.weight_randomizer = weight_randomizer
         self.column_type = column_type
 
     def fit(self, data: pd.DataFrame):
-        self.is_positive = (data >= 0).sum().item() >= len(data) * 0.99
-        normality = shapiro(data.sample(n=min(len(data), 500))).pvalue
-        self.scaler = StandardScaler() if normality >= 0.05 else MinMaxScaler()
+        self.scaler = StandardScaler()
         self.scaler.fit(data)
         self.input_dimension = data.shape[1]
 
     def transform(self, data: pd.DataFrame) -> np.ndarray:
         return self.scaler.transform(data).astype("float32")
 
     def inverse_transform(self, data: np.ndarray) -> np.ndarray:
         reverse_transformed = self.scaler.inverse_transform(data)
-        reverse_transformed = np.abs(reverse_transformed) if self.is_positive else reverse_transformed
         return (
             reverse_transformed
             if self.column_type is float
             else np.around(reverse_transformed).astype("int64")
         )
 
     @lazy
@@ -240,21 +204,20 @@
         low = self.weight_randomizer[0]
         high = self.weight_randomizer[1]
         random_weight = K.random_uniform_variable(shape=(1,), low=low, high=high)
 
         return random_weight * tf.keras.losses.MSE(self.input, self.decoder)
 
 
-class CategoricalFeature(BaseFeature):
-    """
-    A class to process categorical values, i.e. values with 2 < unique_values < 50
-    """
+class CategoricalFeature:
+    # A class to process categorical values, i.e. values with 2 < unique_values < 50
     def __init__(
         self,
         name: str,
+        weight: float = 1.0,
         decoder_layers: Union[None, tuple, int] = (60,),
         weight_randomizer: Union[None, bool, tuple] = None,
     ):
 
         if decoder_layers is None:
             decoder_layers = ()
         elif isinstance(decoder_layers, int):
@@ -265,29 +228,30 @@
         ):
             weight_randomizer = (1, 1)
         elif isinstance(weight_randomizer, (float, int)):
             weight_randomizer = (weight_randomizer, weight_randomizer)
         elif isinstance(weight_randomizer, bool) and weight_randomizer:
             weight_randomizer = (0, 1)
 
-        super().__init__(name="_".join(name.split()))
+        self.name = check_name("_".join(name.split()))
+        self.weight = weight
         self.one_hot_encoder = ce.OneHotEncoder(
             return_df=False, handle_unknown="ignore"
         )
         self.decoder = None
         self.decoder_layers = decoder_layers
         self.weight_randomizer = weight_randomizer
 
     def fit(self, data: pd.DataFrame):
         data = data.astype(object)
         self.one_hot_encoder.fit(data)
         self.mapping = {
             k: v for k, v in self.one_hot_encoder.category_mapping[0]["mapping"].items()
         }
-        self.inverse_mapping = inverse_dict(self.mapping)
+        self.inverse_mapping = dict_inverse(self.mapping)
         self.inverse_vectorizer = np.vectorize(self.inverse_mapping.get)
 
         # because in mapping exist additional class None, input dimensionality should be less on 1
         self.input_dimension = len(self.mapping) - 1
 
     def transform(self, data: pd.DataFrame) -> np.ndarray:
         if isinstance(data, pd.Series):
@@ -359,26 +323,27 @@
         random_weight = K.random_uniform_variable(shape=(1,), low=low, high=high)
 
         return random_weight * tf.keras.losses.categorical_crossentropy(
             self.input, self.decoder
         )
 
 
-class CharBasedTextFeature(BaseFeature):
-    """
-    A class to process the text features
-    """
+class CharBasedTextFeature:
+    # A class to process the text features
     def __init__(
         self,
         name: str,
         text_max_len: int,
+        weight: float = 1.0,
         rnn_units: int = 128,
         dropout: int = 0,
     ):
-        super().__init__(name=name)
+
+        self.name = check_name("_".join(name.split()))
+        self.weight = weight
         self.decoder = None
         self.text_max_len = text_max_len
         self.rnn_units = rnn_units
         self.rnn_unit = LSTM
         self.dropout = dropout
 
     def fit(self, data: pd.DataFrame):
@@ -387,15 +352,15 @@
         if len(data.columns) > 1:
             raise Exception("CharBasedTextFeature can work only with one text column")
 
         data = data[data.columns[0]]
 
         tokenizer = Tokenizer(lower=False, char_level=True)
         tokenizer.fit_on_texts(data)
-        tokenizer.inverse_dict = inverse_dict(tokenizer.word_index)
+        tokenizer.inverse_dict = dict_inverse(tokenizer.word_index)
 
         self.vocab_size = len(tokenizer.word_index)
         self.tokenizer = tokenizer
 
     def transform(self, data: pd.DataFrame) -> np.ndarray:
 
         if len(data.columns) > 1:
@@ -497,16 +462,18 @@
                 logits,
             )
 
         return logits_removed
 
     def inverse_transform(self, data: np.ndarray, **kwargs) -> List[str]:
         top_p = 0.9
+        top_k = 0.0
         if len(kwargs) > 0:
             top_p = kwargs["top_p"]
+            top_k = kwargs["top_k"]
 
         out = []
         for batch in data:
             # batch shape (self.text_max_len, self.vocab_size)
             logits = self.top_k_top_p_filtering(
                 tf.convert_to_tensor(batch), top_p=top_p
             )
@@ -574,19 +541,17 @@
         return self.weight * K.mean(
             tf.nn.softmax_cross_entropy_with_logits(
                 labels=self.input, logits=self.decoder
             )
         )
 
 
-class DateFeature(BaseFeature):
-    """
-    A class to process datetime features
-    """
-    def __init__(self, name, decoder_layers=(60,), weight_randomizer=None):
+class DateFeature:
+    # A class to process datetime features
+    def __init__(self, name, weight=1.0, decoder_layers=(60,), weight_randomizer=None):
 
         if decoder_layers is None:
             decoder_layers = ()
         elif isinstance(decoder_layers, int):
             decoder_layers = (decoder_layers,)
 
         # TODO: teset features
@@ -595,87 +560,57 @@
         ):
             weight_randomizer = (1, 1)
         elif isinstance(weight_randomizer, bool) and weight_randomizer:
             weight_randomizer = (0, 1)
         elif isinstance(weight_randomizer, (float, int)):
             weight_randomizer = (weight_randomizer, weight_randomizer)
 
-        super().__init__(name=name)
+        self.name = check_name("_".join(name.split()))
+        self.weight = weight
         self.decoder_layers = decoder_layers
         self.weight_randomizer = weight_randomizer
 
-    @staticmethod
-    def __validate_format(date_text: pd.DataFrame):
-        """
-        Define the most common date format.
-        Supported date formats -
-        MM/DD/YYYY; MM-DD-YYYY; DD/MM/YYYY; DD-MM-YYYY;
-        YYYY/MM/DD; YYYY-MM-DD; MMM DD, YYYY; MMM DD YYYY;
-        DD MMM YYYY; YYYY-MM-DD HH:MM:SS
-
-        Not supported formats -
-        MM/DD/YY, DD/MM/YY, YY/MM/DD, MM-DD-YY, DD-MM-YY
+    def __validate_format(self, date_text: pd.DataFrame):
 
-        """
-        pattern = r"\s{0,1}\d+[-/\\:]\s{0,1}\d+[-/\\:]\s{0,1}\d+|" \
-                  r"[A-Z][a-z]+ \d{1,2} \d{4}|" \
-                  r"[A-Z][a-z]+ \d{1,2}, \d{4}|" \
-                  r"\d{2} [A-Z][a-z]+ \d{4}"
+        pattern = r"\s{0,1}\d+[-/\\:]\s{0,1}\d+[-/\\:]\s{0,1}\d+"
         types = []
-        sample = date_text.dropna().sample(100, replace=len(date_text) <= 100).values
-        for i in sample:
-            date_format = guess_datetime_format(re.match(pattern, i[0]).group(0))
-            types.append(date_format)
-        if not list(filter(lambda x: bool(x), types)) or not types:
-            return "%d-%m-%Y"
-        if Counter(types).most_common(1)[0][0] is None:
-            return Counter(types).most_common(2)[1][0]
+        for i in date_text.dropna().sample(15).values:
+            try:
+                format = guess_datetime_format(re.match(pattern, i[0]).group(0))
+                types.append(format)
+            except AttributeError:
+                pass
+
         return Counter(types).most_common(1)[0][0]
 
     def fit(self, data):
         self.date_format = self.__validate_format(data)
         data = chain.from_iterable(data.values)
-        data = pd.DataFrame(list(map(lambda d: pd.Timestamp(d).value, data)))
-        self.is_positive = (data >= 0).sum().item() >= len(data) * 0.99
-        normality = shapiro(data.sample(n=min(len(data), 500))).pvalue
+        data = list(map(lambda d: pd.Timestamp(d).value, data))
         data = np.array(data).reshape(-1, 1)
 
-        self.scaler = StandardScaler() if normality >= 0.05 else MinMaxScaler()
+        self.scaler = StandardScaler()
         self.scaler.fit(data)
         self.input_dimension = data.shape[1]
 
     def transform(self, data):
         data = chain.from_iterable(data.values)
         data = list(map(lambda d: pd.Timestamp(d).value, data))
         data = np.array(data).reshape(-1, 1)
         return self.scaler.transform(data)
 
     def inverse_transform(self, data):
-        max_allowed_time_ns = int(9.2E18)
-        min_allowed_time_ns = int(-9.2E18)
-        unscaled = self.scaler.inverse_transform(data)
+        unscaled = self.scaler.inverse_transform(data).astype(np.uint64)
         unscaled = chain.from_iterable(unscaled)
-        if self.is_positive:
-            return list(
-                map(
-                    lambda l: pd.Timestamp(
-                        abs(min(max_allowed_time_ns, int(l)))
-                    ).strftime(self.date_format),
-                    unscaled,
-                )
-            )
-        else:
-            return list(
-                map(
-                    lambda l: pd.Timestamp(
-                        max(min(max_allowed_time_ns, int(l)), min_allowed_time_ns)
-                    ).strftime(self.date_format),
-                    unscaled,
-                )
+        return list(
+            map(
+                lambda l: pd.Timestamp(int(str(l)[:19])).strftime(self.date_format),
+                unscaled,
             )
+        )
 
     @lazy
     def input(self):
         return Input(
             shape=(self.input_dimension,), name="input_%s" % self.name, dtype="float64"
         )
 
@@ -725,7 +660,16 @@
             Exception("Decoder isn't created")
 
         low = self.weight_randomizer[0]
         high = self.weight_randomizer[1]
         random_weight = K.random_uniform_variable(shape=(1,), low=low, high=high)
 
         return random_weight * tf.keras.losses.MSE(self.input, self.decoder)
+
+
+class InverseTransformer:
+    def __init__(self, name, transformer):
+        self.name = check_name(name)
+        self.transformer = transformer
+
+    def transform(self, data):
+        return self.transformer(data)
```

### Comparing `syngen-0.0.89/src/syngen/ml/vae/models/model.py` & `syngen-0.0.9/src/syngen/ml/vae/models/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from pathlib import Path
+import re
 
 import tensorflow as tf
 from loguru import logger
 import pickle
+from pathlib import Path
 from tensorflow.keras.models import Model
 from tensorflow.keras.layers import (
     Input,
     Dense,
     Dropout,
     LeakyReLU,
     concatenate,
@@ -15,50 +16,54 @@
     Activation,
 )
 from sklearn.mixture import BayesianGaussianMixture
 import numpy as np
 import pandas as pd
 
 from syngen.ml.vae.models.custom_layers import FeatureLossLayer
-from syngen.ml.utils import slugify_parameters
+
+
+def check_name(name):
+    pattern = r"[^A-Za-z0-9_\\.]"
+    return re.sub(pattern, "_", name)
+
 
 class CVAE:
     """
     A class implementing the model architecture.
     """
 
     def __init__(
         self,
         dataset,
-        batch_size,
-        latent_dim,
-        intermediate_dim,
-        latent_components
+        batch_size=32,
+        latent_dim=40,
+        intermediate_dim=512,
+        latent_components=40,
+        keys_mode="ml",
+        cond_columns={},
+        is_cond=False,
     ):
         self.dataset = dataset
         self.intermediate_dim = intermediate_dim
         self.batch_size = batch_size
         self.latent_dim = latent_dim
         self.latent_components = min(latent_components, len(self.dataset.df))
         self.model = None
         self.latent_model = None
         self.metrics = {}
-        self.cond_features = {}
-        self.is_cond = False
+        self.keys_mode = keys_mode
+        self.cond_features = cond_columns
+        self.is_cond = is_cond
 
     def sample_z(self, args):
         mu, log_sigma = args
         eps = tf.random.normal(shape=(self.latent_dim,), mean=0.0, stddev=1.0)
         return mu + tf.exp(log_sigma / 2) * eps
 
-    @staticmethod
-    @slugify_parameters(exclude_params=("feature",))
-    def _create_feature_loss_layer(feature, name):
-        FeatureLossLayer(feature, name=name)
-
     def build_model(self):
         self.inputs = list()
         self.encoders = list()
         self.feature_decoders = list()
         self.loss_models = dict()
         self.cond_inputs = list()
 
@@ -95,15 +100,15 @@
             gen_inp_shape = self.latent_dim
             # decoder_input = Lambda(lambda x: x, name='decoder_inp')(embed_layer)
             # encoder_output = embed_layer
             decoder_input = z
             encoder_output = self.mu
 
         kl_loss = (
-            1
+            0.2
             * 0.5
             * tf.reduce_sum(
                 tf.exp(self.log_sigma) + self.mu ** 2 - 1.0 - self.log_sigma, 1
             )
         )
 
         generator_input = Input(shape=(gen_inp_shape,))
@@ -113,47 +118,51 @@
         )
 
         generator_outputs = list()
         feature_losses = list()
         for i, (name, feature) in enumerate(self.dataset.features.items()):
             feature_decoder = feature.create_decoder(self.global_decoder)
 
-            self._create_feature_loss_layer(feature=feature, name=name)
+            feature_layer = FeatureLossLayer(feature, name=check_name(name))
             feature_tensor = feature_decoder
             feature_losses.append(feature.loss)
 
             self.feature_decoders.append(feature_tensor)
 
             generator_outputs.append(feature.create_decoder(self.generator))
 
         self.model = Model(self.inputs, self.feature_decoders)
 
         self.model.add_loss(feature_losses)
-        self.model.add_loss(kl_loss * 0)
+        self.model.add_loss(kl_loss)
 
         self.encoder_model = Model(self.inputs, encoder_output)
 
         # generator
         self.generator_model = Model(generator_input, generator_outputs)
 
         return self.model
 
+    def __append_metric(self, name, tensor):
+        self.model.metrics.append(tensor)
+        self.model.metrics_names.append(check_name(name))
+
     def __build_encoder(self, input):
         h0 = Dense(self.intermediate_dim, name="Encoder_0")(input)
-        h0 = BatchNormalization(name="First_encoder_BN")(h0)
+        h0 = BatchNormalization()(h0)
         h0 = Activation(tf.nn.leaky_relu)(h0)
         h0 = Dropout(0.2)(h0)
 
         h1 = Dense(self.intermediate_dim, name="Encoder_1")(h0)
-        h1 = BatchNormalization(name="Second_encoder_BN")(h1)
+        h1 = BatchNormalization()(h1)
         h1 = Activation(tf.nn.leaky_relu)(h1)
         h1 = Dropout(0.2)(h1)
 
         h2 = Dense(self.intermediate_dim, name="Encoder_2")(h1)
-        h2 = BatchNormalization(name="Third_encoder_BN")(h2)
+        h2 = BatchNormalization()(h2)
         h2 = Activation(tf.nn.leaky_relu)(h2)
         h2 = Dropout(0.2)(h2)
 
         mu = Dense(self.latent_dim, name="mu")(h2)
         log_sigma = Dense(self.latent_dim, name="log_sigma")(h2)
         return mu, log_sigma
 
@@ -209,19 +218,17 @@
         return self.dataset.inverse_transform(prediction)
 
     def sample(self, nb_samples: int) -> pd.DataFrame:
         latent_sample = self.latent_model.sample(nb_samples)[0]
         np.random.shuffle(latent_sample)
 
         synthetic_prediction = self.generator_model.predict(latent_sample)
-        self.inverse_transformed_df = self.dataset.inverse_transform(synthetic_prediction)
-        pk_uq_keys_mapping = self.dataset.primary_keys_mapping
-        if pk_uq_keys_mapping:
-            self.__make_pk_uq_unique(pk_uq_keys_mapping)
-        return self.inverse_transformed_df
+        inverse_transformed_df = self.dataset.inverse_transform(synthetic_prediction)
+
+        return inverse_transformed_df
 
     def less_likely_sample(
         self, nb_samples: int, temp: float = 0.05, variaty: int = 3
     ) -> pd.DataFrame:
         def pop_npoints(latent_vector, log):
             log_probs = {prob: idx for idx, prob in enumerate(log)}
             sorted_log_probs_keys = np.sort(list(log_probs.keys()))
@@ -234,29 +241,14 @@
             latent_sample = self.latent_model.sample(nb_samples)[0]
             log_likelihoods = self.latent_model.score_samples(latent_sample)
             sliced_latent_sample.append(pop_npoints(latent_sample, log_likelihoods))
 
         synthetic_prediction = self.generator_model.predict(sliced_latent_sample)
         return self.dataset.inverse_transform(synthetic_prediction)
 
-    def __check_pk_numeric_convertability(self, column, key_type):
-        if key_type is str:
-            return self.inverse_transformed_df[column].dropna().str.isnumeric().all()
-        else:
-            return False
-
-    def __make_pk_uq_unique(self, pk_uq_keys_mapping):
-        for key_name, config in pk_uq_keys_mapping.items():
-            key_columns = config.get("columns")
-            for column in key_columns:
-                key_type = self.dataset.pk_uq_keys_types[column]
-                if key_type is float or self.__check_pk_numeric_convertability(column, key_type):
-                    mapped_keys = np.arange(len(self.inverse_transformed_df[column])) + 1
-                    self.inverse_transformed_df[column] = mapped_keys
-
     def show_model(self):
         from IPython.display import SVG
         from keras.utils.vis_utils import model_to_dot
         return SVG(model_to_dot(self.model).create(prog="dot", format="svg"))
 
     def save_state(self, path: str):
         pth = Path(path)
@@ -269,13 +261,14 @@
 
         if self.latent_model is not None:
             with open(str(pth / "latent_model.pkl"), "wb") as f:
                 f.write(pickle.dumps(self.latent_model))
 
     def load_state(self, path: str):
         pth = Path(path)
+
         self.model.load_weights(str(pth / "vae.ckpt"))
         self.generator_model.load_weights(str(pth / "vae_generator.ckpt"))
 
         with open(str(pth / "latent_model.pkl"), "rb") as f:
             self.latent_model = pickle.loads(f.read())
         return self
```

### Comparing `syngen-0.0.89/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.0.9/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,43 @@
-from typing import Tuple, List, Optional, Dict
+from typing import Tuple
 from abc import ABC, abstractmethod
-from collections import defaultdict
-from pathlib import Path
-
 import warnings
 import pickle
-import tensorflow as tf
 from tensorflow.python.data.experimental import AutoShardPolicy
 import matplotlib.pyplot as plt
 import time
 import tqdm
 from loguru import logger
-import pandas as pd
-import numpy as np
+from collections import defaultdict
+from pathlib import Path
 
+from syngen.ml.vae.models.features import *
 from syngen.ml.vae.models.model import CVAE
 from syngen.ml.vae.models import Dataset
-from syngen.ml.utils import fetch_dataset
 
 warnings.filterwarnings("ignore")
 
-BATCH_SIZE_DEFAULT = 32
-
 
 class BaseWrapper(ABC):
     """
     Abstract class for wrappers
     """
 
     def __init__(self):
         self.model = None
 
     @abstractmethod
     def fit_on_df(
         self,
         df: pd.DataFrame,
-        epochs: int,
-        columns_subset: List[str] = None
+        row_subset: List[int] = None,
+        columns_subset: List[str] = None,
+        batch_size: int = 10,
+        epochs: int = 30,
+        verbose: int = 0,
     ):
         pass
 
     @abstractmethod
     def predict_sampled_df(self, n: int) -> pd.DataFrame:
         pass
 
@@ -54,20 +51,17 @@
 
 
 class VAEWrapper(BaseWrapper):
     """Base class that implements end to end train and generation of structured data.
 
     Attributes
     ----------
-    df
-    schema
     metadata
-    table_name
     paths
-    process
+    keys_mode
     batch_size
     latent_dim
     latent_components
 
     Methods
     -------
     _pipeline()
@@ -78,141 +72,105 @@
 
     display_losses()
         show train losses curve by each feature
 
     predict_sampled_df(df, n)
         generate new data based on df that consist of n rows and return the result as pd.DataFrame
 
-    predict_less_likely_samples(df, n, temp=0.05, variety=3)
-        generate new data based on df that consist of n which has less probability
-        computed as log likelihood and return the result as pd.DataFrame
+    predict_less_likely_samples(df, n, temp=0.05, variaty=3)
+        generate new data based on df that consist of n which has less probablity
+        computed as log lokelihood and return the result as pd.DataFrame
     """
 
     def __init__(
         self,
-        df: pd.DataFrame,
-        schema: Optional[Dict],
         metadata: dict,
-        table_name: str,
         paths: dict,
-        process: str,
-        batch_size: int,
-        latent_dim: int = 10,
-        latent_components: int = 30,
+        keys_mode: bool = False,
+        batch_size: int = 100,
+        latent_dim: int = 40,
+        latent_components: int = 40,
     ):
-        super().__init__()
-        self.df = df
-        self.schema = schema
-        self.process = process
+        super(VAEWrapper, self).__init__()
         self.batch_size = batch_size
         self.latent_dim = latent_dim
         self.latent_components = latent_components
         self.metadata = metadata
-        self.table_name = table_name
+        self.keys_mode = keys_mode
         self.vae_resources_path = paths["state_path"]
         self.dataset_pickle_path = paths["dataset_pickle_path"]
-        self.fk_kde_path = paths["fk_kde_path"]
-
-    def __post__init(self):
-        if self.process == "train":
-            self.dataset = Dataset(
-                df=self.df,
-                schema=self.schema,
-                metadata=self.metadata,
-                table_name=self.table_name,
-                fk_kde_path=self.fk_kde_path
-            )
-        elif self.process == "infer":
-            self.dataset = fetch_dataset(self.dataset_pickle_path)
 
-    def _pipeline(self):
-        self.dataset.set_metadata()
+    def _pipeline(self, df, keys_mode):
+        self.dataset = Dataset(df, self.metadata, keys_mode)
         self.df = self.dataset.pipeline()
 
         with open(self.dataset_pickle_path, "wb") as f:
             f.write(pickle.dumps(self.dataset))
 
-    def _restore_zero_values(self, df):
-        for column in self.dataset.zero_num_column_names:
-            if column.endswith("_zero"):
-                # remove _zero to get original column name
-                num_column_name = column[:-5]
-                num_column = df[num_column_name].copy()
-                zero_column_mask = df[column].astype("float") >= 0.5
-                num_column = num_column.where(zero_column_mask, 0)
-                num_zero_values = (num_column == 0).sum()
-                df[num_column_name] = num_column
-                df = df.drop(column, axis=1)
-                logger.info(
-                    f"Column {column} has {num_zero_values} ({round(num_zero_values * 100 / len(num_column))}%) "
-                    f"zero values generated"
-                )
-        return df
-
     def _restore_nan_values(self, df):
-        for column in self.dataset.null_num_column_names:
+        for column in self.dataset.null_column_names:
             if column.endswith("_null"):
                 # remove _null to get original column name
                 num_column_name = column[:-5]
                 num_column = df[num_column_name].copy()
-                not_null_column_mask = df[column].astype("float64") <= 0.5
+                not_null_column_mask = df[column] <= 0.5
                 num_column = num_column.where(not_null_column_mask, np.nan)
                 df[num_column_name] = num_column
                 df = df.drop(column, axis=1)
-                num_nan_values = num_column.isna().sum()
-                logger.info(
-                    f"Column {column} has {num_nan_values} ({round(num_nan_values * 100 / len(num_column))}%) "
-                    f"empty values generated."
-                )
         return df
 
     def _restore_nan_labels(self, df):
         for column_name, nan_label in self.dataset.nan_labels_dict.items():
-            if nan_label is None:
-                nan_label = np.nan
-            df[column_name] = df[column_name].fillna(np.nan) if nan_label is None else df[column_name].fillna(nan_label)
+            df[column_name] = df[column_name].fillna(nan_label)
         return df
 
     @abstractmethod
     def _init_model(self):
         pass
 
     def fit_on_df(
         self,
         df: pd.DataFrame,
-        epochs: int,
+        row_subset: int = None,
         columns_subset: List[str] = None,  # TODO columns_subset does not work
+        batch_size: int = 32,
+        epochs: int = 30,
+        verbose: int = 0,
+        keys_mode: bool = False,
     ):
-        self.__post__init()
-        self._pipeline()
+        row_subset = row_subset or len(df)
+
+        self._pipeline(df, keys_mode)
         self._init_model()
 
+        # feature_names = ['mmd'] + [name.name for name in self.dataset.features.values()]
+
         if columns_subset is None:
             columns_subset = self.df.columns
         else:
             # if a column is in columns_subset, its null column should also be added if present
             columns_subset += [
                 col
                 for col in self.df.columns
-                if col.endswith(("_null", "_zero")) and (col[:-5] in columns_subset)
+                if col.endswith("_null") and (col[:-5] in columns_subset)
             ]
 
         df = self.df.loc[:, list(set(columns_subset))]
 
         train_dataset = self._create_batched_dataset(df)
         self.vae = self.model.model
 
         self.optimizer = self._create_optimizer()
         self.loss_metric = self._create_loss()
-        self._train(train_dataset, epochs)
+        self._train(train_dataset, row_subset, epochs)
 
         self.model.model = self.vae
         self.fit_sampler(df.dropna())
 
-    def _train(self, dataset, epochs: int):
+    def _train(self, dataset, row_subset, epochs: int):
         step = self._train_step
 
         self.feature_losses = defaultdict(list)
         loss_grows_num_epochs = 0
         prev_total_loss = float("inf")
         es_min_delta = 0.005
         es_patience = 10
@@ -244,17 +202,17 @@
                 self.vae.load_weights(str(pth / "vae_best_weights_tmp.ckpt"))
                 logger.info(
                     f"The loss does not become lower for {loss_grows_num_epochs} epochs in a row. Stopping the training."
                 )
                 break
             epoch += 1
 
-    # @staticmethod
-    def _create_optimizer(self):
-        learning_rate = 1e-04 * np.sqrt(self.batch_size / BATCH_SIZE_DEFAULT)
+    @staticmethod
+    def _create_optimizer():
+        learning_rate = 1e-03
         return tf.keras.optimizers.Adam(learning_rate=learning_rate)
 
     @staticmethod
     def _create_loss():
         return tf.keras.metrics.Mean()
 
     def _create_batched_dataset(self, df: pd.DataFrame):
@@ -269,15 +227,15 @@
             feature_datasets.append(dataset)
 
         dataset = tf.data.Dataset.zip(tuple(feature_datasets)).with_options(options)
         return dataset.batch(self.batch_size, drop_remainder=True)
 
     def _train_step(self, batch: Tuple[tf.Tensor]) -> tf.Tensor:
         with tf.GradientTape() as tape:
-            self.vae(batch)
+            reconstructed = self.vae(batch)
 
             # Compute reconstruction loss
             loss = sum(self.vae.losses)
 
         self.optimizer.minimize(
             loss=loss, var_list=[self.vae.trainable_weights], tape=tape
         )
@@ -294,16 +252,15 @@
 
     def fit_sampler(self, df: pd.DataFrame):
         self.model.fit_sampler(df)
 
     def predict_sampled_df(self, n: int) -> pd.DataFrame:
         sampled_df = self.model.sample(n)
         sampled_df = self._restore_nan_values(sampled_df)
-        sampled_df = self._restore_zero_values(sampled_df)
-        return sampled_df
+        return self._restore_nan_labels(sampled_df)
 
     def predict_less_likely_samples(
         self, df: pd.DataFrame, n: int, temp=0.05, variaty=3
     ):
         self.fit_sampler(df)
         return self.model.less_likely_sample(n, temp, variaty)
 
@@ -334,18 +291,17 @@
     Attributes
     ----------
     model : CVAE
         final model that we will use to generate new data
     """
 
     def _init_model(self):
-        latent_dim = min(self.latent_dim, int(len(self.dataset.columns) / 2))
-
         self.model = CVAE(
             self.dataset,
             batch_size=self.batch_size,
-            latent_dim=latent_dim,
-            latent_components=min(self.latent_components, latent_dim * 2),
+            latent_dim=self.latent_dim,
+            latent_components=self.latent_components,
             intermediate_dim=128,
+            keys_mode=self.keys_mode,
         )
 
         self.model.build_model()
```

### Comparing `syngen-0.0.89/src/syngen.egg-info/SOURCES.txt` & `syngen-0.0.9/src/syngen.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,46 @@
+CHAGELOG.txt
 DESCRIPTION
+LICENCE.txt
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+requirements.txt
 setup.cfg
 src/syngen/VERSION
 src/syngen/__init__.py
 src/syngen/infer.py
 src/syngen/train.py
 src/syngen.egg-info/PKG-INFO
 src/syngen.egg-info/SOURCES.txt
 src/syngen.egg-info/dependency_links.txt
 src/syngen.egg-info/entry_points.txt
 src/syngen.egg-info/requires.txt
 src/syngen.egg-info/top_level.txt
 src/syngen/ml/__init__.py
 src/syngen/ml/config/__init__.py
 src/syngen/ml/config/configurations.py
-src/syngen/ml/convertor/__init__.py
-src/syngen/ml/convertor/convertor.py
 src/syngen/ml/data_loaders/__init__.py
 src/syngen/ml/data_loaders/data_loaders.py
 src/syngen/ml/metrics/__init__.py
 src/syngen/ml/metrics/utils.py
 src/syngen/ml/metrics/accuracy_test/__init__.py
-src/syngen/ml/metrics/accuracy_test/accuracy_report.html
 src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
 src/syngen/ml/metrics/metrics_classes/__init__.py
 src/syngen/ml/metrics/metrics_classes/metrics.py
-src/syngen/ml/metrics/sample_test/__init__.py
-src/syngen/ml/metrics/sample_test/sample_report_template.html
-src/syngen/ml/metrics/sample_test/sample_test.py
+src/syngen/ml/pipeline/__init__.py
+src/syngen/ml/pipeline/pipeline.py
 src/syngen/ml/reporters/__init__.py
 src/syngen/ml/reporters/reporters.py
 src/syngen/ml/strategies/__init__.py
 src/syngen/ml/strategies/strategies.py
 src/syngen/ml/train_chain/__init__.py
 src/syngen/ml/train_chain/train_chain.py
-src/syngen/ml/utils/__init__.py
-src/syngen/ml/utils/utils.py
 src/syngen/ml/vae/__init__.py
 src/syngen/ml/vae/models/__init__.py
 src/syngen/ml/vae/models/custom_layers.py
 src/syngen/ml/vae/models/dataset.py
 src/syngen/ml/vae/models/features.py
 src/syngen/ml/vae/models/model.py
 src/syngen/ml/vae/wrappers/__init__.py
-src/syngen/ml/vae/wrappers/wrappers.py
-src/syngen/ml/validation_schema/__init__.py
-src/syngen/ml/validation_schema/validation_schema.py
-src/syngen/ml/worker/__init__.py
-src/syngen/ml/worker/worker.py
+src/syngen/ml/vae/wrappers/wrappers.py
```

