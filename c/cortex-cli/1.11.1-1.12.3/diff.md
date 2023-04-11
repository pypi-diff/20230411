# Comparing `tmp/cortex_cli-1.11.1.tar.gz` & `tmp/cortex_cli-1.12.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_cli-1.11.1.tar", last modified: Thu Apr  6 21:58:35 2023, max compression
+gzip compressed data, was "cortex_cli-1.12.3.tar", last modified: Tue Apr 11 16:16:30 2023, max compression
```

## Comparing `cortex_cli-1.11.1.tar` & `cortex_cli-1.12.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5185 2023-04-06 19:56:17.000000 cortex_cli-1.11.1/README.md
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/cortex_cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       22 2023-04-06 21:42:23.000000 cortex_cli-1.11.1/cortex_cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/cortex_cli/cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.11.1/cortex_cli/cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/cortex_cli/cli/api/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.11.1/cortex_cli/cli/api/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3990 2023-03-21 14:31:47.000000 cortex_cli-1.11.1/cortex_cli/cli/api/github_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.11.1/cortex_cli/cli/api/http_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.11.1/cortex_cli/cli/cli_api_base.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.11.1/cortex_cli/cli/cli_api_base_config.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.11.1/cortex_cli/cli/clients.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      821 2023-04-04 00:22:55.000000 cortex_cli-1.11.1/cortex_cli/cli/configure.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      971 2023-03-16 20:39:49.000000 cortex_cli-1.11.1/cortex_cli/cli/cortex_cli.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.11.1/cortex_cli/cli/generic_get.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.11.1/cortex_cli/cli/inferences.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    22292 2023-04-06 21:58:30.000000 cortex_cli-1.11.1/cortex_cli/cli/models.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3248 2023-04-06 21:20:24.000000 cortex_cli-1.11.1/cortex_cli/cli/pipelines.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/cortex_cli/core/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.11.1/cortex_cli/core/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4024 2023-03-16 20:39:49.000000 cortex_cli-1.11.1/cortex_cli/core/cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.11.1/cortex_cli/core/drift_checks.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    10969 2023-03-09 15:57:05.000000 cortex_cli-1.11.1/cortex_cli/core/ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/cortex_cli/core/mlflow/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.11.1/cortex_cli/core/mlflow/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.11.1/cortex_cli/core/mlflow/mlflow_cortex.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/cortex_cli/core/models/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.11.1/cortex_cli/core/models/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     7010 2023-03-21 15:45:49.000000 cortex_cli-1.11.1/cortex_cli/core/models/cortex_model.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/cortex_cli/ml_model_template/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-03-21 14:31:47.000000 cortex_cli-1.11.1/cortex_cli/ml_model_template/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-03-21 14:31:47.000000 cortex_cli-1.11.1/cortex_cli/ml_model_template/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.11.1/cortex_cli/ml_model_template/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      346 2023-04-06 21:44:35.000000 cortex_cli-1.11.1/cortex_cli/ml_model_template/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-03-21 14:31:47.000000 cortex_cli-1.11.1/cortex_cli/ml_model_template/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-03-21 14:31:47.000000 cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1602 2023-03-21 14:31:47.000000 cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      164 2023-04-06 21:45:02.000000 cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      533 2023-04-06 19:56:03.000000 cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-06 19:56:06.000000 cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/cortex_cli/tests/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.11.1/cortex_cli/tests/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.11.1/cortex_cli/tests/test_cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.11.1/cortex_cli/tests/test_ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/cortex_cli.egg-info/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-06 21:58:35.000000 cortex_cli-1.11.1/cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1909 2023-04-06 21:58:35.000000 cortex_cli-1.11.1/cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-04-06 21:58:35.000000 cortex_cli-1.11.1/cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-04-06 21:58:35.000000 cortex_cli-1.11.1/cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-04-06 21:58:35.000000 cortex_cli-1.11.1/cortex_cli.egg-info/requires.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-04-06 21:58:35.000000 cortex_cli-1.11.1/cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.11.1/pyproject.toml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      206 2023-04-06 21:58:35.083259 cortex_cli-1.11.1/setup.cfg
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      841 2023-04-06 21:41:11.000000 cortex_cli-1.11.1/setup.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5185 2023-04-06 19:56:17.000000 cortex_cli-1.12.3/README.md
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       22 2023-04-07 17:57:53.000000 cortex_cli-1.12.3/cortex_cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.12.3/cortex_cli/cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/cli/api/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/cli/api/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3990 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/cli/api/github_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/cli/api/http_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.12.3/cortex_cli/cli/cli_api_base.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.12.3/cortex_cli/cli/cli_api_base_config.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/cli/clients.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      880 2023-04-07 17:56:26.000000 cortex_cli-1.12.3/cortex_cli/cli/configure.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      971 2023-03-16 20:39:49.000000 cortex_cli-1.12.3/cortex_cli/cli/cortex_cli.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.12.3/cortex_cli/cli/generic_get.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/cli/inferences.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    22303 2023-04-07 20:22:18.000000 cortex_cli-1.12.3/cortex_cli/cli/models.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3248 2023-04-07 17:56:26.000000 cortex_cli-1.12.3/cortex_cli/cli/pipelines.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/core/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/core/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4124 2023-04-11 16:15:11.000000 cortex_cli-1.12.3/cortex_cli/core/cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/core/drift_checks.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    10969 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/core/ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/core/mlflow/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/core/mlflow/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/core/mlflow/mlflow_cortex.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/core/models/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/core/models/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     7010 2023-03-21 15:45:49.000000 cortex_cli-1.12.3/cortex_cli/core/models/cortex_model.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/ml_model_template/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      346 2023-04-07 17:56:26.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1602 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      164 2023-04-07 17:56:26.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      533 2023-04-06 19:56:03.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-06 19:56:06.000000 cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli/tests/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/tests/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/tests/test_cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.12.3/cortex_cli/tests/test_ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/cortex_cli.egg-info/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-11 16:16:30.000000 cortex_cli-1.12.3/cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1909 2023-04-11 16:16:30.000000 cortex_cli-1.12.3/cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-04-11 16:16:30.000000 cortex_cli-1.12.3/cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-04-11 16:16:30.000000 cortex_cli-1.12.3/cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-04-11 16:16:30.000000 cortex_cli-1.12.3/cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-04-11 16:16:30.000000 cortex_cli-1.12.3/cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.12.3/pyproject.toml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      206 2023-04-11 16:16:30.810097 cortex_cli-1.12.3/setup.cfg
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1053 2023-04-07 18:01:54.000000 cortex_cli-1.12.3/setup.py
```

### Comparing `cortex_cli-1.11.1/README.md` & `cortex_cli-1.12.3/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/cli/api/github_api.py` & `cortex_cli-1.12.3/cortex_cli/cli/api/github_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/cli/api/http_api.py` & `cortex_cli-1.12.3/cortex_cli/cli/api/http_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/cli/cli_api_base.py` & `cortex_cli-1.12.3/cortex_cli/cli/cli_api_base.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/cli/cli_api_base_config.py` & `cortex_cli-1.12.3/cortex_cli/cli/cli_api_base_config.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/cli/configure.py` & `cortex_cli-1.12.3/cortex_cli/cli/configure.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,9 +17,10 @@
 
         config[profile] = {
             'api_url': api_url,
             'api_key': api_key
         }
 
         path = os.path.expanduser('~/.nearlyhuman/config')
+        os.makedirs(os.path.dirname(path), exist_ok=True)
         with open(path, 'w') as file:
             config.write(file)
```

### Comparing `cortex_cli-1.11.1/cortex_cli/cli/cortex_cli.py` & `cortex_cli-1.12.3/cortex_cli/cli/cortex_cli.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/cli/generic_get.py` & `cortex_cli-1.12.3/cortex_cli/cli/generic_get.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/cli/inferences.py` & `cortex_cli-1.12.3/cortex_cli/cli/inferences.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/cli/models.py` & `cortex_cli-1.12.3/cortex_cli/cli/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,23 +164,24 @@
             except Exception as e:
                 raise Exception(f'An error occurred while initializing the GitHub repo.\n{e}')
 
 
     def _register_model(self):
         if self._register:
             response = requests.post(
-                url=self.endpoint,
-                headers=self.headers,
+                url=self._endpoint,
+                headers=self._headers,
                 json={
                     'name': self._name,
                     'repo': self._repo
                 }
             )
+
             self._handle_api_response(
-                response, f'Registered the model repository {response["_id"]}')
+                response, f'Registered the model repository {response.json()["_id"]}')
 
 
 @ModelsCli.subcommand('register')
 class RegisterModel(CliApiBase):
     _repo = plumbum.cli.SwitchAttr(
         names=['-r', '--repo'],
         argtype=str,
```

### Comparing `cortex_cli-1.11.1/cortex_cli/cli/pipelines.py` & `cortex_cli-1.12.3/cortex_cli/cli/pipelines.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/core/cortex_data.py` & `cortex_cli-1.12.3/cortex_cli/core/cortex_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     def load(self):
         try:
             with open(self.local_path, 'rb') as file:
                 if self.type in ['xls', 'xlsx', 'xlsm', 'xlsb', 'odf', 'ods', 'odt']:
                     self._loaded_data = pd.read_excel(file)
                 if self.type=='csv':
                     self._loaded_data = pd.read_csv(file)
+                if self.type=='parquet':
+                    self._loaded_data = pd.read_parquet(file)
                 if self.type=='pkl':
                     self._loaded_data = pickle.load(file)
                 if self.type=='json':
                     self._loaded_data = json.load(file)
                 if self.type=='yml':
                     self._loaded_data = yaml.load(file)
                 return self._loaded_data
@@ -81,15 +83,15 @@
         self._local_dir = local_dir
 
         self._files = self._list_remote_files()
 
 
     def _list_remote_files(self):
         response = requests.get(
-            f'{self._api_url}/models/{self._model_id}/files/list',
+            f'{self._api_url}/models/{self._model_id}/files',
             headers=self._headers
         ).json()
 
         return [CortexFile(self._local_dir, file['Key'], file['Size'], file['ETag'], file['LastModified'])
                 for file in response]
```

### Comparing `cortex_cli-1.11.1/cortex_cli/core/drift_checks.py` & `cortex_cli-1.12.3/cortex_cli/core/drift_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/core/ethics_checks.py` & `cortex_cli-1.12.3/cortex_cli/core/ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/core/mlflow/mlflow_cortex.py` & `cortex_cli-1.12.3/cortex_cli/core/mlflow/mlflow_cortex.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/core/models/cortex_model.py` & `cortex_cli-1.12.3/cortex_cli/core/models/cortex_model.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/ml_model_template/.gitignore` & `cortex_cli-1.12.3/cortex_cli/ml_model_template/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/ml_model_template/README.md` & `cortex_cli-1.12.3/cortex_cli/ml_model_template/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/.gitignore` & `cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/README.md` & `cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/cortex.yml` & `cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/cortex.yml`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.12.3/cortex_cli/ml_model_template/{{cookiecutter.__model_slug}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/tests/test_cortex_data.py` & `cortex_cli-1.12.3/cortex_cli/tests/test_cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli/tests/test_ethics_checks.py` & `cortex_cli-1.12.3/cortex_cli/tests/test_ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/cortex_cli.egg-info/SOURCES.txt` & `cortex_cli-1.12.3/cortex_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.11.1/setup.py` & `cortex_cli-1.12.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 from setuptools import find_packages, setup
 
+# Setup custom import schema
+# cortex_cli.cli
+# cortex_cli.core
+import os
+import sys
+current = os.path.dirname(os.path.realpath(__file__))
+sys.path.append(current)
+
+from cortex_cli import __version__
 
 setup(
     name="cortex_cli",
-    version="1.11.1",
+    version=__version__,
     packages=find_packages(exclude=['tests*']),
     author='Nearly Human',
     author_email='support@nearlyhuman.ai',
     description='Nearly Human Cortex CLI for interacting with model functions.',
     keywords='CLI, API, nearlyhuman, nearly human, cortex',
 
     python_requires='>=3.8.10',
```

